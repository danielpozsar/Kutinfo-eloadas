# Kutatómunka információs eszközei előadás
Homework:
Digital image processing / Képfeldolgozási eljárások

Amiről beszéltem:





2. dia:
1960: Bell laborok, Jet Propulsion Laboratory, MIT műhold felvételek: javítás helyreállítás tömörítés
Space Detector Ranger 7 in 1964: több ezer kép geometriai korrekció, zajszűrés hold feltérképezése
komplexebb eljárás több százezer kép hold domborzata holdraszállás megalapozása

1972 angolok CT(több szögben röntgen áteresztés, keresztmetszet helyreállítása)
1975 teljes testre
1979 Nobel díj

korábban sok erőforrás, 1970es évek MOS processzorok valós időben dolgoznak pl. tv közvetítő rendszerek nemzetek közti sugárzás a 2000es évekre gyors gépek és jelprocesszorok olcsó elterjedt sokoldalú
digital signal processor digitális jelfeldolgozás architektúra

analóg áramkörök




3. dia:
Mintavételezés (rácspontokban): folytonos képből diszkrét mennyiségek 

Kvantálás (intenzitások reprezentálása): amplitúdó nagyság diszkretizálása 
képsík meghatározott pontjaiban mintákat veszünk a képjelből színek intenzitás
Analóg-digitális átalakító áramkör:folytonos kvantált (I, V egy szám)

világosságkód nem-negatív egész szám és értéke a gyakorlatban 0 <= q <= 255
mintavételezési frekvencia

jelfeldolgozás formája 2 dimenziós mátrixok vagy több szín (3db 2Ds mátrix)
analóg képfeldolgozással szemben: algoritmusok nagyobb variációja , komplexebb





4. dia:
zajok véletlenszerű külső forrás
determinisztikus torzulás:árnyékolás, életlenség

gauss zaj: normális eloszlású sűrűségfüggvény
elektromos zaj(erősítők, érzékelők)
só és bors zaj: max fekete-fehér pixelek
poissonzaj: shot noise
elektromágneses sugárzás statisztikai jellege
ismétlődő zaj




5. dia:
szintaxis magyarázat





6. dia:
Mindennapi használat
Alacsony szint egyenletes műveletek:
fókusz
körbevágás
filterek
motion blur
kontraszt





7. dia:
Közép szint: összetett műveletek
sok módszer előnyök és hátrányok
LoG operátor:
Élek ott lehetnek, ahol a második derivált értéke nulla és a környezetében előjelet vált.
derivált képzés: adott irány  tetszőleges irányú él:kellően nagy számú irányban amelyik a legnagyobb értéket adta.
Viszont minden irányban egyformán érzékeny, nem szükséges külön X, Y kernel.
Rendkívül zajérzékeny, előzetes simítás erősen javasolt!





8. dia:
Parciális derivált közelítése konvolúciós maszkkal. X-irányú élekre érzékeny. Figyeljük meg, hogy a vizsgált képpont jobb oldali szomszédainak súlyozott összegéből vonjuk ki a bal oldaliak súlyozott összegét.
nem végez előjelváltás keresést, csak a Laplace eredmény abszolútértékét képzi, ami elrontja az élkeresési lehetőséget.

szintaxis magyarázat





9. dia:
Magas szint: felismerés
deep learning
alakfelismerés
számítógépes látás
maxpooling tömörebb reprezentáció





10. dia:
klasszifikáció
önvezető autó elengedhetetlen része

crowdsourcing: vissza az alapokhoz
maxar: 2019 sept 1 Bahamák
eddigi legerősebb ottani vihar
nagyfelbontású műholdképek 
1óra és 12 perc alatt 3009 épület elemzése

motion capture:  military, entertainment, sports
fényvisszaverő jelzők
mozgás követés, oscar díj





11. dia:
jó:
fekete lyuk
chirp az adatok összekapcsolására

rossz:
kína arcfelismerés
szociális pontozási rendszer
telefonszolgáltatóknak kell arckép 





12. dia:
források:
https://en.wikipedia.org/wiki/Digital_image_processing#History
https://regi.tankonyvtar.hu/hu/tartalom/tamop412A/2011-0063_15_gepi_latas/ch02.html
https://en.wikipedia.org/wiki/MOSFET
http://www.inf.u-szeged.hu/~tanacs/pyocv/
https://gyires.inf.unideb.hu/KMITT/c01/ch03s02.html
https://patbaa.github.io/physdl/
https://blog.maxar.com/earth-intelligence/2019/in-the-wake-of-dorian-maxars-geohive-damage-assessment-and-the-state-of-the-bahamas?utm_source=maxar.com-use-cases&utm_medium=website
https://medium.com/image-vision/noise-in-digital-image-processing-55357c9fab71
https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53
https://www.unite.ai/what-is-computer-vision/
http://www.asianews.it/news-en/Beijing,-facial-recognition-to-buy-a-SIM-card-48696.html
https://techcrunch.com/2019/04/10/the-creation-of-the-algorithm-that-made-the-first-black-hole-image-possible-was-led-by-mit-grad-student-katie-bouman/
