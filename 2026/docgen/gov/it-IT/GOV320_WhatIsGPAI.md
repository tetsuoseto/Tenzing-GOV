###@ Quali sono i sistemi di intelligenza artificiale per scopi generici?

I sistemi di AI generici per scopi generali sono programmi software che imparano modelli da grandi quantità di dati, permettendo loro di svolgere una varietà di compiti invece di essere specializzati per una singola funzione o un singolo dominio (vedi Tabella 1.1). Per creare questi sistemi, gli sviluppatori di AI eseguono un processo articolato in più fasi che richiede risorse computazionali considerevoli, dataset di grandi dimensioni e competenze specialistiche (vedi Tabella 1.2). Le risorse computazionali (spesso abbreviate in “compute”) sono necessarie sia per sviluppare sia per distribuire i sistemi di AI e includono chip per computer specializzati, oltre al software e all’infrastruttura necessari per farli funzionare.† Poiché vengono addestrati su dataset grandi e diversificati, i sistemi di AI generici per scopi generali possono svolgere molti compiti diversi, come riassumere testo, generare immagini o scrivere codice per computer. Questa sezione spiega come vengono realizzati i sistemi di AI generici per scopi generali, quali sono i modelli di “ragionamento” e come le decisioni di policy modellano lo sviluppo dei sistemi di AI generici per scopi generali.

    Nota † -- Il termine ‘compute’ può riferirsi anche a una misura del numero di calcoli che un processore può eseguire (tipicamente misurata in operazioni in virgola mobile al secondo) oppure, in modo specifico, all’hardware (come le unità di elaborazione grafica) che esegue tali calcoli.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistemi di linguaggio
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Comando A (‡3*)
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
###@ Generatori di immagini
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Generatori video
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Vedo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistemi di robotica e navigazione
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Predittori di classi diverse di strutture biomolecolari
- AlphaFold 3 (‡27)
- Amplify (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Agenti AI
- AlphaEvolve (‡31*)
- Agente ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Lo Scienziato di AI-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 1.1: Tipi di AI di uso generale
>white|black||9|11|br Esistono diversi tipi di AI generica. In questa Relazione, i modelli in grado di predire informazioni strutturali per classi diverse di molecole sono considerati “AI generica” perché possono essere adattati a una varietà di compiti. Ad esempio, i modelli addestrati per predire la struttura proteica sono applicabili a una varietà di altri compiti, come predire interazioni proteiche, predire siti di legame di piccole molecole e predire e progettare peptidi ciclici (‡40).


>white|orangered|left|13|15|bb L'apprendimento profondo è fondamentale per l'AI di scopo generale

I ricercatori costruiscono modelli di AI generici tramite un processo chiamato "deep learning", che addestra i modelli a imparare da esempi (‡41). A differenza dell’ingegneria del software, i modelli di deep learning imparano a svolgere compiti dai dati, invece di fare affidamento su istruzioni scritte a mano. Elaborando grandi quantità di dati, come immagini, testo o audio, questi modelli scoprono i modi per rappresentare tali dati, creando rappresentazioni interne di pattern (come forme, associazioni tra parole o strutture dei suoni) che aiutano il modello a riconoscere relazioni e a generare output allineati all’obiettivo di addestramento. Successivamente usano queste rappresentazioni interne apprese come caratteristiche astratte per analizzare nuovi dati simili e generare output nello stesso stile. Ad esempio, un modello di AI generico addestrato su un numero sufficiente di esempi di poesia inglese romantica del XIX secolo può riconoscere nuove poesie in quello stile e produrre nuovo materiale in uno stile simile.

A un livello più granulare, l’apprendimento profondo funziona elaborando i dati attraverso livelli di nodi interconnessi per l’elaborazione delle informazioni. Questi nodi sono spesso chiamati ‘neuroni’ perché sono ispirati in modo approssimativo ai neuroni presenti nei cervelli biologici (‘reti neurali’) (Figura 1.1) (‡42). Poiché l’informazione fluisce da un livello di neuroni al successivo, il modello trasforma progressivamente i dati in rappresentazioni sempre più astratte, come gruppi di feature apprese – pattern che il modello ha scoperto automaticamente nei dati, anziché quelli codificati a mano. Ad esempio, in un modello di elaborazione delle immagini, i primi livelli potrebbero imparare a rilevare feature semplici come bordi o forme di base, mentre i livelli più profondi combinano queste feature per individuare pattern più complessi, come volti o oggetti.

Le caratteristiche a tutti i livelli vengono scoperte tramite il processo di ottimizzazione che definisce la procedura di training. Durante l’addestramento, quando il modello commette errori, gli algoritmi di deep learning regolano la forza delle varie connessioni tra i neuroni per migliorare le prestazioni del modello. La forza di ogni connessione tra i nodi è spesso chiamata “peso” (weight). Questo approccio a livelli conferisce al deep learning il suo nome.

Il deep learning si è dimostrato molto efficace nel consentire ai sistemi di IA di svolgere compiti che in precedenza erano considerati difficili per i sistemi computazionali tradizionali programmati a mano e per altri metodi di IA simbolica o basati su regole più antichi. La maggior parte dei modelli di IA generali all’avanguardia si basa ora su una specifica architettura di rete neurale nota come “transformer” (‡43, ‡44). I transformer utilizzano un meccanismo di “attenzione” (‡45) che aiuta il modello a concentrarsi sulle parti più rilevanti dei dati di input quando elabora le informazioni, ad esempio determinando quali parole in una frase siano più importanti per comprenderne il significato. Questo particolare modo di costruire i modelli ha portato a miglioramenti significativi nella traduzione (‡43), nell’elaborazione del linguaggio naturale (‡46), nel riconoscimento delle immagini (‡47) e nel riconoscimento vocale (‡48, ‡49), arrivando infine allo sviluppo dei modelli più avanzati di oggi.

![fig1.1](images/fig1.1_neural_network.png)

##### Figura 1.1: Una rappresentazione illustrativa di una “rete neurale”
>white|black||9|11|br I modelli di AI generica odierni si basano su queste reti, che sono ispirate in modo approssimativo ai cervelli biologici. Reti diverse hanno dimensioni e architetture diverse. Tuttavia, tutte sono composte da unità di elaborazione delle informazioni connesse chiamate 'neuroni', in cui la forza delle connessioni tra i neuroni è chiamata 'pesi'. I pesi vengono aggiornati tramite l’addestramento con grandi quantità di dati. Fonte: International AI Safety Report 2025 (‡50) (modificato).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figura 1.2: Una rappresentazione schematica delle fasi dello sviluppo dell’AI a scopo generale
>white|black|left|9|11|br Rapporto internazionale sulla sicurezza dell’IA 2026.


>white|orangered|left|13|15|bb L'AI generica viene sviluppata per fasi

Sviluppare un sistema di AI generico comporta più fasi, dall’addestramento iniziale del modello fino al monitoraggio post-deployment e agli aggiornamenti (Figura 1.2). In pratica, questi passaggi spesso si sovrappongono in modo iterativo. Ciascuna fase richiede diversi input di risorse (ad es. dati, lavoro, compute) e tecniche diverse, e talvolta vengono svolte da sviluppatori diversi (Figura 1.2 e Tabella 1.2).

Ad esempio, la pre-formazione del modello generalmente richiede grandi quantità di calcolo e di dati, rendendo questa fase particolarmente sensibile a politiche che incidono sull’accesso alle risorse computazionali o ai dati di addestramento (‡51, ‡52). Analogamente, la curatela dei dati e alcuni metodi di fine-tuning del modello attualmente comportano grandi quantità di lavoro umano per l’etichettatura iniziale dei dati (‡53). Pertanto, questa fase è sensibile a cambiamenti nei costi della manodopera, nelle policy delle piattaforme o nelle normative che incidono sugli accordi di contrattazione transfrontaliera.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Raccolta e curation dei dati
> 
  Prima di addestrare un modello di AI generica, gli sviluppatori e gli operatori dei dati raccolgono, puliscono, curano e standardizzano i dati grezzi di addestramento in un formato da cui il modello possa apprendere. Questo può essere un processo che richiede molta manodopera. I dataset di addestramento alla base dei modelli all’avanguardia comprendono un numero enorme di esempi provenienti da tutto il web.
  I team spesso sviluppano metodi di filtraggio sofisticati per ridurre i contenuti dannosi, eliminare i dati duplicati e migliorare la rappresentazione tra argomenti e fonti diversi (‡54, ‡55). La curatela dei dati può anche aiutare a ridurre le violazioni del copyright e della privacy, rimuovere esempi che includono conoscenze pericolose, gestire più lingue e migliorare la documentazione per la provenienza dei dati (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Pre-addestramento (prima fase dell’addestramento)

  Durante il pre-addestramento, gli sviluppatori forniscono ai modelli enormi quantità di dati diversi per instillare una base ampia di informazioni e una comprensione contestuale. Questo processo produce un “modello di base”. Si tratta di un processo altamente intensivo in termini di dati e di calcolo.

  Durante il pre-addestramento, i modelli vengono esposti a miliardi o trilioni di esempi di contenuti come immagini, testi o audio. Attraverso questa esposizione, il modello scopre gradualmente caratteristiche astratte per rappresentare i dati e impara come tali caratteristiche siano correlate, il che gli consente di dare senso a nuovi input nel relativo contesto. Questo processo di pre-addestramento richiede settimane o mesi (‡59) e utilizza decine o centinaia di migliaia di unità di elaborazione grafica (GPU) o unità di elaborazione dei tensori (TPU) (‡60) – chip informatici specializzati progettati per elaborare rapidamente molte di queste elaborazioni. Alcuni sviluppatori eseguono il pre-addestramento con il proprio calcolo, mentre altri utilizzano risorse fornite da provider di calcolo specializzati.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Post-formazione e fine-tuning (seconda fase di addestramento)

  ‘Post-training’ raffina ulteriormente il modello di base per ottimizzarlo per una specifica applicazione. Si tratta di un processo moderatamente oneroso dal punto di vista computazionale e altamente dispendioso in termini di lavoro. Uno spostamento verso l’uso di ‘synthetic data’ – informazioni generate artificialmente che imitano i dati del mondo reale ma sono create tramite algoritmi o simulazioni – sta contribuendo a rendere questa fase meno dispendiosa in termini di lavoro.
  La post-training include varie tecniche di fine-tuning e altre modifiche. Il ‘fine-tuning supervisionato’ implica un ulteriore addestramento di un modello già addestrato su dataset specifici per migliorare le prestazioni del modello in quel dominio (‡61, ‡62). Per esempio, un modello general-purpose potrebbe essere ulteriormente addestrato su una grande raccolta di immagini radiologiche. Il ‘reinforcement learning’ (RL) implica il miglioramento delle prestazioni del modello ‘ricompensandolo’ (fornendo feedback positivo) per output desiderabili e ‘penalizzandolo’ (fornendo feedback negativo) per output indesiderabili. Ha due sottocategorie principali. Il ‘reinforcement learning from human feedback’ implica il fatto di ricompensare gli output che sono in linea con le preferenze umane e penalizzare quelli che non lo sono, in base al feedback umano (‡63, ‡64*). Il ‘reinforcement learning with verifiable rewards’ (RLVR) viene utilizzato per migliorare le prestazioni del modello in compiti che richiedono correttezza fattuale, come la generazione di codice o di matematica. Gli sviluppatori in genere alternano tra l’applicazione di tecniche di post-training e l’esecuzione di test fino a quando i risultati mostrano che il modello soddisfa le specifiche desiderate.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integrazione di sistema

  Gli sviluppatori combinano uno o più modelli AI generici con altri componenti per creare un’«AI system» pronto all’uso. GPT-5 (ad esempio) è un modello AI generico che elabora testo, immagini e audio, mentre ChatGPT è un sistema AI generico che combina diversi modelli di dimensioni e capacità differenti con un’interfaccia di chat, l’elaborazione dei contenuti, l’accesso al Web e l’integrazione delle applicazioni per creare un prodotto funzionale.
  In aggiunta a rendere operativi i modelli di AI, i componenti aggiuntivi in un sistema di AI mirano anche a migliorare capacità, utilità e sicurezza. Per esempio, un sistema potrebbe includere un filtro che rileva e blocca input o output del modello che contengono contenuti dannosi (‡65*). Gli sviluppatori stanno anche sempre più usando lo “scaffolding” – software aggiuntivo costruito attorno a modelli di AI di uso generale che consente loro di pianificare in anticipo, perseguire obiettivi e interagire con il mondo (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Distribuzione e rilascio
  Il deployment è il processo di rendere il sistema AI integrato disponibile per l’uso previsto. Sviluppatori e operatori di deployment implementano i sistemi AI in applicazioni, prodotti o servizi del mondo reale. Gli sviluppatori possono effettuare il deployment dei sistemi AI internamente (per il proprio utilizzo) o esternamente (per clienti privati o per uso pubblico). Quando si effettuano deployment di sistemi AI esternamente, le aziende spesso forniscono agli utenti l’accesso tramite interfacce utente online o interfacce di programmazione applicativa (API) che consentono agli utenti di accedere ed eseguire il sistema. Ad esempio, una società potrebbe progettare un chatbot personalizzato per il servizio clienti, alimentato da un altro sistema AI generico di un’altra società.
  “Distribuzione di un sistema AI” si riferisce al rendere un modello disponibile per l’uso nel mondo reale con strumenti e interfacce integrate, mentre “rilascio del modello” implica rendere il modello di base accessibile ad altri, sia come open-weight (parametri scaricabili) sia come closed-weight (solo accesso via API). Vedi §3.4. Modelli open-weight.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Monitoraggio post-deployment e aggiornamenti

  Gli sviluppatori spesso raccolgono e analizzano il feedback degli utenti, tracciano l’impatto e le metriche di performance e apportano miglioramenti iterativi per affrontare i problemi individuati durante l’uso nel mondo reale (‡67). I miglioramenti vengono effettuati aggiornando le integrazioni del sistema, spesso tramite fine-tuning continuo e fornendo ai modelli l’accesso a basi di dati esterne di (recenti) fatti. Questo consente ai grandi modelli di IA di rimanere aggiornati senza ripetere l’intero processo di pre-addestramento (‡68*). Questo permette alle capacità di accumularsi attraverso successive fasi di training mantenendo la stabilità e riducendo i costi computazionali.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 1.2: Fasi di sviluppo dell'AI a scopo generale
>white|black||9|11|br Ad ogni fase di sviluppo dell’AI di uso generale, il modello di AI viene migliorato per l’uso a valle e, infine, distribuito come sistema di AI completamente integrato, monitorato e aggiornato.


>white|orangered|left|13|15|bb I sistemi di ragionamento generano «catene di pensiero» durante l’inferenza per migliorare le prestazioni

L’inferenza avviene quando qualcuno utilizza il modello di AI dopo che è stato addestrato. Per esempio, l’inferenza si verifica quando una persona chiede a un sistema di AI di pianificare un viaggio e il modello che sta dietro ad esso si basa su aspetti pertinenti di ciò che ha appreso riguardo geografia, trasporti e cucina per generare un itinerario.

Nell’ultimo decennio, i progressi nelle capacità dell’AI sono in gran parte derivati da training di dimensioni maggiori; cioè, dall’aumento della quantità di compute utilizzata per addestrare un modello di AI. Recentemente, tuttavia, i ricercatori hanno ottenuto più risultati consentendo ai modelli di elaborare informazioni per periodi più lunghi e addestrandoli a produrre passaggi di ragionamento espliciti mentre completano un compito (‡69*, ‡70). I sistemi di AI che funzionano in questo modo sono chiamati ‘sistemi di ragionamento’, e le spiegazioni intermedie che attraversano mentre risolvono un problema o rispondono a una domanda sono chiamate ‘catene di pensiero’. I sistemi di ragionamento richiedono più risorse computazionali al momento dell’uso per generare queste sofisticate catene di pensiero (‡71, ‡72, ‡73, ‡74), e più risorse durante l’addestramento affinché imparino a ragionare meglio. Nella pratica, queste capacità di ragionamento consentono ai sistemi di AI di risolvere problemi più complessi scomponendo iterativamente un compito in passaggi più piccoli. La Tabella 1.3 mostra un esempio di un sistema non di ragionamento e di un sistema di ragionamento che risolvono lo stesso problema.

I sistemi di ragionamento hanno ottenuto importanti progressi nelle capacità su problemi difficili. Ad esempio, nel 2025, i sistemi di ragionamento specializzati per la risoluzione di problemi matematici, come Gemini Deep Think di Google e un modello non rilasciato e sperimentale di OpenAI, hanno risolto problemi delle Olimpiadi Internazionali di Matematica (in un contesto di test strutturato) a un livello equivalente alle prestazioni umane da medaglia d’oro (‡75, ‡76). I sistemi di ragionamento hanno dimostrato progressi significativi in ambiti formali come la matematica, i puzzle logici e domande scientifiche strutturate, in cui il ragionamento passo-passo può essere verificato in modo esplicito (‡77). Tuttavia, i sistemi di ragionamento possono anche fallire producendo catene di pensieri irrilevanti, improduttive o ripetitive (‡78, ‡79).

###@ Aggiornamenti sui metodi di addestramento

Dalla pubblicazione dell’ultimo Report (gennaio 2025), un metodo di training chiamato «distillazione» ha aumentato notevolmente l’efficienza con cui alcuni modelli possono essere ottimizzati (fine-tuned). La distillazione consiste nell’addestrare un modello «student» sugli output di un modello «teacher» più potente (e di solito più grande), permettendo allo student model di imitare direttamente gli output del teacher (‡80). Per esempio, DeepSeek ha sviluppato un grande modello chiamato DeepSeek-R1, che eccelle nel reasoning basato su catene di pensiero (chain-of-thought). R1 ha prodotto output di reasoning che sono stati poi usati per ottimizzare modelli student più piccoli, inclusi DeepSeek-V3. DeepSeek-V3 mantiene gran parte delle capacità matematiche, di coding e di analisi dei documenti di R1 e, secondo quanto riportato, è stato ottimizzato per circa $10,000 USD (sebbene i costi di pre-training non siano stati riportati) (‡81). È probabile che ciò sia di ordini di grandezza inferiore rispetto al costo di ottimizzare modelli più grandi e altrettanto capaci.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabella 1.3: Un esempio di un sistema non basato sul ragionamento (a sinistra) rispetto a un sistema basato sul ragionamento (a destra)
>white|black||9|11|br Risolviamo lo stesso enigma; questi esempi sono adattati da risposte reali dell’AI. Il sistema di ragionamento impiega più tempo e potenza computazionale per “pensare”, costruendo una “chain of thought” prima di fornire la sua risposta finale.

![figure.3](images/fig1.3_AI_agent.png)

##### Figura 1.3: Una rappresentazione illustrativa di un agente IA
>white|black||9|11|br Un modello di IA (al centro) configurato per pianificare iterativamente, ragionare e usare strumenti per portare a termine attività nel mondo reale. Fonte: International AI Safety Report 2026.


La distillazione può quindi rappresentare un modo economico ed efficiente per consentire ai modelli di acquisire capacità più potenti (‡82). Alcuni ricercatori hanno utilizzato la distillazione per mettere a punto modelli altamente capaci usando anche solo 1,000 esempi generati da modelli all'avanguardia (‡83). Poiché la distillazione richiede un modello insegnante pre-esistente, non può essere usata direttamente per far avanzare le capacità dei modelli all'avanguardia. Tuttavia, può accelerare la diffusione di capacità avanzate di AI, anche a partire da modelli proprietari a codice chiuso (‡84*).

Insieme ai progressi tecnologici nel cosiddetto ‘distributed compute’ (elaborazione distribuita) e all’addestramento decentralizzato (approcci in cui gli sviluppatori utilizzano più processori, server o data centre che lavorano insieme per eseguire l’addestramento o l’inferenza dell’AI (‡85, ‡86, ‡87)), il grado in cui molti progetti di sviluppo dell’AI dipendono da infrastrutture di calcolo grandi e centralizzate è stato ridotto. Questo consente sempre più spesso ad attori meno dotati di risorse di sviluppare e distribuire sistemi potenti.

###@ Aggiornamenti sugli agenti di IA

Dall’ultimo Report (January 2025), i progressi su come gli sviluppatori combinano modelli di AI con strumenti hanno abilitato lo sviluppo di agenti AI sempre più potenti. Gli agenti AI sono progettati per perseguire obiettivi, spesso specificati dagli utenti in linguaggio naturale. Per raggiungere questi obiettivi, vengono dotati dell’accesso a strumenti, come memoria, un’interfaccia per computer e browser web. Questi strumenti e il codice usato per combinarli con il modello sono indicati come ‘scaffolding’ e aiutano gli agenti AI a interagire autonomamente con il mondo, a formulare piani, a ricordare dettagli importanti e a perseguire obiettivi (‡88*, ‡89) con una supervisione o assistenza da parte degli esseri umani molto minore. Ad esempio, Manus AI è un popolare agente AI che può automatizzare varie attività, tra cui Web search, sviluppo di software e acquisti online (‡90). La Figura 1.3 illustra un semplice esempio di un agente AI composto da un modello di AI ‘brain’ general-purpose, capace di pianificare, ragionare e usare strumenti in modo iterativo per memoria, navigazione web e uso del computer.

L’infrastruttura digitale per gli agenti AI si sta espandendo (‡91) e sono sempre più comuni in vari settori (‡92, ‡93, ‡94). Gli agenti AI sono stati sviluppati per attività come la ricerca (‡37), l’ingegneria del software (‡95), il controllo robotico (‡96) e il servizio clienti (‡97). La ricerca e lo sviluppo in corso hanno portato a agenti AI o sistemi multi-agente sempre più capaci e più autonomi. I ricercatori hanno stimato che la complessità delle attività di benchmark software che gli agenti AI possono svolgere raddoppia circa ogni sette mesi (si veda anche §1.2. Capacità attuali) (‡98). Gli esperti sostengono che gli agenti AI sempre più capaci daranno origine sia a grandi opportunità sia a rischi (‡99, ‡100*) (si veda §2.2.1. Sfide di affidabilitá).

###@ lacune di evidenza

Le principali lacune di evidenza attorno al processo di sviluppo di un sistema di AI di carattere generale (general-purpose AI) derivano da una mancanza di informazioni pubblicamente disponibili su come essi vengano sviluppati. Alcuni sviluppatori sono altamente trasparenti su come sviluppano sistemi di AI di carattere generale (‡1, ‡101). Tuttavia, in generale, esiste un grado limitato di conoscenza pubblica e dei responsabili delle politiche (policymaker) su come la maggior parte dei modelli avanzati vengono sviluppati, messi in sicurezza, valutati e distribuiti. Ciò è particolarmente vero per i sistemi di AI distribuiti internamente che sono utilizzati all’interno delle aziende di AI ma non vengono usati o compresi da soggetti esterni interessati (‡102, ‡103). Questa limitata visibilità esterna crea sfide per la trasparenza e la supervisione. Vari ricercatori hanno indicato una trasparenza limitata e incoerente in merito a dati di addestramento (‡104, ‡105, ‡106), modelli di AI di carattere generale (‡107, ‡108), agenti di AI (‡92), valutazioni (‡109), pipeline di sviluppo (‡110) e sicurezza (‡111). Le limitazioni alla divulgazione esterna sono talvolta necessarie per proteggere i segreti commerciali e la proprietà intellettuale delle aziende. Allo stesso tempo, una bassa trasparenza rende più difficile per ricercatori indipendenti e responsabili delle politiche studiare modelli e sistemi di AI di carattere generale.


