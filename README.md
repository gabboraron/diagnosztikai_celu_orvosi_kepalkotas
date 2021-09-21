 # Diagnosztikai célú orvosi képalkotás

>
> ***Államvizsgás tárgy!***
>

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
- digitek/kvantált sázmjegyek írják le
- 2d kép elemi egyésge a pixel
- felbontás: kép méret (szélességx hosszúság pixelben)
- színmélység bitben mérve
- színtér (RGB, CMYK, HSV, HSL)
- fájlformátumok

### 3D képeken
- elemi egysége: voxel
- térrész homogén 3 tengelyű kiterjedéssel rendlekezik, egyszínű


beadndóhoz:

https://docplayer.net/amp/208626422-Context-recognition-by-wireless-sensing-a-comprehensive-survey.html

https://sci-hub.se/https://doi.org/10.1145/3328918

https://news.ncsu.edu/2019/08/wifi-to-track-indoor-odometry/

## EA-GY2
### Röntgen (Rtg)
Már a polgárháborúban is használták.

![röntgen spektrumok](https://www.biolegend.com/Files/Images/BioLegend/blog/100814blog/Spectrum.png)

egy sugaarat kilövünk és azt mérjük, hogy hogyan csapódik be az atomokba és ott hogy törik meg, milyen "árnyékot" ad, a külféle spektrumokat könfélre finomságon használjuk.

Két vezetéket használvva ha az egyikbe nagy feszültséget kötünk akkor átvándorol a másikra, így mikor ezt bekapcsolva hagyta Röntgen, és azt próbálva jutott arra, hogy az anyagoknak van sugárzási együtthatója.

A `kilépő sugárintenzitás = belépő sugárzás * anyag sugárzási együtthatója ^ (sugárgyengítési együttható * anyag_vastagság)` 

[How does an X-ray Tube Work (Radiation Protection)](http://www.youtube.com/watch?v=Bc0eOjWkxpU)

A kollimátor használatótól függően meg tudjuk változtatni a sugárnyaláb méretét és kiterjedését is (tipikus röntgen szögek anód esetén)[https://www.mta-r.de/site/assets/files/9355/fig_5_6.png]

Ahol van szövet ott kisebb intenzitással megy át, ahol nincs ott nagyal.

![the five main daiodensities ona standard radiograph](https://veteriankey.com/wp-content/uploads/2016/05/B9781455703647000053_f005-002-9781455703647.jpg)

Az infra fény áthatol a szöveten.

## Computer tomográfia (CT)
- röntgen
- MRI-vel
- PET-tel

Radon találta ki 1917-ben

Egy testet `n` irányból lövünk meg röntgen sugárral ami `n` db egyenletet sé `n-1` ismeretlent jelentjelent a mi esetünkben tehát a feladat megoldható.

![Handsfield unit](https://ars.els-cdn.com/content/image/1-s2.0-B9780444534859000015-f01-01-9780444534859.jpg)

![handsfield séma](https://prod-images-static.radiopaedia.org/images/52608436/ffb5a7e3ebb12255dec689e924ddbd_jumbo.jpeg)


Kiszámolod az adott térrész sugárggyengítési értékét és azt hozzárendelem egy szürke képhez.

- lineáris tomográfia - ez a tomográfia legalapvetőbb formája
- poli tomográfia - geometriks mozgásokkal képalkotás
- zonográfia - ez a lineáris tomográfia változata

A tomogramm egy sugárgyengítési együtthatóval csinál egy képet, a sok képből létrehoz egy 3D objektumot szeletenként.

A 3D képhez minden 2D képen keresünk közös beazonosítható közös pontot, hogy térbeli koordinátát nyerjünk.

Röntgennél a röntgencsőből a sugárkapunk lépnek kia a sugarak ahol tudjuk változtatni a sugár irányát és nagyságát.
- szcintillációs: a detektor ért sugarak felvillanásokat okoznak a fotodetektorral ezt érzékelik. Jellemzői a mechanikai stabilitás, kis méret, alacsony tápfeszültség, modulárisan cserélhető.
- ionizációs detektorok:
  - nemesgáz töltés esetén az ionizált gáz áramot gerjeszt és a keletkező jelenséget rögzíthetjük.

alkotó részei:
- adatgyűjtő rendszer: analóg jeleket jelerősítéssel mintavételt alkalmazok
- páciens asztal: stabil és ~1mm pontosságú
- nagyfeszültségű generátor: 12-140 kV, 80-400mA, 50-60kW háromfázisú
- vezérlőpult
- számítógép ami menti az adatokat és összeállíŧja a képet

### Röntgen vs CT
| röntgen        | CT           |
| ------------- |:-------------:|
|       | jobb térbeli felbontás, lényegesne jobb kontrastfelbontás |
|       |       |
|  |       |

Képminőség:
- fantomokkal mérhető, hogy jól van-e bekalibrálva, térbeli speciális fantommal mérik
- vonalpár/cm
- függ:
  -  a detektor méretétpt
  - a páciens méretétől, mert változik a fókuszpont

#### CT generációk
![egyben](https://www.researchgate.net/profile/Emanuele-Mikhaeil/publication/343193759/figure/fig1/AS:916910753476608@1595619967129/Generations-of-CT-scanners-6.png)

>**1. gen CT***
>
> csak két párhuzamos röntgen detektor, végigszkennelte, arrépp ment
> 
> ![1st gen ct](https://radiologykey.com/wp-content/uploads/2016/02/B9780323069748100165_f16-03ad-9780323069748.jpg)

> **2. gen CT**
> 
> 30 detektor, 600 sugár x 540 négyzet, 18 szelet

> **3. gen CT**
>
> - több mint 800 detektor, tlejes testes besugárzás, forog a test körül a fej.
> - röntgencső és detektor mechanikailag egybefüggő egység
> => egy rossz pixel egy teljes kört alkot a kész képen amit eliminálni kell
> - a sugárforrás és a adetektorok is forognak
> 
> ![3th gen ct](https://lh3.googleusercontent.com/proxy/TUNuTmgeiySQUj4_OQK64aJXPdHNMbkaMhRKADiGGXIOPzRJgdxgus_DFxhLOoOQaNdAaWC4cvH25SWoyJeTQiYtrHbGX7LHpQw)

> **4. gen CT**
> 
> - gyűrű műtermékek eliminálása => nem egy kört okoz egy rossz pixel hanem 1 pontot
> - 4800 detektor
> - csak a sugárforrás forog, detektorokkal rajtuk körbe
>
> ![4th gen ct](https://lh3.googleusercontent.com/proxy/XSv3qbU6x72V0jlg8jWM5h_rv5pgvGpXUxgRAwW8N1udq2hOUppdknvW5WQKQn2tbwTCQ7yJNdJ3oz2qEvDY3bDgkB1HG9LsjSo)

## CTA (computed tomography angiography)
CT amivel ereket figylenek meg.
- kontraszt anyagos CT

Sugárterhelése (mSv-ben):
- CT koponya - 3.8
- vese - 4.6
- vastagbél - 7.4
- CT egésztest - 8.2
A Föld népessége  átlagosan évente 2,4 mSV sugárterhelést kap

# MRI
Hidrogén protonokat egy irányba állítunk amiket ha bárhol megváltoztatunk akkor az feltűnő lesz, ezt egy sugárral és egy rf antennával érzékelhetem
- homogén mágneses tér
- alagút típusúba betesszük a mukit vagy félig nyitottnál nem olyan jó a képmínőség. Alagútasnál 1; 1,5; 3; 7 teslásat is előállíthatunk.

![mri szerkezet](https://mersz.hu/mod/object.php?objazonosito=m538it_541_i1_idx)
![mri szerkezete 2](https://cms.sulinet.hu/get/d/45d45d68-1d9c-4e3f-ab81-6c3715093917/1/1/b/Normal/normal.png)

![mri struct](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS1G0xq7rXmsuFvTqW8tQ5Pjtdun1y9x8_OOQ&usqp=CAU)


