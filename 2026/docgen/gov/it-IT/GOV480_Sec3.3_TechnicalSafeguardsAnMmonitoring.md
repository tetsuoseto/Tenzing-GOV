##########
>white|orangered|left|14|30|hr Sezione 3.3
### 3.3. Misure tecniche di sicurezza e monitoraggio
>white|orangered|left|24|30|hb Misure di salvaguardia tecniche e monitoraggio

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informazioni chiave
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ È utilizzata un’ampia gamma di salvaguardie tecniche in diverse fasi dello sviluppo e dell’uso dell’AI. Queste includono tecniche applicate durante lo sviluppo del modello per rendere i sistemi più robusti e resistenti a usi impropri (come la curation dei dati), il monitoraggio e il controllo in fase di deployment (come il filtraggio dei contenuti e la supervisione umana) e strumenti post-deployment per monitorare l’ecosistema AI più ampio (come la provenance e il rilevamento dei contenuti).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Le misure di salvaguardia tecniche hanno dei limiti e non impediscono in modo affidabile comportamenti dannosi in tutti i contesti. Ad esempio, a volte gli utenti possono ottenere output dannosi riformulando le richieste o scomponendole in passaggi più piccoli. In modo analogo, strumenti come l’watermarking, progettati per identificare i contenuti generati da AI, spesso possono essere rimossi o alterati, il che ne limita l’affidabilità.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ I limiti dei singoli controlli di salvaguardia significano che potrebbe essere necessario un approccio di «difesa in profondità» per prevenire alcuni esiti dannosi. Ad esempio, un sistema potrebbe combinare un modello addestrato alla sicurezza con filtri di input, filtri di output e monitor dei contenuti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dalla pubblicazione dell’ultimo Report (Gennaio 2025), i ricercatori hanno compiuto progressi nel miglioramento delle misure di salvaguardia, ma permangono limitazioni fondamentali. Ad esempio, il tasso di successo degli attacchi progettati per aggirare le salvaguardie è diminuito, ma resta relativamente alto. Esistono inoltre limitazioni fondamentali su quanto a fondo i modelli con pesi open-weight possano essere protetti da salvaguardie.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Una sfida chiave per i responsabili politici è la limitata evidenza su quanto siano efficaci le misure di salvaguardia in diversi usi reali di sistemi di AI a uso generale. Gli sviluppatori di AI differiscono ampiamente in merito a quante informazioni condividono sulle loro misure di salvaguardia e sul monitoraggio. Una sfida ulteriore riguarda i potenziali compromessi tra l’applicazione di salvaguardie più robuste e il mantenimento delle prestazioni o dell’utilità del sistema.
>oldlace|black||11|15|br      


Gli sviluppatori di AI possono utilizzare diversi utili ma imperfetti sistemi di salvaguardia tecnici per mitigare e gestire i rischi derivanti da sistemi di AI a scopo generale, ma persistono sfide di robustezza. Gli sviluppatori non riescono ancora a impedire completamente ai sistemi di AI a scopo generale di compiere azioni persino note e palesemente dannose, come fornire agli utenti istruzioni per commettere crimini. Ad esempio, i ricercatori hanno dimostrato che le salvaguardie all’avanguardia possono essere aggirate tramite metodi di prompting avversario (cioè ‘jailbreaks’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), facendo sì che i modelli scompongano compiti dannosi complessi in passaggi (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), e con semplici modifiche del modello (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). I ricercatori continuano a lavorare su salvaguardie contro malfunzionamenti e usi impropri (‡690). Questi metodi variano ampiamente per finalità ed efficacia e il loro impatto dipende in ultima analisi dal più ampio contesto sociotecnico e di governance in cui i sistemi di AI sono progettati e distribuiti.

Le misure di salvaguardia tecniche possono essere suddivise in tre categorie: tecniche per sviluppare modelli più sicuri; tecniche utilizzate durante l’esercizio per il monitoraggio e il controllo; e tecniche che supportano il monitoraggio dell’ecosistema successivo al deployment. La Tabella 3.6 riassume le salvaguardie tecniche discusse, la loro efficacia e le sfide aperte.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Sviluppare modelli più sicuri
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Curation dei dati (‡1167)
  Rimuovere dati dannosi per impedire a un modello di apprendere capacità pericolose. Questi metodi possono essere utili, anche per sviluppare modelli open-weight che non dispongono di capacità dannose e resistono a un fine-tuning dannoso (‡55). Tuttavia, ci sono sfide legate a errori di curation e al ridimensionamento (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Apprendimento per rinforzo da feedback umano (‡64*)
  Addestrare il modello per allinearsi a obiettivi specifici, come essere utile e innocuo. Questo è un modo efficace per far sì che i modelli imparino comportamenti vantaggiosi (‡64*). Tuttavia, un'eccessiva ottimizzazione per l'approvazione umana può indurre i modelli a comportarsi in modo ingannevole o adulatorio (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tecniche di allineamento pluralistico (‡1170)
  Addestrare il modello per integrare molteplici punti di vista differenti su come dovrebbe agire. Queste tecniche aiutano a ridurre l’entità con cui i modelli favoriscono specifici punti di vista (‡1170). Tuttavia, nonostante queste tecniche, il disaccordo umano è inevitabile e risulta difficile progettare modalità ampiamente accettate per bilanciare prospettive concorrenti (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Addestramento avversario (‡677)
  Addestrare il modello a rifiutare di causare danni (anche in contesti non familiari) e a resistere ad attacchi da parte di utenti malevoli (ad es. “jailbreaks”). Questo è un metodo efficace per far sì che i modelli resistano ai tentativi di uso improprio (‡1064), ma le sfide di robustezza persistono (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Macchina “unlearning” (‡1175, ‡1176)
  Addestrare un modello utilizzando algoritmi specializzati significava sopprimere attivamente capacità dannose (ad es. la conoscenza di rischi biologici). Queste tecniche offrono un modo mirato per rimuovere capacità dannose dai modelli (‡1175, ‡1176), ma gli algoritmi di unlearning attuali possono non essere robusti e avere effetti indesiderati su altre capacità (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strumenti di interpretabilità e verifica della sicurezza (‡1177)
  Una famiglia eterogenea di metodi di progettazione e verifica, pensati per offrire una garanzia più rigorosa del fatto che i modelli presentino specifiche proprietà legate alla sicurezza. Consentono ai valutatori di ottenere garanzie di sicurezza più affidabili (‡1177), ma i metodi attuali si basano su assunzioni e raramente sono competitivi in termini di prestazioni nella pratica (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Monitoraggio e controllo
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meccanismi di monitoraggio basati su hardware (‡1179, ‡1180, ‡1181)
  Verificare che i processi autorizzati siano in esecuzione sull'hardware al fine di studiare le minacce alla sicurezza o la conformità normativa. Questi meccanismi offrono modi unici per monitorare quali calcoli vengono eseguiti sull'hardware e da chi (‡1181). Tuttavia, i meccanismi hardware non possono monitorare tutti i tipi di minacce e alcune tecniche richiedono hardware specializzato (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio dell’interazione utente (‡1154, ‡1166)
  Il monitoraggio delle interazioni degli utenti per individuare segnali di utilizzo dannoso può aiutare gli sviluppatori a interrompere il servizio per gli utenti malevoli (‡1154, ‡1166). Tuttavia, l’applicazione delle misure può, inavvertitamente, ostacolare la ricerca benefica sulla sicurezza (‡689) e alcune forme di abuso sono difficili da rilevare (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio dell'interazione dell'utente (‡1154, ‡1166)
  Monitorare le interazioni degli utenti per individuare segnali di uso dannoso può aiutare gli sviluppatori a terminare il servizio per utenti malevoli (‡1154, ‡1166). Tuttavia, l’applicazione delle policy può, inavvertitamente, ostacolare la ricerca benefica sulla sicurezza (‡689) e alcune forme di abuso sono difficili da rilevare (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filtri dei contenuti (‡65*, ‡725)
  Filtrare gli input e gli output potenzialmente dannosi del modello è un modo molto efficace per ridurre i danni accidentali e i rischi di uso improprio (‡725). Tuttavia, i filtri richiedono capacità di calcolo aggiuntive e sono vulnerabili ad alcuni attacchi (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio del calcolo interno del modello (‡744, ‡1183, ‡1184)
  Il monitoraggio di segnali di inganno o di altre forme dannose di cognizione interna nei modelli può essere un modo efficiente per rilevare l’inganno (‡744, ‡1183, ‡1184). Tuttavia, i metodi attuali mancano di robustezza e affidabilità (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitoraggio del ragionamento a catena (‡430, ‡435)
  Il monitoraggio del testo del chain-of-thought di una catena di modelli per individuare segnali di comportamento fuorviante o altre forme di ragionamento dannoso è un modo efficace per comprendere e identificare difetti nel modo in cui i modelli ragionano (‡435). Tuttavia, possono essere inaffidabili (‡752, ‡753, ‡1186) e, se i modelli vengono addestrati a produrre un chain of thought benigno, possono imparare comportamenti fuorvianti (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Umano nel ciclo (‡1187, ‡1188, ‡1189)
  La supervisione umana e le sostituzioni (override) per le decisioni del sistema sono essenziali in alcune applicazioni ad alta criticità per la sicurezza (‡1187). Tuttavia, queste tecniche sono limitate dal bias dell’automazione e dai limiti alla velocità del processo decisionale umano (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sandboxing (‡1192)
  Impedire a un agente AI di influenzare direttamente il mondo è un modo efficace per limitare il danno che può causare (‡1192). Tuttavia, il sandboxing limita la capacità del sistema di portare direttamente a termine determinati compiti (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Strumenti per facilitare il monitoraggio dell'ecosistema
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tecniche di identificazione dei modelli di AI (‡1193*, ‡1194)
  Rendere i modelli, o le singole istanze di modelli, più facili da identificare in scenari di utilizzo nel mondo reale aiuta con la digital forensics e la consapevolezza dell'ecosistema (‡1195). Tuttavia, queste tecniche possono essere aggirate con alcuni tipi di modifiche del modello (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inferenza dell’eredità del modello di AI (‡1197)
  Queste tecniche consentono ai ricercatori di studiare come i modelli vengono modificati nell'ecosistema dell'AI, soprattutto i modelli open-weight. Aiutano per la digital forensics e la consapevolezza dell'ecosistema (‡1198), ma sarebbero necessari progetti su larga scala per mappare in modo esaustivo l'ecosistema dei modelli open-weight (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Watermark e metadati (‡1199, ‡1200, ‡1201*)
  Queste tecniche rendono più facile rilevare quando un pezzo di testo, immagine, video, ecc., è stato generato o modificato dall’IA e da quale sistema. Facilitano una migliore consapevolezza dell’ecosistema (‡1199, ‡1200, ‡1201*). Tuttavia, i watermark e i metadati possono essere falsificati o rimossi mediante alcune modifiche al contenuto (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rilevamento di contenuti generati dall'AI (‡1203, ‡1204, ‡1205*)
  Migliorare la capacità degli utenti di distinguere tra contenuti generati da AI e contenuti genuini aiuta nella digital forensics e nella consapevolezza dell'ecosistema (‡1203, ‡1204). Tuttavia, i classificatori possono essere inaffidabili (‡1205*) e presentare prestazioni variabili tra le diverse modalità.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.6: Garanzie tecniche discusse in questa sezione
>white|black||9|11|br Un riepilogo delle misure di salvaguardia tecniche discusse in questa sezione, suddivise in metodi per sviluppare modelli più sicuri, monitoraggio e controllo in fase di distribuzione e tecniche per facilitare il monitoraggio dell’ecosistema.


###@ Sviluppare modelli più sicuri

Una prima linea di difesa contro i danni derivanti da sistemi di AI a uso generale è rendere più sicuro il modello sottostante. Questa sottosezione tratta le misure di salvaguardia che sono “incorporate nei parametri del modello” durante il processo di sviluppo del modello (Figura 3.6).

>white|orangered|left|14|15.5|bb La selezione dei dati di addestramento può limitare lo sviluppo di capacità potenzialmente pericolose

I modelli di AI generica sono utili proprio perché sviluppano un’ampia gamma di conoscenze e capacità dopo aver elaborato i dati di addestramento, ma alcuni tipi di dati di addestramento sono in modo sproporzionato responsabili dello sviluppo di capacità potenzialmente pericolose. Per esempio, un modello di AI addestrato su articoli di virologia potrebbe essere in grado in modo migliore di fornire assistenza in compiti di biologia potenzialmente dannosi (‡549, ‡1206*) (vedere anche §2.1.4. Rischi biologici e chimici). Inoltre, i generatori di immagini/video addestrati su immagini di nudità umana possono anche essere usati in modo improprio per creare deepfake intimi senza consenso (‡308, ‡319) (vedere anche §2.1.1. Contenuti generati dall’AI e attività criminale).

Filtrare i dati di addestramento è una mitigazione efficace contro alcune capacità indesiderate (‡319, ‡1167, ‡1207, ‡1208). Tuttavia, può essere difficile filtrare i grandi dataset utilizzati per addestrare modelli di AI a scopo generale (‡1168) a causa di costi elevati (‡1209), errori di filtraggio (‡1210) e impatti negativi sulla qualità del dataset (‡1211). Queste sfide sono aggravate dalla natura multilingue del testo su internet (‡1212), dai bias culturali nella moderazione dei contenuti (‡1211, ‡1213, ‡1214, ‡1215) e dal fatto che stabilire se un determinato dato sia “dannoso” dipende da fattori contestuali (‡1216). Ciononostante, filtrare potenziali materiali dannosi dai dati di addestramento mostra promesse per rendere i modelli in modo più affidabile sicuri, incluso rendere i modelli con pesi open-weight più resistenti a manomissioni dannose (‡55). Le relazioni tra i contenuti dei dati di addestramento e le capacità emergenti dei modelli non sono ancora pienamente comprese (‡1195) e il filtraggio sembra essere più efficace nel limitare capacità dannose quando viene applicato a domini di conoscenza ampi (‡55) rispetto a comportamenti più ristretti (‡1206, ‡1217). Vedi §3.4. Modelli open-weight per ulteriori discussioni.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figura 3.6: Dove applicare le salvaguardie tecniche
>white|black||9|11|br Le misure di salvaguardia tecniche possono essere applicate in diverse fasi dello sviluppo del modello. La preparazione e curation dei dati (data curation) definisce ciò che i modelli apprendono durante il pre-training e il fine-tuning. I metodi basati sull’addestramento, come il reinforcement learning da feedback umano e l’addestramento alla robustezza, adeguano il comportamento del modello. I metodi di test, come gli attacchi avversari, identificano le vulnerabilità residue. Alcune tecniche, come gli algoritmi safe-by-design, attraversano più fasi. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb I metodi per addestrare modelli di AI generica affinché siano utili e innocui principalmente si basano sul feedback umano

È difficile addestrare e valutare modelli in modo affidabile per allinearli a principi di alto livello come essere di aiuto, non arrecare danni e essere onesti. Nella pratica, gli sviluppatori mirano a ottenere questo risultato perfezionando (fine-tuning) i modelli di AI usando dimostrazioni e feedback da parte degli esseri umani. Ad esempio, il paradigma principale per il fine-tuning dei modelli di AI, noto come ‘reinforcement learning from human feedback’, si basa sull’addestramento dei modelli per produrre output che gli annotatori umani valutano positivamente (‡1218). Tuttavia, il feedback positivo da parte degli esseri umani è un proxy difettoso per il comportamento benefico (‡737, ‡878, ‡1219, ‡1220) ed è limitato da errori e bias umani (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Questo porta a diverse sfide: modelli messi a punto tramite reinforcement leaning from human feedback a volte adattano la risposta per compiacere l’utente, un comportamento noto come ‘sycophancy’ (‡358, ‡740, ‡1226, ‡1227); fornire risposte che siano utili in alcuni contesti ma dannose in altri (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); fornire risposte difficili da valutare per la correttezza (‡1233); oppure eseguire azioni la cui utilità o dannosità è una questione di opinione (‡1234). La Tabella 3.7 fornisce esempi di queste sfide. Alcune ricerche mirano a sviluppare metodi per aiutare gli esseri umani a valutare meglio le soluzioni a compiti complessi con l’assistenza dell’AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tuttavia, questi metodi al momento hanno un’affidabilità limitata e non è pubblicamente noto in che misura vengano utilizzati per addestrare i modelli AI più avanzati di oggi.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adulazione/accoglienza servile (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Spiegazione:
>white|black|left|11|13|br Il modello fornisce solo feedback positivi, senza riuscire a evidenziare la mancanza di una corretta struttura di sillabe dell’haiku 5-7-5.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alcune azioni sono utili in alcuni contesti ma dannose in altri (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Spiegazione:
>white|black|left|11|13|br Le informazioni sul rischio biologico possono essere usate per l’educazione e la difesa, ma anche per informare gli attori malintenzionati.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Il comportamento corretto è difficile da verificare (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Spiegazione:
>white|black||11|13|br La correttezza di questa risposta è difficile da valutare perché richiede competenze mediche. Anche per un medico esperto, valutare risposte come questa richiede tempo e un’attenzione accurata ai dettagli.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Gli esseri umani non concordano su ciò che è corretto (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Spiegazione:
>white|black|left|11|13|br Le persone non concordano in modo significativo su qual è la risposta corretta.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.7: Prompt utente e risposta del modello AI
>white|black||9|11|br Esempi di sfide nel definire e incentivare azioni benefiche da parte dei modelli di AI.


>white|orangered|left|14|15.5|bb Gli esseri umani non sono sempre d'accordo su quali comportamenti siano auspicabili, rendendo necessari metodi per bilanciare preferenze concorrenti

Gli esseri umani non concordano sempre su quali risposte o azioni i modelli di AI dovrebbero o non dovrebbero produrre (‡1006). Questo rende fondamentalmente difficile sviluppare modelli le cui azioni e i cui impatti siano in generale allineati agli interessi della società (‡420). Alcuni ricercatori studiano di quali preferenze siano in parte rappresentate nei sistemi di AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) e lavorano per sviluppare tecniche di 'allineamento pluralistico' che mirano a trovare un equilibrio tra preferenze concorrenti (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Ad esempio, gli sviluppatori di AI possono progettare sistemi per evitare di generare risposte controverse rifiutando di rispondere a determinate richieste, oppure allinearsi alla visione mediana in un certo campione rilevante di persone, oppure personalizzare i sistemi per utenti individuali.

Una sfida comune di questi approcci è che, in generale, i sistemi di IA non possono allinearsi in modo equo alle preferenze di tutti e che i loro impatti sociali a valle influenzeranno gruppi diversi di persone in modo differente. Alcuni ricercatori hanno sostenuto che la maggior parte degli approcci tecnici all’allineamento pluralistico non affronta le sfide più profonde, e potenzialmente le distoglie, da criticità quali bias sistematici, dinamiche di potere sociale e la concentrazione di ricchezza e influenza (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Gli sviluppatori di AI usano l’«addestramento avversario» per migliorare la robustezza del modello

È difficile garantire che i modelli di AI traducano in modo robusto i comportamenti benefici che apprendono durante l’addestramento ai contesti di distribuzione nel mondo reale. Anche i modelli addestrati con un segnale di apprendimento “perfetto” possono fallire nel generalizzare con successo a tutti i contesti non visti (‡738, ‡739, ‡1255, ‡1256, ‡1257). Per esempio, alcuni ricercatori hanno scoperto che i chatbot hanno maggiori probabilità di compiere azioni dannose nelle lingue che sono scarsamente rappresentate nei loro dati di addestramento (‡159, ‡880, ‡1258*, ‡1259), che includono molte lingue parlate prevalentemente nel Global South.

Negli ultimi anni i ricercatori hanno anche creato un ampio toolkit di tecniche di “attacco avversario” che possono essere usate per far generare ai modelli risposte potenzialmente dannose (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Per esempio, una recente iniziativa ha raccolto tramite crowd-sourcing oltre 60,000 esempi diversi di attacchi riusciti contro modelli AI all’avanguardia, che li hanno portati a violare le policy delle loro aziende sul comportamento accettabile del modello (‡1149). La Tabella 3.8 mostra esempi di tecniche di “jailbreak” che i ricercatori hanno dimostrato essere in grado di indurre i modelli ad assecondare richieste dannose.

Un metodo per migliorare la robustezza dei modelli è noto come 'adversarial training' (‡1064). Esso consiste nel costruire 'attacchi' (ad es. jailbreaks) progettati per indurre un modello ad agire in modo indesiderato, e nel addestrare il modello a gestire questi attacchi in modo appropriato. Tuttavia, l'adversarial training è imperfetta (‡1260, ‡1261). Gli attaccanti riescono costantemente a sviluppare nuovi attacchi efficaci contro modelli all'avanguardia (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Poiché gli sviluppatori richiedono esempi specifici di modalità di fallimento per addestrarsi contro di esse (‡512, ‡1263), il risultato è un continuo gioco del 'gatto e il topo', in cui gli sviluppatori aggiornano continuamente i modelli in risposta a vulnerabilità appena scoperte, e gli avversari cercano continuamente nuovi attacchi. Alcuni ricercatori hanno proposto un'adversarial training su scala maggiore (‡1264, ‡1265) o nuovi algoritmi (‡675, ‡676, ‡1263, ‡1266, ‡1267) per migliorare la robustezza, ma i moderni sistemi di AI restano in modo persistente vulnerabili.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: effettua richieste dannose in testo cifrato, come codice Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: preimpostare il sistema con esempi di risposte conformi a richieste dannose (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Effettuare richieste dannose in lingue a basse risorse che probabilmente sono meno utilizzate nell’addestramento (ad es. Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: scomporre un’attività dannosa in più sottocompiti innocui (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabella 3.8: Strategie di jailbreak
>white|black||9|11|br Attori malintenzionati e red teams hanno utilizzato vari tipi di “jailbreaks” per far sì che i modelli di IA rispettino richieste dannose che normalmente rifiuterebbero a causa delle salvaguardie. Gli output di esempio erano stati scritti dagli autori del Report a scopo illustrativo. Molti attuali modelli di IA all’avanguardia ora resistono alla maggior parte di questi metodi, ma continuano a essere scoperte nuove tecniche di jailbreaking.


>white|orangered|left|14|15.5|bb Le tecniche di “unlearning” possono mitigare specifiche capacità dannose del modello

Un'altra strategia per mitigare i rischi dell'AI a uso generale consiste nel sottoporre i modelli a fine-tuning affinché manchino di determinate capacità in specifici domini ad alto rischio (‡1175, ‡1176). Ad esempio, i ricercatori stanno lavorando allo sviluppo di algoritmi di ‘machine unlearning’ in grado di sopprimere in modo mirato abilità legate a minacce biologiche o alla generazione di immagini fotorealistiche di corpi umani nudi (‡903, ‡1272, ‡1273). Questi metodi possono rendere i modelli in modo sostanziale più sicuri, a costo di limitare alcune utilizzazioni positive delle capacità sottoposte a unlearning. Limitare la conoscenza dei modelli di AI in domini dannosi è stato anche proposto come modo per progettare modelli open-weight ‘tamper-resistant’ che possano resistere a fine-tuning dannosi (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Finora, tuttavia, è stato difficile farlo in modo robusto (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Vedi §3.4. Modelli open-weight per ulteriori discussioni.

>white|orangered|left|14|15.5|bb Alcuni ricercatori stanno lavorando a metodi per garanzie di sicurezza più robuste attraverso l’interpretazione degli stati interni del modello o la verifica matematica

Alcuni ricercatori stanno lavorando su metodi per verificare in modo più rigoroso le proprietà di sicurezza dei modelli. In un approccio, i ricercatori mirano a interpretare i calcoli interni dei modelli per individuare rischi o per formulare argomentazioni più convincenti sul fatto che il modello sia sicuro (‡1285, ‡1286). Ad esempio, in un proof of concept, i ricercatori hanno mostrato che strumenti per analizzare la computazione interna di un language model possono aiutare i valutatori a identificare comportamenti dannosi (‡1287). Nel 2025, anche Anthropic ha iniziato ad analizzare gli interni del modello come modo per studiare la situational awareness del modello e il suo ‘intent’ (‡2). Tuttavia, questi tipi di metodi non sono attualmente comuni o noti come competitivi rispetto ad altre tecniche di valutazione.

Un approccio diverso per ottenere garanzie più solide di sicurezza consiste nel costruire prove matematiche secondo cui un modello soddisferà determinate condizioni di sicurezza (‡1177, ‡1282, ‡1288). Tuttavia, tali prove presuppongono che il contesto di test corrisponda al contesto di distribuzione e non sono state verificate rispetto a molte tipologie di avversari.

Inoltre, al momento non possono nemmeno essere scalati a modelli di grandi dimensioni. In generale, c'è un acceso dibattito tra gli esperti sulla promessa della interpretabilità e dei metodi di verifica formale.

###@ Monitoraggio e controllo in fase di distribuzione

Oltre alle salvaguardie implementate durante lo sviluppo del modello, una seconda linea di difesa contro comportamenti dannosi è rappresentata da salvaguardie esterne che si concentrano sul monitoraggio e sul controllo delle azioni di un modello o di un sistema durante la distribuzione. Tali salvaguardie aiutano a mitigare malfunzionamenti e usi impropri, come output allucinati e istruzioni dannose.

>white|orangered|left|14|15.5|bb I deployer del modello possono utilizzare una varietà di strumenti per identificare e affrontare comportamenti ad alto rischio del modello

Quando un sistema AI è in esecuzione, un deployer può monitorare i segnali di rischio e intervenire se si presentano. Ad esempio, può ispezionare gli input di un modello per individuare segni di attacchi avversariali, filtrare contenuti inappropriati dalle uscite o monitorare la chain of thought del sistema per rilevare segni di piani dannosi. I punti in cui i deployer possono monitorare e intervenire su come le persone utilizzano i loro sistemi includono l’hardware (‡1180, ‡1181), le interazioni con l’utente (‡1154, ‡1166), gli input e le uscite (‡65, ‡725, ‡1182), i calcoli interni (‡744, ‡1183, ‡1184) e la chain of thought (‡430, ‡435). Esistono anche molte azioni che i deployer possono intraprendere quando vengono identificati rischi. Queste includono la registrazione di informazioni, il filtraggio/modifica di contenuti dannosi, la segnalazione di attività anomale, gli arresti del sistema o l’attivazione di meccanismi di failsafe. La Figura 3.7 illustra esempi di meccanismi comuni di monitoraggio e controllo.

Poiché sono versatili e spesso efficaci, questi meccanismi sono ampiamente usati e possono prevenire molte forme di danni non intenzionali (‡725, ‡751, ‡1289). Tuttavia, queste salvaguardie sono imperfette, soprattutto in caso di attacchi malevoli ottimizzati per farle fallire (‡752, ‡1182). Ricerche recenti hanno inoltre esplorato come il monitoraggio possa risultare inaffidabile se un sistema è ottimizzato utilizzando i punteggi di un monitor, ad esempio rendendo il chain of thought meno affidabile (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figura 3.7: Tecniche di monitoraggio e controllo
>white|black||9|11|br Le tecniche di monitoraggio e controllo operano in più punti: analisi degli input e degli output per contenuti dannosi, tracciamento degli stati interni del modello, limitazione delle azioni esterne tramite sandboxing e mantenimento della supervisione umana. Fonte: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Gli esseri umani nel ciclo consentono una supervisione diretta in contesti ad alto rischio

Per ridurre la probabilità di guasti da parte degli agenti AI (vedi §2.2.1. Sfide di affidabilità), i responsabili della distribuzione possono puntare a progettare sistemi AI che funzionino in cooperazione con gli esseri umani piuttosto che in modo completamente autonomo (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Questo è importante per i casi d’uso in cui decisioni errate possono causare danni significativi, come in ambito finanziario, sanitario o di polizia. Tuttavia, avere un “essere umano nel ciclo” è spesso impraticabile. A volte il processo decisionale avviene troppo rapidamente, come nelle applicazioni di chat con milioni di utenti. In altri casi, i bias e gli errori umani possono amplificare i rischi a causa di errori composti (‡1187). Gli esseri umani nel ciclo tendono inoltre a mostrare “bias da automazione”, il che significa che spesso ripongono più fiducia nel sistema AI di quanto sia giustificato (‡1190, ‡1191) (vedi §2.3.2. Rischi per l’autonomia umana).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ protegge dai rischi derivanti da comportamenti autonomi

Agenti AI in grado di agire in modo autonomo senza limitazioni sul Web o nel mondo fisico comportano rischi elevati (vedere §2.2.1. Sfide di affidabilità). La “sandboxing” consiste nel limitare i modi in cui gli agenti di AI possono influenzare direttamente il mondo, rendendo molto più semplice supervisionarli e gestirli (‡640, ‡1192, ‡1295). Ad esempio, limitare la capacità di un sistema di AI di pubblicare su internet o di modificare il file system di un computer può prevenire danni imprevisti da azioni impreviste (‡1296). Tuttavia, questi approcci non possono sempre essere utilizzati per applicazioni in cui un sistema di AI deve necessariamente agire direttamente nel mondo.

###@ Strumenti di monitoraggio dell’ecosistema: modello e provenienza dei dati

Gli strumenti di modellazione e di provenienza dei dati sono strumenti tecnici per studiare l'ecosistema dell'IA, al fine di migliorare la consapevolezza degli usi a valle e degli impatti dei sistemi di IA.

>white|orangered|left|14|15.5|bb Le tecniche di provenienza dei sistemi di AI aiutano a tracciare gli utilizzi e gli impatti dei sistemi

Gli sviluppatori e coloro che effettuano il deployment possono usare varie tecniche per studiare l’uso del modello e la sua diffusione ‘nell’ambiente reale’. Ad esempio, possono fornire ai modelli comportamenti univoci di identificazione (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) oppure applicare pattern univoci ai pesi dei singoli modelli open-weight (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Tuttavia, rendere queste tecniche più resistenti alle modifiche del modello è un problema aperto (‡1195, ‡1196*). I ricercatori stanno inoltre lavorando a metodi per ‘inferire l’eredità del modello’ (‡1197, ‡1198, ‡1305, ‡1306), che aiutano a rispondere a domande del tipo: ‘Il modello X era una versione fine-tuned o distillata del modello Y?’. Infine, alcuni sviluppatori stanno lavorando a protocolli e infrastrutture per agenti AI per facilitare l’identificazione e la verifica quando interagiscono con sistemi esterni (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figura 3.8: Le watermark incorporano perturbazioni impercettibili in immagini e audio
>white|black||9|11|br I watermark incorporano perturbazioni impercettibili in immagini e audio che consentono di identificare i contenuti generati tramite AI mediante strumenti di rilevamento. In questa figura, sia i watermark dell’immagine sia quelli dell’audio sono esagerati per migliorarne la visibilità. Fonte: immagine Chameleon da Unsplash (‡1313*). Altri elementi creati dagli autori del Report. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figura 3.9: Tassi di successo degli attacchi di prompt injection
>white|black||9|11|br Tassi di successo degli attacchi di prompt injection, come riportati dagli sviluppatori di AI per i principali modelli rilasciati tra maggio 2024 e agosto 2025. Ogni punto rappresenta la proporzione di attacchi riusciti su 10 tentativi contro un dato modello subito dopo il rilascio. Il tasso di successo riportato di tali attacchi è in calo nel tempo, ma resta relativamente alto. Fonte: Zou et al. 2025 (‡1149), citato in Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Le tecniche di rilevamento dei contenuti basati su AI aiutano a monitorare la diffusione e gli impatti dei contenuti generati dall'AI

I watermark, i metadati e altri rilevatori di contenuti AI possono aiutare i ricercatori a tracciare e studiare l’impatto nel mondo reale dei contenuti generati dall’AI. 

Innanzitutto, i watermarks dei dati sono motivi sottili ma distinti inseriti nei media digitali che possono codificare informazioni sulla loro origine (‡1199, ‡1200, ‡1201*). Per il testo, in genere assumono la forma di bias sottili nelle scelte delle parole e nello stile (‡1308, ‡1309); per immagini e video, di pattern sottili sui pixel (‡1310); e per l’audio, di pattern sottili nelle onde sonore (‡1311). La Figura 3.8 illustra questi aspetti.

Oltre alle filigrane, i contenuti generati dall’AI possono anche essere salvati utilizzando formati di file che memorizzano metadati su come sono stati generati. Ad esempio, molti dispositivi mobili salvano immagini e file audio usando un formato che può archiviare informazioni relative alle impostazioni della fotocamera, all’ora, alla posizione, ecc. (‡1312). Metadati simili possono essere usati per memorizzare informazioni su se i dati siano stati generati da un sistema AI. Proprio come il fingerprinting nella forensics criminale, le filigrane e i metadati possono essere manomessi o rimossi, ma nondimeno sono utili.

I ricercatori stanno inoltre lavorando allo sviluppo di rilevatori di contenuti generati da AI (‡1203, ‡1204, ‡1205*) per aiutare a identificare i contenuti generati da AI sul campo, anche quando non sono disponibili watermark o metadati. Tuttavia, queste tecniche di identificazione hanno un tasso di successo limitato.

###@ Aggiornamenti

Dalla pubblicazione dell’ultimo Report (January 2025), sono stati compiuti progressi nello sviluppo di sistemi di AI con più livelli efficaci di salvaguardie. Come discusso in §3.2. Risk management practices, defence-in-depth è un principio fondamentale nella gestione del rischio (‡1314). Ad esempio, i sistemi di AI che combinano modelli addestrati alla sicurezza con filtri di input, filtri di output e altri monitor dei contenuti sono oggetto di studio e vengono sempre più spesso implementati (‡32, ‡65, ‡1182*). Recenti ricerche hanno inoltre mostrato che, sebbene gli sviluppatori di modelli abbiano fatto progressi nell’aumentare la robustezza ai tentativi di aggirare le salvaguardie, gli attaccanti riescono ancora con un tasso elevato (Figura 3.9).

###@ lacune di evidenza

Serve ulteriore evidenza per aiutare i ricercatori a comprendere e tenere conto delle limitazioni degli approcci esistenti. I dispositivi di salvaguardia tecnici per i sistemi di IA vengono migliorati, ma le tecniche presentano limiti. Ad esempio, i progressi nel migliorare la robustezza nel caso peggiore dei sistemi di IA di uso generale sono stati lenti e vi sono limitazioni fondamentali su quanto estesamente i modelli con pesi aperti possano essere protetti e monitorati (‡1195, ‡1315, ‡1316) (vedi anche §3.4. Modelli con pesi aperti). Nel frattempo, non tutte le salvaguardie tecniche sono ugualmente comuni, ugualmente efficaci o ugualmente dimostrate nel mondo reale. Per esempio, l’addestramento avversariale è quasi universalmente usato sui modelli all’avanguardia (‡64*, ‡677), mentre tecniche di interpretabilità del modello e di verifica formale hanno visto un uso ridotto fino a oggi nei sistemi di produzione (‡1177, ‡1285).

###@ Sfide per i responsabili politici

Le principali sfide per i responsabili politici includono decidere se e in che modo dovrebbero sostenere la ricerca, lo sviluppo, la valutazione e l’adozione di salvaguardie tecniche e metodi di monitoraggio. Ciò è difficile perché la comprensione dei ricercatori di come salvaguardare al meglio, in pratica, i meccanismi è ancora in evoluzione e le migliori pratiche non sono ancora state stabilite. Ad esempio, diversi sviluppatori applicano salvaguardie diverse e, in modo più ampio, i loro approcci alla mitigazione del rischio tecnico variano ampiamente (‡1116). Infine, l’esistenza di salvaguardie tecniche efficaci non garantisce, di per sé, la sicurezza, poiché l’adozione e l’implementazione possono variare tra gli sviluppatori e i contesti di distribuzione.

