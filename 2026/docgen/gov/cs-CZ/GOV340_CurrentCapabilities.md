###@ Aktuální možnosti

Všeobecně účelové systémy umělé inteligence vykazují mnoho pozoruhodných schopností. Vedoucí systémy nyní dosahují úrovně zlaté medaile v matematických soutěžích a pomáhají vědeckým výzkumníkům při generování hypotéz a při odstraňování problémů v laboratorní práci. V široké škále benchmarků a hodnocení zaměřených na konkrétní úkoly se vyrovnávají výkonu odborníků a v některých případech jej i překonávají.

Přesto se také profil výkonu těchto systémů jeví jako „zubatý“: jejich schopnosti se mezi různými úkoly a kontexty velmi liší. Občas stále generují nepravdivé informace („halucinace“) a produkují nekonzistentní výstupy i tehdy, když dostanou identické nebo podobné vstupy. Existuje „hodnotící mezera“: systémy AI často podávají působivý výkon v řízených podmínkách, jako jsou hodnocení před nasazením, ale v reálných podmínkách fungují podstatně hůř. Tato variabilita ztěžuje posouzení schopností všeobecné AI pomocí jedné jediné metriky. Tato část popisuje jak schopnosti systémů AI, tak i jejich nedostatky (Tabulka 1.4).

![table1.4](images/table1.4_summary_current_GAI.png)

##### Tabulka 1.4: Shrnutí hlavních schopností současných univerzálních systémů umělé inteligence

###@ Co mohou současné obecně účelové systémy AI?

Systémy obecného účelu AI nyní dosahují na standardizovaných vyhodnoceních úrovně lidských odborníků nebo ji překračují a pokrývají stále širší škálu dobře definovaných profesních a vědeckých oborů (Postava 1.4). Například přední modely dosahují skóre přes 90 % u zkoušek na úrovni vysokoškolského studia v předmětech od chemie po právo (MMLU, (‡112)) a dosahují přes 80 % u vědeckých testů na úrovni postgraduálního studia (GPQA, (‡14)). V červenci 2025 modely od Google DeepMind a OpenAI dosáhly zlaté medaile na úrovni Mezinárodní matematické olympiády a vyřešily pět z šesti úloh v podmínkách podobných soutěžním (‡76). Nad rámec uvažování založeného na textu tyto systémy vykazují i silné multimodální schopnosti: umí vytvářet fotorealistické obrazy, krátká videa ve vysokém rozlišení, 3D scény a hudební skladby z jednoduchých textových promptů (‡13, ‡18, ‡113, ‡114, ‡115, ‡116), a začínají zpracovávat komplexní údaje ze senzorů tak, aby řídily fyzické roboty (‡21*).

>white|orangered|left|14|15.5|bb Pokročilé schopnosti zvyšují produktivitu v medicíně, vzdělávání, vývoji softwaru a dalších odvětvích

Pokročilé schopnosti umělé inteligence nyní pohánějí praktické nástroje, které na konkrétních úlohách dosahují výkonu srovnatelného nebo vyššího než výkon člověka, čímž zvyšují produktivitu v několika odvětvích (‡117*).

![fig1.4](images/fig1.4_scores_GAI.png)

##### Postava 1.4: Skóre předních univerzálních systémů AI
>white|black||9|11|br Skóre předních univerzálních systémů umělé inteligence na klíčových benchmarcích od dubna 2023 do listopadu 2025. Tyto benchmarcy pokrývají náročné úlohy v programování (SWE-bench Verified), matematiku (MATH a FrontierMath) a vědecké uvažování (GPQA Diamond). Uvažovací systémy, jako například OpenAI’s o1, vykazují výrazně zlepšený výkon na matematických úlohách, což je na benchmarku MATH zřetelně znázorněno. Zdroj: Epoch AI, 2025 (‡138).


■ V medicíně mohou systémy AI analyzovat klinické situace a vést diagnostické konverzace s cílem vygenerovat seznamy možných diagnóz. V konkrétních simulovaných prostředích může jejich přesnost překročit přesnost lidských lékařů (‡118, ‡119), avšak postrádají spolehlivost a konzistenci potřebnou pro nasazení v reálné klinické praxi.
■ Ve vzdělávání jsou systémy umělé inteligence rychle zaváděny v oblastech od návrhu kurikula po hodnocení studentů, čímž se transformuje vzdělávací proces (‡120*, ‡121), zatímco široké používání studenty přináší významné výzvy pro integritu a validitu stávajících akademických hodnocení (‡122).
■ Ve vývoji softwaru se AI kódovací asistenti nyní široce používají; některé studie naznačují, že vývojáři používající AI asistenty v průměru dokončí určité úkoly o 20–30% rychleji než ti bez nich (‡123, ‡124, ‡125).
■ Studie ve velkém měřítku v jiných odvětvích, jako je zákaznický servis, poradenství a odborné psaní, nacházejí měřitelné nárůsty produktivity z práce s asistencí AI, i když se tyto účinky liší napříč úlohami a skupinami pracovníků (‡126, ‡127, ‡128, ‡129, ‡130). (Podrobnější diskusi dopadů na trh práce obecněúčelové AI viz §2.3.1. Dopady na trh práce.)

>white|orangered|left|13|15|bb Systémy obecného umělého inteligence napomáhají vědeckému výzkumu

Systémy obecného účelu AI jsou nyní využívány výzkumníky k podpoře relativně komplexních úkolů napříč obory. Výzkumníci prokázali, že AI systémy mohou při vysoké úrovni lidského vedení navrhovat nové proteiny pro lékařské použití, které jsou následně ověřeny v fyzické laboratoři (‡131). Jiné systémy objevily nové algoritmy, které jsou účinnější než dlouhodobě používané metody navržené člověkem (‡31*). Zvláště významné je, že takové pokroky často spoléhají méně na surový výkon nejnovějších modelů a více na vhodné integrování systému. Obecný účel AI je také stále častěji používán k urychlení samotného výzkumu AI, což je trend s významnými dopady, které jsou dále probírány v §1.3. Schopnosti do roku 2030. V společenských vědách výzkumníci využívají AI k urychlení analýzy dat prostřednictvím automatizovaného anotování a ke zkoumání společenských dynamik simulováním individuálního i kolektivního chování pomocí AI agentů (‡132, ‡133, ‡134). Při přechodu od analýzy k přímému použití začínají výzkumníci používat systémy obecného účelu AI k návrhu a studiu škálovatelných, nových společenských intervencí. Například nedávná práce zkoumala využití AI zprostředkovaných konverzací k nalezení společné shody v demokratických debatách nebo ke snížení víry v konspirační teorie prostřednictvím dialogu (‡135, ‡136, ‡137).

###@ Jaká jsou současná omezení systémů obecně určené umělé inteligence?

Navzdory pokrokům ve schopnostech zůstává výkon univerzálních systémů umělé inteligence napříč úlohami a kontexty nerovnoměrný. Tato část zdůrazňuje některá významná omezení, i když celá škála problémů je širší.

>white|orangered|left|13|15|bb Přetrvávající problémy s spolehlivostí přetrvávají i v současných systémech AI

Navzdory nedávným zlepšením mohou být univerzální systémy umělé inteligence nespolehlivé a náchylné k základním chybám faktů a logiky. I systémy, které vynikají v komplexních úlohách, mohou vytvářet neexistující citace, biografie nebo tvrzení  – tento jev se označuje jako ‘halucinace’ (‡139, ‡140, ‡141). Jejich výkon může být také nekonzistentní; například přesnost u matematických úloh může výrazně klesnout, když se do zadání vloží irelevantní informace (‡142). Tato křehkost se vztahuje i na multimodální schopnosti, kde modely často vykazují nízký výkon v úlohách prostorového uvažování, jako je základní počítání objektů na scéně (‡143, ‡144).

Ačkoli může odborný lidský dohled zmírnit některá z těchto rizik, existuje k tomu odpovídající nebezpečí nadměrného spoléhání, kdy uživatelé věří nesprávným výstupům, protože jsou prezentovány plynule a s přesvědčivou jistotou (‡145, ‡146) (viz §2.3.2. Rizika pro lidskou autonomii). Tato nespolehlivost ztěžuje bezpečné zavádění takových systémů v situacích s vysokými nároky na spolehlivost, jako je medicína a finance, kde mohou mít chyby vážné následky, a lidské ověřování výstupů systému zůstává nezbytné.

>white|orangered|left|13|15|bb Systémy mají potíže s dlouhodobým plánováním a neočekávanými překážkami

Všeobecně použitelným systémům AI se také nedaří úspěšně vykonávat úlohy, které vyžadují dlouhodobé plánování, udržování koherentní strategie v mnoha krocích a přizpůsobení se neočekávaným překážkám. Jak úlohy rostou na délku, AI agenti často ztrácejí přehled o svém postupu a nedokážou spolehlivě reagovat na neočekávané vstupy (‡147, ‡148, ‡149*). Například i jednoduchá vyskakovací reklama na webové stránce může vyvést celou úlohu z rovnováhy (‡150). Rozsáhlé evaluace potvrzují tento vzorec: při vývoji software nejvýkonnější systémy dosahují pouze 50% úspěšnosti u úloh trvajících jen o něco více než dvě hodiny a dosažení 80% úspěšnosti vyžaduje omezit je na mnohem jednodušší úlohy trvající 25 minut (‡98, ‡151). Zatím zůstává spolehlivé automatizování dlouhých nebo komplexních úloh neproveditelné.

>white|orangered|left|13|15|bb Interakce s fyzickým světem zůstává náročná

Pokrok v digitálních úlohách se také ukázal jako obtížné přenést do robotiky, kde složitost fyzického světa přináší nové výzvy. Nedávné pokroky jsou soustředěny na modely Vision-Language-Action (VLA) – základní modely navržené tak, aby umožnily robotům plnit instrukce v přirozeném jazyce, interpretovat multimodální senzorická data a generovat příkazy pro pohyb. Současné špičkové systémy, jako jsou π0.5 (‡152) a Gemini Robotics (‡21), nyní dokážou interpretovat jednoduché verbální příkazy typu „ukliď kuchyň“ a provést sekvenci fyzických kroků v neznámém, řízeném prostředí. Stávající modely VLA však stále nepodávají dobré výsledky u neobvyklých tvarů objektů a u neočekávaných událostí (‡152). Zajistit, aby takové systémy mohly bezpečně a spolehlivě fungovat, čímž se minimalizuje riziko fyzického ublížení nebo poškození majetku, a zároveň podávat dobré výsledky v různorodých prostředích, zůstává aktivní oblastí výzkumu (‡153, ‡154, ‡155).

>white|orangered|left|13|15|bb Výkon je v jednotlivých jazycích a kulturách nerovnoměrný

Schopnosti univerzálních modelů a systémů umělé inteligence se také liší napříč jazyky a kulturami. Výkon je nejvyšší u úloh v angličtině, což odráží skutečnost, že většina trénovacích dat pochází ze západních zdrojů (‡156, ‡157). Například jedna evaluace AI modelů napříč 83 jazyky zjistila podstatně nižší výkonnost u jazyků, které používají ne-latinské písmo, a u jazyků s omezenými digitálními zdroji (‡158). Tato nerovnost se promítá i do kulturních znalostí (‡159); v jedné studii AI modely správně odpověděly na 79% otázek o každodenní kultuře v USA, ale pouze na 12% otázek o etiopské kultuře (‡160). Další studie zjišťuje, že současné modely „uvažují“ efektivněji ve vysoce zdrojových jazycích, což může rozšířit výkonnostní propast mezi jazyky (‡161). Nad rámec jazyka a kultury se podobné vzorce objevují podél geografických a socioekonomických linií. Modely v doporučeních podreprezentují lokality s znevýhodněnými demografickými skupinami (‡162) – například, pokud se zeptají na doporučení restaurace, nemusí navrhnout restaurace v chudších oblastech – a jejich výkon v úlohách na faktické vybavování se pro země s nižšími příjmy zhoršuje (‡163, ‡164). Tato nerovnost je umocněna hodnoticími benchmarky, které jsou samy o sobě silně vychýlené směrem k angličtině, čímž vzniká ekosystém, v němž jazyky s nízkými zdroji zůstávají systematicky nedostatečně zkoumané a nedostatečně optimalizované (‡165, ‡166).

###@ Aktualizace

Od vydání poslední Zprávy (leden 2025) se „reasoning“ systémy staly mainstreamem (viz §1.1. Co je obecně účelová AI? pro podrobnosti o jejich vývoji). Tyto systémy vykazují podstatně zlepšený výkon v náročné matematice, programování a vědeckých úlohách tím, že generují a porovnávají více odpovědí v rámci vlastního „chain of thought“, než nakonec vytvoří výslednou odpověď (Postava 1.5) (‡112, ‡167). Vzhledem k tomu, že výkon těchto modelů závisí zčásti na výpočetním výkonu při inferenci, mohou se jejich efektivní schopnosti měnit po počátečním vývoji – zlepšují se, když je přiděleno více výpočetních zdrojů. Současně se však AI společnosti více zaměřily na vývoj AI agentů, zejména v oblastech, jako je softwarové inženýrství (‡168) a práce s počítačem (‡169, ‡170). Ačkoli spolehlivost zůstává úzkým hrdlem, složitost úloh, které tito agenti dokážou automatizovat, roste velmi rychle (‡98). A konečně, umožnění modelům vytvářet dlouhodobé paměti a průběžně se učit na základě interakce s uživateli se objevuje jako klíčová vývojová oblast (‡171, ‡172*).

![fig1.5](images/fig1.5_perf_GAI_models.png)

##### Postava 1.5: Výkonnost univerzálního modelu umělé inteligence
>white|black||9|11|br Výkon obecného modelu umělé inteligence (s1) na úlohách náročných na uvažování při různém množství výpočetního výkonu během testování (tj. při použití dodatečného výpočetního výkonu během inferencování). Přidělení více výpočetního času během generování odpovědi vede k výrazně lepším výsledkům v matematice (AIME 24) i v otázkách na úrovni PhD v oblasti vědy (GPQA Diamond). Zdroj: Muennighoff et al., 2025 (‡173).


###@ Mezery v důkazech

Trhavé schopnosti a hodnoticí mezera ztěžují spolehlivé měření a předvídání schopností obecně použití umělé inteligence (‡174, ‡175). Výkon navíc silně závisí na konkrétních testovacích příkladech a použité výzvě (promptu), což ztěžuje prokázat s vysokou mírou důvěry, že AI systém nemůže provádět určité – potenciálně nebezpečné – úlohy (‡176*). Neexistuje žádná jednotná, komplexní a průběžně aktualizovaná syntéza schopností AI, což vede k roztříštěnému a často zastaralému porozumění oboru. Stávající přehledy (‡138, ‡177), včetně této Zprávy, poskytují cenná shrnutí, ale představují statické snímky v rychle se vyvíjejícím oboru. Bez široce přijímané taxonomie schopností musí tvůrci politik procházet mozaikou benchmarků a zdrojů, aby vytvořili ucelený obrázek.

>white|orangered|left|13|15|bb Benchmarky často selhávají při předpovídání výkonu v reálném světě

Integrita benchmarků je stále větším problémem. Mnoho hodnocení schopností se opírá o standardizované benchmarky. Řada modelů však mohla být trénována na datech z těchto stejných benchmarků – problém označovaný jako „kontaminace dat“, který většina vývojářů v současnosti nesleduje ani nezveřejňuje (‡178). To může vést k nadhodnoceným skóre výkonnosti, jež neodrážejí skutečné schopnosti modelu (‡179), ale spíše jeho schopnost memorovat odpovědi (‡180, ‡181, ‡182). Dalším omezením současných postupů hodnocení je, že se opírají o automatizované testování v kontrolovaných laboratorních podmínkách. To však často přeceňuje praktickou užitečnost systémů AI v dynamickém prostředí reálného světa (‡147, ‡149, ‡183, ‡184). Například jedna studie zjistila, že ačkoli AI agent dokázal generovat funkční kód, před jeho použitím v reálném projektu vyžadoval kód stále značné lidské úsilí k opravě problémů v dokumentaci, formátování a kvalitě (‡185). Aby se tato omezení řešila, objevuje se specializovaná „evaluation science“, která prosazuje důsledné metodologie zajišťující externí validitu a lepší predikci výkonu v reálném světě (‡186, ‡187). Například nedávné benchmarky začaly měřit výkon systémů AI na ekonomicky cenných úlohách (‡188, ‡189) a na vzdálené práci z reálného světa (‡190, ‡191*).

>white|orangered|left|13|15|bb Důkazy o tom, jak umělá inteligence zvyšuje lidské schopnosti, jsou neprůkazné.

Důsledné měření praktických přínosů AI je obtížné, protože úspěch závisí jak na konkrétním úkolu, tak na schopnosti uživatele jej pomocí AI využít, což znamená, že výsledky z laboratoří často nedokážou předpovědět reálnou hodnotu. Například jedna studie ukazuje, že samostatná přesnost modelu není spolehlivým prediktorem výkonu lidsko-AI týmu (‡192). Mnohé studie potvrzují pozitivní nárůst při používání AI (‡126, ‡127, ‡128). Avšak jedna nedávná studie zjistila, že i když softwaroví vývojáři věřili, že je AI dělá produktivnějšími, ve skutečnosti zpomalila zkušené programátory o 19% u komplexních úloh kódování (‡129).

