# yet-another-arabic-romanization

## Goals
- correctness of pronunciation by uninitiated readers
    - usage of closest english sounds, e.g. `th` for ث and `sh` for ش
- enable uninitiated readers to separate words from each other
- complete control over resulting text in arabic script
- legibility and aesthetics
    - only lower-case letters
    - separation of repeated letters by `-`, e.g. `kath-thar` vs. `kaththar`


| Letter      | Unicode     | Name            | yaar        |
|-------------|-------------|-----------------|-------------|
| ؟           | 0x061f      | 'istifhhaam     | ?           |
|             | 0x0620      |                 |             |
| ء           | 0x0621      | hhamza          | '           |
| آ           | 0x0622      |                 | 'aa         |
| أ           | 0x0623      |                 | '           |
| ؤ           | 0x0624      |                 | '           |
| إ           | 0x0625      |                 | '           |
| ئ           | 0x0626      |                 | '           |
| ا           | 0x0627      | 'alif           | aa          |
| ب           | 0x0628      | baa'            | b           |
| ة           | 0x0629      | taa' marbuuttah | ah, aht     |
| ت           | 0x062a      | taa'            | t           |
| ث           | 0x062b      | thaa'           | th          |
| ج           | 0x062c      | jiim            | j           |
| ح           | 0x062d      | ~haa'           | ~h          |
| خ           | 0x062e      | khaa'           | kh          |
| د           | 0x062f      | daal            | d           |
| ذ           | 0x0630      | dhaal           | dh          |
| ر           | 0x0631      | raa'            | r           |
| ز           | 0x0632      | zayn            | z           |
| س           | 0x0633      | siin            | s           |
| ش           | 0x0634      | shiin           | sh          |
| ص           | 0x0635      | ssaad           | ss          |
| ض           | 0x0636      | ddaad           | dd          |
| ط           | 0x0637      | ttaa'           | tt          |
| ظ           | 0x0638      | zhaa'           | zh          |
| ع           | 0x0639      | ~ayn            | ~           |
| غ           | 0x063a      | ghayn           | gh          |
| ف           | 0x0641      | faa'            | f           |
| ق           | 0x0642      | qaaf            | q           |
| ك           | 0x0643      | kaaf            | k           |
| ل           | 0x0644      | laam            | l           |
| م           | 0x0645      | miin            | m           |
| ن           | 0x0646      | nuun            | n           |
| ه           | 0x0647      | hhaa'           | hh          |
| و           | 0x0648      | waaw            | w, uu       |
| ى           | 0x0649      | 'alif maqssuurah| aah         |
| ي           | 0x064a      | yaa'            | y, ii       |
| ٠           | 0x0660      | sifr            | 0           |
| ١           | 0x0661      | waa~hid         | 1           |
| ٢           | 0x0662      | 'ithnaan        | 2           |
| ٣           | 0x0663      | thalaathah      | 3           |
| ٤           | 0x0664      | 'arba~ah        | 4           |
| ٥           | 0x0665      | khamsah         | 5           |
| ٦           | 0x0666      | sit-tah         | 6           |
| ٧           | 0x0667      | sab~ah          | 7           |
| ٨           | 0x0668      | thamaaniyah     | 8           |
| ٩           | 0x0669      | tis~ah          | 9           |
| ٪           | 0x066a      | bi almi'ah      | %           |
|             |             |                 |             |

- fatha, kasra, damma: a, i, u
- tanwiin: ann, inn, unn
- special:
    - al at-ta~riif: alqamar, ash-shams
    - shad-dA: `<letter>-<letter>`


## version with only one letter per arabic letter

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
| ع           | 0x0639      | ~ayn           | ~           |
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
