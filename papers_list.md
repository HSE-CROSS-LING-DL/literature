Список статей к изучению
* https://arxiv.org/pdf/1804.07875.pdf

* https://arxiv.org/pdf/1910.10893.pdf

* https://www.aclweb.org/anthology/D19-1076.pdf

* https://www.aclweb.org/anthology/E17-1088.pdf (2017) *[Влад]*

* https://arxiv.org/pdf/1902.00508v1.pdf (2019) *[Влад]*

* https://openreview.net/pdf?id=r1xCMyBtPS (2019) *[Олег?]*

* https://www.aclweb.org/anthology/K18-2024.pdf

* https://www.mitpressjournals.org/doi/abs/10.1162/tacl_a_00288 (2019) *[Олег]*
единый BiLSTM энкодер с BPE для всех языков, 
как-то присобачен декодер, 
обучение языковой модели на параллельных данных, 
но обучать классификатор над ней потом можно используя только данные для одного языка 
(как? 
наверное, на основании факта того, что вывод энкодера для всех языков одинаковый по смыслу, 
что-то в духе аттеншна. 
но это я не читал ещё).

* https://www.aclweb.org/anthology/W19-4222 (2019) *[Олег]*
**малоресурсные!** **полисинтетические!** 
unsupervised approaches for morphological segmentation of low-resource polysynthetic languages based on Adaptor Grammars (что это?)

* https://arxiv.org/abs/1908.05838 (2019)
**attention** **low-resource** **морфология**! *[Олег]* вроде огонь и будет на EMNLP.
Also, we identify the crucial factors for success with cross-lingual transfer for morphological inflection: typological similarity and a common representation across languages.

* https://arxiv.org/abs/1802.05368 (2018) 
трансфер лёрнинг и для both эмбеддингов слов и эмбеддингов предложений. тоже вроде шарят энкодеры (в sentence-level) как-то. есть **какой-то zero-shot** вариант

* https://www.aclweb.org/anthology/E17-1088/ (2017) *[Олег]*
кейс настоящего low-resource, использует параллельные словари для получения aligned эмбеддингов. 
Похоже на [MUSE](https://github.com/facebookresearch/MUSE), интересно тем, что **репорт поведения на боевой задаче**.

* https://arxiv.org/abs/1604.02201 (2016) *[Олег]*
использование высокоресурсных по-одному, малоресурсных по-другому (<-- **это круто!**) (какой-то трансфер-лёрнинк) чтобы улучшить перевод в малоресурсных
говорят, получилось норм

* https://arxiv.org/abs/1907.10129 (2019)
Сигморфон 2019, CRF, трансфер лёрнинг, чот надо вникать

* https://arxiv.org/abs/1707.06961 (2017)
учат отображение из пр-ва поверхностных форм в пространство заранее обученных эмбеддингов чтобы deal with low-resource

* https://arxiv.org/abs/1606.0940 (2016)
CBOW с билингвальным словарём сводит переводы в близкие друг к другу векторы. 
классная идея, но подозрительно простой w2v.

* https://www.aclweb.org/anthology/P15-2139/ (2015)
учатся делать синтаксис, используя меньше данных для достижения competitive результата.
в абстракте темнят, подробностей не раскрывают.

* https://arxiv.org/abs/1706.09031 (2017)
репорт с сигморфона 2017

* https://dspace.mit.edu/handle/1721.1/110739 (2016)
translation pairs to establish a linear mapping between monolingual embeddings. 
We further refine the model in an unsupervised manner by initializing and regularizing it to be close to the direct transfer model. 
ИМХО **скучно**.
Вроде то же самое лучше сделали через 2 года в [MUSE](https://github.com/facebookresearch/MUSE).

