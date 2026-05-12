##########
>white|orangered|left|14|30|hr Sezione 3.4
### 3.4. Modelli open-weight
>white|orangered|left|24|30|hb Modelli open-weight

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informazioni chiave
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Il livello di accesso che le aziende di AI forniscono ai “pesi” dei loro modelli influisce sui rischi che questi modelli comportano. I pesi sono i parametri matematici che consentono ai modelli di AI di elaborare input e generare output. Per un dato modello, le aziende possono scegliere di mantenere i pesi completamente riservati, fornire a parte degli utenti un accesso limitato o consentire a chiunque di scaricarli integralmente. I modelli i cui pesi sono disponibili pubblicamente sono chiamati “open-weight models”.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ I modelli open-weight facilitano la ricerca e l'innovazione, ma le loro salvaguardie possono essere rimosse più facilmente. In tutto il mondo, vari soggetti – soprattutto quelli con risorse inferiori – possono usare i modelli open-weight per scopi di ricerca e commerciali. Tuttavia, rispetto ai modelli closed-weight, i modelli open-weight sono più facilmente modificabili per esibire comportamenti potenzialmente dannosi, e  s più difficile.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ I rilasci di modelli open-weight sono irreversibili. Una volta rilasciati, i pesi del modello non possono essere richiamati. Questo rende più difficile mitigare i potenziali danni derivanti dal rilascio di un modello con capacità pericolose.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dalla pubblicazione dell’ultimo Rapporto (gennaio 2025), importanti rilasci con pesi aperti hanno ridotto il divario di capacità rispetto ai modelli chiusi leader. Gli sviluppatori cinesi DeepSeek e Alibaba hanno rilasciato rispettivamente i loro modelli R1 e Qwen, che hanno raggiunto prestazioni comparabili a quelle dei modelli chiusi leader, mentre OpenAI ha rilasciato i suoi primi modelli con pesi aperti dal 2019. Le capacità dei modelli chiusi leader sono ora stimate come inferiori di meno di un anno rispetto ai modelli con pesi aperti leader su importanti benchmark di AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Una sfida chiave delle politiche è accedere ai benefici che forniscono i modelli open-weight, gestendo al contempo i loro rischi distintivi. Un approccio consiste nel valutare i modelli open-weight in termini di loro “rischio marginale”: la misura in cui il loro rilascio, in modo controfattuale, aumenta il rischio sociale oltre quello già posto dai modelli esistenti o da altre tecnologie. Tuttavia, questo è complesso nella pratica. Anche piccoli incrementi del rischio marginale nel tempo possono sommarsi fino a determinare aumenti sostanziali del rischio complessivo.
>oldlace|black||11|15|br      


I modelli a pesi open-weight, i cui parametri sono pubblicamente disponibili per il download, hanno implicazioni distinte per molte delle sfide discusse nelle sezioni precedenti. I «pesi» di un modello di AI contengono le informazioni cruciali che gli consentono di generare risposte utili per gli utenti. Una volta rilasciati, questi pesi non possono essere richiamati: chiunque può scaricarli, studiarli, modificarli, condividerli e utilizzarli sui propri computer o account cloud. Quando i pesi sono disponibili in modo aperto, altri possono più facilmente costruire su di essi e modificarli, soddisfacendo esigenze diverse e favorendo l’innovazione (‡1317). Tuttavia, con lo stesso meccanismo, gli utenti con intenzioni malevole possono anche rimuovere più facilmente le misure di salvaguardia e modificare i modelli open-weight per impieghi dannosi (‡1122, ‡1160). Ciò ha sollevato la questione se alcuni modelli open-weight debbano essere soggetti a requisiti speciali (ad es. test più rigorosi prima del rilascio) oppure, in alternativa, ricevere esenzioni speciali (ad es. dall’obbligo di segnalazione regolatoria) (‡1033).

###@ Contesto sui modelli open-weight

>white|orangered||14|15.5|bb I modelli open-weight possono essere, ma non necessariamente, modelli “open source”

Sebbene spesso definiti come ‘open source’, la maggior parte dei modelli rilasciati pubblicamente è più precisamente descritta come ‘open-weight’. Questo perché, sebbene gli sviluppatori forniscano i pesi del modello, non rilasciano il codice di addestramento o i dataset associati. Inoltre, il software open source è in genere caratterizzato da licenze permissive che impongono requisiti minimi agli attori a valle che usano o modificano il software (‡1318). Ad esempio, i modelli Llama di Meta hanno condizioni di licenza restrittive e includono solo codice di inferenza, non codice di addestramento, e quindi in genere non sono considerati open source (‡1319, ‡1320). Le opzioni di rilascio del modello esistono lungo uno spettro che va da completamente chiuso a completamente open source, con diversi compromessi rischio-beneficio in ciascun punto (‡1086*, ‡1320, ‡1321). La Tabella 3.9 descrive queste opzioni.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Completamente chiuso
  Gli utenti non possono interagire direttamente con il modello in alcun modo
  Esempi: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Accesso ospitato
  Gli utenti possono interagire solo tramite una specifica applicazione o interfaccia, come ad esempio un'applicazione mobile di chatbot
  Esempi: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Accesso API al modello
  Gli utenti possono inviare richieste al modello tramite codice, consentendone l’uso in applicazioni esterne
  Esempi: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Accesso API al fine-tuning
  Gli utenti possono ottimizzare ulteriormente il modello per le loro esigenze specifiche
  Esempi: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Open-weight: pesi disponibili per il download
  Gli utenti possono scaricare ed eseguire il modello sui propri computer
  Esempi: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Pesi, dati e codice disponibili per il download con restrizioni d'uso
  Gli utenti possono scaricare e avviare il modello, così come il codice di inferenza e di addestramento, ma ci sono alcune restrizioni di licenza sul loro utilizzo
  Esempi: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Interamente aperto: pesi, dati e codice disponibili per il download senza restrizioni d’uso
  Gli utenti hanno piena libertà di scaricare, usare e modificare il modello, il codice completo e i dati
  Esempi: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.9: Opzioni di condivisione del modello che vanno da completamente chiuse a completamente aperte
>white|black||9|11|br Una selezione illustrativa di opzioni di condivisione dei modelli, che va da modelli completamente chiusi (i modelli sono privati e detenuti solo per uso proprietario) a modelli completamente aperti e open source (i pesi del modello, i dati e il codice sono liberamente e pubblicamente disponibili senza restrizioni di utilizzo, modifica e condivisione). I modelli che rientrano nelle prime quattro categorie sono spesso indicati come «chiusi». Questa sezione si concentra sulle tre righe inferiori. Fonte: adattato da Bommasani, 2024 (‡1317).


###@ Benefici e rischi

>white|orangered|left|14|15.5|bb I modelli open-weight possono essere personalizzati ed valutati più facilmente.

I modelli open-weight offrono vantaggi significativi per la ricerca, l’innovazione e l’accesso. Come discusso in §1.1. Che cos’è l’AI di finalità generale?, addestrare modelli di AI di finalità generale è estremamente costoso – i modelli di punta richiedono centinaia di milioni di dollari per essere sviluppati. Pubblicare in modo aperto i pesi del modello consente ad attori con risorse meno abbondanti di replicare, studiare e costruire a partire da sistemi esistenti. Senza tale accesso, le comunità nelle regioni a bassa disponibilità di risorse rischiano di essere escluse dai benefici dell’AI, rendendo i pesi open fondamentali per abilitare una partecipazione della maggioranza globale allo sviluppo dell’AI (‡1322). Gli sviluppatori a valle possono ottimizzare ulteriormente i modelli per applicazioni diverse, ad esempio adattandoli per lingue minoritarie poco supportate o ottimizzando le prestazioni per compiti specifici come la redazione di atti legali o la presa di note mediche (‡1323, ‡1324*). In questo modo, i modelli open-weight possono permettere a più persone e comunità di usare e trarre vantaggio dall’AI rispetto a quanto sarebbe altrimenti possibile (‡1325). Nel caso di modelli che non sono sufficientemente capaci da risultare pericolosi, questi benefici possono superare il rischio aggiuntivo di rilasciare i pesi in modo aperto, sebbene ciò dipenda dalla tolleranza al rischio dei decisori competenti.

La pubblicazione con pesi open-weight amplia anche la cerchia di sviluppatori e ricercatori in grado di studiare il modello, valutarne le capacità, testare le vulnerabilità e iterare i miglioramenti (‡1326, ‡1327). Ciò rende più probabile l’identificazione sia di applicazioni benefiche sia di gravi difetti dannosi, sebbene questo non sia garantito (‡1328, ‡1329). Gli utenti possono inoltre eseguire modelli open-weight sui propri dispositivi, consentendo loro di mantenere il controllo sui dati sensibili ed evitare di inviarli a server di terze parti.

Ci sono ulteriori vantaggi quando gli sviluppatori condividono informazioni come dati di addestramento, codice, strumenti di valutazione e documentazione oltre ai pesi del modello (‡1320, ‡1330, ‡1331, ‡1332*). Con maggiori informazioni, gli sviluppatori a valle e altri ricercatori possono comprendere meglio i modelli open-weight e adattarli a nuove applicazioni.

>white|orangered|left|14|15.5|bb Le misure di salvaguardia dei modelli open-weight sono più facili da rimuovere, consentendo un potenziale uso malevolo

I modelli open-weight pongono anche ulteriori rischi, perché i loro sistemi di salvaguardia sono più facili da rimuovere. Sebbene sia i modelli open-weight che quelli closed possano avere salvaguardie per rifiutare richieste dell’utente dannose, per i modelli open-weight queste salvaguardie sono molto più facili da rimuovere. Attori malevoli possono mettere a punto (fine-tune) un modello per ottimizzarne le prestazioni per applicazioni dannose, rimuovere parti del codice progettate per prevenire usi dannosi o annullare una precedente messa a punto di sicurezza (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Di conseguenza, i pesi dei modelli open possono aggravare i rischi di uso improprio discussi in §2.1. I rischi derivanti da un uso malevolo, consentendo a un numero maggiore di attori di sfruttare e potenziare capacità esistenti a fini dannosi senza supervisione (‡1122, ‡1315). Sebbene molti utenti non abbiano la competenza o l’incentivo per rimuovere le salvaguardie nei modelli open-weight, gli attori malevoli altamente motivati sono una preoccupazione. Inoltre, gli attori malevoli potrebbero anche essere in grado di usare modelli open-weight per identificare vulnerabilità in modelli closed simili (‡1055*). Tali difetti sono più difficili da individuare facendo girare soltanto modelli closed, a causa del maggiore controllo e delle misure di monitoraggio che i fornitori di modelli closed sono in grado di implementare.

>white|orangered|left|14|15.5|bb La condivisione dei pesi del modello è irreversibile

Una volta che i pesi del modello sono disponibili per il download pubblico, non c'è modo di implementare un rollback generalizzato di tutte le copie esistenti. Le piattaforme di hosting su Internet come GitHub e Hugging Face possono rimuovere i modelli dalle loro piattaforme, rendendo difficile per alcuni attori trovare copie scaricabili e creando una barriera significativa per molti utenti malintenzionati occasionali (‡1339). Tuttavia, gli attori motivati possono comunque ottenere copie se il modello è stato scaricato e riethostato altrove oppure memorizzato localmente. Inoltre, gli sviluppatori a valle che integrano modelli open-weight nei loro sistemi ereditano anche qualsiasi difetto, come vulnerabilità a attacchi avversari (‡1055) o capacità del modello di aggirare i sistemi di monitoraggio (vedi §2.2.2. Perdita di controllo) (‡1315). A differenza dei modelli chiusi, in cui gli host possono distribuire universalmente le correzioni, gli sviluppatori di modelli open-weight non possono garantire che gli aggiornamenti vengano adottati dagli utenti.

###@ Aggiornamenti

Dalla pubblicazione dell’ultimo Rapporto (Gennaio 2025), il divario di capacità tra modelli open-weight leader e modelli closed si è ridotto. Gli sviluppatori cinesi sono diventati in particolare fornitori importanti di modelli open-weight. Nel gennaio 2025 DeepSeek ha rilasciato il modello R1, che ha ottenuto prestazioni comparabili a quelle di o1 di OpenAI su una serie di benchmark (‡1340). I modelli Qwen di Alibaba hanno ugualmente guadagnato terreno, occupando la prima posizione per un modello open-weight su Chatbot Arena, un benchmark di prestazioni ampiamente utilizzato, a partire da agosto 2025 (‡1341, ‡1342*). Nel agosto 2025 OpenAI ha rilasciato i suoi primi modelli open-weight dopo il rilascio di GPT-2 nel 2019, gpt-oss-120b e gpt-oss-20b. Meta ha continuato a rilasciare modelli Llama con pesi aperti. Si stima che le capacità dei modelli closed leader siano ora inferiori a un anno di distanza rispetto ai modelli open leader nei principali benchmark di AI (Figura 3.10).

###@ Lacune di evidenza

Una lacuna cruciale nelle evidenze riguarda l’efficacia nel mondo reale delle soluzioni tecniche per prevenire l’uso improprio dei modelli open-weight. I ricercatori hanno proposto vari approcci per rendere i modelli resistenti alle manomissioni. Questo include nuove tecniche di addestramento progettate per rendere i modelli resistenti a modifiche dannose (‡1276), il filtraggio dei contenuti dannosi dai dati di addestramento (‡55) e difese contro i jailbreak (‡675, ‡676). Queste tecniche vengono ora adottate in rilasci nel mondo reale da parte di sviluppatori di primo piano. Per esempio, OpenAI ha impiegato alcune di queste tecniche nei suoi modelli gpt-oss, riportando che le versioni sottoposte a fine-tuning avversariale non raggiungevano soglie di elevata capacità (‡1344*). Tuttavia, la ricerca ha dimostrato che soggetti malevoli possono disabilitare i sistemi di salvaguardia riaddestrando i modelli su esempi dannosi (‡1345, ‡1346). Inoltre, è ancora difficile valutare in modo affidabile la robustezza delle salvaguardie, rendendo incerta la loro efficacia contro gli attacchi nel mondo reale (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figura 3.10: Divario di capacità tra i modelli di AI open-weight leader e i modelli di AI closed
>white|black||9|11|br Punteggi dell’Epoch Capabilities Index (ECI) dei modelli open-weight con prestazioni migliori (blu scuro) e dei modelli closed (blu chiaro) nel tempo. L’ECI combina i punteggi di 39 benchmark in una singola scala generale delle capacità. I migliori modelli open-weight sono in ritardo di circa un anno rispetto ai modelli closed. Fonte: Epoch AI, 2025 (‡1343).


###@ Mitigazioni

Le mitigazioni tecniche per i rischi dei modelli open-weight operano durante l'intero processo di sviluppo e distribuzione dell'AI (‡1141, ‡1195, ‡1347). Ad esempio, durante lo sviluppo dei modelli, gli sviluppatori e gli adattatori a valle possono filtrare i contenuti sensibili dai dati di addestramento per minimizzare le capacità dannose. Rimuovere esempi dannosi dai dati di addestramento di un modello può prevenire il fine-tuning avversario in modo 10 volte più efficace rispetto alle difese aggiunte dopo l'addestramento, anche se può a sua volta incidere sulle capacità benefiche (‡55). I fornitori di applicazioni AI possono inoltre implementare meccanismi di segnalazione e risposta agli incidenti (‡1348).

Inoltre, piattaforme di hosting come HuggingFace e GitHub possono stabilire termini di servizio della piattaforma per rimuovere modelli modificati per scopi dannosi (‡1141, ‡1324). Gli sviluppatori del modello possono fornire accesso completo agli revisori prima del rilascio, oppure adottare una strategia di rilascio “a fasi” – rilasciando i modelli a gruppi via via più ampi (‡1086). Questo può aiutare a identificare potenziali malfunzionamenti o vulnerabilita prima che un modello sia ampiamente disponibile (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Riquadro 3.1: Sicurezza dei pesi del modello
>oldlace|black|left|13|15|hb Riquadro 3.1: Sicurezza del peso del modello
>oldlace|black||11|15|br      
>oldlace|black||11|15|br I rischi discussi in questa sezione presuppongono che i pesi del modello vengano rilasciati intenzionalmente. Tuttavia, anche i pesi di modelli chiusi possono diventare accessibili tramite furto o fuoriuscita di dati. I modelli chiusi costano centinaia di milioni di dollari per essere sviluppati (§1.1. What is general-purpose AI?) e, in media, sono più capaci dei modelli con pesi aperti (‡1343). Questo li rende bersagli attraenti per attori che vanno dagli hacker amatoriali fino agli stati-nazione che cercano di ottenere i modelli AI leader.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Le chiavi (weights) chiuse del modello sottratte comporterebbero rischi simili a quelli descritti sopra per i modelli con pesi open, ma potenzialmente senza nessuna delle mitigazioni. Gli attori malevoli potrebbero rimuovere le misure di salvaguardia dai modelli più capaci. A differenza dei sviluppatori legittimi, tali attori non dovrebbero affrontare i vincoli reputazionali, legali o commerciali che attualmente incentivano le aziende di AI di frontiera a distribuire i propri modelli in modo sicuro.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br I livelli di sicurezza attuali variano nel settore e possono risultare insufficienti contro avversari sofisticati. Alcuni sviluppatori si impegnano a proteggere i pesi del modello contro i gruppi criminali informatici e le minacce interne (‡582), mentre altri non hanno assunto alcun impegno di sicurezza pubblico (‡1109, ‡1349). La ricerca indica che i data centre di AI potrebbero non essere in grado di resistere ad attacchi da parte degli attori più sofisticati e ben dotati di risorse (‡582, ‡1350, ‡1351). A dicembre 2025, non esistono istanze confermate e documentate pubblicamente di furto dei pesi del modello. Tuttavia, sono state segnalate altre violazioni della sicurezza presso aziende leader nel settore dell’AI, inclusa un’infiltrazione nei sistemi di posta elettronica di Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br La chiusura di queste lacune di sicurezza richiederebbe investimenti sostanziali in hardware, software, personale e sicurezza delle strutture. Alcuni miglioramenti della sicurezza potrebbero essere implementati relativamente rapidamente con uno sforzo coordinato (‡1122). Altre misure critiche, tuttavia, come mettere in sicurezza le catene di fornitura dell’hardware e le strutture, richiederebbero probabilmente anni (‡1122). Le aziende private possono inoltre non disporre delle risorse o delle informazioni necessarie per sviluppare adeguate protezioni da sole. Ad esempio, gli sviluppatori di AI non hanno l’accesso alle informazioni riservate sulle minacce che hanno i governi (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Sfide per i responsabili delle politiche

Una sfida fondamentale per i responsabili politici è garantire i benefici della condivisione dei modelli open-weight senza aumentare in modo significativo il rischio. Per evitare danni catastrofici, gli sviluppatori di modelli open-weight non dovrebbero rilasciare modelli senza valutarne i rischi, sia utilizzando metodi di valutazione consolidati impiegati per i modelli closed, sia tramite ulteriori test, considerando che soggetti maleintenzionati possono mettere a punto (fine-tune) i modelli e rimuovere le protezioni di sicurezza. In pratica, ciò può risultare difficile perché gli sviluppi delle capacità possono essere imprevedibili, i rilasci open-weight sono irreversibili e sono necessari sforzi di valutazione per prevedere quando un rilascio comporterebbe un potenziale danno significativo. Un approccio consiste nel valutare il “rischio marginale” delle release open: in che misura la release controfattualmente accresce il rischio per la società oltre quello già posto da modelli esistenti o da altre tecnologie (‡556, ‡1033, ‡1354, ‡1355) (vedi §3.2. Pratiche di gestione del rischio). Tuttavia, stimare come un sistema aumenterà o ridurrà il rischio a valle dopo la sua distribuzione è complesso e dipende dal contesto. Incrementi incrementali del rischio con rilasci successivi possono sommarsi nel tempo fino a determinare aumenti sostanziali del rischio totale, anche se il rischio marginale associato a ciascuna release appare accettabile (‡1356, ‡1357). La natura dual-use delle capacità dell’AI complica ulteriormente la governance: funzionalità che abilitano applicazioni benefiche in medicina o nella ricerca possono essere rimesse a nuovo (repurposed) per arrecare danni e, una volta che i pesi sono pubblici, distinguere usi legittimi da usi malevoli può essere difficile. Inoltre, non è chiaro a chi debba essere attribuita la responsabilità quando i modelli open-weight vengono modificati per finalità dannose.

