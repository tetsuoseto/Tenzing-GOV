##########
>white|orangered|left|14|30|hr Sekce 3.2
### 3.2. Postupy řízení rizik
>white|orangered|left|24|30|hb Postupy řízení rizik

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Klíčové informace
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Správa rizik obecněúčelové AI zahrnuje řadu postupů používaných k identifikaci, vyhodnocení a snížení rizik plynoucích z obecněúčelové AI. Patří sem testování a hodnocení na úrovni modelu (například „red-teaming“), organizační procesy řídící rozhodnutí o vývoji a uvolnění, podmíněné ochranné mechanismy (například „if-then“ závazky) a hlášení incidentů.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Několik vývojářů AI vytvořilo Rámce pro bezpečnost AI Frontier. Tyto rámce obsahují informace o posuzování rizik a stanovují podmíněná opatření, jako jsou omezení přístupu, která společnosti plánují zavést pro výkonnější modely. Liší se v tom, jaká rizika pokrývají, jak definují prahové hodnoty schopností a jaké akce se spustí, když jsou prahové hodnoty dosaženy.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Důkazy o reálné účinnosti postupů řízení rizik v oblasti AI nadále zůstávají omezené. Chybějící hlášení incidentů a monitorování ztěžuje posouzení toho, jak dobře současné postupy snižují rizika, ani jak konzistentně jsou zaváděny.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od zveřejnění poslední Zprávy (leden 2025) se řízení rizik stalo strukturovanějším díky novým iniciativám v oblasti průmyslu a správy a řízení. Nové nástroje, jako je Kodex postupů pro obecné účely EU v oblasti AI, Rámec pro bezpečnostní řízení AI v Číně 2.0 a Rámec pro podávání zpráv v rámci Hiroshima AI Process skupiny G7, spolu s iniciativami vedenými společnostmi, ilustrují trend směrem k více standardizovaným přístupům k transparentnosti, vyhodnocování a hlášení incidentů.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dynamika trhu a tempo vývoje AI přinášejí další výzvy. V důsledku konkurenčního tlaku mohou společnosti vyvíjející AI čelit kompromisům mezi rychlejšími vydáními produktů a investicemi do úsilí o snížení rizik. Mnohé škody související s AI jsou navíc přenášeny na externí subjekty a právní odpovědnost za ně zůstává nejasná a procesy řízení se mohou jen pomalu přizpůsobovat změnám v prostředí AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mezi klíčové výzvy pro tvůrce politik patří stanovit priority mezi různými riziky, která představuje generická umělá inteligence, a vyjasnit, které subjekty napříč hodnotovým řetězcem umělé inteligence jsou k jejich zmírňování nejlépe předurčeny. Tyto výzvy se zhoršují omezenou viditelností toho, jak se rizika v praxi identifikují, hodnotí a řídí, a také roztříštěným sdílením informací mezi vývojáři, nasazujícími subjekty a poskytovateli infrastruktury.
>oldlace|black||11|15|br      


Řízení rizik v oblasti AI zahrnuje řadu postupů, jejichž cílem je identifikovat, vyhodnocovat a snižovat pravděpodobnost a závažnost rizik spojených s systémy AI. Tyto postupy mohou zavádět vývojáři AI, nasazovatelé, hodnotitelé i regulátoři. Příklady zahrnují modelování hrozeb, zařazování rizik do úrovní, red-teaming, auditování a hlášení incidentů. Tato část popisuje současné postupy řízení rizik, novinky ve vývoji a zbývající omezení.

Od začátku roku 2025 se vyvinulo několik nových mezinárodních iniciativ pro řízení rizik obecněúčelové umělé inteligence, včetně rámců organizační transparentnosti a reportingu rizik a také regulačních a governance rámců.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Postava 3.4: Čtyři komponenty řízení rizik
>white|black||9|11|br Čtyři kategorie metod pro řízení rizik obecné umělé inteligence: identifikace rizik; analýza a vyhodnocení rizik; zmírňování rizik; a řízení rizik. Tyto činnosti tvoří iterativní a cyklický proces. Řízení rizik, zobrazené uprostřed, napomáhá úspěchu ostatních komponent. Zdroj: International AI Safety Report 2026.


Mezi zbývající výzvy patří omezená standardizace, která komplikuje shodu a hodnocení, a omezené důkazy o reálné účinnosti v praxi. Dále se institucionální, kulturní a politické kontexty liší po celém světě, což znamená, že přístupy k identifikaci a řízení rizik, včetně akceptovatelných prahů rizika, se mohou v jednotlivých regionech lišit. Diskuse v této části o přístupech k řízení rizik je popisná: jejím cílem je informovat aktéry v ekosystému AI o současných globálních přístupech k řízení rizik. Kde jsou k dispozici, probírá se také dostupnými důkazy podložená účinnost a omezení těchto přístupů, nicméně doporučení pro politiku nejsou předmětem této práce.

###@ Součásti řízení rizik

Řízení rizik je iterativní proces s postupy a metodami, které pokrývají celý cyklus vývoje a nasazení AI, ale které spolu koherentně fungují (‡969). Řízení rizik pro obecněúčelovou AI může zahrnovat role pro širokou škálu aktérů včetně datových vědců, inženýrů modelů, auditorů, odborníků z praxe, vedoucích pracovníků, koncových uživatelů, dotčených komunit, dodavatelů třetích stran, tvůrců politik, vlád, organizací pro standardizaci a organizací občanské společnosti (‡970, ‡971, ‡972). Vedoucí standardy pro řízení rizik jsou často vzájemně kompatibilní, ale používají odlišnou terminologii pro popis prvků řízení rizik (‡973, ‡974). Obvykle mají čtyři propojené komponenty (Postava 3.4): identifikace; analýza a vyhodnocení; zmírňování; a řízení rizik (‡970, ‡973, ‡975, ‡976). Následující tabulky poskytují ilustrativní příklady relevantních metod, technik a nástrojů. Postupy se nadále vyvíjejí, takže tabulky nejsou vyčerpávající a použitelnost se bude lišit podle kontextu.

###@ Identifikace rizik

Identifikace rizik je proces hledání, rozpoznávání a popisování rizik. Komplexní identifikace rizik typicky zahrnuje hodnocení řízená schopnostmi, která testují, zda modely disponují konkrétními nebezpečnými schopnostmi (‡977), a také modelování rizik (‡978) a predikci (‡715*), které se používají k zkoumání existujících a nově vznikajících rizik. Tabulka 3.1 uvádí různé příklady postupů identifikace rizik. Identifikace rizik dále čerpá z zapojení relevantních odborníků a komunit, aby se porozumělo širšímu kontextu, v němž rizika vznikají (‡979, ‡980). Mechanismy, jako jsou programy bug bounty, mohou tento proces podpořit tím, že motivují identifikaci dříve neznámých zranitelností (‡981) (Tabulka 3.1). Klíčovým cílem identifikace rizik je zohlednit jak dobře známá a dobře pochopená rizika, tak i potenciální budoucí rizika, která zůstávají nejistá nebo jsou špatně charakterizovaná (‡982). To je obzvlášť důležité pro obecněúčelovou umělou inteligenci, kde mnoho rizik zatím nemusí být plně pochopeno nebo pozorovatelné (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Programy bug bounty
  Bug bounties nebo programy pro zveřejňování zranitelností motivují lidi k nalezení a nahlášení zranitelností v systémech AI. Několik vývojářů zavedlo programy bug bounty (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Odborná konzultace
  Oboroví experti, uživatelé a dotčené komunity poskytují poznatky o pravděpodobných rizicích. Vznikají pokyny pro participativní a inkluzivní umělou inteligenci (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Diagram rybí kosti (Ishikawa)
  Diagramy rybí kosti jsou dobře zavedené nástroje analýzy příčin, a výzkumníci navrhli používat je pro strukturovanou analýzu incidentů souvisejících s riziky v oblasti AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Předpovídání
  Předpovídání je proces určování budoucích událostí nebo trendů na základě analýzy minulých a současných dat. Používá se k porovnání relativní pravděpodobnosti, například různých ekonomických výsledků, díky pokročilé umělé inteligenci (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Taxonomie rizik
  Taxonomie rizik jsou způsob, jak kategorizovat a organizovat rizika napříč více dimenzemi. Existuje několik takových, které popisují rizika obecněúčelové umělé inteligence (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Plánování scénářů
  Plánování scénářů zahrnuje vytváření věrohodných budoucích scénářů a analýzu toho, jak se rizika realizují. Použilo se to k prozkoumání rizik a dopadů modelů umělé inteligence (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelování hrozeb
  Modelování hrozeb je proces identifikace hrozeb a zranitelností systému. Mnoho vývojářů AI zdůrazňuje jeho využití k předvídání možných scénářů zneužití systémů AI (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.1: Příklady identifikace rizik v obecné správě rizik pro umělou inteligenci pro všeobecné použití
>white|black||9|11|br Příkladové metody pro identifikaci rizik v oblasti AI uvedené abecedně. Zahrnuté metody
jsou navrženy tak, aby podporovaly identifikaci rizik pro mnoho různých typů rizik, včetně rizik spojených se škodlivým zneužitím, rizik spojených s poruchami a systémových rizik. Vzhledem k počínajícímu stavu řízení rizik obecněúčelové umělé inteligence nebudou všechny metody vhodné pro každého vývojáře nebo provozovatele umělé inteligence.


>white|orangered|left|14|15.5|bb Modelování hrozeb a taxonomie rizik jsou významné metody identifikace rizik

Dvě významné metody pro identifikaci rizik plynoucích z generativního účelového AI jsou modelování hrozeb (International AI Safety Report 2026) (strukturovaný proces mapování toho, jak se mohou projevit rizika související s AI) a risk taxonomie. Společnost Meta například používá cvičení modelování hrozeb k předjímání možných scénářů zneužití svých AI modelů (‡990), a Anthropic zahrnuje modelování hrozeb jako součást svého ASL-3 Deployment Standardu (‡991). AI risk a hazard taxonomie, které vyjmenovávají kategorie rizik a příklady, mohou stejně tak sloužit jako výchozí bod pro konceptualizaci, identifikaci a specifikaci podstatných rizik spojených s generativním účelovým AI v konkrétních aplikačních doménách (‡906, ‡988, ‡992, ‡993).

###@ Analýza rizik a vyhodnocení

Analýza a vyhodnocení rizik je proces určování úrovně rizika modelu nebo systému AI a jejího porovnání se stanovenými kritérii za účelem posouzení přijatelnosti nebo potřeby zmírnění (‡994, ‡995, ‡996, ‡997). Zahrnuje postupy, jako je měření výkonnosti modelu na benchmarcích (‡998) a vyhodnoceních (‡176, ‡715), provádění cvičení typu red-teaming (‡999*), posuzování dopadů (‡1000) a audity (‡1001, ‡1002). Příklady obecné analýzy a vyhodnocení rizik pro AI pro všeobecné použití naleznete v Tabulka 3.2. Metody jsou navrženy tak, aby podporovaly analýzu a vyhodnocení mnoha různých typů rizik současně.

Klíčovými cíli analýzy a vyhodnocení rizik je provádět hodnocení schopností modelů a zranitelností (‡1003), využívat robustní modelování rizik k informování rozhodnutí o prahových hodnotách rizika (‡1004, ‡1005) a porozumět tomu, jak se systémy AI v praxi používají, aby bylo možné posoudit navazující společenské dopady (‡869, ‡904, ‡905, ‡1006). Procesy analýzy a vyhodnocení rizik se často považují za pravděpodobnější způsob, jak identifikovat rizika, když zahrnují nezávislé přezkoumání (‡1001, ‡1007), opírají se o odborné znalosti napříč sektory (‡1008) a zahrnují různé pohledy z více oblastí a disciplín, stejně jako z komunit, jichž se to týká (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audity
  Audity jsou formální posouzení výkonu a dopadů modelů AI a/ nebo souladu organizace s normami, politikami a postupy, prováděné interně nebo externí stranou. Auditování AI je rychle rostoucí obor a existuje mnoho nástrojů a postupů pro auditování modelů AI a postupů vývojářů modelů AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmarky
  Benchmarky jsou standardizované, často kvantitativní testy nebo metriky používané k vyhodnocení a porovnání výkonu systémů AI na pevně dané sadě úloh navržených tak, aby reprezentovaly reálné použití (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metoda motýlku
  Metoda motýlku (bowtie) je dobře známý způsob vizualizace, kde lze přidat kontroly pro zmírnění rizikových událostí. Poskytuje jasné rozlišení mezi proaktivním a reaktivním řízením rizik (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb metoda Delphi
  Metoda Delphi je technika skupinového rozhodování, která používá řadu dotazníků k získání shody od panelu odborníků (‡1020, ‡1021). Používá se k tomu, aby napomohla zkoumat možné budoucnosti s pokročilou umělou inteligencí (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Testování v terénu
  Terénní testování vyhodnocuje výkon a dopad systému AI v reálném, provozním prostředí. Některé výzkumy zdůrazňují terénní testování jako doplněk k vyhodnocování modelu pro posuzování reálných výsledků a následků (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Posouzení dopadu
  Hodnocení dopadů posuzují potenciální dopady technologie nebo projektu. To může zahrnovat kvantifikaci, agregaci a upřednostnění dopadů. Například Nařízení o umělé inteligenci (AI Act) EU vyžaduje, aby vývojáři systémů umělé inteligence s vysokým rizikem provedli posouzení dopadů na základní práva (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hodnocení modelu
  Hodnocení modelů zahrnuje procesy a testy pro posouzení a měření výkonu modelu AI na konkrétní úloze. Existuje celá řada hodnocení AI pro posouzení různých schopností a rizik, včetně oblasti bezpečnosti, kybernetické bezpečnosti a společenského dopadu (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pravděpodobnostní posouzení rizik
  Pro posuzování pravděpodobnostního rizika je metodika pro vyhodnocování rizik spojených se složitými systémy nebo procesy, která zahrnuje nejistotu. Byla přizpůsobena pro pokročilé AI systémy (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teamování
  Red-teamování je cvičení, v němž skupina lidí nebo automatizované systémy předstírají, že jsou protivníkem, a napadají technologické systémy organizace, aby identifikovaly zranitelnosti. Mnoho společností zabývajících se AI má interní postupy pro red-teamování AI systémů (‡458, ‡1028). Red-teamování mohou provádět i aktéři mimo společnosti. Týmy čelí výzvám, jako je omezený přístup, ale mohou také přinést odlišné postřehy (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rizikové matice
  Rizikové matice jsou vizuální nástroj, který pomáhá upřednostňovat rizika podle pravděpodobnosti výskytu a potenciálního dopadu (‡1027). Někteří vývojáři AI zahrnují do svých Rámců bezpečnosti Frontier AI Safety základní rizikové matice (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prahové hodnoty rizika/ úrovně rizika
  Prahové hodnoty nebo úrovně rizika jsou kvantitativní nebo kvalitativní limity, které rozlišují přijatelné od nepřijatelné riziko a spouštějí konkrétní opatření řízení rizik při jejich překročení. Pro AI pro obecné účely se určují na základě kombinace schopností, dopadu, výpočetního výkonu, dosahu a dalších faktorů (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolerance rizika
  Tolerance vůči riziku označuje úroveň rizika, kterou je organizace ochotna přijmout. V oblasti AI se tolerance vůči riziku často nastavuje implicitně prostřednictvím firemních politik a praxe, zatímco některé regulační režimy explicitně definují nepřijatelné riziko a připojují k němu právní důsledky (‡1032). Některé společnosti popisují svou toleranci vůči riziku z hlediska mezního rizika nového modelu; tedy míry, do jaké model kontrafaktuálně zvyšuje riziko nad rámec toho, které již způsobují existující modely nebo jiné technologie (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bezpečnostní případy
  Bezpečnostní případ je strukturovaná argumentace podpořená důkazy, která prokazuje, že je systém v daném kontextu přijatelně bezpečný pro provoz. Novější literatura (‡1037, ‡1038, ‡1039) zkoumala bezpečnostní případy pro systémy „frontier AI“ a některé Rámce bezpečnosti pro „Frontier AI“ na ně odkazují (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Analýza bezpečnosti systému
  Analýza bezpečnosti systému zdůrazňuje závislosti mezi jednotlivými komponentami a systémem, jehož jsou součástí, aby bylo možné předvídat, jak se na úrovni systému mohou objevit systémová nebezpečí v důsledku selhání komponent nebo procesů, případně interakcí mezi subsystémy, vlivů lidských faktorů a podmínek prostředí. Přístupy uplatňované pro systémy s umělou inteligencí v literatuře zahrnují systémo-teoretickou procesní analýzu (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.2: Analýza/vyhodnocení rizik v řízení rizik obecné umělé inteligence
>white|black||9|11|br Příklady metod pro analýzu/hodnocení rizik AI, uvedené v abecedním pořadí. Vzhledem k tomu, že řízení rizik obecněúčelové AI je v počátečním stadiu, ne všechny metody budou vhodné pro každého vývojáře nebo provozovatele AI.


>white|orangered|left|14|15.5|bb Mezi běžné nástroje analýzy rizik patří benchmarky a hodnocení modelů

Benchmarky a vyhodnocení modelů jsou standardizované testy k posouzení výkonu všeobecných systémů umělé inteligence na konkrétních úlohách. Výzkumníci vyvinuli širokou škálu benchmarků a vyhodnocení, včetně sad náročných otázek s možností odpovědi, problémů z oblasti softwarového inženýrství a pracovních úloh v simulovaných kancelářských prostředích (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Hodnocení škodlivých schopností (‡715) se používá k posouzení, zda má všeobecný model nebo systém umělé inteligence obzvlášť nebezpečné znalosti nebo dovednosti, jako je schopnost napomáhat při kybernetických útocích (viz §2.1.3. Cyberattacks).

Vysoce významná rozhodnutí společností a vlád týkající se uvolnění modelů se částečně opírají o tyto evaluace (‡1050, ‡1051, ‡1052). Benchmarchy však výrazně kolísají co do kvality i rozsahu (‡998, ‡1003) a může být obtížné posoudit jejich validitu kvůli četným nedostatkům v benchmarkových postupech (‡902, ‡909, ‡1003, ‡1053*). Například benchmarchy mohou dosáhnout stavu „saturace“ – když se skóre mnoha modelů blíží hornímu skóre – což znamená, že již modely nedokážou silně odlišit. Modely navíc stále častěji dokážou rozpoznat určité úlohy jako evaluace a vykazovat odlišné chování než by tomu bylo u podobných úloh v kontextech nasazení v důsledku „situačního povědomí“ (viz §2.2.2. Ztráta kontroly). Nakonec mají benchmarchy a evaluace dobře zdokumentovaná omezení: zejména nezachycují rizika spojená s použitím obecněúčelové AI v nových doménách a pro nové úlohy, protože se testovací podmínky od reálného používání v různé míře liší (‡913) (viz §1.2. Aktuální schopnosti a §3.1. Technické a institucionální výzvy).

>white|orangered|left|14|15.5|bb Red teaming umožňuje provádět specifičtější posuzování rizik pro danou oblast.

Další běžnou metodou pro vyhodnocování rizik je red-teaming. „Red team“ je skupina hodnotitelů pověřená hledáním zranitelností, omezení nebo možností zneužití. Red-teaming může být specifický pro danou doménu a prováděný odborníky z praxe, nebo může být otevřený, aby prozkoumal nové rizikové faktory. Například red tým může zkoumat „jailbreaking“ útoky, které obcházejí bezpečnostní omezení modelu (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Na rozdíl od benchmarků je klíčovou výhodou red-teamingu to, že red teamy mohou přizpůsobit své vyhodnocování konkrétnímu testovanému systému. Například red teamy mohou navrhnout vlastní vstupy pro identifikaci nejhorších typů chování, příležitostí pro zlomyslné použití a neočekávaných selhání. Může však vyžadovat zvláštní přístup k modelům a nemusí odhalit důležité třídy rizik (‡999, ‡1028).

Důležité je, že absence identifikovaných rizik neznamená, že tato rizika jsou nízká: předchozí práce ukazuje, že chyby často unikají detekci, zejména když mají red teamy omezený přístup nebo zdroje (‡1060). Výzkum se také ptá, zda může red-teaming poskytovat spolehlivé a reprodukovatelné výsledky (‡1061). Složení red teamu a pokyny poskytnuté red-teamérům (‡1062), počet kol útoků (‡1063) a přístup modelu k nástrojům (‡1064, ‡1065) mohou významně ovlivnit výsledky, včetně toho, jaký rizikový povrch je pokryt. Komplexní směrnice pro red-teaming usilují o řešení některých z těchto problémů (‡1066).

###@ Zmírnění rizik

Zmírňování rizik je proces upřednostňování, vyhodnocování a zavádění kontrol a protiopatření s cílem snížit identifikovaná rizika. Příklady zahrnují přístupové kontroly (‡991), průběžné monitorování (‡986) a podmíněné závazky typu if-then (‡700). Zmírňování rizik vyvolává klíčovou otázku: jaká je akceptovatelná úroveň rizika? Nedávné rámce a firemní politiky začaly formalizovat kritéria pro „akceptaci rizika“ (‡965, ‡1040). Stanovení vhodných prahových hodnot však zůstává obtížné zejména u rizik s širokými dopady na společnost (‡986, ‡1067). V současnosti neexistuje žádný zavedený mechanismus pro ověřování rozhodnutí o akceptaci rizika učiněných vývojáři před vydáním (‡1005).

Metody zmírňování rizik popsané v Tabulka 3.3 níže jsou přizpůsobitelné a mohou zmírnit celou řadu rizik, včetně některých neočekávaných rizik. Tabulka nezahrnuje technické metody zmírňování, jako je adversarial training, obsahové filtry a monitorování chain-of-thought. To je pokryto v §3.3. Technické ochranné mechanismy a monitoring, stejně jako v celém Reportu v odstavcích „Mitigations“ pro každé riziko v §2. Risks.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zásady přijatelného používání
  Politika přijatelného použití je soubor pravidel a pokynů pro odpovědné, etické a právně správné používání modelů AI. Je běžné, že vývojáři AI zveřejňují politiky přijatelného použití, stejně jako politiky zakázaného použití, spolu s novými vydáními modelů (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Řízení přístupu/ověřování uživatelů
  Řízení přístupů zahrnuje používání zásad a pravidel k omezení přístupu k modelům AI, datům a systémům na základě rolí uživatelů, atributů a dalších podmínek, aby se zabránilo neoprávněnému použití, manipulaci nebo únikům dat. Společnosti zabývající se AI často deaktivují účty, u nichž se zjistí, že se zapojují do trestné činnosti (‡486), a zahrnují prověřování uživatelů a prověrky Know-Your-Customer k zajištění, že modely jsou používány pouze důvěryhodnými aktéry (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Specifikace chování/modelu
  Specifikace chování pro AI je dokument, který definuje, jak se model AI má chovat v různých situacích. Slouží jako šablona pro sladění AI a bezpečnost a řídí vývoj modelu, trénování, vyhodnocování a výstupy. Několik společností zabývajících se AI používá dokumenty specifikace modelu a zpřístupňuje alespoň jejich části veřejnosti (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Průběžné monitorování
  Nepřetržité monitorování je průběžný, automatizovaný proces pozorování, analýzy a řízení nasazených systémů AI, sledování jejich výkonu a omezování jejich chování tak, aby byla zajištěna spolehlivost, účinnost a bezpečnost. K dispozici je mnoho nástrojů pro nepřetržité monitorování (‡1073*) a také technik k podpoře
Pozorovatelnost umělé inteligence (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Obrana do hloubky
  Obrana do hloubky je myšlenka, že lze zavést více nezávislých a překrývajících se vrstev obrany tak, aby i když jedna selže, ostatní zůstaly účinné (‡1075, ‡1076). Více Rámců Frontier AI Safety se na ni odkazuje (např. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitorování ekosystému
  Toto je proces sledování širšího ekosystému AI, včetně sledování výpočetního výkonu a hardwaru, původu modelů, původu dat a vzorců použití. Odborná literatura zkoumá takové sledování v souvislosti s riziky obecně použitelných AI (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Podmíněné závazky
  Podmíněné závazky (if-then) jsou souborem technických a organizačních protokolů a závazků pro řízení rizik, jak se AI modely stávají schopnějšími. Několik vývojářů AI používá tyto typy závazků jako součást svých Rámců bezpečnosti Frontier AI (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Červené čáry nebo zákazy
  Červené čáry jsou konkrétní hranice vyjádřené jako schopnosti, dopad nebo typy použití. Tento koncept se objevuje ve veřejných prohlášeních a iniciativách, stejně jako v regulačních zákazech (‡1079, ‡1080, ‡1081). Odborná literatura také uvádí omezení přístupů založených na červených čarách, včetně problémů ohledně shody a vymahatelnosti.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie vydání a nasazení
  Strategie vydávání a nasazení pro obecně účelovou AI mohou zahrnovat použití postupných vydání nebo zpřístupnění přes API, aby bylo v případě zneužití nebo neočekávané škody k dispozici více možností zmírnění (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.3: Opatření ke zmírnění rizik v řízení rizik obecněúčelové umělé inteligence
>white|black||9|11|br Příkladné metody zmírňování rizik pro umělou inteligenci uvedené abecedně. Uvedené metody jsou navrženy tak, aby současně podporovaly zmírňování rizik pro mnoho různých typů rizik, včetně rizik vyplývajících z úmyslného zneužití, rizik z poruch a systémových rizik. Vzhledem k počátečnímu stavu řízení rizik pro všeobecně použitelnou umělou inteligenci ne všechny metody budou vhodné pro každého vývojáře nebo provozovatele AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Postava 3.5: Ilustrace přístupu „obrana do hloubky“ pomocí „diagramu švýcarského sýra“
>white|black||9|11|br Více vrstev obrany může kompenzovat nedostatky jednotlivých vrstev. Současné techniky řízení rizik pro AI mají nedostatky, ale jejich vrstvení může nabídnout mnohem silnější ochranu proti rizikům. Zdroj: Mezinárodní zpráva o bezpečnosti umělé inteligence 2026.


>white|orangered|left|14|15.5|bb Obranná hloubka a strategie uvolnění jsou důležité nástroje pro zmírnění dopadů

Model „defense-in-depth“ může podpořit obecné řízení rizik umělé inteligence. V tomto kontextu „defense-in-depth“ označuje kombinaci technických, organizačních a společenských opatření uplatňovaných v různých fázích vývoje a nasazení (Postava 3.5). To znamená vytvářet vrstvy nezávislých záruk, takže pokud jedna vrstva selže, jiné vrstvy mohou i nadále zabránit škodám. Často uváděným příkladem modelu defense-in-depth je řada preventivních opatření nasazovaných k prevenci infekčních onemocnění. Vakcíny, roušky a mytí rukou, mimo jiné opatření, mohou riziko infekce v kombinaci výrazně snížit, i když žádná z těchto metod není sama o sobě 100% účinná (‡1083*). Pro obecnou umělou inteligenci bude defense-in-depth zahrnovat kontroly, které nejsou přímo v samotném modelu AI, ale spíše v širším ekosystému. Patří sem (například) kontroly materiálů potřebných k provedení biologického útoku, jako jsou reagencie (‡1084, ‡1085). Opatření defense-in-depth však primárně řeší rizika související s nehodami, poruchami a škodlivým použitím a mohou mít menší roli při zvládání systémových rizik (viz §3.5. Budování společenské odolnosti).

Strategie vydání a nasazení společnosti je důležitou součástí zmírňování rizik. Rozhodnutí o tom, jak jsou modely zpřístupňovány uživatelům, mohou významně ovlivnit míru vystavení riziku (‡1082). Mezi různé možnosti vydání a nasazení patří postupné vydání omezeným skupinám uživatelů, zpřístupnění prostřednictvím řízených online služeb (například API) a použití licenčních smluv a zásad přijatelného používání, které právně zakazují určité škodlivé aplikace (‡176, ‡1086, ‡1087). §3.4. Open-weight models se podrobněji zabývá tím, jak zveřejnění vah modelu ovlivňuje rizika.

###@ Řízení rizik

Řízení rizik je proces, pomocí kterého se hodnocení řízení rizik, rozhodnutí a akce propojují se strategií a cíli organizace nebo jiného subjektu (‡1088, ‡1089). Tabulka 3.4 poskytuje přehled běžných technik řízení rizik. Jak je znázorněno na Postava 3.4, řízení rizik lze chápat jako jádro řízení rizik, protože umožňuje efektivní fungování dalších komponent řízení rizik. Zajišťuje odpovědnost, transparentnost a srozumitelnost, které podporují informovaná rozhodnutí v oblasti řízení rizik. Řízení rizik může zahrnovat postupy, jako je hlášení incidentů (‡1090), přidělování odpovědnosti za rizika (‡965) a ochranu oznamovatelů (‡1091). Širší pojetí řízení rizik může zahrnovat vedení, rámce, legislativu, regulaci, národní a mezinárodní standardy, stejně jako školení a vzdělávací iniciativy. Klíčovým účelem řízení rizik je stanovit organizační zásady a mechanismy, které objasňují, jak jsou odpovědnosti za řízení rizik rozděleny v rámci organizace nebo jiného subjektu, aby byla podpořena vhodná kontrola a odpovědnost (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentace
  Postupy dokumentace pomáhají sledovat klíčové informace o systémech AI, jako jsou trénovací data, návrhová rozhodnutí, zamýšlené použití, omezení a rizika. „Model cards“ a „system cards“, které poskytují informace o tom, jak byl model nebo systém AI trénován a vyhodnocen, jsou příklady významných osvědčených postupů v oblasti dokumentace AI (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Oznamování incidentů
  Incident reporting je proces systematického dokumentování a sdílení případů, ve kterých vývoj nebo nasazení AI způsobily přímou nebo nepřímou újmu. Existuje několik platforem, které usnadňují incident reporting pro AI (‡1096, ‡1097), a rámců, které umožňují efektivnější incident reporting AI (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rámce řízení rizik
  Rámce řízení rizik jsou organizační plány pro snížení mezer v pokrytí rizik, koordinaci různých činností v oblasti řízení rizik a zavedení kontrol a protiváh. Rámce specifické pro obecně použitou umělou inteligenci (‡986, ‡1098) často odkazují na další opatření uvedená v této části.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Seznam rizik
  Registr rizik je úložiště různých rizik, jejich prioritizace, odpovědných osob a plánů mitigace. Tyto postupy jsou poměrně běžné v mnoha odvětvích, včetně kybernetické bezpečnosti (‡1099), a někdy se používají k naplnění požadavků na regulatorní soulad.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Přidělení odpovědnosti za řízení rizik
  Přidělení rolí a odpovědností pro řízení rizik v organizaci může strukturovat interní dohled nad rozhodováním (‡1002, ‡1093). Taková uspořádání se odrážejí v některých rámcích správy a řízení, včetně Kodexu postupů pro obecné účely v oblasti umělé inteligence EU (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Transparenzní zprávy
  Transparentní zprávy popisují postupy řízení rizik společnosti zabývající se umělou inteligencí tím, že veřejně zveřejňují určité informace, nebo sdílejí dokumentaci s oborovými skupinami či vládními institucemi. Například řada společností zabývajících se umělou inteligencí předkládá transparentní zprávy Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ochrana oznamovatelů
  Protože velká část vývoje v oblasti umělé inteligence probíhá za zavřenými dveřmi, některé rámce governance zahrnují ochranu oznamovatelů, aby umožnily nahlášení potenciálních rizik orgánům (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.4: Řízení rizik v rámci obecné správy rizik pro systémy s umělou inteligencí pro všeobecné použití
>white|black||9|11|br Příkladové metody pro řízení rizik v oblasti umělé inteligence jsou uvedeny v abecedním pořadí. Zahrnuté metody jsou navrženy tak, aby současně podporovaly řízení rizik pro mnoho různých typů rizik, včetně rizik plynoucích z úmyslného zneužití, rizik plynoucích z poruch a systémových rizik. Vzhledem k nezralosti obecného řízení rizik u AI nebudou všechny metody vhodné pro každého vývojáře nebo provozovatele AI.


>white|orangered|left|14|15.5|bb Dokumentace a transparentnost jsou součásti řízení rizik

Dokumentační a institucionální mechanismy transparentnosti spolu s postupy sdílení informací usnadňují vnější kontrolu a podporují úsilí o řízení rizik spojených s obecně použitelnou umělou inteligencí (‡1101, ‡1102). Stalo se běžnou praxí zveřejňovat výsledky přednasazovacích testů v tzv. „model card“ nebo „system card“, spolu se základními informacemi o modelu nebo systému, včetně toho, jak byl vycvičen, a jaká jsou jeho potenciální omezení (‡1094, ‡1095). Někteří vývojáři také zveřejňují zprávy o transparentnosti, které zahrnují podrobnosti o svých postupech řízení rizik v širším měřítku (‡1103). Mezi další prvky dokumentace a transparentnosti patří monitorování a hlášení incidentů (‡176, ‡1083*, ‡1103) a sdílení informací, které mohou zprostředkovat třetí strany, jako je Frontier Model Forum. Některé regulační rámce, jako je nařízení EU o AI (EU AI Act) nebo Kalifornie’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), v některých případech nařizují sdílení informací o rizicích obecně použitelné umělé inteligence.

>white|orangered|left|14|15.5|bb Závazek vedení a pobídky utvářejí postupy řízení rizik

Organizační kultura, struktura vedení a pobídky ovlivňují úsilí v oblasti řízení rizik různými způsoby (‡1105). Závazek vedení a struktury pobídek jsou často relevantní k tomu, jak se zásady řízení rizik uplatňují v praxi. Někteří vývojáři mají interní rozhodovací panely, které zvažují, jak bezpečně a odpovědně navrhovat, vyvíjet a revidovat nové systémy umělé inteligence. Dozorčí a poradní výbory, svěřenectví, nebo rady pro etiku AI mohou rovněž sloužit jako mechanismy pro poskytování pokynů v oblasti řízení rizik a pro organizační dohled (‡1092*, ‡1106, ‡1107, ‡1108). Výzkumníci tvrdili, že problémy spojené s dobrovolnou samoregulací znamenají, že audity třetích stran, ověřování a standardizace by mohly pomoci posílit obecné řízení rizik pro systémy obecného účelu umělé inteligence (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organizační řízení rizik, transparentnost a rámce pro vykazování rizik

Několik nových iniciativ se zaměřuje na procesy řízení rizik, dokumentaci a transparentnost. V současné podobě funguje Kodex postupů pro obecné účely AI v EU jako dobrovolný rámec, který má vést transparentní, autorskoprávní a postupy v oblasti bezpečnosti a zabezpečení s cílem podpořit shodu s ustanoveními Aktu o umělé inteligenci EU pro systémy obecného účelu AI (‡965). Ke dni prosince 2025 podepsalo více než dvě desítky společností†. Rámec pro reportování G7 Hiroshima AI Process (HAIP) (‡1100) je první mezinárodní rámec pro dobrovolné veřejné reportování organizačních postupů řízení rizik pro pokročilé systémy AI. Nejprve nejméně 20 vývojářů zveřejnilo veřejné zprávy o transparentnosti pokrývající identifikaci rizik, metriky vyhodnocování, strategie zmírňování dopadů a procesy zabezpečení dat.

Vývojáři AI přijali dobrovolné závazky týkající se transparentnosti. V Číně byly v prosinci 2024 (‡1113) zveřejněny přísliby 17 čínských společností zabývajících se AI, koordinované Aliancí odvětví AI v Číně, a v roce 2025 byly aktualizovány (‡1114). Na květnovém summitu AI Seoul v Jižní Koreji v roce 2024 podepsalo 16 vývojářů AI z více zemí dobrovolné závazky zveřejnit Frontier AI Safety Frameworks pro své nejschopnější modely a systémy a přijmout postupy řízení rizik napříč fázemi vývoje a nasazení modelů (‡1052).

    Poznámka † -- Podepisující subjekty k prosinci 2025 zahrnují: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing a WRITER.

>white|orangered|left|14|15.5|bb Rámce Frontier AI Safety se staly významným organizačním přístupem k řízení rizik v oblasti AI

Od roku 2023 několik předních vývojářů v oblasti AI dobrovolně zveřejnilo dokumenty popisující, jak hodlají identifikovat a reagovat na závažná rizika ze svých nejpokročilejších systémů. Tyto Frontier AI Safety Frameworks popisují, jak vývojář AI plánuje vyhodnocovat, monitorovat a řídit své nejpokročilejší modely a systémy před nasazením i během něj. Tyto rámce se v mnoha ohledech shodují, ale liší se v klíčových aspektech (‡1115, ‡1116). Většina se zaměřuje na rizika spojená s hrozbami chemického, biologického, radiologického a jaderného (CBRN) charakteru, na pokročilé kybernetické schopnosti a na pokročilé autonomní chování (‡1115, ‡1117). Menšina rámců řeší i další oblasti rizik, jako je nezákonná diskriminace ve velkém měřítku a sexuální vykořisťování dětí.

Několik vývojářů v roce 2025 aktualizovalo své frameworky a doplnilo nové sekce o škodlivé manipulaci, riziku nesouladu (misalignment) a autonomní replikaci a adaptaci (‡1078, ‡1118). Zatímco mnohé frameworky popisují podobné přístupy k řízení rizik – včetně modelování hrozeb, red-teamingu a hodnocení nebezpečných schopností – liší se v tom, jak definují úrovně rizika a prahové hodnoty, jak často provádějí hodnocení, jaké jsou časové rezervy mezi hodnoceními a prahovými hodnotami a jak komplexní jsou jejich závazky k mitigaci (například zda zahrnují mazání váh modelu, nebo pouze pozastavení vývoje) (‡1115, ‡1119). Další informace naleznete v Tabulka 3.5.

>white|orangered|left|14|15.5|bb Mnoho akcí ve Frontier AI Safety Frameworks je založeno na závazcích typu if-then.

Klíčovou součástí Rámců bezpečnosti AI pro Frontier AI jsou „if-then závazky“. Jde o podmíněné protokoly, které spouštějí konkrétní reakce, když modely a systémy AI dosáhnou předem definovaných prahů schopností (‡1120). Například if-then závazek může uvádět, že pokud se zjistí, že model má schopnost smysluplně pomáhat začátečníkům při vytváření a nasazování zbraní CBRN, pak vývojář implementuje posílená bezpečnostní opatření, kontrolu nasazení a průběžné monitorování v reálném čase (‡991*).

V roce 2025 oznámilo několik vývojářů AI, že nové modely spustily předběžné výstražné hlášení, nebo že nemohli vyloučit možnost, že další vyhodnocení ukáže, že modely překročily prahové hodnoty schopností. To je vedlo k tomu, aby jako preventivní opatření použili zesílená bezpečnostní opatření (‡7, ‡33, ‡1121*). Rámce pro bezpečnost AI „Frontier“ běžně vyžadují nejprve vyhodnocení schopností před zavedením mitigace rizik, a dále analýzu zbytkového rizika nebo bezpečnostní případ, často informovaný red teamingem, po mitigaci. Podrobnosti viz Tabulka 3.5.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Rámec připravenosti 2 (‡1078*)
  Zakrytá rizika:
1. Biologické a chemické schopnosti
2. Schopnosti v oblasti kybernetické bezpečnosti
3. Schopnosti samostatného zlepšování pomocí AI
  Úrovně rizika nebo ekvivalentní a související ochranná opatření:
- Vysoké: Může zesílit stávající cesty k závažné újmě (Vyžaduje bezpečnostní kontroly a ochranná opatření)
- Kritické: Mohlo by zavést bezprecedentně nové cesty k závažnému poškození (Zastavit další vývoj, dokud nebudou splněny specifikované ochranné mechanismy a bezpečnostní řídicí standardy na úrovni Kritické)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Zásady zodpovědného škálování 2.2 (‡991*)
  Zakrytá rizika:
1. zbraně CBRN
2. Autonomní výzkum a vývoj umělé inteligence (AI R&D)
3. Kybernetické operace (v posuzování)
  Úrovně rizika nebo ekvivalentní a související ochranná opatření:
  Úrovně bezpečnosti AI (ASL)
- ASL-1: Žádné významné katastrofické riziko
- ASL-2: Rané příznaky nebezpečných schopností (Modely musí splňovat standardy nasazení a zabezpečení ASL-2)
- ASL-3: Výrazně zvýšené riziko katastrofického zneužití (Modely musí splňovat požadavky na nasazení a/nebo bezpečnost podle ASL-3)
- ASL-4+: Budoucí klasifikace (zatím nedefinované)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Rámec bezpečnosti Frontier 3.0 (‡1040*)
  Zakrytá rizika:
1. Zneužití
    a. CBRN
    b. Kybernetické
    c. Škodlivá manipulace
2. Výzkum a vývoj v oblasti strojového učení
3. Nesoulad/ instrumentální uvažování
  Úrovně rizik nebo ekvivalentní a související ochranná opatření:
  Kritické úrovně schopností
    Úrovně schopností, při kterých mohou AI modely nebo systémy bez zmírňujících opatření (bezpečnostní případy pro nasazení a bezpečnostní zmírňující opatření v souladu s úrovněmi zabezpečení RAND 2, 3 nebo 4 (‡1122)) představovat zvýšené riziko závažného ublížení. Úrovně schopností zahrnují „hodnocení včasného varování“ se specifickými „prahy výstrah“
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Rámec pro Frontier AI 1.1 (‡990*)
  Zakrytá rizika:
1. Kybernetická bezpečnost
2. Chemická a biologická rizika
  Stupně rizika nebo rovnocenné kategorie a související ochranná opatření:
  Úrovně prahových hodnot rizik
- Mírné (uvolnění s odpovídajícími bezpečnostními opatřeními a zmírněními)
- igh (neuvolňovat)
- Kritické (zastavit vývoj)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Rámec bezpečnosti pro modely Frontier (‡1123*)
  Zakrytá rizika:
1. šíření zbraní CBRN
2. Ofenzivní kybernetické operace
3. Automatizovaný výzkum a vývoj v oblasti AI
  Stupně rizika nebo ekvivalentní úrovně a související ochranná opatření:
  Prahy kritických schopností
    Schopnosti modelu, které mohou při zneužití způsobit významnou újmu veřejnosti. (Pokud jsou prahové hodnoty splněny nebo překročeny, model nebude veřejně nasazen bez odpovídajících opatření k mitigaci rizik)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Rámec řízení pro Frontier (‡1124*)
  Zakrytá rizika:
1. zbraně CBRN
2. Ofenzivní kybernetické operace
3. Pokročilá autonomie (včetně výzkumu a vývoje AI)
  Úrovně rizika nebo ekvivalentní a související ochranná opatření:
  Úrovně rizika
- Nízká nebo Střední (nasazení povoleno v souladu s požadavky programu odpovědné umělé inteligence)
- Vysoké nebo Kritické (další kontrola a zmírňující opatření)
(povinné)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Posouzení rizik AI pro Frontier (‡1029*)
  Zakrytá rizika:
1. Kybernetický útok
2. CBRN
3. Přesvědčování a manipulace
4. Nezákonná diskriminace ve velkém měřítku
  Úrovně rizik nebo rovnocenné a související ochranná opatření:
  Prahové hodnoty rizika – skóre rizika modelu (MR)
- MR1 nebo MR2 (hodnoticí výsledky dokumentují inženýrské týmy)
- MR3 (Zmírňující opatření k rizikům a výsledky hodnocení jsou zdokumentovány inženýrskými týmy a pravidelně revidovány)
- MR4 (Důkladné posouzení rizik musí být dokončeno a je vyžadován souhlas vedoucího příslušné obchodní jednotky)
- MR5 (Podrobnou analýzu rizik je třeba dokončit a schválit nezávislým výborem, např. etickou komisí pro umělou inteligenci společnosti NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Rámec modelu Secure AI Frontier Model (‡1125*)
  Zakrytá rizika:
1. Zneužití se zlým úmyslem (např. malware, sexuální vykořisťování dětí)
2. Škodlivé následky při běžném, neškodlivém použití, např. výstupy, které vedou k nezákonnému diskriminačnímu výsledku, nebo generování nezabezpečeného kódu
  Úrovně rizika nebo ekvivalentní a související ochranná opatření:
  Pravděpodobnost a závažnost újmy v kontextu
- Nízká
- Střední
- Vysoká
- Velmi vysoká
    (Odstraňující rizika a bezpečnostní kontroly jsou zavedeny pro všechny systémy a procesy; další opatření je třeba přizpůsobit systému AI a konkrétnímu případu použití, ve kterém je model nasazen)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Zásady připravenosti na AGI (‡1127*)
  Zakrytá rizika:
1. Kybernetický útok
2. Automatizovaný výzkum a vývoj v oblasti AI
3. Autonomní replikace a adaptace
4. Pomoc při biologických zbraních
  Úrovně rizik nebo ekvivalentní a související ochranná opatření:
  Prahy kritických schopností
    Kvantitativní prahové hodnoty na ukazatelích výkonnosti schopností (Pokud budou překročeny, proveďte nebezpečné posouzení schopností, opatření v oblasti informační bezpečnosti a opatření pro nasazení, nebo zastavte vývoj)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Politika připravenosti pro Magic: AGI (‡1127*)
  Zakrytá rizika:
1. Kybernetický útok
2. Automatizovaný výzkum a vývoj v oblasti AI
3. Autonomní replikace a adaptace
4. Pomoc při biologických zbraních
  Úrovně rizika nebo rovnocenné a související záruky:
  Prahy kritických schopností
    Kvantitativní prahové hodnoty na ukazatelích výkonnosti schopností (Pokud jsou překročeny, proveďte nebezpečné hodnocení schopností, opatření v oblasti informační bezpečnosti a zmírnění nasazení, nebo zastavte vývoj)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Rámec bezpečnosti AI (‡1128*)
  Zakrytá rizika:
1. Ztráta kontroly
2. Zneužití (např. biochemická zbraňová výroba
  Úrovně rizika nebo odpovídající kategorie a související ochranná opatření:
  Úrovně rizika
- Nízké riziko (Nasazujte systémy AI, ale po nasazení provádějte monitorování, abyste řídili rizika)
- Riziko identifikováno (Buď zpřístupnit systémy OpenAI pouze autorizovaným uživatelům pro zmírnění rizik, nebo odložit nasazení, dokud nebudou přijata další bezpečnostní opatření, v závislosti na konkrétním použití)
- Vysoké riziko (Nepoužívat systémy umělé inteligence)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Rámec pro bezpečnost umělé inteligence Frontier (‡1129*)
  Zakrytá rizika:
1. Biologické hrozby
2. Útočná kybernetická bezpečnost
3. Autonomní provoz a pokročilá manipulace
  Úrovně rizika nebo ekvivalentní kategorie a související ochranná opatření:
  Úrovně rizika
- Úroveň 1 (Základní ochranná opatření pro minimální rizika a potenciál pro vydání do open source)
- Úroveň 2 (monitorování v reálném čase, filtrování promptů, detekce behaviorálních anomálií, přístupové kontroly, red-teaming a adversariální simulace)
- Úroveň 3 (Pokročilé ochranné mechanismy včetně red- teaming, postupných nasazení, testování proti protivníkovi, šifrování, řízení přístupu s více stranami a architektury s nulovou důvěrou)
- Úroveň 4 (maximální bezpečnostní protokoly pro modely s vysokými nároky a maximální bezpečnostní opatření)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.5: Rámce pro bezpečnost Frontier AI
>white|black||9|11|br První sada Rámců bezpečnosti AI pro Frontier, která byla vydána podmnožinou vývojářů AI, jež podepsali Závazky bezpečnosti AI pro Frontier. Rámce pokrývají podobná rizika (s drobnými odchylkami) a používají různé úrovně rizik a různé přístupy k řízení rizik.


>white|orangered|left|14|15.5|bb Účinnost rámců Frontier AI Safety je nejistá

Frontier AI Safety Frameworks mohou za určitých podmínek a pro určitá riziková kategorie sloužit jako nástroje řízení rizik s uvěřitelnou cestou k újmě (‡1117). Zároveň několik analýz probírá otázky týkající se jejich srozumitelnosti a rozsahu (‡111, ‡986) a také odolnosti prahů pro schopnosti AI a rizika (‡1031, ‡1130). Existující frameworky obvykle se zaměřují na podmnožinu oblastí rizik. V důsledku toho některá významná rizika, jako je nezákonné sledování (‡1131, ‡1132) a intimní zobrazování bez souhlasu (‡287), dostávají menší důraz. Na rozdíl od přístupů k řízení rizik z jiných odvětví, jako je letectví nebo jaderná energetika (‡1133*), Frontier AI Safety Frameworks typicky nepoužívají explicitní kvantitativní prahy rizika (‡1134).

Externí hodnocení souladu vývojářů s jejich Rámcemi bezpečnosti pro Frontier AI zatím zůstává omezené, mimo jiné proto, že většina rámců je nová, veřejně dostupné informace jsou skrovné a neexistují standardizované externí audity. Jejich účinnost bude rovněž utvářena tím, jak dobře – a v jakém rozsahu – jsou závazky v praxi naplňovány. Samotné tyto rámce nemusí zajistit účinné řízení rizik, protože jejich praktický dopad závisí na tom, jak dobře a v jakém rozsahu jsou naplňovány. Doteď se plně neshodují s mezinárodními standardy pro řízení rizik (‡1135). Studie předchozích dobrovolných závazků zjistila nerovnoměrné plnění napříč opatřeními, což naznačuje, že dodržování dobrovolných závazků se pravděpodobně bude lišit mezi společnostmi a doménami (‡1109).

Společně se Rámce bezpečnosti Frontier AI Safety Frameworks představují nejpodrobnější formu dobrovolného řízení organizačních rizik, která se v současnosti používá, ale výrazně se liší v rozsahu, prahových hodnotách a vymahatelnosti.

###@ Regulační a vládní iniciativy

>white|orangered|left|14|15.5|bb Několik jurisdikcí zavedlo zákony s požadavky na transparentnost

Několik raných regulatorních přístupů zavádí právní požadavky zaměřené na zvýšení standardizace a transparentnosti v řízení rizik. Nařízení EU o AI (EU AI Act), které nabylo účinnosti v roce 2024, stanovuje požadavky týkající se transparentnosti, autorského práva a bezpečnosti pro modely obecného účelu AI. V roce 2025 byl zveřejněn Kodex postupů EU pro AI obecného účelu, aby podpořil dodržování těchto povinností poskytnutím pokynů k dokumentaci modelů a autorskému právu a také – pro nejpokročilejší modely – postupů řízení rizik, jako jsou hodnocení, posuzování rizik a zmírňování rizik, zabezpečení informací a oznamování závažných incidentů (‡965).

Mezi další příklady nových regulačních požadavků patří rámcový zákon Jižní Koreje o rozvoji umělé inteligence a o budování důvěry, který zavádí požadavky pro „vysoce dopadové“ systémy umělé inteligence v kritických odvětvích (‡1136), a kalifornský zákon SB 53, který stanovuje požadavky na transparentnost bezpečnostních rámců a na hlášení incidentů (‡1104). Vzhledem k tomu, jak nedávno byly tyto požadavky zavedny, je příliš brzy na to, aby bylo možné podrobně vyhodnotit, jak ovlivní postupy řízení rizik nebo skutečné rizikové dopady.

>white|orangered|left|14|15.5|bb Širší iniciativy v oblasti správy nabízejí dobrovolné pokyny

Několik regionálních i meziregionálních rámců správy nyní vymezuje společná očekávání pro řízení rizik spojených s obecně použitelnou umělou inteligencí tím, že poskytuje nezávazné pokyny pro tvůrce politik a organizace. Čínský „Rámec správy bezpečnosti AI 2.0“, zveřejněný v roce 2025, poskytuje strukturované pokyny pro kategorizaci rizik a protiopatření napříč procesem vývoje a nasazení AI (‡1137). Členské státy ASEAN zveřejnily „Rozšířenou příručku ASEAN k řízení a etice AI (generativní AI)“, která poskytuje pokyny pro správu a etiku obecně použitelné AI a má podporovat větší sladění politik napříč členskými státy ASEAN (‡1138). Kromě toho iniciativy řízené odborníky, jako je „Singapore Consensus“, vyvinuté AI vědci z více zemí, vymezují výzkumné priority pro bezpečnost obecně použitelné AI napříč posuzováním rizik, vývojem a řízením (‡690).

###@ Aktualizace

Od vydání poslední Zprávy (leden 2025) se prostředí řízení rizik pro obecně účelovou umělou inteligenci (general-purpose AI) vyvinulo; došlo k zveřejnění nových zdrojů, jako je Kodex postupů pro obecně účelovou AI (General-Purpose AI Code of Practice) Evropské unie, Rámec pro podávání zpráv HAIP skupiny G7 (G7 HAIP Reporting Framework), národní Rámec pro řízení bezpečnosti AI v Číně 2.0 (China’s national AI Safety Governance Framework 2.0) a různé Rámce pro bezpečnost AI Frontier (Frontier AI Safety Frameworks) od jednotlivých vývojářů AI. Tyto iniciativy popisují přístupy a postupy, které vývojáři AI používají k řízení rizik spojených s obecně účelovými systémy AI (‡1115). Mezi jednotlivými Rámci pro bezpečnost AI Frontier a napříč transparentními zprávami HAIP (‡1103) existují značné rozdíly, což odráží odlišnosti v organizačních postupech, prioritizaci rizik a v rané fázi ekosystému řízení rizik obecně účelové AI. Důvěryhodný ekosystém, v němž různí aktéři v oblasti AI přispívají vzájemně se doplňujícími postupy řízení rizik v celém životním cyklu, může přispět k účinnému řízení rizik (‡690).

###@ Mezery v důkazech

Chybí důkazy o tom, jak měřit závažnost, výskyt a časový rámec vznikajících rizik; do jaké míry lze tato rizika zmírňovat v reálných kontextech; a jak účinně podporovat nebo vynucovat přijetí opatření pro zmírňování napříč různými aktéry. Je potřeba více výzkumu, aby se porozumělo tomu, jak rozšířené jsou jednotlivé typy rizik a do jaké míry se liší napříč různými regiony světa, zejména pro regiony jako Asie, Afrika a Latinská Amerika, které se rychle digitalizují. Vzhledem k tomu, že jsou modelům AI udělována stále větší míra autonomie a pravomocí a že se posouvá stav vědy ohledně rizik spojených s obecněúčelovou AI, budou se muset vyvíjet i přístupy k řízení rizik (‡639, ‡1139).

Určitá opatření ke zmírnění rizik získávají na popularitě (‡690, ‡956), ale je zapotřebí dalšího výzkumu, aby se porozumělo tomu, jak robustní jsou opatření ke zmírnění rizik a ochranná opatření v praxi pro různé komunity a aktéry v oblasti AI (včetně malých a středních podniků). Pro taková hodnocení je relevantní větší dostupnost dat o reálném nasazení a používání modelů. Kromě toho se úsilí v oblasti řízení rizik v současnosti mezi předními společnostmi zabývajícími se AI výrazně liší. Bylo tvrzeno, že pobídky vývojářů nejsou dobře sladěny s důkladným posuzováním a řízením rizik (‡934). Stále existuje mezer(a) v důkazech ohledně toho, do jaké míry jsou plněny různé dobrovolné závazky, jaké překážky společnosti čelí při plném dodržování závazků a jak začleňují Frontier AI Safety Frameworks do širších postupů řízení rizik v AI.

###@ Výzvy pro tvůrce politik

Mezi klíčové výzvy patří určení, jak upřednostnit různé typy rizik, která představuje obecně použitelná AI, vyjasnění, kteří aktéři mají nejlepší předpoklady tato rizika zmírňovat, a pochopení pobídek a omezení, jež formují jejich jednání. Důkazy naznačují, že tvůrci politik v současnosti mají omezený přístup k informacím o tom, jak vývojáři a nasazovatelé AI testují, vyhodnocují a monitorují vznikající rizika, a také o účinnosti různých postupů ke zmírňování (‡1140). Výzkumníci a tvůrci politik diskutovali o úsilí v oblasti transparentnosti a systematičtějším ohlašování incidentů jako možných způsobech, jak informovat o prioritizaci rizik, podporovat důvěru a motivovat k odpovědnému vývoji (‡957). V praxi řízení rizik zahrnuje více aktérů napříč hodnotovým řetězcem AI – například poskytovatele dat a cloudu, vývojáře modelů a platformy pro hostování modelů – z nichž každý má odlišné možnosti posoudit a řídit různá rizika (‡1141). Omezené sdílení informací mezi těmito aktéry ztěžuje určit, která rizika jsou nejpravděpodobnější nebo nejvíce dopadová, zejména když se zohledňují dopady na společnost na úrovni downstreamu.

