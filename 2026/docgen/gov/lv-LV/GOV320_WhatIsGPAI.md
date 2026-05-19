###@ Kas ir vispārējas nozīmes AI sistēmas?

Vispārējas nozīmes AI sistēmas ir programmatūras programmas, kas mācās modeļus no lieliem datu apjomiem, ļaujot tām veikt dažādus uzdevumus, nevis būt specializētām tikai vienai konkrētai funkcijai vai jomai (skat. 1. tabulu). Lai izveidotu šīs sistēmas, AI izstrādātāji veic daudzpakāpju procesu, kas prasa būtiskus skaitļošanas resursus, lielus datu kopumus un specializētas zināšanas (skat. 1. tabulu). Skaitļošanas resursi (bieži saīsināti uz “compute”) ir nepieciešami gan AI sistēmu izstrādei, gan izvietošanai, un tie ietver specializētas datora mikroshēmas, kā arī programmatūru un infrastruktūru, kas nepieciešama to darbībai.† Tā kā tās tiek apmācītas uz lielām, daudzveidīgām datu kopām, vispārējas nozīmes AI sistēmas var veikt daudz dažādu uzdevumu, piemēram, apkopot tekstu, ģenerēt attēlus vai rakstīt datorprogrammas kodu. Šajā sadaļā ir izskaidrots, kā tiek veidotas vispārējas nozīmes AI sistēmas, kas ir “iemiesošanas” modeļi, un kā politikas lēmumi ietekmē vispārējas nozīmes AI sistēmu izstrādi.

    Piezīme † -- Termins “compute” var attiekties arī uz vai nu mērījumu par aprēķinu skaitu, ko procesors var veikt (parasti mērīts peldošā komata operācijās sekundē), vai tieši uz aparatūru (piemēram, grafisko procesoru vienībām), kas veic šos aprēķinus.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Valodu sistēmas
- Apertus (‡1)
- Kloda Soneta 4.5 (‡2*)
- Komanda A (‡3*)
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
###@ Attēlu ģeneratori
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Video ģeneratori
- Kosmoss (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Redzu 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotiķa un navigācijas sistēmas
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Dažādu biomolekulāru struktūru klašu prognozētāji
- AlphaFold 3 (‡27)
- Pastiprināt (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI aģenti
- AlphaEvolve (‡31*)
- ChatGPT aģents (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI zinātnieks-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabula 1.1: Vispārējas nozīmes AI veidi
>white|black||9|11|br Ir vairāki dažādi vispārējas nozīmes AI veidi. Šajā Pārskatā modeļi, kas spēj prognozēt strukturālu informāciju dažādām molekulu klasēm, tiek uzskatīti par “vispārējas nozīmes” AI, jo tos var pielāgot dažādiem uzdevumiem. Piemēram, modeļi, kas apmācīti olbaltumvielu struktūras prognozēšanai, ir piemērojami dažādiem citiem uzdevumiem, piemēram, olbaltumvielu mijiedarbību prognozēšanai, mazu molekulu saistīšanās vietu prognozēšanai, kā arī ciklisku peptīdu (‡40) prognozēšanai un projektēšanai.


>white|orangered|left|13|15|bb Dziļā mācīšanās ir pamats vispārējas nozīmes mākslīgajam intelektam

Pētnieki izveido vispārējas nozīmes AI modeļus, izmantojot procesu, ko sauc par “dziļo mācīšanos” (deep learning), kas apmāca modeļus mācīties no piemēriem (‡41). Atšķirībā no programmatūras inženierijas dziļās mācīšanās modeļi uzdevumu izpildei mācās no datiem, nevis paļaujas uz ar roku rakstītām instrukcijām. Apstrādājot lielus datu apjomus, piemēram, attēlus, tekstu vai audio, šie modeļi atklāj veidus, kā attēlot šos datus, radot iekšējus modeļu attēlojumus par tādiem paraugiem kā formas, vārdu saistības vai skaņu struktūras, kas palīdz modelim atpazīt sakarības un ģenerēt izvades, kas atbilst tā apmācības mērķim. Pēc tam tie izmanto šos apgūtos iekšējos attēlojumus kā abstraktas iezīmes, lai analizētu jaunus, līdzīgus datus un ģenerētu izvades tādā pašā stilā. Piemēram, vispārējas nozīmes AI modelis, kas apmācīts ar pietiekami daudz piemēru 19. gadsimta romantiskās angļu poēzijas, var atpazīt jaunus šī stila dzejoļus un radīt jaunu materiālu līdzīgā stilā.

Padziļinātākā līmenī dziļā mācīšanās darbojas, apstrādājot datus ar slāņiem, kuros savstarpēji saistīti informācijas apstrādes mezgli. Šos mezglus bieži sauc par “neironiem”, jo tie ir tikai aptuveni iedvesmoti no neironiem bioloģiskās smadzenēs (“neironu tīkli”) (Figūra 1.1) (‡42). Tā kā informācija plūst no viena neironu slāņa uz nākamo, modelis pakāpeniski pārveido datus arvien abstraktākos attēlojumos kā apgūtu pazīmju kopumos – modeļa automātiski atklātos modeļos datos, nevis ar rokām kodētās pazīmēs. Piemēram, attēlu apstrādes modelī pirmie slāņi var iemācīties atklāt vienkāršas pazīmes, piemēram, malas vai pamatformas, kamēr dziļāki slāņi apvieno šīs pazīmes, lai izceltu sarežģītākus modeļus, piemēram, sejas vai objektus.

Funkcijas visos slāņos tiek atklātas optimizācijas procesā, kas nosaka apmācības procedūru. Apmācības laikā, kad modelis pieļauj kļūdas, dziļās mācīšanās algoritmi pielāgo dažādu savienojumu stiprumu starp neironiem, lai uzlabotu modeļa veiktspēju. Katras savienojuma stiprumu starp mezgliem bieži dēvē par “svaru”. Šī slāņotā pieeja ir tā, kas dziļajai mācīšanai piešķir tās nosaukumu.

Dziļā mācīšanās ir pierādījusi sevi kā ļoti efektīvu, ļaujot AI sistēmām paveikt uzdevumus, kas iepriekš tika uzskatīti par sarežģītiem tradicionālām, ar rokām programmētām skaitļošanas sistēmām, kā arī citiem agrākiem simboliskās vai uz noteikumiem balstītās AI paņēmieniem. Lielākā daļa mūsdienu vadošo, vispārējas nozīmes AI modeļu tagad balstās uz noteiktu neironu tīkla arhitektūru, kas pazīstama kā “transformators” (‡43, ‡44). Transformatori izmanto “uzmanības” (attention) mehānismu (‡45), kas palīdz modelim apstrādes laikā koncentrēties uz visatbilstošākajām ievades datu daļām, piemēram, nosakot, kuri vārdi teikumā ir visnozīmīgākie, lai izprastu tā nozīmi. Šāda modeļu veidošanas pieeja ir novedusi pie būtiskiem uzlabojumiem tulkošanā (‡43), dabiskās valodas apstrādē (‡46), attēlu atpazīšanā (‡47) un runas atpazīšanā (‡48, ‡49), un galu galā ir veicinājusi mūsdienu visprogresīvāko modeļu izstrādi.

![fig1.1](images/fig1.1_neural_network.png)

##### Figūra 1.1: Illustratīvs attēlojums “neironu tīkls”
>white|black||9|11|br Mūsdienu vispārējas nozīmes AI modeļi ir balstīti uz šiem tīkliem, kas ir tikai brīvi iedvesmoti no bioloģiskām smadzenēm. Dažādiem tīkliem ir atšķirīgi izmēri un arhitektūras. Tomēr visi ir veidoti no savstarpēji savienotiem informācijas apstrādes vienību ‘neironiem’, kur savienojumu stiprumus starp neironiem sauc par ‘svariem’ . Svari tiek atjaunināti apmācības laikā, izmantojot lielus datu apjomus. Avots: International AI Safety Report 2025 (‡50) (modified).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figūra 1.2: Shematiskā ģenerāluzdevuma AI attīstības posmu attēlojuma shēma
>white|black|left|9|11|br Starptautiskais AI drošības ziņojums 2026.


>white|orangered|left|13|15|bb Vispārējas nozīmes AI tiek izstrādāta posmos

Vispārējas nozīmes AI sistēmas izstrāde ietver vairākus posmus, sākot no sākotnējās modeļa apmācības līdz pēcapstrādes uzraudzībai un atjauninājumiem (Figūra 1.2). Praktiski šie soļi bieži pārklājas iteratīvā veidā. Katra posma īstenošanai ir vajadzīgi atšķirīgi resursu ieguldījumi (piem., dati, darbaspēks, skaitļošana) un atšķirīgas metodes, un tos dažkārt veic dažādi izstrādātāji (Figūra 1.2 un Tabula 1.2).

Piemēram, modeļa iepriekšēja apmācība parasti prasa lielus skaitļošanas resursu un datu apjomus, tādēļ šis posms ir īpaši jutīgs pret politiku, kas ietekmē piekļuvi skaitļošanas resursiem vai treniņu datiem (‡51, ‡52). Līdzīgi, datu sagatavošana un dažas modeļa pielāgošanas metodes pašlaik ietver lielus cilvēka darba apjomus sākotnējai datu iezīmēšanai (‡53). Tādēļ šis posms ir jutīgs pret izmaiņām darbaspēka izmaksās, platformu politikām vai noteikumiem, kas ietekmē pārrobežu līgumslēgšanas vienošanās.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Datu vākšana un sagatavošana
> 
  Pirms vispārēja mērķa AI modeļa apmācības izstrādātāji un datu darbinieki apkopo, attīra, sagatavo un standartizē neapstrādātos apmācības datus formātā, no kura modelis var mācīties. Tas var būt darbietilpīgs process. Apmācības datkopas aiz jaunākajiem, valsts līmeņa modeļiem ietver milzīgu skaitu piemēru no visas interneta.
  Komandas bieži izstrādā izsmalcinātas filtrēšanas metodes, lai samazinātu kaitīga satura izplatību, novērstu dublētu datu parādīšanos un uzlabotu pārstāvniecību dažādās tēmās un avotos (‡54, ‡55). Datu sagatavošana (kurēšana) var arī palīdzēt mazināt autortiesību un privātuma pārkāpumus, noņemt piemērus, kas satur bīstamas zināšanas, apstrādāt vairākas valodas un uzlabot dokumentāciju par datu izcelsmi (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Pirmapmācība (pirmais apmācības posms)

  Pirmapmācības laikā izstrādātāji modeļiem ievada milzīgus apjomus dažādu datu, lai ieaudzinātu plašu informācijas bāzi un konteksta izpratni. Šis process rada “bāzes modeli”. Šī ir ļoti datu- un skaitļošanas ietilpīga procedūra.

  Sākotnējās apmācības (pre-training) laikā modeļi tiek pakļauti miljardiem vai triljoniem satura piemēru, piemēram, attēliem, tekstiem vai audio. Ar šādu pakļaušanu modelis pakāpeniski atklāj abstraktas iezīmes datu attēlošanai un iemācās, kā šīs iezīmes ir savstarpēji saistītas, kas ļauj tam kontekstā saprast jaunus ievades datus. Šis sākotnējās apmācības process ilgst nedēļas vai mēnešus (‡59) un izmanto desmitiem vai simtiem tūkstošu grafikas procesoru vienību (GPU) vai tenzoru apstrādes vienību (TPU) (‡60) – specializētas datora mikroshēmas, kas izstrādātas, lai ļoti ātri veiktu daudz šādu aprēķinu. Daži izstrādātāji veic sākotnējo apmācību ar savu skaitļošanas jaudu, bet citi izmanto resursus, ko nodrošina specializēti skaitļošanas pakalpojumu sniedzēji.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Pēc-apmācība un smalkā pielāgošana (apmācības otrais posms)

  ‘Pēcapmācība’ vēl vairāk pilnveido bāzes modeli, lai to optimizētu konkrētam pielietojumam. Tā ir mēreni resursietilpīga un ļoti darbietilpīga procesa. Pāreja uz ‘sinētiskiem datiem’ – mākslīgi ģenerētu informāciju, kas atdarina reālas vides datus, bet tiek veidota ar algoritmiem vai simulācijām – palīdz šo posmu padarīt mazāk darbietilpīgu.
  Pēcapmācība ietver dažādas smalkas pielāgošanas metodes un citas modifikācijas. “Uzraudzīta smalkā pielāgošana” ietver apmācīta modeļa turpmāku apmācību uz konkrētiem datu kopumiem, lai uzlabotu modeļa sniegumu attiecīgajā jomā (‡61, ‡62). Piemēram, vispārīga nolūka modelis var tikt papildus apmācīts uz liela radioloģisko attēlu kopuma. “Pastiprinātā mācīšanās” (RL) ietver modeļa snieguma uzlabošanu, “atlīdzinot” modelim (nodrošinot pozitīvu atgriezenisko saiti) par vēlamām izvades iespējām un “sodot” modeli (nodrošinot negatīvu atgriezenisko saiti) par nevēlamām izvades iespējām. Tai ir divas izteiktas apakškategorijas. “Pastiprinātā mācīšanās no cilvēka atgriezeniskās saites” ietver tādu izvades rezultātu atalgošanu, kas atbilst cilvēku vēlmēm, un tādu rezultātu sodīšanu, kas neatbilst, balstoties uz cilvēka atgriezenisko saiti (‡63, ‡64*). “Pastiprinātā mācīšanās ar pārbaudāmiem atalgojumiem” (RLVR) tiek izmantota modeļa snieguma uzlabošanai uzdevumos, kas prasa faktoloģisku pareizību, piemēram, matemātikas vai koda ģenerēšanā. Izstrādātāji parasti mijas starp pēcapmācības paņēmienu piemērošanu un testu veikšanu, līdz rezultāti parāda, ka modelis atbilst vēlamajām specifikācijām.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Sistēmas integrācija

  Izstrādātāji apvieno vienu vai vairākus vispārējas nozīmes AI modeļus ar citiem komponentiem, lai izveidotu “AI sistēmu”, kas ir gatava lietošanai. GPT-5 (piemēram) ir vispārējas nozīmes AI modelis, kas apstrādā tekstu, attēlus un audio, savukārt ChatGPT ir vispārējas nozīmes AI sistēma, kas apvieno vairākus dažāda lieluma un iespēju modeļus ar tērzēšanas saskarni, satura apstrādi, Web piekļuvi un lietojumprogrammu integrāciju, lai izveidotu funkcionālu produktu.
  Papildus tam, lai padarītu AI modeļus operacionālus, papildu komponenti AI sistēmā arī tiecas uzlabot spējas, lietderību un drošību. Piemēram, sistēma var būt aprīkota ar filtru, kas nosaka un bloķē modeļa ievades vai izvades, kurās ir kaitīgs saturs (‡65*). Izstrādātāji arvien biežāk izmanto arī ‘scaffolding’ – papildu programmatūru, kas tiek veidota ap vispārējas nozīmes AI modeļiem un ļauj tiem iepriekš plānot, tiekties pēc mērķiem un mijiedarboties ar pasauli (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Izvietošana un izlaidšana
  Darbība (Deployment) ir process, kurā integrēto AI sistēmu padara pieejamu paredzētajam lietojumam. Izstrādātāji un izvietošanas veicēji (deployers) ievieš AI sistēmas reālās pasaules lietojumprogrammās, produktos vai pakalpojumos. Izstrādātāji var izvietot AI sistēmas iekšēji (savām vajadzībām) vai ārēji (privātiem klientiem vai publiskai lietošanai). Izvietojot AI sistēmas ārēji, uzņēmumi bieži nodrošina lietotājiem piekļuvi, izmantojot tiešsaistes lietotāja saskarnes vai lietojumprogrammu saskarnes (API), kas ļauj lietotājiem piekļūt sistēmai un to palaist. Piemēram, viens uzņēmums var izstrādāt pēc pasūtījuma veidotu klientu apkalpošanas tērzēšanas robotu, ko darbina cita uzņēmuma vispārēja mērķa AI sistēma.
  “AI sistēmas izvietošana” attiecas uz modeļa nodrošināšanu reālai izmantošanai ar integrētiem rīkiem un saskarnēm, savukārt “modeļa izlaišana” ietver pamatmodeļa padarīšanu pieejamu citiem – vai nu kā atvērta svara (lejupielādējami parametri), vai slēgta svara (tikai API piekļuve). Sk. §3.4. Atvērtā svara modeļi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Pēcizvietošanas uzraudzība un atjauninājumi

  Izstrādātāji bieži apkopo un analizē lietotāju atsauksmes, izseko ietekmes un veiktspējas rādītājus un veic iteratīvus uzlabojumus, lai risinātu problēmas, kas atklājas reālas izmantošanas laikā (‡67). Uzlabojumi tiek veikti, atjauninot sistēmas integrācijas, bieži vien izmantojot nepārtrauktu smalkāku pielāgošanu (continual fine-tuning) un nodrošinot modeļiem piekļuvi ārējām datubāzēm ar (jaunākajiem) faktiem. Tas ļauj lielajiem AI modeļiem būt atjauninātiem, neatkārtojot pilno pirmapmācības procesu (‡68*). Tas ļauj iespējām uzkrāties nākamajās apmācības kārtās, vienlaikus saglabājot stabilitāti un samazinot aprēķinu izmaksas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### 1.2. tabula: Vispārējas nozīmes AI izstrādes posmi
>white|black||9|11|br Katrā vispārējas nozīmes AI izstrādes posmā AI modelis tiek pilnveidots turpmākai izmantošanai un galu galā izvietots kā pilnībā integrēta AI sistēma, kur to uzrauga un atjauno.


>white|orangered|left|13|15|bb Spriešanas sistēmas ģenerē “domu ķēdes” secināšanas laikā, lai uzlabotu veiktspēju

Inferēšana notiek tad, kad kāds izmanto AI modeli pēc tam, kad tas ir apmācīts. Piemēram, inferēšana notiek brīdī, kad persona lūdz AI sistēmu izplānot ceļojumu, un tā pamatā esošais modelis izmanto atbilstošus aspektus no tā, ko tas ir iemācījies par ģeogrāfiju, transportu un virtuvi, lai ģenerētu maršrutu.

Pēdējās desmitgadēs sasniegumi AI spējās lielā mērā ir nākuši no lielākiem apmācības cikliem; tas ir, palielinot skaitļošanas jaudu, kas tiek izmantota, lai apmācītu AI modeli. Tomēr nesen pētnieki ir panākuši vairāk ieguvumu, ļaujot modeļiem apstrādāt informāciju ilgāk, un apmācot tos ģenerēt skaidrus pamatojuma soļus, kad tie izpilda uzdevumu (‡69*, ‡70). Šādus AI sistēmas sauc par “pamatojuma sistēmām”, un starpposma skaidrojumi, kurus tās iziet problēmas risināšanas vai jautājuma atbildēšanas gaitā, tiek saukti par “domāšanas ķēdēm”. Pamatojuma sistēmas lietošanas brīdī prasa vairāk skaitļošanas resursu, lai ģenerētu šīs izsmalcinātās domāšanas ķēdes (‡71, ‡72, ‡73, ‡74), kā arī vairāk resursu apmācības laikā, lai tās iemācītos domāt labāk. Praktiski šīs pamatojuma spējas ļauj AI sistēmām atrisināt sarežģītākas problēmas, iteratīvi sadalot uzdevumu mazākos soļos. Tabula 1.3 parāda piemēru, kā ne-pamatojuma sistēma un pamatojuma sistēma risina vienu un to pašu problēmu.

Pamatojuma sistēmas ir sasniegušas ievērojamus izrāvienus spējās sarežģītu uzdevumu risināšanā. Piemēram, 2025. gadā pamatojuma sistēmas, kas specializējas matemātisku problēmu risināšanā, piemēram, Google’s Gemini Deep Think, un nepubliskots, eksperimentāls OpenAI modelis, atrisināja Starptautiskās matemātikas olimpiādes uzdevumus (strukturētā testa vidē) līmenī, kas atbilst cilvēka zelta medaļas sniegumam (‡75, ‡76). Pamatojuma sistēmas ir parādījušas būtisku progresu formālās jomās, piemēram, matemātikā, loģikas mīklās un strukturētos zinātniskos jautājumos, kur soli pa solim pamatojumu var skaidri pārbaudīt (‡77). Tomēr pamatojuma sistēmas var arī neizdoties, radot nesaistītas, neproduktīvas vai atkārtotas domu ķēdes (‡78, ‡79).

###@ Atjauninājumi apmācības metodēs

Kopš pēdējā Ziņojuma publicēšanas (January 2025), apmācības metode, ko sauc par ‘distillation’, ir ievērojami palielinājusi efektivitāti, ar kādu dažus modeļus var pielāgot (fine-tuned). Distillation ietver ‘student’ modeļa apmācīšanu uz izvadiem no jaudīgāka (un parasti lielāka) ‘teacher’ modeļa, ļaujot student modelim tieši atdarināt teacher modeļa izvades (‡80). Piemēram, DeepSeek izstrādāja lielu modeli, ko sauc par DeepSeek-R1, un tas izceļas ar chain-of-thought reasoning. R1 ģenerēja reasoning izvades, kuras pēc tam tika izmantotas, lai pielāgotu mazākus student modeļus, tostarp DeepSeek-V3. DeepSeek-V3 saglabā lielu daļu R1 matemātiskās, kodēšanas un dokumentu analīzes spēju, un, kā ziņots, tas tika pielāgots (fine-tuned) aptuveni par $10,000 USD (lai gan tā iepriekšējās apmācības izmaksas netika norādītas) (‡81). Tas, visticamāk, ir par vairākiem lieluma pakāpieniem mazāk nekā izmaksas, kas būtu nepieciešamas, lai pielāgotu līdzīgi spējīgus, lielākus modeļus.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabula 1.3: Neapsveršanas sistēmas piemērs (pa kreisi) salīdzinājumā ar spriešanas sistēmu (pa labi)
>white|black||9|11|br Risinot to pašu mīklu, šie piemēri ir pielāgoti no reālām AI atbildēm. Iemeslošanas sistēma pavada vairāk laika un skaitļošanas jaudas uz “domāšanu”, veidojot “domu ķēdi” pirms savas galīgās atbildes sniegšanas.

![figure.3](images/fig1.3_AI_agent.png)

##### Figūra 1.3: Iliustratīvs AI aģenta attēlojums
>white|black||9|11|br AI modelis (centrā), kas ir konfigurēts iteratīvi plānot, veikt spriešanu un izmantot rīkus, lai paveiktu reālas pasaules uzdevumus. Avots: International AI Safety Report 2026.


Tādējādi destilācija var būt lēts un efektīvs veids, kā modeļi iegūst jaudīgākas spējas (‡82). Daži pētnieki ir izmantojuši destilāciju, lai pielāgotu (fine-tune) augsti spējīgus modeļus, izmantojot pat tikai 1,000 piemērus, kas ģenerēti no jaunākā līmeņa (state-of-the-art) modeļiem (‡83). Tā kā destilācijai ir nepieciešams jau eksistējošs “skolotāja” modelis, to nevar tieši izmantot, lai attīstītu jaunākā līmeņa modeļu spējas. Tomēr tā var paātrināt uzlabotu AI spēju izplatīšanos pat no slēgtā pirmkoda (closed-source) modeļiem (‡84*).

Kopā ar tehnoloģiskajiem sasniegumiem jomā “izplatītā skaitļošana” un decentralizētā apmācība (pieejas, kurās izstrādātāji izmanto vairākus procesorus, serverus vai datu centrus, kas darbojas kopā, lai veiktu AI apmācību vai inferenci (‡85, ‡86, ‡87)), ir samazināta pakāpe, kādā daudzi AI izstrādes projekti ir atkarīgi no liela mēroga, centralizētas skaitļošanas infrastruktūras. Tas arvien biežāk ļauj mazāk resursiem nodrošinātiem dalībniekiem izstrādāt un izvietot jaudīgas sistēmas.

###@ Atjauninājumi par AI aģentiem

Kopš pēdējā Pārskata (January 2025), attīstība tajā, kā izstrādātāji apvieno AI modeļus ar rīkiem, ir ļāvusi izstrādāt arvien spēcīgākus AI aģentus. AI aģenti ir izstrādāti, lai sasniegtu mērķus, kurus bieži lietotāji norāda dabiskajā valodā. Lai sasniegtu šos mērķus, tiem tiek dota piekļuve rīkiem, piemēram, atmiņai, datora saskarnei un tīmekļa pārlūkprogrammām. Šie rīki un kods, kas tiek izmantots to apvienošanai ar modeli, tiek dēvēti par “scaffolding”, un tie palīdz AI aģentiem autonomi mijiedarboties ar pasauli, veidot plānus, atcerēties svarīgas detaļas un tiekties pēc mērķiem (‡88*, ‡89) ar ievērojami mazāku cilvēku uzraudzību vai palīdzību. Piemēram, Manus AI ir populārs AI aģents, kas var automatizēt dažādus uzdevumus, tostarp tīmekļa meklēšanu, programmatūras izstrādi un pirkumus tiešsaistē (‡90). Figūra 1.3 parāda vienkāršu piemēru AI aģentam, ko veido vispārējas nozīmes AI modelis “brain”, kurš var iteratīvi plānot, spriest un izmantot rīkus atmiņai, tīmekļa pārlūkošanai un datora lietošanai.

Digitālā infrastruktūra AI aģentiem paplašinās (‡91), un tie kļūst arvien izplatītāki dažādās nozarēs (‡92, ‡93, ‡94). AI aģenti ir izstrādāti tādiem uzdevumiem kā pētniecība (‡37), programmatūras izstrāde (‡95), robotu vadība (‡96) un klientu apkalpošana (‡97). Nepārtraukti pētniecības un izstrādes darbi ir noveduši pie pastāvīgi spējīgākiem un arvien autonomākiem AI aģentiem vai daudz­aģentu sistēmām. Pētnieki ir lēsuši, ka programmatūras etalona uzdevumu (benchmark tasks) sarežģītība, ko AI aģenti spēj izpildīt, aptuveni ik pēc septiņiem mēnešiem dubultojas (sk. arī §1.2. Pašreizējās iespējas) (‡98). Eksperti apgalvo, ka arvien spējīgāki AI aģenti radīs gan nozīmīgas iespējas, gan riskus (‡99, ‡100*) (sk. §2.2.1. Uzticamības izaicinājumi).

###@ Pierādījumu trūkumi

Galvenās pierādījumu nepilnības ap vispārēja nolūka AI sistēmu izstrādes procesu izriet no publiski pieejamas informācijas trūkuma par to, kā tās tiek izstrādātas. Daži izstrādātāji ir ļoti atklāti par to, kā viņi izstrādā vispārēja nolūka AI sistēmas (‡1, ‡101). Tomēr kopumā publiski pieejamās un politikas veidotāju zināšanas par to, kā lielākā daļa progresīvo modeļu tiek izstrādāti, nodrošināti, izvērtēti un izvietoti, ir ierobežotā apjomā. Tas jo īpaši attiecas uz iekšēji izvietotām AI sistēmām, kuras tiek izmantotas AI uzņēmumos, bet kuras netiek izmantotas vai izprastas ārējiem ieinteresētajiem dalībniekiem (‡102, ‡103). Šī ierobežotā ārējā redzamība rada grūtības attiecībā uz pārskatāmību un uzraudzību. Daudzi pētnieki ir norādījuši uz ierobežotu un nevienmērīgu pārskatāmību saistībā ar apmācības datiem (‡104, ‡105, ‡106), vispārēja nolūka AI modeļiem (‡107, ‡108), AI aģentiem (‡92), izvērtējumiem (‡109), izstrādes procesiem (‡110) un drošību (‡111). Ierobežojumi attiecībā uz ārēju izpaušanu dažkārt ir nepieciešami, lai pasargātu uzņēmumu komercnoslēpumus un intelektuālo īpašumu. Tajā pašā laikā zema pārskatāmība apgrūtina neatkarīgu pētnieku un politikas veidotāju iespējas pētīt vispārēja nolūka AI modeļus un sistēmas.


