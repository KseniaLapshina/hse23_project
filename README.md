# hse23_project

Целью работы над проектом является изучение методами сравнительной геномики ранней эволюции белков, выполняющих эпигенетические модификации H3K4me и взаимодействующих с ними в клетках человека.

## Подготовка
Презентация группы находится в папке data.

Линейная последовательность нуклеотидов ДНК является основной формой хранения и передачи генетической информации, однако в реализации генетиеской программы существенную роль играют взаимодействия ДНК с белками и ковалентных модификаций хроматина. В ядрах эукариотических организмов ДНК находится в комплексе с гистонами, оборачиваясь вокруг октамера из двух гистонов каждого из типов H2A, H2B, H3 и H4. N-концевой хвост каждого гистона выступают за изгибы ДНК и является субстратом для множества ковалентных модификаций, включая метилирование, ацетилирование, фосфорилирование, убиквитинирование, АДФ-рибозилирование, биотинилирование. [Eissenberg, Shilatifard, 2010; Luger et al., 1997]

Наша группа работает с эпигенетической модификацией метилирования четвёртого лизина гистона H3.

Метилирование лизина в гистонах может влиять на конформацию, гидрофобность или сродство к ДНК, так в исследовании 2008 года было показано, что метилирование H4 по лизину 20 увеличивает способность нуклеосомных массивов сворачиваться и конденсироваться, однако в том же году было продемонстрировано, что метилирование лизина может создавать сайт связывания для белков, которые могут изменять локальные свойства хроматина для транскрипции. [Eissenberg, Shilatifard, 2010; Fischle et al., 2008; Honda et al., 1975; Kouzarides, 2007; Lu et al., 2008]

Метка метилирования H3K4 связана с активной транскрипцией. Диметилирование H3K4 связано с активными и потенциально активными генами, в то время как триметилирование H3K4 в первую очередь является меткой, связанной с сайтом начала транскрипции. [Bernstein et al., 2002; Eissenberg, Shilatifard, 2010; Krogan et al., 2003; Ng et al., 2003]

Среди выбранных нами для работы белков есть 3 функциональных группы: Histone modification write (KMT2A (MLL1), MLL2 (KMT2D)), Histone modification read (AIRE, ING4, RAG2, TAF3, WDR5, ZCWPW1, CCDC101) и Histone modification erase (PHF8).

#### KMT2A Lysine methyltransferase 2A
"Белки гистон-лизин-метилтрансферазы 2 (KMT2) образуют мультимерные ферментативные комплексы, которые метилируют лизин 4 на гистоне H3 (H3K4) в элементах регуляции транскрипции в геноме." [Park et al., 2020] "KMT2A (MLL1) отвечает за создание моно-, ди- и триметилированного H3K4 посредством домена SET и взаимодействия с кофакторами." [Vallianatos, Iwase, 2015] "Из множества белков PHD (plant homeodomain) пальцев только PHD3 KMT2A семейства KMT2 проявляет свойства связывания H3K4." [Bochynska et al., 2018]
#### MLL2 Myeloid/lymphoid or Mixed-lineage leukemia 2
"Здесь мы показываем, что Mll2, одна из шести метилтрансфераз H3K4 типа Set1/Trithorax у млекопитающих, необходима для триметилирования бивалентных промоторов в эмбриональных стволовых клетках мышей." [Denissov et al., 2014]
#### AIRE Autoimmune regulator
"... AIRE избирательно взаимодействует с гистоном H3 через свой первый палец гомеодомена растений (PHD) (AIRE-PHD1) и преимущественно связывается с неметилированным H3K4 (H3K4me0)... AIRE-PHD1 является важным членом недавно идентифицированного класса PHD пальцы, которые специфически распознают H3K4me0…" [Org et al., 2008] "Некоторые посттрансляционные модификации хвостов H3, особенно диметилирование или триметилирование в H3K4, отменяли связывание Aire, в то время как другие допускались." [Koh et al., 2008]
#### ING4 Inhibitor of growth family member 4
"Полноразмерный ING4 распознает метилированные пептиды H3K4, но производное ING4 без пальца PHD, ING4ΔPHD (aa 1–194), этого не делает, демонстрируя, что палец PHD ING4 необходим и достаточен для активности связывания пептида H3K4me ING4." [Hung et al., 2009]
#### RAG2 Recombination activating gene 2
"RAG2 содержит растительный гомеодомен (PHD) вблизи своего C-конца (RAG2-PHD), который распознает гистон H3, метилированный по лизину 4 (H3K4me), и влияет на рекомбинацию V(D)J. Два аспекта RAG2-PHD уникальны. Во-первых, в отсутствие модифицированного пептида пептид, N-концевой по отношению к RAG2-PHD, занимает сайт связывания субстрата, что может отражать механизм ауторегуляции. Во-вторых, в отличие от других доменов PHD, связывающих H3K4me3, RAG2-PHD заменяет карбоксилат, который взаимодействует с аргинином 2 (R2), на тирозин, что приводит к связыванию с H3K4me3, которое усиливается, а не ингибируется диметилированием аргинина 2." [Ramón-Maiques et al., 2007]
#### TAF3 TATA-box binding protein associated factor 3
"TAF3 способствует распознаванию и селективности промотора и действует как антиапоптотический фактор." "Дальнейшие анализы показывают, что H3K4me3 усиливает р53-зависимую транскрипцию, стимулируя образование комплекса преинициации (PIC); (…) Взаимодействия H3K4me3-TAF3/TFIID регулируют геноселективные функции p53 в ответ на генотоксический стресс." [Lauberth et al., 2013]
#### WDR5 WD repeat domain 5
"Здесь мы показываем, что … белок WDR5 с повторами WD40 напрямую связывается с ди- и триметилированным по K4 гистоном H3 и с H3-K4-диметилированными нуклеосомами. WDR5 необходим для связывания метилтрансферазного комплекса с K4-диметилированным хвостом H3, а также для глобального триметилирования H3K4…" [Wysocka et al., 2005]
#### ZCWPW1 Zinc finger CW-type and PWWP domain containing 1
"Здесь мы демонстрируем, что Zcwpw1 является считывателем H3K4me3, который необходим для DSB (double-strand break) репарации и синапсов в семенниках мышей." [Huang et al., 2020]
#### CCDC101

#### PHF8 PHD finger protein 8
"Белок PHD пальцев 8 (PHF8) принадлежит к семейству белков, содержащих домен JmJc, которые могут удалять метильные группы с остатков аргинина или лизина (…) идентифицированные считыватели H3K4me3 Sgf29, TRRAP, PHF8 (…)" [Vermeulen, et al., 2010] "PHF8 ассоциирован с гипометилированными генами рРНК" [Feng, et al., 2010]

#### Комплексы
Белок KMT2A входит в комплексы MLL-HCF, CHD8, COMPASS-like MLL1,2. Белок MLL2 входит в комплексы Set1/COMPASS,SWI/SNF (BAF),NuA4 (Tip60-p400) ,MLL2.

Белки AIRE, RAG2 и ZCWPW1 в комплексы не входят. Белок ING4 входит в комплекс HBO1. Белок TAF3 входит в комплекс TFIID. Белок WDR5 входит в комплексы ATAC, NSL, RING2-L3MBTL2, MLL1/2, MLL3/4.

Белок PHF8 входит в комплекс PHF8-TOPBP1.

#### Экспрессия в тканях
Белок KMT2A экспрессируется в головном мозге (мозжечке, полушариях мозжечка), яичнике, артериях (большеберцовой и аорте), большеберцовом нерве.
Белок MLL2 экспрессируется в костном мозге, коже, селезенке, семенниках.

Белок AIRE экспрессируется в мозге по GTEx и лимфатическом узле и тимусе по NCBI.
Белок ING4 экспрессируется в полушариях мозжечка, мозжечке, щитовидной железе, эндоцервиксе, эктоцервиксе и матке.
Белок RAG2 экспрессируется в почти только в щитовидной железе, но также понемногу в семенниках и костном мозге [ncbi]. По GTEx, есть на минимальном уровне везде, но в ощутимых размерах в щитовидной железе и немного в семенниках.
Белок TAF3 экспрессируется в артериях, мозге и полушариях мозжечка.
Белок WDR5 экспрессируется в семенниках, полушариях мозжечка, мозжечке.
Белок ZCWPW1 экспрессируется в семенниках.

Белок PHF8 экспрессируется в семенниках, яичнике, матке.

#### Доменная структура
В белке KMT2A наблюдаются домены SET_KMT2A_2B, ePHD_KMT2A, Bromo_ALL-1, PHD3_KMT2A, PHD1_KMT2A, FYRC, PHD2_KMT2A, zf-CXXC, FYRN.
В белке MLL2 наблюдаются домены SET_KMT2D, ePHD2_KMT2D, HMG-box KMT2D, ePHD1_KMT2D, PHD5_KMT2D, PHD3_KMT2D, FYRC, PHD5_KMT2C_like, PHD_SF super family, PHD1_KMT2C_like, FYRN, PHA03247 super family (4). Общие: FYRC, FYRN.

В белке AIRE наблюдаются домены PHA03247 super family (2), PHD_SF super family (2), HSR super family (2), SAND super family, PRK12323 super family.
В белке ING4 наблюдаются домены ING_ING4, TNG2 super family.
В белке RAG2 наблюдаются домены RAG2 super family, PHD_SF super family.
В белке TAF3 наблюдаются домены PHD_TAF3, BTP, PTZ00449 super family, PRK12323 super family.
В белке WDR5 наблюдаются домены WD40 super family (2), CaiC super family, PHA03247 super family.
В белке ZCWPW1 наблюдаются домены PWWP super family(3), zf-CW super family.

В белке PHF8 наблюдаются домены JHD, PHD_PHF8, cupin_RmlC, JmjC.

## Индивидуальная часть
AIRE: https://github.com/KseniaLapshina/hse23_project_AIRE

KMT2A:

RAG2:

PHF8:

ING4:

ZCWPW1:

MLL2:

TAF3:

WDR5:

CCDC101:

## Групповая часть
Презентация группы, таблица с -log(E-value) и код, использованный для построения тепловой карты, находятся в папке data.

## Литература
1. Bernstein, Bradley E., et al. "Methylation of histone H3 Lys 4 in coding regions of active genes." Proceedings of the National Academy of Sciences 99.13 (2002): 8695-8700.
2. Bochynska, Agnieszka, Juliane Lüscher-Firzlaff, and Bernhard Lüscher. "Modes of interaction of KMT2 histone H3 lysine 4 methyltransferase/COMPASS complexes with chromatin." Cells 7.3 (2018): 17.
3. Denissov, Sergei, et al. "Mll2 is required for H3K4 trimethylation on bivalent promoters in embryonic stem cells, whereas Mll1 is redundant." Development 141.3 (2014): 526-537.
4. Eissenberg, Joel C., and Ali Shilatifard. "Histone H3 lysine 4 (H3K4) methylation in development and differentiation." Developmental biology 339.2 (2010): 240-249.
5. Feng, Weijun, et al. "PHF8 activates transcription of rRNA genes through H3K4me3 binding and H3K9me1/2 demethylation." Nature structural & molecular biology 17.4 (2010): 445-450.
6. Fischle, Wolfgang, et al. "Specificity of the chromodomain Y chromosome family of chromodomains for lysine-methylated ARK (S/T) motifs." Journal of Biological Chemistry 283.28 (2008): 19626-19635.
7. Honda, B. M., P. M. Candido, and G. H. Dixon. "Histone methylation. Its occurrence in different cell types and relation to histone H4 metabolism in developing trout testis." Journal of Biological Chemistry 250.22 (1975): 8686-8689.
8. Huang, Tao, et al. "The histone modification reader ZCWPW1 links histone methylation to PRDM9-induced double-strand break repair." Elife 9 (2020): e53459.
9. Hung, Tiffany, et al. "ING4 mediates crosstalk between histone H3 K4 trimethylation and H3 acetylation to attenuate cellular transformation." Molecular cell 33.2 (2009): 248-256.
10. Koh, Andrew S., et al. "Aire employs a histone-binding module to mediate immunological tolerance, linking chromatin regulation with organ-specific autoimmunity." Proceedings of the National Academy of Sciences 105.41 (2008): 15878-15883.
11. Kouzarides, Tony. "Chromatin modifications and their function." Cell 128.4 (2007): 693-705.
12. Krogan, Nevan J., et al. "The Paf1 complex is required for histone H3 methylation by COMPASS and Dot1p: linking transcriptional elongation to histone methylation." Molecular cell 11.3 (2003): 721-729.
13. Lauberth, Shannon M., et al. "H3K4me3 interactions with TAF3 regulate preinitiation complex assembly and selective gene activation." Cell 152.5 (2013): 1021-1036.
14. Lu, Xu, et al. "The effect of H3K79 dimethylation and H4K20 trimethylation on nucleosome and chromatin structure." Nature structural & molecular biology 15.10 (2008): 1122-1124.
15. Luger, Karolin, et al. "Crystal structure of the nucleosome core particle at 2.8 Å resolution." Nature 389.6648 (1997): 251-260.
16. Ng, Huck Hui, et al. "Targeted recruitment of Set1 histone methylase by elongating Pol II provides a localized mark and memory of recent transcriptional activity." Molecular cell 11.3 (2003): 709-719.
17. Org, Tonis, et al. "The autoimmune regulator PHD finger binds to non‐methylated histone H3K4 to activate gene expression." EMBO reports 9.4 (2008): 370-376.
18. Park, Kihyun, Jung-Ae Kim, and Jaehoon Kim. "Transcriptional regulation by the KMT2 histone H3K4 methyltransferases." Biochimica et Biophysica Acta (BBA)-Gene Regulatory Mechanisms 1863.7 (2020): 194545.
19. Ramón-Maiques, Santiago, et al. "The plant homeodomain finger of RAG2 recognizes histone H3 methylated at both lysine-4 and arginine-2." Proceedings of the National Academy of Sciences 104.48 (2007): 18993-18998.
20. Vallianatos, Christina N., and Shigeki Iwase. "Disrupted intricacy of histone H3K4 methylation in neurodevelopmental disorders." Epigenomics 7.3 (2015): 503-519.
21. Vermeulen, Michiel, et al. "Quantitative interaction proteomics and genome-wide profiling of epigenetic histone marks and their readers." Cell 142.6 (2010): 967-980.
22. Wysocka, Joanna, et al. "WDR5 associates with histone H3 methylated at K4 and is essential for H3 K4 methylation and vertebrate development." Cell 121.6 (2005): 859-872.
