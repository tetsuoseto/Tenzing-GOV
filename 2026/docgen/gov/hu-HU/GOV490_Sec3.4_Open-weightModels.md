##########
>white|orangered|left|14|30|hr 3.4. szakasz
### 3.4. Nyílt súlyú modellek
>white|orangered|left|24|30|hb Nyílt súlyú modellek

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Fontos információk
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Az AI-vállalatok által a modelljeik „súlyaihoz” biztosított hozzáférés szintje befolyásolja az ezen modellek által jelentett kockázatokat. A súlyok azok a matematikai paraméterek, amelyek lehetővé teszik az AI-modellek számára, hogy bemeneteket feldolgozzanak és kimeneteket generáljanak. Bármely adott modell esetén a vállalatok dönthetnek úgy, hogy a súlyokat teljes mértékben magántulajdonban tartják, bizonyos felhasználóknak korlátozott hozzáférést adnak, vagy lehetővé teszik, hogy bárki teljes terjedelemben letöltse azokat. Azok a modellek, amelyeknek a súlyai nyilvánosan elérhetők, „nyílt súlyú modelleknek” nevezik őket.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Az open-weight modellek megkönnyítik a kutatást és az innovációt, de a védelmi mechanizmusaikat könnyebben el lehet távolítani. A világ számos szereplője – különösen azok, akiknek kevesebb erőforrásuk van – használhat open-weight modelleket kutatási és kereskedelmi célokra. Ugyanakkor a closed-weight modellekhez képest az open-weight modellek könnyebben módosíthatók olyan, potenciálisan káros viselkedések megjelenítésére, és nehezebb.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A nyílt súlyú modellek kiadásai visszavonhatatlanok. A kiadást követően a modell súlyai nem hívhatók vissza. Ez megnehezíti a potenciális károk mérséklését, amelyeket az olyan modellek kiadása okozhat, amelyek veszélyes képességekkel rendelkeznek.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ A legutóbbi jelentés (2025 január) megjelenése óta a nagy, nyílt súlyokat (open-weight) használó kiadások jelentősen csökkentették a képességbeli szakadékot a vezető, zárt (closed) modellekhez képest. A kínai fejlesztők, a DeepSeek és az Alibaba, rendre kiadták az R1, illetve a Qwen modelljeiket, amelyek a teljesítményükkel a vezető zárt modellekhez mérhető eredményeket értek el, miközben az OpenAI 2019 óta először adott ki nyílt súlyú modelleket. A vezető zárt modellek képességeit jelenleg úgy becsülik, hogy kevesebb mint 1 évvel vannak a vezető nyílt súlyú modellek előtt a kiemelt AI benchmarkokon.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A kulcsfontosságú szakpolitikai kihívás az, hogy hozzáférjünk azokhoz az előnyökhöz, amelyeket a nyílt súlyú modellek nyújtanak, miközben kezeljük azok egyedi kockázatait. Az egyik megközelítés a nyílt súlyú modellek értékelése az általuk jelentett „marginális kockázat” szempontjából: annak mértéke, amennyiben a kiadásuk kontrafaktuálisan növeli a társadalmi kockázatot a már meglévő modellek vagy más technológiák által okozott kockázaton túl. Ez azonban a gyakorlatban bonyolult. A marginális kockázat időbeli kis mértékű növekedései is összeadódhatnak, és a teljes kockázat jelentős növekedéséhez vezethetnek.
>oldlace|black||11|15|br      


A nyílt súlyú modellek, amelyek paraméterei nyilvánosan letölthetők, számos, az előző szakaszokban tárgyalt kihívással kapcsolatban sajátos következményekkel járnak. Egy AI-modell „súlyai” tartalmazzák azt a kritikus információt, amely lehetővé teszi számára, hogy a felhasználók számára hasznos válaszokat generáljon. Kiadásuk után ezek a súlyok nem vonhatók vissza: bárki letöltheti, tanulmányozhatja, módosíthatja, megoszthatja, és saját számítógépén vagy felhőfiókjában használhatja őket. Ha a súlyok nyíltan elérhetők, mások könnyebben tudnak ezekre építeni és a modellt módosítani, így sokféle igényt tudnak kiszolgálni, és innovációt ösztönöznek (‡1317). Ugyanakkor ugyanez a mechanizmus azt is megkönnyíti, hogy rosszindulatú felhasználók eltávolítsák a védelmi korlátokat, és az nyílt súlyú modelleket káros célokra módosítsák (‡1122, ‡1160). Ez felvetette annak kérdését, hogy egyes nyílt súlyú modelleket különleges követelményekhez kell-e kötni (pl. a kiadás előtti szigorúbb teszteléshez), vagy ezzel ellentétben különleges felmentéseket kell-e kapniuk (pl. a szabályozói jelentéstételi követelmények alóli mentességet) (‡1033).

###@ Háttér a nyílt súlyú modellekről

>white|orangered||14|15.5|bb A nyílt súlyú modellek lehetnek, de nem feltétlenül, „nyílt forráskódú” modellek

Bár gyakran „nyílt forráskódúnak” nevezik, a legtöbb nyilvánosan kiadott modell pontosabban „nyílt súlyúnak” (open-weight) írható le. Ennek oka, hogy bár a fejlesztők a modell súlyait biztosítják, nem adják ki a kapcsolódó tanítási kódot vagy az adatkészleteket. Ezenkívül a nyílt forráskódú szoftvereket általában olyan engedélyek jellemzik, amelyek a felhasználó vagy módosító downstream szereplőkkel szemben minimális követelményeket támasztanak (‡1318). Például a Meta Llama modelljei korlátozó licencfeltételekkel rendelkeznek, és kizárólag következtetési (inference) kódot tartalmaznak, nem pedig tanítási kódot, ezért általában nem tekintik őket nyílt forráskódúnak (‡1319, ‡1320). A modellek kiadási lehetőségei a teljesen zárttól a teljesen nyílt forráskódúig egy spektrumon helyezkednek el, és az egyes pontokon eltérő kockázat–haszon kompromisszumok merülnek fel (‡1086*, ‡1320, ‡1321). A 3.9. Táblázat ezeket a lehetőségeket írja le.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Teljesen zárt
  A felhasználók egyáltalán nem tudnak közvetlenül kapcsolatba lépni a modellel
  Példák: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Közvetített hozzáférés
  A felhasználók kizárólag egy meghatározott alkalmazáson vagy felületen keresztül tudnak kapcsolatba lépni, például egy mobil chatbot alkalmazáson keresztül
  Példák: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb API hozzáférés a modellhez
  A felhasználók kódból is küldhetnek kéréseket a modellnek, így külső alkalmazásokban is használható
  Példák: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb API-hozzáférés a finomhangoláshoz
  A felhasználók finomhangolhatják a modellt a saját, egyedi igényeikhez.
  Példák: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Nyílt súlyok: letölthető súlyok
  A felhasználók letölthetik és futtathatják a modellt a saját számítógépükön
  Példák: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Súlyok, adatok és kód letölthetők, felhasználási korlátozásokkal
  A felhasználók letölthetik és futtathatják a modellt, valamint az inferencia- és betanítási kódot is, de bizonyos licencelési korlátozások vonatkoznak a felhasználásukra.
  Példák: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teljesen nyitott: a súlyok, az adatok és a kód letölthetők, felhasználási korlátozások nélkül
  A felhasználóknak teljes szabadságuk van a modell letöltésére, használatára és módosítására, valamint a teljes kód és az adatok felhasználására.
  Példák: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.9. Táblázat: A modellmegosztási lehetőségek a teljesen zárttól a teljesen nyitottig
>white|black||9|11|br A modelmegosztási lehetőségek szemléltető válogatása a teljesen zárt modellektől (a modellek privátak, és kizárólag védett, saját célú felhasználásra vannak fenntartva) a teljesen nyitott és nyílt forráskódú modellekig (a modell-súlyok, az adatok és a kód szabadon és nyilvánosan elérhetők felhasználási, módosítási és megosztási korlátozás nélkül). Az első négy kategóriába tartozó modelleket gyakran „zártnak” nevezik. Ez a szakasz a három alsó sorra összpontosít. Forrás: Bommasani, 2024 (‡1317) alapján átdolgozva.


###@ Előnyök és kockázatok

>white|orangered|left|14|15.5|bb A nyílt súlyú modellek könnyebben testre szabhatók és kiértékelhetők

A nyílt súlyú modellek jelentős előnyöket kínálnak a kutatás, innováció és hozzáférés terén. Amint azt az §1.1. What is general-purpose AI? részben tárgyaljuk, az általános célú mesterséges intelligenciát megvalósító modellek betanítása rendkívül költséges – a vezető modellek kifejlesztése több százmillió dollárba kerül. A modell-súlyok nyílt közzététele lehetővé teszi, hogy a kevésbé jól erőforrásokkal rendelkező szereplők másolják, tanulmányozzák és építsenek a meglévő rendszerekre. Az ilyen hozzáférés nélkül az alacsony erőforrású régiók közösségei veszélyeztetve vannak abban, hogy kimaradjanak az AI előnyeiből, így a nyílt súlyok kritikus fontosságúak a globális többség részvételének biztosításához az AI fejlesztésében (‡1322). A downstream fejlesztők a modelleket különféle alkalmazásokhoz finomhangolhatják, például úgy alakíthatják őket, hogy alul-erőforrásokkal rendelkező kisebbségi nyelveket is támogassanak, vagy optimalizálhatják a teljesítményt olyan specifikus feladatokra, mint a jogi iratok szerkesztése vagy az orvosi megjegyzések rögzítése (‡1323, ‡1324*). Ily módon a nyílt súlyú modellek több embernek és közösségnek tehetik lehetővé az AI használatát és az abból származó előnyök kihasználását, mint ami egyébként lehetséges lenne (‡1325). Azoknál a modelleknél, amelyek nem elég képesek ahhoz, hogy veszélyesek legyenek, ezek az előnyök felülmúlhatják a súlyok nyílt közzétételével járó további kockázatot, bár ez a releváns döntéshozók kockázattűrő képességétől függ.

A nyílt súlyokkal (open-weight) történő kiadás tovább szélesíti azon fejlesztők és kutatók körét, akik képesek a modell tanulmányozására, képességeinek értékelésére, sérülékenységek tesztelésére, valamint a fejlesztések iteratív végrehajtására (‡1326, ‡1327). Ez növeli annak valószínűségét, hogy mind a hasznos alkalmazásokat, mind a káros hibákat azonosítják, bár ez nem garantált (‡1328, ‡1329). A felhasználók emellett saját eszközeiken is futtathatnak nyílt súlyú modelleket, így megőrizhetik az ellenőrzést az érzékeny adatok felett, és elkerülhetik azok harmadik fél szervereinek történő elküldését.

További előnyök származnak abból, ha a fejlesztők megosztják az olyan információkat, mint a betanítási adatok, a kód, az értékelő eszközök és a dokumentáció, valamint a modell-súlyok (‡1320, ‡1330, ‡1331, ‡1332*). Mivel több információ áll rendelkezésre, a downstream fejlesztők és más kutatók jobban megérthetik a nyílt súlyú modelleket, és azokat új alkalmazásokhoz tudják igazítani.

>white|orangered|left|14|15.5|bb A nyílt súlyú modellek védelmi intézkedései könnyebben eltávolíthatók, ezáltal potenciálisan rosszindulatú felhasználásra is lehetőséget teremtenek

A nyílt súlyú (open-weight) modellek emellett további kockázatokat is jelentenek, mert a védelmi mechanizmusok könnyebben eltávolíthatók. Bár mind a nyílt súlyú, mind a zárt (closed) modellek rendelkezhetnek olyan biztosítékokkal, amelyek képesek elutasítani a káros felhasználói kéréseket, ezek a biztosítékok a nyílt súlyú modelleknél sokkal könnyebben eltávolíthatók. A rosszindulatú szereplők finomhangolással (fine-tune) optimalizálhatják a modellt káros alkalmazásokhoz, eltávolíthatják a káros felhasználás megakadályozását szolgáló kódrészleteket, vagy visszavonhatják a korábbi biztonsági finomhangolást (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Ennek következtében a nyílt modellek súlyai fokozhatják az itt tárgyalt (így: §2.1) visszaélési kockázatokat. A rosszindulatú felhasználásból eredő kockázatok abból fakadnak, hogy több szereplő számára teszik lehetővé a meglévő képességek kiaknázását és káros célokra való kiterjesztését felügyelet nélkül (‡1122, ‡1315). Bár sok felhasználónak nem lesz meg az a tudása vagy ösztönző ereje, hogy eltávolítsa a biztosítékokat a nyílt súlyú modelleken, a magasan motivált rosszindulatú szereplők még így is aggályt jelentenek. Továbbá a rosszindulatú szereplők képesek lehetnek a nyílt súlyú modellek segítségével azonosítani a hasonló zárt modellek sebezhetőségeit (‡1055*). Az ilyen hibákat nehezebb megtalálni kizárólag zárt modellek futtatásával, a zárt-modell szolgáltatók által megvalósítható nagyobb kontroll és megfigyelési intézkedések miatt.

>white|orangered|left|14|15.5|bb A modell súlyainak megosztása visszafordíthatatlan

Miután a modell súlyai nyilvános letöltésre elérhetővé válnak, nincs mód az összes meglévő példány teljes, nagymértékű visszagörgetésének (rollback) végrehajtására. Az olyan internetes tárhelyszolgáltatók, mint a GitHub és a Hugging Face, eltávolíthatják a modelleket a platformjaikról, ami megnehezíti egyes szereplők számára, hogy letölthető másolatokat találjanak, és ezzel jelentős akadályt jelentenek sok alkalmi rosszindulatú felhasználó számára (‡1339). Mindazonáltal a kitartó szereplők még mindig juthatnak másolatokhoz, ha a modellt már letöltötték, és máshol újratárolták (rehosted), vagy helyben (lokálisan) elmentették. Továbbá azok a downstream fejlesztők is, akik a nyílt súlyú (open-weight) modelleket beépítik a saját rendszereikbe, átörökítenek minden hibát is, például az ellenséges támadásokkal szembeni sebezhetőségeket (‡1055), vagy a modell azon képességét, hogy megkerülje a megfigyelő rendszereket (lásd §2.2.2. Loss of control) (‡1315). A zárt modellekkel ellentétben, ahol a hosztok általánosan tudnak javításokat (fixeket) bevezetni, a nyílt súlyú modellek fejlesztői nem tudják garantálni, hogy a felhasználók átveszik a frissítéseket.

###@ Frissítések

A legutóbbi Jelentés (2025 január) megjelenése óta a vezető nyílt súlyú és zárt modellek közötti képességbeli rés csökkent. A kínai fejlesztők különösen fontos szolgáltatóivá váltak a nyílt súlyú modelleknek. 2025 januárjában a DeepSeek kiadta az R1 modelljét, amely több mérőszámon (‡1340) hasonló teljesítményt ért el, mint az OpenAI o1-je. Az Alibaba Qwen modelljei szintén egyre nagyobb teret nyertek: 2025 augusztusára a Chatbot Arenán, egy széles körben használt teljesítménybenchmarkon, a nyílt súlyú modellek között elfoglalták az első helyet (‡1341, ‡1342*). 2025 augusztusában az OpenAI kiadta első nyílt súlyú modelljeit 2019-es GPT-2 kiadása óta, a gpt-oss-120b-t és a gpt-oss-20b-t. A Meta továbbra is kiadja a Llama modelleket nyílt súlyokkal. A vezető zárt modellek képességeit ma már úgy becsülik, hogy a kiemelt AI-benchmarkokon kevesebb mint egy évvel vannak a vezető nyílt modellek előtt (3.10 Ábra).

###@ Bizonyítéki hiányosságok

Egy kulcsfontosságú bizonyítékalapú hiányosság az, hogy a nyílt súlyú modellek visszaélésének megakadályozását célzó technikai megoldások mennyire hatékonyak a valós környezetben. A kutatók többféle megközelítést javasoltak annak érdekében, hogy a modellek ellenállóbbá váljanak a manipulációval szemben. Ide tartozik olyan új betanítási technikák bevezetése, amelyek célja, hogy a modellek ellenálljanak a káros módosításoknak (‡1276), a káros tartalom kiszűrése a betanítási adatokból (‡55), valamint a védekezések a jailbreakek ellen (‡675, ‡676). Ezeket a technikákat ma már a valós környezetben is alkalmazzák nagy fejlesztők kiadásaiban. Például az OpenAI alkalmazott néhány ilyen technikát a gpt-oss modelljeiben, és arról számolt be, hogy az ellenségesen finomhangolt változatok nem érték el a magas képességi küszöböket (‡1344*). Ugyanakkor a kutatások azt mutatták, hogy a rosszindulatú szereplők a modellek káros példákkal történő újratanításával ki tudják iktatni a védelmi mechanizmusokat (‡1345, ‡1346). Ezenfelül még mindig nehéz a biztosítékok (safeguards) robusztusságát megbízhatóan értékelni, így hatékonyságuk a valós támadásokkal szemben bizonytalan (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Ábra 3.10: Képességhiány a vezető nyílt súlyú és a zárt AI modellek között
>white|black||9|11|br A csúcsteljesítményt nyújtó, nyílt súlyú (sötétkék) és zárt (világoskék) modellek időbeli Epoch Capabilities Index (ECI) pontszámai. Az ECI 39 benchmark eredményeit egyesíti egyetlen általános képességskálává. A legjobb nyílt súlyú modellek hozzávetőleg egy évvel le vannak maradva a zárt modellek mögött. Forrás: Epoch AI, 2025 (‡1343).


###@ Mérséklések

Az nyílt súlyú modellek kockázataival kapcsolatos technikai mitigációk az AI fejlesztési és bevezetési folyamatának egészében érvényesülnek (‡1141, ‡1195, ‡1347). Például amikor a modelleket fejlesztik, a fejlesztők és a downstream adapterek képesek kiszűrni a kényes tartalmakat a betanítási adatokból, hogy minimalizálják a káros képességeket. Ha eltávolítják a káros példákat egy modell betanítási adataiból, az megakadályozhatja az ellenséges fine-tuningot 10-szer hatékonyabban, mint az edzés után hozzáadott védelmek, bár ez hatással lehet a hasznos képességekre is (‡55). Az AI-alkalmazásszolgáltatók emellett bevezethetnek incidens-jelentési és reagálási mechanizmusokat (‡1348).

Emellett olyan tárhelyszolgáltatók, mint a HuggingFace és a GitHub, be tudnak vezetni platformfelhasználási feltételeket, hogy eltávolítsák a káros célokra módosított modelleket (‡1141, ‡1324). A modellfejlesztők a kiadás előtt teljes hozzáférést biztosíthatnak a felülvizsgálatot végzőknek, vagy alkalmazhatnak egy „fokozatos” kiadási stratégiát – a modelleket egyre nagyobb csoportoknak adva ki (‡1086). Ez segíthet az esetleges meghibásodások vagy sebezhetőségek azonosításában, mielőtt a modell széles körben elérhetővé válna (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Jegyzet 3.1: Modell súlyának biztonsága
>oldlace|black|left|13|15|hb 3.1-es doboz: Modell súlyainak biztonsága
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ebben a szakaszban tárgyalt kockázatok feltételezik, hogy a modell-súlyokat szándékosan kiadják. Azonban a zárt modell-súlyok lopás vagy kiszivárgás révén is hozzáférhetővé válhatnak. A zárt modellek kifejlesztése több százmillió dollárba kerül (§1.1. What is general-purpose AI?) és átlagosan képességesebbek, mint a nyílt súlyú modellek (‡1343). Ez vonzó célponttá teszi őket a szereplők széles köre számára, a hobbihackerektől a nemzetállamokig, amelyek vezető AI modellek megszerzésére törekszenek.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br A ellopott, zárt modell-súlyok hasonló kockázatokat jelentenének, mint amelyek fentebb a nyílt súlyú modelleknél leírásra kerültek, de potenciálisan bármilyen enyhítő intézkedés nélkül. A rosszindulatú szereplők eltávolíthatják a legképességesebb modellekből a biztosítékokat. A legitim fejlesztőktől eltérően az ilyen szereplők nem lennének kitéve azoknak a reputációs, jogi vagy kereskedelmi korlátoknak, amelyek jelenleg arra ösztönzik a legmodernebb AI-t fejlesztő vállalatokat, hogy modelljeiket biztonságosan telepítsék.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br A jelenlegi biztonsági szintek iparágonként eltérnek, és előfordulhat, hogy nem elegendők a kifinomult támadók ellen. Egyes fejlesztők elköteleződnek amellett, hogy a modell súlyait megvédik a kiberdűnözői szindikátusok és belső fenyegetések ellen (‡582), míg mások semmilyen nyilvános biztonsági elköteleződést nem tettek (‡1109, ‡1349). A kutatások szerint a mesterséges intelligenciával működő adatközpontok esetleg képtelenek ellenállni a legkifinomultabb és a legjobban felkészített szereplők támadásainak (‡582, ‡1350, ‡1351). 2025 decemberéig nem léteznek megerősített, nyilvánosan dokumentált esetek a modell súlyok ellopására vonatkozóan. Ugyanakkor a vezető mesterséges intelligenciával foglalkozó vállalatoknál más biztonsági incidensekről is beszámoltak, ideértve a Microsoft e-mail rendszereinek beszivárgását (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ezeknek a biztonsági hiányosságoknak a megszüntetése jelentős beruházásokat igényelne hardver-, szoftver-, személyzeti és létesítménybiztonsági területen. Néhány biztonsági fejlesztés viszonylag gyorsan, összehangolt erőfeszítéssel megvalósítható (‡1122). Más, azonban kritikus intézkedések, például a hardverszállítási láncok és a létesítmények biztosítása, várhatóan évekig tartanának (‡1122). A magáncégeknek emellett elképzelhetően hiányoznak azok az erőforrások vagy információk, amelyek önállóan megfelelő védelmek kidolgozásához szükségesek. Például az AI-fejlesztőknek nincs hozzáférésük ahhoz a minősített fenyegetés-elemzési (threat intelligence) információhoz, amelyet a kormányok kapnak (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Kihívások a döntéshozók számára

A döntéshozók egyik kulcsfontosságú kihívása, hogy biztosítsák a nyílt súlyú modellek megosztásából származó előnyöket anélkül, hogy jelentősen növelnék a kockázatot. A katasztrofális károk elkerülése érdekében a nyílt súlyú modellek fejlesztőinek nem szabad a modelleket a kockázatok értékelése nélkül kiadniuk: egyrészt a zárt modelleknél már bevált felmérési módszereket kell alkalmazniuk, másrészt további tesztelést is szükséges végezniük, figyelembe véve, hogy a rosszindulatú szereplők a modelleket finomhangolhatják és eltávolíthatják a biztonsági védelmeket. A gyakorlatban ez azonban nehéz lehet, mert a képességek fejlődése kiszámíthatatlan lehet, a nyílt súlyú kiadások visszafordíthatatlanok, és olyan értékelési erőfeszítésekre van szükség, amelyek előre jelzik, mikor jelentene a kiadás jelentős potenciális kárt. Az egyik megközelítés a nyílt kiadások „marginális kockázatának” felmérése: annak mértéke, amennyiben a kiadás ellenkező tényállás szerint (counterfactually) növeli a társadalmi kockázatot a már meglévő modellek vagy más technológiák által okozott kockázaton túl (‡556, ‡1033, ‡1354, ‡1355) (lásd §3.2. Kockázatkezelési gyakorlatok). Ugyanakkor annak becslése, hogy egy rendszer mennyiben növeli vagy csökkenti a közvetett (downstream) kockázatot a beüzemelése után, összetett és kontextusfüggő. A kockázat egymást követő kiadásokkal bekövetkező, fokozatos növekedése idővel felhalmozódva a teljes kockázat jelentős növekedéséhez vezethet, még akkor is, ha az egyes kiadásokhoz tartozó marginális kockázat elfogadhatónak tűnik (‡1356, ‡1357). Az AI-képességek kettős felhasználású jellege tovább bonyolítja a kormányzást: az olyan funkciók, amelyek a gyógyászatban vagy a kutatásban hasznos alkalmazásokat tesznek lehetővé, átirányíthatók (repurpose) a károkozásra, és amint a súlyok nyilvánossá válnak, nehézzé válhat megkülönböztetni a legitim és a rosszindulatú felhasználást. Az is bizonytalan, hogy ki legyen felelősnek tekinthető, amikor a nyílt súlyú modelleket káros célokra módosítják.

