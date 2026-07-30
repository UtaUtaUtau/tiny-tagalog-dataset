# tiny-tagalog-dataset
A public Tagalog singing dataset with a masculine voice

# Licensing
 This repository includes multiple licences, but the gist of it is the following:

 - Repository contents are licensed under the MIT License. See [LICENSE](./LICENSE ) for details.
 - The datasets that are accessible through the [releases](https://github.com/UtaUtaUtau/tiny-tagalog-dataset/releases) are licensed under CC BY-NC 4.0. See [LICENSE-DATASET](./LICENSE-DATASET) for details. By downloading the datasets, you are agreeing to abide by this license.

# FAQ
### Does this mean I can't use the dataset commercially?
No. Non-commercial for Creative Commons only makes non-commercial usage its default. You can ask me for permission to use the dataset commercially.

### What does the repository contain then?
It contains supporting files specifically for [OpenUtau](https://github.com/stakira/OpenUtau). The .dll is a phonemizer that can be installed by putting it in the Plugins folder, and dsdict-fil.yaml contains the replacements table for this phonemizer. The glottal stop phoneme in this case is `q` instead of `cl`.

# Dataset Information
## Phoneme System
 This phoneme system follows a phoneme system mostly based on Tagalog orthography. The phonemes are as follows:
 ### Vowels
 | Phoneset | X-SAMPA |
 | -------- | ------- |
 | a        | a       |
 | e        | e       |
 | i        | i       |
 | o        | o       |
 | u        | u       |
 ### Consonants
 | Phoneset | X-SAMPA |
 | -------- | ------- |
 | b        | b       |
 | d        | d       |
 | dy       | dZ      |
 | g        | g       |
 | h        | h       |
 | k        | k       |
 | l        | l       |
 | m        | m       |
 | n        | n       |
 | ng       | N       |
 | p        | p       |
 | r        | 4       |
 | s        | s       |
 | sy       | S       |
 | t        | t       |
 | ty       | tS      |
 | w        | w       |
 | W        | w (coda)|
 | y        | j       |
 | Y        | j (coda)|
 | cl       | ?       |

 Other phonemes included are as follows:
 | Phoneme |   Description   |
 | ------- | --------------- |
 | SP      | Pure silence    |
 | AP      | Breathing       |
 | exh     | Breathy release |
 | vf      | Vocal fry       |

## Processing
 This dataset was not recorded in a professional environment, but I tried my best to keep them as good as possible. The audio was also put through a compressor to roughly equalize its dynamics. To compensate for the improper environment, the dataset has been denoised and dereverbed by [PixPrucer](https://youtube.com/@PixPrucer). Long silences were cut-out automatically after. It is then saved in 44.1kHz 16-bit wavs.

 The tools used for each process is the following:
 - Recording - Audacity/REAPER
 - Compressor - [LALA by Analog Obsession](https://www.patreon.com/analogobsession/posts/lala-36128829)
 - Denoise - [melband-roformer-denoise](https://huggingface.co/poiqazwsx/melband-roformer-denoise)
 - Dereverb - [dereverb_bs_roformer](https://huggingface.co/anvuew/dereverb_bs_roformer)

 ## Labeling
 Base labels were generated using SOFA. All of the labels were then corrected by hand.

# Song List
|   Filename   |                     Song                      |
| ------------ | --------------------------------------------- |
| TGL_core_001 | Kitchie Nadal - Huwag Na Huwag Mong Sasabihin |
| TGL_core_002 | MYMP - Kailan                                 |
| TGL_core_003 | MYMP - Kailan                                 |
| TGL_core_004 | Eraserheads - Spoliarium                      |
| TGL_core_005 | Eraserheads - Spoliarium                      |
| TGL_core_006 | IV of Spades - Mundo                          |
| TGL_core_007 | IV of Spades - Mundo                          |
| TGL_core_008 | IV of Spades - Mundo                          |
| TGL_core_009 | Moonstar88 - Torete                           |
| TGL_core_010 | Up Dharma Down - Tadhana                      |
| TGL_core_011 | Up Dharma Down - Tadhana                      |
| TGL_core_012 | Moonstar88 - Migraine                         |
| TGL_core_013 | Maldita - Porque                              |
| TGL_core_014 | Up Dharma Down - OO                           |
| TGL_core_015 | Paramita - Hiling                             |
| TGL_core_016 | Paramita - Hiling                             |
| TGL_core_017 | Paramita - Hiling                             |
| TGL_core_018 | Aneka Abarrientos - Bakit ('Pag Pinahiwatig)  |
| TGL_core_019 | Zack Tabudlo - Habang Buhay                   |

