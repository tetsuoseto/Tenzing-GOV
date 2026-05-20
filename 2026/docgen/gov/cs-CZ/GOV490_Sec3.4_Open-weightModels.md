##########
>white|orangered|left|14|30|hr Sekce 3.4
### 3.4. Modely s otevřenou váhou
>white|orangered|left|24|30|hb Modely s otevřenou váhou

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Klíčové informace
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Úroveň přístupu, kterou AI společnosti poskytují k „vahám“ svých modelů, ovlivňuje rizika, která tyto modely představují. Vahy jsou matematické parametry, které umožňují AI modelům zpracovávat vstupy a generovat výstupy. U daného modelu mohou společnosti zvolit, že budou váhy zcela soukromé, poskytnou některým uživatelům určitý omezený přístup, nebo umožní komukoli je stáhnout v plné podobě. Modely, jejichž váhy jsou veřejně dostupné, se nazývají „open-weight modely“.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Modely s otevřenou váhou usnadňují výzkum a inovace, ale jejich ochranná opatření se odstraňují snáze. Po celém světě mohou různí aktéři – zejména ti, kteří mají méně zdrojů – používat modely s otevřenou váhou pro výzkumné i komerční účely. Nicméně ve srovnání s modely s uzavřenou váhou se modely s otevřenou váhou snáze upravují tak, aby vykazovaly potenciálně škodlivé chování, a je obtížnější to ovlivnit.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Vydání modelů s otevřenou licencí je nevratné. Jakmile jsou vydány, váhy modelu nelze odvolat. To ztěžuje zmírnění možných škod vyplývajících z vydání modelu s nebezpečnými schopnostmi.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Od zveřejnění poslední zprávy (leden 2025) se výrazné open-weight (otevřené váhy) aktualizace přiblížily schopnostnímu náskoku vedoucích uzavřených modelů. Čínští vývojáři DeepSeek a Alibaba vydali své modely R1 a Qwen, které dosáhly výkonu srovnatelného s předními uzavřenými modely, zatímco OpenAI vydala své první open-weight modely od roku 2019. V současnosti se odhaduje, že schopnosti vedoucích uzavřených modelů jsou na významných benchmarkách v oblasti umělé inteligence méně než 1 rok před schopnostmi předních open-weight modelů.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Hlavní politická výzva spočívá v tom, jak zpřístupnit výhody, které poskytují modely s otevřenou váhou, a zároveň řídit jejich odlišná rizika. Jedním z přístupů je posuzovat modely s otevřenou váhou z hlediska jejich „mezního rizika“: do jaké míry jejich zpřístupnění kontrafakticky zvyšuje společenské riziko nad rámec toho, které by již způsobovaly existující modely nebo jiné technologie. V praxi je to však složité. I malé nárůsty mezního rizika v čase se mohou postupně nahromadit a vést k podstatnému nárůstu celkového rizika.
>oldlace|black||11|15|br      


Modely s otevřenými váhami, jejichž parametry jsou veřejně dostupné ke stažení, mají odlišné dopady na mnoho výzev probíraných v předchozích částech. „Váhy“ AI modelu obsahují klíčové informace, které mu umožňují vytvářet užitečné odpovědi pro uživatele. Jakmile jsou tyto váhy zveřejněny, nelze je odvolat: kdokoli si je může stáhnout, prostudovat, upravit, sdílet a používat na vlastních počítačích nebo v cloudových účtech. Když jsou váhy otevřeně dostupné, ostatní je mohou snáze rozvíjet a upravovat, čímž uspokojují rozmanité potřeby a podporují inovace (‡1317). Zároveň však stejný mechanismus umožňuje uživatelům se škodlivým úmyslem snáze odstranit bezpečnostní prvky a upravit modely s otevřenými váhami pro škodlivé případy použití (‡1122, ‡1160). To vyvolalo otázku, zda by některé modely s otevřenými váhami měly podléhat zvláštním požadavkům (např. přísnějšímu testování před uvedením) nebo naopak dostat zvláštní výjimky (např. z požadavků na regulační ohlašování) (‡1033).

###@ Pozadí otevřených váhových modelů

>white|orangered||14|15.5|bb Modely s otevřenou váhou mohou být, ale nutně nemusí, „open source“ modely

Ačkoli se to často označuje jako „open source“, většina veřejně vydaných modelů je přesněji popsána jako „open-weight“. Je to proto, že i když vývojáři poskytují váhy modelu, neuvolňují související trénovací kód ani datové sady. Kromě toho se open source software obvykle vyznačuje licencemi, které kladou na navazující aktéry používající nebo upravující software minimální požadavky (‡1318). Například modely Meta Llama mají restriktivní podmínky licence a obsahují pouze inferenční kód, nikoli trénovací kód, a proto se typicky nepovažují za open source (‡1319, ‡1320). Možnosti uvolnění modelů existují na škále od plně uzavřeného po plně open source, přičemž v každém bodě existují různé kompromisy mezi rizikem a přínosem (‡1086*, ‡1320, ‡1321). Tabulka 3.9 popisuje tyto možnosti.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Plně uzavřeno
  Uživatelé se s modelem nemohou přímo interagovat vůbec
  Příklady: Plameňák (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Hostovaný přístup
  Uživatelé mohou komunikovat pouze prostřednictvím konkrétní aplikace nebo rozhraní, například mobilní chatbot aplikace
  Příklady: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Přístup k modelu přes API
  Uživatelé mohou odesílat požadavky na model prostřednictvím kódu, což umožňuje použití v externích aplikacích
  Příklady: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Přístup k API pro jemné doladění
  Uživatelé mohou model doladit podle svých konkrétních potřeb
  Příklady: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Otevřená váha: váhy dostupné ke stažení
  Uživatelé si mohou stáhnout a spustit model na vlastních počítačích
  Příklady: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Váhy, data a kód k dispozici ke stažení s omezeními použití
  Uživatelé si mohou stáhnout a spustit model, stejně jako kód pro inference a trénování, ale na jeho používání se vztahují určitá licenční omezení
  Příklady: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Plně otevřené: váhy, data a kód jsou k dispozici ke stažení bez omezení použití
  Uživatelé mají naprostou svobodu si model, kompletní kód a data stáhnout, používat a upravovat
  Příklady: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabulka 3.9: Možnosti sdílení modelů od plně uzavřených až po plně otevřené
>white|black||9|11|br Ilustrační výběr možností sdílení modelů, od plně uzavřených modelů (modely jsou soukromé a uchovávané pouze pro proprietární použití) až po plně otevřené a open source modely (váhy modelu, data a kód jsou volně a veřejně dostupné bez omezení použití, úprav a sdílení). Modely spadající do prvních čtyř kategorií se často označují jako „uzavřené“. Tato část se zaměřuje na tři spodní řádky. Zdroj: převzato a upraveno z Bommasani, 2024 (‡1317).


###@ Výhody a rizika

>white|orangered|left|14|15.5|bb Modely s otevřenou váhou lze snáze přizpůsobit a vyhodnocovat

Modely s otevřenými váhami přinášejí významné výhody pro výzkum, inovace a přístup. Jak je uvedeno v §1.1. Co je obecná umělá inteligence?, trénování modelů obecné umělé inteligence je mimořádně drahé – přední modely vyžadují stovky milionů dolarů na vývoj. Otevřené zpřístupnění vah umožňuje méně dobře vybaveným aktérům replikovat, studovat a stavět na existujících systémech. Bez takového přístupu hrozí komunitám v regionech s nízkými zdroji vyloučení z výhod, které AI přináší, a proto jsou otevřené váhy klíčové pro umožnění globální většinové účasti na vývoji AI (‡1322). Následní vývojáři mohou upravovat modely pro různé aplikace; například je přizpůsobit pro nedostatečně obsluhované menšinové jazyky nebo optimalizovat výkon pro konkrétní úkoly, jako je právní sepis nebo pořizování lékařských poznámek (‡1323, ‡1324*). Tímto způsobem mohou modely s otevřenými váhami umožnit více lidem a komunitám používat AI a mít z ní prospěch, než by jinak bylo možné (‡1325). V případě modelů, které nejsou dostatečně schopné, aby byly nebezpečné, mohou tyto přínosy převážit nad dodatečným rizikem otevřeného zpřístupnění vah, ačkoli to závisí na míře tolerance k riziku ze strany relevantních rozhodovatelů.

Uvolnění s otevřenou vahou zároveň rozšiřuje okruh vývojářů a výzkumníků, kteří mohou model studovat, vyhodnocovat jeho schopnosti, testovat zranitelnosti a iterovat na zlepšeních (‡1326, ‡1327). Tím se zvyšuje pravděpodobnost, že budou identifikovány prospěšné aplikace i škodlivé nedostatky, i když to není zaručeno (‡1328, ‡1329). Uživatelé navíc mohou spouštět modely s otevřenou vahou na vlastních zařízeních, což jim umožňuje udržet kontrolu nad citlivými daty a vyhnout se jejich odesílání na servery třetích stran.

Existují další výhody, když vývojáři sdílejí informace, jako jsou trénovací data, kód, nástroje pro vyhodnocení a dokumentace, stejně jako váhy modelu (‡1320, ‡1330, ‡1331, ‡1332*). S více informacemi mohou navazující vývojáři a další výzkumníci lépe porozumět modelům s otevřenými váhami a přizpůsobit je novým aplikacím.

>white|orangered|left|14|15.5|bb Zábrany u modelů s otevřenými váhami se odstraňují snadněji, což umožňuje potenciální zneužití k škodlivým účelům

Modely s otevřenou váhovou sadou rovněž představují dodatečná rizika, protože jejich ochranná opatření se dají snáze odstranit. Zatímco otevřené i uzavřené modely mohou mít ochranná opatření, která odmítají škodlivé uživatelské požadavky, tato ochranná opatření jsou u otevřených modelů mnohem snazší odstranit. Zlomyslní aktéři mohou model doladit tak, aby optimalizoval svůj výkon pro škodlivé aplikace, odstranit části kódu určené k zabránění škodlivému použití, nebo zrušit předchozí bezpečnostní doladění (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). V důsledku toho mohou otevřené modelové váhy zhoršit rizika zneužití probíraná v §2.1. Rizika ze zlomyslného použití tím, že umožní více aktérům využít a rozšířit existující schopnosti pro škodlivé účely bez dohledu (‡1122, ‡1315). Ačkoli mnoho uživatelů nebude mít dovednosti ani motivaci odstranit ochranná opatření u otevřených modelů, znepokojiví jsou vysoce motivovaní zlomyslní aktéři. Kromě toho mohou zlomyslní aktéři rovněž využít otevřené modely k identifikaci zranitelností v podobných uzavřených modelech (‡1055*). Takové nedostatky se hůře odhalují pouhým spouštěním uzavřených modelů, protože poskytovatelé uzavřených modelů mohou zavádět vyšší míru kontroly a monitoringu.

>white|orangered|left|14|15.5|bb Sdílení modelových vah je nevratné

Jakmile budou modelové váhy k dispozici pro veřejné stažení, neexistuje způsob, jak provést plošný rollback všech stávajících kopií. Platformy pro internetový hosting, jako je GitHub a Hugging Face, mohou odstranit modely ze svých platforem, což ztěžuje některým aktérům nalézt stažitelné kopie a vytváří významnou překážku pro mnoho nezkušených škodlivých uživatelů (‡1339). Motivovaní aktéři však mohou kopie stále získat, pokud byl model stažen a znovu hostován jinde, nebo pokud byl uložen lokálně. Navíc vývojáři navazujících řešení, kteří integrují open- weight modely do svých systémů, tím také přebírají jakékoli nedostatky, například zranitelnost vůči adversariálním útokům (‡1055) nebo schopnost modelů obcházet systémy monitorování (viz §2.2.2. Ztráta kontroly) (‡1315). Na rozdíl od uzavřených modelů, kde mohou hostitelé plošně nasadit opravy, vývojáři open- weight modelů nemohou zaručit, že uživatelé přijmou aktualizace.

###@ Aktualizace

Od vydání poslední Zprávy (leden 2025) se rozdíl v schopnostech mezi předními otevřenými modely a uzavřenými modely zúžil. Čínští vývojáři se stali obzvláště důležitými poskytovateli otevřených modelů. V lednu 2025 společnost DeepSeek uvedla svůj model R1, který dosáhl výkonu srovnatelného s modelem OpenAI o1 na řadě benchmarků (‡1340). Modely Alibaba Qwen si získaly podobně na popularitě; od srpna 2025 obsadily v Chatbot Areně, široce používaném ukazateli výkonu, první místo pro otevřený model (‡1341, ‡1342*). V srpnu 2025 OpenAI vydala své první otevřené modely od vydání GPT-2 v roce 2019, gpt-oss-120b a gpt-oss-20b. Společnost Meta nadále vydává modely Llama s otevřenými váhami. Odhaduje se, že schopnosti předních uzavřených modelů jsou nyní na významných AI benchmarkách méně než jeden rok za schopnostmi předních otevřených modelů (Postava 3.10).

###@ Mezery v důkazech

Jedna klíčová mezera v důkazech se týká skutečné účinnosti technických řešení k zabránění zneužití modelů s otevřenou váhovou sadou. Výzkumníci navrhli různé přístupy, jak učinit modely odolnými vůči zásahům. Patří sem nové trénovací techniky navržené tak, aby byly modely odolné vůči škodlivým úpravám (‡1276), filtrování škodlivého obsahu z trénovacích dat (‡55) a obrany proti jailbreakům (‡675, ‡676). Tyto techniky se nyní zavádějí do reálných vydání od významných vývojářů. Například OpenAI použila některé z těchto technik v modelech gpt-oss a uvedla, že protireverzně (adversarialně) jemně doladěné verze nedosáhly vysokých prahů schopností (‡1344*). Avšak výzkum ukázal, že aktéři se zlými úmysly mohou deaktivovat ochranné mechanismy tím, že modely znovu natrénují na škodlivých příkladech (‡1345, ‡1346). Navíc je stále obtížné spolehlivě vyhodnocovat odolnost těchto ochranných mechanismů, což činí jejich účinnost proti útokům v reálném světě nejistou (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Postava 3.10: Kognitivní mezera mezi vedoucími modely s otevřenou váhou a uzavřenými AI modely
>white|black||9|11|br Skóre Epoch Capabilities Index (ECI) nejvýkonnějších otevřených (tmavě modrá) a uzavřených (světle modrá) modelů v čase. ECI kombinuje skóre z 39 benchmarků do jedné obecné škály schopností. Nejlepší otevřené modely zaostávají přibližně o jeden rok za uzavřenými modely. Zdroj: Epoch AI, 2025 (‡1343).


###@ Mitigace

Technická opatření k mitigaci rizik modelů s otevřenou váhou fungují v celém procesu vývoje a nasazení AI (‡1141, ‡1195, ‡1347). Například při vývoji modelů mohou vývojáři a navazující adaptéry filtrovat citlivý obsah z trénovacích dat, aby minimalizovali škodlivé schopnosti. Odstranění škodlivých příkladů z trénovacích dat modelu může zabránit adversariální jemnému ladění účinněji 10krát než obrany přidané až po trénování, i když to může také ovlivnit prospěšné schopnosti (‡55). Poskytovatelé AI aplikací mohou také zavést mechanismy pro hlášení incidentů a reakci na ně (‡1348).

Kromě toho mohou hostitelské platformy, jako je HuggingFace a GitHub, stanovit podmínky služby platformy, aby odstranily modely upravené pro škodlivé účely (‡1141, ‡1324). Vývojáři modelů mohou auditorům poskytnout plný přístup ještě před vydáním, nebo zvolit strategii „postupného“ vydávání – vydávat modely směrem k postupně větším skupinám (‡1086). To může pomoci odhalit potenciální poruchy nebo zranitelnosti ještě předtím, než bude model široce dostupný (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Poznámka 3.1: Zabezpečení hmotnosti modelu
>oldlace|black|left|13|15|hb  Poznámka 3.1: Zabezpečení hmotnosti modelu
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Rizika probíraná v této části předpokládají, že jsou váhy modelu záměrně zpřístupněny. Uzavřené váhy modelu se však mohou stát dostupnými i prostřednictvím krádeže nebo úniku. Uzavřené modely stojí stovky milionů dolarů na vývoj (§1.1. Co je všeobecná AI?) a v průměru jsou schopnější než modely s otevřenými váhami (‡1343). To z nich činí atraktivní cíle pro aktéry od amatérských hackerů až po státy usilující o získání předních AI modelů.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ukradené uzavřené váhy modelu by představovaly rizika podobná těm, která byla popsána výše pro modely s otevřenými váhami, ale potenciálně bez jakýchkoli zmírňujících opatření. Zlomyslní aktéři by mohli odstranit bezpečnostní prvky z nejvýkonnějších modelů. Na rozdíl od legitimních vývojářů by tito aktéři nebyli vystaveni reputačním, právním ani obchodním omezením, která v současnosti motivují špičkové společnosti v oblasti AI k bezpečnému nasazování jejich modelů.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Aktuální úrovně zabezpečení se v celém odvětví liší a mohou být nedostatečné proti sofistikovaným útočníkům. Někteří vývojáři se zavazují k zajištění váh modelů proti kyberzločineckým syndikátům a hrozbám zevnitř (‡582), zatímco jiní neučinili žádné veřejné bezpečnostní závazky (‡1109, ‡1349). Výzkum naznačuje, že AI datová centra mohou být neschopná odolat útokům ze strany nejsofistikovanějších a nejlépe vybavených aktérů (‡582, ‡1350, ‡1351). Od prosince 2025 nejsou známy žádné potvrzené, veřejně zdokumentované případy krádeže váh modelů. Byly však hlášeny jiné bezpečnostní incidenty u předních společností v oblasti AI, včetně proniknutí do e-mailových systémů Microsoftu (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Uzavření těchto bezpečnostních mezer by vyžadovalo značné investice do hardwaru, softwaru, personálu a zabezpečení prostor. Některá bezpečnostní vylepšení by mohla být zavedena relativně rychle za koordinovaného úsilí (‡1122). Ostatní však kritická opatření, jako je zajištění dodavatelských řetězců hardwaru a zabezpečení zařízení, by pravděpodobně trvala roky (‡1122). Soukromé společnosti navíc nemusí mít zdroje nebo informace k tomu, aby samy vyvinuly odpovídající ochrany. Například vývojáři AI nemají přístup ke klasifikované zpravodajské informaci o hrozbách, kterou mají vlády (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Výzvy pro tvůrce politik

Klíčovou výzvou pro tvůrce politik je zajistit přínosy sdílení modelů s otevřenou váhovou částí, aniž by se výrazně zvýšilo riziko. Aby se předešlo katastrofickému poškození, vývojáři modelů s otevřenou váhovou částí by neměli uvolňovat modely bez vyhodnocení rizik, a to jak pomocí zavedených metod posuzování používaných pro uzavřené modely, tak i prostřednictvím dodatečného testování, protože špatní aktéři mohou modely doladit a odstranit bezpečnostní ochrany. V praxi to může být obtížné, protože vývoj schopností může být nepředvídatelný, uvolnění s otevřenými váhami je nevratné a je třeba vyhodnocovat úsilí nutné k odhadu, kdy by uvolnění představovalo významné potenciální škody. Jedním z přístupů je vyhodnocovat „hraniční riziko“ otevřených uvolnění: míru, do jaké by uvolnění kontrafaktuálně zvýšilo společenské riziko nad rámec již existujícího rizika způsobovaného stávajícími modely nebo jinými technologiemi (‡556, ‡1033, ‡1354, ‡1355) (viz §3.2. Praktiky řízení rizik). Odhadovat však, jak systém zvýší nebo sníží riziko v navazujících (downstream) procesech poté, co byl nasazen, je složité a závislé na kontextu. Postupné zvyšování rizika s postupnými uvolněními se může v čase kumulovat do značných nárůstů celkového rizika, i když se hraniční riziko spojené s každým jednotlivým uvolněním jeví jako přijatelné (‡1356, ‡1357). Dvojúčelová povaha schopností v oblasti umělé inteligence dále komplikuje řízení: vlastnosti umožňující prospěšné aplikace v medicíně nebo ve výzkumu mohou být přesměrovány na škodlivé účely a jakmile jsou váhy veřejné, může být obtížné odlišit legitimní od škodlivých použití. Není také jasné, kdo by měl nést odpovědnost v případě, že jsou modely s otevřenou váhovou částí upraveny pro škodlivé účely.

