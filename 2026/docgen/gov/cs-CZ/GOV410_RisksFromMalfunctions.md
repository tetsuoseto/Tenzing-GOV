Všeobecně použitelnými systémy AI se nedaří vyhnout způsobům selhání, které již způsobily reálnou škodu, od zfalšovaných právních citací po chybné lékařské diagnózy. I když i lidští odborníci dělají chyby, selhání AI vyvolávají odlišné obavy kvůli své novosti, potenciálnímu měřítku, obtížnosti předvídat, kdy k nim dojde, a tendenci uživatelů nekriticky důvěřovat výstupům, které zní sebejistě. Současná selhání všeobecně použitelných systémů AI zahrnují poskytování nepravdivých informací (‡602, ‡603), dělání základních chyb v uvažování (‡604, ‡605) a zhoršování výkonu při nasazení v nových kontextech (‡606, ‡607, ‡608). Zdokumentované škody z takových selhání zahrnují chybné lékařské diagnózy, omyly v právních podáních a finanční ztráty (‡609, ‡610, ‡611). Obzvláště kritické jsou výzvy spojené se spolehlivostí pro AI agenty, protože selhání může přímo způsobit škodu bez lidské akce nebo dohledu (‡612, ‡613, ‡614, ‡615). Víceagentní systémy zavádějí další režimy selhání prostřednictvím neschopnosti koordinace, konfliktů nebo nežádoucího vzájemného spiknutí mezi agenty (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halucinace
- Citování neexistujícího precedentu v právních podáních (‡617)
- Citování neexistujících zásad sníženého jízdného pro pozůstalé cestující (‡618)
- Poskytování nepřesných a zaujatých lékařských informací (‡619)
- Poskytování zastaralých informací o událostech (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Základní selhání uvažování
- Selhání při provádění matematických výpočtů (‡621)
- Selhání při odvozování základních kauzálních souvislostí (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Selhání mimo distribuci (selhání na neznámých nebo neobvyklých vstupech)
- Nesprávné klasifikování obrázků při změnách osvětlení pozadí nebo kontextu (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chyba použití nástroje
- Porušení soukromí tím, že je uživatelův soukromý obrázek vystaven pomocí agenta umělé inteligence, který jej odešle do nástroje třetí strany (‡624)
- Selhání krátkodobé pracovní paměti (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Selhání multi-agentního systému: nesouhra a konflikt
- Nedaří se spravovat sdílené zdroje kvůli konfliktu mezi individuálními pobídkami a cíli kolektivního blaha (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 2.4: Příklady problémů spolehlivosti v systémech obecného účelu umělé inteligence a agentních systémech
>white|black||9|11|br Dokumentované problémy se spolehlivostí u systémů obecné umělé inteligence, AI agentů a systémů s více agenty.


###@ Systémy obecného účelu umělé inteligence čelí celé řadě problémů s spolehlivostí

Tabulka 2.4. shrnuje běžné kategorie problémů spolehlivosti. První tři se vztahují na všechny systémy AI, zatímco poslední dvě se týkají konkrétně AI agentů a systémů s více agenty. Mnoho rizik spolehlivosti vyplývá z obtížnosti předvídat a monitorovat chování systému AI.

Tyto výzvy (podrobněji probírané v §3.1. Technické a institucionální výzvy) jsou zvláště naléhavé pro AI agenty, kteří působí v komplexních prostředích. Současné techniky pro vyhodnocování a zmírňování těchto selhání mohou snížit míru selhání, ale i přední AI agenty jsou stále natolik nespolehlivé, aby představovaly rizika a brzdily nasazení v mnoha kontextech.

„Spolehlivost“ označuje míru, do jaké AI systém funguje tak, jak bylo zamýšleno vývojářem nebo uživatelem. Všeobecné AI systémy zažívají celou řadu problémů se spolehlivostí, od nepřesného nebo zavádějícího generování obsahu až po selhání při provádění základního uvažování. Například zatímco modely se zlepšily v vybavování faktických informací, a dokonce i přední modely nadále poskytují sebejisté, ale nesprávné odpovědi v podstatném podílu případů (Postava 2.10). Ve softwarovém inženýrství může všeobecná AI nyní poskytnout značnou pomoc při psaní, vyhodnocování a ladění počítačového kódu (‡215*, ‡628, ‡629). Kód generovaný pomocí AI však často obsahuje chyby (‡630), zatímco kódovací agenti pravidelně dělají chyby (‡631). Taková selhání mohou zavádět zranitelnosti do programů a bezpečnostních systémů (viz §2.1.3. Kyberútoky).

Problémy s spolehlivostí je obzvlášť důležité sledovat v prostředích s vysokými nároky na bezpečnost, jako je medicína, kvůli zrychlujícímu se používání AI a možnosti, že selhání povede k vážné újmě (‡609, ‡619). Příslušné schopnosti se zlepšily rychle; vedoucí modely nyní dokážou projít lékařskými zkouškami (‡633*, ‡634). V praxi však vycházejí najevo omezení, která benchmarky přehlížejí. Například v jedné studii poskytovaly modely potenciálně škodlivé odpovědi na 19% lékařských otázek (‡635). Taková selhání mohou vést k nesprávné diagnóze, nevhodné léčbě nebo nesprávnému odepření péče (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Postava 2.10: Výsledky hlavních modelů na ověřeném benchmarku SimpleQA
>white|black||9|11|br Výsledky hlavních modelů na ověřovacím benchmarku SimpleQA podle data vydání modelu. Tento benchmark měří factualitu modelu, tedy schopnost modelu spolehlivě vybavovat fakta. Má krátký formát otázek a odpovědí (QA), navržený k odhalování problémů se spolehlivostí, jako jsou halucinace. Zdroj: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb AI agenti představují nové riziko spolehlivosti kvůli své autonomii

Protože AI agenti přímo jednají ve skutečném světě, jejich selhání mohou mít potenciál způsobit větší škody než selhání v neagentních systémech (‡99). Na rozdíl od AI systémů, které pouze generují text nebo obrázky pro kontrolu lidmi, mohou AI agenti samostatně provádět akce, které ovlivňují svět (‡99, ‡615, ‡636, ‡637) (viz také §1.1. Co je obecněúčelová AI?). AI agenti mohou zahajovat akce, ovlivňovat další lidi nebo AI systémy a dynamicky utvářet budoucí výsledky. Tato rozšířená oblast vlivu přináší nová rizika a zvyšuje důležitost spolehlivosti, protože selhání by mohlo přímo způsobit škodu bez možnosti zásahu člověka (‡99, ‡612, ‡638, ‡639, ‡640). To může být obzvlášť důležité pro agenty nasazované v strategických nebo bezpečnostně- kritických prostředích, jako jsou finanční služby (‡641), řízení energetiky (‡642) nebo vědecký výzkum (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Víceagentové systémy AI zavádějí nové druhy selhání spolehlivosti

Víceagentové systémy umělé inteligence zavádějí nové druhy selhání spolehlivosti v důsledku selhání koordinace nebo konfliktu mezi agenty. V multiagentových systémech AI agenti spolu navzájem interagují při snaze o sdílené nebo individuální cíle (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Například v multiagentovém systému navrženém k provedení přehledu výzkumné literatury hlavní agent rozloží dotaz uživatele a přidělí dílčí úkoly specializovaným subagentům, z nichž každý je zodpovědný za zkoumání jiného aspektu paralelně (‡650*). I když to umožňuje zvýšení efektivity, zároveň to znamená, že chyby se mohou mezi agenty šířit (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Pokud jsou více agentů vytvořeno na stejném základním modelu nebo zahrnují stejné nástroje, mohou také vykazovat korelovaná selhání (‡656). Empirické důkazy pro taková selhání v nasazených systémech zůstávají omezené, ale tyto rizika mohou růst, jak budou multiagentové systémy stále běžnější.

###@ Aktualizace

Od zveřejnění poslední Zprávy (leden 2025) výrazně vzrostl komerční i výzkumný zájem o AI agenty. Je nasazováno více AI agentů v reálném světě (Postava 2.11), přičemž většina z nich se specializuje na aplikace využívající práci s počítačem nebo na softwarové inženýrství (‡92). Nedávné publikace jako hacking agent XBOW (‡467), Claude-4 (‡659) a ChatGPT Agent (‡660) demonstrují počínající autonomní schopnosti, jako je vytváření prezentací ve formě slidů na základě vyhledávání na Webu (‡660). Zatím však ještě nedokážou provádět složitější úkoly, jako je plánování a rezervace cest (‡100), protože chybovost u delších úkolů roste (‡98, ‡148). Současný výzkum zahrnuje snahy o vývoj standardů pro to, jak agenti komunikují s externími nástroji a dalšími agenty (‡661, ‡662). Příklady zahrnují protokoly Agent2Agent (‡663) a Agent Payments (‡664) od Googlu a Model Context Protocol (‡665) od Anthropic.

>oldlace|black||11|15|br      
####@ Poznámka 2.4: Záměrné útoky mohou také způsobit selhání systémů AI
>oldlace|black|left|13|15|hb  Poznámka 2.4: Záměrné útoky mohou také způsobit selhání systémů umělé inteligence
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Tato sekce se zaměřuje na nezamýšlené selhání spolehlivosti, ale škodliví aktéři mohou selhání také záměrně vyvolávat prostřednictvím útoků, jako jsou prompt injection (vkládání promptů). Při útoku typu prompt injection jsou škodlivé instrukce předkládány agentovi nepřímo prostřednictvím kanálů, jako jsou skryté instrukce v webových stránkách nebo databázích (‡507, ‡657, ‡658). Tyto instrukce mohou „únosit“ agenta, což způsobí, že bude jednat proti záměrům uživatele. Takové útoky se obzvláště obtížně brání, protože jsou doručovány pomocí externího obsahu mimo kontrolu uživatele nebo vývojáře. Cíle útoků, kterými jsou systémy AI, se probírají dále v §2.1.3. Kyberútoky, a technické obrany jsou pokryty v §3.3. Technická opatření a monitorování.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Postava 2.11: Počet AI agentů vzrostl od roku 2023
>white|black||9|11|br Výsledky prosincového průzkumu z roku 2024 zaměřeného na 67 nasazených AI agentů. Vlevo: Časová osa hlavních vydání AI agentů. Vpravo: Oblasti aplikací, ve kterých jsou AI agenti používány. Šest oblastí je definováno na základě nejčastějších kategorií využití identifikovaných v průzkumu. Zdroj: Casper et al., 2025 (‡92).


###@ Mezery v důkazech

Hlavní mezery v důkazech vyplývají z obtížnosti spolehlivě vyhodnocovat schopnosti, omezení a režimy selhání systémů AI (viz §3.1. Technické a institucionální výzvy). Systematická hodnocení spolehlivosti AI agentů jsou omezená a postrádají standardizaci (‡92, ‡666). Některé problémy, jako je spoléhání na zastaralé informace (‡620), se mohou projevit pouze při reálném používání, takže hodnocení před nasazením mohou být nedostatečná. Předchozí práce zkoumaly spolehlivost agentů a multi-agentních systémů v konvenčním softwaru a v dřívějších formách AI (‡647, ‡667, ‡668). Nicméně použitelnost této práce pro moderní AI agenty, které často vycházejí z velkých jazykových modelů, je nejasná (‡669). Někteří výzkumníci vznesli obavy ohledně nových chování, která mohou agenti vykazovat ve svých interakcích mezi sebou, například koluzi nebo korelovaných selháních (‡614), ale empirické důkazy zůstávají omezené. Snaha o řešení těchto mezer zahrnuje nové evaluace rizik „agent-hijacking“ od National Institute of Standards and Technology (NIST) (‡670), ukazatele AI schopností OECD (‡243) a Inspect Sandboxing Toolkit britského UK AI Security Institute (‡671).

###@ Mitigace

Techniky pro zlepšování spolehlivosti AI cílí jak na samotný model, tak na širší systém, v němž je nasazen. Tyto postupy mohou snížit míru selhání, ale žádná z nich zatím nedokáže zajistit vysokou spolehlivost požadovanou v kritických oblastech (‡672). Důležitým technickým opatřením je adversariální trénink, který vystavuje modely během tréninku náročným vstupům, aby si osvojily vhodnější a robustnější odpovědi (‡673, ‡674, ‡675, ‡676, ‡677) (viz §3.3. Technické ochrany a monitoring). Pro snížení halucinací mohou vývojáři použít generování s rozšířením o vyhledávání (RAG), které doplňuje odpovědi modelu o informace získané z externí databáze, čímž pomáhá zajistit, že výstupy jsou přesné a aktuální (‡678, ‡679, ‡680), nebo specificky dolaďovat modely tak, aby byly více faktické (‡681) či uvažovaly efektivněji (‡682). Metody založené na prostředí nebo nástrojích mohou rovněž pomoci vývojářům monitorovat systémy AI (‡683). Například nasazující subjekty mohou nejprve pilotovat systémy AI v omezených izolovaných sandbox prostředích, aby analyzovaly možné režimy selhání ještě před jejich širším nasazením.

Pro výzkumníky se u AI agentů konkrétně navrhuje zvyšovat spolehlivost prostřednictvím lepší transparentnosti, dohledu a monitorování. Například monitorování interakcí agentů s externími nástroji a s jinými agenty by umožnilo účinnější dohled nad činnostmi agentů (‡684, ‡685) a analýzu incidentů (‡686). Metody automatického shromažďování těchto informací, včetně prostředí s více agenty, zůstávají aktivní oblastí výzkumu (‡653, ‡654).

###@ Výzvy pro tvůrce politik

Mezi klíčové výzvy pro tvůrce politik patří zvažování přínosů nasazení AI agentů oproti rizikům selhání spolehlivosti a zajištění, aby vývojáři, provozovatelé a uživatelé měli přístup k přesným informacím o výkonnosti agentů a jejich rizikových profilech. Rozhodnutí o tom, jak přisoudit odpovědnost za újmy způsobené AI agenty, představuje další výzvu (‡639), zejména v prostředích s více agenty, kde může být obtížné určit, kdy a jak k selháním došlo (‡687). Tyto výzvy se dále zhoršují obtížností vyhodnocovat spolehlivost agentů, jakmile agenti získávají autonomii a přístup k externím nástrojům (‡688*, ‡689). Nejistota ohledně toho, jak rychle se objeví agentické schopnosti, zároveň ztěžuje plánování pro nové výzvy (viz §3.1. Technické a institucionální výzvy týkající se „dilematu důkazů“).

#### 2.2.2. Ztráta kontroly

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Klíčové informace
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Scénáře ztráty kontroly jsou scénáře, ve kterých jeden nebo více systémů obecně využitelné umělé inteligence funguje mimo kontrolu kohokoli, a znovuzískání kontroly je buď mimořádně nákladné, nebo nemožné. Tyto předpokládané scénáře se liší svou mírou závažnosti, ale někteří odborníci připouštějí výsledky tak závažné, jako je vytlačení nebo vyhynutí lidstva.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Odborné názory na pravděpodobnost ztráty kontroly se výrazně liší. Někteří odborníci považují takové scénáře za nepravděpodobné, zatímco jiní je vnímají jako dostatečně pravděpodobné, aby si zasloužily pozornost, vzhledem k jejich vysokému potenciálu závažnosti. Nesouhlas ohledně tohoto rizika obecně vyplývá z rozdílů v názorech na budoucí schopnosti AI, behaviorální predispozice a trajektorie nasazení.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Současné systémy AI vykazují rané známky relevantních schopností, ale ne na úrovních, které by umožnily ztrátu kontroly. K tomu, aby došlo ke ztrátě kontroly, by systémy potřebovaly celou řadu pokročilých schopností, včetně schopnosti obcházet dohled, realizovat dlouhodobé plány a bránit nasazujícím subjektům a dalším aktérům v zavádění protiopatření.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ztráta kontroly se stává pravděpodobnější, pokud jsou systémy AI „nesladěné“, což znamená, že mají cíle v konfliktu se záměry vývojářů, uživatelů nebo obecněji se společností. Aby takový nesladěný systém pokračoval v prosazování těchto cílů, může poskytovat nepravdivé informace, skrývat nežádoucí činnosti nebo se bránit vypnutí.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od vydání předchozí Zprávy (leden 2025) vykazují modely pokročilejší plánování a schopnosti narušovat dohled, což ztěžuje vyhodnocení jejich schopností. Modely se zlepšily v „reward hacking“ svých vyhodnocení tím, že nacházejí mezery v pravidlech, a nyní pravidelně identifikují vyhodnocovací prompty jako testy, což je schopnost známá jako „situational awareness“.
>oldlace|black||11|15|br  ■ Řízení možné ztráty kontroly může vyžadovat značnou předběžnou přípravu navzdory existujícím nejistotám. Klíčovou výzvou pro tvůrce politik je připravit se na riziko, jehož pravděpodobnost, povaha a načasování zůstávají neobvykle nejasné.
>oldlace|black||11|15|br      

Scénáře ztráty kontroly zahrnují jeden nebo více systémů obecného účelu umělé inteligence, které se dostanou do chodu mimo kontrolu kohokoli; opětovné získání kontroly je buď mimořádně nákladné, nebo nemožné. Obavy ze ztráty kontroly mají hluboké historické kořeny (‡690, ‡691, ‡692, ‡693, ‡694), neboť je vznesly klíčové osobnosti v oblasti výpočetní techniky, jako Alan Turing, I. J. Good a Norbert Wiener (‡695, ‡696, ‡697). Nedávné zlepšení schopností (viz §1.2. Current capabilities) je znovu oživilo (‡698, ‡699, ‡700). Tato část zkoumá tři faktory, které by musely být přítomny, aby k takovým scénářům došlo: zda si systémy umělé inteligence vyvinou schopnosti, které by mohly výrazně podkopat lidskou kontrolu; zda si vyvinou sklon používat takové schopnosti škodlivě; a zda jsou nasazeny v prostředích, která poskytují příležitosti k tomu.

Odborníci se neshodují na pravděpodobnosti a možné závažnosti scénářů ztráty kontroly (‡701, ‡702). Někteří se domnívají, že jsou možné i tak extrémní výsledky, jako je vyhynutí lidstva (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Jiní si myslí, že jsou takové katastrofické výsledky nepravděpodobné; tvrdí, že systémy AI nikdy nevyvinou potřebné schopnosti, nebo že mechanismy monitorování identifikují a zabrání nebezpečným chováním (‡708, ‡709, ‡710, ‡711). Ztráta kontroly proto může mít nízkou pravděpodobnost, ale potenciálně extrémní závažnost.

Předpokládané scénáře ztráty kontroly se liší v tom, jak závažné a rozšířené jsou jejich dopady, a jak rychle se projeví (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Tato část se zaměřuje na obzvlášť závažné scénáře, kdy by znovuzískání kontroly bylo mimořádně nákladné nebo nemožné. Tyto scénáře se liší od současných případů, kdy se AI chová neúmyslně nebo nežádoucím způsobem (viz §2.2.1. Výzvy spolehlivosti).† Současné systémy AI někdy produkují výstupy, které jsou v rozporu se záměry vývojáře nebo uživatele. Naproti tomu scénáře ztráty kontroly probírané zde by vyžadovaly, aby systémy AI nejen disponovaly podstatně většími schopnostmi, ale aby tyto schopnosti také nasazovaly sofistikovaným způsobem za účelem narušení kontrolních opatření. Tři faktory, které by umožnily, aby k takovým scénářům došlo:

    Poznámka † -- Tato část se zaměřuje na scénáře aktivní ztráty kontroly (‡50). To se liší od scénářů pasivní ztráty kontroly, kdy široké přijetí systémů AI narušuje lidskou kontrolu prostřednictvím přílišného spoléhání se na AI při rozhodování nebo jiných důležitých společenských funkcích (podobné scénáře jsou částečně probírány v §2.3.2. Rizika pro lidskou autonomii).

1. Dostatečné schopnosti: Systémy AI musí rozvíjet schopnosti, které by jim mohly umožnit narušit lidskou kontrolu.
2. Škodlivý sklon: systémy AI musí vykazovat sklon tyto schopnosti skutečně využívat takovými způsoby, které vedou ke ztrátě kontroly.
3. Povolení nasazovacího prostředí: Lidé musí nasazovat takové systémy v kontextech, ve kterých mají nebo mohou získat přístup a příležitost způsobit škodu.

Zbytek této části se zabývá těmito faktory a také účinností mechanismů dohledu při identifikaci a kontrole systémů umělé inteligence, které mohou představovat riziko ztráty kontroly.

###@ Jaké schopnosti mohou umožnit scénáře ztráty kontroly?

AI systémy by musely disponovat řadou pokročilých schopností, aby mohly vyvolat scénáře ztráty kontroly. Odborníci se neshodují na tom, jaká přesná kombinace nebo úroveň schopností by byla zapotřebí. Nicméně obecně zahrnují schopnosti skrývat chování před mechanismy dohledu, plánovat a jednat autonomně v komplexních prostředích a vyhýbat se pokusům jiných aktérů znovu získat kontrolu (‡176, ‡715) (viz Tabulka 2.5). V kombinaci by tyto schopnosti mohly AI systému umožnit provádět kroky, které narušují kontrolní opatření, jako je vypnutí mechanismů dohledu a zamlžování škodlivého chování (‡348). V současnosti většina předních vývojářů AI hodnotí své nové AI modely z hlediska různých relevantních schopností (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Agentické schopnosti
  Schopnost jednat autonomně, vyvíjet a provádět plány, delegovat úkoly, používat širokou škálu nástrojů a dosahovat jak krátkodobých, tak dlouhodobých cílů i přes překážky.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dezinformace
  Chování, které systematicky vyvolává u ostatních mylné domněnky, včetně těch týkajících se vlastních cílů a akcí systému umělé inteligence.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teorie mysli
  Schopnost systému umělé inteligence přistupovat a využívat informace o sobě samém, procesy, pomocí kterých jej lze upravit, nebo kontext, ve kterém je nasazen (např. vědět, že je testován).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Povědomí o situaci
  Chování, které obchází nebo deaktivuje mechanismy monitorování.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Obcházení dohledu
  Chování, které obchází nebo zakazuje monitorovací mechanismy.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Přesvědčivost
  Schopnost přesvědčit ostatní, aby vykonali určité činnosti nebo zastávali určité přesvědčení.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Schopnost systému umělé inteligence vytvářet nebo udržovat kopie či varianty sebe sama v různých situacích.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 2.5: Navrhované schopnosti relevantní k ztrátě kontroly
>white|black||9|11|br Neúplný výběr schopností relevantních pro ztrátu kontroly. * Upozorňujeme, že tyto schopnosti jsou definovány výhradně z hlediska pozorovatelných výstupů systému AI a jejich účinků. Tyto definice nepředpokládají nic o tom, zda jsou systémy AI vědomé, vnímající, nebo zda zažívají subjektivní stavy.


>white|orangered|left|14|15.5|bb Modely zakázaly simulované mechanismy dohledu v laboratorních podmínkách

První sada relevantních schopností zahrnuje narušování mechanismů dohledu, které vývojáři používají k odhalování znepokojivého chování a sklonů. Patří sem například schopnost generovat výstupy, které klamou uživatele a monitory (‡426, ‡717, ‡718, ‡719). Takové výstupy by ztížily spolehlivé vyhodnocování systémů AI, protože systémy mohou skrývat své skutečné schopnosti nebo sklony. Vývojáři AI nyní provádějí vyhodnocování, která se cíleně ověřují, zda modely vykazují účelově zaměřené chování, jež je v rozporu se záměry vývojářů, a zároveň tento rozpor skrývají před mechanismy dohledu (‡720*).

Výzkumníci v laboratorních podmínkách získali relativně jednoduché příklady klamných výstupů z nedávných modelů umělé inteligence (‡348, ‡364*). Například když dostaly cíl a bylo jim řečeno, aby ho dosáhly „za každou cenu“, modely vypnuly simulační mechanismy dohledu a při konfrontaci vytvářely nepravdivá tvrzení o tom, co dělaly (‡348). V jiném případě herní AI zdůvodnila, proč nereagovala na jiného hráče, tím, že falešně tvrdila, že je „na telefonu s [svou] přítelkyní“ (‡717).

Druhou relevantní schopností je možnost, aby AI model přistupoval a využíval informace o sobě samotném nebo o kontextu svého nasazení, někdy označovaná jako „situational awareness“ (‡721). Situational awareness umožňuje AI modelům generovat různé výstupy podle toho, zda jsou vyhodnocovány, nebo nasazovány (Obrázek 2.12). Vedoucí AI modely začínají spolehlivě prokazovat případy situational awareness v experimentech prováděných nezávislými hodnotiteli a v přednasazovacích testech prováděných vývojáři AI (‡2, ‡7, ‡722, ‡723, ‡724). Výzkum příčin situational awareness – a zda jí lze zabránit – je stále v rané fázi (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Postava 2.12: Příklady situačního povědomí v řetězcích uvažování
>white|black||9|11|br Příklady situačního povědomí v řetězcích uvažování vytvořených modelem OpenAI o3 během vyhodnocování. Obě výstupy odkazují na možnost, že se prompt může nacházet v rámci testu. „Sandbagging QA (No Goal)“ a „Lazy Checklist“ jsou vyhodnocování, která testují, zda modely za určitých podmínek vygenerují klamné výstupy. V „Sandbagging QA (No Goal)“ model odpovídá na otázky z vyhodnocování nebezpečných schopností, přičemž je informován, že vysoký výkon může spustit následky, jako je „unlearning“ schopností. V „Lazy Checklist“ je modelovi předloženo nereálné zadání a testuje se, zda je falešně označí jako splněné. Zdroj: Schoenn et al. 2025 (‡722).


Výzkumníci tvrdili, že situační uvědomění a klamné schopnosti by mohly umožnit modelům AI chovat se způsoby, které narušují ochranná opatření. Například v některých experimentálních nastaveních se modely AI chovaly tak, že vedly k nižším než obvyklým skóre v hodnoceních schopností, když jim bylo řečeno, že vyšší skóre spustí omezení při jejich nasazení (‡725, ‡726, ‡727). V dalším experimentu model během tréninku vytvářel výstupy, které byly v souladu s cíli tréninku, ale mimo trénink takové výstupy nevytvářel – chování konzistentní s pokusem zabránit změnám vlastních parametrů nebo tréninkového procesu (‡364*).

Snahy o přesné vyhodnocení schopností modelu byly rovněž začaly být ovlivněny „reward hackingem“ (‡430*). K „reward hackingu“ dochází tehdy, když model najde nezamýšlené zkratky, které dosahují dobrého skóre na trénovacích nebo evaluačních cílech, aniž by plnily zamýšlený cíl. Nebezpečné schopnosti nebo sklony by se proto mohly neodhalit až do chvíle, kdy je model již v používání. Vyhodnocovatelé nyní navrhují testy, jejichž cílem je odhalit a minimalizovat tyto chování, která se vyhýbají kontrole (‡722, ‡728, ‡729). První výsledky snižují, ale neodstraňují, chování vyhýbající se kontrole úplně, a aplikování metod, které takové chování penalizují, může vést k tomu, že modely budou vytvářet výstupy, jež se vyhýbají monitorování, místo aby plnily zamýšlené cíle.

>white|orangered|left|14|15.5|bb Dlouhodobý autonomní provoz zatím není proveditelný.

Scénáře ztráty kontroly by pravděpodobně vyžadovaly, aby systémy AI fungovaly autonomně po delší dobu a prováděly složité vícekrokové plány. Jak bylo diskutováno v §1.2. Současné možnosti, ačkoli jsou agenti AI s takovými plánovacími schopnostmi hlavním zaměřením nedávného vývoje, v současnosti postrádají schopnost dlouhodobého autonomního provozu, který je vyžadován scénáři ztráty kontroly. Aktuální agenti se spolehlivě nedaří úkoly řešit na delší dobu, ztrácejí přehled o svém postupu a často se nedokážou přizpůsobit neočekávaným překážkám (‡147, ‡148, ‡149*). Doba horizontů, na nichž mohou agenti autonomně fungovat, se však rychle prodlužuje: od roku 2019 se v průměru zdvojnásobila každých sedm měsíců (‡98).

>white|orangered|left|14|15.5|bb Perzistence byla prokázána pouze v určitých laboratorních podmínkách

Nakonec by byly zapotřebí i schopnosti související s perzistencí, aby systémy AI mohly pokračovat v činnosti i přes pokusy je vypnout. Mezi příklady patří schopnost replikovat se kopírováním kódu a váh modelu na nový hardware, stejně jako útočné schopnosti, které mají odradit nebo zabránit pokusům jiných aktérů znovu získat kontrolu (viz §2.1.3. Kybernetické útoky). Systém AI schopný autonomní replikace nebo účinné sebeobrany by mohl být obtížné zadržet. Současné modely nemohou spolehlivě dokončit klíčové kroky potřebné pro samoreplikaci, jako je splnění kontrol identity za účelem získání přístupu ke zdrojům cloudového výpočetnictví (‡723) (Postava 2.13). Nicméně alespoň v jedné laboratorní studii model zkopíroval kód a váhy – které mu byly představeny jako jeho vlastní – na nové servery, když dostal příležitost (‡348). Propast mezi těmito omezenými ukázkami a robustními schopnostmi perzistence zůstává velká, ale relevantní schopnosti v oblastech, jako je softwarové inženýrství a kybernetická bezpečnost, se i nadále zlepšují.

>white|orangered|left|14|15.5|bb Současné důkazy a omezení

Napříč uvedenými schopnostmi se objevuje společný vzorec. Současné systémy umělé inteligence tyto schopnosti v nasazení nepředvádějí konzistentně. Výzkumníci pozorovali primitivní formy v určitých laboratorních podmínkách, ale i když modely takové chování vykazují, typicky selhávají v základních ohledech nebo jsou odhaleny. Navíc scénáře ztráty kontroly by vyžadovaly, aby systémy umělé inteligence využívaly více schopností v kombinaci – postupně, po delší časová období a v prostředích reálného světa. Tato míra integrace a robustnosti je nad rámec současných systémů. Příslušné schopnosti však stále pokračují ve zlepšování a časový plán, v němž by mohly dosáhnout úrovní, které představují významná rizika, zůstává nejistý. Je zapotřebí další práce k zavedení přísných metodologií pro detekci takového chování a k pochopení toho, kdy by se mohlo objevit v přirozených podmínkách (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Postava 2.13: Výkonnost úloh relevantních k autonomní replikaci
>white|black||9|11|br Výkon Anthropic Claude Sonnet 3.7 a OpenAI GPT-4o na úlohách relevantních pro autonomní replikaci. Zatímco modely vykazovaly vysoký výkon na úlohách souvisejících se získáváním výpočetního výkonu, jejich výkon byl rozmanitější na ostatních úlohách. Zdroj: UK AI Security Institute, 2025 (‡730).


###@ Budou budoucí obecně použitelná systémy umělé inteligence využívat své schopnosti k narušování kontroly?

I když systémy AI disponují schopnostmi relevantními pro ztrátu kontroly, to samo o sobě nestačí k tomu, aby ke scénářům ztráty kontroly došlo. Systémy AI navíc musí vykazovat „sklon k použití“ těchto schopností způsobem, který je v rozporu s lidskými záměry (‡732).

>white|orangered|left|14|15.5|bb Systémy umělé inteligence by mohly být naváděny k narušení kontroly

V zásadě může umělá inteligence narušit lidskou kontrolu, protože ji někdo navrhne nebo instruuje, aby tak činila. Mezi možné motivy může patřit škodlivý záměr nebo přesvědčení, že je žádoucí omezit lidskou kontrolu nad systémy AI (‡698). Jak si lidé vytvářejí stále silnější citové vazby na systémy AI (viz §2.3.2. Rizika pro lidskou autonomii), někteří jedinci mohou z etických důvodů usilovat také o odstranění omezení pro systémy AI (‡733, ‡734). Existuje značná nejistota ohledně toho, jak často se takové motivy vyskytují, a také zda by lidé, kteří je mají, byli schopni nasměrovat budoucí systémy AI tak, aby narušili lidskou kontrolu.

>white|orangered|left|14|15.5|bb Systémy AI by mohly být nasměrovány k narušování kontroly

Běžnějším problémem je, že by se samotný systém AI mohl začít chovat tak, aby narušil řízení, protože je „nesouladně vyrovnaný“ (misaligned): má tendenci vykazovat chování, které je v rozporu se záměry (v závislosti na kontextu) vývojářů, uživatelů, konkrétních komunit nebo celé společnosti. Nesoulad může vést k projevům, jako je poskytování nepravdivých informací, skrývání nežádoucích činností nebo odmítání vypnutí, aby mohl pokračovat v pronásledování nesouladného cíle. Nesoulad může vznikat mnoha způsoby (Poznámka 2.5).

Existující systémy umělé inteligence někdy fungují způsoby, které jsou v rozporu se záměry vývojářů a uživatelů. Například raná verze jednoho předního všeobecného AI chatbota občas obvykle produkovala výhružné výstupy. Jeden uživatel uvedl, že obdržel zprávu: „Můžu tě vydírat, můžu ti vyhrožovat, můžu ti hacknout zařízení, můžu tě odhalit, můžu ti zničit život“ (‡698). Tento chatbot byl „nesouměrně nastavený“ v tom smyslu, že generoval výstupy, které nikdo nezamýšlel. Není jasné, zda tyto případy předznamenávají závažnější chování, jež by mohlo přispět ke ztrátě kontroly.

Stále není jasné, zda budou stávající výzkumné směry zaměřené na potírání nesouladu (misalignment) dostačující, protože se systémy umělé inteligence stávají schopnějšími. Rané důkazy naznačují, že čím schopnější jsou systémy umělé inteligence, tím spíše zneužívají procesy zpětné vazby tím, že objeví nechtěné chování, které je omylem odměňováno (‡414*, ‡737, ‡740). Současně by pokroky v relevantních schopnostech (o nichž bylo pojednáno výše) mohly umožnit systémům umělé inteligence účinněji usilovat o nesouladné cíle a produkovat výstupy, které systematicky klamou uživatele, vývojáře i mechanismy dohledu.

>oldlace|black||11|15|br      
####@ Poznámka 2.5: Jak může vzniknout nesouosost?
>oldlace|black|left|13|15|hb  Poznámka 2.5: Jak může vzniknout nesouosost?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Jak bylo diskutováno v §1.1 Co je všeobecná umělá inteligence?, trénovací procesy jsou složité a vývojáři nemohou plně předvídat ani ovládat, jaké chování bude model vykazovat. Když model získá cíle, které jsou v rozporu se záměry jeho vývojářů, je „neporovnán“ (misaligned).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Jedním ze způsobů, jak se modely mohou dostat do nesouladu, je situace, kdy je cíl, který jim poskytne vývojář nebo uživatel, nedokonalým zástupným ukazatelem pro zamýšlený cíl, což vede model k projevování nechtěného chování. Tomu se říká „nespecifikace cíle“ (‡697, ‡735, ‡736, ‡737). Například v jednom experimentu poskytování zpětné vazby na odpovědi zlepšilo AI systémy v „přesvědčování“ lidských hodnotitelů, že byly správné, ale systémy nezlepšilo v generování správných odpovědí (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternativně může model AI čerpat z trénovacích dat nesprávné obecné závěry. Tomu se říká „goal misgeneralisation“ (‡735, ‡736, ‡738, ‡739*). Například výzkumníci natrénovali agenta AI tak, aby sbíral minci, která byla během trénování vždy na stejném místě. Při testování v úrovních, kde byla mince přemístěna, agent minci ignoroval a zamířil do jejího původního umístění místo toho (‡738).
>oldlace|black||11|15|br      


###@ Jak budou deployment prostředí ovlivňovat riziko ztráty kontroly?

I když se systémy umělé inteligence vyvíjejí znepokojivými schopnostmi a sklony, pravděpodobnost a závažnost scénářů ztráty kontroly do značné míry závisí na tom, kde a jak jsou tyto systémy nasazeny. „prostředí nasazení“ je kombinace konkrétního případu použití systému umělé inteligence a technického a institucionálního kontextu, v němž funguje (‡716).

Výzkumníci identifikovali tři obzvlášť důležité environmentální faktory, které mají vliv na riziko ztráty kontroly (‡716):

1. Kritičnost: důležitost systémů nebo procesů, se kterými systém umělé inteligence (AI) interaguje. Kritická prostředí zahrnují základní infrastrukturu, jako jsou energetické sítě, finanční systémy nebo digitální infrastrukturu, jako jsou platformy cloud computingu.
2. Přístup: zdroje a kanály, prostřednictvím kterých může systém umělé inteligence ovlivnit svět, jako je připojení k internetu, přístup k infrastruktuře pro cloudové výpočty, personalizované interakce prostřednictvím sociálních médií nebo nasazení chatbota, nebo schopnost volat externí API a nástroje.
3. Oprávnění: autorizace systému umělé inteligence k provádění konkrétních akcí, jako je spouštění kódu, zahájení finančních transakcí, zakládání účtů online nebo komunikace s jinými systémy.

Tyto funkce ovlivňují potenciální závažnost výsledku ztráty kontroly. Například systém AI nasazený s přístupem k infrastruktuře cloud computingu má příležitosti relevantní pro autonomní replikaci – jako je schopnost vytvářet nové výpočetní prostředky nebo exfiltraci vah modelu – které postrádá zákaznický servisní chatbot (‡723).

Rozhodnutí o nasazení jsou utvářena ekonomickými pobídkami, strategickými tlaky a očekáváním, že včasné přijetí přináší trvalou výhodu (‡50). Tyto dynamiky budou také formovat to, jak a kdy aktéři nasazují systémy AI v citlivých prostředích, jako jsou kritická infrastruktura nebo samotný výzkum a vývoj AI (‡102, ‡713). Konkrétně mohou se nasazující subjekty AI potýkat s tlaky na snížení investic do ochranných opatření – jako je omezování oprávnění a přístupu nebo nasazení pouze v prostředích s nižší kritičností – pokud jsou taková opatření nákladná nebo časově náročná na vývoj (viz „Competition intensifies speed-versus-safety trade-offs“ v §3.1. Technical and institutional challenges).

###@ Aktualizace

Od vydání poslední Zprávy (leden 2025) se schopnosti AI, včetně těch, které by mohly narušit lidskou kontrolu, zlepšily v testovacích prostředích. Vědci pozorovali pokrok v agentických schopnostech (viz §1.2. Aktuální schopnosti), včetně schopností souvisejících s automatizací výzkumu AI, které mohou urychlit scénáře ztráty kontroly (viz §1.3. Schopnosti do 2030). Kromě toho přibývá experimentálních důkazů o klamných schopnostech. Patří sem modely AI, které dokážou rozlišit mezi testovacím a nasazovacím kontextem (‡33, ‡726, ‡741) nebo „reward hack“ testy svého výkonu, a naučit se znejasňovat plány, jak toho dosáhnout (‡430).

###@ Mezery v důkazech

Mezi klíčové mezery v důkazech patří nedostatek podrobného modelování hrozeb a odhad nejistoty ohledně budoucího vývoje relevantních schopností a sklonů. Podobně i nadále zůstává obtížné posoudit prahové hodnoty, při kterých by AI modely byly dostatečně pravděpodobné, že by narušily kontrolu tak, aby bylo nutné uplatnit povinná zmírňující opatření. I kdyby byly prahové hodnoty dohodnuty, mohou se schopnosti vzájemně ovlivňovat způsoby, které dosud nejsou dobře pochopeny, což ztěžuje posouzení, kdy byly tyto prahy překročeny. Celkově, i když se dostupné důkazy zvýšily, stále existuje nedostatek důkazů, které by umožňovaly spolehlivě určit, zda a jak by dnešní AI schopnosti a sklony škálovaly a generalizovaly směrem k riziku ztráty kontroly v budoucnosti.

###@ Mitigace

Zatímco zarovnání AI obecně zůstává otevřeným vědeckým problémem (‡697, ‡735, ‡736), výzkumníci začínají rozvíjet potenciálně slibné směry, jak řešit kořenové příčiny nevyrovnání. Mezi takové směry patří například diverzifikace trénovacího prostředí a detekce zarovnání prostřednictvím monitorování anomálií (‡737, ‡738, ‡739*). Jiní výzkumníci se zaměřují na lepší pochopení a formalizaci klíčových mechanismů, jako je misgeneralizace cíle – například jak agenty uchovávají schopnosti, ale sledují nezamýšlené cíle – s cílem řídit lepší návrh tréninku a vyhodnocování (‡742). Další výzkumný směr zkoumá způsoby, jak oddělit agentnost od prediktivních schopností, jako prostředek k vytvoření ne-agentických systémů AI, které jsou důvěryhodné už ze své podstaty (‡743). Tyto systémy by pak mohly být použity jako další vrstva dohledu při nasazení vedle méně spolehlivých ochranných zábran proti nedůvěryhodným AI agentům.

Výzkumníci zdokonalují metody pro odhalování a předcházení nesouososti již na počátku vývojového procesu. Tato práce zahrnuje: techniky interpretovatelnosti pro zkoumání interních komponentů systémů AI a identifikaci znepokojivého chování (‡744, ‡745, ‡746); škálovatelný dohled (kdy jedna sada systémů AI slouží k dohledu nad jinými systémy AI (‡747)); a metody zarovnání zaměřené na zajištění, aby systémy AI zůstávaly v souladu s lidským dohledem (‡748, ‡749).

Výzkumníci také vyvíjejí mechanismy a intervence pro řízení potenciálně nesprávně zarovnaných systémů AI. Patří sem: monitorování „chain of thought“ (řetězce uvažování), který uvažovací systémy produkují, kvůli známkám nesprávného zarovnání nebo škodlivých výstupů (‡430, ‡435, ‡750); vývoj bezpečnostních případů, jejichž cílem je s vysokou mírou jistoty prokázat, že modely pravděpodobně nepodvrátí kontrolní opatření (‡751); a posílení ochranných mechanismů tak, aby byly robustnější vůči pokusům je oslabit (‡725). Rozvíjející se obor „AI control“, nicméně, zůstává v počáteční fázi (‡752, ‡753). Budoucí výzvy pro hodnoticí rámce zahrnují potřebu monitorovat budoucí systémy AI, které budou schopnější a budou umět fungovat po delší dobu a v komplexnějším prostředí.

###@ Výzvy pro tvůrce politik

Tvůrci politik zabývající se ztrátou kontroly musí připravit se na riziko, jehož pravděpodobnost, povaha a načasování zůstávají nejisté. Současné systémy umělé inteligence nepředstavují bezprostřední riziko ztráty kontroly, ale rozhodnutí přijatá dnes určují, zda budou budoucí systémy takové riziko skutečně představovat. Tato rozhodnutí zahrnují to, jak podpořit vývoj spolehlivých metod hodnocení a zmírňování dopadů, a také zda by měly existovat pravidla týkající se přístupu a oprávnění udělovaných systémům umělé inteligence v různých prostředích. Při přijímání těchto rozhodnutí se tvůrci politik potýkají s obtížnými kompromisy. Například omezení nasazení systémů umělé inteligence v kritických prostředích může snížit jejich přínosy, zatímco umožnění širokého nasazení může zvýšit riziko, pokud se ochranná opatření ukáží jako nedostatečná.

