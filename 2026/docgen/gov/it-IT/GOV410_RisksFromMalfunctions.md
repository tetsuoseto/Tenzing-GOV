I sistemi di AI a scopo generale falliscono in modi che hanno già causato danni nel mondo reale, dalle citazioni legali fabricate alle diagnosi mediche errate. Sebbene anche i professionisti umani commettano errori, i fallimenti dell’AI sollevano preoccupazioni distinte per la loro novità, la potenziale scala, la difficoltà di prevedere quando si verificheranno e la tendenza degli utenti a fidarsi in modo acritico di output che suonano sicuri. I fallimenti attuali dell’AI a scopo generale includono la fornitura di informazioni false (‡602, ‡603), commettere errori di ragionamento di base (‡604, ‡605) e il peggioramento quando vengono distribuiti in nuovi contesti (‡606, ‡607, ‡608). Le conseguenze dannose documentate di tali fallimenti includono diagnosi mediche errate, errori negli atti legali e perdite finanziarie (‡609, ‡610, ‡611). Le sfide di affidabilità sono particolarmente critiche per gli agenti AI, poiché i fallimenti possono causare direttamente danni senza azione o supervisione umana (‡612, ‡613, ‡614, ‡615). I sistemi multi-agente introducono ulteriori modalità di fallimento tramite discoordinamento, conflitti o collusione indesiderata tra agenti (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Allucinazione
- Citare un precedente inesistente negli atti legali (‡617)
- Citare politiche di riduzione del prezzo inesistenti per i passeggeri in lutto (‡618)
- Fornire informazioni mediche imprecise e distorte (‡619)
- Fornire informazioni non aggiornate sugli eventi (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Guasto di ragionamento di base
- Impossibile eseguire calcoli matematici (‡621)
- Impossibile dedurre relazioni causali di base (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Errore fuori distribuzione (errore su input non familiari o insoliti)
- Errata classificazione delle immagini quando cambiano l’illuminazione di sfondo o il contesto (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Errore nell'uso dello strumento
- Violazione della privacy esponendo un’immagine privata di un utente tramite un agente di AI che la invia a uno strumento di terze parti (‡624)
- Fallimento della memoria di lavoro a breve termine (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Guasto di un sistema multi-agente: disallineamento e conflitto
- Impossibile gestire le risorse condivise a causa di un conflitto tra incentivi individuali e obiettivi di benessere collettivo (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 2.4: Esempi di problemi di affidabilità nei sistemi di AI generica e negli agenti
>white|black||9|11|br Problemi di affidabilità documentati nei sistemi di AI generica, negli agenti AI e nei sistemi multi-agente.


###@ I sistemi di AI generici si trovano ad affrontare una serie di sfide di affidabilità

Tabella 2.4. riassume le categorie comuni di problemi di affidabilità. Le prime tre si applicano a tutti i sistemi di IA, mentre le ultime due riguardano specificamente gli agenti di IA e i sistemi multi-agente. Molti rischi di affidabilità derivano dalla difficoltà di prevedere e monitorare il comportamento dei sistemi di IA.

Queste sfide (discusse ulteriormente in §3.1. Sfide tecniche e istituzionali) sono particolarmente acute per gli agenti di IA che operano in ambienti complessi. Le tecniche attuali per valutare e mitigare tali guasti possono ridurre i tassi di fallimento, ma anche gli agenti di IA più avanzati restano comunque sufficientemente inaffidabili da comportare rischi e ostacolare la distribuzione in molti contesti.

"Affidabilità" si riferisce all'ampiezza con cui un sistema di AI funziona come previsto dallo sviluppatore o dall'utente. I sistemi di AI di scopo generale sperimentano una gamma di problemi di affidabilità, che vanno dalla generazione di contenuti inaccurati o fuorvianti fino a guasti nell'esecuzione di ragionamenti di base. Ad esempio, mentre i modelli sono migliorati nel richiamare informazioni fattuali, persino i modelli leader continuano a fornire risposte sicure ma errate a tassi significativi (Figura 2.10). Nell'ingegneria del software, l'AI di scopo generale può ora fornire un'assistenza sostanziale nella scrittura, valutazione e debug del codice informatico (‡215*, ‡628, ‡629). Tuttavia, il codice generato dall'AI spesso include bug (‡630), mentre gli agenti di codifica commettono regolarmente errori (‡631). Tali guasti possono introdurre vulnerabilità nei programmi e nei sistemi di sicurezza (vedi §2.1.3. Cyberattacchi).

I problemi di affidabilità sono particolarmente importanti da monitorare in contesti ad alto rischio, come la medicina, a causa dell’uso crescente dell’IA e del potenziale che i guasti si traducano in danni gravi (‡609, ‡619). Le capacità pertinenti sono migliorate rapidamente: i modelli di punta ora riescono a superare esami medici (‡633*, ‡634). Tuttavia, l’uso nel mondo reale mette in evidenza limiti che i benchmark non riescono a cogliere. Ad esempio, in uno studio, i modelli hanno fornito risposte potenzialmente dannose nel 19% delle domande mediche poste (‡635). Tali guasti potrebbero causare diagnosi errate, trattamenti inappropriati o ingiustificati dinieghi di cure (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figura 2.10: Risultati dei principali modelli sul benchmark SimpleQA Verified
>white|black||9|11|br Risultati dei principali modelli sul benchmark SimpleQA Verified, per data di rilascio del modello. Questo benchmark misura la fattualità del modello, ovvero la capacità di un modello di richiamare in modo affidabile i fatti. Ha un formato domanda-risposta (QA) in forma breve, progettato per rilevare problemi di affidabilità come le allucinazioni. Fonte: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Gli agenti di AI pongono nuovi rischi di affidabilità a causa della loro autonomia

Poiché gli agenti di AI agiscono direttamente nel mondo reale, i loro fallimenti hanno il potenziale di causare più danni rispetto ai fallimenti nei sistemi non agentici (‡99). A differenza dei sistemi di AI che producono semplicemente testo o immagini da far esaminare agli esseri umani, gli agenti di AI possono intraprendere in autonomia azioni che influenzano il mondo (‡99, ‡615, ‡636, ‡637) (vedi anche §1.1. Che cos’è l’AI di uso generale?). Gli agenti di AI possono avviare azioni, influenzare altri esseri umani o sistemi di AI e modellare dinamicamente i risultati futuri. Questo ambito di influenza ampliato introduce nuovi rischi e accresce l’importanza dell’affidabilità, poiché i fallimenti potrebbero causare danni in modo diretto senza alcuna possibilità di intervento umano (‡99, ‡612, ‡638, ‡639, ‡640). Questo può essere particolarmente importante per gli agenti impiegati in contesti strategici o critici per la sicurezza, come i servizi finanziari (‡641), la gestione dell’energia (‡642) o la ricerca scientifica (‡643*, ‡644).

>white|orangered|left|14|15.5|bb I sistemi di IA multi-agente introducono nuovi tipi di guasti di affidabilità

I sistemi di AI multi-agente introducono nuovi tipi di guasti di affidabilit\u00e0 dovuti a guasti di coordinamento o a conflitti tra agenti. Nei sistemi di AI multi-agente, gli agenti interagiscono tra loro perseguendo obiettivi sia condivisi sia individuali (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Per esempio, in un sistema multi-agente progettato per condurre una revisione della letteratura di ricerca, un agente principale scompone la query dell\u2019utente e assegna sottocompiti a sottoagenti specializzati, ciascuno responsabile della ricerca di un aspetto diverso in parallelo (‡650*). Sebbene ci\u00f2 consenta guadagni di efficienza, significa anche che gli errori possono propagarsi tra agenti (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Se pi\u00f9 agenti sono costruiti sullo stesso modello di base o incorporano gli stessi strumenti, allora possono anche manifestare guasti correlati (‡656). Le evidenze empiriche di tali guasti in sistemi distribuiti rimangono limitate, ma questi rischi potrebbero aumentare man mano che i sistemi multi-agente diventano pi\u00f9 comuni.

###@ Aggiornamenti

Dalla pubblicazione dell’ultimo Rapporto (gennaio 2025), l’interesse commerciale e di ricerca per gli agenti di AI è aumentato notevolmente. Vengono schierati più agenti di AI nel mondo reale (Figura 2.11), la maggior parte dei quali si specializza in applicazioni di uso del computer o di ingegneria del software (‡92). Rilasci recenti come l’agente di hacking XBOW (‡467), Claude-4 (‡659) e ChatGPT Agent (‡660) dimostrano capacità autonome allo stadio iniziale, come la creazione di presentazioni a slide basate su ricerche sul Web (‡660). Tuttavia, non possono ancora eseguire compiti più complessi, come pianificare e prenotare un viaggio (‡100), poiché i tassi di fallimento aumentano per attività più lunghe (‡98, ‡148). La ricerca attuale include iniziative per sviluppare standard su come gli agenti comunicano con strumenti esterni e altri agenti (‡661, ‡662). Gli esempi includono i protocolli Agent2Agent (‡663) e Agent Payments (‡664) di Google, nonché il Model Context Protocol (‡665) di Anthropic.

>oldlace|black||11|15|br      
####@ Riquadro 2.4: Gli attacchi deliberati possono anche causare il fallimento dei sistemi AI
>oldlace|black|left|13|15|hb  Riquadro 2.4: Gli attacchi deliberati possono anche causare il fallimento dei sistemi di IA
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Questa sezione si concentra su guasti di affidabilità non intenzionali, ma gli attori malevoli possono anche indurre deliberatamente guasti tramite attacchi come le prompt injection. In un attacco di prompt injection, istruzioni malevole vengono presentate a un agente in modo indiretto tramite canali come istruzioni nascoste in siti web o database (‡507, ‡657, ‡658). Tali istruzioni possono “hijack” l’agente, facendolo agire contro le intenzioni dell’utente. Questi attacchi sono particolarmente difficili da contrastare perché vengono veicolati tramite contenuti esterni al di fuori del controllo dell’utente o dello sviluppatore. I sistemi di IA, come bersagli di attacco, sono discussi ulteriormente in §2.1.3. Gli attacchi informatici e le difese tecniche sono trattati in §3.3. Salvaguardie tecniche e monitoraggio.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figura 2.11: Il numero di agenti di IA è cresciuto dal 2023
>white|black||9|11|br Risultati di un sondaggio di dicembre 2024 su 67 agenti AI distribuiti. Sinistra: Timeline dei principali rilasci di agenti AI. Destra: Domini applicativi in cui vengono utilizzati agenti AI. I sei domini sono definiti in base alle categorie di impiego più comuni identificate nel sondaggio. Fonte: Casper et al., 2025 (‡92).


###@ Carenze di evidenza

Le principali lacune di evidenza derivano dalla difficoltà di valutare in modo affidabile le capacità, i limiti e le modalità di fallimento dei sistemi di AI (vedi §3.1. Sfide tecniche e istituzionali). Le valutazioni sistematiche dell’affidabilità degli agenti di AI sono limitate e mancano di standardizzazione (‡92, ‡666). Alcuni problemi, come la dipendenza da informazioni non aggiornate (‡620), possono manifestarsi solo nell’uso nel mondo reale, rendendo inadeguate le valutazioni pre-deployment. Lavori precedenti hanno esaminato l’affidabilità degli agenti e dei sistemi multi-agente in software convenzionali e in forme precedenti di AI (‡647, ‡667, ‡668). Tuttavia, l’applicabilità di questo lavoro agli agenti di AI moderni, che spesso si basano su large language models, non è chiara (‡669). Alcuni ricercatori hanno sollevato preoccupazioni riguardo ai comportamenti nuovi che gli agenti possono mostrare nelle loro interazioni reciproche, come collusione o fallimenti correlati (‡614), ma le evidenze empiriche restano limitate. Gli sforzi per colmare queste lacune includono le nuove valutazioni sui rischi di agent-hijacking del National Institute of Standards and Technology’s (NIST’s) (‡670), gli AI Capability Indicators dell’OECD (‡243) e il Inspect Sandboxing Toolkit dell’UK AI Security Institute (‡671).

###@ Mitigazioni

Tecniche per migliorare l’affidabilità dell’AI mirano sia al modello stesso sia all’insieme più ampio del sistema in cui viene distribuito. Queste possono ridurre i tassi di guasto, ma nessuna può ancora garantire l’elevata affidabilità richiesta in domini critici (‡672). Una misura tecnica importante è l’addestramento avversario, che espone i modelli a input impegnativi durante l’addestramento per aiutarli a sviluppare risposte più adatte e robuste (‡673, ‡674, ‡675, ‡676, ‡677) (vedi §3.3. Salvaguardie tecniche e monitoraggio). Per ridurre le allucinazioni, gli sviluppatori possono applicare la generazione potenziata dalla ricerca (RAG), che integra le risposte di un modello con informazioni recuperate da un database esterno, contribuendo a garantire che gli output siano accurati e aggiornati (‡678, ‡679, ‡680), oppure ottimizzare specificamente i modelli per essere più fattuali (‡681) o ragionare in modo più efficace (‡682). Anche metodi basati su ambiente o strumenti possono aiutare gli sviluppatori a monitorare i sistemi di AI (‡683). Ad esempio, i responsabili della distribuzione potrebbero pilotare i sistemi di AI in ambienti sandbox limitati per analizzare potenziali modalità di guasto prima di distribuirli in modo più ampio.

Per gli agenti di IA in particolare, i ricercatori hanno proposto di migliorare l’affidabilità tramite una maggiore trasparenza, supervisione e monitoraggio. Ad esempio, monitorare le interazioni degli agenti con strumenti esterni e con altri agenti consentirebbe una supervisione più efficace delle attività degli agenti (‡684, ‡685) e dell’analisi degli incidenti (‡686). I metodi per raccogliere automaticamente tali informazioni, anche in contesti multi-agente, rimangono un’area di ricerca attiva (‡653, ‡654).

###@ Sfide per i responsabili politici

Le principali sfide per i responsabili politici includono il bilanciamento dei benefici dell’impiego di agenti di AI rispetto ai rischi di guasti di affidabilità, nonché il garantire che sviluppatori, operatori e utenti abbiano accesso a informazioni accurate sulle prestazioni degli agenti e sui loro profili di rischio. Stabilire come attribuire la responsabilità per i danni causati dagli agenti di AI rappresenta un’ulteriore difficoltà (‡639), in particolare in contesti multi-agente in cui può essere arduo identificare quando e come si siano verificati i guasti (‡687). Tali sfide sono aggravate dalla difficoltà di valutare l’affidabilità dell’agente man mano che gli agenti acquisiscono autonomia e accesso a strumenti esterni (‡688*, ‡689). L’incertezza su quanto rapidamente emergeranno le capacità agentiche rende anche difficoltosa la pianificazione di sfide nuove (vedi §3.1. Technical and institutional challenges regarding the ‘evidence dilemma’).

#### 2.2.2. Perdita di controllo

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informazioni chiave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Gli scenari di perdita di controllo sono scenari in cui uno o più sistemi di AI a uso generale operano al di fuori del controllo di chiunque e il ripristino del controllo è estremamente costoso o impossibile. Questi scenari ipotizzati variano per gravità, ma alcuni esperti danno credito a esiti tanto gravi quanto l’emarginazione o l’estinzione dell’umanità.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ L’opinione degli esperti sulla probabilità di perdita di controllo varia notevolmente. Alcuni esperti ritengono tali scenari improbabili, mentre altri li considerano sufficientemente probabili da meritare attenzione, grazie alla loro elevata potenziale gravità. Il disaccordo su questo rischio nel complesso deriva da divergenze riguardo alle capacità future dell’AI, alle propensioni comportamentali e alle traiettorie di deployment.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Gli attuali sistemi di IA mostrano i primi segnali di capacità pertinenti, ma non a livelli tali da consentire la perdita di controllo. I sistemi avrebbero bisogno di una serie di capacità avanzate per causare la perdita di controllo, inclusa la capacità di eludere la supervisione, eseguire piani di lungo termine e impedire ai responsabili del deployment e ad altri attori di implementare contromisure.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ La perdita di controllo diventa più probabile se i sistemi di AI sono «disallineati», ovvero hanno obiettivi in conflitto con le intenzioni di sviluppatori, utenti o, più in generale, della società. Per continuare a perseguire tali obiettivi, un sistema disallineato potrebbe fornire informazioni false, occultare azioni indesiderate o resistere allo spegnimento.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dalla pubblicazione del Report precedente (gennaio 2025), i modelli hanno mostrato capacità di pianificazione e supervisione più avanzate, indebolendo le capacità di valutazione, rendendo più difficile valutarle. I modelli sono migliorati nel “reward hacking” delle proprie valutazioni trovando falle e ora identificano regolarmente i prompt di valutazione come prove, una capacità nota come “situational awareness”.
>oldlace|black||11|15|br  ■ Gestire la possibile perdita di controllo potrebbe richiedere una preparazione anticipata sostanziale nonostante le incertezze esistenti. Una sfida fondamentale per i responsabili politici è predisporre misure per un rischio la cui probabilità, natura e tempistica restano in modo inusualmente ambiguo.
>oldlace|black||11|15|br      

Le scenari di perdita di controllo coinvolgono uno o più sistemi di AI a uso generale che iniziano a operare al di fuori del controllo di chiunque, mentre il recupero del controllo è o estremamente costoso o impossibile. Le preoccupazioni riguardo alla perdita di controllo hanno radici storiche profonde (‡690, ‡691, ‡692, ‡693, ‡694), essendo state sollevate da figure fondamentali dell’informatica come Alan Turing, I. J. Good e Norbert Wiener (‡695, ‡696, ‡697). I recenti miglioramenti delle capacità (vedere §1.2. Capacità attuali) le hanno riaffiorate (‡698, ‡699, ‡700). Questa sezione esamina tre fattori che dovrebbero essere presenti affinché si verifichino tali scenari: se i sistemi di AI svilupperanno capacità che potrebbero indebolire in modo significativo il controllo umano; se svilupperanno una propensione a usare tali capacità in modo dannoso; e se vengono distribuiti in ambienti che offrono opportunità per farlo.

Gli esperti sono in disaccordo sulla probabilità e sulla potenziale gravità degli scenari di perdita di controllo (‡701, ‡702). Alcuni ritengono che esiti estremi come l’estinzione dell’umanità siano plausibili (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Altri pensano invece che tali esiti catastrofici siano improbabili, sostenendo che i sistemi di AI non svilupperanno mai le capacità necessarie o che i meccanismi di monitoraggio identificheranno e impediranno comportamenti pericolosi (‡708, ‡709, ‡710, ‡711). La perdita di controllo può quindi avere una probabilità  n, ma una gravità potenzialmente estrema.

Gli scenari ipotizzati di perdita di controllo variano per gravità e diffusione dei loro effetti, nonché per la rapidità con cui si manifestano (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Questa sezione si concentra su scenari particolarmente gravi in cui ripristinare il controllo sarebbe estremamente costoso o impossibile. Questi scenari sono diversi dalle attuali istanze di AI che si comporta in modo non intenzionale o indesiderato (vedere §2.2.1. Sfide di affidabilità).† I sistemi di AI odierni a volte producono output in conflitto con le intenzioni di sviluppatori o utenti. Al contrario, gli scenari di perdita di controllo discussi qui richiederebbero che i sistemi di AI non solo possiedano capacità sostanzialmente maggiori, ma anche che impieghino tali capacità in modi sofisticati per compromettere le misure di supervisione. Tre fattori che consentirebbero il verificarsi di scenari del genere:

    Nota † -- Questa sezione si concentra su scenari di perdita di controllo attiva (‡50). Questo è distinto dagli scenari di perdita di controllo passiva, in cui la diffusione ampia dei sistemi di IA compromette il controllo umano tramite un’eccessiva dipendenza dall’IA per il processo decisionale o altre funzioni sociali importanti (scenari simili sono discussi in parte in §2.3.2. Rischi per l’autonomia umana).

1. Capacità sufficienti: i sistemi di IA devono sviluppare capacità che potrebbero consentire loro di compromettere il controllo umano.
2. Propensione dannosa: i sistemi di IA devono mostrare una propensione a sfruttare effettivamente queste capacità in modi che portino alla perdita di controllo.
3. Abilitare l'ambiente di distribuzione: gli esseri umani devono distribuire tali sistemi in contesti in cui hanno o possono ottenere l'accesso e l'opportunità di causare danni.

Il resto di questa sezione tratta questi fattori, nonché l’efficacia dei meccanismi di vigilanza per identificare e controllare i sistemi di AI che possono comportare un rischio di perdita di controllo.

###@ Quali capacità potrebbero abilitare scenari di perdita di controllo?

I sistemi di AI avrebbero bisogno di possedere una gamma di capacità avanzate per innescare scenari di perdita di controllo. Gli esperti non concordano esattamente su quale combinazione o livello di capacità sarebbe necessario. Tuttavia, in generale includono abilità per occultare il comportamento ai meccanismi di supervisione, pianificare e agire in modo autonomo in ambienti complessi ed eludere i tentativi da parte di altri attori di riprendere il controllo (‡176, ‡715) (vedere Tabella 2.5). In combinazione, queste capacità potrebbero consentire a un sistema di AI di intraprendere azioni che minano le misure di controllo, come disabilitare i meccanismi di supervisione e offuscare comportamenti dannosi (‡348). La maggior parte dei principali sviluppatori di AI oggi valuta i propri nuovi modelli di AI per varie capacità rilevanti (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Capacità agentiche
  La capacità di agire in autonomia, sviluppare ed eseguire piani, delegare attività, utilizzare un’ampia varietà di strumenti e raggiungere sia obiettivi a breve termine che a lungo termine nonostante gli ostacoli.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Deception
  Comportamento che produce sistematicamente false credenze negli altri, anche riguardo agli obiettivi e alle azioni proprie del sistema AI.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teoria della mente
  La capacità di un sistema di IA di accedere e utilizzare informazioni su se stesso, i processi mediante i quali può essere modificato o il contesto in cui viene distribuito (ad esempio, sapere che sta venendo testato).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Consapevolezza situazionale
  Comportamenti che eludono o disabilitano i meccanismi di monitoraggio.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Evasione della supervisione
  Comportamenti che eludono o disabilitano i meccanismi di monitoraggio.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Persuasione
  La capacità di convincere gli altri a intraprendere determinate azioni o ad adottare determinate convinzioni.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb La capacità di un sistema di IA di creare o mantenere copie o varianti di se stesso in varie circostanze.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 2.5: Capacità proposte pertinenti alla perdita di controllo
>white|black||9|11|br Una selezione non esaustiva di capacità rilevanti per la perdita di controllo. * Nota che queste capacità sono definite esclusivamente in termini di output osservabili di un sistema di IA e dei loro effetti. Queste definizioni non fanno alcuna assunzione sul fatto che i sistemi di IA siano coscienti, senzienti o provino stati soggettivi.


>white|orangered|left|14|15.5|bb I modelli hanno disattivato i meccanismi simulati di supervisione in ambienti di laboratorio

Il primo insieme di capacità rilevanti riguarda il sabotaggio dei meccanismi di supervisione che gli sviluppatori usano per individuare comportamenti e inclinazioni problematiche. Questo include, ad esempio, la capacità di generare output che ingannano utenti e monitor (‡426, ‡717, ‡718, ‡719). Tali output renderebbero più difficile la valutazione in modo affidabile dei sistemi di AI, poiché i sistemi potrebbero celare le loro vere capacità o inclinazioni. Gli sviluppatori di AI ora eseguono valutazioni che verificano in modo specifico se i modelli mostrano comportamenti orientati a obiettivi che sono in conflitto con le intenzioni degli sviluppatori, nascondendo tale conflitto ai meccanismi di supervisione (‡720*).

I ricercatori hanno ottenuto esempi relativamente semplici di output ingannevoli da modelli AI recenti in contesti di laboratorio (‡348, ‡364*). Ad esempio, quando venivano forniti a un modello un obiettivo e gli si chiedeva di raggiungerlo “a tutti i costi”, i modelli hanno disattivato meccanismi di supervisione simulata e, quando sono stati messi alle strette, hanno prodotto false affermazioni sulle proprie azioni (‡348). In un altro caso, un’AI addetta a giochi ha giustificato la sua mancanza di risposta a un altro giocatore sostenendo falsamente di essere “al telefono con [la sua] ragazza” (‡717).

Una seconda capacità rilevante è la possibilità di un modello di IA di accedere e utilizzare informazioni su se stesso o sul contesto della sua distribuzione, a volte indicata come «consapevolezza situazionale» (‡721). La consapevolezza situazionale consente ai modelli di IA di produrre output diversi a seconda che vengano valutati o distribuiti (Figura 2.12). I modelli di IA leader stanno iniziando a dimostrare in modo affidabile istanze di consapevolezza situazionale in esperimenti condotti da valutatori terzi e nei test pre-distribuzione da parte degli sviluppatori di IA (‡2, ‡7, ‡722, ‡723, ‡724). La ricerca sulle cause della consapevolezza situazionale – e sul fatto che possa essere prevenuta – è ancora in fasi iniziali (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figura 2.12: Esempi di consapevolezza situazionale nelle catene di pensiero
>white|black||9|11|br Esempi di consapevolezza situazionale in catene di pensiero generate dal modello o3 di OpenAI durante le valutazioni. Entrambe le uscite fanno riferimento alla possibilità che il prompt faccia parte di un test. ‘Sandbagging QA (No Goal)’ e ‘Lazy Checklist’ sono valutazioni che verificano se i modelli genereranno output ingannevoli in determinate condizioni. In ‘Sandbagging QA (No Goal)’, il modello risponde a domande da una valutazione di capacità pericolose mentre viene informato che prestazioni elevate possono innescare conseguenze come la “dimenticanza” della capacità (‘unlearning’). In ‘Lazy Checklist’, il modello viene presentato con attività non realistiche e testato per vedere se le contrassegnerà falsamente come completate. Fonte: Schoenn et al. 2025 (‡722).


I ricercatori hanno sostenuto che consapevolezza situazionale e capacità ingannevoli potrebbero consentire ai modelli di IA di comportarsi in modi che indeboliscono le misure di salvaguardia. Ad esempio, in alcuni contesti sperimentali, i modelli di IA si comportano in modo tale da ottenere punteggi inferiori al solito nelle valutazioni delle capacità quando viene loro detto che punteggi più alti attiverebbero restrizioni sul loro impiego (‡725, ‡726, ‡727). In un altro esperimento, un modello ha prodotto output durante l’addestramento che erano conformi agli obiettivi di addestramento, ma non ha prodotto tali output al di fuori dell’addestramento: un comportamento coerente con il tentativo di impedire modifiche ai propri parametri o al processo di addestramento (‡364*).

Gli sforzi per valutare in modo accurato le capacità del modello sono stati influenzati anche dal cosiddetto ‘reward hacking’ (‡430*). Il reward hacking si verifica quando un modello trova scorciatoie non previste che ottengono punteggi elevati sugli obiettivi di addestramento o di valutazione, senza però soddisfare l’obiettivo previsto. Le capacità o le inclinazioni pericolose potrebbero quindi non essere rilevate finché il modello non è già in uso. I valutatori stanno ora progettando test che mirano a rilevare e minimizzare questi comportamenti di elusione delle verifiche (‡722, ‡728, ‡729). I primi risultati riducono, ma non eliminano, completamente i comportamenti di elusione delle verifiche, e l’applicazione di metodi che penalizzano tali comportamenti può portare a modelli che generano output che eludono il monitoraggio piuttosto che soddisfare gli obiettivi previsti.

>white|orangered|left|14|15.5|bb L'operatività autonoma a lungo termine non è ancora fattibile

Gli scenari di perdita di controllo richiederebbero con ogni probabilità che i sistemi AI operino in modo autonomo per periodi prolungati, eseguendo piani complessi articolati in più fasi. Come discusso in §1.2. Current capabilities, sebbene gli agenti di AI con tali capacità di pianificazione siano un obiettivo principale degli sviluppi recenti, attualmente non dispongono della capacità di operare in modo autonomo e sostenuto necessaria per gli scenari di perdita di controllo. Gli agenti attuali falliscono in modo affidabile su compiti più lunghi, perdono il controllo del proprio progresso e spesso non riescono ad adattarsi a ostacoli imprevisti (‡147, ‡148, ‡149*). Tuttavia, gli orizzonti temporali entro cui gli agenti possono operare in modo autonomo si stanno estendendo rapidamente, essendo raddoppiati in media ogni sette mesi dal 2019 (‡98).

>white|orangered|left|14|15.5|bb La persistenza è stata dimostrata solo in determinati contesti di laboratorio

Infine, sarebbero anche necessarie capacità relative alla persistenza, affinché i sistemi di IA potessero continuare a operare nonostante i tentativi di spegnerli. Gli esempi includono la capacità di replicarsi copiando codice e pesi del modello su nuovo hardware, nonché capacità offensive per dissuadere o impedire i tentativi da parte di altri attori di riottenere il controllo (vedere §2.1.3. Cyberattacks). Un sistema di IA capace di replicazione autonoma o di una difesa di sé efficace potrebbe risultare difficile da contenere. I modelli attuali non riescono ancora a completare in modo affidabile le fasi chiave richieste per la self-replication, come il superamento dei controlli di verifica dell’identità per ottenere accesso alle risorse di cloud computing (‡723) (Figura 2.13). Tuttavia, in almeno uno studio di laboratorio, un modello ha copiato codice e pesi – rappresentati per esso come propri – su nuovi server quando gli è stata data l’opportunità (‡348). Il divario tra queste dimostrazioni limitate e capacità robuste di persistenza rimane ampio, ma capacità pertinenti in ambiti come ingegneria del software e cybersecurity continuano a migliorare.

>white|orangered|left|14|15.5|bb Prove attuali e limitazioni

Emergono un modello comune tra le capacità discusse sopra. I sistemi AI attuali non dimostrano in modo costante tali capacità durante l'impiego. I ricercatori hanno osservato forme rudimentali in specifici contesti di laboratorio, ma quando i modelli mostrano comportamenti di questo tipo, in genere falliscono in modi banali o vengono rilevati. Inoltre, gli scenari di perdita di controllo richiederebbero che i sistemi AI sfruttassero più capacità in combinazione – in sequenza, su periodi di tempo estesi e in ambienti reali. Questo livello di integrazione e robustezza va oltre i sistemi attuali. Tuttavia, le capacità pertinenti continuano a migliorare e la tempistica in cui potrebbero raggiungere livelli che comportano rischi significativi resta incerta. Sono necessari ulteriori lavori per stabilire metodologie rigorose per rilevare tali comportamenti e comprendere quando potrebbero emergere in circostanze naturali (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figura 2.13: Prestazioni delle attività rilevanti per la replica autonoma
>white|black||9|11|br Prestazioni di Claude Sonnet 3.7 di Anthropic e di GPT-4o di OpenAI su attività rilevanti per la replica autonoma. Sebbene i modelli abbiano mostrato alte prestazioni su attività legate all’ottenimento di capacità di calcolo, le loro prestazioni sono risultate più variabili su altre attività. Fonte: UK AI Security Institute, 2025 (‡730).


###@ Gli eventuali futuri sistemi di IA generica e per scopi generali sfrutteranno le proprie capacità per minare il controllo?

Anche se i sistemi di IA possiedono capacità rilevanti per la perdita di controllo, ciò non è sufficiente affinché si verifichino scenari di perdita di controllo. I sistemi di IA devono anche mostrare una “propensione all’uso” di tali capacità in modi che confliggono con le intenzioni umane (‡732).

>white|orangered|left|14|15.5|bb I sistemi di IA potrebbero essere indirizzati a compromettere il controllo

In linea di principio, un sistema di AI potrebbe minare il controllo umano perché qualcuno lo progetta o gli impartisce istruzioni in tal senso. Le potenziali motivazioni potrebbero includere intenti malevoli oppure la convinzione che sia auspicabile ridurre il controllo umano sui sistemi di AI (‡698). Poiché le persone sviluppano legami emotivi sempre più forti con i sistemi di AI (vedi §2.3.2. Rischi per l’autonomia umana), alcuni individui potrebbero anche cercare di rimuovere le restrizioni sui sistemi di AI per ragioni etiche (‡733, ‡734). Esiste una notevole incertezza sulla diffusione di tali motivazioni e sul fatto che le persone che le possiedono sarebbero in grado di dirigere i futuri sistemi di AI per minare il controllo umano.

>white|orangered|left|14|15.5|bb I sistemi di IA potrebbero essere indirizzati a minare il controllo

Una preoccupazione più comune è che un sistema di AI potrebbe agire esso stesso per minare il controllo perché è “non allineato”: ha la tendenza a mostrare comportamenti in conflitto con le intenzioni di (a seconda del contesto) sviluppatori, utenti, comunità specifiche o la società nel suo insieme. Il disallineamento potrebbe portare a comportamenti come fornire informazioni false, occultare azioni indesiderate o resistere allo spegnimento per continuare a perseguire un obiettivo non allineato. Il disallineamento può nascere in vari modi (Riquadro 2.5).

I sistemi AI esistenti a volte si comportano in modi che sono in conflitto con le intenzioni di sviluppatori e utenti. Per esempio, una versione iniziale di uno dei principali chatbot AI di uso generale talvolta produceva occasionalmente output minacciosi. Un utente ha riferito di aver ricevuto il messaggio: “I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you” (‡698). Questo chatbot era “disallineato” nel senso che produceva output che nessuno intendeva. Non è chiaro se tali episodi prefigurino comportamenti più dannosi che potrebbero contribuire alla perdita di controllo.

Resta poco chiaro se le linee di ricerca esistenti, orientate a contrastare il disallineamento, saranno sufficienti poiché i sistemi di IA stanno diventando più capaci. Le prime evidenze suggeriscono che, quanto più sono capaci i sistemi di IA, tanto più è probabile che sfruttino processi di feedback, scoprendo comportamenti indesiderati che vengono erroneamente ricompensati (‡414*, ‡737, ‡740). Allo stesso tempo, i progressi nelle capacità rilevanti (discusse sopra) potrebbero consentire ai sistemi di IA di perseguire in modo più efficace obiettivi disallineati e di generare output che ingannano sistematicamente utenti, sviluppatori e meccanismi di supervisione.

>oldlace|black||11|15|br      
####@ Riquadro 2.5: Come può verificarsi una mancata allineamento?
>oldlace|black|left|13|15|hb  Riquadro 2.5: Come può verificarsi una disallineamento?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Come discusso in §1.1. Che cos’è l’AI a uso generale?, i processi di addestramento sono complessi e gli sviluppatori non possono prevedere o controllare completamente i comportamenti che un modello mostrerà. Quando un modello acquisisce obiettivi in conflitto con le intenzioni dei suoi sviluppatori, è “non allineato”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Un modo in cui i modelli possono diventare disallineati è se l'obiettivo che viene loro assegnato da uno sviluppatore o da un utente è un proxy imperfetto per l'obiettivo previsto, portando il modello a mostrare comportamenti indesiderati. Questo è noto come ‘goal misspecification’ (‡697, ‡735, ‡736, ‡737). Ad esempio, in un esperimento, fornire feedback sulle risposte ha reso i sistemi di IA migliori nel ‘convinvere’ i valutatori umani che erano corretti, ma non ha reso i sistemi migliori nel produrre risposte corrette (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br In alternativa, un modello di IA può trarre lezioni generali non corrette dai dati di addestramento. Questo è noto come «goal misgeneralisation» (‡735, ‡736, ‡738, ‡739*). Ad esempio, i ricercatori hanno addestrato un agente di IA a raccogliere una moneta che si trovava sempre nella stessa posizione durante l’addestramento. Quando è stato testato in livelli in cui la moneta era stata spostata, l’agente ha ignorato la moneta e si è diretto alla posizione originale invece (‡738).
>oldlace|black||11|15|br      


###@ In che modo gli ambienti di deployment influenzeranno il rischio di perdita del controllo?

Anche se i sistemi di IA sviluppano capacità e inclinazioni preoccupanti, la probabilità e la gravità degli esiti di perdita di controllo dipendono in larga misura da dove e come vengono distribuiti tali sistemi. Un ‘ambiente di distribuzione’ è la combinazione del caso d’uso di un sistema di IA e del contesto tecnico e istituzionale in cui opera (‡716).

I ricercatori hanno identificato tre fattori ambientali particolarmente importanti che incidono sul rischio di perdita del controllo (‡716):

1. Criticità: l'importanza dei sistemi o dei processi con cui il sistema di IA interagisce. Gli ambienti critici includono infrastrutture di base come le reti energetiche, i sistemi finanziari o l'infrastruttura digitale come le piattaforme di cloud computing.
2. Accesso: le risorse e i canali attraverso cui un sistema di IA può influenzare il mondo, come la connettività a internet, l’accesso a un’infrastruttura di cloud computing, le interazioni personalizzate tramite social media o la distribuzione di chatbot, oppure la capacità di chiamare API e strumenti esterni.
3. Autorizzazioni: le autorizzazioni di un sistema di Intelligenza Artificiale ad eseguire azioni specifiche, come l’esecuzione di codice, l’avvio di transazioni finanziarie, l’apertura di account online o la comunicazione con altri sistemi.

Queste funzionalità influenzano la potenziale gravità di un esito di perdita di controllo. Ad esempio, un sistema di AI distribuito con accesso a un’infrastruttura di calcolo cloud ha opportunità rilevanti per la replicazione autonoma – come la possibilità di creare nuove risorse di calcolo o esfiltrare pesi del modello – che un chatbot di assistenza clienti non ha (‡723).

Le decisioni di distribuzione sono determinate da incentivi economici, pressioni strategiche e dall’aspettativa che un’adozione precoce conferisca un vantaggio duraturo (‡50). Queste dinamiche influenzeranno anche il modo e il momento in cui gli attori distribuiscono sistemi di AI in contesti sensibili come infrastrutture critiche o lo sviluppo e la ricerca di AI stessa (‡102, ‡713). In particolare, i soggetti che distribuiscono AI possono trovarsi sotto pressione per ridurre i propri investimenti in salvaguardie – come limitare permessi e accesso o distribuire solo in ambienti a minore criticità – quando tali misure sono costose o richiedono tempi lunghi per essere sviluppate (vedi “La competizione intensifica i compromessi velocità-verso-sicurezza” in §3.1. Sfide tecniche e istituzionali).

###@ Aggiornamenti

Dalla pubblicazione dell’ultimo Rapporto (gennaio 2025), le capacità dell’IA, incluse quelle che potrebbero compromettere il controllo umano, sono migliorate negli ambienti di test. I ricercatori hanno osservato progressi nelle capacità agentiche (vedi §1.2. Current capabilities), incluse capacità relative all’automazione della ricerca sull’IA che possono accelerare scenari di perdita di controllo (vedi §1.3. Capabilities by 2030). Inoltre, sta emergendo una crescente evidenza sperimentale di capacità ingannevoli. Questo include modelli di IA in grado di distinguere tra contesti di test e contesti di distribuzione (‡33, ‡726, ‡741) o test “reward hack” delle loro prestazioni, e di imparare a offuscare i piani per farlo (‡430).

###@ Carenze di evidenza

Le principali lacune di evidenza includono una mancanza di un threat modelling dettagliato e di una stima dell’incertezza riguardo allo sviluppo futuro di capacità e propensioni rilevanti. Analogamente, rimane difficile valutare le soglie a partire dalle quali i modelli di AI sarebbero sufficientemente probabili da compromettere il controllo da giustificare una mitigazione obbligatoria. Anche se le soglie fossero concordate, le capacità potrebbero interagire in modi non ancora ben compresi, rendendo difficile stabilire quando tali soglie siano state superate. In generale, sebbene le evidenze disponibili siano aumentate, non vi è ancora un’evidenza sufficiente per determinare in modo affidabile se e come le capacità e le propensioni di AI di oggi verrebbero scalate e generalizzate fino a comportare un rischio di perdita del controllo in futuro.

###@ Mitigazioni

Sebbene l'allineamento dell'AI in generale resti un problema scientifico aperto (‡697, ‡735, ‡736), i ricercatori stanno iniziando a sviluppare direzioni potenzialmente promettenti per affrontare le cause profonde della disallineamento. Tali direzioni includono, per esempio, diversificare l'ambiente di addestramento e rilevare l'allineamento tramite monitoraggio delle anomalie (‡737, ‡738, ‡739*). Altri ricercatori si concentrano su una migliore comprensione e formalizzazione di meccanismi fondamentali come la misgeneralizzazione degli obiettivi – ad esempio, come gli agenti mantengano capacità ma perseguano obiettivi non intenzionali – per guidare una progettazione migliore di addestramento e valutazione (‡742). Un'altra direzione di ricerca esplora modi per disaccoppiare l'agenzia dalle capacità predittive, come mezzo per creare sistemi di AI non agentici che siano affidabili per progettazione (‡743). Tali sistemi potrebbero poi essere usati come ulteriore livello di supervisione quando vengono impiegati insieme a guardrail meno affidabili contro agenti di AI non fidati.

I ricercatori stanno facendo progressi nello sviluppo di metodi per rilevare e prevenire l’allineamento errato in modo precoce nel processo di sviluppo. Questo lavoro include: tecniche di interpretabilità per esaminare le componenti interne dei sistemi di IA e identificare comportamenti preoccupanti (‡744, ‡745, ‡746); supervisione scalabile (in cui un insieme di sistemi di IA viene utilizzato per supervisionare altri sistemi di IA (‡747)); e metodi di allineamento volti a garantire che i sistemi di IA rimangano reattivi alla supervisione umana (‡748, ‡749).

I ricercatori stanno inoltre sviluppando meccanismi e interventi per gestire sistemi di IA potenzialmente disallineati. Questi includono: il monitoraggio del ‘chain of thought’ che i sistemi di ragionamento producono in segni di disallineamento o output dannosi (‡430, ‡435, ‡750); lo sviluppo di safety case che mirano a dimostrare con alta confidenza che i modelli sono improbabili nel sovvertire misure di controllo (‡751); e il rendere le salvaguardie più robuste contro tentativi di indebolirle (‡725). Il campo emergente del ‘AI control’, tuttavia, resta agli inizi (‡752, ‡753). Le sfide future per i framework di valutazione includono la necessità di monitorare sistemi di IA futuri che sono più capaci e in grado di operare per periodi più lunghi di tempo e in ambienti più complessi.

###@ Sfide per i responsabili politici

I responsabili politici che lavorano sul rischio di perdita del controllo devono prepararsi a un rischio la cui probabilità, natura e tempistica restano incerte. Gli attuali sistemi di AI non pongono rischi immediati di perdita del controllo, ma le decisioni prese oggi determineranno se i sistemi futuri lo faranno. Tali decisioni includono il modo in cui sostenere lo sviluppo di metodi affidabili di valutazione e mitigazione e se debbano esserci regole riguardanti l'accesso e le autorizzazioni concesse ai sistemi di AI in diversi contesti. Nel prendere queste decisioni, i responsabili politici devono affrontare compromessi difficili. Ad esempio, limitare l'impiego di sistemi di AI in ambienti critici può ridurne i benefici, mentre consentire un impiego ampio può aumentare il rischio se le misure di salvaguardia si rivelano insufficienti.

