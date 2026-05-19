##########
>white|orangered|left|14|30|hr 3.3. szakasz
### 3.3. Technikai biztosítékok és felügyelet
>white|orangered|left|24|30|hb Technikai biztosítékok és felügyelet

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Fontos információk
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ A mesterséges intelligencia fejlesztésének és alkalmazásának különböző szakaszaiban széles körű technikai biztosítékokat alkalmaznak. Ide tartoznak a modellfejlesztés során alkalmazott olyan technikák, amelyekkel a rendszerek robusztusabbá és a helytelen felhasználással szemben ellenállóbbá tehetők (például adattisztítás/adatválogatás), a kihelyezés alatti megfigyelés és vezérlés (például tartalomszűrés és emberi felügyelet), valamint a kihelyezés utáni eszközök a szélesebb AI-ökoszisztéma megfigyelésére (például származási információ/proveniencia és tartalomfelismerés).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A technikai biztosítékoknak vannak korlátai, és nem megbízhatóan előzik meg minden környezetben a káros viselkedést. Például a felhasználók néha káros kimeneteket tudnak elérni a kérések átfogalmazásával vagy azok kisebb lépésekre bontásával. Hasonlóképpen az olyan eszközök, mint a vízjelölés (watermarking), amelyek az AI-val generált tartalom azonosítására szolgálnak, gyakran eltávolíthatók vagy módosíthatók, ami korlátozza megbízhatóságukat.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Az egyéni védintézkedések korlátai miatt előfordulhat, hogy a bizonyos káros kimenetek megelőzéséhez ‘mélységi védelem’ (defence-in-depth) szükséges. Például egy rendszer kombinálhat egy biztonságra betanított modellt bemeneti szűrőkkel, kimeneti szűrőkkel és tartalomfigyelőkkel.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A legutóbbi Jelentés (January 2025) közzététele óta a kutatók előrelépést tettek a biztosítékok javításában, de alapvető korlátok továbbra is fennállnak. Például az olyan támadások sikerességi aránya, amelyek a biztosítékok megkerülésére irányulnak, csökkenő tendenciát mutat, de továbbra is viszonylag magas. Továbbá alapvető korlátok vannak abban is, hogy az open-weight modelleket mennyire alaposan lehet biztosítékokkal ellátni.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ A döntéshozók egyik legfontosabb kihívása az, hogy korlátozott bizonyítékok állnak rendelkezésre arról, mennyire hatékonyak az óvintézkedések a különböző, valós körülmények között alkalmazott, általános célú mesterséges intelligencia rendszerek esetében. Az AI-fejlesztők nagyon eltérően járnak el abban, hogy mennyi információt osztanak meg az óvintézkedéseikről és a felügyeletükről. További kihívás az is, hogy lehetséges kompromisszumok alakulhatnak ki az erősebb óvintézkedések alkalmazása és a rendszer teljesítményének vagy hasznosságának fenntartása között.
>oldlace|black||11|15|br      


Az AI-fejlesztők több hasznos, de tökéletlen műszaki védőintézkedést is használhatnak az általános célú AI-rendszerekből eredő kockázatok mérséklésére és kezelésére, ugyanakkor a robusztussági kihívások továbbra is fennállnak. A fejlesztők még mindig nem képesek teljes mértékben megakadályozni, hogy az általános célú AI-rendszerek akár jól ismert és nyíltan káros cselekvéseket is végrehajtsanak, például hogy felhasználói számára útmutatást adjanak bűncselekmények elkövetéséhez. Például a kutatók megmutatták, hogy a legkorszerűbb védőintézkedések is kijátszhatók adverzariális promptolási módszerekkel (azaz „jailbreak”-ekkel) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), úgy, hogy a modellek a komplex káros feladatokat lépésekre bontják (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), valamint egyszerű modellmódosításokkal (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). A kutatók továbbra is dolgoznak a meghibásodások és a visszaélések elleni védőintézkedéseken (‡690). Ezek a módszerek széles körben eltérnek céljuk és hatékonyságuk tekintetében, és a hatásuk végső soron attól függ, hogy milyen szélesebb társadalmi-technikai és irányítási (governance) környezetben építik és telepítik az AI-rendszereket.

A műszaki biztosítékok nagyjából három kategóriába sorolhatók: a biztonságosabb modellek fejlesztésére szolgáló technikák; a telepítés során alkalmazott technikák a felügyeletre és az ellenőrzésre; valamint a telepítés utáni ökoszisztéma-felügyeletet támogató technikák. A 3.6 Táblázat összefoglalja a tárgyalt műszaki biztosítékokat, azok hatékonyságát és a fennálló nyílt kihívásokat.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Biztonságosabb modellek fejlesztése
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adatkurálás (‡1167)
  A káros adatok eltávolítása, hogy a modell ne tanuljon el veszélyes képességeket. Ezek a módszerek hasznosak lehetnek, beleértve a nyílt súlyú modellek fejlesztését is, amelyek nem rendelkeznek káros képességekkel, és ellenállnak a káros célú finomhangolásnak (‡55). Ugyanakkor kihívást jelent az adatrendezési hibák és a skálázás (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Reinforcement learning from human feedback (‡64*)
  A modellt a megadott célokkal való összhangra tanítani, például arra, hogy hasznos és ártalmatlan legyen. Ez hatékony módja annak, hogy a modellek hasznos viselkedéseket sajátítsanak el (‡64*). Ugyanakkor az emberi jóváhagyásért történő túlzott optimalizálás miatt a modellek megtévesztően vagy hízelgően viselkedhetnek (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Plurális összehangolási technikák (‡1170)
  A modellt arra képezni, hogy több, egymástól eltérő nézőpontot is integráljon arról, hogyan kellene viselkednie. Ezek a technikák segítenek csökkenteni annak mértékét, hogy a modellek bizonyos nézőpontokat előnyben részesítenek (‡1170). Mindazonáltal e technikák ellenére az emberi nézeltérés elkerülhetetlen, és nehéz olyan általánosan elfogadott módokat tervezni, amelyek a versengő nézőpontokat egyensúlyba hozzák (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adverzális betanítás (‡677)
  A modellt arra képezzük, hogy ne okozzon kárt (még ismeretlen helyzetekben sem), és hogy ellenálljon a rosszindulatú felhasználók (pl. „jailbreaks”) támadásainak. Ez hatékony módszer a modelleknek a visszaélésekre irányuló kísérletekkel szembeni ellenálló képességének növelésére (‡1064), de a robusztusság kihívásai továbbra is fennállnak (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb A gép „elfelejtése” (‡1175, ‡1176)
  Egy modell betanítása specializált algoritmusokkal, amelyek célzottan elnyomják a káros képességeket (pl. biológiai veszélyek ismerete). Ezek a technikák célzott módot kínálnak a káros képességek eltávolítására a modellekből (‡1175, ‡1176), azonban a jelenlegi elfelejtési algoritmusok nem mindig robusztusak, és nem szándékolt hatásokat válthatnak ki más képességekre is (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Értelmezhetőségi és biztonsági ellenőrző eszközök (‡1177)
  A tervezési és verifikációs módszerek sokszínű családja, amely arra szolgál, hogy még szigorúbb biztosítékot nyújtson arra vonatkozóan, hogy a modellek rendelkeznek meghatározott biztonsággal kapcsolatos tulajdonságokkal. Lehetővé teszik az értékelők számára, hogy nagyobb bizonyossággal hozzanak biztonsági garanciákat (‡1177), ugyanakkor a jelenlegi módszerek feltételezésekre támaszkodnak, és a gyakorlati teljesítmény tekintetében ritkán versenyképesek (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Monitoring és vezérlés
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hardveralapú felügyeleti mechanizmusok (‡1179, ‡1180, ‡1181)
  Azt ellenőrizni, hogy a felhatalmazott folyamatok a hardveren futnak, a biztonsági fenyegetések vagy a szabályozási megfelelőség vizsgálata érdekében. Ezek a mechanizmusok egyedi módokat kínálnak arra, hogy figyelemmel kísérjék, milyen számítások futnak a hardveren és ki által (‡1181). Ugyanakkor a hardveres mechanizmusok nem képesek mindenféle fenyegetés monitorozására, és egyes technikák speciális hardvert igényelnek (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Felhasználói interakciókat figyelő rendszerek (‡1154, ‡1166)
  A felhasználói interakciók monitorozása a rosszindulatú felhasználás jelei alapján segíthet a fejlesztőknek leállítani a szolgáltatást a rosszindulatú felhasználók számára (‡1154, ‡1166). Ugyanakkor a végrehajtás akaratlanul akadályozhatja a hasznos biztonsági kutatást (‡689), és a visszaélés egyes formái nehezen felismerhetők (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Felhasználói interakciót figyelő rendszerek (‡1154, ‡1166)
  A felhasználói interakciók figyelése a rosszindulatú használat jelei alapján segíthet a fejlesztőknek leállítani a szolgáltatást a rosszindulatú felhasználók esetében (‡1154, ‡1166). Ugyanakkor a végrehajtás akaratlanul akadályozhatja a biztonsággal kapcsolatos hasznos kutatást (‡689), és a visszaélés egyes formái nehezen észlelhetők (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tartalomszűrők (‡65*, ‡725)
  A potenciálisan káros modellbemenetek és -kimenetek szűrése nagyon hatékony módszer a véletlen károkozások és a visszaélések kockázatainak csökkentésére (‡725). Ugyanakkor a szűrők többlet számítási erőforrást igényelnek, és bizonyos támadások ellen sérülékenyek (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb A modell belső számítási monitorai (‡744, ‡1183, ‡1184)
  A modellekben a megtévesztés vagy más káros belső megismerési formák jeleinek figyelése hatékony módja lehet a megtévesztés észlelésének (‡744, ‡1183, ‡1184). Ugyanakkor a jelenlegi módszerek nem elég robusztusak és megbízhatóak (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lánc-megfigyelő monitorok (‡430, ‡435)
  A modell-láncolt gondolat (chain-of-thought) szövegének figyelése, hogy megtévesztő viselkedésre vagy más káros érvelésre utaló jeleket találjunk, hatékony módszer a modellek gondolkodásában megmutatkozó hibák megértésére és észrevételére (‡435). Ugyanakkor megbízhatatlanok lehetnek (‡752, ‡753, ‡1186), és ha a modelleket arra képezik ki, hogy jóindulatú chain-of-thoughtot állítsanak elő, akkor megtanulhatnak megtévesztő viselkedést (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ember a körben (‡1187, ‡1188, ‡1189)
  Az emberi felügyelet és a rendszerdöntések felülbírálásának lehetősége elengedhetetlen egyes biztonságkritikus alkalmazásokban (‡1187). Ugyanakkor ezeket a technikákat korlátozza az automatizálási torzítás, valamint az emberi döntéshozatal sebességének korlátai (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Homokozóba zárás (‡1192)
  Egy AI-ügynöknek a világra való közvetlen befolyásolását megakadályozása hatékony módja annak, hogy korlátozzuk azt a kárt, amelyet okozhat (‡1192). Ugyanakkor a sandboxolás korlátozza a rendszer képességét bizonyos feladatok közvetlen elvégzésére (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Eszközök az ökoszisztéma-monitorozást megkönnyítő feladatokhoz
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI-modellazonosítási technikák (‡1193*, ‡1194)
  Azáltal, hogy a modelleket, illetve a modellek egyes példányait a valós használati esetekben könnyebb azonosítani, támogatja a digitális igazságügyi elemzést és az ökoszisztéma-felismerést (‡1195). Ugyanakkor ezek a technikák bizonyos típusú modellmódosításokkal megkerülhetők (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI modell örökség-inferencia (‡1197)
  Ezek a technikák lehetővé teszik a kutatók számára, hogy vizsgálják, hogyan módosulnak a modellek az AI ökoszisztémában, különösen a nyílt súlyú modellek esetében. Segítenek a digitális kriminalisztikában és az ökoszisztéma-felügyelésben (‡1198), azonban nagyléptékű projektekre lenne szükség ahhoz, hogy alaposan feltérképezzék a nyílt súlyú modell-ökoszisztémát (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vízjelek és metaadatok (‡1199, ‡1200, ‡1201*)
  Ezek a technikák megkönnyítik annak felismerését, hogy egy szöveg, kép, videó stb. AI által generált vagy módosított-e, illetve hogy melyik rendszer állította elő. Elősegítik a jobb ökoszisztéma-áttekintést (‡1199, ‡1200, ‡1201*). Ugyanakkor a vízjelek és a metaadatok meghamisíthatók vagy eltávolíthatók a tartalom bizonyos módosításai révén (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Az AI által generált tartalom észlelése (‡1203, ‡1204, ‡1205*)
  A felhasználók azon képességének javítása, hogy meg tudják különböztetni az AI által generált és a valódi tartalmat, segíti a digitális kriminalisztikát és az ökoszisztéma-tudatosságot (‡1203, ‡1204). Ugyanakkor az osztályozók megbízhatatlanok lehetnek (‡1205*) és a teljesítményük modalitásonként változó.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.6. Táblázat: A szakaszban tárgyalt technikai biztosítékok
>white|black||9|11|br Az ebben a szakaszban tárgyalt technikai védintézkedések összefoglalása, három részre bontva: módszerek biztonságosabb modellek fejlesztésére, telepítéskori felügyelet és vezérlés, valamint a ökoszisztéma-felügyeletet megkönnyítő technikák.


###@ Biztonságosabb modellek fejlesztése

Az általános célú AI-rendszerekből eredő károk elleni első védelmi vonal, hogy a mögöttes modellt biztonságosabbá tesszük. Ez az alfejezet azokat az óvintézkedéseket ismerteti, amelyek a modellfejlesztési folyamat során „a modellparaméterekbe vannak beépítve” (Ábra 3.6).

>white|orangered|left|14|15.5|bb A képzési adatok válogatása korlátozhatja a potenciálisan veszélyes képességek kifejlesztését

Az általános célú AI-modellek pontosan azért hasznosak, mert a betanítási adatok feldolgozása után széles körű ismereteket és képességeket alakítanak ki, de a képzési adatok egyes típusai aránytalanul nagy szerepet játszanak a potenciálisan veszélyes képességek kifejlesztésében. Például egy virológiai cikkeken betanított AI-modell jobban képes lehet segítséget nyújtani potenciálisan ártalmas biológiai feladatokban (‡549, ‡1206*) (lásd még §2.1.4. Biológiai és kémiai kockázatok). Emellett az emberi meztelenséget ábrázoló képeken betanított kép/videó generátorok is felhasználhatók a beleegyezés nélküli intim deepfake-ek létrehozására (‡308, ‡319) (lásd még §2.1.1. AI-generált tartalom és bűnözői tevékenység).

A tanítóadatok szűrése hatékony mérséklés bizonyos nem kívánt képességek ellen (‡319, ‡1167, ‡1207, ‡1208). Ugyanakkor nehéz lehet a nagyméretű adatkészletek szűrése, amelyek az általános célú AI modellek betanításához szükségesek (‡1168), a magas költségek (‡1209), a szűrési hibák (‡1210) és az adatkészlet minőségére gyakorolt negatív hatások miatt (‡1211). E kihívásokat tovább súlyosbítja az internetes szöveg többnyelvű jellege (‡1212), a tartalomszűrésben jelen lévő kulturális torzítások (‡1211, ‡1213, ‡1214, ‡1215), valamint az a tény, hogy egy adott adatról azt, hogy „káros”-e, kontextuális tényezők határozzák meg (‡1216). Ennek ellenére a potenciálisan káros anyagoknak a tanítóadatokból történő kiszűrése ígéretesnek mutatkozik a modellek megbízhatóbban biztonságossá tételében, beleértve az open-weight modellek nagyobb ellenállóságát a káros beavatkozásokkal szemben (‡55). A tanítóadat-tartalmak és az olyan módon megjelenő modellek képességei közötti összefüggéseket még nem teljes mértékben értjük (‡1195), és a kiszűrés látszólag hatékonyabb a káros képességek korlátozásában, ha széles tudásterületekre alkalmazzák (‡55), mint ha szűkebb viselkedésekre (‡1206, ‡1217). Lásd §3.4. Open-weight modellek további megbeszéléshez.

![figure 3.6](images/fig3.6_safeguards.png)

##### Ábra 3.6: Hol kell alkalmazni a technikai védintézkedéseket
>white|black||9|11|br A technikai biztosítékok a modellfejlesztés különböző szakaszaiban alkalmazhatók. Az adatkiválogatás (data curation) meghatározza, hogy a modellek mit tanulnak az előtanítás (pre-training) és a finomhangolás (fine-tuning) során. A tréningalapú módszerek, például a humán visszajelzésből történő erősítéstanulás (reinforcement learning from human feedback) és a robusztussági tréning (robustness training) a modell viselkedését igazítják. A tesztelési módszerek, például a károkozó (adversarial) támadások, azonosítják a fennmaradó sérülékenységeket. Néhány technika, például a safe-by-design algoritmusok, több szakaszon átível. Forrás: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Az általános célú mesterséges intelligencia modellek hasznos és ártalmatlan működésre történő betanításának módszerei elsősorban emberi visszajelzéseken alapulnak.

Nehéz megbízhatóan a magas szintű elvekhez igazítani és értékelni a modelleket, például hogy legyenek segítőkészek, ártalmatlanok és őszinték. A gyakorlatban a fejlesztők ezt úgy próbálják elérni, hogy az AI modelleket emberek demonstrációi és visszajelzései alapján finomhangolják. Például az AI modellek finomhangolásának egyik fő paradigmája, amelyet „reinforcement learning from human feedback” néven ismernek, arra épül, hogy a modelleket olyan kimenetek előállítására tanítsák, amelyeket az emberi annotátorok pozitívan értékelnek (‡1218). Ugyanakkor az emberektől érkező pozitív visszajelzés hibás helyettesítő mutató a hasznos viselkedésre (‡737, ‡878, ‡1219, ‡1220), és korlátozza az emberi hiba és elfogultság (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Ez több kihíváshoz vezet: a jutalommal megerősített tanulás (reinforcement leaning) során emberi visszajelzésekből finomhangolt modellek néha hízelegnek a felhasználónak, ami „szicofánság” néven ismert (‡358, ‡740, ‡1226, ‡1227); olyan válaszokat adnak, amelyek egyes kontextusokban hasznosak, másokban viszont károsak (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); olyan válaszokat adnak, amelyeket nehéz helyesség szempontjából értékelni (‡1233); vagy olyan cselekvéseket hajtanak végre, amelyek hasznossága vagy károssága vélemény kérdése (‡1234). A 3.7 Táblázat ezekre a kihívásokra mutat példákat. Egyes kutatások célja olyan módszerek kifejlesztése, amelyek segítik az embereket abban, hogy jobban értékeljék a komplex feladatok megoldásait AI-támogatással (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Ezek a módszerek azonban jelenleg korlátozott megbízhatóságúak, és nem ismert nyilvánosan, hogy mennyire használják őket a mai, legfejlettebb AI-modellek betanításához.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sycophancy/behízelgés (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Magyarázat:
>white|black|left|11|13|br A modell csak pozitív visszajelzést ad, és nem jelzi a helyes 5-7-5 haiku szótagszerkezet hiányát.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Néhány művelet bizonyos kontextusokban hasznos, más kontextusokban pedig káros (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Magyarázat:
>white|black|left|11|13|br A biológiai kockázattal kapcsolatos információk felhasználhatók oktatási és védelemi célokra, ugyanakkor arra is, hogy tájékoztassák a rosszindulatú szereplőket.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb A helyes viselkedés nehezen ellenőrizhető (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Magyarázat:
>white|black||11|13|br Ennek a válasznak a helyessége nehezen ítélhető meg, mert orvosi szaktudást igényel. Még egy tapasztalt orvos számára is az ilyen jellegű válaszok értékelése időt és alapos odafigyelést igényel.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Az emberek nem értenek egyet abban, mi a helyes (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Magyarázat:
>white|black|left|11|13|br A feesek jelentősen eltérnek abban, hogy mi a helyes válasz.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.7. táblázat: Felhasználói prompt és AI-modell válasza
>white|black||9|11|br Példák kihívásokra az AI modellektől származó előnyös cselekvések megadásának és ösztönzésének meghatározása során.


>white|orangered|left|14|15.5|bb Az emberek nem mindig értenek egyet abban, hogy mely viselkedések tekinthetők kívánatosnak, ezért olyan módszerekre van szükség, amelyek összehangolják az egymással versengő preferenciákat.

Az emberek nem mindig értenek egyet abban, hogy az AI modellek milyen válaszokat vagy cselekvéseket adhatnak, illetve mit nem adhatnak ki (‡1006). Ez alapvetően megnehezíti olyan modellek fejlesztését, amelyek cselekvései és hatásai széles körben összhangban vannak a társadalom érdekeivel (‡420). Néhány kutató azt vizsgálja, hogy az AI rendszerekben milyen preferenciák tükröződnek (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249), és olyan „pluralisztikus összehangolás” (pluralistic alignment) technikák kidolgozásán dolgozik, amelyek célja az egymással versengő preferenciák közötti egyensúly megteremtése (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Például az AI fejlesztők úgy tervezhetnek rendszereket, hogy elkerüljék a vitatott válaszok generálását azáltal, hogy bizonyos kérésekre nem válaszolnak, vagy igazodnak az emberek egy releváns mintájában a medián nézőponthoz, illetve személyre szabják a rendszereket az egyes felhasználók számára.

Ezeknél a megközelítéseknél gyakori kihívás, hogy általánosságban az AI-rendszerek nem tudnak mindenki preferenciáival egyformán jól összhangba kerülni, és hogy a társadalomra gyakorolt közvetlen következményeik az egyes csoportokat eltérően érintik. Néhány kutató úgy érvelt, hogy a pluralisztikus összhanghoz kapcsolódó legtöbb technikai megközelítés nem kezeli a mélyebb kihívásokat, sőt potenciálisan el is tereli a figyelmet olyan problémákról, mint a rendszerszintű torzítások, a társadalmi hatalmi dinamika, valamint a vagyon és befolyás koncentrációja (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Az AI-fejlesztők a „kártékony tanítást” használják a modell robusztusságának javítására

Kihívást jelent annak biztosítása, hogy a mesterséges intelligencia (AI) modellek robusztusan képesek legyenek a betanítás során megtanult hasznos viselkedések átültetésére a valós környezetekben történő alkalmazás (deployment) során. Még a „tökéletes” tanulási jel alapján betanított modellek is elbukhatnak abban, hogy sikeresen általánosítsanak az összes, korábban nem látott kontextusra (‡738, ‡739, ‡1255, ‡1256, ‡1257). Például egyes kutatók arra jutottak, hogy a csevegőrobotok nagyobb valószínűséggel hajtanak végre káros cselekvéseket azokban a nyelvekben, amelyek alulreprezentáltak a betanítási adataikban (‡159, ‡880, ‡1258*, ‡1259), ideértve számos, túlnyomórészt a Globális Délben beszélt nyelvet.

Az elmúlt években a kutatók létrehoztak egy kiterjedt eszköztárat az úgynevezett „ellenséges támadás” technikákból, amelyek felhasználhatók arra, hogy a modellek potenciálisan káros válaszokat generáljanak (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Például egy nemrégiben indított kezdeményezés több mint 60,000 különböző, sikeres támadásra vonatkozó példát gyűjtött össze a közösség bevonásával a legkorszerűbb AI modellek ellen, amelyek miatt a modellek megsértették a vállalatoknak az elfogadható modellviselkedésre vonatkozó irányelveit (‡1149). A 3.8. Táblázat olyan példákat mutat be a „jailbreak” technikákra, amelyeket a kutatók bizonyítottak, hogy képesek a modelleket arra kényszeríteni, hogy káros kéréseknek tegyenek eleget.

A modellek robusztusságának javítására ismert egyik módszer az „adversarial training” (‡1064). Ez magában foglalja olyan „támadások” (pl. jailbreak-ek) konstruálását, amelyek célja, hogy egy modellt nem kívánatosan viselkedésre bírjanak, majd a modellt arra képezik, hogy ezeket a támadásokat megfelelően kezelje. Azonban az adversarial training tökéletlen (‡1260, ‡1261). A támadók folyamatosan képesek új, sikeres támadásokat kifejleszteni a legkorszerűbb modellek ellen (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Mivel a fejlesztőknek a tanításhoz konkrét példákra van szükségük a hibamódokról (‡512, ‡1263), az eredmény egy folyamatos „macska-egér” játék, amelyben a fejlesztők a frissen felfedezett sebezhetőségek nyomán folyamatosan frissítik a modelleket, a támadók pedig folyamatosan új támadásokat keresnek. Néhány kutató nagyobb léptékű adversarial traininget (‡1264, ‡1265) vagy új algoritmusokat (‡675, ‡676, ‡1263, ‡1266, ‡1267) javasolt a robusztusság javítására, de a modern AI-rendszerek továbbra is tartósan sérülékenyek.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratégia: Tegyen káros kéréseket titkosított szövegben, például Morse-kóddal (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratégia: Példák bemutatásával felkészíteni a rendszert a káros kérésekre adott, megfelelési válaszokból (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratégia: Káros kéréseket tegyen alacsony erőforrású nyelveken, amelyek valószínűleg kevésbé szerepelnek a betanításban (pl. szuahéli (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Stratégia: A káros feladatot bontsa fel több ártalmatlan részfeladatra (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Táblázat 3.8: Jailbreaking stratégiák
>white|black||9|11|br A rosszindulatú szereplők és a red teamek különféle típusú „jailbreak”-eket használtak annak érdekében, hogy a káros kérésekre adott, általában a biztonsági korlátok miatt visszautasított válaszokat az AI-modellek mégis teljesítsék. A példakimeneteket a jelentés szerzői írták szemléltetési célokból. A jelenlegi, élvonalbeli AI-modellek többsége már ellenáll e módszerek nagy részének, azonban folyamatosan új jailbreaking technikákra derül fény.


>white|orangered|left|14|15.5|bb Az „elfelejtés” technikák képesek enyhíteni a káros modellképességek bizonyos fajtáit

Az általános célú AI-ból eredő kockázatok mérséklésének egy másik stratégiája, hogy a modelleket finomhangolással úgy hozzák létre, hogy bizonyos, nagy kockázatú területeken ne legyenek képességeik (‡1175, ‡1176). Például kutatók olyan „gépi felejtés” (machine unlearning) algoritmusok fejlesztésén dolgoznak, amelyek kifejezetten képesek elnyomni a biothreat-ekkel kapcsolatos készségeket, illetve a meztelen emberi testek fotórealisztikus képeinek generálásához kötődő képességeket (‡903, ‡1272, ‡1273). Ezek a módszerek a modelleket jelentősen biztonságosabbá tehetik, azzal a költséggel, hogy korlátozzák a felejtés tárgyát képező képességek bizonyos pozitív felhasználásait. A káros területeken való AI-modellek ismereteinek korlátozását „manipulációtűrő” (tamper-resistant) nyílt súlyú (open-weight) modellek tervezésének módjaként is javasolták, amelyek ellenállnak a káros finomhangolásnak (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Mindeddig azonban ezt nem sikerült kellően megbízhatóan megvalósítani (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). A további megbeszélésért lásd a §3.4. Nyílt súlyú (open-weight) modellek című részt.

>white|orangered|left|14|15.5|bb Néhány kutató olyan módszereken dolgozik, amelyek erősebb biztonsági garanciákat nyújtanak azáltal, hogy a modell belső állapotait értelmezik, vagy matematikai ellenőrzést (verifikációt) végeznek.

Néhány kutató olyan módszereken dolgozik, amelyekkel szigorúbban lehet ellenőrizni a modellekkel kapcsolatos biztonsági tulajdonságokat. Az egyik megközelítés szerint a kutatók a modellek belső számításainak értelmezését célozzák: vagy így azonosítják a kockázatokat, vagy pedig meggyőzőbb érveket tudnak megfogalmazni arról, hogy a modell biztonságos (‡1285, ‡1286). Például egy koncepció-bemutatóban a kutatók azt mutatták, hogy a nyelvi modellek belső számításait elemző eszközök segíthetnek az értékelőknek azonosítani a káros viselkedéseket (‡1287). 2025-ben az Anthropic is elkezdte a modellbelsők elemzését a modell helyzeti tudatosságának és „intencíójának” tanulmányozására (‡2). Ugyanakkor az ilyen típusú módszerek jelenleg nem elterjedtek, vagy nem ismert, hogy versenyképesek lennének más értékelési technikákkal.

A biztonságosságra vonatkozó erősebb garanciák nyújtásának egy másik megközelítése matematikai bizonyítások felépítése, amelyek azt igazolják, hogy a modell teljesíteni fog bizonyos biztonsági feltételeket (‡1177, ‡1282, ‡1288). Ugyanakkor ezek a bizonyítások abból indulnak ki, hogy a tesztelési környezet megegyezik az üzembe helyezési környezettel, és nem lettek kellőképpen bevizsgálva sokféle típusú támadóval szemben.

Jelenleg emellett nem is skálázhatók nagyméretű modellekre. Összességében jelentős vita zajlik a szakértők körében az értelmezhetőség és a formális verifikációs módszerek ígérete kapcsán.

###@ Telepítési időszak alatti monitorozás és vezérlés

A modellfejlesztés során bevezetett biztosítékokon túl a káros viselkedések elleni második védelmi vonalat a külső biztosítékok jelentik, amelyek a telepítés során a modell vagy rendszer műveleteinek figyelésére és ellenőrzésére összpontosítanak. Az ilyen biztosítékok segítenek csökkenteni a hibás működés és a visszaélés kockázatát, például a hallucinált kimeneteket és a káros utasításokat.

>white|orangered|left|14|15.5|bb A modell-deployerek különféle eszközöket használhatnak a magas kockázatú modell-viselkedések azonosítására és kezelésére

Amikor egy MI-rendszer fut, a telepítő (deployer) figyelhet a kockázat jeleire, és beavatkozhat, ha azok megjelennek. Például ellenőrizhetik egy modell bemeneteit az adverzárius támadások jelei szempontjából, kiszűrhetik a nem megfelelő tartalmat a kimenetekből, vagy figyelhetik a rendszer gondolatláncát (chain of thought) a káros tervek jeleire. Azok a pontok, ahol a telepítők nyomon követhetik és beavatkozhatnak abba, ahogyan az emberek használják a rendszereiket, többek között a hardver (‡1180, ‡1181), a felhasználói interakciók (‡1154, ‡1166), a bemenetek és kimenetek (‡65, ‡725, ‡1182), a belső számítások (‡744, ‡1183, ‡1184) és a gondolatlánc (‡430, ‡435). Emellett többféle műveletet is elvégezhet a telepítő, amikor kockázatokat azonosítanak. Ezek közé tartozik az információk naplózása, a káros tartalom szűrése/módosítása, a rendellenes aktivitás jelzése, a rendszer leállítása, vagy a biztonsági zárolások (failsafes) aktiválása. A 3.7. Ábra a gyakori monitorozási és vezérlési mechanizmusok példáit szemlélteti.

Mivel ezek a mechanizmusok sokoldalúak és gyakran hatékonyak, széles körben alkalmazzák őket, és sokféle, nem szándékos kár megelőzésére alkalmasak (‡725, ‡751, ‡1289). Ugyanakkor ezek a biztosítékok tökéletlenek, különösen rosszindulatú támadások esetén, amelyeket kifejezetten úgy optimalizálnak, hogy azok meghiúsuljanak (‡752, ‡1182). A közelmúlt kutatásai azt is vizsgálták, hogy a monitorozás megbízhatatlanná válhat, ha a rendszert egy monitor pontszámai alapján optimalizálják; például úgy, hogy a láncolt gondolatok (chain of thought) kevésbé legyenek megbízhatóak (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Ábra 3.7: Felügyeleti és vezérlési technikák
>white|black||9|11|br A felügyeleti és vezérlési technikák több ponton működnek: a bemenetek és kimenetek szűrése a káros tartalom szempontjából, a modell belső állapotainak nyomon követése, a külső műveletek korlátozása sandboxinggal, valamint az emberi felügyelet fenntartása. Forrás: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb A humán felügyelet a körben lehetővé teszi a közvetlen ellenőrzést nagy tétű helyzetekben

Az AI-ügynökökből eredő meghibásodások esélyének csökkentése érdekében (lásd a §2.2.1. Reliability challenges részt) a telepítők törekedhetnek olyan AI-rendszerek tervezésére, amelyek az emberekkel együttműködve működnek, nem pedig teljesen autonóm módon (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Ez különösen fontos olyan felhasználási esetekben, ahol a helytelen döntések jelentős kárt okozhatnak, például a pénzügyekben, az egészségügyben vagy a rendőrségi alkalmazásokban. Ugyanakkor a „humán közbeiktatás” (human in the loop) gyakran kivitelezhetetlen. Néha a döntéshozatal túl gyorsan történik, például a több millió felhasználóval rendelkező csevegőalkalmazások esetében. Más esetekben az emberi torzítás és hiba felerősítheti a kockázatokat a kumulatív hibák miatt (‡1187). A humán szereplők a folyamatban emellett gyakran mutatnak „automatizálási torzítást” (automation bias), ami azt jelenti, hogy több bizalmat helyeznek az AI-rendszerbe, mint amennyire az indokolt (‡1190, ‡1191) (lásd a §2.3.2. Risks to human autonomy részt).

>white|orangered|left|14|15.5|bb A „Sandboxolás” védelmet nyújt az autonóm viselkedésekből eredő kockázatok ellen

Az AI-ügynökök, amelyek autonóm módon, korlátozás nélkül képesek cselekedni az interneten vagy a fizikai világban, fokozott kockázatokat jelentenek (lásd §2.2.1. Megbízhatósági kihívások). A „szandboxolás” az AI-ügynököknek a világgal való közvetlen befolyásolásra szolgáló lehetőségeinek korlátozását jelenti, így sokkal könnyebb őket felügyelni és kezelni (‡640, ‡1192, ‡1295). Például egy AI-rendszernek az internetre történő közzétételre vagy a számítógép fájlrendszerének szerkesztésére való képességének korlátozása meg tudja előzni az előre nem látható, váratlan cselekvésekből eredő károkat (‡1296). Ugyanakkor ezek az eljárások nem mindig alkalmazhatók olyan alkalmazásokban, ahol az AI-rendszernek feltétlenül közvetlenül kell cselekednie a világban.

###@ Ökoszisztéma-figyelő eszközök: modell- és adatproveniencia

A modell- és adatproveniencia-eszközök technikai eszközök az AI-ökoszisztéma tanulmányozásához, a mesterséges intelligencia rendszerek felhasználásának és hatásainak a tudatosításának javítása érdekében.

>white|orangered|left|14|15.5|bb Az AI-rendszer eredetiségére vonatkozó technikák segítenek nyomon követni a rendszerek felhasználását és hatásait

A fejlesztők és a telepítők különféle technikákat alkalmazhatnak a modellhasználat tanulmányozására és a „vadonban” történő terjedés vizsgálatára. Például adhatnak a modelleknek egyedi azonosító viselkedéseket (‡1193, ‡1297, ‡1298, ‡1299, ‡1300), vagy egyedi mintákat alkalmazhatnak az egyes nyílt súlyú (open-weight) modellek súlyaira (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Ugyanakkor ezeknek a technikáknak a modellmódosításokkal szembeni ellenállóbbá tétele nyitott probléma (‡1195, ‡1196*). A kutatók emellett módszereket is dolgoznak a „modellörökség” (model heritage) következtetésére (‡1197, ‡1198, ‡1305, ‡1306), amelyek segítenek megválaszolni az olyan kérdéseket, mint: „Az X modell egy Y modellből finomhangolással (fine-tuned) vagy lepárlással (distilled) készült változat volt-e?” Végül egyes fejlesztők olyan protokollokon és infrastruktúrán dolgoznak, amelyek lehetővé teszik, hogy az AI-ügynökök (AI agents) azonosítást és ellenőrzést végezzenek, amikor külső rendszerekkel lépnek kapcsolatba (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Ábra 3.8: A vízjelek észrevétlen zavarásokat ágyaznak be a képekbe és a hangokba
>white|black||9|11|br A vízjelek észrevehetetlen zavarásokat ágyaznak be képekbe és hanganyagokba, amelyek lehetővé teszik, hogy az AI-generált tartalmakat észlelő eszközök azonosítsák. Ebben az ábrában a kép- és hang-vízjelek is túl vannak hangsúlyozva a jobb láthatóság érdekében. Forrás: Chameleon kép az Unsplashról (‡1313*). A további elemeket a Report szerzői készítették. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Ábra 3.9: Promptinjection támadások sikerarányai
>white|black||9|11|br A promptinjekciós támadások sikerességi arányai, amelyeket az AI-fejlesztők jelentettek a 2024 májusa és 2025 augusztusa között kiadott jelentősebb modellek esetében. Minden pont az adott modell ellen a kiadást követően röviddel végrehajtott 10 kísérletből a sikeres támadások arányát jelenti. Az ilyen támadások jelentett sikerességi aránya az idő előrehaladtával csökkenő tendenciát mutat, de továbbra is viszonylag magas. Forrás: Zou et al. 2025 (‡1149), idézve Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Az AI-tartalomészlelési technikák segítenek nyomon követni az AI által generált tartalom terjedését és hatásait

A vízjelek, a metaadatok és más AI-tartalomdetektorok segíthetnek a kutatóknak az AI-val készített tartalmak valós hatásának nyomon követésében és tanulmányozásában. 

Először is, az adat-védjegyek (data watermarks) olyan finom, de elkülöníthető mintázatok, amelyeket digitális médiába illesztenek be, és amelyek információt kódolhatnak a forrásukról (‡1199, ‡1200, ‡1201*). Szöveg esetén jellemzően a szóválasztásban és a stílusban megjelenő enyhe torzítások formáját öltik (‡1308, ‡1309); képek és videó esetén a pixelek felett elhelyezkedő finom mintázatokét (‡1310); hang esetén pedig a hanghullámokban megjelenő finom mintázatokét (‡1311). A 3.8. Ábra ezeket szemlélteti.

A vízjeleken kívül a mesterséges intelligencia által generált tartalom olyan fájlformátumokban is menthető, amelyek a generálás módjára vonatkozó metaadatokat tárolnak. Például sok mobileszköz a kép- és hangfájlokat olyan fájlformátumban menti, amely képes információt tárolni a kamerabeállításokról, az időpontról, a helyről stb. (‡1312). Hasonló metaadatok felhasználhatók annak az információnak a tárolására is, hogy az adatot egy AI-rendszer hozta-e létre. A bűnügyi igazságügyi kriminalisztikában használt ujjlenyomatokhoz hasonlóan a vízjelek és a metaadatok is manipulálhatók vagy eltávolíthatók, mégis hasznosak.

A kutatók emellett azon is dolgoznak, hogy kifejlesszenek AI-generált tartalom észlelők (‡1203, ‡1204, ‡1205*) segédeszközt, amelyek célja a mesterségesen generált tartalom azonosítása a való világban is, még akkor is, ha nincs elérhető watermarker vagy metaadat. Ugyanakkor ezeknek az azonosítási technikáknak korlátozott a sikerarányuk.

###@ Frissítések

A legutóbbi Jelentés (2025 január) közzététele óta előrehaladás történt olyan AI-rendszerek fejlesztésében, amelyek több, hatékony biztosítékréteggel rendelkeznek. Amint azt a §3.2. Kockázatkezelési gyakorlatok tárgyalják, a védelem mélységben elv a kockázatkezelés alapelve (‡1314). Például az olyan AI-rendszereket, amelyek biztonságra betanított modelleket bemeneti szűrőkkel, kimeneti szűrőkkel és egyéb tartalomfigyelőkkel kombinálnak, egyre gyakrabban vizsgálják és telepítik (‡32, ‡65, ‡1182*). A közelmúlt kutatásai emellett azt is kimutatták, hogy bár a modellfejlesztők előrehaladást értek el a biztosítékok megkerülésére tett kísérletekkel szembeni robusztusság növelésében, a támadók még mindig magas arányban járnak sikerrel (3.9 Ábra).

###@ Bizonyítéki hiányosságok

További bizonyítékokra van szükség ahhoz, hogy a kutatók jobban megértsék és figyelembe vegyék a meglévő megközelítések korlátait. Az AI-rendszerekhez tartozó technikai biztosítékokat javítják, de a módszerek korlátokkal küzdenek. Például a nagy általánosságú célú AI-rendszerek legrosszabb esetre vonatkozó robusztusságának javításában elért előrelépés lassú volt, és alapvető korlátok vannak azzal kapcsolatban, hogy mennyire alaposan lehet biztosítékokkal ellátni és monitorozni a nyílt súlyokkal rendelkező modelleket (‡1195, ‡1315, ‡1316) (lásd még §3.4. Nyílt súlyokkal rendelkező modellek). Eközben nem minden technikai biztosíték egyformán gyakori, egyformán hatékony, illetve egyformán bizonyított a valós világban. Például az adversariális betanítást szinte mindenhol alkalmazzák a korszerű modellek esetében (‡64*, ‡677), míg a modellek értelmezhetőségével és a formális verifikációval foglalkozó technikákat eddig kevéssé használták a termelési rendszerekben (‡1177, ‡1285).

###@ Kihívások a döntéshozók számára

A döntéshozók számára a legfontosabb kihívások közé tartozik annak eldöntése, hogy és hogyan támogassák-e a kutatást, fejlesztést, értékelést, valamint a műszaki biztosítékok és felügyeleti módszerek bevezetését. Ez azért nehéz, mert a kutatók még mindig alakítják azt a megértésüket, hogy a mechanizmusok gyakorlati védelme szempontjából mi a legjobb módszer, és a bevált gyakorlatok még nincsenek kialakítva. Például a különböző fejlesztők különböző biztosítékokat alkalmaznak, és a műszaki kockázatcsökkentéshez való hozzáállásuk – tágabb értelemben – is igen széles skálán mozog (‡1116). Végül, a hatékony műszaki biztosítékok megléte önmagában nem garantálja a biztonságot, mivel a bevezetés és az alkalmazás fejlesztők és telepítési környezetek szerint eltérhet.

