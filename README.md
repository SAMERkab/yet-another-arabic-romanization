# Yet Another Arabic Romanization

## Goals
- correctness of pronunciation by uninitiated readers
    - usage of closest english sounds, e.g. `th` for ث and `sh` for ش
- enable uninitiated readers to separate words from each other
- complete control over resulting text in arabic script
- legibility and aesthetics
    - only lower-case latin alphabet letters
    - optional separation of repeated letters by `-`, e.g. `kath-thar` vs. `kaththar`

## Letters

| Letter      | Unicode     | Name            | yaar        |
|-------------|-------------|-----------------|-------------|
| ؟           | 0x061f      | -istifhhaam     | ?           |
|             | 0x0620      |                 |             |
| ء           | 0x0621      | hhamza          | -           |
| آ           | 0x0622      |                 | -aa         |
| أ           | 0x0623      |                 | -           |
| ؤ           | 0x0624      |                 | -           |
| إ           | 0x0625      |                 | -           |
| ئ           | 0x0626      |                 | -           |
| ا           | 0x0627      | alif            | aa          |
| ب           | 0x0628      | baa-            | b           |
| ة           | 0x0629      | taa- marbuutdah | ah, aht     |
| ت           | 0x062a      | taa-            | t           |
| ث           | 0x062b      | thaa-           | th          |
| ج           | 0x062c      | jiim            | j           |
| ح           | 0x062d      | -haa-           | -h          |
| خ           | 0x062e      | khaa-           | kh          |
| د           | 0x062f      | daal            | d           |
| ذ           | 0x0630      | dhaal           | dh          |
| ر           | 0x0631      | raa-            | r           |
| ز           | 0x0632      | zayn            | z           |
| س           | 0x0633      | siin            | s           |
| ش           | 0x0634      | shiin           | sh          |
| ص           | 0x0635      | szaad           | sz          |
| ض           | 0x0636      | dzaad           | dz          |
| ط           | 0x0637      | tdaa-           | td          |
| ظ           | 0x0638      | zhaa-           | zh          |
| ع           | 0x0639      | _ayn            | _           |
| غ           | 0x063a      | ghayn           | gh          |
| ف           | 0x0641      | faa-            | f           |
| ق           | 0x0642      | qaaf            | q           |
| ك           | 0x0643      | kaaf            | k           |
| ل           | 0x0644      | laam            | l           |
| م           | 0x0645      | miin            | m           |
| ن           | 0x0646      | nuun            | n           |
| ه           | 0x0647      | hhaa-           | hh          |
| و           | 0x0648      | waaw            | w, uu       |
| ى           | 0x0649      | alif maqssuurah | aah         |
| ي           | 0x064a      | yaa-            | y, ii       |
| ٠           | 0x0660      | sifr            | 0           |
| ١           | 0x0661      | waa_hid         | 1           |
| ٢           | 0x0662      | ithnaan         | 2           |
| ٣           | 0x0663      | thalaathah      | 3           |
| ٤           | 0x0664      | arba_ah         | 4           |
| ٥           | 0x0665      | khamsah         | 5           |
| ٦           | 0x0666      | sit-tah         | 6           |
| ٧           | 0x0667      | sab_ah          | 7           |
| ٨           | 0x0668      | thamaaniyah     | 8           |
| ٩           | 0x0669      | tis_ah          | 9           |
| ٪           | 0x066a      | bi almi-ah      | %           |
|             |             |                 |             |

## Special

- `fat-hah`, `kasrah`, `dammah`: `a`, `i`, `u`
- `tanwiin`: `ann`, `inn`, `unn`
- `laamu t ta_riif`:
    - `al laamu l qamariyyah`: `al qamar`, `ra-aytu l qamar`
    - `al laamu sh shamsiyyah`: `ash shams`, `ra-aytu sh shamsa`
- `shaddah`: `<letter><letter>`, `<letter>-<letter>`

## Sample Text
```
bukaa-ukumaa yashfii wa in kaana laa yujdii         fa juudaa fa qad awdaah nazhiirukumaa _indii
bunayya l ladhii ahhdathhu kaffaaya li th tharaah   fa yaa _izzahta l muhhdaah wa yaa hhasratahta l mahhdii
alaa qaatala llaahhu l manaayaa wa ramyahhaa        mina l qawmi habbaati l quluubi _alaah _amdi
tawakh-khaah himaamu l mawti awsatda szibyatii      fa li llaahhi kaifa khtaara waasitdahta l _iqdi
_alaah hiini shumtu l khaira min lama-haatihhi      wa aanastu min af_aalihhi aayahta r rushdi
tdawaahhu r radaah _annii fa adz-haah mazaaruhhu    ba_iidann _alaah qurbinn qariibann _alaah bu_di
laqad anjazat fihhi l manaayaa wa_iidahaa           wa akhlafati l aamaalu maa kaana min wa_di
laqad qalla bayna l mahhdi wa l la-hdi lubthuhhu    fa lam yansa _ahhda l mahhdi idh dzumma fi l lahhdi
tanagh-ghasza qabla r riyyi maa-u hayaatihhi        wa fujji_a minhhu bi l _udhuubahti wa l bardi
ala-h-ha _alayhhi n nazfu hattaah a-haalahhu        ilaah szufrahti l jaadiyyi _an humrahti l wardi
wa zhalla _alaah l aydii tasaaqatdu nafsuhhu        wa yadhwii ka maa yadhwii l qadziibu mina r randi
fa yaalaki min nafsinn tasaaqatdu anfusann          tasaaqutda durrinn min nizhaaminn bilaa _iqdi
_ajibtu li qalbii kaifa lam yanfatdir lahhu         wa law annahhu aqsaah mina l hajari sz szaldi
bi wudddiya annii kuntu quddimtu qablahhu           wa anna l manaayaa duunahhu szamadat szamdi
wa laakinna rabbii shaa-a ghaira mashii-atii        wa li r rabbi imdzaa-u l mashii-ahti la l _abdi
wa maa sarranii an bi_tuhhu bi thawaabihhi          wa law annahhu t takhliidu fi jannahti l khuldi
wa laa bi_tuhhu tdaw_ann wa laakin ghuszibtuhhu     wa laysa _alaah zhulmi l hawaadithi min mu_di
```

## Ideas
- switch dz and dh?
- dash instead of apostrophe for hamza
- dash at beginning of words is ommited
- underscore instead of tilde for `_ayn`

## Problems
- when a dash is omitted from a shadda, the letters become ambiguous because of ss, tt and dd.

## Version with Only One Letter per Arabic Letter

| Letter      | Unicode     | Name           | yaar        |
|-------------|-------------|----------------|-------------|
| ء           | 0x0621      | hamza          | '           |
| ا           | 0x0627      | 'alif          | A           |
| ب           | 0x0628      | baa'           | b           |
| ة           | 0x0629      | taa' marbuutah | e           |
| ت           | 0x062a      | taa'           | t           |
| ث           | 0x062b      | thaa'          | S           |
| ج           | 0x062c      | jeem           | j           |
| ح           | 0x062d      | hhaa'          | H           |
| خ           | 0x062e      | KHaa'          | x           |
| د           | 0x062f      | daal           | d           |
| ذ           | 0x0630      | THaal          | Z           |
| ر           | 0x0631      | raa'           | r           |
| ز           | 0x0632      | zayn           | z           |
| س           | 0x0633      | siin           | s           |
| ش           | 0x0634      | chiin          | $           |
| ص           | 0x0635      | Saad           | c           |
| ض           | 0x0636      | Daad           | D           |
| ط           | 0x0637      | Taa'           | T           |
| ظ           | 0x0638      | dhaa'          | C           |
| ع           | 0x0639      | _ayn           | _           |
| غ           | 0x063a      | ghayn          | g           |
| ف           | 0x0641      | faa'           | f           |
| ق           | 0x0642      | qaaf           | q           |
| ك           | 0x0643      | kaaf           | k           |
| ل           | 0x0644      | laam           | l           |
| م           | 0x0645      | miin           | m           |
| ن           | 0x0646      | nuun           | n           |
| ه           | 0x0647      | haa'           | h           |
| و           | 0x0648      | waaw           | w U         |
| ي           | 0x064a      | yaa'           | y I         |
|             |             |                |             |

- fatha, kasra, damma: a, i, u
