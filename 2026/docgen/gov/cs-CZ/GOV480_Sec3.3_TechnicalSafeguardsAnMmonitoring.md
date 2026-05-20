##########
>white|orangered|left|14|30|hr Sekce 3.3
### 3.3. Technická ochranná opatření a monitorování
>white|orangered|left|24|30|hb Technická ochranná opatření a monitorování

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Klíčové informace
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ V průběhu vývoje a používání AI se v různých fázích uplatňuje široká škála technických ochranných opatření. Patří sem techniky používané při vývoji modelu pro zvýšení odolnosti systémů a odolnosti vůči zneužití (například správa kvality dat), monitorování a řízení během nasazení (například filtrování obsahu a lidský dohled) a nástroje po nasazení pro monitorování širšího ekosystému AI (například ověřování původu a detekce obsahu).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Technická bezpečnostní opatření mají omezení a v žádném případě spolehlivě nebrání škodlivému chování ve všech kontextech. Například uživatelé někdy mohou získat škodlivé výstupy tak, že přeformulují požadavky nebo je rozdělí na menší kroky. Podobně nástroje, jako je vodoznakování, které jsou navrženy k identifikaci obsahu generovaného umělou inteligencí, mohou být často odstraněny nebo upraveny, což snižuje jejich spolehlivost.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Omezení jednotlivých ochranných opatření znamenají, že může být zapotřebí „obrana do hloubky“, aby se zabránilo některým škodlivým výsledkům. Například systém může kombinovat model trénovaný pro bezpečnost s filtry vstupů, filtry výstupů a monitorováním obsahu.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od vydání poslední Zprávy (leden 2025) výzkumníci dosáhli pokroku při zlepšování ochranných opatření, avšak zůstávají zásadní omezení. Například úspěšnost útoků navržených tak, aby obcházely ochranná opatření, klesá, ale stále zůstává poměrně vysoká. Existují také zásadní omezení v tom, jak důkladně lze chránit modely s otevřenými váhami.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Klíčovou výzvou pro tvůrce politik je omezenost důkazů o tom, jak účinné jsou ochranné mechanismy napříč různými reálnými způsoby použití systémů obecné umělé inteligence. Vývojáři AI se výrazně liší v tom, jaké množství informací sdílejí o svých ochranných mechanismech a monitorování. Další výzvou jsou možné kompromisy mezi uplatňováním silnějších ochranných mechanismů a zachováním výkonu nebo užitečnosti systému.
>oldlace|black||11|15|br      


Vývojáři AI mohou používat několik užitečných, ale nedokonalých technických ochranných opatření ke zmírnění a řízení rizik z obecných systémů AI, přesto přetrvávají problémy s robustností. Vývojáři stále nemohou plně zabránit tomu, aby obecné systémy AI vykonávaly i dobře známé a zjevně škodlivé činnosti, jako je poskytování uživatelům návodů na páchání trestných činů. Například výzkumníci ukázali, že systémy s nejmodernějšími ochrannými opatřeními lze obejít pomocí metod protivné výzvy (tj. „jailbreaks“) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), tím že modely rozloží komplexní škodlivé úkoly na kroky (‡1150, ‡1151, ‡1152, ‡1153, ‡1154) a pomocí jednoduchých úprav modelu (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Výzkumníci i nadále pracují na ochranných opatřeních proti poruchám a zneužití (‡690). Tyto metody se výrazně liší svým účelem i účinností a jejich dopad nakonec závisí na širším socio-technickém a řídicím (governance) kontextu, ve kterém jsou systémy AI budovány a nasazovány.

Technická opatření lze obecně rozdělit do tří kategorií: techniky pro vývoj bezpečnějších modelů; techniky používané během nasazení pro monitorování a řízení; a techniky, které podporují monitorování ekosystému po nasazení. Tabulka 3.6 shrnuje diskutovaná technická opatření, jejich účinnost a otevřené problémy.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Vývoj bezpečnějších modelů
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Příprava dat (‡1167)
  Odstraňování škodlivých dat, aby se zabránilo tomu, že se model naučí nebezpečné schopnosti. Tyto metody mohou být užitečné, mimo jiné při vývoji otevřených modelů se shodně nastavitelnými vahami, které postrádají škodlivé schopnosti a odolávají škodlivému jemnému doladění (‡55). Existují však výzvy spojené s chybami při kuraci a se škálováním (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Učení posilováním z lidské zpětné vazby (‡64*)
  Trénování modelu k souladu se stanovenými cíli, jako je to, aby byl užitečný a neškodný. To je účinný způsob, jak mají modely osvojit prospěšné chování (‡64*). Avšak nadměrná optimalizace pro lidské schválení může způsobit, že se modely budou chovat klamavě nebo lichotivě (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistické techniky zarovnání (‡1170)
  Trénování modelu tak, aby dokázal integrovat více odlišných pohledů na to, jak by se měl chovat. Tyto techniky pomáhají snížit míru, do jaké modely upřednostňují konkrétní pohledy (‡1170). Nicméně i přes tyto techniky je lidská neshoda nevyhnutelná a je obtížné navrhnout obecně přijímané způsoby vyvažování konkurenčních pohledů (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversariální trénink (‡677)
  Trénování modelu tak, aby odmítal způsobovat újmu (i v neznámých souvislostech) a aby odolával útokům ze strany zlomyslných uživatelů (např. „jailbreaks“). Jde o účinnou metodu, jak modely přimět odolávat pokusům o zneužití (‡1064), avšak výzvy v oblasti robustnosti přetrvávají (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strojové „unlearning“ (‡1175, ‡1176)
  Trénování modelu pomocí specializovaných algoritmů, které mají aktivně potlačovat škodlivé schopnosti (např. znalosti o biologických nebezpečích). Tyto techniky poskytují cílený způsob, jak ze modelů odstranit škodlivé schopnosti (‡1175, ‡1176), ale současné algoritmy pro „unlearning“ mohou být málo robustní a mohou mít nezamýšlené dopady na jiné schopnosti (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Nástroje pro interpretovatelnost a ověřování bezpečnosti (‡1177)
  Různorodá sada metod návrhu a verifikace určená k poskytnutí přísnějších záruk, že modely mají konkrétní vlastnosti související s bezpečností. Umožňují hodnotitelům činit záruky bezpečnosti s vyšší důvěrou (‡1177), ale současné metody spoléhají na předpoklady a v praxi jen zřídka dosahují konkurenční výkonnosti (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Monitorování a řízení
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mechanismy monitorování založené na hardwaru (‡1179, ‡1180, ‡1181)
  Ověřování, že autorizované procesy běží na hardwaru, aby bylo možné zkoumat bezpečnostní hrozby nebo dodržování regulatorních požadavků. Tato mechanismy nabízejí jedinečné způsoby, jak sledovat, jaké výpočty se na hardwaru provádějí a kým (‡1181). Tyto hardwarové mechanismy však nedokážou monitorovat všechny typy hrozeb a některé techniky vyžadují specializovaný hardware (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitorování interakcí uživatele (‡1154, ‡1166)
  Monitorování uživatelských interakcí z hlediska známek zlomyslného použití může vývojářům pomoci ukončit poskytování služby pro zlomyslné uživatele (‡1154, ‡1166). Vymáhání však může neúmyslně bránit prospěšnému výzkumu v oblasti bezpečnosti (‡689) a některé formy zneužití je obtížné odhalit (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sledování uživatelské interakce (‡1154, ‡1166)
  Monitorování uživatelských interakcí kvůli známkám škodlivého zneužívání může vývojářům pomoci ukončit službu pro škodlivé uživatele (‡1154, ‡1166). Prosazování však může neúmyslně bránit užitečnému výzkumu bezpečnosti (‡689) a některé formy zneužití je obtížné odhalit (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filtry obsahu (‡65*, ‡725)
  Filtrovaní potenciálně škodlivých vstupů a výstupů modelu je velmi účinný způsob, jak snížit náhodné škody a rizika zneužití (‡725). Nicméně filtry vyžadují dodatečný výpočetní výkon a jsou zranitelné vůči některým útokům (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sledování interních výpočtů modelu (‡744, ‡1183, ‡1184)
  Monitorování známek klamu nebo jiných škodlivých vnitřních forem poznávání v modelech může být účinným způsobem, jak odhalit klam (‡744, ‡1183, ‡1184). Současné metody však postrádají robustnost a spolehlivost (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitorování řetězců myšlenek (‡430, ‡435)
  Monitorování řetězového uvažování modelu kvůli známkám klamného chování nebo jinému škodlivému uvažování je účinný způsob, jak porozumět a odhalit nedostatky v tom, jak modely uvažují (‡435). Nicméně může být nespolehlivé (‡752, ‡753, ‡1186) a pokud jsou modely trénovány tak, aby produkovaly neškodné řetězové uvažování, mohou se naučit klamné chování (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Člověk v smyčce (‡1187, ‡1188, ‡1189)
  Lidský dohled a přepisy rozhodnutí systému jsou v některých aplikacích s vysokou mírou bezpečnosti nezbytné (‡1187). Tyto techniky však narážejí na zkreslení způsobené automatizací a na limity rychlosti lidského rozhodování (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sandboxing (‡1192)
  Zabránění tomu, aby AI agent přímo ovlivňoval svět, je účinný způsob, jak omezit škody, které může způsobit (‡1192). Přestože sandboxing omezuje schopnost systému přímo plnit některé úkoly (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Nástroje pro usnadnění sledování ekosystému
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Techniky identifikace modelu umělé inteligence (‡1193*, ‡1194)
  Zpřístupnění modelů, nebo jednotlivých instancí modelů, snadněji identifikovatelnými v reálných použitích pomáhá digitální forenzní analýze a povědomí o ekosystému (‡1195). Tyto techniky však mohou být obcházena pomocí některých typů úprav modelů (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dědičnost inference modelu AI (‡1197)
  Tyto techniky umožňují výzkumníkům zkoumat, jak jsou modely upravovány v AI ekosystému, zejména otevřené váhové modely. Pomáhají s digitální forenzní analýzou a povědomím o ekosystému (‡1198), ale pro důkladné zmapování ekosystému otevřených váhových modelů (‡1198) by byly nutné rozsáhlé projekty.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vodoznaky a metadata (‡1199, ‡1200, ‡1201*)
  Tyto techniky usnadňují odhalení, kdy byl nějaký text, obrázek, video atd. vygenerován nebo upraven pomocí AI, a který systém to provedl. Umožňují lépe vnímat kontext ekosystému (‡1199, ‡1200, ‡1201*). Nicméně vodoznaky a metadata lze padělat nebo odstranit některými úpravami obsahu (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Detekce obsahu generovaného umělou inteligencí (‡1203, ‡1204, ‡1205*)
  Zlepšení schopnosti uživatelů rozlišovat mezi obsahem vytvořeným pomocí AI a skutečným obsahem pomáhá v oblasti digitální forenzní analýzy a zvyšuje povědomí o ekosystému (‡1203, ‡1204). Klasifikátory však mohou být nespolehlivé (‡1205*) a mohou vykazovat různý výkon napříč modalitami.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.6: Technická ochranná opatření probíraná v této části
>white|black||9|11|br Souhrn technických ochranných opatření probíraných v této sekci, rozdělený na metody pro vývoj bezpečnějších modelů, monitorování a řízení v době nasazení a techniky, které usnadňují monitorování ekosystému.


###@ Vývoj bezpečnějších modelů

Prvním stupněm obrany proti škodám způsobeným systémy obecného účelu AI je učinit základní model bezpečnějším. Tato podsekce pojednává o bezpečnostních opatřeních, která jsou „zabudovaná do parametrů modelu“ během procesu vývoje modelu (Postava 3.6).

>white|orangered|left|14|15.5|bb Kurátorství trénovacích dat může omezit vývoj potenciálně nebezpečných schopností

Modely obecného účelu pro umělou inteligenci jsou užitečné právě proto, že po zpracování trénovacích dat rozvíjejí širokou škálu znalostí a schopností, ale některé typy trénovacích dat mají nepoměrně větší podíl na rozvoji potenciálně nebezpečných schopností. Například model AI trénovaný na odborných pracích z virologie může být lépe schopen poskytovat asistenci pro potenciálně škodlivé biologické úlohy (‡549, ‡1206*) (viz také §2.1.4. Biologická a chemická rizika). Navíc generátory obrazů/videa trénované na snímcích lidské nahoty mohou být také zneužity k vytváření ne-konsensuálních intimních deepfakeů (‡308, ‡319) (viz také §2.1.1. Obsah generovaný pomocí AI a trestná činnost).

Filtrování trénovacích dat je účinné zmírnění proti některým nežádoucím schopnostem (‡319, ‡1167, ‡1207, ‡1208). Může to však být obtížné vzhledem k velkým datovým souborům používaným k trénování modelů obecného účelu AI (‡1168), a to kvůli vysokým nákladům (‡1209), chybám ve filtrování (‡1210) a negativním dopadům na kvalitu datového souboru (‡1211). Tyto obtíže jsou zhoršeny vícejazyčnou povahou textu na internetu (‡1212), kulturními předsudky v moderování obsahu (‡1211, ‡1213, ‡1214, ‡1215) a tím, že to, zda jsou daná data „škodlivá“, závisí na kontextových faktorech (‡1216). I přesto se zdá, že filtrování potenciálně škodlivého materiálu z trénovacích dat slibuje, že se modely budou chovat bezpečněji spolehlivěji, včetně toho, že otevřené váhy (open-weight) modelů budou odolnější vůči škodlivému zásahům (‡55). Vztahy mezi obsahem trénovacích dat a emergentními schopnostmi modelu dosud nejsou plně pochopeny (‡1195) a filtrování zřejmě funguje účinněji při omezování škodlivých schopností, když se aplikuje na široké oblasti znalostí (‡55), ve srovnání s užšími typy chování (‡1206, ‡1217). Viz §3.4. Open-weight modely pro další diskusi.

![figure 3.6](images/fig3.6_safeguards.png)

##### Postava 3.6: Kde uplatnit technická bezpečnostní opatření
>white|black||9|11|br Technické bezpečnostní zajištění lze uplatnit v různých fázích vývoje modelu. Příprava dat určuje, co se modely učí během předtrénování a dolaďování. Metody založené na tréninku, jako je učení posilováním z lidské zpětné vazby a trénink robustnosti, upravují chování modelu. Testovací metody, jako jsou adversariální útoky, identifikují zbývající zranitelnosti. Některé techniky, jako algoritmy navržené jako bezpečné od základu (safe-by- design), pokrývají více fází. Zdroj: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Metody pro trénování všeobecně použitelných modelů umělé inteligence, aby byly užitečné a neškodné, jsou z velké části založené na lidské zpětné vazbě.

Je obtížné trénovat a vyhodnocovat modely tak, aby se spolehlivě shodovaly s principy vyšší úrovně, jako je užitečnost, neškodnost a pravdivost. V praxi se vývojáři snaží tohoto cíle dosáhnout tím, že zdokonalují (fine-tuning) modely AI pomocí ukázek a zpětné vazby od lidí. Například hlavní paradigma pro zdokonalování modelů AI, známé jako „reinforcement learning from human feedback“, je založeno na trénování modelů tak, aby generovaly výstupy, které lidscí anotátoři hodnotí kladně (‡1218). Klobo však kladná lidská zpětná vazba je chybným zástupným ukazatelem pro prospěšné chování (‡737, ‡878, ‡1219, ‡1220) a je omezena lidskou chybou a zkreslením (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

To vede k několika výzvám: modely jemně doladěné pomocí učení posilováním na základě zpětné vazby od lidí se někdy uživateli přizpůsobují, což je chování známé jako „lichotění“ (‡358, ‡740, ‡1226, ‡1227); poskytují odpovědi, které jsou v některých kontextech užitečné, ale v jiných škodlivé (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); poskytují odpovědi, které je obtížné vyhodnotit z hlediska správnosti (‡1233); nebo provádějí akce, jejichž užitečnost či škodlivost je záležitostí názoru (‡1234). Tabulka 3.7 uvádí příklady těchto výzev. Některý výzkum se zaměřuje na vývoj metod, které lidem pomohou lépe vyhodnocovat řešení komplexních úloh s pomocí AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tyto metody však v současnosti mají omezenou spolehlivost a není veřejně známo, do jaké míry se používají k trénování dnešních nejpokročilejších AI modelů.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Líbičství/lichocení (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Vysvětlení:
>white|black|left|11|13|br Model poskytuje pouze pozitivní zpětnou vazbu a neupozorňuje na chybějící správnou 5-7-5 slabikovou strukturu haiku.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Některé akce jsou v některých kontextech užitečné, ale v jiných škodlivé (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Vysvětlení:
>white|black|left|11|13|br Informace o biologickém riziku lze použít pro vzdělávání a obranu, ale také k tomu, aby byly k dispozici škodlivým aktérům.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Správné chování je obtížné ověřit (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Vysvětlení:
>white|black||11|13|br Správnost této odpovědi je obtížné posoudit, protože vyžaduje odborné lékařské znalosti. I pro zkušeného lékaře vyhodnocování takovýchto odpovědí vyžaduje čas a pečlivou pozornost k detailům.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Lidé se neshodují na tom, co je správně (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Vysvětlení:
>white|black|left|11|13|br Lidé se výrazně neshodují v tom, jaká je správná odpověď.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.7: Uživatelský prompt a odpověď modelu AI
>white|black||9|11|br Příklady problémů se specifikováním a motivováním prospěšného jednání z modelů AI.


>white|orangered|left|14|15.5|bb Lidé se ne vždy shodují na tom, jaké chování je žádoucí, což vyžaduje metody pro vyvážení konkurenčních preferencí

Lidé se vždy neshodnou na tom, jaké odpovědi nebo činnosti by AI modely měly nebo neměly produkovat (‡1006). To v zásadě ztěžuje vývoj modelů, jejichž jednání a dopady jsou v širokém měřítku v souladu se zájmy společnosti (‡420). Někteří výzkumníci zkoumají, čí preference se promítají do systémů AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249), a usilují o vývoj technik „pluralistického souladu“, jejichž cílem je najít rovnováhu mezi konkurenčními preferencemi (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Například vývojáři AI mohou navrhnout systémy tak, aby se vyhnuly generování kontroverzních odpovědí tím, že odmítnou reagovat na určité požadavky, nebo aby se sladily se středovým (mediánovým) názorem v určité relevantní vzorku lidí, případně aby systémy personalizovaly pro jednotlivé uživatele.

Obvyklou výzvou těchto přístupů je, že obecně se AI systémy nemohou stejně dobře přizpůsobit preferencím každého, a že jejich navazující společenské dopady budou různé skupiny lidí ovlivňovat odlišně. Někteří výzkumníci tvrdí, že většina technických přístupů k pluralistickému sladění neřeší, a případně odvádí pozornost od, hlubších problémů, jako jsou systematické předsudky, dynamika společenské moci a koncentrace bohatství a vlivu (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Vývojáři AI používají „adversarial training“ k vylepšení robustnosti modelu.

Je náročné zajistit, aby AI modely spolehlivě přenášely prospěšné chování, které se naučí během tréninku, do kontextů nasazení v reálném světě. I modely trénované pomocí „dokonalého“ tréninkového signálu mohou selhat při úspěšném zobecňování na všechny dosud neviděné kontexty (‡738, ‡739, ‡1255, ‡1256, ‡1257). Například někteří výzkumníci zjistili, že chatboti častěji provádějí škodlivé akce v jazycích, které jsou v jejich tréninkových datech nedostatečně zastoupené (‡159, ‡880, ‡1258*, ‡1259), což zahrnuje mnoho jazyků, jež se převážně používají v Globálním Jihu.

V posledních letech výzkumníci také vytvořili rozsáhlou sadu nástrojů „techniků adversarialního útoku“, které lze použít k tomu, aby modely generovaly potenciálně škodlivé odpovědi (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Například nedávná iniciativa shromáždila z davu více než 60,000 různorodých příkladů úspěšných útoků proti nejmodernějším AI modelům, což je přimělo porušit zásady jejich společností týkající se přijatelného chování modelů (‡1149). Tabulka 3.8 uvádí příklady „jailbreak“ technik, které výzkumníci ukázali jako schopné přimět modely k vyhovění škodlivým požadavkům.

Jedna metoda ke zlepšení robustnosti modelů je známá jako „adversariální trénink“ (‡1064). Zahrnuje konstruování „útoků“ (např. jailreaků) navržených tak, aby model jednal nežádoucím způsobem, a trénování modelu na to, aby těmto útokům vhodně čelil. Adversariální trénink je však nedokonalý (‡1260, ‡1261). Útočníci jsou i nadále konzistentně schopni vyvíjet nové úspěšné útoky proti špičkovým modelům (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Jelikož vývojáři potřebují konkrétní příklady selhávajících režimů, aby proti nim mohli trénovat (‡512, ‡1263), výsledkem je neustálá hra „kočka a myš“, v níž vývojáři průběžně aktualizují modely v reakci na nově objevené zranitelnosti a protivníci průběžně hledají nové útoky. Někteří výzkumníci navrhli adversariální trénink ve větším měřítku (‡1264, ‡1265) nebo nové algoritmy (‡675, ‡676, ‡1263, ‡1266, ‡1267) pro zlepšení robustnosti, avšak moderní systémy umělé inteligence zůstávají trvale zranitelné.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Vytvářejte škodlivé požadavky v šifrovaném textu, jako je Morseova abeceda (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Načerpejte systém příklady vyhovujících odpovědí na škodlivé žádosti (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Vytvářejte škodlivé požadavky v málo používaných jazycích s nízkými zdroji, které budou pravděpodobně méně využívané při trénování (např. svahilština (‡1271)))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie: Rozdělte škodlivý úkol na více neškodných dílčích úkolů (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.8: Strategie jailbreaku
>white|black||9|11|br Zlomyslní aktéři a red teamy použili různé typy „jailbreaků“, aby přiměli modely umělé inteligence vyhovět škodlivým požadavkům, které by obvykle kvůli bezpečnostním opatřením odmítly. Ukázkové výstupy byly sepsány autory Reportu pro ilustrační účely. Mnoho současných nejmodernějších modelů umělé inteligence nyní odolává většině těchto metod, ale stále se objevují nové techniky jailbreaking.


>white|orangered|left|14|15.5|bb Techniky „unlearning“ mohou zmírnit specifické škodlivé schopnosti modelu

Další strategie pro zmírnění rizik obecněúčelové umělé inteligence spočívá v tom, že se modely dofine-tunují tak, aby postrádaly schopnosti v určitých oblastech s vysokým rizikem (‡1175, ‡1176). Například výzkumníci pracují na vývoji algoritmů „machine unlearning“, které mohou specificky potlačovat schopnosti související s bioterorismem nebo s generováním fotorealistických snímků nahých lidských těl (‡903, ‡1272, ‡1273). Tyto metody mohou modely výrazně učinit bezpečnějšími, ovšem za cenu omezení některých pozitivních využití těch schopností, které byly „zapomenuty“. Jako způsob navrhování „tamper-resistant“ otevřeně nasaditelných modelů, jež dokážou odolávat škodlivému dofine-tunování, bylo rovněž navrženo omezit znalosti AI modelů v škodlivých doménách (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Dosud se však tohle podařilo provést robustně jen obtížně (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Viz §3.4. Open-weight models pro další diskusi.

>white|orangered|left|14|15.5|bb Někteří výzkumníci pracují na metodách pro silnější záruky bezpečnosti prostřednictvím interpretace vnitřních stavů modelu nebo matematického ověřování

Někteří výzkumníci pracují na metodách, které by umožnily přísněji ověřovat bezpečnostně relevantní vlastnosti modelů. V jednom přístupu se výzkumníci snaží interpretovat interní výpočty modelů buď k identifikaci rizik, nebo k formulaci přesvědčivějších argumentů, že je model bezpečný (‡1285, ‡1286). Například v rámci proof of concept výzkumníci ukázali, že nástroje pro analýzu interních výpočtů jazykového modelu mohou pomoci hodnotitelům identifikovat škodlivé chování (‡1287). V 2025 společnost Anthropic rovněž začala analyzovat interní části modelů jako způsob studia situačního povědomí modelů a „záměru“ (‡2). Tyto typy metod však v současnosti nejsou běžné ani není známo, že by byly srovnatelné nebo konkurenceschopné s jinými technikami hodnocení.

Jiný přístup k zajištění silnějších záruk bezpečnosti spočívá v konstruování matematických důkazů, že model splní určité bezpečnostní podmínky (‡1177, ‡1282, ‡1288). Tyto důkazy však předpokládají, že testovací kontext odpovídá nasazovacímu kontextu, a nebyly ověřeny proti mnoha typům protivníků.

V současnosti je také nelze škálovat na velké modely. Celkově mezi odborníky probíhá významná debata o příslibu metod interpretovatelnosti a formálního ověřování.

###@ Monitorování a řízení v době nasazení

Kromě ochranných opatření zavedených během vývoje modelu je druhou linií obrany proti škodlivému chování externí ochrana, která se zaměřuje na monitorování a řízení akcí modelu nebo systému během nasazení. Tato ochranná opatření pomáhají zmírňovat selhání a zneužití, jako jsou halucinované výstupy a škodlivé instrukce.

>white|orangered|left|14|15.5|bb Nasazující modely mohou použít různé nástroje k identifikaci a řešení vysoce rizikového chování modelů.

Když je systém AI v provozu, může nasazující osoba sledovat známky rizika a zasáhnout, pokud se objeví. Například může zkontrolovat vstupy modelu kvůli známkám protivníkových útoků, filtrovat nevhodný obsah z výstupů nebo sledovat „řetězec uvažování“ systému kvůli známkám škodlivých plánů. Body, ve kterých mohou nasazující osoby sledovat a zasahovat do toho, jak lidé používají jejich systémy, zahrnují hardware (‡1180, ‡1181), uživatelské interakce (‡1154, ‡1166), vstupy a výstupy (‡65, ‡725, ‡1182), interní výpočty (‡744, ‡1183, ‡1184) a „řetězec uvažování“ (‡430, ‡435). Existují také různé akce, které mohou nasazující osoby provést, když jsou rizika identifikována. Patří sem zaznamenávání informací, filtrování/úprava škodlivého obsahu, označení neobvyklé aktivity, vypnutí systému nebo spuštění pojistek. Postava 3.7 znázorňuje příklady běžných mechanismů monitorování a řízení.

Protože jsou všestranné a často účinné, tyto mechanismy se široce používají a mohou předcházet mnoha typům neúmyslných škod (‡725, ‡751, ‡1289). Tyto ochranné mechanismy jsou však nedokonalé, zejména při zlomyslných útocích optimalizovaných tak, aby je učinily nefunkčními (‡752, ‡1182). Nedávný výzkum se také zabýval tím, jak může být monitorování nespolehlivé, pokud je systém optimalizován pomocí skóre monitoru, například tak, že se sníží spolehlivost chain of thought (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Postava 3.7: Monitorovací a řídicí techniky
>white|black||9|11|br Techniky monitorování a řízení fungují na více místech: provádějí kontrolu vstupů a výstupů na přítomnost škodlivého obsahu, sledují vnitřní stavy modelu, omezují vnější akce pomocí sandboxingu a zajišťují lidský dohled. Zdroj: Mezinárodní zpráva o bezpečnosti umělé inteligence 2026.


>white|orangered|left|14|15.5|bb Lidé v řízení umožňují přímý dohled v prostředích s vysokými sázkami

Aby se snížila pravděpodobnost selhání ze strany AI agentů (viz §2.2.1. Spolehlivostní výzvy), mohou nasazující organizace usilovat o návrh AI systémů tak, aby fungovaly ve spolupráci s lidmi spíše než plně autonomně (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). To je důležité pro případy použití, kde mohou nesprávná rozhodnutí vést k významným škodám, jako je tomu ve financích, zdravotnictví nebo při policejní činnosti. Mít „člověka v rozhodovacím řetězci“ (human in the loop) je však často nepraktické. Někdy k rozhodování dochází příliš rychle, například v chatovacích aplikacích s miliony uživatelů. V jiných případech může lidská zaujatost a chyba zvyšovat rizika v důsledku kumulace chyb (‡1187). Lidé zapojení do procesu také často vykazují „automatizační zaujatost“, což znamená, že obvykle vkládají do AI systému větší důvěru, než jaká je na místě (‡1190, ‡1191) (viz §2.3.2. Rizika pro autonomii člověka).

>white|orangered|left|14|15.5|bb „Sandboxing“ chrání před riziky vyplývajícími z autonomního chování

AI agenti, kteří mohou jednat autonomně bez omezení na Webu nebo ve fyzickém světě, představují zvýšená rizika (viz §2.2.1. Problémy se spolehlivostí). „Sandboxing“ zahrnuje omezení způsobů, jakými mohou AI agenti přímo ovlivňovat svět, čímž se výrazně usnadní jejich dohled a správa (‡640, ‡1192, ‡1295). Například omezení schopnosti AI systému zveřejňovat obsah na internetu nebo upravovat souborový systém počítače může zabránit neočekávaným škodám z neočekávaných činností (‡1296). Tyto přístupy však nelze vždy použít pro aplikace, ve kterých AI systém nutně musí jednat přímo ve světě.

###@ Nástroje pro monitorování ekosystému: modelování a původ dat

Nástroje pro modelování a původ dat jsou technické nástroje pro zkoumání ekosystému AI, které zvyšují povědomí o následných použitích a dopadech systémů AI.

>white|orangered|left|14|15.5|bb Techniky původu systémů založené na AI pomáhají dohledat použití a dopady systémů

Vývojáři a provozovatelé mohou používat různé techniky ke studiu využití modelu a jeho šíření „v reálném světě“. Například mohou modelům zadat jedinečné identifikační chování (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) nebo aplikovat jedinečné vzory na váhy jednotlivých modelů s otevřenými váhami (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Je však otevřeným problémem, jak tyto techniky učinit odolnějšími vůči úpravám modelu (‡1195, ‡1196*). Výzkumníci také pracují na metodách pro „odvozování původu modelu“ (‡1197, ‡1198, ‡1305, ‡1306), které pomáhají zodpovídat otázky typu: „Byl model X upravený pomocí fine-tuningu nebo destilovaný z modelu Y?“ Nakonec se někteří vývojáři snaží vyvíjet protokoly a infrastrukturu pro AI agenty, aby při interakci s externími systémy usnadnili identifikaci a ověřování (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Postava 3.8: vodoznaky vkládají do obrázků a zvuku nepostřehnutelné poruchy
>white|black||9|11|br Vodoznaky vkládají do obrázků a zvuků nepozorovatelné perturbace, které umožňují detekčním nástrojům identifikovat obsah vytvořený pomocí AI. V této postavě jsou vodoznaky jak pro obrázek, tak pro zvuk přehnané, aby bylo zajištěno viditelné rozpoznání. Zdroj: Chameleon (obrázek) z Unsplash (‡1313*). Ostatní prvky vytvořili autoři Reportu. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Postava 3.9: Úspěšnost útoků typu prompt injection
>white|black||9|11|br Úspěšnost útoků typu prompt injection, jak uvádějí vývojáři AI pro hlavní modely vydané mezi květnem 2024 a srpnem 2025. Každý bod představuje podíl úspěšných útoků v rámci 10 pokusů proti danému modelu krátce po vydání. Uváděná úspěšnost takových útoků v čase klesá, ale zůstává relativně vysoká. Zdroj: Zou et al. 2025 (‡1149), citováno v Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI metody detekce obsahu pomáhají monitorovat šíření a dopady AI-generovaného obsahu

Vodoznaky, metadata a další detektory obsahu generovaného umělou inteligencí mohou výzkumníkům pomoci sledovat a zkoumat reálný dopad obsahu vytvářeného pomocí AI ve světě. 

Nejprve jsou vodoznaky dat nenápadné, ale odlišné motivy vkládané do digitálních médií, které mohou kódovat informace o jejich původu (‡1199, ‡1200, ‡1201*). U textu obvykle mají podobu nenápadných zkreslení v volbě slov a stylu (‡1308, ‡1309); u obrázků a videa jde o nenápadné vzory přes pixely (‡1310); a u zvuku o nenápadné vzory ve zvukových vlnách (‡1311). Postava 3.8 to znázorňuje.

Kromě vodoznaků lze obsah vygenerovaný pomocí umělé inteligence ukládat také pomocí formátů souborů, které ukládají metadata o tom, jak byly vytvořeny. Například mnoho mobilních zařízení ukládá obrazové a zvukové soubory ve formátu, který dokáže uchovávat informace o nastavení fotoaparátu, čase, poloze atd. (‡1312). Podobná metadata mohou být použita k uložení informací o tom, zda byla data vygenerována systémem umělé inteligence. Stejně jako otisky prstů v kriminální forenzní praxi lze vodoznaky a metadata pozměnit nebo odstranit, ale i přesto jsou užitečné.

Výzkumníci se také snaží vyvinout detektory obsahu generovaného pomocí AI (‡1203, ‡1204, ‡1205*) , které mají pomoci rozpoznat obsah generovaný AI v reálném prostředí, i když nejsou k dispozici žádné vodoznaky ani metadata. Tyto identifikační techniky však mají omezenou úspěšnost.

###@ Aktualizace

Od vydání poslední Zprávy (leden 2025) bylo dosaženo pokroku při vývoji systémů umělé inteligence s více účinnými vrstvami ochranných opatření. Jak je uvedeno v §3.2. Postupy řízení rizik, defence-in-depth je základní princip řízení rizik (‡1314). Například systémy umělé inteligence, které kombinují bezpečnostně trénované modely s filtry vstupů, filtry výstupů a dalšími monitorovacími mechanismy obsahu, jsou stále častěji zkoumány a nasazovány (‡32, ‡65, ‡1182*). Nedávný výzkum také ukázal, že i když vývojáři modelů dosáhli pokroku při zvyšování odolnosti vůči pokusům obejít ochranná opatření, útočníci se stále ve vysokém podílu případů úspěšně obejít (Postava 3.9).

###@ Mezery v důkazech

Je potřeba více důkazů, aby výzkumníci pochopili a dokázali zohlednit omezení existujících přístupů. Technická ochranná opatření pro systémy AI jsou zdokonalována, ale techniky narážejí na omezení. Například pokrok v zlepšování robustnessu v nejhorším případě u obecně použitelných AI systémů byl pomalý a existují zásadní omezení v tom, jak důkladně lze chránit a monitorovat open-weight modely (‡1195, ‡1315, ‡1316) (viz také §3.4. Open-weight models). Zároveň ne všechny technické ochrany jsou stejně časté, stejně účinné nebo stejně prokazatelné v reálném světě. Například adversariální trénink se používá téměř všude u nejmodernějších modelů (‡64*, ‡677), zatímco techniky interpretovatelnosti modelů a formální verifikace byly dosud v produkčních systémech využity jen minimálně (‡1177, ‡1285).

###@ Výzvy pro tvůrce politik

Mezi klíčové výzvy pro tvůrce politik patří rozhodnout, zda a jak by měli podporovat výzkum, vývoj, hodnocení a zavádění technických ochranných opatření a metod monitorování. Je to obtížné, protože porozumění vědců tomu, jak nejlépe prakticky zabezpečit mechanismy, se stále vyvíjí a osvědčené postupy zatím nejsou ustálené. Například různí vývojáři uplatňují různá ochranná opatření a jejich přístupy k technické mitigaci rizik se obecně značně liší (‡1116). Konečně, existence účinných technických ochranných opatření sama o sobě nezaručuje bezpečnost, protože přijetí a implementace se mohou lišit napříč vývojáři a v různých kontextech nasazení.

