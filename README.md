![](https://img.shields.io/github/v/release/nurtdinovadf/open_adt?include_prereleases&style=for-the-badge) [![Mailing list : test](http://img.shields.io/badge/Email-gray.svg?style=for-the-badge&logo=gmail)](mailto:nurtdinovadf@gmail.com) [![Mailing list : test](http://img.shields.io/badge/Telegram-blue.svg?style=for-the-badge&logo=telegram)](https://t.me/yara_tchk)


[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

# **Open ADT (Automatic Drum Transcription) Dataset**

- ~100 000 synthetically generated loops using **real drum tabs** and drum samples (~250 hrs total).
- Loops are 1-15 seconds length.

![image](https://user-images.githubusercontent.com/12515311/94298663-2f67b580-ff6f-11ea-8ebd-fd72fb857199.png)

# **Downloads**

Available on [Academic Torrents](https://academictorrents.com/details/9c920dd59f83241124b1e2c345db31f3a2edcd31)

# **Using opus**

Please refer to [Open STT opus helpers](https://github.com/snakers4/open_stt/blob/master/README.md#how-to-open-opus)

# **Annotation format**

Each loop is annotated as a list of combined strokes. Each combined stroke has a unique ID, and each instrument (or single stroke, or note) has its own unique ID. The `DOUBLE` stroke simply means repeat the previous stroke.
```
strokes = {
 1: 'Kick',
 2: 'Snare',
 3: 'Tom',
 4: 'Cymbal',
 5: 'Tambourine',
 6: 'Cowbell',
 -4: 'DOUBLE',
 -3: 'OTHER',
 -5: 'PAD',
 0: 'BLANK'}
 
combstrokes = {
 1: (1, 4),
 2: (1,),
 3: (4,),
 4: (2, 4),
 5: (2,),
 6: (3,),
 7: (1, 2, 4),
 8: (1, 3),
 9: (1, 2),
 10: (3, 4),
 11: (5,),
 12: (1, 3, 4),
 13: (2, 3),
 14: (1, 2, 3),
 ...
}
```

# **Further work**

- Eliminating some known issues like abrupt hit endings.
- More detailed anotations.
- Finding more samples. Please contact me in case you can give advice on this or share some sources.

# **License**

![сс-nc-by-license](https://static.wixstatic.com/media/342407_05e016f9f44240429203c35dfc8df63b~mv2.png/v1/fill/w_563,h_200,al_c,lg_1,q_80/342407_05e016f9f44240429203c35dfc8df63b~mv2.webp)

CC-BY-NC and commercial usage available after agreement with dataset authors.

# **Authors and contacts**

[Diliara Nurtdinova](https://entombed.space/contacts/)
