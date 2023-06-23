 # Diagnosztikai célú orvosi képalkotás

>
> ***Államvizsgás tárgy!***
> ## ZV tételek a tárgyból:
> - [Röntgen](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#r%C3%B6ntgen-rtg)
> - [CT](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#computer-tomogr%C3%A1fia-ct)
> - [OCT](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#oct)
> - [MRI](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#mri)
> - [PET](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#pet)
> - [spektroszkopia](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#vispektroszk%C3%B3piaspektrometria)
> - [CTI](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#viicti---computerised-thermal-imaging)
> - [NIRS](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#viiinirs---near-infrared-spectroscopy)
> - [UH](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#ultrahang)
> - [kép ábrázolás](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#optika-mikroszk%C3%B3pia)
> - [nagyfelbontású mikroszkópia I](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#nagyfelbont%C3%A1s%C3%BA-f%C3%A9nymikroszk%C3%B3pia-i)
> - [nagyfelbontású mikroszkópia II](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#nagyfelbont%C3%A1s%C3%BA-f%C3%A9nymikroszk%C3%B3pia-ii)
> - Digitális mikroszkópia

- 2 zh
- 1 féléves feladat
--------

## GY-EA1
> **cél:**
>
> *A képalkotás egyszerű dolog*


A [top 500 szuperszámítógép](https://www.top500.org) amik önálló hálózatok.

- **diagnosztika:** a betegség felismerésének és megállapításának tudománya. A `pácieens tünetei` + `kiegészítő szakvizsgálatok` 1 tünet <> sok lehetséges kórok
- **diagnózis:** a kórisme a betegség felismerése és meghatározása
- **terápia:** a betgeségek kzeleésével/gyógy ításával fogallakozó tudományág. A terápa gyógyítás során az alkalmazott eljárások összessége

**Orvosi diagnózis:**
- a lehetséges betegség meghatározásának folyamata (diagnosztikus eljárás)
- a vélemény/másod vélmeény ami  ennek a folyamatnak az eredményeként kialakul, a probléma kategorizálása és orvosi döntés a terápiára, a prognózisok definiálása
  - hagyományos kínai orvoslás: szemügyre vétel, meghallgatás, megszagolás, kikérdezés, pulzus

**vizsgálatok:**
- fizikális
- műszeres
- laboratóriumi
- képalkotó

>
> ***Occam borotvája:  ha van több magyarázat egy adot dologra akkor válaszd az egyszerűbbet!***
>

**makroszkopikus mérettartomány:**
- nukleráis medicina
  - Rtg - röntgen

**adattárolás:**
- szabványok: DICOM
- infrastrukturák: PACS
- jogszabályok: tárolással kapcsolatban

### 2D kép, hagyományos képen
- kép elemi egysége a filmen levő kisebb-nagyobb méretű ezüstalapú/színezék - szemcse véletlenszerű, de jó lefedettségű
- színtér: színes/fekete fehér
- három alap színnel mait maxwell kitalált

digitális képen:
- digitek/kvantált számjegyek írják le
- 2d kép elemi egyésge a pixel
- felbontás: kép méret (szélességx hosszúság pixelben)
- színmélység bitben mérve
- színtér (RGB, CMYK, HSV, HSL)
- fájlformátumok

### 3D képeken
- elemi egysége: voxel
- térrész homogén 3 tengelyű kiterjedéssel rendlekezik, egyszínű


beadndóhoz:

- https://docplayer.net/amp/208626422-Context-recognition-by-wireless-sensing-a-comprehensive-survey.html
- https://sci-hub.se/https://doi.org/10.1145/3328918
- https://news.ncsu.edu/2019/08/wifi-to-track-indoor-odometry/

## EA-GY2
### Röntgen (Rtg)
Egyéb források röntgen téren: 
- https://medlineplus.gov/xrays.html
- https://www.mayoclinic.org/tests-procedures/x-ray/about/pac-20395303
- https://tech.snmjournals.org/content/32/3/139
Egyéb források röntgencső téren:
- https://www.britannica.com/technology/X-ray-tube
- https://radiopaedia.org/articles/x-ray-tube-1
- http://www.elektroncso.hu/cikkek/xray.php
- https://medicalimaginghelp.blog.hu/2019/09/12/rontgencso_i

Nagyon korán feltalálása után megkezdték használatát. *([[1]](https://www.kumc.edu/school-of-medicine/academics/departments/history-and-philosophy-of-medicine/archives/wwi/base-hospital-28/clinical-services/radiology.html) [[2]](https://en.wikipedia.org/wiki/X-ray#History))* Kifejleszétse nem csak Röntgen, de Lénárd Fülöphöz is köthető.

Gyors összefoglalás: [NIBIB gov - How Do X-rays Work? ](https://www.youtube.com/watch?v=hTz_rGP4v9Y)

#### Alapelv
A röntgen hullámok a test nagy részén áthatolnak, de vannak olyan részek amik a röntgenhullámot elnyelik vagy megtörik. Ilyen a kalcium is.

![röntgen spektrumok](https://www.biolegend.com/Files/Images/BioLegend/blog/100814blog/Spectrum.png)

Egy sugarat kilövünk és azt mérjük, hogy hogyan csapódik be az atomokba és ott hogy törik meg, milyen "árnyékot" ad, a külféle spektrumokat könfélre finomságon használjuk.

Két vezetéket használva ha az egyikbe nagy feszültséget kötünk akkor átvándorol a másikra, így mikor ezt bekapcsolva hagyta Röntgen, és azt próbálva jutott arra, hogy az anyagoknak van sugárzási együtthatója.

> A `kilépő sugárintenzitás = belépő sugárzás * anyag sugárzási együtthatója ^ (sugárgyengítési együttható * anyag_vastagság)` 

[How does an X-ray Tube Work (Radiation Protection)](http://www.youtube.com/watch?v=Bc0eOjWkxpU)

A kollimátor használatótól függően meg tudjuk változtatni a sugárnyaláb méretét és kiterjedését is 

| ![tipikus röntgen szögek anód esetén](https://www.mta-r.de/site/assets/files/9355/fig_5_6.png) | ![https://tech.snmjournals.org/content/32/3/139](https://tech.snmjournals.org/content/jnmt/32/3/139/F3.large.jpg) |
| --- | ---- |

Ahol van szövet ott kisebb színintenzitással megy át, ahol nincs ott nagyobbal. Ahol, áthalad ott a szövetek elnyelik a sugárzást, a fenti képlet értékében, így az elnyelés végső mértéke összegződik az árnyék képen. Ez a szummációs felvétel. Éppen ezért használható pl csontritkulás megállapítására is. [*- medlineplus -*](https://medlineplus.gov/lab-tests/bone-density-scan/) De pont ezért számít a felvétel készítésének iránya is! Rosszul állítjuk be nem látszik a törés pl, mert  pont fedésben van a törött rész.

| ![the five main daiodensities ona standard radiograph](https://veteriankey.com/wp-content/uploads/2016/05/B9781455703647000053_f005-002-9781455703647.jpg) | ![electric and magnetic waves are perpendicular](https://tech.snmjournals.org/content/jnmt/32/3/139/F1.medium.gif) |
| --- | --- | 

Éppen ezért, néhány röntgenvizsgálathoz kontrasztanyag használata is szükséges lehet, melyet intravénásan, belélegezve vagy nyeléssel juttatnak a páciens szervezetébe. A kontrasztanyag általában valamilyen jódtartalmú vegyület, mely a röntgenfelvételen jól kirajzolja az általa elfoglalt teret a testben. A kontrasztanyagos vizsgálat előtt fontos tájékoztatni a szakembereket a kontrasztanyaggal szembeni allergiáról, illetve fennálló vesebetegségről.

Az infra fény áthatol a szöveten.

**felhasználása:**
- Mammography
- X-ray radiography
- Fluoroscopy (kontrasztos)
- Radiation therapy in cancer treatment

> A röntgen legegyszerűbb előállítási formája a [röntgencső](http://oftankonyv.reak.bme.hu/tiki-index.php?page=R%C3%B6ntgencs%C5%91&structure=Book+for+fisics&no_bl=y). 
> 
> Egy röntgencső a legegyszerűbb kivitelnél egy katódból és egy anódból áll, amik egy üvegburában vannak légmentesen lezárva. Vákuum azért szükséges mert ha  túl gyakori az ütközés, akkor már nem fognak tudni az elektronok megfelelő sebességre jutni ahhoz, hogy röntgensugárzás jöjjön létre. 
> 
> A katód a negatív pólus. Itt alakul ki az elektronfelhő, hő hatására. Az elektronfelhőből elindulnak az elektronok a nagyfeszültség megegyőző ereje miatt az anód felé. A katódszerkezet állítja megfelelő irányba az elektron sokaságot = az anód megfelelő részére. A katód egy wolfram tekercs. A tekercs/szál hossza és átmérője befolyásolja a készült kép minőségét!
> 
> ![bővebben: https://medicalimaginghelp.blog.hu/2019/09/12/rontgencso_i](https://m.blog.hu/me/medicalimaginghelp/image/crt_rontgencsoaa.gif)
> 
> A katódszál elektromos ellenállása miatt hő fejlődik. Emiatt pedig elektronfelhő jön létre. Hozzávetőlegesen 2200 ºC felett jelentkezik a termoionikus hatás a wolframszálban. Emiatt az elektronok elhagyják a katódot, majd nagyfeszültség hatására elindulnak az anód felé. Az anódba csapódva legnagyobb részük visszatér az áramkörbe.
> 
> Első kísérleti kisülési csöveinél az X-sugárzás keletkezési helyén a katóddal szembeni üvegfalon zöld fluoreszcens fényjelenség megfigyelhető. 
> 



#### kiértékelése, felhasználása
- https://youtu.be/3Ok6wIiu0zk
- a 2D röntgen kép tükrözött
- látszanak rajta a légbuborékok is
- törések, ficamok, sérülések, gyulladások, elváltozások vizsgálatához (például: mellkasröntgen, fogászati röntgen, mammográfia). 
- https://egeszsegvonal.gov.hu/r/714-rontgenvizsgalat.html?

## Computer tomográfia (CT)
- http://www.impactscan.org/#ctdose
- https://egeszsegvonal.gov.hu/c-cs/648-ct-vizsgalat.html
- http://oftankonyv.reak.bme.hu/tiki-index.php?page=Vizsg%C3%A1l%C3%B3elj%C3%A1r%C3%A1sok+klinikai+jelent%C5%91s%C3%A9ge+-+Computer+Tomographia
- http://itl7.elte.hu/hlabdb/tomo/tomo.html
- https://howradiologyworks.com/ct/

> gyakorlatilag röntgen
> 
> **használható:**
> - MRI-vel
> - PET-tel

Radon találta ki 1917-ben

Egy testet `n` irányból lövünk meg röntgen sugárral ami `n` db egyenletet és `n-1` ismeretlent jelent a mi esetünkben tehát a feladat megoldható.

<img src="https://ars.els-cdn.com/content/image/1-s2.0-B9780444534859000015-f01-01-9780444534859.jpg" width=50% height=50%><img src="https://prod-images-static.radiopaedia.org/images/52608436/ffb5a7e3ebb12255dec689e924ddbd_jumbo.jpeg" width=50% height=50%>

Kiszámolod az adott térrész sugárgyengítési értékét és azt hozzárendelem egy szürke képhez.

[Tomográfiák](https://hu.wikipedia.org/wiki/Orvosi_k%C3%A9palkot%C3%A1s#Tomogr%C3%A1fia): 
- lineáris tomográfia 
  - ez a tomográfia legalapvetőbb formája
  - *A páciens felett A pontból B pontba mozog a röntgensugarakat kibocsátó cső, míg a röntgenfilmet tartalmazó másik egység a páciens alatt mozog szimultán módon B pontból A-ba. Az alátámasztási pont vagy forgáspont az érdeklődésünknek megfelelő területhez van beállítva. Ily módon a gyújtóponti sík felett és alatt lévő pontok elmosódottak, akárcsak akkor, amikor a kamera pásztázásakor a háttér elmosódik.* ***EZ NEM CT***
- poli tomográfia 
  - geometriks mozgásokkal képalkotás
  - *ez egy bonyolultabb formája volt a tomográfiának. Ezzel a technikával képesek voltak számos geometrikus mozgást programozni, mint például a ciklikus, a 8-as alakzatú vagy az elliptikus mozgást.* ***EZ SEM CT***
- zonográfia 
  - ez a lineáris tomográfia változata
  - *Ez a lineáris tomográfia egy változata, ahol a mozgás egy meghatározott ívét használják. Ezt az eljárást még mindig alkalmazzák néhány helyen, hogy láthatóvá tegyék a vesét egy intravénás urogram közben* ***EZ SEM CT***

A tomogramm egy sugárgyengítési együtthatóval csinál egy képet, a sok képből létrehoz egy 3D objektumot szeletenként.

A 3D képhez minden 2D képen keresünk közös beazonosítható közös pontot, hogy térbeli koordinátát nyerjünk.

Röntgennél a röntgencsőből a sugárkapun keresztül lépnek ki a sugarak ahol tudjuk változtatni a sugár irányát és nagyságát.
- oszcintillációs: a detektort ért sugarak felvillanásokat okoznak a fotodetektorral ezt érzékelik. Jellemzői a mechanikai stabilitás, kis méret, alacsony tápfeszültség, modulárisan cserélhető.
- ionizációs detektorok:
  - nemesgáz töltés esetén az ionizált gáz áramot gerjeszt és a keletkező jelenséget rögzíthetjük.

**alkotó részei:**
- adatgyűjtő rendszer: analóg jeleket jelerősítéssel mintavételt alkalmazok
- páciens asztal: stabil és ~1mm pontosságú
- nagyfeszültségű generátor: 12-140 kV, 80-400mA, 50-60kW háromfázisú
- vezérlőpult
- számítógép ami menti az adatokat és összeállíŧja a képet

### Röntgen vs CT
- https://www.hopkinsmedicine.org/health/treatment-tests-and-therapies/ct-vs-mri-vs-xray

| röntgen       | CT           |
| ------------- |-------------|
|     |rosszabb térbeli felbontás, lényegesen jobb kontrasztfelbontás |
| 2D | 3D |
| csont törés kimutatása, csontritkulás | vérrögök, törések, szervi károsodások | 
| gyorsabb | lassabb mint a röntgen de még mindig elégy gyors, hogy sürgősségi eljáráshoz használják |
| - | nagyobb sugárterhelés mivel több kép készül |

Képminőség:
- fantomokkal mérhető, hogy jól van-e bekalibrálva, térbeli speciális fantommal mérik
- vonalpár/cm
- függ:
  - a detektor méretétől
  - a páciens méretétől, mert változik a fókuszpont

#### CT generációk
![https://howradiologyworks.com/ctgenerations/](https://cdn.shortpixel.ai/spai/w_800+q_lossy+ret_img+to_webp/https://howradiologyworks.com/wp-content/uploads/2020/06/GenerationsOfCTScanning.jpg)

> minőségi vizsonyokról ad visszacsatolást

>**1. gen CT**
>
> - csak két párhuzamos röntgen detektor, végigszkennelte, arrépp ment
> - a legelső demonál a beteg forgott, nem a gép körülötte
> - lassú volt
> - csak fej scan
> 
> <img src="http://www.impactscan.org/slides/impactcourse/basic_principles_of_ct/img24.gif" width=50% height=50% ><img src="https://cdn.shortpixel.ai/spai/w_1200+q_lossy+ret_img+to_webp/https://howradiologyworks.com/wp-content/uploads/2019/07/ct_gen_first_gen_bench-1.gif
" width=50% height=50% alt="https://howradiologyworks.com/ctgenerations/">
> 

> **2. gen CT**
> 
> - 30 detektor, 600 sugár x 540 négyzet, 18 szelet
> - gyorsabb, kb 2 perc 1 scan
> ![gen2](https://cdn.shortpixel.ai/spai/w_1200+q_lossy+ret_img+to_webp/https://howradiologyworks.com/wp-content/uploads/2019/07/ct_gen_second_gen_2nd.gif)


> **3. gen CT**
>
> - több mint 800 detektor, tlejes testes besugárzás, forog a test körül a fej.
> - röntgencső és detektor mechanikailag egybefüggő egység
> => egy rossz pixel egy teljes kört alkot a kész képen amit eliminálni kell <- ez a beackprojection hiba
> 
> - a sugárforrás és a detektorok is forognak
> 
> ![3th gen ct](http://www.impactscan.org/slides/impactcourse/basic_principles_of_ct/img26.gif)
>
> ![](https://cdn.shortpixel.ai/spai/w_800+q_lossy+ret_img+to_webp/https://howradiologyworks.com/wp-content/uploads/2019/07/parallelBeam_fanBeam_coneBeam_800_1600-1.jpg)

> **4. gen CT**
> 
> - gyűrű műtermékek eliminálása => nem egy kört okoz egy rossz pixel hanem 1 pontot
> - 4800 detektor
> - csak a sugárforrás forog, detektorokkal rajtuk körbe
>
> ![4th gen ct](http://www.impactscan.org/slides/impactcourse/basic_principles_of_ct/img27.gif)

> **5. gen CT**
>
> - a forrás és a szenzorok si helyben maradnak, csak az elektron nyaláb mozog mint a régi TV-kben
> - nagyon gyors, 17 ms
> - alkalmazható érrendszeri vizsgálatokhoz is
> 
> ![mindne fix, csak a beam mozog mint egy katódos TVben](https://cdn.shortpixel.ai/spai/w_1200+q_lossy+ret_img+to_webp/https://howradiologyworks.com/wp-content/uploads/2019/07/ct_gen_fifth_gen.gif)

## CTA (computed tomography angiography)
CT amivel ereket figylenek meg.
- kontraszt anyagos CT
![CTA image](https://ars.els-cdn.com/content/image/1-s2.0-S0735109720359659-gr2.jpg)

Sugárterhelése (mSv-ben):
- CT koponya - 3.8
- vese - 4.6
- vastagbél - 7.4
- CT egésztest - 8.2
A Föld népessége  átlagosan évente 2,4 mSV sugárterhelést kap

# MRI
> - http://mriquestions.com/index.html
> - https://egeszsegvonal.gov.hu/m/877-mr-vizsgalat.html
> - http://oftankonyv.reak.bme.hu/tiki-index.php?page=MRI+posztgrad&structure=Orvosi_Posztgradu%C3%A1lis
> - https://www.hopkinsmedicine.org/health/treatment-tests-and-therapies/magnetic-resonance-imaging-mri

röviden: https://www.youtube.com/watch?v=1CGzk-nV06g

hosszabban: 
- [YouTube - How MRI Works - Part 1 - NMR Basics ](https://www.youtube.com/watch?v=TQegSF4ZiIQ) 
- [YouTube - How MRI Works - Part 2 - The Spin Echo ](https://www.youtube.com/watch?v=M7yh0To6Wbs) 
- [YouTube -  How MRI Works - Part 3 - Fourier Transform and K-Space ](https://www.youtube.com/watch?v=R_4GuyJTzMo)

Hidrogén protonokat egy irányba állítunk amiket ha bárhol megváltoztatunk akkor az feltűnő lesz, ezt egy sugárral és egy rf antennával érzékelhetem
- homogén mágneses tér
- alagút típusúba betesszük a mukit vagy félig nyitottnál nem olyan jó a képmínőség. Alagútasnál 1; 1,5; 3; 7 teslásat is előállíthatunk.

<img src="https://mersz.hu/mod/object.php?objazonosito=m538it_541_i1_idx" alt="mri gép" width=50% height=50% ><img src="https://cms.sulinet.hu/get/d/45d45d68-1d9c-4e3f-ab81-6c3715093917/1/1/b/Normal/normal.png" width=50% height=50% alt="mri szekezete">

![mri struct](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS1G0xq7rXmsuFvTqW8tQ5Pjtdun1y9x8_OOQ&usqp=CAU)

[YouTube K-Space: A way to understand how MRI parameters affect images](https://www.youtube.com/watch?v=QHtZR0mtB80)

- Diffúziós MRI ami valaminek a folyamatát tudja monitorizálni. 
- [Tractographya](http://trackvis.org/) valaminek az útvonalait adja vissza.

> Nagy mágnesességű (tesla nagyság) párhuzamos elektormágnes tekercsekkel létrehozunk egy elektromágneses mezőt, ahol a szövetben levő hidrogén atomok protonjait egy irányba rendezzük (hidrogén mag polarizálása) homogén mágneses mező létrehozásával. Ugyanis a protonok mágneses térben képesek elektromágneses energiát befogadni és kiadni ellenben nyugalmi állapotban a protonok mágneses tulajdonsága véletlen eloszlású.
> 
> A befogadott energia ugyanakkor távozik amint a mágneses tér megszűnik, sőt, nem csak távozik, de a protonk vissza is rendeződnek eredeti állapotukba. A `protonok keringésnek frekvenciája = gyromgáneses_együttható * mágneses mező ` szorzatból áll össze, a keringési frekvencia másik neve *[precesszió](https://hu.wikipedia.org/wiki/Precesszi%C3%B3)*. Épp ezért befolyásolja a mágneses mező erősségének változása. Mikor a mágneses mező megszűnik a spin adott időegység alatt áll vissza az eredeti pozíciójába. Ez különbözik a különböző szövetek esetén, és ezt tudjuk mérni. Ez gyorsan történik meg pl csontok esetén, és a leglassabb a víz esetén, a szöveek vízzel való tetlítettsége befolyásolja a köztes skálát. 
> 
> E mellett egy gyengébb, időben változó (1 kHz nagyságrendű), térbeli kódoláshoz szükséges, ún. gradiens mezőt is létrehozunk. E mellett egy gyenge rádiófrekvenciás (RF) mező, mely egy RF antennán keresztül összegyűjthető, mérhető jelek produkálását lehetővé tevő manipulációjára képes a hidrogénmagoknak. Ezek a mágneses térre merőleges jelek, melyek kitérítik a protonokat. A gerjesztés után (adott Hz H:64) mérhetőek a kitérés (elektromágneses energia leadásának) komponensei
>
> A három gradiens tekercs a főbb irányok felé van állítva, így létrejön a térbeli lefedettség.
> 
> - A mágneses tér erőssége nagyban meghatározza a kinyerhető jel erősségét
> - Rádióhullámok segítségével közlünk energiát, és a kapott „visszhangot” rögzítjük
>
> Ezeket az adatokat vizualizálhatjuk valós vagy imaginárius értékek mentén, de fázis vagy amplitúdó alapján is lehet. Ugyanakkor a gyakorlatban ezen a ponton Fourier transzformálunk, hogy a frekvenciát elemezzük. Ezt terjeszthetjük ki 2D-be, úgy, hogy a jeleket egymás mellé téve értelmezzük, és így kapunk egy 2D szeletet. Ezt kibővítjük 3D-re tomográfiával, azaz egymás mellé tesszük a szeleket.
> 
> A kontraszton tudunk állítani ha nem azt mérjük, hogy mennyi idő után áll vissza eredeti spinbe a proton, hanem adott idő után  mérjük az aktuálisan mérhető a visszaálláskor elengedett elektronokat. Ezzel minden pont ahonnan már épp nem jön jel lehet fekete, ahol még erős ott meg fehér, és az összes többi a szürke 255 árnyalata.
 
Ahogy az látható, az eljárás drága, és értelemszerűen nem alkalmazható akkor ha valamilyen fém tárgy van a testben, pl pacemaker, csont erősítő váz, börtöntetkó, exoskeleton stb.

## fMRI
- https://www.radiologyinfo.org/en/info/fmribrain
- http://fmri.ucsd.edu/Research/whatisfmri.html

A kifejezetten agyra kitalált kontrasztos MRI. A vér áramlását méri az agyban. Nyilván ehhez szükség van valamilyen ingerre ami az agyi folyamatokat változtatja.

röviden: https://www.youtube.com/watch?v=rJjHjnzmvDI

## DWI
- https://radiopaedia.org/articles/diffusion-weighted-imaging-2
- https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5039674/

> Kiemeli azon részét az MRI-nek ahol nem jó a nedvesség, tehát azt ami alapból nem reagálna kellő mértékben a mágneses sugárzásra. 
> 
> Brown mozgáson alapul.

## Hyperfine
mobil MRI készülék https://hyperfine.io/

# PET
- https://egeszsegvonal.gov.hu/p-q/898-pet-vizsgalat.html
- https://www.hopkinsmedicine.org/health/treatment-tests-and-therapies/positron-emission-tomography-pet

> Pozitron emisszós tomográfia - nukleáris medicína
>
> Mennyiségi viszonyokat ad meg, mennyi van az adott szövetből.
>
> Egy sugárzó anyagot adunk be amit mérünk és a mérések alapján készítünk képet, ezzel folyamatokat lehet monitorizálni, keringési problémát, agyi, vagy daganatos jelenségeket figyelünk, folyamatokat vizsgálhatunk közel valós időben.
> 
> ~ 11mSv egység
> 
> Ha az alanyt egy csőszeletben helyezzük el akkor a mérés közben a kilövelő beta részécskéket egy szenzoron érzékeljük, amikor beérkezett megnézzük, hogy az átelmmeben levő oldalon az átmérő fénysebeségel való átfutási idejével megegyező időn belül lesz-e becsapódás, ha lesz akkor tudunk képet készíteni, 2D szeletben, mivel a time of flightot visszaszámoljuk a két átellenben levő szenzorból, és ismerjük a részecske sebességét és a becsapódások közti időkülönbséget így a távolságot is megkaphatjuk. Ez a [time of flight](https://info.blockimaging.com/what-is-time-of-flight-pet-scanning) . A rögzített kép egy hamis színkép, hőtérkép szerű eredményt ad.
>
> ![](https://www.researchgate.net/publication/337325700/figure/fig1/AS:826576459530243@1574082593894/The-basic-principle-of-a-positron-emission-tomography-PET-system-A-PET-detector-ring.png)![](https://www.researchgate.net/publication/342053802/figure/fig1/AS:902008584294400@1592067013365/Positron-Emission-Tomography-PET-imaging-a-neutron-deficient-radioisotope-positron.png)
> 
> *A daganatos sejtek energiaigénye jóval meghaladja a normál sejtekét, így azok cukorból is többet fogyasztanak. Mivel a vizsgálat során felhasznált izotóp speciális cukormolekula, nagyobb koncentrációban lesz megfigyelhető a daganatos területen. A szívvizsgálat során ezzel szemben kimutathatók azok a területek, ahol valamilyen oknál fogva éppen csökkent a sejtek anyagcseréje, ami arra utalhat, hogy az érintett terület károsodott.*
>
> - carbon11
> - nitrogén 13
> - oxigén
> - fluór 18
> - rubidum 82
>
> ezért egyértellműen időkritikus a vizsgálat.
> 
> ![](https://image.slidesharecdn.com/earlyadwebinarlandau-121130144021-phpapp02/95/early-alzheimers-disease-webinarlandau-7-638.jpg?cb=1354286480)
> 
> kombinálhható:
> - CT
> - MRI


> SPECT - single photoemission PET  
> - [PET vs SPECT](https://www.youtube.com/watch?v=_NSyAEi12M0)
> - gamma részecskét használ
> - https://www.nature.com/articles/nrclinonc.2012.188
> 
> ![](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fnrclinonc.2012.188/MediaObjects/41571_2012_Article_BFnrclinonc2012188_Fig1_HTML.jpg)


> ![](http://www.eventideib.polimi.it/wp-content/uploads/2019/05/PastedGraphic-1-730x410.png)![](https://ars.els-cdn.com/content/image/1-s2.0-S1120179715010492-ejmp619-fig-0001.jpg)

- https://www.youtube.com/watch?v=Bgkta3D1TfA
- https://www.youtube.com/watch?v=Bmj30dBWelE


### A PET-vizsgálat nem kívánt hatásai
*A vizsgálat során nagyon ritkán a beadott izotóp hatására túlérzékenységi reakció alakulhat ki. Az ilyen jellegű allergiás reakciók ellátására azonban a vizsgálatot végző intézmény fel van készülve. Bár a vizsgálat során a sugárzás mértéke csekély, az mégis beavatkozhat a magzat fejlődésébe, így terhesség során a PET-vizsgálat általában ellenjavallt*

# OCT
- https://repo.lib.semmelweis.hu/bitstream/handle/123456789/122/schneidermiklos_DOIs.pdf?sequence=4
- http://titan.physx.u-szeged.hu/tamop411c/public_html/L%C3%A9zerek%20az%20orvostudom%C3%A1nyban/841_az_optikai_koherencia_tomogrfia.html

![OCT VS MRI VS CT](http://obel.ee.uwa.edu.au/wp-content/uploads/2015/01/Fig_3_OCTcomparison.png)

- https://www.youtube.com/watch?v=HJnNJIUPm4s
- https://www.youtube.com/watch?v=FKzIH7o8zTA
- https://www.youtube.com/watch?v=dlkXHWUhpV4

használt:
- bőrgyógyászatban
- megtudom mondani melyik irányban áramlik a vér

> Fény alapú koherens tomográfia, *tulajdonképpen az ultrahangos képalkotás optikai analógiájának tekinthető, azonban annál akár két nagyságrenddel jobb.*
> 
> Az OCT legegyszerűbb változatának működési elve megegyezik a fehér fényű interferencia mikroszkópéval, vagy éppen a fehérfényű optikai profilométerével. A készülék alapját egy Michelson-féle interferométer képezi: egy fényforrásból kiinduló nyalábot egy féligáteresztő tükörrel ketté osztanak, majd egy bizonyos távolság megtétele után egy-egy tükörről visszaverődve a nyalábosztó újból egyesíti és egy detektorra irányítja őket.
> 
> Három esetl lehetséges:
>  - a vizsgált és a refernecia hullámok épp erősítik egymást
>  - a vizsgált és a refernecia hullámok épp gyengítik egymást
>  - a vizsgált és a refernecia hullámok épp egymás után csapódnak be, különbözik a hullámhosszuk
>  
>  Ezeket egy minimális hullámhossz különbséggel lehet kijavítani
> 
> ![Michelson interferometer](http://titan.physx.u-szeged.hu/tamop411c/public_html/L%C3%A9zerek%20az%20orvostudom%C3%A1nyban/8.4.1_abra.jpg)
>
> SLED/LED - 800--1300-1550 nm hullámhosszal
> 
> 5-10-30 fpses feptosecundumos laser
> 
> 4-5mm mélyen mérhető a szövet
>
> - erő és távolság mérésre is használható, az üveg (*amiben megy a jel*) törési mutatójának segíŧségével
> - amikor a szemben a nyomás lecsökken beomlik a retina és részleges vakság áll elő
>   - ekkor egy trombózis állhat elő ami a szem hajszálér hálózatában áll elő, és az azt övező rész elhal
>     - ez vérhígitóval enyhíthető, 15 - 20 um

## Time domain OCT
> - monochrome fényt használ
> - 2 eszköz van, egy referencia tükör, amit piezoval rezegetek, másik oldalon az intrfeernciát nézem.
> - ezzel az adott szövet visszaverési képességeit nézhetem, amit így um pontossággal mérhetek rétegenként
> ![OCT](https://marvel-b1-cdn.bc0a.com/f00000000038905/www.aao.org/full/image.axd?id=d176ad37-e1c1-4090-a7be-fc863dc43756&t=636737514114430000)
> 
> A visszaverődés minden rétegből egy-egy jelet küld vissza, aminek a végén egy summát kapok. A referencia tükör mozgatható, és olyan távolságba tesszük amivel pont azt a hullámhosszt kapjuk meg amelyik az általunk visgált mértékből érkezik. A piezo ciklikus rezgéséből egy időrés keletkezik amiben mozgatjuk a tükröt és ebből fakad az idő alapúsága az eljárásnak.
> 
> *Ha a két nyaláb a pontosan ugyanakkora utat tett meg a detektorig, akkor fázisban vannak, konstruktív interferencia jön létre. Ha valamely tükröt mozgatjuk, akkor a Δl útkülönbségnek megfelelően a két nyaláb hol erősíteni, hol pedig gyengíteni fogja egymást, a detektor a tükör helyzetének függvényében egy periodikus jelet fog mérni. A jel modulációja annál nagyobb, minél kisebb a különbség a két nyaláb intenzitása között.*
>
> ***A scan***
> - *x* tengely távolság
> - *y* tengely optikai denzitás
> - oszcilloszcopeon látszik
> 
> ***B scan***
> - távolság alapján mondható meg a pixel intenzitása
>  
> http://obel.ee.uwa.edu.au/research/fundamentals/introduction-oct/
> ![TOCT](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/OCT_B-Scan_Setup.GIF/545px-OCT_B-Scan_Setup.GIF)![](http://obel.ee.uwa.edu.au/wp-content/uploads/2015/01/Fig_1_TDOCT.png)

## Multi spectrum OCT
> - több fénynyalábot használ
> - a különböző spektrumokat furier transzformációcal szétbontják, így az egyes mélységek denzitásai megmondhatóak
> - itt nincs rezgő tükör, többféle hullámhosszt ad ki a fényforrásom.
> - itt 1024-es A-scant használok.
> ![](http://obel.ee.uwa.edu.au/wp-content/uploads/2015/01/Fig_2_SDOCT.png)![](https://www.researchgate.net/profile/Pengfei-Zhang-17/publication/281790160/figure/fig1/AS:795469957582848@1566666225195/Multispectral-SLO-OCT-system-schematic-BS-Beam-Splitter-DM-Dichroic-Mirror-DC.png) ![](https://www.bmo.uni-luebeck.de/fileadmin/_processed_/3/e/csm_Forschung_OCT_Multi_00_277d1b3b5a.png)

# ultrahang
- a hang sebessége függ az adott közeg összetételétől
- a beadott energia visszaverődését mérjük
- kvantitatív és kvalitatív szerv morfológiát lehet vele nézni;
- nem invazív
- nincs káros biológiai hatása
- a szövet áteresztőkpességén / törésmutatóján múlik az ultrahang működőképessége, ez levegeőben rossz, ezért pl tüdőt/csontot nem lehet
- a képben keletkező levegőbuborékok a műtermékek
- külöünféle ultrahang vizsgálatnál különféle fejekkel különböző mélységig vizsgálni a szövetben, így egy tárgy-transducer távolság kétszeresét nézzük

![](http://www.sprawls.org/ppmi2/USPRO/usimage2.JPG)

A hanghullámnál mini terjedések kezdenek kialakulni.
mindezt egy piezoelektomos jellel tudom megtenni.

Az oszcilloszkópon megjelenik a visszajövő jel az A scan

A térrész minden eleméhez rendelek egy értéket és attól függően mikor ér vissza onnan a jel adok hozzá színt 0-255 tartományon. a legmesszebbi a legsötétebb a legközelebbi a fehér. Ez a **B mód**.

Ha több `B módú` scant összetesszük kapjuk az `M-módú`t.

Dopler hatáson alapszik, így akár folyamatokat is láthatunk, hogy merre folyik a vér.
- ha kiküldök egy frekvenciát és a visszapattanó nagyobb akkor jön fleém
- ha a visszapattanó kisebb akkor megy elfele

https://piurimaging.com/

- felszíni, textúra mód
- elmosott mód
- megvilágított mód
- maximum/minmum mód
- x-ray mód

használata:
- daganatok pontos volumen mérse, stb
- transrectális, transvaginalis ultrahang

[Több lentebb](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#ixultrahangos-k%C3%A9palkot%C3%A1s)

## Optika, mikroszkópia
> Képalkotás, optikai tartományban, mik a lencse hibák, mivel korrigálhatóak, stb.
>
> Megvilágítás, milyen a mikroszkóp beli megvilágítás, milyen előfeldolgozás lehetséges, festés, dlc, hoffmann, fázis, sötét látóteres mikroszkóp.
> 

több: https://www.ibiology.org/online-biology-courses/microscopy-series/


### Mikroszkóp felépítése
![mikroszkóp szerkezete](http://clipart-library.com/images/gie5864eT.jpg)

1. fényforrás
2. fénnyaláb
3. tükör
4. kondenzor
5. tárgylemez
6. objektív / tárgylencse
7. test
8. szmelencse

### Lencse rendszer
http://mesterandras.hu/wp-content/uploads/2020/03/Geom_optikalencsek-1.pdf
- lencse fősíkja és a fókusz között a fókusztávolság
- a kettő közötti közeg törésmutatója befolyásolja a fény törésmutatóját

### lencse tulajdonságai
https://docplayer.hu/43658178-Optika-gombtukrok-kepalkotasa-lekepezesi-hibak-dr-seres-istvan.html
- törésmutatója
- numerikus apertúra: a lecse fénygyűjtő képessége, jele *NA*, az olajé a legjobb
- felbontása, jele *`d = lambda/2*NA`[~micro m]*
- mélységélesség *z-tartomány*
- látómező: megvilágított kör szemlencsében [~mm]
- munkatávolság: objektív-fedőlemez táv

![objektív](http://www.bwoptics.com/html/UploadFile/201056846928.jpg)

- szférikus aberráció: ![szférikus aberráció](https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/Spherical_aberration_2.svg/1024px-Spherical_aberration_2.svg.png)
  a lencse nem meg  fókuszpontba öszpontosít
- kromatikus aberráció: ![kromatikus aberráció](https://digiretus.hu/wp-content/uploads/2017/12/photoshop-szinhiba-eltavolitasa-6.jpg)
  másképp töri meg a fénysugarakat, és a színek kettéválnak
  **javítása:** a lencse állíása mert nem jó pontban van
- képmezőelhajlás/mezgörbület
  ![képmezőelhajlás](https://docplayer.hu/docs-images/59/43658178/images/21-0.png)
  **javítása:** digitálisan szorzzuk egy korrekciós mátrixszal
- asztigmatizmus ![asztigmatizmus](http://autosjatekok.co.hu/images/lts-lesen-esett-az-asztigmatizmus.jpg)
  **javítása:** növeljük a látómezőt
- üstököshiba: ![üstököshiba](https://cdn-60a62604c1ac1c1d10df7525.closte.com/wp-content/uploads/sites/321/2010/12/v_o_koma_hiba.png)
  **javítása:** több lencsét tudunk használni

## nagyfelbontású fénymikroszkópia I.
- Lézer: koncentrált fénnyaláb, leadja az energiatöbbletet, ezt kezeljük fotonként,
A fény mindenképpp szinuszosan moszog!

Hullmámhossz egyensen arányos a frekvenciával.
 
**Huygens elv:** körhullám -> hullámtér -> minden egyes pont egy-egy egyedi hullámforásnak tekinthető -> ezek széle egy gömbhullám amin van a hullámgörbe

**Fresnel elv:** ezek a köthulllámok interferálnak, és ezek eredője adja meg milyen az egész fényünk.

Étendue: geometriai kiterjedés.
         - https://en.wikipedia.org/wiki/Etendue

**fázis konjugált tükrök:** visszatükrözi és folymatosan normalizálja az Étenduet

**Festési eljárások:**
- hematoxifin: mivel savas ezért a sejtmagokhoz ideális
- eosin: bázikus, pl citoplazmához való.

**kotrasztosíás**
- kvalitatív 3D fotografikus
- 2x prizma, fény polarizálása
- analizátor: fáisretardáció, fénnyaláb rekombinálása
- DIC
- Hoffmann modulációs kontraszt mikroszkóp: aaz aperturán lévő lyukakkal állítja a éfny mennyiségét, és így csökkenti a glória hatást.
- fázisrárgy: a féyn amplitúdóján lehet ávltoztatni, ezzel fáziskontraszt mikroszkópot alakíthatnunk ki, át állítjuk a fény mennnyisgét, a kondenzátor egységesíti, de a fázisát beállíottuk, így csak a kontúrok jelennek meg.

**sötétlátóteres mikrszkóp:** kolloid mintáknál lehet használni, tegár képesek a fényt szórni, és mi ezt a szórt fényt látjuk a végén. Mindent mai mikrométers tartományba esik és festetlen alkalmas rá.

## mediso
egyedül nekik van 3 fejő MRIük

a spektnél a adott keresett problémához igazítjuk az izotópot ami a leginkább reagál az adott valamire.

egy spekt felvétel 25-40 percig tart a valóságban

6 milli sv az éves határ amit nem haladhat meg az egy főre eső sugárzás

## Nagyfelbontású fénymikroszkópia II.
### Konfokális mikroszkóp
> **fluoreszencia mikroszkóp**
>
> Az angyagot megvilágítjuk fénnyel amit utána emittál, ez a stokes shift: abszorció - emisszió
>
> - minden anyagot ami hullámváltoztatásra képes *flourofór*
>
> A mintán belül csak a kiválasztott sejtekkel tudjon érdemi mennyiségben elreagálni. Az energiát átadjuk és az fényként emittálódik
>
> - *adszorció:* csak a felületén képes anyagokat megkötni
> - *abszorció:* az anyag mélyében is képesek vagyunk megkötni az anyagot <- *fluoereszcencia*
>
> 1. *dichroicus* tükörrel megtörjük a fényt de csak az adott hullámhosszon, amit egy *excitation* szűrővel szűrünk, visszajuttatjuk a tükörnek az objektíven keresztül majd a másik hullámhosszon amit már a tükör átenged és ez jut az oculárba.
> 2. szelektív megjelenés + emissziós szűrő -> jó kontraszt -> specifikus megfigyelhetőség
>    **előnye**: jól színezhető


#### Abbey-elv
> https://en.wikipedia.org/wiki/Diffraction-limited_system
>
> fénynyalábot nem lehet minden határon túl fókuszálni  => egy elemi tárgypont képe elmosódott lesz => Airy korong => felbontás limit
>
> **felbontás javítás:**
> - ha a képet megvilágítjuk nem csak X-Y síkban történik a diffrakció
> - Ha a lencse széléből jön a fénynyaláb is zavart okozhat
> - síkokból érkező fénynyalábok kiküszöbölése
> - a képsíkban a szélső területekről érkező fénynalábok kiküszöbölése
> - diffrakciós limit átlépése: ![The Abbe diffraction limit for a microscope](https://wikimedia.org/api/rest_v1/media/math/render/svg/2a4dfa1f30e4a718d5c4573d5bdac3fd96e248fb)

### Konfokális mikroszkóp
> **Lumineszencia:** gerjesztés után elindul a relaxációs folyamat
>
> **foszfor esszencia:** olyan állapotokba is belép az eleketron amikbe ha önmagában lenne nem lépne be.
>
> ![konfokális mikroszkóp](https://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/Confocalprinciple_in_English.svg/1024px-Confocalprinciple_in_English.svg.png)
>
> Ezzel kiküszöböljük a nem képsíkból érkező nyalábokat. Ezért pásztáznunk kell, mivel ekkor egy pontból kapunk fénnyalábokat.
>
> - vízszintes ~ 200 nm
> - függőleges ~ 500 nm -> baktérium vírus vizsgálata
> -> xy-síkszilárd 

### STED: Stimulált emissziós kioltásos mikroszkóp
> Kontra fényeket indítunk melyek hullámhossza kioltja a megjelenő fényt és ezzel pásztázunk így az adott ponthoz pontos értéket tudunk mondani.
>
> a fény hullámhossza úgy van belőve, hogy más sejteket ne lássunk.
>
> - felbontás: 40-90nm -> fehérjék nayobb szerkezetét látjuk

### NSOM - Near field scanning optical microscope
> Az apperturához közel tesszük a mintát, ezért kevesebb fény megy át.
> - felbontás: ~ 10nm -> proteinek kisebb szerkezeteinek vizsgálata

### elektronmikroszkóp / pásztázó próba mikroszkóp
> https://www.zeiss.com/microscopy/int/cmp/lsc/21/sim-squared.html
>
> STM = Scanning Tunneling Microsckope (elektron)
>
> **Alapjelenség:** alagút effektus: szubnanonméteres távolságra levő potenciál különbséggel rendelkező pontok között az elektronok csak egy nagy valószínűséggel jellemzett "csatornán" keresztül közlekedhetnek
>
> **működés:** feszültséget adunk a rendszerre, ezért a minta elkezd mozogni, a mintára lézerfényt vetítünk, ami visszaverődik egy tükörre amin mérjük a fény mennyiségét, és így tudjuk mérni a fizikai felületünk felszínét.
>
> felbontás: ~ 1nm -> molekulák szintje

## Digitális mikroszkópia III.
- https://docplayer.hu/21681267-Feny-es-fluoreszcens-mikroszkopia-szuperrezolucios-mikroszkopia.html

> Képalkotás érzékelt jelek feldolgozásával alkaítunk ki látható digitális képeket
>
> képfeldolgozás a kialakított kép sajátosságait módosítás szűrés keresés elemzés
>
> **képalkotás menete:**
> - jel átalakítás elektromossá
>   - CCD: fotoérzékeny áramköri lapka
>   - fény intenzitása ~ áramerősség
>     - a különböző irányból érkező fény egymáshoz képest is arányos kell legyen
>   - étalkítás precizitásának biztosításához at analóg jelet megfelelően kell erősíteni/csillapítani
>   - túlfeszültség védelem -> adott fényerősség fölött maximum érték átadása
> - analóg jel kondicionálása
> - analóg jel mintavételezése
>   - piramis képként van tárolva
>   - felbontás változtatható -> file pixelek negyedelése
>   - 3D: összeillesztés z-tengely mentén-> praffin blokk rekonstruálása <- stitching
> - minták kvantálása
> - kódolás
>
> **Hibák a képalkotásban** ugyanúgy lehetséges mint [korábban](https://github.com/gabboraron/diagnosztikai_celu_orvosi_kepalkotas#lencse-tulajdons%C3%A1gai)
> - alulmintázás is történhet egy változó rendszerből: Nyquist-kritérium
> - [Hisztogram](https://github.com/gabboraron/szamitogepes_kepfeldolgozas#hisztogram) pixel fényesség eloszlás
> - alacsony bitmélység: kvantáláskor
> - adott pixel intenzitás mennyi bittel írható le, kontraszt elveszhet, javítás: több biten tárolunk.

## 0,1 THz inpulzusos sugárzás mérés
elektrooptikai mintavételező

> Revolutionary enhancement of visibility by exploring active light fields
- kis energia
- alkalmas spektroszkópiához is
- biztosnágtechniaki alkalmazása
- belemegy az anyagba

## UWB radar alapú képalkotás
- https://www.radartutorial.eu/02.basics/UWB%20Radar.en.html
- https://en.wikipedia.org/wiki/Ultra-wideband

kis hatótávolságú radar technológia, nagy rádió spektrumon. Pontos helymeghatározásra és követésre alkalmas.

- kis impulzusok
- rövid dieig
- nagy energiát ad át
- camero tech 

![](https://www.mdpi.com/sensors/sensors-21-02488/article_deploy/html/images/sensors-21-02488-g001.png)

## spektroszkópia
visszavert fény alapján képalkotás

## képi adatok tárolása, menedzselése
> képformátumok:
> - raw (bináris)
>   - szigetszerű
>   - fájlkonvertálásánál elvesztünk adatot
> - JPEG/JPEG200/TIFF/BMP
>   - streamelhető
>   - lehet nem veszteséges tömörítés
>   - eltűnnek az annotációk
> - strukturált adatokként
>   - json/xml
>   
> a nagy képeket is tileonknt használhtjuk és összevarhatjuk (stiching)
> 
> dicon a köztes formátum amit mindegyik tároló rendszer tud értelmezni. 
>   
> az emberi test  Metszettis síkokon:
> - longitudinális
> - transzerzlis
> - horizontális
> 
> DIICON fájlként tároljuk rawban a nagy képeket ezekeet metaadattal való támogatását a DICCOM fájl `.dcc3` 
> 
> ![](https://dicom.nema.org/medical/dicom/current/output/chtml/part05/figures/PS3.5_7.1-1.svg)
> 
> - tag: egyedi aznosító
> - value length:
> 
> [PACS](https://en.wikipedia.org/wiki/Picture_archiving_and_communication_system)-ban tároljuk a kpeket amiket `C-FIND`al keresünk `C-RESPONSE`-ban kapunk váalszt.
> 
> Mango a PACS adatainak megjelenítője.
> 
> ![](https://www.visualmedica.com/wp-content/uploads/2020/09/Esquema.png)
> 
> ### alternatívák
> - HL7
> - pathonet

## vérkenet
> meg tdom mondani egy vörösvvértestről, ohgoy az-e vag yvörösvérsejt, vagy mondjuk röntfgenre tudok berajzolni olyasmit mai egyébként nem látható
> 
> A kamera egy kis lyukon át kapja a jelet a tárgyról, a munka nagyját a szoftver végzi el.





-----
## Beadandó - Mikroszkóp építés
- [I made a scanning laser microscope](https://www.youtube.com/watch?v=9TYlQ4urcg8)
- https://openflexure.org/

----

## ZH II. - felkészülés
### VI.Spektroszkópia/spektrometria
#### 1. A spektroszkópia/spektrometria alapjai
> - egy színkép megfigyelésének módszere
> - A molekula energiaállapotát az elektronok energiaállapota (`Eel`) az atomok rezgési (`Ev`) és forgási állapota (`Er`) együtt szabja meg: `h = E1-E2 = (Eel,1-Eel,2) + (Ev,1-Ev,2) + (Er,1-Er,2)`
> 
> **hullámok típusa szerint:**
> - elektromágneses sugárzás
>   - Látható fény spektroszkópia
>   - Gamma spektroszkópia
>   - Röntgen spektroszkópia
>   - Ultraibolya spektroszkópia
>   - Infravörös spektroszkópia
>     - távoli, közép és közeli
>   - Terahertzes spektroszkópia
>   - Mikrohullámú spektroszkópia
>   - Rádióspektroszkópia
> - részecskesugárzás
> - nyomáshullám
> 
> **Raman elvű spektroszkópia**
>> egy anyagot erős monokróm az arról visszaverődő fény az anyag összetételétől függően frekvenciájában megváltozik, egy fénysprektrumot eredményez. A spektrumból következtetni lehet a vizsgált anyag tulajdonságaira
>>
>> ![Raman spektrométer](http://www2.sci.u-szeged.hu/inorg/MOMA/resources/img-07-07.jpg)
>> 
>> *A lézerfényt ráirányítjuk a mintára majd az onnan visszaverődő fényt egy szűrővel kiszűrjük, hogy biztosan csak a visszaverődőt kapjuk meg, majd ezután egy spektrumra leképezzük a rács segíségével.*
>> 
>> A minta lehet gáz, folyadék vagy szilárd is!
>
> **kölcsönhatás szerint:**
> - abszorpciós spektroszkópia
> - emissziós spektroszkópia
> - rugalmas szórás
> - rugalmatlan szórás
> - rezonancia spektroszkópia
>
> **Termikus:** infrasugárzás hatására felmelegszenek és ennek hatására valamelyik fizikai (villamos) paraméterük megváltózik => villamos jel "kinyerhető„
>
> **Foton-detektoros:** fotonok számával arányos villamos jelet adnak, de működésükhöz mély hőmérsékletre való lehűtésük szükséges
>
> **A termográfia (hőtérképezés):** 
>> funkcionális eljárás, az emberi test hőmérsékletét mérjük infrakamerával és szoftver segítségével. A bőrfelszínen és a test belsejében zajló egyes élettani vagy kórélettani folyamatokis figyelhetőek vele.
>> 
>> **Szkennelő (letapogató):**
>> egyelemű ("pont"-) detektort használnak az infravörös sugárzás átalakítására és a mérendő tárgyat egy mechanikus rendszerrel tapogatják le.
>> 
>> **Mátrixdetektoros hőkamerák:** 
>> mechanikailag egyszerűbb, hőkép minden egyes képpontját egy-egy egyedi érzékelő alakítja át.
>> 
>> **termográfai főbb típusai:**
>> - **Natív termográfia:** test hősugarainak manipuláció nélküli vizsgálata. *Szűrővizsgálatoknál használható.*
>> - **Funkcionális termográfia (stresz termográfia)**
>>     - Terhelés esetén, a test hőmérsékletében gyors változást tudunk elérni, mely lassan rendeződik vissza. 
>>     - Termogén (hideg illetve a meleg próba), melyhez használhatunk: vizet, alkoholt, levegőt, klóretilt, száraz jeget stb.
>>     - Fizikai terhelést jelent, azaz, pl. lépéspróba. *Izomcsoportok vizsgálatára alkalmas.*
>>     - Kémiai próbák. Kemikáliákat alkalmazásával: cukrot a mellrák esetében, nitroglicerint az artériás érbetegségek esetén. 
>> - **Dinamikus termográfia:**
>>     Ez a módszer vagy folyamatos, vagy intermittáló felvételek készítéséből áll. Alkalmas *terápia hatékonyságának követésére*. 
 
#### 2. A spektroszkópia/spektrometria előnyei, 
> **termográfiás spektroszkópia (hőkamera):**
> - A sugárforrás maga az ember  
> - Nincs a szervezetre kisebb-nagyobb mértékben károsító hatás (CTI, MRI)
> - Teljes mértékben nem invazív vizsgálat
> - Nem szükséges szüneteket pihenő időket tartani két mérés között
> - Más képalkotó módszerekhez képest olcsóbb  (a szükséges technikai háttér megvalósítása)
> - Betegség/kór megelőző eljárás 
> - Vizsgálatait az alaktani (morfológiai) elváltozásokra épít
> - Alaktani elváltozások a struktúrák denzitás eltérésein át észlelhetők
> - Gyors, fájdalommentes, nincs mellékhatása.
> - Egy-három méteres távolságból készíthető.
> - nem igényel különös előkészítést a beteg részére
> - a vizsgálat gyors, kockázat- és fájdalommentes
> - a vizsgálat korlátlan számban ismételhető, mivel a testet nem éri semmilyen káros hatás, vagy beavatkozás
> - a vizsgálat során képet kaphatunk az egyes elváltozások korai stádiumáról, amikor azok jó eséllyel gyógyíthatóak
> - a vizsgálat sikeresen alkalmazható együtt bármilyen más diagnosztikai és gyógyászati módszerrel
> - nyomon követi az alkalmazott gyógyszer(ek), terápiák hatását
> - olyan személyek részére is alkalmas, akiknél egyes diagnosztikai eljárások az állapotuk, vagy betegségük miatt csak korlátozottan, vagy egyáltalán nem jöhetnek szóba (várandós, szoptatós kismamák, stb.)
> - Általános állapotfelmérés
> - Szűrővizsgálatok végzésére
> - Egyes gyomor-bélrendszeri betegségek szűrésére
> - A váz- és izomrendszer állapotfelmérésére
> - Ízületek, inak, csontok
> - Egyes daganatok vagy megelőző állapotok szűrésére
> - Egyes neurológiai megbetegedések szűrésére
> - krónikus és heveny hátfájdalom
> - migrén okainak szűrésére
> - Keringési megbetegedések vizsgálatához
> 
> **Pulzoximetria**
> - Fájdalommentes vizsgálat 

#### 3. A spektroszkópia/spektrometria hátrányai
> **hőkameránál:**
> - Ritkán előfordulat, hogy nehéz korrekt véleményt mondani.
> - Az alkohol és az altatók olykor különös és váratlan eltérés okoznak a bőrön
> - Erős gyógyszerek is korlátozzák a vizsgálat értékelhetőségét.
> - Napégés jelentősen befolyásolja a vizsgálatot.
> - A menstruáció időszaka is nehézséget jelent a diagnosztikában.
> 
> **Pulzoximetria**
> - Kritikus állapotú betegben a módszer sajnos gyakran megbízhatatlan a perifériás vasoconstrictio miatt (az eszköz nem érzékeli a pulzushullámot).

#### 4. Spektroszkópia/spektrometria vizsgálati megoldások
> **Kvalitatív vizsgálatok:**
> - **spektrum alapján:** Két anyagot akkor tekintünk azonosnak, ha abszorpciós színképük teljes egészében megegyezik
> - **abszorpciós színkép alapján:** eldönthető egy-egy anyag tisztasága ill. szennyezettsége, a szennyező abszorciójának mértéke is megadható.
> 
> **Kvantitatív vizsgálat:**
> - Kis koncentrációjú anyagok, ún. nyomszennyezők vizsgálata
> - több anyag keverékéből valamelyik komponens meghatározása 
> - Több komponensű rendszer mennyiségi meghatározását
>
> **Pulzoximetria**
> Nem invazív
> Oxigén szaturációt lehet vele mérni
> Véroxigén szint változás érzékelés
> Milyen hatékonyan tud a szív oxigéndús vért pumpálni 
> Kis csipeszhez hasonló készülék
> Ujjra csiptethető, lábra (csecsemők), vagy fülre
> Elterjedten használják intenzív osztályokon, illetve kórházakban
>
> *Alkalmazásai:*
> - *Chronic obstructive pulmonary disease (COPD)*
> - *Asztma*
> - *Pneumonia*
> - *Tüdőrák*
> - *Anémia*
> - *Szívinfarktus, szívproblémák*
> - *Hypoxia kimutatására*
> - *oxigénterápia ellenőrzésére
> - *Folyamatos monitorozás*
> - *Könnyen használható*
> - *használható távmonitorozásra is*

#### 5. A spektroszkópia/spektrometer berendezés általános belső működése
> **Hőkamera:**
>> - Melegvérű állatok szervezetében folyamatok során hő keletkezik, amely infravörös fény formájában kilép a testből.
>> - A hőkamera a testfelszín által kibocsátott 1-100 mikron közötti hosszúhullámú infravörös sugárzást méri.
>> - A test felszínéről érkező hősugárzást a kamera érzékeli és méri, az adatot villamos jellé alakítja és digitalizálja.
>> - A számadatokhoz színskálákat rendelnek => ez kerül megjelenítésre képként
>> - A hősugárzás mennyisége és hullámhossza a testfelület hőmérsékletétől és hősugárzó képességétől függ. 
>> - Az emberi bőrnek ideális, 94-95% a sugárzóképessége. Minden biokémiai folyamatnak sajátos termikus függősége, infravörös másodlagos kisugárzása van.
>>   - általánosan a végtagoknál a legalacsonyabb, a belsőszerveknél a legmagasabb
>> - A keletkezett hő kb. 85%-ban a bőrön és 15%-ba a tüdőn kelresztül távozik
>> - hőszállító közeg a vér, ezért a szervekből jövő vénás vér hőmérséklete magasabb, mint az odaáramló artériás véré, bőrből és a tüdőből jövő pedig még alacsonyabb.
>> - standard körülmények kzött 37,5˙C maghőmérséklet; 1˙C napszaknyi ingadozása van. Szájban ugyanez 36,8˙C; 0,4˙C ingadozással
> 
> **Pulzoximetria**
>> - Különböző hullámhosszúságú fény különböző mértékben nyelődik el az oxidált és a redukált haemoglobinban.
>> - A pulzushullám alatti nettó abszorpciót (elnyelést) mérik. Ez minimálisra csökkenti a szövetek, valamint a vénás és capillaris vér hatását az eredményre.
>> - Az eszközt általában 75–99%-os SaO2 értéken kalibrálják, a maximális hiba kb 2%
>> ![spo2 mérés](https://slideplayer.hu/slide/5747458/18/images/22/AZ+OXIMETRIA+ALAPELVEI.jpg)
>> 
>> érétkek:
>> - 95%-100% normális *(75-100 Hgmm)*
>> - 95% alatt hpoxemia *(60 Hgmm)*
>> - tartósan 89% alatt sejt károsodás

### VII.CTI - Computerised Thermal Imaging
- https://www.muszeroldal.hu/measurenotes/termografiaorvosi.html
- https://pubmed.ncbi.nlm.nih.gov/2600750/
- https://www.imaginis.com/thermography-cti/thermography-computerized-thermal-imaging-2?r

#### 1. A CTI alapú képalkotás
A termográfia (hőtérképezés) egy olyan funkcionális vizsgáló eljárás, amelynek során az emberi test hőmérsékletét mérjük infrakamerával egy erre a célra kifejlesztett számítógépes szoftver segítségével.

A CTI a legmodernebb orvostechnikai vizsgáló módszerek egyike, mely húsz év nemzetközi kutató munka eredményeként lehetővé teszi a szervezet kóros működéseinek korai felismerését. 

Az emberi test többek között infravörös hullámokat bocsát ki magából. A különböző helyeken fellépő minimális hőenergetikai különbségek termokamerával történő mérésével a szervezetben zajló kóros folyamatok korai felismerése válik lehetővé.

A gyulladásos szövetek, az aktív növekedési fázisban lévő daganatos sejtek legtöbbjének hőkibocsátása fokozott, míg a sorvadt, heges, alulműködő sejtek hőtermelése csökkent. Azon daganatos sejtek, amelyek hőtermelése nem magasabb a normál sejtekénél, a fokozott anyagcsereigény miatt megnövekedett számú erek (ún. "perivascularisatio") miatt mutathat emelkedett hőleadást.

![https://www.researchgate.net/figure/Schematic-diagram-of-infrared-thermography-camera_fig1_264185886](https://www.researchgate.net/profile/Young-Jo-14/publication/264185886/figure/fig1/AS:327936021417992@1455197448941/Schematic-diagram-of-infrared-thermography-camera.png)

#### 2. A CTI vizsgálat előnyei, hátrányai
A CTI elősegíti a góc felismerését. Érzékenysége miatt a kóros eltéréseket korán jelzi.
A teljesség nélkül, a következő betegségek lehetnek góceredetűek:
- szívizomgyulladás
- rheumás láz
- az izületek rheumás gyulladása
- egyes vesegyulladások
- kóros hajhullás
- egyes szemgyulladások
- tartós hőemelkedés
- egyes ideggyulladások
- visszatérő érgyulladások
- krónikus kiütések bizonyos típusai
- az úgynevezett eruptív psoriasis


Napjaink egyik leggyakoribb betegsége a különböző perifériás keringési eltérések. Egy bizonyos kor után szinte nincs olyan ember, akinek ne lenne visszértágulata. Ez a vénás keringés leggyakoribb zavara, amikor is leggyakrabban az alsó végtagon a véna fala kitágul, egyenetlen lefutásúvá válik és a vénákban lévő billentyűk elégtelenül működnek. A két lábon járás átalakította a test szerkezetét, de a vénabillentyűk nem rendeződtek át. Fekvő helyzetben a boka környékén a vénás nyomás kb.11 Hgmm. Járás nélküli állás közben a vénás nyomás kb. 100 Hgmm-re nő. Álló helyzetben a vénás vér áramlása a visszerekben megfordulhat. A helyi keringési feltételek elősegítik ezen visszerek begyulladását.  A CTI elősegíti ezen kóros folyamatok korai felismerését, így lehetővé válik megfelelő életmódváltással, kezelésekkel a keringési zavarok megszűntetése, prolongálása.

#### 3. A CTI alapú vizsgálatok típusai
A 80-as években az Amerikai Védelmi Minisztérium titkos, nagyléptékű megbízást adott a hűtés nélküli infravörös érzékelő technológia kifejlesztésére. A hadsereg olyan érzékelőt akart, amelynek nagyon rövid a mérési ideje.

Az infravörös módszerrel dolgozó eljárások lényege, hogy minden anyag energiát bocsát ki elektromágneses sugárzás formájában. Az abszolút nulla hőmérséklet -273,15fok Celsius. Az e fölötti hőmérsékletű tárgyak, szövetek által kibocsátott sugárzást a hőkamera méri, hőképpé alakítja át. Az infravörös sugárzás tartománya 0,75 és 100 mikron között van. Az infravörös kamera segítségével a láthatatlan hőenergia válik láthatóvá. 

1992-ben az Amerikai Kormány engedélyezte az infravörös technológia kereskedelmét, de az ellenőrzése alatt tartja a technológiát.

#### 4. A főbb hőkamera típusok/általános belső működésük 
- https://www.findlight.net/blog/everything-you-should-know-about-thermal-imaging-cameras/
- https://pim-kft.hu/szakmai-segitseg/publikaciok/hokamera-alaptipusok/

típusok:
- Letapogató hőkamerák - tükröt mozgat egy stabil szenzorral, az OCT-hez hasonlóan, csak refenrecia nélkül.
- Mátrixdetektoros hőkamerák - hasonlóak a hagyományos cmos kamerákhoz.

<img src="https://pim-kft.hu/wp-content/uploads/2016/02/szkenner.jpg" width=50% height=50%><img src="https://pim-kft.hu/wp-content/uploads/2016/02/matixos.jpg" width=50% height=50%>


#### 5. A CTI alapú képalkotás problémái
- Nem váltja ki az orvoslásban hagyományos diagnosztikai vizsgálatokat, azonban, mint funkcionális vizsgálat, új területet nyit a kóros folyamatok felismerésében, a kezelések hatékonyságának ellenőrzésében. 
- nem reprodukálható
- befolyásolják a körülmények
- befolyásolják a vizsgált alany közelmúlt beli cselekvései

### VIII.NIRS - Near-infrared spectroscopy
- https://en.wikipedia.org/wiki/Near-infrared_spectroscopy
- https://www.youtube.com/watch?v=ZUghUo-0p6E
- https://www.frontiersin.org/articles/10.3389/fped.2019.00560/full
- https://www.frontiersin.org/articles/10.3389/fnins.2020.00724/full

#### 1. A NIRS alapú képalkotás
> - Agyi oxigenizáció és hemodinamika monitorozása
> - Közeli infra abszorpció [O2Hb] és Hb [HHb]
> - Helyi  és agyi O2 szaturáció: rScO2
> - szövetek oxigéntetlítettsége, esetleg kisebb tumor észlelése

Különböző lézerdiódák különböző hullámhosszon világítják meg a szövetet optikai kábelekkel, foto detektorokkal érzékelünk a túloldalon, és a jelet kielemezhetjük. 

![](https://www.frontiersin.org/files/Articles/540710/fnins-14-00724-HTML/image_m/fnins-14-00724-g002.jpg)

#### 2. A NIRS vizsgálat előnyei, hátrányai
> ##### előnye:
> - Újszülötteknél jól használható
>
> ##### hátránya:
> - nem részletgazdag, az utófeldolgozás nélkül nem sokat jelentenek az adatok, nem hatol túl mélyre  

#### 3. A NIRS alapú vizsgálatok típusai
> ![NIRS](https://www.researchgate.net/publication/341805968/figure/fig1/AS:899134651392001@1591381814410/ERP-and-near-infrared-spectroscopy-NIRS-measurement-system-EEG-was-measured-at-T3-and.png)

#### 4. A NIRS berendezések általános belső működése 
> https://www.youtube.com/watch?v=Dj-X1t5pXvQ&feature=youtu.be
> 
> Házi barkácsabb megoldás:
> 
> https://www.youtube.com/watch?v=m6zpNSoQTV8

#### 5. A NIRS problémái
> nem túl részletgazdag

### IX.Ultrahangos képalkotás
#### 1. Az ultrahang  berendezés részei, elrendezése, működése
> A hang terjedése mindig valamilyen anyagban, közegben történik, vákuumban nem terjed. A hangsebesség nagyságát az anyag illetve annak fizikai állapota határozza meg.
> 
> - Hallható hang: 20-20.000 Hz
> - Infrahang: <20 Hz
> - Ultrahang: >20.000 Hz
> - Orvosi diag. ultrahang:>1MHz
> 
> Távolság (`d`) arányos az idővel (`t`). Ha tudom a  terjedési sebességet (`c`) akkor a távolság: `d=1/2 (cxt)`. `c = fxλ`, ezzel a frekvencia és a hullámhossz is kiejthető.
> 
> ![how ultrasound works](https://djmedquip.co.za/wp-content/uploads/2017/08/How-does-an-ultrasound-work.jpg) 
> 
> A nyalábméret Visszaverődik -> Megtörik -> Széttörik -> Elnyelődik -> Interferálódik.

#### 2. Az ultrahangos vizsgálat jellemzői, előnyei/hátrányai
> ##### előnyei
> - Hasi, kismedencei vagy lágyrész elváltozások esetén első vizsgálati módszer → meghatározza a további vizsgálatokat
> - gyors tájékozódásra, több szerv egymás utáni áttekintésére 
> - Terhes hölgyeknél betegségek, deformitások kizárása
> - Kvantitatív, kvalitatív szerv morfológiai és funkcionális vizsgálatok 
> - nem invazív
> - nincs káros biológiai hatása?! (Ellenjavallata nem ismert)
> - a beteg legtöbbször külön előkészítést nem igényel
> - nem kell idegen anyagot a betegbe juttatni a vizsgálathoz
> - az elváltozások belső szerkezetéről is ad pontos információt
> - széles körben hozzáférhető, egyszerű, „olcsó”
> - Nem ionizál -> gyermekekben, terhesekben előnyben részesítendő
> - Komplex vizsgáló módszer, légtartó csonttal fedett területek kivételével, minden szerv és szervrendszer vizsgálható.
> - Egyszerűen kivitelezhető → gyors, ismételhető
> - Gyorsasága miatt jól használható szűrésekhez: veleszületett csípőficam
>  
> ##### hátrányai
> - Közvetlen kontaktus a beteggel (kikérdezés, tapintás)
> - A bélgázok és a tüdőszövet akadályozzák a leképezést
> - Vizsgálófüggő, nehezen reprodukálható 
> - Műtermékek, pontatlan mérések
> - A kép sok esetben csak az ultrahang mérési pont ismeretében lehetséges

#### 3. Az ultrahangos képalkotás: A-mód, B-mód, M-mód, Doppler technikák
> ##### A-mód
> - Piezoelem, jel (hang) kibocsátás és fogadás
> - A visszaérkező jelet nézhetjük oszcilloszkópon
> - TGC – idő vétel kompenzáció (adott időablak kimaszkolása) 
>   - szöveti abszorpció hatásának kiküszöbölésére
>   
> ![](https://slidetodoc.com/presentation_image/fd81e2a20533eddb5c55c970c1380011/image-7.jpg)
> 
> ##### B-mód *(brightness modulation)*
> - Mint az A mód, csak fényességével jelenítünk meg. 
> - probléma a gömbszerű terjedés → interferencia!
> 
> *felhasználás:*
> - *vese vagy máj körvonalai*
> - *érfalak*
> - *vese üregrendszere*
> - *epehólyag bennéke*
> - *cisztában lévő folyadék és lágyrész közötti határ*
> - *májban elkülöníthetők az egyenletesen szétoszló és a gócos elváltozások*
> - *daganatos és ép szövetek határa*
> - *kontrasztanyag*
> - *intervenciók vezérlése: ciszta, tályog, aspiráció, biopszia, szervek mozgásjelenségei*
> 
> ![ultrasound b mode](https://radiologykey.com/wp-content/uploads/2016/03/B9781437714173000024_f02-08-9781437714173.jpg)
> 
> ##### M-mód (TM - Time Motion mód)
> Az  M-módú ábrázolás egyetlen B képbeli egyenes időbeli változásainak megjelenítése. (*pl: echokardiográfia*)
> 
> ![](https://ecgwaves.com/wp-content/uploads/2019/10/motion-m-mode-echocardiography-ultrasound-image-echo-1.jpg)
> 
> ##### Color Doppler, Power Doppler, Spektrum Doppler
> Ha a kibocsátott nyaláb hozzánk közeledő véráramról verődik vissza, nagyobb frekvenciát kapunk, mint amit kibocsátottunk, amennyiben tőlünk távolodik az áramlás, alacsonyabb frekvencia érkezik vissza.
> - Ha pontosan felénk vagy tőlünk el áramlik, akkor a legnagyobb a frekvencia változása
> - Csak a merőlegestől eltérő komponens mérhető
> - Ezzel tudjuk a vért megnézni folyásirányban
> 
> ![](https://pulseandprime.com/wp-content/uploads/2020/12/b4baef4e-036a-4172-88aa-f30c4c14f197.jpg)
> 
> - Megfigyelni: érszűkület, shunt, szöveti perfúzió
> - Erek térbeli elhelyezkedése, az egyes szervek vérellátása, a fejlődési rendellenességek és súlyosabb áramlási zavarok 
> - Alacsony vagy nagy ellenállású terület 
> 
> **Power Doppler:** nem az áramló sebesség nagysága, hanem az átáramló közeg tömege jelenítődik meg színskálán.

#### 4. Az ultrahangos képalkotás: 3D 4D, 3D leképezés/renderelési módok,
> **Leggyakoribb vizsgálati területek:**
> - hasi és kismedencei szervek
> - emlő
> - érrendszer
> - magzat
> - vázizom-rendszer, ízület
> 
> **3D**: Sok, egymás melletti 2D, azaz síkképet egymás mellé pakolva térbeli képet kaphatunk
> **4D**-ben időben változóvá tesszük (mozog)
> - Diagnosztikus pontosság, gyorsaság 
> - Reprodukálhatóság
> - Fotorealisztikus képi megjelenítés
> - *„Felületi, áttetsző, kevert”* vizsgálati mód
> - Néhány milliméteres képletek in vivo térbeli megjelenítése
> - Számos fejlődési rendellenesség korábban ismerhető fel
> 
> **3D volumetriás vizsgálatok**, 3D color histogram, 3D power doppler (szövetek, szervek szerkezetének, áramlási viszonyainak vizsgálatát teszik lehetővé)
> 
> ![2d vs 3d vs 4d](https://www.bloomingbaby.com/wp-content/uploads/2d3d4d_animated_MASTER.gif)

#### 5. Felületi képrekonstrukciók és ábrázolási módok, VCI, VOCAL
> **Felszíni (textúra) mód /Surface texture/** A felszín szöveti módon kerül ábrázolásra
> 
> **Felületi (elmosott) mód** A felszín kisimított, felszíni módban ábrázolódik
> 
> **Megvilágított mód** A felszín megvilágított módon kerül ábrázolásra
> 
> **Grádiens megvilágított mód** A felszín, mintha egy pontszerű fényforrásból lenne megvilágítva
> 
> **Maximum mód:** legnagyobb szürkeérték ábrázolása: csontstruktúrák
> 
> **Minimum mód:** legkisebb szürkeértékek ábrázolása: erek, folyadékkal telt üregek
> 
> **X-ray mód:** összes szürkeérték ábrázolása: szövetszaporulatok 
> 
> ##### VCI
> - Speciális 4D leképezési mód
> - A VOL- BOX-on belül, meghatározott „vastag” szelet-térfogaton belül, keskeny szeletek sokaságából történik a leképezés
> - Tökéletesíti a kontrasztfelbontást, kiváló jel-zaj viszony
> - Felület textúra mód és a transzparens maximum mód 70/30 %-os keverése + felület transzparens mód
> - Valós idejű  4D leképezés pszeudo 2D módban
> 
> ##### VOCAL
> - Automatikus kontúrfelismerés (6-120 síkban automatikusan méri a volument, függ az elforgatás szögétől, 9, 15, 30 fok)
> - Egy virtuális burok létrehozása az elváltozás körül. A burok falvastagsága meghatározható
> - A vascularisatio automatikus számítása a burkon belül a 3D színhisztogram segítségével
> - Daganatok pontos volumen mérése (Prostata, ovarium, endometrium, stb.)
> - Terápia tervezése, ellenőrzése
> - A legpontosabb térfogat számítási módszer

### X.Képalkotás 
#### 1. Lencsék tulajdonságai (szférikus, aszférikus, chromat/achromat)
> Fénytörés/refrakció
> - Nagyítás: `tárgylencse*szemlencse`
> - Mélységélesség: `z-tartomány`
> - Látómező: megvilágított kör szemlencsében, (~mm)
> - Munkatávolság: `objektív-fedőlemez táv`
> 
> ![](https://docplayer.hu/docs-images/43/6085367/images/page_4.jpg) 

#### 2. Felbontás és számolása, numerikus apertúra
> Felbontás `d = λ/2*NA [~µm]`
> 
> Numerikus apertúra:
>   `NA = n * sin (θ) [-]`
>    törésmutató növelése: 
>     - levegő: (1,000293)
>     - víz (1.33)
>     - glicerin (1.47)
>     - immerziós olaj (1.51)
>    NA 1 – 1.4 között (TIRF: akár 1.89 is!)
    
#### 3. Aberrációk a mikroszkópiában
> ![optical aberrations](https://cdn.dynasil.com/assets/optical-aberrations.jpg)
> 
> ![optical aberrations](https://www.handprint.com/ASTRO/IMG/spotdiag.gif)
> 
> - Szférikus aberráció
> - Kromatikus aberráció
> - Geometrikus aberráció
> - Asztigmatizmus
> - Üstököshiba

#### 4. Kamerák jellemzői és típusai
> Fizikai jelek átalakítása elektromos jellé:
>   Kamera: CCD: fényérzékeny cellákat tartalmazó áramköri lapka → beeső fényt érzékeli → elektromos töltésként továbbadja → áram
>   
>   Fény intenzitása ~ áramerősség
>   
>   1 fotocella → 1 pixel → felbontás
>   
> **Kicsi érzékenység:** mennyi jelet fogsz kapni a kameramodultól egy adott fényerő esetén `1 lux , 1 mp → ? e-` 
> Nagyobb fényerősséget érzékeli csak
> - Javítás: erősebb festés, érzékenyebb kamera
> - Nagy jel-zaj viszony
> - Elektromos jellé alakításkor
> - Zajjal telített kép keletkezik → pl.: salt & pepper
> 
> **Javítása:**
> - több kép átlagolása
> - Feltétel: időben álló kép
> - Erózió, dilatáció

#### 5. Nagyítás és számolása, fénytörés, Látómező, Mélységélesség, Munkatávolság
> Nagyítás: `tárgylencse*szemlencse`
> 
> Látómező: `megvilágított kör szemlencsében, (~mm)`
> 
> Munkatávolság: `objektív-fedőlemez táv`

### XI.Nagyfelbontású (fény)mikroszkópia I.
1. Airy minta
2. Modulációs átviteli függvény (MTF) 
3. A mikroszkópok főbb fajtái és jellemzőik
4. Az átmenőfényes mikroszkóp részei, elrendezése, működése
5. Az átmenőfényes mikroszkóp jellemzői, előnyei/hátrányai

### XII.Nagyfelbontású (fény)mikroszkópia II.
1. Huygens-Fresnel elv
2. A fluoreszcens mikroszkóp részei, elrendezése, működése
3. A fluoreszcens mikroszkóp jellemzői, előnyei/hátrányai
4. A sötétlátóteres (darkfield) mikroszkóp része, elrendezése, működése
5. A sötétlátóteres (darkfield) mikroszkóp jellemzői, előnyei/hátrányai

### XIII.Digitális mikroszkópia
1. A digitális mikroszkópia előnyei
2. Szuperrezolúció elve, működése, előnyei/hátrányai
3. A tárgylemez scanner felépítése,működése, előnyei/hátrányai
4. Szkennelési típusok
5. Mintavétel képek esetében (Nyquist)

### XIV.Képi adatok tárolása és menedzselése
1. Képtárolás fájl formátum szinten
2. Orvosi képalkotókból származó információk tárolásának problémái 
3. Metszeti síkok és képi orientáció
4. DICOM szabvány
5. PACS feladatai, felépítése



### fogalmak: 
- **1.	Spektroszkópia:** egy színkép megfigyelésének módszere
     - **1.1 Spektrometria:** nagy érzékenység, nagy pontosság, rendkívüli egyszerűsége, gyorsasága, kis anyagigény
- **2.	Spektrum:**
- **3.	abszorpciós spektroszkópia**
- **4.	emissziós spektroszkópia**
- **5.	rezonancia spektroszkópia**
- **6.	Fekete test**
- **7.	Abszorpciós tényező**
- **8.	Transzmissziós tényező **
- **9.	Reflexiós tényező**
- **10.	MIR - Mid InfraRed**  
- **11.	NIR – Near Infrared**  
- **12.	Termikus infrasugárzás-érzékelő:** infrasugárzás hatására felmelegszenek és ennek hatására valamelyik fizikai (villamos) paraméterük megváltózik, amiből pedig a szükséges villamos jel "kinyerhető„
- **13.	Foton-detektoros  infrasugárzás-érzékelő: ** fotonok számával arányos villamos jelet adnak, de működésükhöz mély hőmérsékletre való lehűtésük szükséges
- **14.	Termogram:** Hoterkep.
- **15.	termográfia: ** A termográfia (hőtérképezés) egy olyan funkcionális vizsgáló eljárás, amelynek során az emberi test hőmérsékletét mérjük infrakamerával egy erre a célra kifejlesztett számítógépes szoftver segítségével.
- **16.	CTI  - Computerised Thermal Imaging**
- **17.	Szkennelő hőkamera:** egyelemű ("pont"-) detektort használnak az infravörös sugárzás átalakítására és a mérendő tárgyat egy mechanikus rendszerrel tapogatják le
- **18.	Mátrixdetektoros hőkamera:** mechanikailag egyszerűbb, hőkép minden egyes képpontját egy-egy egyedi érzékelő alakítja át.
- **19.	hőszállító közeg:** Peldaul a ver. A szervekből jövő vénás vér hőmérséklete magasabb, mint az odaáramló artériás véré, bőrből és a tüdőből jövő pedig még alacsonyabb.
- **20.	fiziológiás testhőmérséklet:** A normal mukodes mellett merheto homerseklet(szajban mert adat).
- **21.	maghőmérséklet:** A belso szervekre jellemzo homerseklet. Ez magasabb nehany fokkal, mint a test felszinen merheto homerseklet.
- **22.	Invazív vizsgálat:** Olyan vizsgalat mely soran ver serken.
- **23.	Denzitás:** Valamilyen ertek suruseget fejezi ki adott dimenzioban.(EZT EN TALALTAM KI. FOGALMAZD AT!)
- **24.	Natív termográfia:** A test hősugarainak manipuláció nélküli vizsgálata. Szűrővizsgálatoknál elterjedten használják.
- **25.	Funkcionális termográfia/stressz termográfia:** Terhelés esetén, a test hőmérsékletében gyors változást tudunk elérni, mely lassan rendeződik vissza.
- **26.	Termogén:** (hideg illetve a meleg próba), melyhez használhatunk: vizet, alkoholt, levegőt, klóretilt, száraz jeget stb.
- **27.	Dinamikus termográfia:** Ez a módszer vagy folyamatos, vagy intermittáló felvételek készítéséből áll.
- **28.	Near Infrared Spectroscopy (NIRS)**
- **29.	hemodinamika**
- **30.	agyi O2 szaturáció**
- **31.	piezoelektromos kristály**
- **32.	A-mód:** Jel kibocsatas. Majd a visszaerkezo jelet oszcilloszkopon nezzuk.
- **33.	B-mód:** A visszaerkezo jelet szinesitve jelenitjuk meg. 
- **34.	M-mód:** B mod idobeli abrazolasa.
- **35.	TGC – idő vétel kompenzáció:** Hang terjedese szempontjabol azonos szoveteket. Tavolabbi szovetekrol kisebb jelek verodnek vissza mint a kozelebbiekrol. TGC az azonos tipusu szoveteknel azonos amplitudot eredmenyez.
- **36.	Color Doppler:** 
- **37.	Power Doppler:** nem az áramló sebesség nagysága, hanem az átáramló közeg tömege jelenítődik meg színskálán.
- **38.	Spektrum Doppler**
- **39.	transducer**
- **40.	Fotorealisztikus képi megjelenítés**
- **41.	Felületi/surface vizsgálati mód**
- **42.	Áttetsző/transzparens vizsgálati mód**
- **43.	Kevert vizsgálati mód**
- **44.	in vivo** szó szerinti jelentése: élőben
- **45.	in vitro** szó szerinti jelentése: üvegben. A kísérleti folyamat az élő szervezeten kívül (Petri-csészében, kémcsőben) zajlik le.
- **46.	in silico**
- **47.	volumen renderelés**
- **48.	ROI**
- **49.	orientáció**
- **50.	longitudinális**
- **51.	transzverzális**
- **52.	Horizontális**
- **53.	coronalis**
- **54.	axialis**
- **55.	anterior** 
- **56.	posterior** 
- **57.	cranialis** 
- **58.	caudalis** 
- **59.	Niche mód** 
- **60.	Felszíni (textúra) mód /Surface texture/:** Ultrahang - A felszín szöveti módon kerül ábrázolásra
- **61.	Felületi (elmosott) mód:** Ultrahang - A felszín kisimított, felszíni módban ábrázolódik.
- **62.	Megvilágított mód:** Ultrahang - A felszín megvilágított módon kerül ábrázolásra. 
- **63.	Grádiens megvilágított mód:** Ultrahang - A felszín, mintha egy pontszerű fényforrásból lenne megvilágítva.
- **64.	Maximum mód:** Ultrahang - Legnagyobb szürkeérték ábrázolása: csontstruktúrák.
- **65.	Minimum mód:** Ultrahang - Legkisebb szürkeértékek ábrázolása: erek, folyadékkal telt üregek.
- **66.	X-ray mód:** Ultrahang - Osszes szürkeérték ábrázolása: szövetszaporulatok.
- **67.	Transrectalis 3D vizsgálat**
- **68.	Transvaginalis  3D vizsgálat**
- **69.	Huygens elv**
- **70.	Huygens-Fresnel elv**
- **71.	diffrakció**
- **72.	Airy korong:** fénynyalábot nem lehet minden határon túl fókuszálni => egy elemi tárgypont képe elmosódott lesz => Airy korong => felbontás limit. Ez a legjobban fokuszalt pont.
- **73.	Airy minta:** Ha feny athalad egy nyilason mindig valamilyen mertekben meg fog torni. Igy a leheto legjobban fokuszalt pont kore is fog szorodni. Ezer nem lehet egy vegtelen kis pontba fokuszalni.
- **74.	PSF: Point Spread Functions**
- **75.	Rayleigh kritérium**
- **76.	Dawes kritérium**
- **77.	szuperrezolúció**
- **78.	Numerikus Apertúra:** A numerikus apertúra az optikai lencserendszerek fénygyűjtő képességének egység nélküli mérőszáma
- **79.	Térbeli felbontás:** A ternek az a legkisebb egysege amit meg meg tudunk kulonboztetni a levetult kepen.
- **80.	diffrakciós minta:** Ha egy hullam nyilason halad at, akkor megtorik es szorodik. Mintazat fog kirajzolodni a levetulesen, amik maximum es minimum erositesu helyek.
- **81.	Nyquist kritérium:** A felnyitott rendszernek nincs pizitiv valos reszu polusa, akkor stabil a zart rendszer.
- **82.	Modulációs átviteli függvény - MTF**
- **83.	Kondenzor apertúra**
*ezek kimaradtak:*
- **84.	DICOM - Digital Imaging and COmmunication in Medicine **
- **85.	MIME**
- **86.	PACS - Picture Archiving and Communications System**
- **87.	HL7- Health Level Seven**
- **88.	Electronic Health Record (EHR)**
- **89.	Personal Health Record (PHR)**


