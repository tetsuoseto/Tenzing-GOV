##########
>white|orangered|left|14|30|hr Sezione 3.2
### 3.2. Pratiche di gestione del rischio
>white|orangered|left|24|30|hb Pratiche di gestione del rischio

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informazioni chiave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ La gestione del rischio per l’AI a uso generico comprende una gamma di pratiche utilizzate per identificare, valutare e ridurre i rischi derivanti dall’AI a uso generico. Queste includono test e valutazioni a livello di modello (come il “red-teaming”), processi organizzativi che guidano le decisioni di sviluppo e rilascio, salvaguardie condizionali (come gli impegni “if-then”), e la segnalazione degli incidenti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Diversi sviluppatori di AI hanno prodotto Frontier AI Safety Frameworks. Questi framework includono informazioni sulle valutazioni del rischio e specificano misure condizionali, come le restrizioni di accesso che le aziende intendono implementare per modelli più capaci. Si differenziano per i rischi che coprono, per come definiscono le soglie di capacità e per quali azioni vengono attivate quando tali soglie vengono raggiunte.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Le prove sull’efficacia nel mondo reale delle pratiche di gestione del rischio dell’AI rimangono limitate. La mancanza di segnalazione degli incidenti e di monitoraggio rende difficile valutare quanto bene le pratiche attuali riducano i rischi o quanto coerentemente vengano implementate.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dalla pubblicazione dell’ultimo Rapporto (gennaio 2025), la gestione del rischio è diventata più strutturata grazie a nuove iniziative di settore e di governance. Nuovi strumenti come il Codice di Pratica per l’AI a Uso Generale dell’UE, il Quadro di Governance della Sicurezza dell’AI della Cina 2.0 e il Quadro per la Rendicontazione del Processo sull’AI di Hiroshima del G7, insieme alle iniziative promosse dalle aziende, illustrano la tendenza verso approcci più standardizzati alla trasparenza, alla valutazione e alla rendicontazione degli incidenti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Le dinamiche di mercato e il ritmo dello sviluppo dell'AI pongono ulteriori sfide. A causa delle pressioni competitive, le aziende di AI possono trovarsi di fronte a compromessi tra rilasci di prodotto più rapidi e investimenti nelle attività di riduzione del rischio. Molti danni legati all'AI vengono anche esternalizzati e la responsabilità legale per essi resta poco chiara, mentre i processi di governance possono essere lenti ad adattarsi ai cambiamenti nel panorama dell'AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Le principali sfide per i responsabili delle politiche includono dare priorità tra i diversi rischi posti dall'AI per finalità generiche, e chiarire quali attori lungo la catena del valore dell'AI siano meglio posizionati per mitigarli. Queste sfide sono ulteriormente aggravate da una visibilità limitata su come i rischi vengano identificati, valutati e gestiti nella pratica, nonché da una condivisione delle informazioni frammentata tra sviluppatori, operatori e fornitori di infrastrutture.
>oldlace|black||11|15|br      


La gestione del rischio per l'AI comprende una gamma di pratiche volte a identificare, valutare e ridurre la probabilità e la gravità dei rischi associati ai sistemi di AI. Tali pratiche possono essere implementate da sviluppatori di AI, operatori (deployer), valutatori e regolatori. Esempi includono modellazione delle minacce, classificazione dei rischi (risk tiering), red-teaming, audit e reporting degli incidenti. Questa sezione descrive le pratiche di gestione del rischio attualmente in uso, i nuovi sviluppi e i limiti ancora esistenti.

Dall’inizio del 2025, diverse nuove iniziative internazionali per la gestione del rischio dell’AI per scopi generali si sono sviluppate, incluse framework di trasparenza organizzativa e di reporting del rischio, nonché framework regolatori e di governance.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Figura 3.4: Quattro componenti della gestione del rischio
>white|black||9|11|br Le quattro categorie di metodi per la gestione del rischio di AI per scopi generali: identificazione del rischio; analisi e valutazione del rischio; mitigazione del rischio; e governance del rischio. Queste costituiscono un processo iterativo e ciclico. La governance del rischio, mostrata al centro, facilita il successo degli altri componenti. Fonte: International AI Safety Report 2026.


Le sfide rimanenti includono una standardizzazione limitata, che complica la conformità e la valutazione, e una documentazione limitata relativa all’efficacia nel mondo reale. Inoltre, i contesti istituzionali, culturali e politici differiscono a livello globale, il che implica che gli approcci per identificare e gestire i rischi, inclusi i livelli di rischio accettabili, possano variare tra le regioni. La discussione in questa sezione sugli approcci di gestione del rischio è descrittiva: mira a informare gli attori dell’ecosistema dell’IA sugli approcci globali attuali alla gestione del rischio. Quando disponibile, viene discusso il livello di evidenza sull’efficacia e sui limiti di tali approcci, ma le raccomandazioni di policy esulano dall’ambito di questo lavoro.

###@ Componenti della gestione del rischio

La gestione del rischio è un processo iterativo con pratiche e metodi che coprono l'intero ciclo di sviluppo e di deployment dell'AI, ma che lavorano insieme in modo coerente (‡969). La gestione del rischio per l'AI a finalità generali può includere ruoli per un'ampia gamma di attori, tra cui data scientist, ingegneri del modello, revisori (auditor), esperti di dominio, dirigenti, utenti finali, comunità interessate, fornitori terzi, responsabili delle politiche pubbliche, governi, organizzazioni di standardizzazione e organizzazioni della società civile (‡970, ‡971, ‡972). I principali standard di gestione del rischio sono spesso interoperabili, ma utilizzano terminologie diverse per descrivere gli elementi della gestione del rischio (‡973, ‡974). In genere presentano quattro componenti interconnesse (Figura 3.4): identificare; analizzare e valutare; mitigare; e governare il rischio (‡970, ‡973, ‡975, ‡976). Le tabelle riportate di seguito forniscono esempi illustrativi di metodi, tecniche e strumenti rilevanti. Le pratiche continuano a evolvere, quindi le tabelle non sono esaustive e l'applicabilità varierà in base ai contesti.

###@ Rilevazione dei rischi

L’identificazione dei rischi è il processo di individuare, riconoscere e descrivere i rischi. Un’identificazione dei rischi completa in genere include valutazioni guidate dalla capacità, che verificano se i modelli possiedono specifiche capacità pericolose (‡977), oltre alla modellazione del rischio (‡978) e alla previsione (‡715*), utilizzate per esplorare rischi esistenti ed emergenti. La Tabella 3.1 fornisce vari esempi di pratiche di identificazione dei rischi. L’identificazione dei rischi si basa inoltre sul coinvolgimento di esperti e comunità rilevanti per comprendere il contesto più ampio in cui i rischi emergono (‡979, ‡980). Meccanismi come i programmi di bug bounty possono supportare questo processo incentivando l’identificazione di vulnerabilità precedentemente sconosciute (‡981) (Tabella 3.1). Un obiettivo chiave dell’identificazione dei rischi è considerare sia i rischi noti e ben compresi sia i potenziali rischi futuri che restano incerti o scarsamente caratterizzati (‡982). Questo è particolarmente importante per l’AI di finalità generale, in cui molti rischi potrebbero non essere ancora completamente compresi o osservabili (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb programmi di bug bounty
  I programmi di bug bounty o di divulgazione delle vulnerabilità incentivano le persone a individuare e segnalare vulnerabilità nei sistemi di AI. Diversi sviluppatori hanno implementato programmi di bug bounty (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Consulenza esperta
  Gli esperti di dominio, gli utenti e le comunità interessate forniscono indicazioni sui rischi probabili. Stanno emergendo linee guida per l’IA partecipativa e inclusiva (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Diagramma a lisca di pesce (Ishikawa)
  I diagrammi a lisca di pesce sono strumenti di analisi delle cause radice ben consolidati e i ricercatori hanno proposto di usarli per un’analisi strutturata degli incidenti di rischio dell’AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Previsione
  La previsione è il processo di prevedere eventi o tendenze future sulla base dell’analisi di dati passati e presenti. È stata usata per confrontare la probabilità relativa di, ad esempio, diversi esiti economici dovuti all’AI avanzata (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tassonomia dei rischi
  Le tassonomie del rischio sono un modo per categorizzare e organizzare i rischi lungo più dimensioni. Ne esistono diverse che descrivono i rischi legati all'AI di uso generale (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pianificazione degli scenari
  La pianificazione degli scenari consiste nello sviluppare scenari futuri plausibili e nell’analizzare come si concretizzino i rischi. È stata utilizzata per esplorare i rischi e gli impatti dei modelli di intelligenza artificiale (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb modellazione delle minacce
  La threat modelling è un processo per identificare minacce e vulnerabilità per un sistema. Numerosi sviluppatori di IA evidenziano il suo utilizzo per anticipare potenziali scenari di uso improprio dei sistemi di IA (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.1: Esempi di identificazione dei rischi nella gestione dei rischi dell'AI di uso generale
>white|black||9|11|br Esempi di metodi per l'identificazione dei rischi dell'IA elencati in ordine alfabetico. I metodi inclusi
sono progettati per supportare l’identificazione del rischio per molti tipi diversi di rischio, inclusi i rischi derivanti da usi malevoli, i rischi derivanti da malfunzionamenti e i rischi sistemici. Data la natura ancora agli inizi della gestione del rischio per l’IA di uso generale, non tutti i metodi saranno adatti a ogni sviluppatore o responsabile della distribuzione dell’IA.


>white|orangered|left|14|15.5|bb La modellazione delle minacce e le tassonomie dei rischi sono metodi di identificazione dei rischi di rilievo

Due metodi di rilievo per identificare i rischi derivanti dall’AI a uso generale sono la threat modelling (International AI Safety Report 2026) (un processo strutturato per mappare come i rischi legati all’AI possano concretizzarsi) e le risk taxonomies. Meta, ad esempio, utilizza esercizi di threat modelling per anticipare potenziali scenari di uso improprio dei suoi modelli di AI (‡990), e Anthropic include la threat modelling come parte del suo ASL-3 Deployment Standard (‡991). Le AI risk and hazard taxonomies, che elencano categorie di rischio ed esempi, possono ugualmente fungere da punto di partenza per concettualizzare, identificare e specificare i rischi rilevanti associati all’AI a uso generale in specifici domini applicativi (‡906, ‡988, ‡992, ‡993).

###@ Analisi e valutazione del rischio

L’analisi e la valutazione del rischio è il processo di determinazione del livello di rischio di un modello o sistema di AI e di confronto con criteri stabiliti per valutarne l’accettabilità o la necessità di mitigazione (‡994, ‡995, ‡996, ‡997). Include pratiche come la misurazione delle prestazioni del modello su benchmark (‡998) e valutazioni (‡176, ‡715), lo svolgimento di esercizi di red-teaming (‡999*), le valutazioni di impatto (‡1000) e gli audit (‡1001, ‡1002). Vedere Tabella 3.2 per esempi di analisi e valutazione del rischio dell’AI di finalità generale. I metodi sono progettati per supportare analisi e valutazioni simultanee per molti diversi tipi di rischio.

Gli obiettivi chiave dell’analisi e della valutazione del rischio sono svolgere valutazioni delle capacità e delle vulnerabilità del modello (‡1003), avvalersi di un risk modelling robusto per informare le decisioni in merito a soglie di rischio (‡1004, ‡1005) e comprendere come i sistemi di IA vengono usati nella pratica al fine di valutare gli impatti sociali a valle (‡869, ‡904, ‡905, ‡1006). I processi di analisi e valutazione del rischio sono spesso considerati più propensi a identificare i rischi quando incorporano una revisione indipendente (‡1001, ‡1007), si basano su competenze trasversali tra settori (‡1008) e includono prospettive diverse provenienti da più ambiti e discipline, nonché dalle comunità interessate (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audit
  Gli audit sono revisioni formali delle prestazioni e degli impatti dei modelli di AI e/ o della conformità di un’organizzazione a standard, politiche e procedure, svolte internamente o da una parte esterna. La revisione di AI è un campo in crescita e esistono numerosi strumenti e pratiche per effettuare audit sui modelli di AI e sulle pratiche degli sviluppatori di modelli di AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Benchmark
  I benchmark sono test o metriche standardizzati, spesso quantitativi, utilizzati per valutare e confrontare le prestazioni dei sistemi di IA su un insieme fisso di attività progettate per rappresentare l’uso nel mondo reale (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metodo Bowtie
  Il metodo del papillon è un metodo ben noto per visualizzare dove è possibile aggiungere controlli per mitigare gli eventi di rischio. Esso fornisce una chiara distinzione tra gestione proattiva e reattiva del rischio (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metodo di Delphi
  Il metodo Delphi è una tecnica di presa di decisioni di gruppo che utilizza una serie di questionari per raccogliere il consenso da un panel di esperti (‡1020, ‡1021). È stato utilizzato per aiutare a esplorare possibili futuri con l’AI avanzata (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Prova sul campo
  Il collaudo sul campo valuta le prestazioni e l’impatto di un sistema AI in un ambiente operativo reale. Alcune ricerche enfatizzano il collaudo sul campo come complemento della valutazione del modello per valutare risultati e conseguenze nel mondo reale (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Valutazione dell’impatto
  Le valutazioni di impatto valutano i potenziali effetti di una tecnologia o di un progetto. Questo potrebbe includere la quantificazione, l’aggregazione e la prioritizzazione degli impatti. Il regolamento UE sull’Intelligenza Artificiale, ad esempio, richiede agli sviluppatori di sistemi di IA ad alto rischio di effettuare valutazioni d’impatto sui diritti fondamentali (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Valutazione del modello
  Le valutazioni del modello includono processi e test per valutare e misurare le prestazioni di un modello di AI su un determinato compito. Esistono numerose valutazioni di AI per valutare capacità e rischi diversi, incluse quelle per la sicurezza, la protezione e l’impatto sociale (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Valutazione del rischio probabilistica
  La valutazione del rischio probabilistica è una metodologia per valutare i rischi associati a sistemi o processi complessi che incorpora l'incertezza. È stata adattata per sistemi di AI avanzati (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teaming
  Il red-teaming è un esercizio in cui un gruppo di persone o sistemi automatizzati fingono di essere un avversario e attaccano i sistemi tecnologici di un'organizzazione allo scopo di identificare le vulnerabilità. Numerose aziende di AI hanno pratiche interne per il red-teaming di sistemi di AI (‡458, ‡1028). Il red-teaming può anche essere condotto da soggetti esterni alle aziende. Questi team affrontano sfide come un accesso limitato, ma possono anche far emergere insight distinti (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Matrici dei rischi
  Le matrici del rischio sono uno strumento visivo per aiutare a dare priorità ai rischi in base alla loro probabilità di verificarsi e al potenziale impatto (‡1027). Alcuni sviluppatori di AI includono matrici del rischio di base nei loro Frontier AI Safety Frameworks (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Soglie di rischio/ livelli di rischio
  Le soglie o i livelli di rischio sono limiti quantitativi o qualitativi che distinguono i rischi accettabili da quelli inaccettabili e attivano specifiche azioni di gestione del rischio quando vengono superati. Per l’AI a scopo generale, sono determinati da una combinazione di capacità, impatto, calcolo, diffusione e altri fattori (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolleranza al rischio
  La tolleranza al rischio si riferisce al livello di rischio che un’organizzazione è disposta ad accettare. Nell’IA, le tolleranze al rischio sono spesso definite in modo implicito tramite politiche e pratiche aziendali, mentre alcuni regimi regolatori definiscono esplicitamente i rischi inaccettabili e associano conseguenze legali (‡1032). Alcune aziende descrivono la propria tolleranza al rischio in termini di rischio marginale di un nuovo modello; vale a dire, la misura in cui un modello, controfattualmente, aumenta il rischio oltre quello già posto dai modelli esistenti o da altre tecnologie (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Casi di sicurezza
  Una safety case è un argomento strutturato, supportato da prove, che dimostra che un sistema è sufficientemente sicuro da poter essere operato in un determinato contesto. La letteratura recente (‡1037, ‡1038, ‡1039) ha esplorato le safety case per sistemi AI di frontiera e alcuni Frontier AI Safety Frameworks vi fanno riferimento (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Analisi della sicurezza del sistema
  L’analisi di sicurezza del sistema evidenzia le dipendenze tra i componenti e il sistema di cui fanno parte, al fine di anticipare come possano emergere pericoli a livello di sistema da guasti di componenti o processi, o da interazioni tra sottosistemi, fattori umani e condizioni ambientali. Le approcci applicate per i sistemi di IA nella letteratura includono l’analisi dei processi basata sulla teoria dei sistemi (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.2: Analisi/valutazione del rischio nella gestione del rischio dell’AI di scopo generale
>white|black||9|11|br Esempi di metodi per l’analisi/valutazione del rischio dell’AI, elencati in ordine alfabetico. Data la natura ancora iniziale della gestione del rischio dell’AI di uso generale, non tutti i metodi saranno adatti a ogni sviluppatore o responsabile dell’implementazione dell’AI.


>white|orangered|left|14|15.5|bb Gli strumenti comuni di analisi dei rischi includono benchmark e valutazioni dei modelli

I benchmark e le valutazioni del modello sono test standardizzati per valutare le prestazioni dei sistemi di AI a finalità generali su compiti specifici. I ricercatori hanno sviluppato un’ampia gamma di benchmark e valutazioni, incluse serie di domande a risposta multipla impegnative, problemi di ingegneria del software e compiti legati al lavoro in ambienti d’ufficio simulati (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Le valutazioni delle capacità dannose (‡715) vengono utilizzate per verificare se un modello o un sistema di AI a finalità generali possiede conoscenze o competenze particolarmente pericolose, come la capacità di aiutare negli attacchi informatici (vedi §2.1.3. Attacchi informatici).

Le decisioni altamente rilevanti prese da aziende e governi in merito al rilascio dei modelli si basano in parte su queste valutazioni (‡1050, ‡1051, ‡1052). Tuttavia, i benchmark variano in modo significativo per qualità e ambito (‡998, ‡1003), e può essere difficile valutarne la validità a causa di numerose carenze nelle pratiche di benchmarking (‡902, ‡909, ‡1003, ‡1053*). Ad esempio, i benchmark possono diventare “saturi” – quando i punteggi di molti modelli si avvicinano al punteggio massimo – il che significa che non distinguono più in modo efficace tra modelli. Inoltre, è sempre più probabile che i modelli identifichino alcuni compiti come valutazioni e mostrino comportamenti diversi da quelli che avrebbero su compiti simili in contesti di distribuzione, a causa della “consapevolezza situazionale” (vedi §2.2.2. Perdita di controllo). Infine, benchmark e valutazioni presentano limitazioni ben documentate: in particolare, non riescono a catturare i rischi associati all’uso di AI general-purpose in nuovi domini e per compiti nuovi, poiché le condizioni di test differiscono dall’uso nel mondo reale in vari gradi (‡913) (vedi §1.2. Current capabilities e §3.1. Technical and institutional challenges).

>white|orangered|left|14|15.5|bb Il red teaming consente valutazioni del rischio più specifiche per il dominio

Un altro metodo comune per valutare i rischi è il red-teaming. Un ‘red team’ è un gruppo di valutatori incaricato di cercare vulnerabilità, limitazioni o la possibilità di un uso improprio. Il red-teaming può essere specifico di un dominio e svolto da esperti del settore, oppure può essere aperto, per esplorare nuovi fattori di rischio. Per esempio, un red team potrebbe esplorare attacchi di ‘jailbreaking’ che aggirano le restrizioni di sicurezza del modello (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). In contrapposizione ai benchmark, un vantaggio fondamentale del red-teaming è che i red team possono adattare le proprie valutazioni al sistema specifico che viene testato. Per esempio, i red team possono progettare input personalizzati per identificare comportamenti peggiori, opportunità di uso dannoso e guasti imprevisti. Tuttavia, può richiedere accessi speciali ai modelli e può fallire nel mettere in evidenza classi importanti di rischi (‡999, ‡1028).

Importantly, l’assenza di rischi identificati non implica che tali rischi siano bassi: lavori precedenti mostrano che i bug spesso sfuggono al rilevamento, in particolare quando i red team hanno accesso o risorse limitati (‡1060). La ricerca ha inoltre messo in discussione la possibilità che il red-teaming possa produrre risultati affidabili e riproducibili (‡1061). La composizione del red team e le istruzioni fornite ai red-timer (‡1062), il numero di round di attacco (‡1063) e l’accesso del modello a strumenti (‡1064, ‡1065) possono influenzare in modo significativo gli esiti, inclusa la superficie di rischio coperta. Linee guida complete sul red-teaming mirano ad affrontare alcune di queste sfide (‡1066).

###@ Mitigazione del rischio

La mitigazione del rischio è il processo di definire le priorità, valutare e implementare controlli e contromisure per ridurre i rischi identificati. Gli esempi includono i controlli di accesso (‡991), il monitoraggio continuo (‡986) e gli impegni if-then (‡700). Mitigare il rischio solleva una domanda chiave: qual è il livello di rischio accettabile? I recenti framework e le policy aziendali hanno iniziato a formalizzare criteri di ‘accettazione del rischio’ (‡965, ‡1040). Tuttavia, stabilire soglie appropriate rimane difficile, soprattutto per i rischi con ampi impatti sociali (‡986, ‡1067). Al momento non esiste alcun meccanismo consolidato per convalidare le decisioni di accettazione del rischio prese dagli sviluppatori prima del rilascio (‡1005).

I metodi di mitigazione del rischio descritti nella Tabella 3.3 seguente sono adattabili e possono mitigare una gamma di rischi, inclusi alcuni rischi imprevisti. La tabella non include metodi di mitigazione tecnici come adversarial training, content filters e monitoraggio del chain-of-thought. Questi sono trattati in §3.3 Tecniche di salvaguardia tecniche e monitoraggio, nonché in tutto il Report nelle sezioni “Mitigations” per ciascun rischio in §2 Rischi.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Policy di utilizzo accettabile
  Una policy di utilizzo accettabile è un insieme di regole e linee guida per un uso responsabile, etico e legale dei modelli di AI. È comune che gli sviluppatori di AI pubblichino policy di utilizzo accettabile, nonché policy di utilizzo proibito, con i nuovi rilasci di modelli (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Controllo degli accessi/valutazione degli utenti
  I controlli di accesso includono l’uso di policy e regole per limitare l’accesso ai modelli di AI, ai dati e ai sistemi in base ai ruoli degli utenti, agli attributi e ad altre condizioni, al fine di prevenire usi non autorizzati, manomissioni o violazioni dei dati. Le aziende di AI spesso disabilitano gli account riscontrati come impegnati in attività criminali (‡486) e includono la verifica degli utenti e controlli Know-Your-Customer (KYC) per garantire che i modelli siano utilizzati solo da attori affidabili (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Specifiche di comportamento/modello
  Una specifica di comportamento dell'AI è un documento che definisce come dovrebbe comportarsi un modello di AI in varie situazioni. Serve come modello di riferimento per l'allineamento e la sicurezza dell'AI, guidando lo sviluppo, l'addestramento, la valutazione e gli output del modello. Diverse aziende di AI utilizzano documenti di specifica del modello e rendono pubbliche almeno alcune parti di essi (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio continuo
  Il monitoraggio continuo è il processo continuo, automatizzato, di osservazione, analisi e controllo dei sistemi di IA in uso, tracciandone le prestazioni e limitandone il comportamento per garantire affidabilità, efficacia e sicurezza. Sono disponibili numerosi strumenti per il monitoraggio continuo (‡1073*) nonché tecniche di supporto
Osservabilità dell'AI (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Difesa in profondità
  La difesa in profondità è l’idea secondo cui possono essere implementati più livelli di difesa indipendenti e sovrapposti, in modo tale che, se uno fallisce, gli altri rimangano comunque efficaci (‡1075, ‡1076). Più Frontier AI Safety Frameworks vi fanno riferimento (ad es. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio dell'ecosistema
  Questo è il processo di monitoraggio dell'ecosistema AI più ampio, inclusi il tracciamento del calcolo e dell'hardware, la provenienza del modello, la provenienza dei dati e i modelli di utilizzo. La letteratura di ricerca discute tale monitoraggio in relazione ai rischi derivanti dall'AI per scopi generali (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Impegni if-then
  Gli impegni if-then sono un insieme di protocolli tecnici e organizzativi e di impegni per gestire i rischi man mano che i modelli di AI diventano più capaci. Diversi sviluppatori di AI impiegano questo tipo di impegni come parte dei loro Frontier AI Safety Frameworks (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Line rosse o divieti
  Le linee rosse sono confini specifici espressi come capacità, impatto o tipi di utilizzo. Il concetto compare in dichiarazioni pubbliche e iniziative, nonché in divieti regolatori (‡1079, ‡1080, ‡1081). La letteratura evidenzia inoltre i limiti degli approcci basati sulle linee rosse, inclusi i problemi legati alla definizione di un consenso e alla loro applicabilità.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategie di rilascio e distribuzione
  Le strategie di rilascio e distribuzione per l'AI di uso generale possono includere l'uso di rilasci a fasi o l'accesso tramite API, così da rendere disponibili più opzioni di mitigazione in caso di uso improprio o danni imprevisti (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.3: Mitigazione del rischio nella gestione del rischio dell'AI a uso generale
>white|black||9|11|br Esempi di metodi per la mitigazione del rischio nell'AI elencati in ordine alfabetico. I metodi inclusi sono progettati per supportare la mitigazione del rischio per molti diversi tipi di rischio simultaneamente, inclusi i rischi derivanti da uso malevolo, i rischi derivanti da malfunzionamenti e i rischi sistemici. Data la natura ancora agli inizi della gestione del rischio per l'AI di scopo generale, non tutti i metodi saranno adatti a ogni sviluppatore o utilizzatore responsabile dell'AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Figura 3.5: Un 'diagramma del formaggio svizzero' che illustra l'approccio di difesa in profondità
>white|black||9|11|br Più livelli di difese possono compensare le carenze dei singoli livelli. Le tecniche attuali di gestione del rischio per l’IA presentano difetti, ma sovrapporle può offrire una protezione molto più solida contro i rischi. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Le strategie di difesa in profondità e di rilascio sono strumenti di mitigazione importanti

Un modello di ‘difesa in profondità’ può supportare la gestione del rischio dell’AI a scopo generale. In questo contesto, ‘difesa in profondità’ si riferisce a una combinazione di misure tecniche, organizzative e sociali applicate in diverse fasi di sviluppo e di distribuzione (Figura 3.5). Ciò significa creare livelli di salvaguardie indipendenti, così che, se uno strato fallisce, gli altri strati possano comunque prevenire i danni. Un esempio spesso citato di modello di difesa in profondità è l’insieme di misure preventive messe in atto per prevenire le malattie infettive. I vaccini, le mascherine e il lavaggio delle mani, tra le altre misure, possono ridurre in modo sostanziale il rischio di infezione se combinati, anche se nessuno di questi metodi è 100% efficace da solo (‡1083*). Per l’AI a scopo generale, la difesa in profondità includerà controlli che non sono sul modello di AI stesso, ma sull’ecosistema più ampio. Questo comprende (per esempio) controlli sui materiali necessari per eseguire un attacco biologico come i reagenti (‡1084, ‡1085). Tuttavia, le misure di difesa in profondità affrontano principalmente rischi connessi ad incidenti, malfunzionamenti e uso doloso, e possono avere un ruolo minore nella gestione dei rischi sistemici (vedi §3.5. Costruire la resilienza sociale).

La strategia di rilascio e distribuzione di un’azienda è un componente importante della mitigazione del rischio. Le decisioni su come i modelli vengono resi disponibili agli utenti possono influire in modo sostanziale sull’esposizione al rischio (‡1082). Le diverse opzioni di rilascio e distribuzione includono rilascio graduale a gruppi di utenti limitati, accesso tramite servizi online controllati (come le API) e l’uso di accordi di licenza e policy di uso accettabile che vietano legalmente determinate applicazioni dannose (‡176, ‡1086, ‡1087). §3.4. Open-weight models discute in modo più dettagliato come il rilascio dei pesi del modello influisca sui rischi.

###@ governance dei rischi

La governance del rischio è il processo mediante il quale le valutazioni, le decisioni e le azioni della gestione del rischio vengono collegate alla strategia e agli obiettivi di un’organizzazione o di un altro ente (‡1088, ‡1089). La Tabella 3.4 fornisce una panoramica delle tecniche di governance del rischio più comuni. Come mostrato nella Figura 3.4, la governance del rischio può essere intesa come il nucleo della gestione del rischio, poiché ne facilita il funzionamento efficace degli altri componenti. Fornisce responsabilità, trasparenza e chiarezza che supportano decisioni di gestione del rischio informate. La governance del rischio può includere pratiche quali la segnalazione degli incidenti (‡1090), l’assegnazione della responsabilità del rischio (‡965) e la protezione dei whistleblower (‡1091). In senso più ampio, la governance del rischio può includere indicazioni, framework, legislazione, regolamentazione, standard nazionali e internazionali, oltre a iniziative di formazione e di educazione. Uno scopo fondamentale della governance del rischio è stabilire politiche e meccanismi organizzativi che chiariscano come le responsabilità di gestione del rischio siano allocate in un’organizzazione o in un altro ente, al fine di supportare un’adeguata supervisione e responsabilità (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Documentazione
  Le pratiche di documentazione aiutano a tracciare informazioni chiave sui sistemi di IA, come i dati di addestramento, le scelte di progettazione, gli usi previsti, le limitazioni e i rischi. Le “model cards” e le “system cards”, che forniscono informazioni su come un modello o un sistema di IA è stato addestrato e valutato, sono esempi di best practice di documentazione dell’IA di primo piano (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Segnalazione di incidenti
  La segnalazione degli incidenti è il processo di documentare in modo sistematico e condividere i casi in cui lo sviluppo o l'implementazione dell'AI ha causato danni diretti o indiretti. Esistono diverse piattaforme che facilitano la segnalazione degli incidenti per l'AI (‡1096, ‡1097) e framework per facilitare una segnalazione degli incidenti dell'AI più efficace (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Framework di gestione del rischio
  I framework di gestione del rischio sono piani organizzativi per ridurre le lacune nella copertura del rischio, coordinare le varie attività di gestione del rischio e implementare controlli e contrappesi. I framework specifici per l’AI di uso generale (‡986, ‡1098) spesso richiamano le altre misure menzionate in questa sezione.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Registro dei rischi
  Un registro dei rischi è un repository di vari rischi, la loro prioritizzazione, i responsabili e i piani di mitigazione. Questi sono relativamente comuni in molti settori, inclusa la cybersecurity (‡1099), e a volte vengono utilizzati per soddisfare requisiti di conformità normativa.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Allocazione della responsabilità dei rischi
  L’assegnazione di ruoli e responsabilità per la gestione del rischio all’interno di un’organizzazione può strutturare la supervisione interna del processo decisionale (‡1002, ‡1093). Tali assetti si riflettono in alcuni framework di governance, incluso il Codice di Pratica per l’Intelligenza Artificiale a Scopo Generale dell’UE (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rapporti di trasparenza
  I rapporti di trasparenza descrivono le pratiche di gestione del rischio di un’azienda di IA divulgando pubblicamente alcune informazioni oppure condividendo documentazione con gruppi di settore o enti governativi. Ad esempio, numerose aziende di IA inviano rapporti di trasparenza Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Protezione per i segnalanti
  Poiché gran parte dello sviluppo dell’IA avviene in luoghi chiusi, alcuni framework di governance includono tutele per i segnalanti per consentire la divulgazione di potenziali rischi alle autorità (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.4: Governance del rischio nella gestione del rischio dell'AI di uso generale
>white|black||9|11|br Esempi di metodi per la governance del rischio dell'AI elencati in ordine alfabetico. I metodi inclusi sono progettati per supportare la governance del rischio per molti diversi tipi di rischio in modo simultaneo, inclusi i rischi derivanti da uso malevolo, i rischi da malfunzionamenti e i rischi sistemici. Data la natura ancora embrionale della gestione del rischio dell'AI a finalità generale, non tutti i metodi saranno adatti a ogni sviluppatore o utilizzatore dell'AI.


>white|orangered|left|14|15.5|bb La documentazione e la trasparenza sono componenti della governance del rischio

I meccanismi di documentazione e trasparenza istituzionale, insieme alle pratiche di condivisione delle informazioni, facilitano l’osservazione esterna e supportano gli sforzi per gestire i rischi associati all’AI per scopi generali (‡1101, ‡1102). È diventata pratica comune pubblicare i risultati dei test pre-deployment in un “model card” o in un “system card”, insieme a dettagli di base sul modello o sul sistema, incluso come è stato addestrato e quali sono le sue potenziali limitazioni (‡1094, ‡1095). Alcuni sviluppatori pubblicano anche report di trasparenza che includono dettagli sulle loro pratiche di gestione del rischio in modo più generale (‡1103). Altri elementi di documentazione e trasparenza includono il monitoraggio e la segnalazione degli incidenti (‡176, ‡1083*, ‡1103) e la condivisione delle informazioni, che può essere facilitata da terze parti come il Frontier Model Forum. Alcuni quadri normativi, come l’EU AI Act o la “California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53)” (‡1081, ‡1104), impongono in alcuni casi la condivisione di informazioni sui rischi dell’AI per scopi generali.

>white|orangered|left|14|15.5|bb L’impegno della leadership e gli incentivi modellano le pratiche di gestione del rischio

La cultura organizzativa, la struttura di leadership e gli incentivi influenzano gli sforzi di gestione del rischio in vari modi (‡1105). L’impegno della leadership e le strutture di incentivazione sono spesso rilevanti per come le politiche di gestione del rischio operano nella pratica. Alcuni sviluppatori dispongono di commissioni interne di decision-making che deliberano su come progettare, sviluppare e riesaminare nuovi sistemi di AI in modo sicuro e responsabile. Anche commissioni di supervisione e di consulenza, trust, o comitati di etica dell’AI possono fungere da meccanismi per offrire indicazioni sulla gestione del rischio e per l’oversight organizzativo (‡1092*, ‡1106, ‡1107, ‡1108). I ricercatori hanno sostenuto che le difficoltà legate all’autoregolamentazione volontaria implicano che audit, verifica e standardizzazione da parte di terzi potrebbero contribuire a rafforzare la gestione del rischio dell’AI a finalità generale (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Quadri di gestione del rischio organizzativo, trasparenza e reporting del rischio

Diverse nuove iniziative si concentrano su processi di gestione del rischio, documentazione e trasparenza. Nella sua forma attuale, il Codice di Condotta UE per l’IA di Scopo Generale (General-Purpose AI Code of Practice) funge da quadro volontario per guidare le pratiche di trasparenza, di copyright e di sicurezza e sicurezza informatica a supporto della conformità alle disposizioni dell’EU AI Act per l’IA di scopo generale (‡965). A dicembre 2025, più di due dozzine di aziende† hanno firmato. Il G7 Hiroshima AI Process (HAIP) Reporting Framework (‡1100) è il primo quadro internazionale per la rendicontazione pubblica volontaria delle pratiche di gestione del rischio organizzativo per sistemi di IA avanzati. Almeno 20 sviluppatori hanno pubblicato report pubblici di trasparenza che coprono l’identificazione del rischio, le metriche di valutazione, le strategie di mitigazione e i processi di sicurezza dei dati.

Gli sviluppatori di AI hanno adottato impegni volontari di trasparenza. In Cina, le promesse di 17 aziende cinesi di AI, coordinate dall’AI Industry Alliance of China, sono state pubblicate a dicembre 2024 (‡1113) e aggiornate nel 2025 (‡1114). Al May 2024 AI Seoul Summit in Corea del Sud, 16 sviluppatori di AI provenienti da più Paesi hanno firmato impegni volontari per pubblicare Frontier AI Safety Frameworks per i loro modelli e sistemi più capaci e per adottare pratiche di gestione del rischio in tutte le fasi di sviluppo e distribuzione del modello (‡1052).

    Nota † -- I firmatari aggiornati a dicembre 2025 includono: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing e WRITER.

>white|orangered|left|14|15.5|bb I framework di Frontier AI Safety sono diventati un approccio organizzativo di primo piano per la gestione del rischio dell'AI

Dall 2023, diversi sviluppatori di AI di frontiera hanno pubblicato volontariamente documenti che descrivono come intendono identificare e rispondere a gravi rischi provenienti dai loro sistemi più avanzati. Questi Frontier AI Safety Frameworks descrivono come uno sviluppatore di AI prevede di valutare, monitorare e controllare i propri modelli e sistemi di AI più avanzati prima e durante l’implementazione. Queste framework condividono molte somiglianze, ma differiscono in aspetti chiave (‡1115, ‡1116). La maggior parte si concentra su rischi associati a minacce chimiche, biologiche, radiologiche e nucleari (CBRN), capacità informatiche avanzate e comportamenti autonomi avanzati (‡1115, ‡1117). Una minoranza di framework affronta ulteriori domini di rischio come la discriminazione illegale su larga scala e lo sfruttamento sessuale di minori.

Diversi sviluppatori hanno aggiornato i loro framework nel 2025, aggiungendo nuove sezioni su manipolazione dannosa, rischio di disallineamento e replicazione e adattamento autonomi (‡1078, ‡1118). Sebbene molti framework descrivano approcci di gestione del rischio simili – inclusi threat modelling, red-teaming e valutazioni delle capacità pericolose – essi variano nelle definizioni di livelli di rischio e soglie, nella frequenza delle valutazioni, nei margini tra le valutazioni e le soglie e nella completezza dei loro impegni di mitigazione (ad esempio, se includono la cancellazione dei pesi del modello oppure solo la sospensione dello sviluppo) (‡1115, ‡1119). Vedere Tabella 3.5 per maggiori informazioni.

>white|orangered|left|14|15.5|bb Molte azioni nei Frontier AI Safety Framework basati su impegni if-then

Una parte fondamentale dei Frontier AI Safety Frameworks sono gli “impegni if-then”. Si tratta di protocolli condizionali che attivano risposte specifiche quando modelli AI e sistemi raggiungono soglie di capacità predefinite (‡1120). Ad esempio, un impegno if-then potrebbe affermare che, se viene rilevata la capacità di un modello di assistere in modo significativo i neofiti nella creazione e nel dispiegamento di armi CBRN, allora lo sviluppatore implementerà misure di sicurezza rafforzate, controlli di dispiegamento e monitoraggio in tempo reale (‡991*).

Nel 2025, diversi sviluppatori di AI hanno annunciato che nuovi modelli hanno attivato allarmi di preallarme o che non potevano escludere la possibilità che ulteriori valutazioni mostrassero che i modelli hanno superato soglie di capacità. Ciò li ha indotti ad applicare salvaguardie rafforzate come misura precauzionale (‡7, ‡33, ‡1121*). I Frontier AI Safety Frameworks richiedono comunemente una valutazione iniziale delle capacità prima della mitigazione del rischio, nonché un’analisi del rischio residuo o un safety case, spesso basati su red-teaming, dopo la mitigazione. Vedi Tabella 3.5 per informazioni dettagliate.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Framework di preparazione 2 (‡1078*)
  Rischi coperti:
1. Capacità biologiche e chimiche
2. Capacità di cybersecurity
3. capacità di auto-miglioramento dell'AI
  Livelli di rischio o equivalenti e relative salvaguardie:
- Alto: Potrebbe amplificare i percorsi esistenti verso danni gravi (Richiede controlli di sicurezza e salvaguardie)
- Critico: potrebbe introdurre percorsi nuovi e senza precedenti verso gravi danni (interrompere ulteriori sviluppi fino a quando le misure di salvaguardia specificate e gli standard dei controlli di sicurezza non raggiungono un livello Critico)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Politica di scalabilità responsabile 2.2 (‡991*)
  Rischi coperti:
1. Armi CBRN
2. Ricerca e sviluppo (AI R&D) sull'IA autonoma
3. Operazioni informatiche (sotto valutazione)
  Livelli di rischio o equivalenti e misure di salvaguardia associate:
  Livelli di Sicurezza dell'AI (ASL)
- ASL-1: Nessun rischio catastrofico significativo
- ASL-2: Segnali precoci di capacità pericolose (i modelli devono soddisfare gli standard di distribuzione e sicurezza ASL-2)
- ASL-3: Rischio di uso improprio catastrofico sostanzialmente aumentato (i Modelli devono soddisfare gli standard di Distribuzione e/ o Sicurezza ASL-3)
- ASL-4+: Classificazioni future (non ancora definite)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Rischi coperti:
1. Uso improprio
    a. CBRN
    b. Cyber
    c. Manipolazione dannosa
2. Ricerca e sviluppo nel machine learning
3. Disallineamento/ ragionamento strumentale
  Livelli di rischio o equivalente e relative misure di salvaguardia:
  Livelli di capacità critici
    Livelli di capacità per i quali, in assenza di misure di mitigazione (casi di sicurezza per le distribuzioni e mitigazioni di sicurezza allineate ai livelli di sicurezza RAND 2, 3 o 4 (‡1122)), i modelli o i sistemi di AI possono presentare un rischio accresciuto di gravi danni. I livelli di capacità includono le «valutazioni di allerta precoce», con soglie di «avviso» specifiche
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Framework di Frontier AI 1.1 (‡990*)
  Rischi coperti:
1. Sicurezza informatica
2. Rischi chimici e biologici
  Livelli di rischio o equivalenti e relative misure di salvaguardia:
  Livelli delle soglie di rischio
- Moderato (rilascio con misure di sicurezza e mitigazioni appropriate)
- igh (non rilasciare)
- Critico (interrompere lo sviluppo)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Framework di Sicurezza per Modelli Frontier (‡1123*)
  Rischi coperti:
1. proliferazione di armi CBRN
2. Operazioni cibernetiche offensive
3. Ricerca e sviluppo automatizzata con l’IA
  Livelli di rischio o equivalenti e relative misure di salvaguardia:
  Soglie critiche di capacità
    Capacità del modello che hanno il potenziale di causare danni significativi alla collettività in caso di uso improprio. (Se le soglie sono soddisfatte o superate, il modello non verrà distribuito pubblicamente senza misure di mitigazione del rischio adeguate)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Framework di Governance per Frontier (‡1124*)
  Rischi coperti:
1. Armi CBRN
2. Operazioni cibernetiche offensive
3. Autonomia avanzata (inclusa la ricerca e sviluppo di IA)
  Livelli di rischio o equivalenti e relative salvaguardie:
  Livelli di rischio
- Basso o Medio (Distribuzione consentita in linea con i requisiti del Programma di AI Responsabile)
- Alta o Critica (ulteriore revisione e mitigazioni
(required)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Valutazione del rischio AI di Frontier (‡1029*)
  Rischi coperti:
1. Offesa informatica
2. CBRN
3. Persuasione e manipolazione
4. Discriminazione illecita su larga scala
  Livelli di rischio o equivalenti e misure di salvaguardia associate:
  Soglie di rischio – punteggi di rischio del modello (MR)
- MR1 o MR2 (i risultati di valutazione sono documentati dai team di ingegneria)
- MR3 (Le misure di mitigazione del rischio e i risultati delle valutazioni sono documentati dai team di ingegneria e periodicamente riesaminati)
- MR4 (È necessario completare una valutazione dettagliata del rischio e ottenere l'approvazione del responsabile della business unit)
- MR5 (È necessario completare una valutazione dettagliata del rischio e farla approvare da un comitato indipendente, ad esempio la commissione di etica dell’AI di NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Framework per Modelli di Frontiera di AI Sicura (‡1125*)
  Rischi coperti:
1. Uso dannoso (ad es. malware, sfruttamento sessuale minorile)
2. Danno in uso ordinario, non dannoso, ad esempio output che comportano un risultato discriminatorio illegale o la generazione di codice non sicuro
  Livelli di rischio o equivalenti e relative misure di salvaguardia:
  Probabilità e Gravità del Danno nel Contesto
- Basso
- Medio
- Alto
- Molto Alto
    (Le misure di mitigazione dei rischi e i controlli di sicurezza sono in atto per tutti i sistemi e processi; ulteriori mitigazioni devono essere adattate al sistema di IA e al caso d’uso in cui un modello viene distribuito)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Policy di prontezza per l'AGI (‡1127*)
  Rischi coperti:
1. Offesa informatica
2. Ricerca e sviluppo automatizzata con l’IA
3. replicazione autonoma e adattamento
4. Assistenza per armi biologiche
  Livelli di rischio o equivalenti e salvaguardie associate:
  Soglie critiche di capacità
    Soglie quantitative sui benchmark di capacità (se superate, condurre valutazioni di capacità pericolose, misure di sicurezza delle informazioni e mitigazioni di distribuzione, oppure interrompere lo sviluppo)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: Politica di Readiness per AGI (‡1127*)
  Rischi coperti:
1. Offesa informatica
2. Ricerca e sviluppo automatizzata con l’IA
3. Replicazione autonoma e adattamento
4. Assistenza per armi biologiche
  Livelli di rischio o equivalente e misure di salvaguardia associate:
  Soglie critiche di capacità
    Soglie quantitative sui benchmark delle capacità (se superate, condurre valutazioni di capacità pericolose, misure di sicurezza delle informazioni e mitigazioni di distribuzione, oppure interrompere lo sviluppo)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Framework di Sicurezza dell'AI (‡1128*)
  Rischi coperti:
1. Perdita di controllo
2. Uso improprio (ad es. weaponizzazione di agenti biochimici
  Livelli di rischio o equivalenti e relative misure di salvaguardia:
  Livelli di rischio
- Rischio basso (Distribuire sistemi di IA, ma eseguire monitoraggio successivamente per gestire i rischi)
- Rischio identificato (O utilizzare solo sistemi di OpenAI per utenti autorizzati per mitigare i rischi, oppure rimandare il deployment finché non vengono adottate ulteriori misure di sicurezza, a seconda del caso d’uso)
- Rischio alto (Non distribuire sistemi di AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Framework di Sicurezza per l'AI di Frontiera (‡1129*)
  Rischi coperti:
1. Minacce biologiche
2. Cybersecurity offensiva
3. Funzionamento autonomo e manipolazione avanzata
  Livelli di rischio o equivalenti e relative salvaguardie:
  Livelli di rischio
- Livello 1 (Protezione di base per rischi minimi e potenziale rilascio open source)
- Livello 2 (monitoraggio in tempo reale, filtraggio dei prompt, rilevamento di anomalie comportamentali, controlli di accesso, red-teaming e simulazioni avversarie)
- Livello 3 (garanzie avanzate incluse red teaming, distribuzioni a fasi, test avversariali, crittografia, controlli di accesso multi-parte e architettura zero-trust)
- Livello 4 (massimi protocolli di sicurezza per modelli ad alto impatto e massime misure di sicurezza)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.5: Framework di Frontier AI Safety
>white|black||9|11|br Il primo insieme di Frontier AI Safety Frameworks rilasciato da un sottoinsieme degli sviluppatori di AI che hanno firmato le Frontier AI Safety Commitments. I framework coprono rischi simili (con leggere variazioni) e impiegano diversi livelli di rischio e approcci di risk management.


>white|orangered|left|14|15.5|bb L'efficacia dei Framework di Sicurezza per l'AI di Frontiera è incerta

I Frontier AI Safety Frameworks possono fungere da strumenti di gestione del rischio in condizioni specifiche e per determinate categorie di rischio che presentano una credibile via verso il danno (‡1117). Allo stesso tempo, diverse analisi discutono questioni relative alla loro chiarezza e alla loro portata (‡111, ‡986) e sulla robustezza delle soglie di capacità e rischio dell'AI (‡1031, ‡1130). I framework esistenti tendono a concentrarsi su una parte dei domini di rischio. Di conseguenza, alcuni rischi di rilievo, come la sorveglianza illecita (‡1131, ‡1132) e le immagini intime non consensuali (‡287), ricevono meno enfasi. A differenza di approcci di gestione del rischio di altri settori, come l'aviazione o l'energia nucleare (‡1133*), i Frontier AI Safety Frameworks in genere non utilizzano soglie esplicite di rischio di tipo quantitativo (‡1134).

Le valutazioni esterne della conformità degli sviluppatori ai loro Frontier AI Safety Frameworks finora restano limitate, in parte perché la maggior parte dei framework è recente, le informazioni pubblicamente disponibili sono scarse e non esistono audit esterni standardizzati. La loro efficacia sarà inoltre influenzata da quanto bene – e in che misura – gli impegni vengono implementati nella pratica. Da soli, questi framework potrebbero non garantire una gestione efficace del rischio, poiché il loro impatto pratico dipende da quanto bene e in che misura vengono implementati. Ad oggi, non si allineano pienamente agli standard internazionali di gestione del rischio (‡1135). Uno studio su impegni volontari precedenti ha riscontrato un adempimento non uniforme tra le misure, suggerendo che l’adesione agli impegni volontari probabilmente varierà tra le aziende e i domini (‡1109).

Nel loro insieme, i Frontier AI Safety Frameworks rappresentano la forma più dettagliata di gestione volontaria del rischio organizzativo attualmente in uso, ma variano in modo sostanziale per ambito, soglie e applicabilità.

###@ Iniziative di regolamentazione e governance

>white|orangered|left|14|15.5|bb Diverse giurisdizioni hanno introdotto leggi con requisiti di trasparenza

Diversi primi approcci regolatori introducono requisiti legali intesi ad aumentare la standardizzazione e la trasparenza nella gestione del rischio. Il Regolamento UE sull’IA (AI Act), entrato in vigore nel 2024, stabilisce requisiti relativi alla trasparenza, al copyright e alla sicurezza per i modelli di IA per finalità generiche. Nel 2025, il Codice di Pratica UE per l’IA per Finalità Generiche è stato pubblicato per supportare la conformità a tali obblighi fornendo indicazioni sulla documentazione del modello e sul copyright, nonché – per i modelli più avanzati – pratiche di gestione del rischio quali valutazioni, assessment del rischio e mitigazione, sicurezza delle informazioni e segnalazione di incidenti gravi (‡965).

Altri esempi di nuovi requisiti regolatori includono la Legge quadro della Corea del Sud sulla sviluppo dell’Intelligenza Artificiale e l’istituzione della fiducia, che introduce requisiti per i sistemi di IA «ad alto impatto» nei settori critici (‡1136), e il disegno di legge della California SB 53, che stabilisce requisiti di trasparenza su framework di sicurezza e segnalazione degli incidenti (‡1104). Considerato quanto recentemente siano stati introdotti questi requisiti, è troppo presto per valutare in dettaglio in che modo influenzeranno le pratiche di gestione del rischio o i risultati di rischio effettivi.

>white|orangered|left|14|15.5|bb Le iniziative di governance più ampie offrono indicazioni volontarie

Diversi quadri di governance regionali e interregionali articolano ora aspettative condivise per la gestione dei rischi derivanti dall’AI a scopo generale, fornendo indicazioni non vincolanti per i responsabili politici e per le organizzazioni. Il China’s AI Safety Governance Framework 2.0, pubblicato nel 2025, fornisce indicazioni strutturate sulla classificazione dei rischi e sulle contromisure lungo l’intero processo di sviluppo e impiego dell’AI (‡1137). Gli Stati membri dell’ASEAN hanno pubblicato l’‘ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)’, che fornisce indicazioni sulla governance e sull’etica dell’AI a scopo generale ed è inteso a supportare una maggiore allineamento delle politiche tra gli Stati membri dell’ASEAN (‡1138). Inoltre, iniziative guidate da esperti come il Singapore Consensus, sviluppato da scienziati di AI provenienti da più Paesi, delineano priorità di ricerca per la sicurezza dell’AI a scopo generale in ambiti quali la valutazione, lo sviluppo e il controllo dei rischi (‡690).

###@ Aggiornamenti

Dalla pubblicazione dell’ultimo Rapporto (gennaio 2025), il panorama della gestione del rischio per l’AI a finalità generale si è evoluto, con la pubblicazione di nuove risorse come il Codice di Pratica per l’AI a finalità generale dell’UE, il G7 HAIP Reporting Framework, il China’s national AI Safety Governance Framework 2.0 e vari Frontier AI Safety Frameworks da parte di sviluppatori di AI. Queste iniziative descrivono approcci e pratiche adottate dagli sviluppatori di AI per gestire i rischi associati a sistemi di AI a finalità generale (‡1115). Esiste una notevole variabilità tra i Frontier AI Safety Frameworks e tra i report di trasparenza HAIP (‡1103), che riflette differenze nelle prassi organizzative, nella prioritizzazione dei rischi e nella fase iniziale dell’ecosistema di gestione del rischio per l’AI a finalità generale. Un ecosistema affidabile in cui diversi attori dell’AI contribuiscono a prassi complementari di gestione del rischio lungo l’intero ciclo di vita può contribuire a una gestione efficace del rischio (‡690).

###@ lacune di evidenza

Mancano evidenze su: come misurare la severità, la prevalenza e la tempistica dei rischi emergenti; in che misura tali rischi possano essere mitigati in contesti reali; e come incoraggiare o imporre in modo efficace l’adozione della mitigazione tra diversi attori. Sono necessarie ulteriori ricerche per comprendere quanto siano diffusi i diversi rischi e in che misura varino tra le diverse regioni del mondo, in particolare per regioni come Asia, Africa e America Latina, che stanno digitalizzandosi rapidamente. Poiché ai modelli di AI viene conferita un crescente livello di autonomia e autorità e lo stato della scienza sui rischi dell’AI a finalità generale avanza, anche gli approcci di risk management dovranno evolvere (‡639, ‡1139).

Alcune mitigazioni del rischio stanno diventando sempre più popolari (‡690, ‡956), ma è necessaria ulteriore ricerca per comprendere quanto siano robuste, nella pratica, le mitigazioni e le salvaguardie del rischio per comunità e attori dell’AI diversi (incluse le piccole e medie imprese). L’accesso maggiore ai dati su implementazioni e utilizzi reali dei modelli è rilevante per tali valutazioni. Inoltre, gli sforzi di risk management attualmente variano in modo molto marcato tra le principali aziende di AI. È stato sostenuto che gli incentivi dei sviluppatori non siano ben allineati con una valutazione e gestione rigorosa del rischio (‡934). Permane ancora un divario di evidenze su in che misura vengano rispettati diversi impegni volontari, quali ostacoli le aziende incontrino nel rispettarli pienamente e come stiano integrando i Frontier AI Safety Frameworks nelle più ampie pratiche di risk management dell’AI.

###@ Sfide per i responsabili politici

Le principali sfide includono capire come dare priorità ai diversi rischi posti dall'AI di uso generale, chiarire quali attori siano meglio posizionati per mitigarli e comprendere gli incentivi e i vincoli che modellano le loro azioni. Le evidenze indicano che i responsabili delle politiche pubbliche dispongono attualmente di accesso limitato alle informazioni su come gli sviluppatori e i fornitori di AI stanno testando, valutando e monitorando i rischi emergenti, e sull'efficacia di diverse pratiche di mitigazione (‡1140). Ricercatori e responsabili delle politiche pubbliche hanno discusso iniziative di trasparenza e una segnalazione degli incidenti più sistematica come possibili modi per informare la definizione delle priorità del rischio, promuovere la fiducia e incentivare lo sviluppo responsabile (‡957). Nella pratica, la gestione del rischio coinvolge più attori lungo la catena del valore dell'AI – come provider di dati e di cloud, sviluppatori di modelli e piattaforme di hosting dei modelli – ciascuno con opportunità distinte per valutare e gestire diversi rischi (‡1141). La condivisione limitata delle informazioni tra questi attori rende difficile determinare quali rischi siano più probabili o più impattanti, soprattutto quando si considerano gli effetti sociali a valle.

