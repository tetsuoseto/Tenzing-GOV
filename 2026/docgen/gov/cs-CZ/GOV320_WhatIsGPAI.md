###@ Co jsou systémy obecného účelu pro umělou inteligenci?

Obecně účelové AI systémy jsou softwarové programy, které se učí vzory z velkých množství dat, což jim umožňuje provádět různé úlohy, namísto toho, aby byly specializované na jednu konkrétní funkci nebo doménu (viz Tabulka 1.1). Pro vytvoření těchto systémů provádějí vývojáři AI vícestupňový proces, který vyžaduje značné výpočetní zdroje, rozsáhlé datové sady a specializované odborné znalosti (viz Tabulka 1.2). Výpočetní zdroje (často zkráceně „compute“) jsou potřeba jak pro vývoj, tak pro nasazení AI systémů a zahrnují specializované čipy pro počítače i software a infrastrukturu nezbytnou pro jejich provoz.† Vzhledem k tomu, že jsou trénovány na velkých a rozmanitých datových sadách, mohou obecně účelové AI systémy vykonávat mnoho různých úloh, například shrnovat text, generovat obrázky nebo psát počítačový kód. Tato část vysvětluje, jak se obecně účelové AI systémy vytvářejí, co jsou „modely“ uvažování a jak politická rozhodnutí formují vývoj obecně účelových AI systémů.

    Poznámka † -- Termín ‘compute’ může také označovat buď měření počtu výpočtů, které může procesor provést (obvykle měřeno v operacích s plovoucí řádovou čárkou za sekundu), nebo konkrétně hardware (například grafické procesory), který tyto výpočty provádí.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Jazykové systémy
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Příkaz A (‡3*)
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
###@ generátory obrázků
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Generátory videí
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Vidím 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotika a navigační systémy
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Prediktory různorodých tříd biomolekulárních struktur
- AlphaFold 3 (‡27)
- Zesílit (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI agenti
- AlphaEvolve (‡31*)
- Agent ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 1.1: Obecněúčelové typy umělé inteligence
>white|black||9|11|br Existuje několik různých typů obecně použitelných systémů umělé inteligence. V této zprávě jsou modely, které dokáží predikovat strukturální informace pro různé třídy molekul, považovány za „obecně použitelnou“ AI, protože je lze přizpůsobit celé řadě úloh. Například modely trénované k predikci struktury bílkovin jsou použitelné pro řadu dalších úloh, jako je predikce interakcí bílkovin, predikce vazebných míst pro malé molekuly a predikce a navrhování cyklických peptidů (‡40).


>white|orangered|left|13|15|bb Hluboké učení je základem pro obecně použitelnou umělou inteligenci

Výzkumníci vytvářejí obecně účelové modely umělé inteligence pomocí procesu nazývaného „deep learning“, který trénuje modely tak, aby se učily z příkladů (‡41). Na rozdíl od softwarového inženýrství se modely deep learning učí plnit úkoly z dat, místo aby se spoléhaly na ručně psané instrukce. Zpracováním velkých objemů dat, jako jsou obrázky, text nebo audio, tyto modely objevují způsoby, jak ta data reprezentovat, a vytvářejí vnitřní reprezentace vzorců (například tvarů, asociací slov nebo zvukových struktur), které modelu pomáhají rozpoznávat vztahy a generovat výstupy v souladu s jeho tréninkovým cílem. Následně používají tyto naučené vnitřní reprezentace jako abstraktní příznaky k analýze nových, podobných dat a ke generování výstupů ve stejném stylu. Například obecně účelový model AI trénovaný na dostatečném množství příkladů romantické anglické poezie z 19. století dokáže rozpoznat nové básně v tomto stylu a vytvořit nová díla v podobném stylu.

Na podrobnější úrovni funguje hluboké učení tak, že zpracovává data prostřednictvím vrstev propojených uzlů pro zpracování informací. Tyto uzly se často nazývají „neurony“, protože jsou volně inspirované neurony v biologických mozcích („neuronové sítě“) (Postava 1.1) (‡42). Jak informace proudí z jedné vrstvy neuronů do další, model postupně transformuje data do stále abstraktnějších reprezentací jakožto seskupení naučených příznaků – vzorů, které model v datech automaticky objevil, nikoli těch, které by byly ručně kódované. Například v modelu pro zpracování obrazu mohou první vrstvy učit rozpoznávat jednoduché příznaky, jako jsou hrany nebo základní tvary, zatímco hlubší vrstvy tyto příznaky kombinují tak, aby odhalily složitější vzory, jako jsou obličeje nebo objekty.

Vlastnosti na všech úrovních jsou odhaleny optimalizačním procesem, který definuje trénovací postup. Při trénování, když se model dopouští chyb, algoritmy hlubokého učení upravují sílu různých spojení mezi neurony tak, aby zlepšily výkon modelu. Síla každého spojení mezi uzly se často nazývá „váha“. Tato vrstvená koncepce dala hlubokému učení jeho název.

Hluboké učení se ukázalo jako velmi účinné při umožnění AI systémům plnit úkoly, které byly dříve považovány za obtížné pro tradiční ručně programované výpočetní systémy a další dřívější symbolické nebo pravidlové metody AI. Většina současných špičkových univerzálních AI modelů je dnes založena na specifické architektuře neuronových sítí známé jako „transformer“ (‡43, ‡44). Transformery používají mechanismus „pozornosti“ (‡45), který pomáhá modelu zaměřit se při zpracování informací na nejrelevantnější části vstupních dat, například na to, která slova ve větě jsou nejdůležitější pro pochopení jejího významu. Tento konkrétní způsob budování modelů vedl k významným zlepšením v překladu (‡43), zpracování přirozeného jazyka (‡46), rozpoznávání obrazu (‡47) a rozpoznávání řeči (‡48, ‡49), což nakonec vedlo k vývoji dnešních nejpokročilejších modelů.

![fig1.1](images/fig1.1_neural_network.png)

##### Postava 1.1: Ilustrační znázornění „neuronové sítě“
>white|black||9|11|br Dnešní všeobecně použitelná AI modely jsou založeny na těchto sítích, které jsou volně inspirovány biologickými mozcích. Různé sítě mají různé velikosti a architektury. Všechny jsou však složené z propojených jednotek pro zpracování informací nazývaných „neurony“, kde se síle propojení mezi neurony říká „váhy“. Váhy se při trénování aktualizují na základě velkého množství dat. Zdroj: International AI Safety Report 2025 (‡50) (upraveno).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Postava 1.2: Schématické znázornění fází vývoje obecněúčelové umělé inteligence
>white|black|left|9|11|br Mezinárodní zpráva o bezpečnosti umělé inteligence 2026.


>white|orangered|left|13|15|bb Všeobecná umělá inteligence se vyvíjí po etapách

Vývoj obecně použitelným systémem umělé inteligence zahrnuje více fází, od počátečního trénování modelu až po monitorování a aktualizace po nasazení (Postava 1.2). V praxi se tyto kroky často překrývají iterativním způsobem. Každá fáze vyžaduje různé vstupy zdrojů (např. data, práce, výpočetní výkon) a různé techniky a někdy je provádějí různí vývojáři (Postava 1.2 a Tabulka 1.2).

Například předtrénink modelu obecně vyžaduje velké množství výpočetních prostředků a dat, takže tato fáze je obzvlášť citlivá na politiky, které ovlivňují přístup k výpočetním zdrojům nebo trénovacím datům (‡51, ‡52). Podobně příprava dat (data curation) a některé metody jemného doladění modelu v současnosti zahrnují velké množství lidské práce pro počáteční označování dat (‡53). Tato fáze je proto citlivá na změny v nákladech na pracovní sílu, politikách platforem nebo předpisech ovlivňujících přeshraniční smluvní uspořádání.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Sběr dat a jejich kuratování
> 
  Před trénováním univerzálního modelu AI vývojáři a pracovníci s daty shromažďují, čistí, vybírají a standardizují surová trénovací data do podoby, z níž se model může učit. Jde o proces, který může být náročný na práci. Trénovací datové sady, které stojí za špičkovými modely, zahrnují obrovské množství příkladů z celé sítě internet.
  Týmy často vyvíjejí sofistikované metody filtrování, aby omezily škodlivý obsah, odstranily duplicitní data a zlepšily zastoupení napříč různými tématy a zdroji (‡54, ‡55). Kurátorství dat může také pomoci snížit porušování autorských práv a soukromí, odstranit příklady obsahující nebezpečné znalosti, zpracovat více jazyků a zlepšit dokumentaci pro datovou provenienci (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Předtrénování (první fáze trénování)

  Během předtréninku vývojáři vkládají modelům obrovské množství rozmanitých dat, aby vštípili široký základ informací a kontextové porozumění. Tento proces vytváří „základní model“. Jde o vysoce datově a výpočetně náročný proces.

  Během předtrénování jsou modely vystaveny miliardám nebo bilionům příkladů obsahu, jako jsou obrázky, texty nebo audio. Prostřednictvím této expozice model postupně objevuje abstraktní příznaky pro reprezentaci dat a učí se, jak jsou tyto příznaky vzájemně propojené, což mu umožňuje dávat smysl novým vstupům v jejich kontextu. Tento proces předtrénování trvá týdny nebo měsíce (‡59) a využívá desítky nebo stovky tisíc grafických procesorů (GPU) nebo jednotek pro zpracování tenzorů (TPU) (‡60) – specializované počítačové čipy navržené pro rychlé provádění mnoha takových výpočtů. Někteří vývojáři provádějí předtrénování na vlastním výpočetním výkonu, zatímco jiní využívají prostředky poskytované specializovanými poskytovateli výpočetních služeb.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Post-training a fine-tuning (druhá etapa tréninku)

  „Post-training“ dále zpřesňuje základní model tak, aby jej bylo možné optimalizovat pro konkrétní aplikaci. Jde o proces se středně náročnými výpočetními požadavky a současně s vysokou náročností na lidskou práci. Posun směrem k využívání „syntetických dat“ – uměle vygenerovaných informací, které napodobují data z reálného prostředí, ale jsou vytvářeny pomocí algoritmů nebo simulací – pomáhá učinit tuto fázi méně náročnou na lidskou práci.
  Post-trénování zahrnuje různé techniky jemného doladění a další úpravy. „Řízené jemné doladění“ zahrnuje další trénování již natrénovaného modelu na konkrétních datových sadách za účelem zlepšení výkonu modelu v dané doméně (‡61, ‡62). Například model obecného účelu může být dále trénován na rozsáhlém korpusu radiologických snímků. „Reinforcement learning“ (RL) zahrnuje zlepšování výkonu modelu tím, že model „odměňujeme“ (poskytujeme pozitivní zpětnou vazbu) za žádoucí výstupy a „trestáme“ model (poskytujeme negativní zpětnou vazbu) za nežádoucí výstupy. Má dvě výrazné podkategorie. „Reinforcement learning od human feedback“ zahrnuje odměňování výstupů, které odpovídají lidským preferencím, a trestání těch, které neodpovídají, na základě lidské zpětné vazby (‡63, ‡64*). „Reinforcement learning with verifiable rewards“ (RLVR) se používá pro zlepšování výkonu modelu na úlohách, které vyžadují věcnou správnost, jako je matematika nebo generování kódu. Vývojáři obvykle střídají aplikaci post-trénovacích technik a spouštění testů, dokud výsledky neukážou, že model splňuje požadované specifikace.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integrace systému

  Vývojáři kombinují jeden nebo více univerzálních modelů AI s dalšími komponentami a vytvářejí „systém AI“, který je připraven k použití. GPT-5 (například) je univerzální model AI, který zpracovává text, obrázky a audio, zatímco ChatGPT je univerzální systém AI, jenž kombinuje několik modelů různých velikostí a schopností s rozhraním pro chat, zpracováním obsahu, přístupem k Webu a integrací aplikací tak, aby vznikl funkční produkt.
  Kromě zprovoznění modelů AI se i další komponenty v systému AI snaží zlepšit schopnosti, užitečnost a bezpečnost. Například systém může obsahovat filtr, který detekuje a blokuje vstupy nebo výstupy modelu, jež obsahují škodlivý obsah (‡65*). Vývojáři také stále častěji používají „scaffolding“ – dodatečný software postavený kolem obecně účelových modelů AI, který jim umožňuje plánovat dopředu, sledovat cíle a interagovat se světem (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Nasazení a vydání
  Nasazení je proces, při kterém se integrovaný AI systém zpřístupní pro zamýšlené použití. Vývojáři a nasazující pracovníci začleňují AI systémy do reálných aplikací, produktů nebo služeb. Vývojáři mohou nasazovat AI systémy interně (pro vlastní potřebu) nebo externě (pro soukromé zákazníky či veřejné použití). Při externím nasazování AI systémů často společnosti poskytují uživatelům přístup prostřednictvím online uživatelských rozhraní nebo aplikačních programovacích rozhraní (API), která uživatelům umožňují k systému přistupovat a spouštět jej. Například jedna společnost může navrhnout na míru přizpůsobeného chatbotu pro zákaznickou podporu, který je poháněn obecně použitelným AI systémem jiné společnosti.
  „Nasazení systému AI“ se vztahuje k tomu, že se model zpřístupní pro reálné použití pomocí integrovaných nástrojů a rozhraní, zatímco „uvolnění modelu“ zahrnuje zpřístupnění základního modelu ostatním – buď jako open-weight (stahovatelné parametry), nebo jako closed-weight (pouze přístup přes API). Viz §3.4. Modely typu open-weight.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Monitoring po nasazení a aktualizace

  Vývojáři často shromažďují a analyzují uživatelskou zpětnou vazbu, sledují dopad a výkonnostní metriky a provádějí iterativní zlepšování tak, aby řešili problémy zjištěné při reálném používání (‡67). Zlepšení se provádějí aktualizací systémových integrací, často prostřednictvím průběžného jemného ladění a poskytováním modelů přístupu k externím databázím (nedávných) faktů. Tím se velké AI modely udržují aktuální bez opakování celého procesu předběžného tréninku (‡68*). To umožňuje, aby se schopnosti hromadily napříč postupnými tréninkovými koly při zachování stability a snížení výpočetních nákladů.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 1.2: Vývojové fáze obecně použitelných AI
>white|black||9|11|br V každé vývojové fázi obecně použitelné umělé inteligence je model AI zdokonalován pro navazující použití a nakonec nasazen jako plně integrovaný systém AI, který je monitorován a aktualizován.


>white|orangered|left|13|15|bb Systémy uvažování generují během inferenčních kroků „řetězce uvažování“, aby zlepšily výkon

Inferování probíhá v okamžiku, kdy někdo použije model AI po jeho natrénování. Například k inferování dochází, když osoba požádá systém AI, aby naplánoval cestu, a model, který za tím stojí, čerpá z relevantních aspektů toho, co se naučil ohledně geografie, dopravy a kuchyně, aby vygeneroval itinerář.

V uplynulém desetiletí pokroky v schopnostech AI z velké části vycházely z větších trénovacích běhů; tedy ze zvyšování množství výpočetního výkonu použitého k trénování modelu AI. V poslední době však výzkumníci dosáhli větších zisků tím, že umožnili modelům zpracovávat informace po delší dobu a že je trénovali tak, aby při plnění úkolu produkovaly explicitní kroky uvažování (‡69*, ‡70). Systémy AI, které fungují tímto způsobem, se nazývají „uvažovací systémy“, a průběžná vysvětlení, kterými procházejí při řešení problému nebo zodpovídání otázky, se nazývají „řetězce myšlenek“. Uvažovací systémy vyžadují v době použití více výpočetních zdrojů, aby mohly vygenerovat tyto sofistikované řetězce myšlenek (‡71, ‡72, ‡73, ‡74), a také více zdrojů během trénování, aby se naučily uvažovat lépe. V praxi tyto uvažovací schopnosti umožňují systémům AI řešit komplexnější problémy iterativním rozkládáním úkolu na menší kroky. Tabulka 1.3 ukazuje příklad neuvažovacího systému a uvažovacího systému řešícího stejný problém.

Systémy uvažování dosáhly významných průlomů ve schopnostech při řešení náročných problémů. Například v roce 2025 systémy uvažování specializované na řešení matematických úloh, jako je Deep Think od Google (Gemini Deep Think) a dosud neuvolněný experimentální model od OpenAI, vyřešily úlohy Mezinárodní matematické olympiády (v uspořádaném testovacím prostředí) na úrovni rovnocenné lidskému výkonu se zlatou medailí (‡75, ‡76). Systémy uvažování prokázaly značný pokrok v formálních oblastech, jako je matematika, logické hádanky a strukturované vědecké otázky, kde lze postupné uvažování explicitně ověřit (‡77). Nicméně systémy uvažování mohou také selhat tím, že produkují irelevantní, neproduktivní nebo opakující se řetězce myšlenek (‡78, ‡79).

###@ Aktualizace tréninkových metod

Od vydání poslední Zprávy (leden 2025) výrazně zvýšila účinnost některých modelů metoda tréninku zvaná „distilace“. Distilace spočívá v tom, že se trénuje model „student“ na výstupech výkonnějšího (a obvykle většího) modelu „učitel“, což umožňuje, aby se model student přímo učil napodobovat výstupy učitele (‡80). Například DeepSeek vyvinul velký model s názvem DeepSeek-R1, který vyniká v úvahách založených na řetězení kroků (chain-of-thought reasoning). R1 vygeneroval úvahové výstupy, které následně sloužily k dolaďování menších studentských modelů, včetně DeepSeek-V3. DeepSeek-V3 si zachovává značnou část R1 matematiky, schopností v oblasti kódování a analýzy dokumentů a bylo údajně dolaďováno přibližně za $10,000 USD (přičemž náklady na předtrénink nebyly zveřejněny) (‡81). To je pravděpodobně o několik řádů nižší než náklady na dolaďování obdobně schopných, větších modelů.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabulka 1.3: Příklad systému bez uvažování (vlevo) vs. systému s uvažováním (vpravo)
>white|black||9|11|br Řešením stejné hádanky jsou tato příkladná sdělení upravena z reálných odpovědí AI. Odůvodňovací systém tráví více času a výpočetního výkonu „myšlením“ tím, že před poskytnutím své konečné odpovědi konstruuje „řetězec úvah“.

![figure.3](images/fig1.3_AI_agent.png)

##### Postava 1.3: Ilustrační znázornění AI agenta
>white|black||9|11|br Model umělé inteligence (uprostřed), který byl nakonfigurován tak, aby iterativně plánoval, uvažoval a používal nástroje k plnění úloh v reálném světě. Zdroj: Mezinárodní zpráva o bezpečnosti umělé inteligence 2026.


Distilace tedy může být levný a účinný způsob, jak mohou modely získat silnější schopnosti (‡82). Někteří výzkumníci použili distilaci k jemnému doladění vysoce schopných modelů pomocí pouhých 1,000 příkladů vygenerovaných modely na úrovni špičkových technologií (‡83). Protože distilace vyžaduje předem existující učitelský model, nelze ji přímo použít k posunu možností modelů na úrovni špičkových technologií. Může však urychlit šíření pokročilých schopností umělé inteligence, i když pocházejí z uzavřeně poskytovaných (closed-source) modelů (‡84*).

Společně s technologickým pokrokem v oblasti „distribuovaného výpočetního výkonu“ a decentralizovaného trénování (přístupy, při nichž vývojáři využívají více procesorů, serverů nebo datových center, které spolupracují na provádění trénování nebo inferenování AI (‡85, ‡86, ‡87)) se snížila míra, do jaké mnoho projektů vývoje AI spoléhá na rozsáhlou, centralizovanou výpočetní infrastrukturu. To stále častěji umožňuje i méně dobře vybaveným aktérům vyvíjet a nasazovat výkonné systémy.

###@ Aktualizace týkající se AI agentů

Od poslední Zprávy (leden 2025) pokroky v tom, jak vývojáři kombinují modely AI s nástroji, umožnily vývoj stále výkonnějších AI agentů. AI agenti jsou navrženi k naplňování cílů, které často uživatelé zadávají v přirozeném jazyce. K dosažení těchto cílů mají přístup k nástrojům, jako je paměť, rozhraní počítače a webové prohlížeče. Tyto nástroje a kód používaný k jejich propojení s modelem se označují jako „scaffolding“ a pomáhají AI agentům autonomně interagovat se světem, vytvářet plány, pamatovat si důležité detaily a sledovat cíle (‡88*, ‡89) s mnohem menším dohledem nebo asistencí lidí. Například Manus AI je populární AI agent, který dokáže automatizovat různé úlohy, včetně webového vyhledávání, vývoje softwaru a online nákupů (‡90). Postava 1.3 znázorňuje jednoduchý příklad AI agenta složeného z obecněúčelového AI modelu „brain“, který může iterativně plánovat, uvažovat a používat nástroje pro paměť, webové prohlížení a používání počítače.

Digitální infrastruktura pro AI agenty se rozšiřuje (‡91) a stále častěji se vyskytuje napříč odvětvími (‡92, ‡93, ‡94). AI agenti byli vyvinuti pro úkoly, jako je výzkum (‡37), softwarové inženýrství (‡95), řízení robotů (‡96) a zákaznický servis (‡97). Průběžný výzkum a vývoj vedly k tomu, že AI agenti nebo systémy multiagentů jsou stále schopnější a stále autonomnější. Výzkumníci odhadli, že složitost softwarových benchmarkových úloh, které AI agenti dokážou splnit, se přibližně každých sedm měsíců zdvojnásobí (viz také §1.2. Aktuální schopnosti) (‡98). Odborníci tvrdí, že stále schopnější AI agenti povedou k velkým příležitostem i rizikům (‡99, ‡100*) (viz §2.2.1. Problémy spolehlivosti).

###@ Mezery v důkazech

Hlavní mezery v důkazech kolem procesu vývoje obecně účelových systémů umělé inteligence vyplývají z nedostatku veřejně dostupných informací o tom, jak jsou vyvíjeny. Někteří vývojáři jsou vysoce transparentní ohledně toho, jak vyvíjejí obecně účelové systémy umělé inteligence (‡1, ‡101). Obecně však existuje omezený stupeň veřejné a znalosti ze strany tvůrců politik o tom, jak jsou většina pokročilých modelů vyvíjena, chráněna, vyhodnocována a nasazována. To platí zejména pro interně nasazované systémy umělé inteligence, které se používají v rámci společností zabývajících se AI, ale nejsou využívány ani chápány externími zainteresovanými stranami (‡102, ‡103). Toto omezené externí zviditelnění vytváří problémy pro transparentnost a dohled. Různí výzkumníci poukázali na omezenou a nejednotnou transparentnost týkající se trénovacích dat (‡104, ‡105, ‡106), obecně účelových modelů AI (‡107, ‡108), AI agentů (‡92), vyhodnocování (‡109), vývojových pipeline (‡110) a bezpečnosti (‡111). Omezení externího zveřejňování jsou někdy nezbytná k ochraně obchodního tajemství společností a duševního vlastnictví. Současně nízká transparentnost ztěžuje nezávislým výzkumníkům a tvůrcům politik studovat obecně účelové modely a systémy AI.


