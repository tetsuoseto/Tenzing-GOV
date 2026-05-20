###@ Milyen általános célú AI-rendszerek léteznek?

A többcélú (general-purpose) mesterséges intelligencia rendszerek olyan szoftverprogramok, amelyek nagy mennyiségű adatokból tanulnak mintázatokat, ezáltal képesek számos feladat elvégzésére, nem pedig egyetlen konkrét funkcióra vagy szakterületre vannak specializálva (lásd az 1.1. táblázatot). E rendszerek létrehozásához az AI-fejlesztők egy több lépcsőből álló folyamatot hajtanak végre, amely jelentős számítási erőforrásokat, nagy adatkészleteket és szakosodott szakértelmet igényel (lásd az 1.2. táblázatot). A számítási erőforrásokra (gyakran „compute”-ként rövidítik) szükség van mind az AI-rendszerek fejlesztéséhez, mind pedig a bevezetésükhöz, és ide tartoznak a speciális számítógépes chipek, valamint azok futtatásához szükséges szoftverek és infrastruktúra.† Mivel nagy, sokféle adatkészleteken képezik ki őket, a többcélú AI rendszerek számos különböző feladatot képesek elvégezni, például szövegek összefoglalását, képek generálását vagy számítógépes kód írását. Ez a szakasz bemutatja, hogyan készülnek a többcélú AI rendszerek, mik azok a „reasoning” modellek, és hogy a szakpolitikai döntések miként alakítják a többcélú AI-rendszerek fejlesztését.

    Megjegyzés † -- A „compute” kifejezés a processzor által elvégezhető számítások számának mérésére is utalhat (jellemzően lebegőpontos műveletek per másodpercben mérve), illetve konkrétan azokra a hardverekre is (például grafikusfeldolgozó egységekre), amelyek ezeket a számításokat végzik.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Nyelvrendszerek
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- A parancs (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Képgenerátorok
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videógenerátorok
- Kozmosz (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotika és navigációs rendszerek
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ A biomolekuláris struktúrák különböző osztályainak előrejelzői
- AlphaFold 3 (‡27)
- Amplify (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI-ügynökök
- AlphaEvolve (‡31*)
- ChatGPT Agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Az AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Táblázat 1.1: Általános célú mesterséges intelligencia típusok
>white|black||9|11|br Többféle általános célú AI létezik. Ebben a Jelentésben azokat a modelleket tekintjük „általános célú” AI-nak, amelyek különböző osztályú molekulákra képesek strukturális információt előre jelezni, mivel sokféle feladatra alkalmazhatók. Például a fehérjeszerkezet előrejelzésére betanított modellek számos más feladatra is alkalmazhatók, például fehérjeinterakciók előrejelzésére, kis molekulák kötőhelyeinek előrejelzésére, valamint ciklikus peptidek (‡40) előrejelzésére és tervezésére.


>white|orangered|left|13|15|bb A mélytanulás az általános célú mesterséges intelligencia alapja

A kutatók általános célú AI modelleket építenek egy „deep learning” (mélytanulás) nevű folyamattal, amely a modelleket példákból való tanulásra képzi (‡41). A szoftvermérnökségtől eltérően a mélytanuló modellek adatból tanulják meg a feladatok elvégzését, nem pedig kézzel írt utasításokra támaszkodnak. Nagy mennyiségű adaton, például képeken, szövegen vagy hangon végzett feldolgozás révén ezek a modellek olyan módszereket fedeznek fel az adatok reprezentálására, amelyek belső reprezentációkat hoznak létre a mintákról (például alakzatokról, szókacsolatokról vagy hangstruktúrákról), és amelyek segítik a modellt a kapcsolatok felismerésében, valamint olyan kimenetek előállításában, amelyek összhangban állnak a modell tanulási céljával. Ezután a megtanult belső reprezentációkat absztrakt jellemzőkként használják az új, hasonló adatok elemzésére, illetve az adott stílushoz illeszkedő kimenetek generálására. Például egy általános célú AI modell, amely kellően sok példa alapján tanult a 19. századi romantikus angol költészetből, képes felismerni az ebben a stílusban írt új verseket, és az azokéhoz hasonló stílusban új anyagot tud létrehozni.

Részletesebb szinten a mélytanulás úgy működik, hogy a tanulógépes adatok feldolgozása összekapcsolt információfeldolgozó csomópontok rétegein keresztül történik. Ezeket a csomópontokat gyakran „idegsejteknek” nevezik, mert laza módon a biológiai agy idegsejtjei ihlették őket („neurális hálózatok”) (Ábra 1.1) (‡42). Ahogy az információ egy idegsejt-rétegből a következőbe áramlik, a modell fokozatosan alakítja át az adatokat egyre absztraktabb reprezentációkká, mint például a megtanult jellemzők csoportjai – olyan minták, amelyeket a modell automatikusan fedezett fel az adatokban, nem pedig kézzel kódoltak. Például egy képfeldolgozó modellben az első rétegek olyan egyszerű jellemzőket tanulhatnak meg észlelni, mint a kontúrok vagy az alapvető alakzatok, míg a mélyebb rétegek ezeket a jellemzőket kombinálva az olyan összetettebb mintákat emelik ki, mint az arcok vagy objektumok.

Az összes rétegben a jellemzők a betanítási eljárást meghatározó optimalizálási folyamat során kerülnek felfedezésre. A tanítás során, amikor a modell hibázik, a mélytanulási algoritmusok a neuronok közötti különböző kapcsolatok erősségét úgy hangolják, hogy javítsák a modell teljesítményét. Az egyes csomópontok közötti kapcsolat erősségét gyakran „súlynak” nevezik. Ez a rétegzett megközelítés adja a mélytanulás nevét.

A mélytanulás bebizonyította, hogy rendkívül hatékonyan teszi lehetővé az AI-rendszerek számára olyan feladatok elvégzését, amelyeket korábban a hagyományos, kézzel programozott számítási rendszerek és más korábbi szimbolikus vagy szabályalapú AI-módszerek számára nehéznek tartottak. A legkorszerűbb, általános célú AI-modelljeink többsége ma egy „transzformer” néven ismert, meghatározott neurális hálózati architektúrára épül (‡43, ‡44). A transzformerek egy „figyelmi” mechanizmust („attention”) használnak (‡45), amely segít a modellnek abban, hogy az információfeldolgozás során a bemeneti adatok szempontjából legrelevánsabb részeire összpontosítson, például annak meghatározásában, hogy egy mondat mely szavai a legfontosabbak a jelentésének megértéséhez. Az ilyen módon felépített modellekhez jelentős javulás társult a fordítás (‡43), a természetes nyelvfeldolgozás (‡46), a képfelismerés (‡47) és a beszédfelismerés (‡48, ‡49) területén, ami végső soron a mai, legfejlettebb modellek kifejlesztéséhez vezetett.

![fig1.1](images/fig1.1_neural_network.png)

##### Ábra 1.1: A ‘neurális hálózat’ illusztratív ábrázolása
>white|black||9|11|br A mai általános célú AI modellek ezekre a hálózatokra épülnek, amelyek lazán a biológiai agyak ihletését tükrözik. Különböző hálózatoknak eltérő méretük és architektúrájuk van. Mindazonáltal mindegyik olyan, egymással összekapcsolt információfeldolgozó egységekből áll, amelyeket „neuronoknak” neveznek, ahol a neuronok közötti kapcsolatok erősségét „súlyoknak” nevezik. A súlyokat a betanítás során frissítik nagy mennyiségű adaton keresztül. Forrás: International AI Safety Report 2025 (‡50) (módosítva).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Ábra 1.2: A többcélú mesterséges intelligencia fejlesztésének szakaszait bemutató vázlatos ábra
>white|black|left|9|11|br Nemzetközi AI-biztonsági jelentés 2026.


>white|orangered|left|13|15|bb Az általános célú mesterséges intelligencia szakaszokban kerül kifejlesztésre.

Általános célú AI rendszer kifejlesztése több szakaszból áll: az induló modelltanítástól a kihelyezés utáni felügyeletig és frissítésekig (1.2. Ábra). A gyakorlatban ezek a lépések gyakran egymással átfedésben, iteratív módon zajlanak. Minden szakasz eltérő erőforrás-befektetést igényel (pl. adatok, munkaerő, számítási kapacitás), valamint eltérő technikákat, és néha különböző fejlesztők végzik őket (1.2. Ábra és 1.2. Táblázat).

Például a modell-előtanítás általában jelentős mennyiségű számítási erőforrást és adatot igényel, ezért ez a szakasz különösen érzékeny azokat a politikákat illetően, amelyek befolyásolják a számítási erőforrásokhoz vagy a képzési adatokhoz való hozzáférést (‡51, ‡52). Hasonlóképpen, az adatkészítés és egyes modellek finomhangolási módszerei jelenleg nagy mennyiségű emberi munkát igényelnek a kezdeti adatrögzítéshez (‡53). Ezért ez a szakasz érzékeny a munkaerőköltségek, a platformokra vonatkozó politikák vagy a határokon átnyúló szerződéskötési megállapodásokat érintő szabályozások változásaira.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Adatgyűjtés és feldolgozás
> 
  Mielőtt egy általános célú AI modellt betanítanának, a fejlesztők és az adatszakemberek összegyűjtik, megtisztítják, válogatják és egységesítik a nyers betanítási adatokat olyan formátumba, amelyből a modell tanulni tud. Ez munkaigényes folyamat lehet. A legkorszerűbb modellek mögött álló betanítási adathalmazok az internet egészéről származó példák óriási számát foglalják magukban.
  A csapatok gyakran kifinomult szűrési módszereket fejlesztenek ki, hogy csökkentsék a káros tartalmakat, kiküszöböljék a duplikált adatokat, és javítsák a reprezentációt különböző témák és források között (‡54, ‡55). Az adatkezelés abban is segíthet, hogy csökkenjen a szerzői jogi és adatvédelmi jogsértések száma, eltávolítsák a veszélyes ismereteket tartalmazó példákat, kezeljék a több nyelvet, és javítsák az adatok származásának dokumentálását (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Előtanítás (a képzés első szakasza)

  A betanítás előtti szakaszban a fejlesztők a modellekbe hatalmas mennyiségű, sokféle adatot táplálnak be, hogy széles körű ismeretanyagot és kontextuális megértést sajátítsanak el. Ez a folyamat létrehoz egy „alapmodellt”. Ez egy rendkívül adat- és számításigényes folyamat.

  A betanítás (pre-training) során a modelleket milliárd vagy akár billió példának teszik ki olyan tartalmakból, mint képek, szövegek vagy hanganyagok. Ennek a kitettségnek a révén a modell fokozatosan felfedezi azokat a reprezentációt szolgáló elvont jellemzőket, amelyek az adatok leírására szolgálnak, és megtanulja, hogyan kapcsolódnak egymáshoz ezek a jellemzők. Ez lehetővé teszi számára, hogy összefüggésben értelmezze az új bemeneteket. Ez a betanítási folyamat hetekig vagy hónapokig tart (‡59), és több tíz- vagy százezer darab grafikus feldolgozó egységet (GPU) vagy tensorfeldolgozó egységet (TPU) (‡60) használ – olyan specializált számítógépes chipeket, amelyeket arra terveztek, hogy gyorsan végezzenek sok ilyen jellegű számítással. Egyes fejlesztők saját számítási erőforrással végzik a betanítást, míg mások a specializált számítási szolgáltatók által biztosított erőforrásokat használják.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Utóképzés és finomhangolás (képzési folyamat második szakasza)

  A „post-training” tovább finomhangolja az alapmodellt, hogy optimalizálja azt egy adott alkalmazáshoz. Ez egy mérsékelten erőforrás-igényes, ugyanakkor rendkívül munkaigényes folyamat. A „szintetikus adatok” használata – mesterségesen előállított információk, amelyek a valós adatokhoz hasonlóak, de algoritmusok vagy szimulációk segítségével készülnek – abban segít, hogy ez a szakasz kevésbé legyen munkaigényes.
  A poszttréning többféle finomhangolási technikát és egyéb módosításokat foglal magában. A ‘felügyelt finomhangolás’ magában foglalja az előzetesen betanított modell további betanítását konkrét adatkészleteken annak érdekében, hogy javuljon a modell teljesítménye az adott területen (‡61, ‡62). Például egy általános célú modell tovább képezhető egy nagyméretű radiológiai képadatkészleten. A ‘megerősítéses tanulás’ (RL) a modell teljesítményének javítását jelenti azáltal, hogy a modellt ‘jutalmazzák’ (pozitív visszajelzést adnak) a kívánatos kimenetekért, illetve a modellt ‘büntetik’ (negatív visszajelzést adnak) a nem kívánatos kimenetekért. Két kiemelkedő alkategóriája van. A ‘megerősítéses tanulás emberi visszajelzésekből’ azt jelenti, hogy a humán preferenciáknak megfelelő kimeneteket jutalmazzák, a nem megfelelőket pedig büntetik, az emberi visszajelzések alapján (‡63, ‡64*). A ‘megerősítéses tanulás igazolható jutalmakkal’ (RLVR) olyan feladatoknál használatos a modell teljesítményének javítására, amelyek tényszerű helyességet igényelnek, például matematikai vagy kódgenerálási feladatoknál. A fejlesztők jellemzően addig váltogatják a poszttréning technikák alkalmazását és a tesztek lefuttatását, amíg az eredmények nem azt mutatják, hogy a modell megfelel a kívánt specifikációknak.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Rendszerintegráció

  A fejlesztők egy vagy több általános célú AI modellt más összetevőkkel kombinálva olyan „AI rendszert” hoznak létre, amely készen áll a használatra. A GPT-5 (például) egy általános célú AI modell, amely szöveget, képeket és hangot dolgoz fel, míg a ChatGPT egy általános célú AI rendszer, amely több, eltérő méretű és képességű modellt kombinál egy csevegőfelülettel, tartalomfeldolgozással, Web-hozzáféréssel és alkalmazásintegrációval annak érdekében, hogy működőképes terméket hozzon létre.
  Az AI modellek működőképessé tételén túl az AI rendszeren belüli további összetevők is arra törekszenek, hogy növeljék a képességeit, a hasznosságát és a biztonságát. Például egy rendszerhez tartozhat egy szűrő, amely felismeri és blokkolja azokat a modellbemeneteket vagy modellkimeneteket, amelyek káros tartalmat tartalmaznak (‡65*). A fejlesztők emellett egyre gyakrabban használnak „scaffolding”-et – általános célú AI modellek köré épített kiegészítő szoftvereket, amelyek lehetővé teszik számukra, hogy előre tervezzenek, célokat kövessenek, és kapcsolatba lépjenek a világgal (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Telepítés és kiadás
  A telepítés az a folyamat, amelynek során a integrált AI-rendszert elérhetővé teszik a tervezett felhasználás céljára. A fejlesztők és a telepítők az AI-rendszereket valós alkalmazásokba, termékekbe vagy szolgáltatásokba integrálják. A fejlesztők az AI-rendszereket belsőleg (saját használatra) vagy külsőleg (magán ügyfelek vagy nyilvános felhasználás céljára) is telepíthetik. Amikor az AI-rendszereket külsőleg telepítik, a vállalatok gyakran úgy biztosítanak hozzáférést a felhasználóknak, hogy online felhasználói felületeken vagy alkalmazásprogramozási felületeken (application programming interfaces, APIs) keresztül engednek hozzáférést, illetve futtatást a rendszerhez. Például egy vállalat tervezhet egy egyedi ügyfélszolgálati chatbotot, amelyet egy másik vállalat általános célú AI-rendszere működtet.
  Az „AI rendszer telepítése” a modell valós környezetben történő használatba bocsátását jelenti integrált eszközökkel és felületekkel, míg a „modell kiadása” a kiindulási modell mások számára történő hozzáférhetővé tételét foglalja magában – akár nyílt súlyokkal (letölthető paraméterekkel), akár zárt súlyokkal (csak API-hozzáférés). Lásd: §3.4. Nyílt súlyú modellek.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Telepítés utáni felügyelet és frissítések

  A fejlesztők gyakran gyűjtenek és elemeznek felhasználói visszajelzéseket, követik a hatás- és teljesítménymutatókat, valamint iteratív fejlesztéseket végeznek annak érdekében, hogy kezeljék a valódi használat során feltárt problémákat (‡67). A fejlesztéseket a rendszerintegrációk frissítésével hajtják végre, többnyire folyamatos finomhangolással és úgy, hogy a modellek hozzáférést kapnak külső, (friss) tényekről szóló adatbázisokhoz. Ez naprakészen tartja a nagy AI-modelleket anélkül, hogy megismételnék a teljes előtanítási folyamatot (‡68*). Ez lehetővé teszi, hogy a képességek felhalmozódjanak a következő tanítási körök során, miközben megőrzik a stabilitást, és csökkentik a számítási költségeket.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Táblázat 1.2: Általános célú mesterséges intelligencia fejlesztési szakaszok
>white|black||9|11|br Minden általános célú mesterséges intelligencia fejlesztési szakaszban a mesterséges intelligencia modellt továbbfejlesztik a downstream felhasználás számára, majd végül teljesen integrált mesterséges intelligencia rendszerként üzembe helyezik, amelyet figyelnek és frissítenek.


>white|orangered|left|13|15|bb A következtetési rendszerek az inferencia során „gondolatláncokat” generálnak a teljesítmény javítása érdekében

Az Inference akkor történik, amikor valaki a betanított AI-modellt a tanulási fázis után használja. Például az Inference akkor következik be, amikor egy személy egy AI-rendszertől utazás megtervezését kéri, és a mögötte álló modell a földrajzra, közlekedésre és konyhaművészetre vonatkozóan arról tanult releváns szempontokra támaszkodva állít össze egy útitervet.

Az elmúlt évtizedben az MI-képességek fejlődése nagyrészt nagyobb tanítási futtatásokból származott; vagyis azáltal, hogy növelték az AI-modell betanításához felhasznált számítási erőforrások mennyiségét. Azonban nemrég a kutatók több eredményt értek el azzal, hogy lehetővé tették a modellek számára az információ hosszabb ideig történő feldolgozását, valamint azzal, hogy betanították őket arra, hogy a feladat elvégzése során explicit gondolkodási lépéseket hozzanak létre (‡69*, ‡70). Az ilyen módon működő MI-rendszereket „reasoning systems”-nek, az általuk a probléma megoldása vagy egy kérdés megválaszolása közben végigvitt köztes magyarázatokat pedig „chains of thought”-nak nevezik. A reasoning systems-ek használat közben több számítási erőforrást igényelnek ahhoz, hogy ezeket a kifinomult „chains of thought” szekvenciákat létrehozzák (‡71, ‡72, ‡73, ‡74), és a tanítás során is több erőforrást, hogy jobban megtanuljanak érvelni. Gyakorlatban ezek a reasoning képességek lehetővé teszik az MI-rendszerek számára, hogy bonyolultabb problémákat oldjanak meg azáltal, hogy a feladatot iteratívan kisebb lépésekre bontják. A 1.3. Táblázat egy nem-reasoning rendszer és egy reasoning rendszer példáját mutatja be, amelyek ugyanazt a problémát oldják meg.

A következtetési rendszerek jelentős áttöréseket értek el a nehéz feladatok terén. Például 2025-ben a matematikai problémamegoldásra specializált következtetési rendszerek, mint a Google Gemini Deep Think és az OpenAI egyik kiadatlan, kísérleti modellje, megoldották a Nemzetközi Matematikai Diákolimpiádák feladatait (strukturált tesztkörnyezetben) olyan szintű teljesítménnyel, amely az emberi aranyérmes teljesítménnyel egyenértékű (‡75, ‡76). A következtetési rendszerek jelentős fejlődést mutattak formális területeken is, például a matematikában, a logikai fejtörőkben és az strukturált tudományos kérdésekben, ahol a lépésről lépésre történő következtetés kifejezetten ellenőrizhető (‡77). Ugyanakkor a következtetési rendszerek hibázhatnak is azáltal, hogy irreleváns, nem produktív vagy ismétlődő gondolatmeneteket (‡78, ‡79) állítanak elő.

###@ Frissítések a képzési módszerekről

A legutóbbi Jelentés (2025 január) megjelenése óta egy „desztilláció” nevű képzési módszer jelentősen növelte egyes modellek hatékonyságát a finomhangolás során. A desztilláció során egy „diák” modellt egy erősebb (és általában nagyobb) „tanár” modell kimenetein képeznek ki, lehetővé téve, hogy a diák modell közvetlenül utánozza a tanár modell kimeneteit (‡80). Például a DeepSeek kifejlesztett egy DeepSeek-R1 nevű nagy modellt, amely kiemelkedően teljesít a „chain-of-thought” jellegű érvelésben. Az R1 olyan érvelési kimeneteket állított elő, amelyeket ezután kisebb diákmodellek finomhangolására használtak, köztük a DeepSeek-V3-at. A DeepSeek-V3 nagy mértékben megőrzi az R1 matematikai, kódolási és dokumentumelemzési képességeit, és a beszámolók szerint körülbelül $10,000 USD értékben finomhangolták (bár az előzetes betanítási költségeit nem közölték) (‡81). Ez valószínűleg nagyságrendekkel alacsonyabb, mint az ugyanerre a képességszintre finomhangolt, hasonlóan nagy modellek költsége.

![table1.3](images/table1.3_example_reasoning.png)

##### Táblázat 1.3: Példa egy nem okfejtő rendszerre (balra) egy okfejtő rendszerrel (jobbra) szemben
>white|black||9|11|br Ugyanennek a találós kérdésnek a megoldásakor ezek a példák valós AI-válaszokból lettek adaptálva. A gondolkodási rendszer több időt és számítási erőforrást fordít a „gondolkodásra” azáltal, hogy a végső válasz megadása előtt felépít egy „gondolatláncot”.

![figure.3](images/fig1.3_AI_agent.png)

##### Ábra 1.3: Egy szemléltető ábrázolás egy AI-ügynökről
>white|black||9|11|br Egy AI-modell (középen), amelyet úgy konfiguráltak, hogy iteratívan tervezzen, érveljen, és eszközöket használjon a valós feladatok elvégzéséhez. Forrás: International AI Safety Report 2026.


A desztilláció így olcsó és hatékony módja lehet annak, hogy a modellek nagyobb képességekre tegyenek szert (‡82). Néhány kutató a desztillációt arra használta, hogy rendkívül nagy teljesítményű modelleket finomhangoljanak, már mindössze 1,000, a korszerű modellekből generált példával (‡83). Mivel a desztilláció egy előzetesen létező tanító (teacher) modellt igényel, nem használható közvetlenül a korszerű modellek képességeinek továbbfejlesztésére. Ugyanakkor felgyorsíthatja a fejlett AI-képességek elterjedését, akár zárt forráskódú modellekből is (‡84*).

A technológiai fejlődéssel együtt a „disztribuált számítás” és a decentralizált tanítás (olyan megközelítések, amelyek során a fejlesztők több processzort, szervert vagy adatközpontot használnak együtt a mesterséges intelligencia tanításához vagy következtetéséhez (‡85, ‡86, ‡87)) révén csökkent annak mértéke, hogy sok AI-fejlesztési projekt nagyléptékű, központosított számítási infrastruktúrára támaszkodik. Ez egyre inkább lehetővé teszi, hogy kevésbé jól erőforrásolt szereplők is erőteljes rendszereket fejlesszenek és telepítsenek.

###@ Frissítések a AI-ügynökökről

A legutóbbi jelentés óta (2025 január), a fejlesztőknek az AI modelleket eszközökkel kombináló módszereiben elért fejlődés egyre erősebb AI ügynökök (agentek) kifejlesztését tette lehetővé. Az AI ügynökök célok elérésére vannak tervezve, amelyeket gyakran a felhasználók természetes nyelven adnak meg. E célok eléréséhez hozzáférést kapnak olyan eszközökhöz, mint a memória, a számítógépes felület és a webböngészők. Az ezeket az eszközöket, valamint a modellel való kombinálásukhoz használt kódot „scaffoldingnak” nevezik, és segítenek az AI ügynököknek autonóm módon kapcsolatba lépni a világgal, terveket készíteni, megjegyezni a fontos részleteket, valamint célokat követni (‡88*, ‡89) jóval kevesebb emberi felügyelettel vagy segítséggel. Például a Manus AI egy népszerű AI ügynök, amely képes különféle feladatok automatizálására, ideértve a webes keresést, a szoftverfejlesztést és az online vásárlásokat (‡90). Az 1.3. ábra egy egyszerű példát mutat be egy AI ügynökre: egy általános célú AI modellből („agy”) áll, amely iteratívan képes tervezni, következtetni, és eszközöket használni a memória, a webböngészés és a számítógép használata érdekében.

Az AI-ügynökök digitális infrastruktúrája bővül (‡91), és egyre gyakrabban fordul elő különböző iparágakban (‡92, ‡93, ‡94). Az AI-ügynököket olyan feladatokra fejlesztették ki, mint a kutatás (‡37), a szoftverfejlesztés (‡95), a robotika irányítása (‡96) és az ügyfélszolgálat (‡97). A folyamatos kutatás-fejlesztés egyre felkészültebb és egyre autonómabb AI-ügynököket, illetve többügynökös rendszereket eredményezett. A kutatók becslése szerint azoknak a szoftveres benchmarkfeladatoknak a komplexitása, amelyeket az AI-ügynökök képesek elvégezni, megközelítőleg minden hét hónapban megduplázódik (lásd még §1.2. Jelenlegi képességek) (‡98). A szakértők szerint az egyre képességesebb AI-ügynökök egyszerre jelentős lehetőségeket és kockázatokat fognak felvetni (‡99, ‡100*) (lásd §2.2.1. Megbízhatósági kihívások).

###@ Bizonyítéki hiányosságok

A generikus célú AI-rendszerek fejlesztési folyamata körüli fő bizonyítéki hiányosságok elsősorban abból erednek, hogy nem áll rendelkezésre nyilvánosan hozzáférhető információ arról, hogyan fejlesztik ezeket. Egyes fejlesztők rendkívül átláthatóak azzal kapcsolatban, hogyan fejlesztenek generikus célú AI-rendszereket (‡1, ‡101). Ugyanakkor általánosságban véve korlátozott mértékű a nyilvánosság és a szakpolitikai döntéshozók ismerete arról, hogyan fejlesztik, biztosítják, értékelik és telepítik a legtöbb fejlett modellt. Ez különösen igaz azokra a belső telepítésű AI-rendszerekre, amelyeket AI-vállalatokon belül használnak, de amelyeket a külső érdekelt felek nem használnak, és nem is ismernek (‡102, ‡103). Ez a korlátozott külső láthatóság kihívásokat teremt az átláthatóság és a felügyelet terén. Különböző kutatók rámutattak a képzési adatokkal (‡104, ‡105, ‡106), a generikus célú AI-modellekkel (‡107, ‡108), az AI-ügynökökkel (‡92), az értékelésekkel (‡109), a fejlesztési folyamatokkal (‡110) és a biztonsággal (‡111) kapcsolatos korlátozott és következetlen átláthatóságra. A külső nyilvánosságra hozatal korlátozásai néha szükségesek a vállalatok üzleti titkainak és szellemi tulajdonának védelme érdekében. Ugyanakkor az alacsony átláthatóság megnehezíti, hogy a független kutatók és szakpolitikai döntéshozók tanulmányozzák a generikus célú AI-modelleket és rendszereket.


