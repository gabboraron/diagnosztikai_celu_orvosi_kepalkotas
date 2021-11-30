 # Diagnosztikai célú orvosi képalkotás

>
> ***Államvizsgás tárgy!***
> ## ZV tételek a tárgyból:
> - Röntgen
> - CT
> - OCT
> - MRI
> - PET
> - spektroszkopia
> - CTI
> - NIRS
> - UH
> - kép ábrázolás
> - nagyfelbontású mikroszkópia I
> - nagyfelbontású mikroszkópia II
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

- https://docplayer.net/amp/208626422-Context-recognition-by-wireless-sensing-a-comprehensive-survey.html
- https://sci-hub.se/https://doi.org/10.1145/3328918
- https://news.ncsu.edu/2019/08/wifi-to-track-indoor-odometry/

## EA-GY2
### Röntgen (Rtg)
Már a polgárháborúban is használták.

[NIBIB gov - How Do X-rays Work? ](https://www.youtube.com/watch?v=hTz_rGP4v9Y)

![röntgen spektrumok](https://www.biolegend.com/Files/Images/BioLegend/blog/100814blog/Spectrum.png)

egy sugarat kilövünk és azt mérjük, hogy hogyan csapódik be az atomokba és ott hogy törik meg, milyen "árnyékot" ad, a külféle spektrumokat könfélre finomságon használjuk.

Két vezetéket használvva ha az egyikbe nagy feszültséget kötünk akkor átvándorol a másikra, így mikor ezt bekapcsolva hagyta Röntgen, és azt próbálva jutott arra, hogy az anyagoknak van sugárzási együtthatója.

A `kilépő sugárintenzitás = belépő sugárzás * anyag sugárzási együtthatója ^ (sugárgyengítési együttható * anyag_vastagság)` 

[How does an X-ray Tube Work (Radiation Protection)](http://www.youtube.com/watch?v=Bc0eOjWkxpU)

A kollimátor használatótól függően meg tudjuk változtatni a sugárnyaláb méretét és kiterjedését is ![tipikus röntgen szögek anód esetén](https://www.mta-r.de/site/assets/files/9355/fig_5_6.png)

Ahol van szövet ott kisebb intenzitással megy át, ahol nincs ott nagyobbal.

![the five main daiodensities ona standard radiograph](https://veteriankey.com/wp-content/uploads/2016/05/B9781455703647000053_f005-002-9781455703647.jpg)

Az infra fény áthatol a szöveten.

**felhasználása:**
- Mammography
- X-ray radiography
- Fluoroscopy (kontrasztos)
- Radiation therapy in cancer treatment

> Egy röntgencső a legegyszerűbb kivitelnél egy katódból és egy anódból áll, amik egy üvegburában vannak légmentesen lezárva.

## Computer tomográfia (CT)
http://www.impactscan.org/#ctdose
> gyakorlatilag röntgen

**használható:**
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

Röntgennél a röntgencsőből a sugárkapunk lépnek ki a sugarak ahol tudjuk változtatni a sugár irányát és nagyságát.
- oszcintillációs: a detektor ért sugarak felvillanásokat okoznak a fotodetektorral ezt érzékelik. Jellemzői a mechanikai stabilitás, kis méret, alacsony tápfeszültség, modulárisan cserélhető.
- ionizációs detektorok:
  - nemesgáz töltés esetén az ionizált gáz áramot gerjeszt és a keletkező jelenséget rögzíthetjük.

**alkotó részei:**
- adatgyűjtő rendszer: analóg jeleket jelerősítéssel mintavételt alkalmazok
- páciens asztal: stabil és ~1mm pontosságú
- nagyfeszültségű generátor: 12-140 kV, 80-400mA, 50-60kW háromfázisú
- vezérlőpult
- számítógép ami menti az adatokat és összeállíŧja a képet

### Röntgen vs CT
| röntgen        | CT           |
| ------------- |:-------------:|
|       | rosszabb térbeli felbontás, lényegesen jobb kontrasztfelbontás |


Képminőség:
- fantomokkal mérhető, hogy jól van-e bekalibrálva, térbeli speciális fantommal mérik
- vonalpár/cm
- függ:
  -  a detektor méretétpt
  - a páciens méretétől, mert változik a fókuszpont

#### CT generációk
![egyben](https://www.researchgate.net/profile/Emanuele-Mikhaeil/publication/343193759/figure/fig1/AS:916910753476608@1595619967129/Generations-of-CT-scanners-6.png)

> minőségi vizsonyokról ad visszacsatolást

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
> ![3th gen ct](http://www.impactscan.org/slides/impactcourse/basic_principles_of_ct/img26.gif)

> **4. gen CT**
> 
> - gyűrű műtermékek eliminálása => nem egy kört okoz egy rossz pixel hanem 1 pontot
> - 4800 detektor
> - csak a sugárforrás forog, detektorokkal rajtuk körbe
>
> ![4th gen ct](http://www.impactscan.org/slides/impactcourse/basic_principles_of_ct/img27.gif)

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
> http://mriquestions.com/index.html

Hidrogén protonokat egy irányba állítunk amiket ha bárhol megváltoztatunk akkor az feltűnő lesz, ezt egy sugárral és egy rf antennával érzékelhetem
- homogén mágneses tér
- alagút típusúba betesszük a mukit vagy félig nyitottnál nem olyan jó a képmínőség. Alagútasnál 1; 1,5; 3; 7 teslásat is előállíthatunk.

![mri szerkezet](https://mersz.hu/mod/object.php?objazonosito=m538it_541_i1_idx)
![mri szerkezete 2](https://cms.sulinet.hu/get/d/45d45d68-1d9c-4e3f-ab81-6c3715093917/1/1/b/Normal/normal.png)

![mri struct](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS1G0xq7rXmsuFvTqW8tQ5Pjtdun1y9x8_OOQ&usqp=CAU)

[YouTube K-Space: A way to understand how MRI parameters affect images](https://www.youtube.com/watch?v=QHtZR0mtB80)

- Diffúziós MRI ami valaminek a folyamatát tudja monitorizálni. 
- [Tractographya](http://trackvis.org/) valaminek az útvonalait adja vissza.

> Nagy mágnesességű (tesla nagyság) párhuzamos elektormágnes tekercsekkel létrehozunk egy elektromágneses mezőt, ahol a szövetben levő hidrogén atomok protonjait egy irányba rendezzük (hidrogén mag polarizálása) homogén mágneses mező létrehozásával. Ugyanis a protonok mágneses térben képesek elektromágneses energiát befogadni és kiadni ellenben nyugalmi állapotban a protonok mágneses tulajdonsága véletlen eloszlású.
> 
> E mellett egy gyengébb, időben változó (1 kHz nagyságrendű), téri kódoláshoz szükséges, ún. gradiens mezőt is létrehozunk. E mellett egy gyenge rádiófrekvenciás (RF) mező, mely egy RF antennán keresztül összegyűjthető, mérhető jelek produkálását lehetővé tevő manipulációjára képes a hidrogénmagoknak. Ezek a mágneses térre merőletges jelek, melyek kitérítik a protonokat. A gerjesztés után (adott Hz H:64) mérhetőek a kitérés (elektromágneses energia leadásának) komponensei
>
> A három gradiens tekercs a főbb irányok felé van állítva, így létrejön a térbeli lefedettség.
> 
> - A mágneses tér erőssége nagyban meghatározza a kinyerhető jel erősségét
> - Rádióhullámok segítségével közlünk energiát, és a kapott „visszhangot” rögzítjük
>
> Ezeket az adatokat vizualizálhatjuk valós vagy imaginárius értékek mentén, de fázis vagy amplitúdó alapján is lehet. Ugyanakkor a gyakorlatban ezen a ponton Fourier transzformálunk, hogy a frekvenciát elemezzük. Ezt terjeszthetjük ki 2D-be, úgy, hogy a jeleket egymás mellé téve értelmezzük, és így kapunk egy 2D szeletet. Ezt kibővítjük 3D-re tomográfiával, azaz egymás mellé tesszük a szeleket.


## fMRI
A kifejezetten agyra kitalált kontrasztos MRI.

## DWI
> Kiemeli azon részét az MRI-nek ahol nem jó a nedvesség.

## Hyperfine
mobil MRI készülék https://hyperfine.io/

# PET
> Pozitron emisszós tomográfia
>
> Mennyiségi viszonyokat ad meg, mennyi van az adott szövetből.
>
> Egy sugárzó anyagot adunk be amit mérünk és a mérések alapján készítünk képet, ezzel folyamatokat lehet monitorizálni, keringési problémát, agyi, vagy daganatos jelenségeket figyelünk.
> 
> ~ 11mSv egység
> 
> Ha az alanyt egy csőszeletben helyezzük el akkor a mérés közben a a kilövelő beta részécskéket egy szenzoron érzékeljük, amikor beérkezett megnézzük, hogy az átelmmeben levő oldalon az átmérő fénysebeségel való átfutási idejével megegyező időn belül lesz-e becsapódás, ha lesz akkor tudunk képet készíteni, 2D szeletben.
>
> ![](https://www.researchgate.net/publication/337325700/figure/fig1/AS:826576459530243@1574082593894/The-basic-principle-of-a-positron-emission-tomography-PET-system-A-PET-detector-ring.png)![](https://www.researchgate.net/publication/342053802/figure/fig1/AS:902008584294400@1592067013365/Positron-Emission-Tomography-PET-imaging-a-neutron-deficient-radioisotope-positron.png)
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
> SUV - szöveti uni
> 
> SPECT - single photoemission PET  
> 
> ![](http://www.eventideib.polimi.it/wp-content/uploads/2019/05/PastedGraphic-1-730x410.png)![](https://ars.els-cdn.com/content/image/1-s2.0-S1120179715010492-ejmp619-fig-0001.jpg)


# OCT
![OCT VS MRI VS CT](http://obel.ee.uwa.edu.au/wp-content/uploads/2015/01/Fig_3_OCTcomparison.png)
használt:
- bőrgyógyászatban
- megtudom mondani melyik irányban áramlik a vér
- 

> fény alapú koherens tomográfia
> 
> Michlson féle interfenercia mérő az interfeernciát méri, egy visszaveréssel tud dolgozni ami alapján távolságokat lehet látni
>
> SLED/LED - 800--1300-1550 nm hullámhosszal
> 
> 5-10-30 fpses feptosecundumos laser
> 
> 4-5mm mélyen mérhető a szövet
>
> - erő és távolság mérésre is használható, az üveg (*amiben megy a jel*) törési mutatójának segíŧségével
> - amikor a szemben a nyomás lecsökken beomlik a retina és részleges vaksáág áll elő
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
- a szövet áteresztőkpességén / törésmutatóján múlik az ltrahang működőképessége, ez levegeőben rossz, ezért pl tüdőt/csontot nem lehet
- a képben keletkező levegőbuborékok a műtermékek
- külöünféle ultrahang vizsgálatnál különféle fejekkel különböző mélységig vizsgálni a szövetben, így egy tárgy-transducer távolság kétszeresét nézzzük

![](http://www.sprawls.org/ppmi2/USPRO/usimage2.JPG)

A hagnhullámnál mini terjedések kezdenek kialakulni.
mindezt egy piezoelektomos jellel tudom megtenni.

Az oszcilloszkópon megjelenik a visszajövő jel az A scan

A térrész minden eleméhez rendelek egy értéket és attól függően mikor ér vissza onnan a jel adok hozzá színt 0-255 tartományon. a legmesszebbi a legsötétebb a legközelebbi a fehér. Ez a **B mód**.

Ha több B módú scant öszetsszük kapjuk az Mmódút.

Dopler hatáson alapszik, így akár folyamatokat is láthatunk, hogy merre folyik a vér.
- ha kiküldök egy frekvenciát és a visszapattanó nagyobb akkor jön fleém
- ha a visszapattanó kisebb akkor megy elfele

https://piurimaging.com/

- felsíni, textúra mód
- elmosott mód
- megvilágított mód
- maximum/minmum mód
- x-ray mód

használata:
- daganatok pontos volumen mérse, stb
- transrectális, transvaginalis ultrahang

## Optika, mikroszkópia
> Képalkotás, optikai tartományban, mik a lencse hibák, mivel korrigálhatóak, stb.
>
> Megvilágítás, milyen a mikroszkóp beli megvilágítás, milyen előfeldolgozás lehetséges, festés, dlc, hoffmann, fázis, sötét látóteres mikroszkóp.


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
- numerikus pertúra: a lecse fénygyűjtő képessége, jele *NA*, az olajé a legjobb
- felbontása, jele *`d = lambda/2*NA`[~micro m]*
- mélységélesség *z-tartomány*
- látómező: megvilágított kör szemlencsében [~mm]
- munkatávolság: objektív-fedőlemez táv

![objektív](http://www.bwoptics.com/html/UploadFile/201056846928.jpg)

- szférikus aberráció: ![szférikus aberráció](https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/Spherical_aberration_2.svg/1024px-Spherical_aberration_2.svg.png)
  a lencse nem meg  fókuszpontba öszpontosít
- kromatikus aberráció: ![kromatikus aberráció](https://digiretus.hu/wp-content/uploads/2017/12/photoshop-szinhiba-eltavolitasa-6.jpg)
  másképp töri meg a fénysugarakat, és a színek kettéválnak
  **javítása: ** a lencse állíása mert nem jó pontban van
- képmezőelhajlás/mezgörbület
  ![képmezőelhajlás](https://docplayer.hu/docs-images/59/43658178/images/21-0.png)
  **javítása: ** digitálisan szoorzzuk egy korrekciós mátrixszal
- asztigmatizmus ![asztigmatizmus](http://autosjatekok.co.hu/images/lts-lesen-esett-az-asztigmatizmus.jpg)
  **javítása: ** növeljük a látómezőt
- üstököshiba: ![üstököshiba](https://cdn-60a62604c1ac1c1d10df7525.closte.com/wp-content/uploads/sites/321/2010/12/v_o_koma_hiba.png)
  **javítása: ** több lencsét tudunk használni

## nagyfelbontású fénymikroszkópia I.
- Lézer: koncentrált fénnyaláb, leadja az energiatöbbletet, ezt kezeljük fotonként,
A fény mindenképpp szinuszosan moszog!

Hullmámhossz egyensen arányos a frekvenciával.
 
**Huygens elv:** körhullám -> hullámtér -> minden egye pont egy-egy egyedi hullámforssának tekinthető -> ezek széle egy gömbhullám amin van a hullámgörbe

**Fresnel elv:** ezek a köthulllámok interferálnak, és ezeke eredője adja meg milyen az egész fényünk.

Étendue: geometriai kiterjedés.
         - https://en.wikipedia.org/wiki/Etendue

**fázis konjugált tükrök: ** visszatükrözi sé folymatosan normalizálja az Étenduet

Festési eljárások:
- hematoxifin: mivel savas ezért a sejtmagokhoz ideális
- eosin: bázikus, pl citoplazmához való.

**kotrasztosíás**
- kvalitatív 3D fotografikus
- 2x prizma, fény polarizálása
- analizátor: fáisretardáció, fénnyaláb rekombinálása
- DIC
- Hoffmann modulációs kontraszt mikroszkóp: aaz aperturán lévő lyukakkal állítja a éfny mennyiségét, és így csökkenti a glória hatást.
- fázisrárgy: a féyn amplitúdóján lehet ávltoztatni, ezzel fáziskontraszt mikroszkópot alakíthatnunk ki, át állítjuk a fény mennnyisgét, a kondenzátor egységesíti, de a fázisát beállíottuk, így csak a kontúrok jelennek meg.

**sötétlátóteres mikrszkóp:** kolloid mintáknál lehet használni, tegár kéepsek a fényt szórni, és mi ezt a szórt féynt látjuk a végén. Mindent mai mikrométers tartományba esik és festetlen alalmas rá.

## mediso
egyedül nekik van 3 fejő MRük

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
> 1. *dichroicus* tükörrel megtörjük a fényt de csak az adott hullámhosszon, amit egy *excitation* szűrővel szűrünk, visszajuttatjuk a tükörnek az objektí@en keresztül majd a másik hullámhosszon amit már a tükör átenged és ez jut az oculárba.
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
> **Lumineszencia:** gerjesztés után elindul a relaksázciós folyamat
>
> **foszfor esszencia:** olyan állapotokba is belép az leketron amikbe ha önmagában lenne nem lépne be.
>
> ![konfokális mikroszkóp](https://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/Confocalprinciple_in_English.svg/1024px-Confocalprinciple_in_English.svg.png)
>
> Ezzel kiküszöböljük a nem képsíkból érkező nyalábokat. Ezért pásztáznunk kell, mivel ekkor egy pontból kapunk fénnyalábokat.
>
> - vízszintes ~ 200 nm
> - függőleges ~ 500 nm -> baktérium vírsu vizsgálata
> -> xy-sík

### STED: Stimulált emissziós kioltáso mikrozkóp
> Kontra fényeketi nddítunk melyek hullámhossza kioltja a megjelenő fényt és ezzel pásztázunk így az adott ponthoz pontos értéket tudunk mondani.
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
> Alapjelenség: alagút effektus: szubnanonméteres távolságra levő potenciál különbséggel rendlekező pontok között az elektronok csak egy nagy valószínűséggel jellemzett "scatornán" keresztül közledhetnek
>
> működés: feszültséget adunk a rendszerre, ezért a minta elkezd mozogni, a mintára lézerfényt vetítünk, ami visszaverődik egy tükörre amin mérjk a fény mennyiségét, és így tudjuk mérni a fizikai felületünk felszínét.
>
> felbontás: ~ 1nm -> molekulák szintje

## Digitális mikroszkópia III.
> Képalkotás érzékelt jelek feldolgozásával alkaítunk ki látzható digitális képeket
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
> - alacsoiny bitmélység: kvantáláskor
> - adott pixel intenzitás mennyi bittel írható le, kontraszt elveszhet, javítás: több biten tárolunk.

## 0,1 THz inpulzusos sugárzás mérés
elektrooptikai mintavételező

> Revolutionary enhancement of visibility by exploring active light fields
- kis energia
- alkalmas spektroszkópiához is
- biztosnágtechniaki alkalmazása
- belemegy az anyagba

## UWB radar alapú képalkotás
- kis impulzusok
- rövid dieig
- nagy energiát ad át
- camero tech 

## spektroszkópia
- 

## Beadandó - Mikroszkóp építés
- [I made a scanning laser microscope](https://www.youtube.com/watch?v=9TYlQ4urcg8)
- https://openflexure.org/
