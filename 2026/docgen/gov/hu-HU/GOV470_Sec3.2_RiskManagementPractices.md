##########
>white|orangered|left|14|30|hr 3.2. fejezet
### 3.2. Kockázatkezelési gyakorlatok
>white|orangered|left|24|30|hb Kockázatkezelési gyakorlatok

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb Fontos információk
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Az általános célú AI kockázatkezelése olyan gyakorlatok széles körét foglalja magában, amelyek az általános célú AI-ból eredő kockázatok azonosítására, értékelésére és csökkentésére szolgálnak. Ezek közé tartozik a model-szintű tesztelés és értékelés (például a „red-teaming”), a szervezeti folyamatok, amelyek fejlesztési és kiadási döntéseket irányítanak, feltételes biztosítékok (például „if-then” kötelezettségvállalások), valamint az incidensek jelentése.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Több AI-fejlesztő is létrehozott Frontier AI Safety keretrendszereket. Ezek a keretrendszerek információkat tartalmaznak kockázatértékelésekről, és olyan feltételes intézkedéseket is megadnak, mint például az elérhetőbb modellekhez kapcsolódó vállalati hozzáférés-korlátozások, amelyeket a vállalatok terveznek bevezetni. Abban különböznek, hogy milyen kockázatokat fednek le, hogyan határozzák meg a képességi küszöböket, és milyen lépések indulnak el, amikor a küszöbértékek elérésre kerülnek.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A mesterséges intelligencia kockázatkezelési gyakorlatainak valós, a gyakorlatban mért hatékonyságáról szóló bizonyítékok továbbra is korlátozottak. Az incidensek bejelentésének és a monitorozásnak a hiánya megnehezíti annak értékelését, hogy a jelenlegi gyakorlatok mennyire csökkentik ténylegesen a kockázatokat, illetve mennyire következetesen kerülnek bevezetésre.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ A legutóbbi Jelentés (2025 január) közzététele óta a kockázatkezelés a friss iparági és irányítási kezdeményezések révén strukturáltabbá vált. Olyan új eszközök, mint az EU Általános célú MI Kódexgyakorlata, Kína MI-biztonsági kormányzási keretrendszere 2.0, valamint a G7 Hiroshima MI-folyamat-jelentési keretrendszere, a vállalati kezdeményezésekkel együtt azt a tendenciát mutatják, hogy a transzparencia, az értékelés és az incidensjelentés tekintetében egyre inkább szabványosított megközelítések felé mozdulunk.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A piaci dinamika és a mesterséges intelligencia fejlesztésének üteme további kihívásokat jelent. A versenyhelyzet miatt az MI-vállalatok döntési kényszerekkel szembesülhetnek a gyorsabb termékkiadások és a kockázatcsökkentési erőfeszítésekbe való befektetések között. Sok MI-vel kapcsolatos károkozás is külső hatásként jelentkezik, és a velük összefüggő jogi felelősség továbbra is tisztázatlan, miközben a kormányzási folyamatok lassan alkalmazkodhatnak az MI-környezettel bekövetkező változásokhoz.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ A döntéshozók legfontosabb kihívásai közé tartozik a generikus célú mesterséges intelligencia által jelentett különféle kockázatok közötti prioritások meghatározása, valamint annak tisztázása, hogy az AI-értéklánc mely szereplői vannak a legjobb helyzetben azok mérséklésére. E kihívásokat súlyosbítja a korlátozott rálátás arra, hogy a kockázatokat a gyakorlatban miként azonosítják, értékelik és kezelik, továbbá a fejlesztők, az üzemeltetők és az infrastruktúra-szolgáltatók közötti töredezett információmegosztás.
>oldlace|black||11|15|br      


Az AI-kockázatkezelés olyan gyakorlatok széles körét foglalja magában, amelyek célja az AI-rendszerekhez kapcsolódó kockázatok valószínűségének és súlyosságának azonosítása, felmérése, valamint csökkentése. Ezeket a gyakorlatokat az AI-fejlesztők, az üzembe helyezők, az értékelők és a szabályozók egyaránt alkalmazhatják. Ilyen például a fenyegetésmodellezés, a kockázati szintekbe sorolás, a red-teaming, az auditálás és az incidensjelentés. Ez a szakasz bemutatja a jelenlegi kockázatkezelési gyakorlatokat, az új fejlesztéseket, valamint a fennmaradó korlátokat.

2025 eleje óta több új nemzetközi kezdeményezés is kidolgozásra került az általános célú mesterséges intelligencia kockázatkezelésére vonatkozóan, ideértve a szervezeti átláthatóságot és a kockázatjelentési keretrendszereket, valamint a szabályozási és irányítási keretrendszereket.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Ábra 3.4: A kockázatkezelés négy összetevője
>white|black||9|11|br Az általános célú mesterséges intelligencia kockázatkezelésének módszereit lefedő négy kategória: kockázatazonosítás; kockázatelemzés és -értékelés; kockázatcsökkentés; valamint kockázatirányítás. Ezek egy iteratív és ciklikus folyamatot alkotnak. A középen ábrázolt kockázatirányítás elősegíti a többi komponens sikerét. Forrás: International AI Safety Report 2026.


A fennmaradó kihívások közé tartozik a korlátozott szabványosítás, ami megnehezíti a megfelelőség és az értékelés biztosítását, továbbá a korlátozott bizonyíték a valós környezetben tapasztalható hatékonyságról. Emellett az intézményi, kulturális és politikai kontextusok világszerte eltérnek, ami azt jelenti, hogy a kockázatok azonosítására és kezelésére irányuló megközelítések, beleértve az elfogadható kockázati küszöbértékeket, régiónként eltérhetnek. A jelen szakasz kockázatkezelési megközelítésekről szóló tárgyalása leíró jellegű: célja, hogy tájékoztassa az AI ökoszisztémában érintett szereplőket a kockázatkezelés jelenlegi globális megközelítéseiről. Ahol rendelkezésre áll, szó esik ezen megközelítések hatékonyságáról és korlátairól szóló bizonyítékokról, azonban a szakpolitikai ajánlások e munka hatókörén kívül esnek.

###@ A kockázatkezelés összetevői

A kockázatkezelés iteratív folyamat, olyan gyakorlatokkal és módszerekkel, amelyek az AI fejlesztésének és telepítésének teljes életciklusát lefedik, ugyanakkor koherensen együttműködnek (‡969). Az általános célú AI kockázatkezelése magában foglalhat szerepeket igen széles körű érintettek számára, többek között adattudósok, modellező mérnökök, auditálók, szakterületi szakértők, vezetők, végfelhasználók, érintett közösségek, harmadik fél beszállítói, szakpolitikai döntéshozók, kormányok, szabványügyi szervezetek, valamint civil társadalmi szervezetek számára (‡970, ‡971, ‡972). A vezető kockázatkezelési szabványok gyakran együttműködtethetők, de eltérő terminológiát használnak a kockázatkezelés elemeinek leírására (‡973, ‡974). Tipikusan négy, egymással összekapcsolt komponenst tartalmaznak (3.4. Ábra): a kockázatok azonosítását; elemzését és értékelését; a kockázatok mérséklését; és a kockázatok kormányzását (‡970, ‡973, ‡975, ‡976). Az alábbi táblázatok a releváns módszerekre, technikákra és eszközökre vonatkozó szemléltető példákat mutatnak be. A gyakorlatok folyamatosan fejlődnek, ezért a táblázatok nem teljes körűek, és az alkalmazhatóság kontextusonként eltérő lesz.

###@ Kockázatazonosítás

A kockázatazonosítás a kockázatok feltárásának, felismerésének és leírásának folyamata. Az átfogó kockázatazonosítás jellemzően képességvezérelt értékeléseket foglal magában, amelyek azt vizsgálják, hogy a modellek rendelkeznek-e meghatározott veszélyes képességekkel (‡977), valamint kockázatmodellezést (‡978) és előrejelzést (‡715*), amelyeket az aktuális és a feltörekvő kockázatok feltérképezésére használnak. A 3.1. Táblázat a kockázatazonosítás különféle gyakorlataira mutat példákat. A kockázatazonosítás emellett a releváns szakértőkkel és közösségekkel folytatott egyeztetésekre is támaszkodik, hogy megértsék azt a tágabb kontextust, amelyben a kockázatok kialakulnak (‡979, ‡980). Az olyan mechanizmusok, mint a bug bounty programok, e folyamatot azáltal támogathatják, hogy ösztönzik a korábban ismeretlen sebezhetőségek azonosítását (‡981) (3.1. Táblázat). A kockázatazonosítás egyik fő célja, hogy számot adjon mind a jól ismert, jól értett kockázatokról, mind pedig a lehetséges jövőbeli kockázatokról, amelyek még bizonytalanok vagy rosszul vannak jellemezve (‡982). Ez különösen fontos az általános célú mesterséges intelligencia esetében, ahol sok kockázat még nem teljesen ismert vagy nem megfigyelhető (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bug bounty programok
  A bug bounty programok vagy sérülékenység-bejelentési programok arra ösztönzik az embereket, hogy sebezhetőségeket találjanak az AI-rendszerekben, és bejelentsék azokat. Több fejlesztő is bevezetett bug bounty programokat (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Szakértői konzultáció
  A területi szakértők, a felhasználók és az érintett közösségek betekintést nyújtanak a várható kockázatokba. Egyre több részvételen alapuló és befogadó AI-ra vonatkozó iránymutatás jelenik meg (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halcsont (Ishikawa) diagram
  A halszálka diagramok jól bevált okfeltáró (root cause analysis) eszközök, és a kutatók javasolták ezek alkalmazását az MI-kockázati incidensek strukturált elemzésére (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Előrejelzés
  Az előrejelzés a jövőbeli események vagy trendek előrejelzésének folyamata a múltbeli és jelenlegi adatok elemzése alapján. Arra használták, hogy például a fejlett MI-nek köszönhetően különböző gazdasági kimenetelek relatív valószínűségét összehasonlítsák (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázati taxonómia
  A kockázati taxonómiák a kockázatok több dimenzió mentén történő kategorizálására és rendszerezésére szolgáló eszközök. Több olyan is létezik, amelyek a általános célú MI-ből (‡906, ‡988) eredő kockázatokat vázolják fel.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Forgatókönyv-tervezés
  A szcenáriótervezés magában foglalja valószerű jövőbeli szcenáriók kidolgozását, valamint annak elemzését, hogyan valósulnak meg a kockázatok. Ezt a mesterséges intelligencia modellek kockázatainak és hatásainak feltárására használták (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Fenyegetésmodellezés
  A fenyegetésmodellezés egy folyamat a rendszerrel szembeni fenyegetések és sebezhetőségek azonosítására. Számos AI-fejlesztő hangsúlyozza a fenyegetésmodellezés használatát az AI-rendszerek lehetséges visszaélési forgatókönyveinek előrejelzésére (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.1. Táblázat: Kockázatazonosítási példák általános célú mesterséges intelligencia kockázatkezelésben
>white|black||9|11|br Az AI-kockázatok azonosítására szolgáló példamódszerek betűrendben vannak felsorolva. A módszerek a következők:
úgy vannak kialakítva, hogy különféle kockázattípusok esetén támogassák a kockázatok azonosítását, beleértve a rosszindulatú felhasználásból eredő kockázatokat, a meghibásodásokból eredő kockázatokat és a rendszerszintű kockázatokat is. Mivel a célorientált (általános célú) AI-kockázatkezelés még kialakulóban van, nem minden módszer lesz alkalmas minden AI-fejlesztő vagy -üzemeltető számára.


>white|orangered|left|14|15.5|bb A fenyegetésmodellezés és a kockázati taxonómiák kiemelkedő kockázatazonosítási módszerek

A kockázatok azonosítására szolgáló két kiemelkedő módszer az általános célú AI-ból fakadó fenyegetések feltárása: a threat modelling (nemzetközi AI biztonsági jelentés 2026), amely egy strukturált folyamat az AI-hoz kapcsolódó kockázatok lehetséges bekövetkezési módjainak feltérképezésére, valamint a risk taxonomies. A Meta például threat modelling gyakorlatokat alkalmaz annak érdekében, hogy előre jelezze az AI modelljeinek lehetséges visszaélési forgatókönyveit (‡990), az Anthropic pedig a threat modelling-et beépíti az ASL-3 Deployment Standardjába (‡991). Az AI kockázati és hazard taxonomies, amelyek kockázati kategóriákat és példákat sorolnak fel, kiindulópontként ugyanúgy szolgálhatnak a fogalmi megragadáshoz, az azonosításhoz és a releváns kockázatok meghatározásához az általános célú AI-hoz kapcsolódóan konkrét alkalmazási területeken (‡906, ‡988, ‡992, ‡993).

###@ Kockázatelemzés és értékelés

A kockázatelemzés és -értékelés az az eljárás, amelynek során meghatározzák egy AI-modell vagy -rendszer kockázati szintjét, majd azt az előre rögzített kritériumokkal összevetik annak megállapítására, hogy elfogadható-e, vagy szükség van-e a mérséklésre (‡994, ‡995, ‡996, ‡997). Olyan gyakorlatokat foglal magában, mint a modell teljesítményének mérése benchmarkokon (‡998) és értékeléseken (‡176, ‡715), a red-teaming gyakorlatok lefolytatása (‡999*), a hatásvizsgálatok (‡1000) és az auditok (‡1001, ‡1002). Lásd a 3.2. Táblázatot általános célú AI-kockázatelemzésre és -értékelésre vonatkozó példákért. A módszereket úgy tervezték, hogy egyszerre támogassák az elemzést és az értékelést sokféle kockázattípus esetén.

A kockázatelemzés és értékelés fő céljai a modellképességek és sebezhetőségek (‡1003) értékelésének elvégzése, a kockázatok robusztus modellezésének felhasználása a kockázati küszöbökkel kapcsolatos döntések megalapozására (‡1004, ‡1005), valamint annak megértése, hogy az AI-rendszereket a gyakorlatban hogyan használják, a downstream társadalmi hatások felmérése érdekében (‡869, ‡904, ‡905, ‡1006). A kockázatelemzési és értékelési folyamatokat gyakran úgy tekintik, hogy nagyobb valószínűséggel azonosítanak kockázatokat, ha független felülvizsgálatot is tartalmaznak (‡1001, ‡1007), támaszkodnak ágazatokon átívelő szakértelemre (‡1008), továbbá több területről és tudományágból származó, valamint az érintett közösségekből érkező eltérő nézőpontokat is beépítenek (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditok
  Az auditok az AI-modellek teljesítményének és hatásainak, illetve egy szervezet szabványoknak, irányelveknek és eljárásoknak való megfelelésének formális felülvizsgálatai, amelyeket belsőleg vagy külső fél végzi. Az AI-auditálás gyorsan növekvő terület, és számos eszköz és gyakorlat létezik AI-modellek auditálására, valamint az AI-modellfejlesztők gyakorlatainak auditálására (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarkok
  A benchmarkek szabványosított, gyakran kvantitatív tesztek vagy mutatók, amelyeket az MI-rendszerek teljesítményének értékelésére és összehasonlítására használnak egy rögzített feladatsor alapján, amelyet a valós felhasználást reprezentáló feladatokhoz terveztek (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bowtie módszer
  A masni módszer egy jól ismert módszer annak vizualizálására, hogy hol adhatók be beavatkozások a kockázati események mérséklésére. Egyértelműen megkülönbözteti a proaktív és a reaktív kockázatkezelést (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-módszer
  A Delphi-módszer egy csoportos döntéshozatali technika, amely egymást követő kérdőíveket használ a szakértői paneltől származó konszenzus összegyűjtésére (‡1020, ‡1021). Arra is használták, hogy fejlett MI-vel (‡1022) lehetséges jövőképeket lehessen feltárni.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mezőn végzett tesztelés
  A tereppróbák egy AI-rendszer teljesítményét és hatását értékelik valós, működési környezetben. Egyes kutatások a tereppróbákat a modellértékelés kiegészítéseként hangsúlyozzák a valós kimenetek és következmények felméréséhez (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hatásértékelés
  Az értékelések a technológia vagy projekt lehetséges hatásait mérik fel. Ez magában foglalhatja a hatások számszerűsítését, összesítését és priorizálását. Például az EU AI Act előírja, hogy a magas kockázatú AI rendszerek fejlesztőinek el kell végezniük a Alapvető Jogok Hatásvizsgálatát (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modellértékelés
  A modellértékelések olyan folyamatokat és teszteket foglalnak magukban, amelyekkel az adott feladaton egy AI-modell teljesítményét értékelik és mérik. Számos AI-értékelés létezik a különböző képességek és kockázatok felmérésére, ideértve a biztonságot, a biztonsági (security) területet és a társadalmi hatásokat is (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Valószínűségi kockázatértékelés
  A valószínűségi kockázatértékelés egy olyan módszertan, amely összetett rendszerekhez vagy folyamatokhoz kapcsolódó kockázatok értékelésére szolgál, és amely bizonytalanságot is figyelembe vesz. Ezt a fejlett AI-rendszerekhez is adaptálták (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vörös csapatos tesztelés
  A red-teaming egy olyan gyakorlat, amelynek során egy személyekből vagy automatizált rendszerekből álló csoport úgy tesz, mintha támadóként viselkedne, és egy szervezet technológiai rendszereit támadva azonosítja a sebezhetőségeket. Számos mesterséges intelligencia (AI) vállalat belső eljárásokat alkalmaz az AI-rendszerek red-teamingjére (‡458, ‡1028). A red-teaminget a vállalatokon kívüli szereplők is végezhetik. Az ilyen csapatok olyan kihívásokkal szembesülnek, mint a korlátozott hozzáférés, ugyanakkor eltérő meglátásokat is felszínre tudnak hozni (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázati mátrixok
  A kockázati mátrixok vizuális eszközök a kockázatok rangsorolásának támogatására előfordulásuk valószínűsége és a lehetséges hatásuk alapján (‡1027). Néhány AI-fejlesztő alapvető kockázati mátrixokat is beépít a Frontier AI Safety Frameworks-ekbe (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázati küszöbértékek / kockázati szintek
  A kockázati küszöbök vagy szintek kvantitatív vagy kvalitatív korlátok, amelyek elválasztják az elfogadható kockázatokat a nem elfogadható kockázatoktól, és túllépés esetén meghatározott kockázatkezelési intézkedéseket váltanak ki. Általános célú AI esetén ezeket a képességek, a hatás, a számítási kapacitás, a kitettség és egyéb tényezők együttesen határozzák meg (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázattűrő-képesség
  A kockázattűrés az a kockázati szint, amelyet egy szervezet hajlandó elfogadni. A mesterséges intelligenciában a kockázattűréseket gyakran hallgatólagosan határozzák meg vállalati politikák és gyakorlatok révén, míg egyes szabályozási rendszerek kifejezetten meghatározzák az elfogadhatatlan kockázatokat, és jogi következményeket társítanak hozzájuk (‡1032). Egyes vállalatok a kockázattűrésüket egy új modell marginális kockázatának formájában írják le; vagyis annak mértékében, hogy egy modell ellenpontilag mennyivel növeli a kockázatot a már fennálló kockázatnál, amelyet az existing modellek vagy más technológiák önmagukban is okoznak (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Biztonsági esetek
  A biztonsági eset egy strukturált érvelés, amely bizonyítékokra támaszkodva igazolja, hogy egy rendszer a megadott kontextusban elfogadhatóan biztonságosan üzemeltethető. A közelmúlt szakirodalma (‡1037, ‡1038, ‡1039) a frontier AI rendszerekre vonatkozó biztonsági eseteket vizsgálta, és bizonyos Frontier AI Safety Frameworkek hivatkoznak rájuk (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rendszerbiztonsági elemzés
  A rendszerbiztonsági elemzés kiemeli a komponensek és az általuk alkotott rendszer közötti függőségeket annak érdekében, hogy előre jelezhető legyen, miként alakulhatnak ki rendszerszintű veszélyek komponens- vagy folyamathibákból, illetve alrendszerek közötti kölcsönhatásokból, emberi tényezőkből és környezeti feltételekből. Az irodalomban az AI-rendszerekre alkalmazott megközelítések közé tartozik a rendszerszintű folyamatok elemzése (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.2. Táblázat: Kockázatelemzés/értékelés általános célú mesterséges intelligencia kockázatkezelésében
>white|black||9|11|br Példa módszerek az AI-kockázatelemzéshez/kockázatértékeléshez, ábécé szerinti felsorolásban. A többcélú AI kockázatkezelés korai, kialakuló jellegéből adódóan nem minden módszer lesz alkalmas minden AI-fejlesztő vagy -üzemeltető számára.


>white|orangered|left|14|15.5|bb A közös kockázatelemzési eszközök közé tartoznak a benchmarkok és a modellek értékelései

A benchmarkok és modellszintű értékelések olyan standardizált tesztek, amelyekkel megítélhető az általános célú AI-rendszerek teljesítménye meghatározott feladatokon. A kutatók széles körben dolgoztak ki benchmarkokat és értékeléseket, ideértve a nehéz feleletválasztós kérdésekből álló készleteket, a szoftvermérnöki problémákat, valamint a munkahelyi feladatokat szimulált irodai környezetekben (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). A káros képességek értékelései (‡715) arra szolgálnak, hogy felmérjék: egy általános célú AI-modell vagy -rendszer különösen veszélyes tudással vagy képességekkel rendelkezik-e, például azzal, hogy segíthet a kiber­támadásokban (lásd §2.1.3. Cyberattacks).

A vállalatok és kormányok modellkiadásokkal kapcsolatos erősen következményes döntései részben ezekre az értékelésekre támaszkodnak (‡1050, ‡1051, ‡1052). Ugyanakkor a benchmarkok minősége és hatóköre jelentősen eltér (‡998, ‡1003), és nehéz lehet érvényességüket megítélni a benchmarkolási gyakorlatok számos hiányossága miatt (‡902, ‡909, ‡1003, ‡1053*). Például a benchmarkok „telítődhetnek” – amikor sok model pontszámai a legmagasabb pontszámhoz közelítenek –, ami azt jelenti, hogy már nem különböztetik meg erősen a modelleket egymástól. A modellek emellett egyre nagyobb valószínűséggel képesek bizonyos feladatokat értékelésként felismerni, és a bevezetési (deployment) kontextusban a hasonló feladatokon tapasztalttól eltérő viselkedést mutatni a „helyzeti tudatosság” miatt (lásd §2.2.2. Kontrollvesztés). Végül a benchmarkoknak és az értékeléseknek jól dokumentált korlátai vannak: nevezetesen nem képesek megragadni az általános célú mesterséges intelligencia új területeken és új feladatoknál történő alkalmazásához kapcsolódó kockázatokat, mivel a tesztfeltételek különböznek a valós használattól eltérő mértékben (‡913) (lásd §1.2. Jelenlegi képességek és §3.1. Technikai és intézményi kihívások).

>white|orangered|left|14|15.5|bb A red-teaming lehetővé teszi a kockázat domain-specifikusabb felmérését

A kockázatok felmérésének egy másik gyakori módszere a red teaming. A „red team” egy olyan értékelőcsoport, amelynek feladata sérülékenységek, korlátok vagy a visszaélés lehetőségének keresése. A red teaming lehet szakterület-specifikus, és végezhetik szakterületi szakértők, vagy nyitott jellegű lehet új kockázati tényezők feltárására. Például a red team olyan „jailbreaking” támadásokat fedezhet fel, amelyek kijátsszák a modell biztonsági korlátozásait (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). A benchmarkokkal szemben a red teaming egyik fő előnye, hogy a red team-ek a tesztelt rendszer sajátosságaihoz tudják igazítani az értékeléseiket. Például a red team-ek képesek testreszabott bemeneteket tervezni a legrosszabb viselkedések, a rosszindulatú felhasználási lehetőségek és a váratlan hibák azonosítására. Ugyanakkor külön hozzáférést igényelhet a modellekhez, és előfordulhat, hogy nem tárja fel a fontos kockázati osztályokat (‡999, ‡1028).

Fontos megjegyezni, hogy a beazonosított kockázatok hiánya nem jelenti azt, hogy ezek a kockázatok alacsonyak: korábbi munkák azt mutatják, hogy a hibák gyakran kikerülik a detektálást, különösen akkor, ha a red teamnek korlátozott a hozzáférése vagy az erőforrásai (‡1060). A kutatások emellett megkérdőjelezték, hogy a red-teaming képes-e megbízható és reprodukálható eredményeket előállítani (‡1061). A red team összetétele és a red-teamereknek adott utasítások (‡1062), a támadási körök száma (‡1063), valamint a modell eszközökhöz való hozzáférése (‡1064, ‡1065) jelentősen befolyásolhatja az eredményeket, ideértve azt is, hogy milyen kockázati felületet fednek le. A red-teamingre vonatkozó átfogó iránymutatások célja, hogy kezeljék e kihívások közül néhányat (‡1066).

###@ Kockázatcsökkentés

A kockázatcsökkentés a kockázatok azonosítását követően a kontrollok és ellentevékenységek rangsorolásának, értékelésének és bevezetésének folyamata a feltárt kockázatok csökkentése érdekében. Példák erre a hozzáférés-vezérlések (‡991), a folyamatos monitorozás (‡986), valamint a feltétel-ha kötelezettségvállalások (‡700). A kockázat csökkentése felvet egy kulcskérdést: mi a kockázat elfogadható szintje? A közelmúltban megjelent keretrendszerek és vállalati irányelvek megkezdték a „kockázat elfogadása” kritériumainak formalizálását (‡965, ‡1040). Ugyanakkor a megfelelő küszöbértékek meghatározása továbbra is kihívást jelent, különösen a széles társadalmi hatású kockázatok esetében (‡986, ‡1067). Jelenleg nincs bevett mechanizmus a fejlesztők által a kiadás előtt meghozott kockázatelfogadási döntések érvényesítésére (‡1005).

A 3.3. Táblázatban leírt kockázatcsökkentési módszerek rugalmasan alkalmazhatók, és számos kockázatot képesek mérsékelni, beleértve néhány előre nem látható kockázatot is. A táblázat nem tartalmaz olyan technikai kockázatcsökkentési módszereket, mint az ellenséges betanítás (adversarial training), a tartalomszűrők (content filters) és a chain-of-thought monitorozás. Ezek a §3.3. alatt, illetve a jelentésben az egyes kockázatokhoz tartozó §2. Risks részben található „Mitigations” bekezdésekben vannak lefedve.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Elfogadható használati szabályzatok
  A megfelelő használati irányelvek (acceptable use policy) szabályok és útmutatók összessége a mesterséges intelligencia modellek felelős, etikus és jogszerű használatához. Gyakori, hogy az AI-fejlesztők a modellek új kiadásakor közzéteszik a megfelelő használati irányelveket, valamint a tiltott használati irányelveket is (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hozzáférés-vezérlés / felhasználói ellenőrzés
  A hozzáférés-ellenőrzések magukban foglalják a házirendek és szabályok használatát az AI-modellekhez, adatokhoz és rendszerekhez való hozzáférés korlátozására a felhasználói szerepek, attribútumok és egyéb feltételek alapján, annak érdekében, hogy megakadályozzák a jogosulatlan használatot, manipulációt vagy az adatszivárgásokat. Az AI-vállalatok gyakran letiltják azokat a fiókokat, amelyekről megállapítható, hogy bűncselekményben vesznek részt (‡486), és felhasználói ellenőrzést, valamint Know-Your-Customer (KYC) szűréseket alkalmaznak annak biztosítására, hogy a modelleket csak megbízható szereplők használják (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Viselkedés/működési modell specifikáció
  A mesterséges intelligencia viselkedési specifikációja egy olyan dokumentum, amely meghatározza, hogy egy AI modell hogyan viselkedjen különböző helyzetekben. Ez egy alaprajzként szolgál az AI-illeszkedéshez és -biztonsághoz, iránymutatást ad a modellfejlesztéshez, a betanításhoz, az értékeléshez és a kimenetekhez. Több AI-cég is használ modellspecifikációs dokumentumokat, és legalább ezek egyes részeit nyilvánosságra hozza (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Folyamatos felügyelet
  A folyamatos felügyelet az AI rendszerek üzem közbeni, folyamatos, automatizált megfigyelésének, elemzésének és irányításának folyamata, amely a teljesítményük nyomon követésére és viselkedésük korlátozására szolgál annak biztosítása érdekében, hogy azok megbízhatóak, hatékonyak és biztonságosak legyenek. A folyamatos felügyelethez számos eszköz áll rendelkezésre (‡1073*), valamint olyan technikák, amelyek a támogatást nyújtják
AI megfigyelhetőség (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Védelem-mélyítési elv
  A védelmi szintekre épülő megközelítés (defence-in-depth) lényege, hogy több egymástól független, egymással átfedésben lévő védelmi réteg valósítható meg úgy, hogy ha az egyik megbukik, a többiek továbbra is hatékonyak maradnak (‡1075, ‡1076). Több Frontier AI Safety Framework (pl. (‡1077*)) is hivatkozik erre.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ökoszisztéma-figyelés
  Ez a folyamat a tágabb AI-ökoszisztéma monitorozását foglalja magában, beleértve a számítási és hardverkövetést, a modell eredetiségének nyomon követését, az adatok eredetiségének nyomon követését, valamint a felhasználási mintázatokat. A kutatási szakirodalom az ilyen monitorozást a többcélú AI-ból származó kockázatokkal kapcsolatban tárgyalja (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ha-akkor kötelezettségvállalások
  Az if-akkor kötelezettségvállalások olyan technikai és szervezeti protokollokból és kötelezettségvállalásokból álló készletek, amelyek célja a kockázatok kezelése, ahogy az AI-modellek egyre képessébbé válnak. Több AI-fejlesztő is alkalmazza ezeket a típusú kötelezettségvállalásokat a Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*) keretében.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vörös vonalak vagy tiltások
  A piros vonalak konkrét határértékek, amelyeket képességekként, hatásként vagy a felhasználás típusaként fejeznek ki. A fogalom nyilvános nyilatkozatokban és kezdeményezésekben, valamint szabályozási tilalmakban (‡1079, ‡1080, ‡1081) is megjelenik. Az irodalom továbbá megjegyzi a piros-vonalas megközelítések korlátait, beleértve a konszenzusteremtés és az érvényesíthetőség körüli nehézségeket.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kiadási és telepítési stratégiák
  Az általános célú mesterséges intelligencia esetén a kiadási és telepítési stratégiák magukban foglalhatják a fokozatos kiadásokat vagy az API-hozzáférést, hogy visszaélés vagy váratlan károkozás esetén több mérséklési lehetőség álljon rendelkezésre (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.3. Táblázat: Kockázatcsökkentés általános célú mesterséges intelligencia kockázatkezelésben
>white|black||9|11|br Az AI-kockázatcsökkentés példamódszerei betűrendben vannak felsorolva. A beépített módszerek többféle kockázattípus egyidejű kockázatcsökkentését hivatottak támogatni, beleértve a rosszindulatú felhasználásból eredő kockázatokat, a meghibásodásból eredő kockázatokat és a rendszerszintű kockázatokat. Mivel az általános célú AI kockázatkezelés még kialakulóban van, nem minden módszer lesz alkalmas minden AI-fejlesztő vagy üzemeltető számára.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Ábra 3.5: Egy „svájci sajtdiagram”, amely a védelmi mélység (defence-in-depth) megközelítést szemlélteti
>white|black||9|11|br Több védelmi réteg képes ellensúlyozni az egyes rétegek hiányosságait. Az AI-val kapcsolatos jelenlegi kockázatkezelési technikák hibákkal rendelkeznek, de ezek rétegezése sokkal erősebb védelmet nyújthat a kockázatok ellen. Forrás: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb A védelem-szintű kialakítás és a kiadási (release) stratégiák fontos mérséklési eszközök.

A ‘többrétegű védelem’ (defence-in-depth) modell általános célú mesterséges intelligencia kockázatkezelését is támogatni tudja. Ebben az összefüggésben a ‘többrétegű védelem’ a fejlesztés és a telepítés különböző szakaszaiban alkalmazott technikai, szervezeti és társadalmi intézkedések kombinációját jelenti (3.5. Ábra). Ez független biztosítékok rétegeinek létrehozását jelenti, hogy ha az egyik réteg meghibásodik, a többi réteg még mindig meg tudja előzni a károkozást. A többrétegű védelem modelljére gyakran idézett példa a fertőző betegségek megelőzésére bevetett megelőző intézkedések skálája. Oltások, maszkok és kézmosás, többek között, kombinációban jelentősen csökkenthetik a fertőzés kockázatát, még akkor is, ha ezek közül egyik módszer sem 100%-osan hatékony önmagában (‡1083*). Általános célú mesterséges intelligencia esetén a többrétegű védelem olyan kontrollokat is magában foglal, amelyek nem magán a mesterséges intelligencia modelljén vannak, hanem a tágabb ökoszisztémán. Ez magában foglalja (például) a biológiai támadás végrehajtásához szükséges anyagokra vonatkozó kontrollokat, például reagensanyagokra vonatkozó intézkedéseket (‡1084, ‡1085). Ugyanakkor a többrétegű védelem intézkedései elsődlegesen a balesetekhez, a meghibásodáshoz és a rosszindulatú felhasználáshoz kapcsolódó kockázatokat kezelik, és a rendszerszintű kockázatok kezelésében kisebb szerepet játszhatnak (lásd §3.5. Társadalmi reziliencia kialakítása).

Egy vállalat kiadási és telepítési stratégiája a kockázatcsökkentés fontos eleme. Azok a döntések, hogy a modellek hogyan válnak elérhetővé a felhasználók számára, jelentősen befolyásolhatják a kockázati kitettséget (‡1082). Különböző kiadási és telepítési lehetőségek közé tartozik a fokozatos kiadás korlátozott felhasználói csoportok számára, a hozzáférés felügyelt online szolgáltatásokon keresztül (például API-kon) keresztül, valamint a licencmegállapodások és elfogadható felhasználási irányelvek alkalmazása, amelyek jogilag tiltják bizonyos káros alkalmazások használatát (‡176, ‡1086, ‡1087). §3.4. A nyílt súlyú modellek részletesebben tárgyalja, hogy a modell súlyainak kiadása hogyan befolyásolja a kockázatokat.

###@ Kockázatirányítás

A kockázatirányítás az a folyamat, amelynek során a kockázatkezelési értékelések, döntések és intézkedések összekapcsolódnak egy szervezet vagy más entitás stratégiájával és célkitűzéseivel (‡1088, ‡1089). A 3.4. táblázat áttekintést nyújt a gyakori kockázatirányítási technikákról. Amint azt a 3.4. ábra mutatja, a kockázatirányítás a kockázatkezelés magjaként értelmezhető, mivel elősegíti a kockázatkezelés más elemeinek hatékony működését. Olyan felelősséget, átláthatóságot és egyértelműséget biztosít, amelyek megalapozott kockázatkezelési döntéseket támogatnak. A kockázatirányítás magában foglalhat olyan gyakorlatokat, mint az incidensjelentés (‡1090), a kockázati felelősségek kiosztása (‡965) és a bejelentővédelmi intézkedések (‡1091). Tágabb értelemben a kockázatirányítás magában foglalhat útmutatásokat, keretrendszereket, jogszabályokat, szabályozásokat, nemzeti és nemzetközi szabványokat, valamint képzési és oktatási kezdeményezéseket is. A kockázatirányítás egyik legfontosabb célja olyan szervezeti politikák és mechanizmusok kialakítása, amelyek tisztázzák, hogy a kockázatkezelési felelősségek hogyan kerülnek kiosztásra egy szervezeten vagy más entitáson belül, annak érdekében, hogy megfelelő felügyelet és elszámoltathatóság biztosítható legyen (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentáció
  A dokumentációs gyakorlatok segítenek nyomon követni a kulcsfontosságú információkat az AI rendszerekről, például a betanítási adatok, a tervezési döntések, a tervezett felhasználások, a korlátok és a kockázatok tekintetében. A ‘modellkártyák’ és ‘rendszerkártyák’, amelyek tájékoztatást nyújtanak arról, hogyan lettek egy AI modell vagy rendszer betanítva és kiértékelve, a kiemelkedő AI-dokumentációs legjobb gyakorlatok példái (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Eseményjelentés
  Az incidensjelentéskészítés az a folyamat, amelynek során az MI fejlesztése vagy bevezetése során bekövetkező, közvetlen vagy közvetett kárt okozó eseteket szisztematikusan dokumentálják és megosztják. Számos olyan platform létezik, amely támogatja az MI-vel kapcsolatos incidensjelentést (‡1096, ‡1097), továbbá vannak olyan keretrendszerek is, amelyek hatékonyabb MI-incidensjelentést segítenek elő (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb kockázatkezelési keretrendszerek
  A kockázatkezelési keretrendszerek szervezeti szintű tervek a kockázatfedezetben meglévő hiányosságok csökkentésére, a különböző kockázatkezelési tevékenységek összehangolására, valamint az ellenőrzési és ellensúlyozási mechanizmusok bevezetésére. Az általános célú mesterséges intelligenciára (‡986, ‡1098) vonatkozó keretrendszerek gyakran hivatkoznak az ebben a szakaszban említett egyéb intézkedésekre.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázati nyilvántartás
  A kockázatnyilvántartó különféle kockázatokat, azok priorizálását, felelőseit és mérséklési terveit tartalmazó adattár. Ezek viszonylag gyakoriak sok iparágban, többek között a kiberbiztonságban (‡1099), és néha a szabályozási megfelelőségi követelmények teljesítésére is használják őket.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kockázatfelelősség megosztása
  A szervezeten belüli kockázatkezelésre vonatkozó szerepkörök és felelősségek kijelölése képes strukturálni a döntéshozatal belső felügyeletét (‡1002, ‡1093). Az ilyen megoldások bizonyos irányítási keretrendszerekben is megjelennek, ideértve az EU általános célú MI gyakorlatra vonatkozó kódexét (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Átláthatósági jelentések
  A transzparenciajelentések az AI-vállalat kockázatkezelési gyakorlatainak leírását azáltal végzik, hogy bizonyos információkat nyilvánosan közzétesznek, vagy dokumentációt osztanak meg iparági csoportokkal vagy kormányzati szervekkel. Például számos AI-vállalat nyújt be Hirosima AI-folyamatot (HAIP) bemutató transzparenciajelentéseket (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bejelentővédelmi intézkedések
  Mivel a mesterséges intelligencia fejlesztésének nagy része zárt ajtók mögött történik, egyes irányítási keretrendszerek bejelentővédelmet is tartalmaznak, hogy lehetővé tegyék a lehetséges kockázatok hatóságok felé történő bejelentését (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.4. Táblázat: Kockázatirányítás az általános célú mesterséges intelligencia kockázatkezelésében
>white|black||9|11|br Példák az AI kockázatkezelési kockázatirányításra vonatkozó módszerekre, betűrendben felsorolva. A módszerek között szereplő megoldások úgy vannak kialakítva, hogy egyszerre támogassák a kockázatirányítást sokféle kockázattípus esetén, ideértve a rosszindulatú felhasználásból eredő kockázatokat, a meghibásodásokból eredő kockázatokat és a rendszerszintű kockázatokat. Mivel az általános célú AI kockázatkezelés még kialakulóban van, nem minden módszer lesz alkalmas minden AI fejlesztő vagy üzemeltető számára.


>white|orangered|left|14|15.5|bb A dokumentáció és az átláthatóság a kockázatkezelés kockázatirányítási elemei

A dokumentációs és intézményi átláthatósági mechanizmusok, valamint az információmegosztási gyakorlatok elősegítik a külső ellenőrzést, és támogatják az általános célú mesterséges intelligenciával (‡1101, ‡1102) kapcsolatos kockázatok kezelésére irányuló erőfeszítéseket. Közismert gyakorlattá vált, hogy az üzembe helyezés előtti tesztek eredményeit egy „model card” vagy „system card” formájában publikálják, valamint a modellről vagy rendszerről szóló alapvető részleteket is, beleértve azt, hogy hogyan képezték ki, illetve mik a lehetséges korlátai (‡1094, ‡1095). Egyes fejlesztők emellett közzétesznek átláthatósági jelentéseket is, amelyek szélesebb körben tartalmazzák a kockázatkezelési gyakorlatuk részleteit (‡1103). A dokumentáció és az átláthatóság további elemei közé tartozik a monitorozás és az incidensjelentés (‡176, ‡1083*, ‡1103), valamint az információmegosztás, amelyet olyan harmadik felek is elősegíthetnek, mint a Frontier Model Forum. Néhány szabályozási keretrendszer, például az EU AI Act vagy Kalifornia „Transparency in Frontier Artificial Intelligence Act” - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), egyes esetekben előírja az általános célú mesterséges intelligencia kockázataival kapcsolatos információmegosztást.

>white|orangered|left|14|15.5|bb A vezetői elkötelezettség és az ösztönzők alakítják a kockázatkezelési gyakorlatokat

A szervezeti kultúra, a vezetési struktúra és az ösztönzők különböző módokon befolyásolják a kockázatkezelési erőfeszítéseket (‡1105). A vezetői elköteleződés és az ösztönzőrendszerek gyakran relevánsak abban, hogy a kockázatkezelési politikák a gyakorlatban hogyan működnek. Néhány fejlesztő belső döntéshozatali testületeket működtet, amelyek megvitatják, hogyan lehet biztonságosan és felelősen megtervezni, kifejleszteni és felülvizsgálni az új AI-rendszereket. Az ellenőrző és tanácsadó bizottságok, a trustök, vagy az AI-etikával foglalkozó testületek szintén szolgálhatnak a kockázatkezelési iránymutatás és a szervezeti felügyelet mechanizmusaként (‡1092*, ‡1106, ‡1107, ‡1108). A kutatók azt érvelték, hogy az önkéntes önszabályozással kapcsolatos kihívások miatt a harmadik fél általi auditálás, verifikáció és standardizáció hozzájárulhat az általános célú AI kockázatkezelés megerősítéséhez (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Szervezeti kockázatkezelés, átláthatóság, valamint kockázatjelentési keretrendszerek

Több új kezdeményezés a kockázatkezelési folyamatokra, a dokumentációra és az átláthatóságra összpontosít. Jelenlegi formájában az EU általános célú AI Magatartási Kódexe (General-Purpose AI Code of Practice) önkéntes keretrendszerként működik, amely az átláthatósági, szerzői jogi, valamint biztonsági és kockázatcsökkentési (safety and security) gyakorlatok irányítását szolgálja, annak érdekében, hogy támogatást nyújtson az EU AI Act (‡965) általános célú mesterséges intelligenciára (general-purpose AI) vonatkozó rendelkezéseinek való megfeleléshez. 2025 decemberétől több mint két tucat vállalat† írta alá. A G7 Hiroshima AI Process (HAIP) jelentéstételi keretrendszere (‡1100) az első nemzetközi keretrendszer az előrehaladott AI-rendszerek szervezeti kockázatkezelési gyakorlatainak önkéntes, nyilvános jelentéstételére. Legalább 20 fejlesztő tett közzé nyilvános átláthatósági jelentéseket, amelyek a kockázatfelismerést, az értékelési metrikákat, a kockázatcsökkentési stratégiákat, valamint az adatbiztonsági folyamatokat fedik le.

Az AI fejlesztők önkéntes átláthatósági vállalásokat fogadtak el. Kínában a China AI Industry Alliance által koordinált, 17 kínai AI-vállalat által tett vállalásokat 2024 decemberében (‡1113), 2025-ben pedig frissítették (‡1114). A 2024 májusában, Dél-Koreában megrendezett AI Seoul Summit alkalmával 16, több országból származó AI fejlesztő önkéntes kötelezettségvállalásokat írt alá annak érdekében, hogy közzétegyék az általuk legmagasabb képességű modelljeikhez és rendszereikhez kapcsolódó Frontier AI Safety Frameworks-eket, valamint hogy a kockázatkezelési gyakorlatokat a modellfejlesztés és a telepítés szakaszain keresztül alkalmazzák (‡1052).

    Megjegyzés † -- Az aláírók 2025 decemberében a következők: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, and WRITER.

>white|orangered|left|14|15.5|bb A Frontier AI Safety keretrendszerek jelentős szervezeti megközelítéssé váltak a mesterséges intelligencia kockázatkezelés terén

2023 óta több, élvonalbeli AI-fejlesztő önként közzétett olyan dokumentumokat, amelyek leírják, hogyan kívánják azonosítani és kezelni a legfejlettebb rendszereikből származó súlyos kockázatokat. Ezek a Frontiereken alkalmazott AI-biztonsági keretrendszerek azt írják le, hogy az AI-fejlesztő hogyan tervezi értékelni, monitorozni és irányítani a legfejlettebb AI-modelljeit és rendszereit még a bevezetés előtt, illetve a bevezetés során. Ezek a keretrendszerek sok hasonlóságot mutatnak, de fontos szempontokban eltérnek egymástól (‡1115, ‡1116). A legtöbb a vegyi, biológiai, radiológiai és nukleáris (CBRN) fenyegetésekhez kapcsolódó kockázatokra, a fejlett kibertámadási képességekre, valamint a fejlett autonóm viselkedésre összpontosít (‡1115, ‡1117). A keretrendszerek kisebb része olyan további kockázati területekkel is foglalkozik, mint a nagymértékű jogellenes megkülönböztetés és a gyermekek szexuális kizsákmányolása.

Több fejlesztő 2025-ben frissítette a keretrendszereit, és új szakaszokat adott hozzá a káros manipulációról, a félreigazítási kockázatról, valamint az autonóm replikációról és adaptációról (‡1078, ‡1118). Bár sok keretrendszer hasonló kockázatkezelési megközelítéseket ír le – ideértve a fenyegetésmodellezést, a red-teaminget és a veszélyes képességek értékelését – eltérnek a kockázati szintek és küszöbértékek meghatározásában, az értékelések gyakoriságában, az értékelések és a küszöbértékek közötti puffer időkben, valamint a mérséklési vállalásaik átfogóságában (például hogy tartalmazzák-e a modell súlyainak törlését, vagy csak a fejlesztés leállítását) (‡1115, ‡1119). További információkért lásd a 3.5. Táblázatot.

>white|orangered|left|14|15.5|bb A Frontier AI Safety keretrendszerekben sok művelet azon múlik, hogy vannak-e feltételes (if-then) vállalások

A Frontier AI Safety Frameworks kulcsfontosságú elemei az „ha-akkor” kötelezettségvállalások. Ezek feltételes protokollok, amelyek egyedi válaszokat váltanak ki, amikor az AI-modellek és -rendszerek előre meghatározott képességi küszöbértékeket (‡1120) elérnek. Például egy ha-akkor kötelezettségvállalás kimondhatja, hogy ha egy modellt úgy találnak, hogy képes érdemben segíteni a kezdőket a CBRN fegyverek létrehozásában és bevetésében, akkor a fejlesztő fokozott biztonsági intézkedéseket, telepítési vezérléseket és valós idejű megfigyelést valósít meg (‡991*).

2025-ben több AI-fejlesztő bejelentette, hogy az új modellek korai figyelmeztető riasztásokat váltottak ki, vagy hogy nem tudták kizárni annak lehetőségét, hogy a további értékelés azt mutatja: a modellek átlépték a képességi küszöböket. Ez arra késztette őket, hogy óvintézkedésként fokozott biztosítékokat alkalmazzanak (‡7, ‡33, ‡1121*). A Frontier AI Safety Frameworks (Frontier AI biztonsági keretrendszerek) jellemzően a kockázatcsökkentés előtt egy kezdeti képességértékelést, valamint a kockázatcsökkentést követően egy fennmaradó kockázatelemzést vagy biztonsági esetet (safety case), gyakran red-teaming (vörös csapatos tesztelés) alapján megközelítve írnak elő. A részletes információkért lásd a Táblázat 3.5-öt.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Felkészültségi keretrendszer 2 (‡1078*)
  Fedezett kockázatok:
1. Biológiai és kémiai képességek
2. Kiberbiztonsági képességek
3. AI önfejlesztési képességek
  Kockázati szintek vagy ezekkel egyenértékű kategóriák, valamint a kapcsolódó biztosítékok:
- Magas: Felerősítheti a meglévő útvonalakat a súlyos károkhoz (Biztonsági vezérlőkre és biztosítékokra van szükség)
- Kritikus: Olyan példátlan új utakat nyithat meg a súlyos károkhoz (A további fejlesztés felfüggesztése, amíg a meghatározott biztosítékok és a biztonsági vezérlők követelményei el nem érik a Kritikus szintet)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Felelős skálázási irányelv 2.2 (‡991*)
  Fedezett kockázatok:
1. CBRN fegyverek
2. Autonóm mesterséges intelligencia kutatás és fejlesztés (AI R&D)
3. Kiberoperációk (értékelés alatt)
  Kockázati szintek vagy azzal egyenértékű kategóriák, valamint a kapcsolódó biztosítékok:
  AI-biztonsági szintek (ASL)
- ASL-1: Nincs jelentős katasztrofális kockázat
- ASL-2: A veszélyes képességek korai jelei (A modelleknek meg kell felelniük az ASL-2 telepítési és biztonsági követelményeinek)
- ASL-3: Jelentősen megnövekedett katasztrofális visszaélési kockázat (A modelleknek meg kell felelniük az ASL-3 üzembe helyezési és/vagy biztonsági szabványoknak)
- ASL-4+: Jövőbeli osztályozások (még nem meghatározott)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Fedezett kockázatok:
1. Visszaélés
    a. CBRN
    b. Kiber
    c. Káros manipuláció
2. Gépi tanulás K+F
3. Rossz illeszkedés/ instrumentális érvelés
  Kockázati szintek vagy azokkal egyenértékű besorolások és a kapcsolódó védintézkedések:
  Kritikus képességszintek
    Képességszintek, amelyeknél – közbeavatkozási intézkedések hiányában (telepítésekre vonatkozó biztonsági esetek, valamint a RAND biztonsági szintek 2, 3 vagy 4 (‡1122) szerinti biztonsági mérséklések) – a mesterséges intelligencia modellek vagy rendszerek fokozott kockázatot jelenthetnek a súlyos károkozás tekintetében. A képességszintek magukban foglalják a „korai figyelmeztetési értékeléseket” is, meghatározott „riasztási küszöbértékekkel”
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Fedezett kockázatok:
1. Kiberbiztonság
2. Kémiai és biológiai kockázatok
  Kockázati szintek vagy azzal egyenértékű kategóriák, valamint a kapcsolódó biztosítékok:
  Kockázati küszöbszintek
- Közepes (kiadás megfelelő biztonsági intézkedésekkel és kockázatcsökkentésekkel)
- igh (ne engedd el)
- Kritikus (fejlesztés leállítása)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier Model Safety Framework (‡1123*)
  Fedezett kockázatok:
1. CBRN fegyverek elterjedése
2. Offenzív kiber-műveletek
3. Automatizált AI-K+F
  Kockázati szintek vagy azzal egyenértékű kategóriák és az azokhoz kapcsolódó biztosítékok:
  Kritikus képességküszöbök
    A modellek olyan képességei, amelyek a nyilvánosságra jelentős kárt okozhatnak, ha nem megfelelően használják őket. (Ha a küszöbértékek teljesülnek vagy meghaladják azokat, a modellt nem helyezik nyilvánosan üzembe megfelelő kockázatcsökkentő intézkedések nélkül)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier Governance keretrendszer (‡1124*)
  Fedezett kockázatok:
1. CBRN fegyverek
2. Offenzív kiber-műveletek
3. Fejlett autonómia (beleértve a AI-kutatást és fejlesztést)
  Kockázati szintek vagy azokkal egyenértékű kategóriák és a kapcsolódó biztosítékok:
  Kockázati szintek
- Alacsony vagy Közepes (Telepítés engedélyezett a Responsible AI Program követelményeivel összhangban)
- Magas vagy Kritikus (További felülvizsgálat és intézkedések)
(szükséges)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier AI kockázatértékelés (‡1029*)
  Fedezett kockázatok:
1. Kiberbűncselekmény
2. CBRN
3. Meggyőzés és manipuláció
4. Jogellenes megkülönböztetés mértékben történő alkalmazásban
  Kockázati szintek vagy azzal egyenértékű kategóriák és a hozzájuk kapcsolódó biztosítékok:
  Kockázati küszöbértékek – modelkockázat (MR) pontszámok
- MR1 vagy MR2 (Az értékelési eredményeket a mérnöki csapatok dokumentálják)
- MR3 (A kockázatcsökkentési intézkedéseket és az értékelési eredményeket a mérnöki csapatok dokumentálják, és rendszeresen felülvizsgálják)
- MR4 (Részletes kockázatértékelést kell elvégezni, és az üzletági vezető jóváhagyása szükséges)
- MR5 (Részletes kockázatértékelést kell elvégezni, és azt független bizottságnak kell jóváhagynia, pl. a NVIDIA AI etikai bizottságának)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Biztonságos AI Frontmodell Keretrendszer (‡1125*)
  Fedezett kockázatok:
1. Rosszindulatú felhasználás (pl. rosszindulatú szoftver, gyermekek szexuális kizsákmányolása)
2. Kár ártalmatlan, hétköznapi használat során, pl. olyan kimenetek, amelyek illegális, megkülönböztető jellegű eredményt hoznak létre, vagy nem biztonságos kód generálását eredményezik
  Kockázati szintek vagy ezekkel egyenértékű kategóriák, valamint a kapcsolódó védintézkedések:
  A károkozás valószínűsége és súlyossága kontextusban
- Alacsony
- Közepes
- Magas
- Nagyon magas
    (Kockázatcsökkentő intézkedések és biztonsági kontrollok minden rendszerhez és folyamathoz rendelkezésre állnak; további kockázatcsökkentő intézkedéseket kell az AI-rendszerhez és ahhoz az felhasználási esetre kell igazítani, amelyben egy modellt telepítenek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI Készenléti Irányelv (‡1127*)
  Fedezett kockázatok:
1. Kiberbűncselekmény
2. Automatizált AI-K+F
3. Önálló replikáció és adaptáció
4. Biológiai fegyverekhez nyújtott segítségnyújtás
  Kockázati szintek vagy ezzel egyenértékű besorolás és a kapcsolódó biztosítékok:
  Kritikus képességküszöbök
    Kvantitatív küszöbértékek a képesség-benchmarkokon (Ha átlépik, végezzen veszélyes képességértékeléseket, információbiztonsági intézkedéseket és telepítési enyhítéseket, vagy függessze fel a fejlesztést)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI Felkészültségi politika (‡1127*)
  Fedezett kockázatok:
1. Kiberbűncselekmény
2. Automatizált AI-K+F
3. Önálló replikáció és adaptáció
4. Biológiai fegyverekhez nyújtott segítségnyújtás
  Kockázati szintek vagy ezekkel egyenértékű kategóriák és a kapcsolódó biztosítékok:
  Kritikus képességküszöbök
    Kvantitatív küszöbértékek a képesség-értékelő mérőszámokon (Ha átlépésre kerülnek, végezzen veszélyes képességértékeléseket, információbiztonsági intézkedéseket és telepítési enyhítéseket, vagy állítsa le a fejlesztést)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: AI-biztonsági keretrendszer (‡1128*)
  Fedezett kockázatok:
1. Vezérlés elvesztése
2. Visszaélés (pl. biokémiai fegyverré alakítás
  Kockázati szintek vagy azokkal egyenértékű besorolás, valamint a kapcsolódó biztosítékok:
  Kockázati szintek
- Alacsony kockázat (AI-rendszerek telepítése, de a kockázatok kezelése érdekében utólag felügyeletet kell végezni)
- Azonosított kockázat (Csak engedélyezett felhasználóknak nyitni meg az OpenAI-rendszereket a kockázatok mérséklése érdekében, vagy az alkalmazás telepítésének visszatartása, amíg további biztonsági intézkedések nem kerülnek bevezetésre, az adott használati esettől függően)
- Magas kockázat (Ne telepítsen mesterséges intelligencia rendszereket)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI Safety Framework (‡1129*)
  Fedezett kockázatok:
1. Biológiai fenyegetések
2. Offenzív kiberbiztonság
3. Önálló működés és fejlett manipuláció
  Kockázati szintek vagy azokkal egyenértékű kategóriák, valamint a kapcsolódó biztosítékok:
  Kockázati szintek
- 1. szint (Alapvető biztosítékok minimális kockázatok esetén, valamint a nyílt forráskódú kiadás lehetősége)
- 2. szint (valós idejű felügyelet, prompt-szűrés, viselkedési anomáliaészlelés, hozzáférés-vezérlés, red-teaming, és adverszárius szimulációk)
- 3. szint (Fejlett biztosítékok, beleértve a red- teaminget, a fokozatos bevezetési szakaszokat, az adversarial tesztelést, a titkosítást, a több fél általi hozzáférés-ellenőrzést és a zero-trust architektúrát)
- 4. szint (maximális biztonsági protokollok a nagy kockázatú modellekhez és maximális biztonsági intézkedések)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 3.5. táblázat: Frontier AI biztonsági keretrendszerek
>white|black||9|11|br A Frontier AI Safety Frameworks első készlete, amelyet a Frontier AI Safety Commitmentsben aláíró AI-fejlesztők egy részhalmaza adott ki. A keretrendszerek hasonló kockázatokat fednek le (enyhe eltérésekkel), és eltérő kockázati szinteket, illetve kockázatkezelési megközelítéseket alkalmaznak.


>white|orangered|left|14|15.5|bb A Frontier AI Safety Framework-ek hatékonysága bizonytalan

A Frontier AI Safety Frameworks kifejezetten bizonyos feltételek mellett és bizonyos kockázati kategóriák esetén kockázatkezelési eszközként szolgálhat, amelyeknek a károkozáshoz vezető hiteles útvonala van (‡1117). Ugyanakkor több elemzés olyan kérdéseket tárgyal, amelyek a keretrendszerek világosságára és hatókörére vonatkoznak (‡111, ‡986), valamint az AI-képességek robusztusságára és a kockázati küszöbértékekre (‡1031, ‡1130) vonatkozó kérdéseket. A meglévő keretrendszerek jellemzően a kockázati domének egy részhalmazára összpontosítanak. Ennek következtében egyes kiemelkedő kockázatok, például a jogellenes megfigyelés (‡1131, ‡1132) és az beleegyezés nélküli intim képek (‡287), kevesebb hangsúlyt kapnak. Más ágazatok, például a repülés vagy a nukleáris energia (‡1133*) kockázatkezelési megközelítéseivel ellentétben a Frontier AI Safety Frameworks általában nem használ explicit kvantitatív kockázati küszöbértékeket (‡1134).

A fejlesztőknek a Frontier AI Safety Frameworks-hez való megfelelésére vonatkozó külső értékelések eddig korlátozottak maradtak, részben azért, mert a legtöbb keretrendszer új keletű, a nyilvánosan elérhető információk ritkák, és nincsenek egységesített külső auditok. Hatékonyságukat az is befolyásolja majd, hogy a kötelezettségvállalások mennyire jól – és milyen mértékben – valósulnak meg a gyakorlatban. Önmagukban ezek a keretrendszerek nem feltétlenül biztosítanak hatékony kockázatkezelést, mivel a gyakorlati hatás attól függ, hogy mennyire jól és milyen mértékben kerülnek bevezetésre. Eddig nem teljes mértékben igazodnak a nemzetközi kockázatkezelési standardokhoz (‡1135). Egy tanulmány a korábbi önkéntes kötelezettségvállalásokról azt találta, hogy a különböző intézkedések teljesítése egyenetlen volt, ami arra utal, hogy az önkéntes kötelezettségvállalások betartása várhatóan vállalatonként és szakterületenként eltérő lesz (‡1109).

Együttesen a Frontier AI Safety Frameworks jelentik a jelenleg alkalmazott, legátfogóbb önkéntes szervezeti kockázatkezelési formát, ugyanakkor jelentős mértékben eltérnek a hatókör, küszöbértékek és kikényszeríthetőség tekintetében.

###@ Szabályozási és irányítási kezdeményezések

>white|orangered|left|14|15.5|bb Több joghatóság is olyan törvényeket vezetett be, amelyek átláthatósági követelményeket írnak elő

Több korai szabályozási megközelítés olyan jogi követelményeket vezet be, amelyek a kockázatkezelés terén a szabványosítás és az átláthatóság növelését célozzák. Az EU AI Act, amely 2024-ben lépett hatályba, a transzparenciával, a szerzői joggal és az általános célú mesterséges intelligencia modellek biztonságával kapcsolatos követelményeket határoz meg. 2025-ben közzétették az EU Általános Célú MI Kódexét a gyakorlatban, amely e kötelezettségeknek való megfelelést hivatott támogatni azáltal, hogy útmutatást ad a modell-dokumentációra és a szerzői jogra vonatkozóan, valamint – a legfejlettebb modellek esetében – olyan kockázatkezelési gyakorlatokra, mint az értékelések, a kockázatértékelés és -csökkentés, az információbiztonság és a súlyos incidensekről szóló jelentéstétel (‡965).

A további új szabályozási követelmények közé tartozik Dél-Korea Keret törvénye a mesterséges intelligencia fejlesztéséről és a bizalom megteremtéséről, amely a kritikus ágazatokban használt „magas hatású” AI rendszerekre (‡1136) vonatkozó követelményeket vezet be, valamint Kalifornia SB 53 törvénye, amely átláthatósági követelményeket határoz meg a biztonsági keretrendszerekre és az incidensjelentésekre vonatkozóan (‡1104). Mivel e követelmények bevezetése viszonylag friss, még túl korai a részletes értékelés ahhoz, hogy milyen módon fognak hatni a kockázatkezelési gyakorlatokra, illetve az elért tényleges kockázati eredményekre.

>white|orangered|left|14|15.5|bb A szélesebb körű kormányzási kezdeményezések önkéntes iránymutatást nyújtanak

Több regionális és régiók közötti kormányzási keretrendszer ma közös elvárásokat fogalmaz meg az általános célú mesterséges intelligenciából eredő kockázatok kezelésére, nem kötelező érvényű iránymutatásokat adva a döntéshozók és a szervezetek számára. A Kínai AI-biztonsági Kormányzási Keretrendszer 2.0, amely 2025-ben jelent meg, strukturált útmutatást nyújt a kockázatok kategorizálására és az ellenintézkedésekre az AI fejlesztési és telepítési folyamata során (‡1137). Az ASEAN-tagállamok közzétették az „ASEAN kibővített útmutatója a mesterséges intelligencia kormányzásához és etikájához (generatív AI)”-t, amely iránymutatást ad az általános célú mesterséges intelligencia kormányzására és etikájára, és célja, hogy elősegítse a nagyobb szakpolitikai összhangot az ASEAN-tagállamok között (‡1138). Emellett szakértők által vezetett kezdeményezések, például a Szingapúri Konszenzus, amelyet több országból származó AI-tudósok dolgoztak ki, kutatási prioritásokat határoznak meg az általános célú AI-biztonság területén a kockázatértékelés, a fejlesztés és a vezérlés során (‡690).

###@ Frissítések

A legutóbbi Jelentés (2025 január) közzététele óta a cél-/általános célú mesterséges intelligencia kockázatkezelési területén változások történtek: új források jelentek meg, például az EU Általános célú mesterséges intelligenciáról szóló magatartási kódexe, a G7 HAIP jelentéstételi keretrendszere, Kína nemzeti AI-biztonsági irányítási keretrendszere 2.0, valamint különféle AI-fejlesztők Frontier AI Safety Frameworks-ei. Ezek a kezdeményezések bemutatják azokat a megközelítéseket és gyakorlatokat, amelyeket az AI-fejlesztők az általános célú mesterséges intelligencia rendszerekkel (‡1115) kapcsolatos kockázatok kezelésére alkalmaznak. Jelentős eltérések tapasztalhatók a Frontier AI Safety Frameworks-ek között, valamint a HAIP átláthatósági jelentésekben (‡1103) is, ami a szervezeti gyakorlatok, a kockázatok rangsorolása és a kockázatkezelési ökoszisztéma korai szakasza közötti különbségeket tükrözi. Egy olyan megbízható ökoszisztéma, ahol különböző AI-szereplők a teljes életcikluson át kiegészítő kockázatkezelési gyakorlatokkal járulnak hozzá, hozzájárulhat a hatékony kockázatkezeléshez (‡690).

###@ Bizonyítéki hiányosságok

Hiányzik az evidencia arra vonatkozóan, hogy miként mérhető az egyre jelentkező kockázatok súlyossága, gyakorisága és időbeli lefutása; mennyiben mérsékelhetők ezek a kockázatok a valós környezetekben; valamint hogy hogyan lehet hatékonyan ösztönözni vagy kikényszeríteni a mérséklési intézkedések bevezetését a különböző szereplők körében. További kutatásokra van szükség annak megértéséhez, hogy a különböző kockázatok mennyire elterjedtek, és mennyire térnek el a világ különböző régióiban, különösen olyan régiókban, mint Ázsia, Afrika és Latin-Amerika, amelyek gyors ütemben digitalizálódnak. Mivel az AI modellek egyre nagyobb önállóságot és felhatalmazást kapnak, és a sokcélú (general-purpose) AI kockázatok tudományos ismeretállapota tovább fejlődik, a kockázatkezelési megközelítéseknek is fejlődniük kell (‡639, ‡1139).

Bizonyos kockázatcsökkentési intézkedések egyre népszerűbbek (‡690, ‡956), de további kutatásokra van szükség annak megértéséhez, hogy a kockázatcsökkentési intézkedések és biztosítékok a gyakorlatban mennyire robusztusak különböző közösségek és AI-aktorok esetében (ideértve a kis- és középvállalkozásokat is). Az ilyen értékelések szempontjából releváns az, hogy mennyiben hozzáférhetők olyan adatok, amelyek a modellek életszerű telepítését és használatát tükrözik. Továbbá a kockázatkezelési erőfeszítések jelenleg erősen eltérnek a vezető AI-vállalatok között. Azt állították, hogy a fejlesztők ösztönzői nincsenek jól összehangolva az alapos kockázatértékeléssel és kockázatkezeléssel (‡934). Még mindig bizonyítékhiány van arra vonatkozóan, hogy különböző önkéntes vállalások mennyiben teljesülnek, milyen akadályokkal szembesülnek a vállalatok a vállalások teljes körű betartása során, illetve hogyan építik be a Frontier AI Safety Frameworks (Frontier AI Safety keretrendszerek) az átfogó AI-kockázatkezelési gyakorlatokba.

###@ Kihívások a döntéshozók számára

A legfontosabb kihívások közé tartozik annak meghatározása, hogyan lehet priorizálni az általános célú AI által jelentett sokféle kockázatot, annak tisztázása, hogy mely szereplők vannak a legjobb helyzetben ezek mérséklésére, valamint annak megértése, hogy milyen ösztönzők és korlátok alakítják a cselekedeteiket. A bizonyítékok arra utalnak, hogy a döntéshozók jelenleg korlátozottan férnek hozzá olyan információkhoz, amelyekből kiderülne, hogy az AI fejlesztői és bevezetői hogyan tesztelik, értékelik és monitorozzák az újonnan felmerülő kockázatokat, illetve hogy a különböző mérséklési gyakorlatok mennyire hatékonyak (‡1140). Kutatók és döntéshozók megvitatták a transzparencia irányába tett erőfeszítéseket és a részletesebb, rendszerezettebb incidensjelentést mint lehetséges módokat a kockázatpriorizálás megalapozására, a bizalom előmozdítására és a felelős fejlesztést ösztönző tényezők megteremtésére (‡957). A gyakorlatban a kockázatkezelés több szereplőt érint az AI értékláncán belül – például az adatszolgáltatókat és a felhőszolgáltatókat, a modellt fejlesztőket, valamint a modellhoszting platformokat –, amelyek mindegyike különböző lehetőségekkel rendelkezik a különféle kockázatok felmérésére és kezelésére (‡1141). E szereplők közötti korlátozott információmegosztás megnehezíti annak meghatározását, hogy mely kockázatok a legvalószínűbbek vagy amelyek a legnagyobb hatással bírnak, különösen akkor, amikor az alsóbb szinteken jelentkező társadalmi következmények is figyelembevételre kerülnek.

