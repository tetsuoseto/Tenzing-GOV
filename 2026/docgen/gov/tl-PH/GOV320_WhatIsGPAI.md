###@ Ano ang mga AI system na pangkalahatang gamit?

Ang mga AI system para sa pangkalahatang layunin ay mga programang software na natututo ng mga padron mula sa maraming datos, kaya nagagawa nila ang iba’t ibang gawain sa halip na maging espesyalisado para sa isang partikular na tungkulin o larangan (tingnan ang Talahanayan 1.1). Para mabuo ang mga system na ito, nagsasagawa ang mga developer ng AI ng prosesong may maraming yugto na nangangailangan ng malalaking computational resource, malalawak na dataset, at espesyalisadong kadalubhasaan (tingnan ang Talahanayan 1.2). Kailangan ang mga computational resource (madalas na pinaikli bilang ‘compute’) kapwa sa pagbuo at sa pag-deploy ng mga AI system, at kabilang dito ang mga espesyalisadong computer chip pati na ang software at imprastrakturang kailangan para patakbuhin ang mga ito.† Dahil sinasanay ang mga ito gamit ang malalaki at sari-saring dataset, nagagawa ng mga AI system para sa pangkalahatang layunin ang maraming iba’t ibang gawain, tulad ng pagbubuod ng teksto, paglikha ng mga larawan, o pagsulat ng computer code. Ipinapaliwanag ng seksiyong ito kung paano binubuo ang mga AI system para sa pangkalahatang layunin, kung ano ang mga modelong ‘nangangatwiran’, at kung paano hinuhubog ng mga desisyon sa patakaran ang pagbuo ng mga AI system para sa pangkalahatang layunin.

    Tandaan † -- Ang terminong ‘compute’ ay maaari ring tumukoy sa sukatan ng bilang ng mga kalkulasyong kayang gawin ng isang processor (karaniwang sinusukat sa mga floating-point operation kada segundo) o partikular sa hardware (gaya ng mga graphics processing unit) na nagsasagawa ng mga kalkulasyong iyon.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Mga sistema ng wika
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Utos A (‡3*)
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
###@ Mga generator ng larawan
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Mga generator ng video
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotics at mga sistema ng nabigasyon
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Mga prediktor para sa iba't ibang uri ng mga biomolekular na istruktura
- AlphaFold 3 (‡27)
- Palakasin (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Mga ahente ng AI
- AlphaEvolve (‡31*)
- Ahente ng ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Ang AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Talahanayan 1.1: Mga Uri ng AI na Pangkalahatang Layunin
>white|black||9|11|br May ilang magkakaibang uri ng AI na pangkalahatang layunin. Sa Ulat na ito, itinuturing na AI na ‘pangkalahatang layunin’ ang mga modelong nakapaghuhula ng impormasyong estruktural para sa iba’t ibang klase ng molekula dahil maaari silang iangkop sa iba’t ibang gawain. Halimbawa, magagamit ang mga modelong sinanay upang hulaan ang estruktura ng protina sa iba’t ibang gawain, gaya ng paghula sa mga interaksiyon ng protina, mga lugar na pinagbibigkisan ng maliliit na molekula, at paghula at pagdidisenyo ng mga paikot na peptide (‡40).


>white|orangered|left|13|15|bb  Malalim na pagkatuto ang pundasyon ng AI para sa pangkalahatang layunin.

Bumubuo ang mga mananaliksik ng mga modelong AI na pangkalahatang layunin sa pamamagitan ng prosesong tinatawag na ‘malalim na pagkatuto’, na nagsasanay sa mga modelo na matuto mula sa mga halimbawa (‡41). Hindi tulad ng inhinyeriya ng software, natututo ang mga modelo ng malalim na pagkatuto na magsagawa ng mga gawain mula sa datos sa halip na umasa sa mga tagubiling isinulat ng tao. Sa pamamagitan ng pagproseso ng maraming datos, gaya ng mga larawan, teksto, o audio, natutuklasan ng mga modelong ito kung paano ilarawan ang datos na iyon, at lumilikha ng mga panloob na representasyon ng mga padron (gaya ng mga hugis, ugnayan ng mga salita, o estruktura ng tunog) na tumutulong sa modelo na makilala ang mga ugnayan at makabuo ng mga output na naaayon sa layunin ng pagsasanay nito. Pagkatapos, ginagamit nila ang mga natutuhang panloob na representasyong ito bilang mga abstraktong katangian upang suriin ang bago at katulad na datos at makabuo ng mga output sa parehong estilo. Halimbawa, kayang makilala ng isang modelong AI na pangkalahatang layunin na sinanay gamit ang sapat na mga halimbawa ng romantikong tulang Ingles noong ika-19 na siglo ang mga bagong tulang nasa estilong iyon at makabuo ng bagong materyal sa katulad na estilo.

Sa mas detalyadong antas, gumagana ang malalim na pagkatuto sa pamamagitan ng pagproseso ng datos sa mga suson ng magkakaugnay na node sa pagproseso ng impormasyon. Madalas tawaging ‘mga neuron’ ang mga node na ito dahil maluwag silang hango sa mga neuron sa biyolohikal na utak (‘mga neural network’) (Figure 1.1) (‡42).Habang dumadaloy ang impormasyon mula sa isang suson ng mga neuron patungo sa kasunod nito, unti-unting binabago ng modelo ang datos tungo sa mas abstraktong mga representasyongbilang mga pangkat ng natutuhang tampok – mga padron na awtomatikong natuklasan ng modelo sa datos, sa halip na mga padron na manu-manong isinulat sa code. Halimbawa, sa isang modelo sa pagproseso ng larawan, maaaring matutuhan ng mga unang suson na makakita ng mga payak na tampok gaya ng mga gilid o payak na hugis, samantalang pinagsasama ng mas malalalim na suson ang mga tampok na ito upang matukoy ang mas masalimuot na mga padron gaya ng mga mukha o bagay.

Natutuklasan ang mga feature sa lahat ng layer sa pamamagitan ng proseso ng optimisasyon na bumubuo sa pamamaraan ng pagsasanay. Habang nagsasanay, kapag nagkakamali ang modelo, inaayos ng mga algorithm ng malalim na pagkatuto ang lakas ng iba’t ibang koneksyon sa pagitan ng mga neuron upang mapahusay ang pagganap ng modelo. Madalas tawaging ‘timbang’ ang lakas ng bawat koneksyon sa pagitan ng mga node. Ang pamamaraang ito na gumagamit ng mga layer ang pinagmulan ng tawag na malalim na pagkatuto.

Napatunayang napakabisa ng malalim na pagkatuto sa pagtulong sa mga sistemang AI na magsagawa ng mga gawaing dating itinuturing na mahirap para sa mga tradisyonal na sistemang komputasyonal na mano-manong ipinrograma at sa iba pang naunang simboliko o nakabatay sa tuntuning mga pamamaraan ng AI. Karamihan sa mga pinakamodernong modelong AI para sa pangkalahatang layunin ay nakabatay na ngayon sa isang partikular na arkitektura ng neural network na kilala bilang ‘transformer’ (‡43, ‡44). Gumagamit ang mga transformer ng mekanismong ‘atensyon’ (‡45) na tumutulong sa modelo na ituon ang pansin sa mga bahaging pinakamahalaga sa input data habang pinoproseso ang impormasyon, gaya ng pagtukoy kung aling mga salita sa isang pangungusap ang pinakamahalaga upang maunawaan ang kahulugan nito. Nagbunga ang partikular na paraang ito ng pagbuo ng mga modelo ng malalaking pagpapahusay sa pagsasalin (‡43), pagproseso ng natural na wika (‡46), pagkilala ng larawan (‡47) at pagkilala ng pananalita (‡48, ‡49), na humantong sa pagbuo ng mga pinakamodernong modelo sa kasalukuyan.

![fig1.1](images/fig1.1_neural_network.png)

##### Figure 1.1: Isang ilustratibong representasyon ng isang ‘neural network’
>white|black||9|11|br Ang mga pangkalahatang AI model ngayon ay nakabatay sa mga network na ito, na bahagyang hango sa mga biyolohikal na utak. Magkakaiba ang laki at arkitektura ng mga network. Gayunman, lahat ng ito ay binubuo ng magkakaugnay na yunit sa pagproseso ng impormasyon na tinatawag na ‘mga neuron’, at ang lakas ng mga ugnayan sa pagitan ng mga neuron ay tinatawag na ‘mga timbang’. Ina-update ang mga timbang sa pamamagitan ng pagsasanay gamit ang maraming datos. Pinagmulan: International AI Safety Report 2025 (‡50) (binago).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figure 1.2: Isang eskematikong representasyon ng mga yugto ng pagbuo ng AI para sa pangkalahatang layunin
>white|black|left|9|11|br Pinagmulan: Pandaigdigang Ulat sa Kaligtasan ng AI 2026.


>white|orangered|left|13|15|bb  Ang AI para sa pangkalahatang layunin ay binubuo sa mga yugto

Kabilang sa pagbuo ng isang sistemang AI na pangkalahatang layunin ang maraming yugto, mula sa paunang pagsasanay ng modelo hanggang sa pagsubaybay at mga update pagkatapos itong ilunsad (Figure 1.2). Sa praktika, madalas na nagsasapawan ang mga hakbang na ito sa paulit-ulit na proseso. Nangangailangan ang bawat yugto ng magkakaibang input ng mga mapagkukunan (hal. datos, paggawa, kapasidad sa pag-compute) at magkakaibang pamamaraan, at kung minsan ay magkakaibang developer ang nagsasagawa sa mga ito (Figure 1.2 at Talahanayan 1.2).

Halimbawa, karaniwang nangangailangan ang paunang pagsasanay ng modelo ng malaking dami ng kakayahan sa pagkukuwenta at datos, kaya partikular na sensitibo ang yugtong ito sa mga patakarang nakaaapekto sa pag-access sa mga mapagkukunan sa pagkukuwenta o datos ng pagsasanay (‡51, ‡52). Gayundin, kasalukuyang nangangailangan ang pag-aayos ng datos at ilang paraan ng pag-fine-tune ng modelo ng malaking dami ng paggawa ng tao para sa paunang paglalagay ng mga etiketa sa datos (‡53). Samakatuwid, sensitibo ang yugtong ito sa mga pagbabago sa mga gastos sa paggawa, mga patakaran ng plataporma, o mga regulasyong nakaaapekto sa mga kaayusan sa pagkontrata sa pagitan ng mga bansa.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Pangangalap at pagsasaayos ng datos
> 
  Bago sanayin ang isang modelong AI na para sa pangkalahatang gamit, nangangalap, naglilinis, pumipili at nag-aayos ang mga developer at manggagawa sa datos ng hilaw na datos sa pagsasanay upang maging format na matututuhan ng modelo. Maaaring matrabaho ang prosesong ito. Binubuo ang mga dataset sa pagsasanay sa likod ng mga makabagong modelo ng napakaraming halimbawa mula sa buong internet.
  Madalas na bumubuo ang mga team ng mga sopistikadong paraan ng pagsasala upang mabawasan ang mapaminsalang nilalaman, maalis ang dobleng datos, at mapahusay ang representasyon sa iba’t ibang paksa at pinagmulan (‡54, ‡55). Makakatulong din ang pag-curate ng datos upang mabawasan ang mga paglabag sa copyright at privacy, maalis ang mga halimbawang naglalaman ng mapanganib na kaalaman, mapangasiwaan ang maraming wika, at mapahusay ang dokumentasyon tungkol sa pinagmulan ng datos (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Paunang pagsasanay (unang yugto ng pagsasanay)

  Sa panahon ng paunang pagsasanay, pinapakain ng mga developer ang mga modelo ng napakaraming magkakaibang datos upang magkaroon ang mga ito ng malawak na pundasyon ng impormasyon at pag-unawa sa konteksto. Ang prosesong ito ay lumilikha ng isang ‘batayang modelo’. Nangangailangan ang prosesong ito ng napakaraming datos at lakas-pagkompyut.

  Sa panahon ng paunang pagsasanay, inilalantad ang mga modelo sa bilyun-bilyon o trilyun-trilyong halimbawa ng nilalaman gaya ng mga larawan, teksto, o audio. Sa pamamagitan ng pagkakalantad na ito, unti-unting nakakahanap ang modelo ng mga abstraktong katangian na ginagamit sa representasyon ng datos at natututuhan nito kung paano nagkakaugnay ang mga katangiang ito, kaya nauunawaan nito ang mga bagong input batay sa konteksto. Tumatagal nang ilang linggo o buwan ang prosesong ito ng paunang pagsasanay (‡59) at gumagamit ito ng sampu-sampu o daan-daang libong graphics processing unit (GPU) o tensor processing unit (TPU) (‡60) – mga espesyal na chip ng computer na idinisenyo upang mabilis na magsagawa ng maraming ganitong kalkulasyon. Isinasagawa ng ilang developer ang paunang pagsasanay gamit ang sarili nilang kapasidad sa pag-compute, samantalang ang iba ay gumagamit ng mga mapagkukunang ibinibigay ng mga espesyalisadong provider ng kapasidad sa pag-compute.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Pagsasanay pagkatapos ng paunang pagsasanay at pagpino (ikalawang yugto ng pagsasanay)

  Mas pinipino pa ng ‘post-training’ ang batayang modelo upang i-optimize ito para sa isang partikular na aplikasyon. Katamtaman ang tindi ng kinakailangang pag-compute para rito, ngunit nangangailangan ito ng maraming paggawa. Nakakatulong ang paglipat sa paggamit ng ‘sintetikong datos’—impormasyong artipisyal na binuo at ginagaya ang datos mula sa totoong mundo, ngunit nilikha gamit ang mga algorithm o simulation—upang mabawasan ang dami ng paggawa sa yugtong ito.
  Kabilang sa pagsasanay pagkatapos ng paunang pagsasanay ang iba’t ibang teknik ng fine-tuning at iba pang pagbabago. Kasama sa ‘supervised fine-tuning’ ang karagdagang pagsasanay sa isang sinanay na modelo gamit ang mga partikular na dataset upang mapahusay ang pagganap ng modelo sa domain na iyon (‡61, ‡62). Halimbawa, maaaring sanayin pa ang isang modelong para sa pangkalahatang gamit gamit ang isang malaking koleksiyon ng mga radiological na larawan. Kasama sa ‘reinforcement learning’ (RL) ang pagpapahusay sa pagganap ng modelo sa pamamagitan ng ‘pagbibigay-gantimpala’ sa modelo (pagbibigay ng positibong feedback) para sa mga kanais-nais na output at ‘pagpaparusa’ sa modelo (pagbibigay ng negatibong feedback) para sa mga hindi kanais-nais na output. Mayroon itong dalawang kilalang subcategory. Kasama sa ‘reinforcement learning from human feedback’ ang pagbibigay-gantimpala sa mga output na umaayon sa mga kagustuhan ng tao at pagpaparusa sa mga hindi umaayon, batay sa feedback ng tao (‡63, ‡64*). Ginagamit ang ‘reinforcement learning with verifiable rewards’ (RLVR) upang mapahusay ang pagganap ng modelo sa mga gawaing nangangailangan ng katumpakan ng mga katotohanan, gaya ng matematika o pagbuo ng code. Karaniwang nagpapalitan ang mga developer sa paglalapat ng mga teknik ng pagsasanay pagkatapos ng paunang pagsasanay at pagpapatakbo ng mga pagsusuri hanggang sa ipakita ng mga resulta na natutugunan ng modelo ang mga hinihinging espesipikasyon.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integrasyon ng sistema

  Pinagsasama ng mga developer ang isa o higit pang mga modelong AI para sa pangkalahatang gamit at iba pang bahagi upang lumikha ng isang ‘AI system’ na handa nang gamitin. Ang GPT-5 (halimbawa) ay isang modelong AI para sa pangkalahatang gamit na nagpoproseso ng teksto, mga larawan at audio, samantalang ang ChatGPT ay isang sistemang AI para sa pangkalahatang gamit na pinagsasama ang ilang modelo na magkakaiba ang laki at kakayahan, kasama ang isang interface ng chat, pagproseso ng nilalaman, access sa Web at integrasyon ng mga application, upang makalikha ng isang produktong gumagana.
  Bukod sa pagpapagana sa mga modelo ng AI, layunin din ng mga karagdagang bahagi ng isang sistema ng AI na pahusayin ang kakayahan, pakinabang, at kaligtasan nito. Halimbawa, maaaring may kasamang filter ang isang sistema na tumutukoy at humaharang sa mga input o output ng modelo na naglalaman ng mapaminsalang content (‡65*). Lalo ring ginagamit ng mga developer ang “scaffolding” – karagdagang software na binubuo sa paligid ng mga modelo ng AI para sa pangkalahatang layunin, na nagbibigay-daan sa mga ito na magplano nang maaga, magsikap na makamit ang mga layunin, at makipag-ugnayan sa mundo (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Pag-de-deploy at paglalabas
  Ang deployment ay proseso ng pagpapagamit sa pinagsamang AI system para sa nilalayong paggamit nito. Ipinatutupad ng mga developer at nagde-deploy ang mga AI system sa mga aplikasyon, produkto, o serbisyong ginagamit sa totoong mundo. Maaaring i-deploy ng mga developer ang mga AI system sa loob ng organisasyon (para sa sarili nilang paggamit) o sa labas nito (para sa mga pribadong customer o pampublikong paggamit). Kapag nagde-deploy ng mga AI system sa labas ng organisasyon, madalas na nagbibigay ang mga kumpanya sa mga user ng access sa pamamagitan ng mga online na user interface o mga application programming interface (API) na nagbibigay-daan sa mga user na i-access at patakbuhin ang system. Halimbawa, maaaring magdisenyo ang isang kumpanya ng pasadyang chatbot para sa serbisyo sa customer na pinapagana ng pangkalahatang layuning AI system ng ibang kumpanya.
  Ang ‘deployment ng AI system’ ay tumutukoy sa pagpapagamit ng isang modelo sa mga totoong sitwasyon, kasama ang mga pinagsamang tool at interface, samantalang ang ‘paglalabas ng modelo’ ay nangangahulugan ng pagbibigay-daan sa iba na ma-access ang batayang modelo – bilang open-weight (mga parameter na mada-download) o closed-weight (API access lamang). Tingnan ang §3.4. Mga open-weight na modelo.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Pagsubaybay at mga update pagkatapos ng deployment

  Madalas mangalap at magsuri ang mga developer ng feedback ng user, subaybayan ang mga sukatan ng epekto at pagganap, at gumawa ng mga paulit-ulit na pagpapahusay upang matugunan ang mga isyung natutuklasan sa aktuwal na paggamit (‡67). Isinasagawa ang mga pagpapahusay sa pamamagitan ng pag-update sa mga integrasyon ng system, kadalasan sa pamamagitan ng patuloy na fine-tuning at pagbibigay sa mga modelo ng access sa mga panlabas na database ng (kamakailang) mga katotohanan. Dahil dito, nananatiling napapanahon ang malalaking modelo ng AI nang hindi inuulit ang buong proseso ng paunang pagsasanay (‡68*). Dahil dito, naiipon ang mga kakayahan sa sunud-sunod na yugto ng pagsasanay habang napapanatili ang katatagan at nababawasan ang mga gastos sa pagkukuwenta.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Talahanayan 1.2: Mga yugto ng pagbuo ng AI na pangkalahatang-layunin
>white|black||9|11|br Sa bawat yugto ng pagbuo ng AI para sa pangkalahatang layunin, pinahuhusay ang modelo ng AI para magamit sa mga susunod na yugto at kalaunan ay ipinapatupad bilang isang ganap na pinagsamang sistema ng AI na sinusubaybayan at ina-update.


>white|orangered|left|13|15|bb Bumubuo ang mga sistema ng pangangatwiran ng ‘mga kadena ng pag-iisip’ sa yugto ng inference upang mapahusay ang pagganap.

Nagaganap ang inference kapag may gumagamit ng AI model matapos itong sanayin. Halimbawa, nagaganap ang inference kapag hiniling ng isang tao sa isang AI system na magplano ng biyahe, at ginagamit ng modelong nasa likod nito ang mga kaugnay na bagay na natutuhan nito tungkol sa heograpiya, transportasyon, at lutuin upang makabuo ng itineraryo.

Sa nakalipas na dekada, pangunahing nagmula ang mga pagsulong sa mga kakayahan ng AI sa mas malalaking training run; ibig sabihin, sa pagdaragdag ng dami ng computing power na ginagamit sa pagsasanay ng isang modelo ng AI. Gayunman, kamakailan ay mas malaki ang mga pagsulong na nagawa ng mga mananaliksik sa pamamagitan ng pagpapahintulot sa mga modelo na magproseso ng impormasyon nang mas matagal at pagsasanay sa mga ito na gumawa ng tahasang mga hakbang sa pangangatwiran habang tinatapos ang isang gawain (‡69*, ‡70). Ang mga AI system na gumagana sa ganitong paraan ay tinatawag na ‘mga sistema ng pangangatwiran’, at ang mga paliwanag sa pagitan ng mga hakbang na binubuo ng mga ito habang nilulutas ang isang problema o sinasagot ang isang tanong ay tinatawag na ‘mga hanay ng pangangatwiran’. Nangangailangan ang mga sistema ng pangangatwiran ng mas maraming computational resource sa oras ng paggamit upang makabuo ng masalimuot na mga hanay ng pangangatwirang ito (‡71, ‡72, ‡73, ‡74), at ng mas maraming resource sa panahon ng pagsasanay upang matuto ang mga ito na mangatwiran nang mas mahusay. Sa aktuwal na paggamit, dahil sa mga kakayahang ito sa pangangatwiran, nalulutas ng mga AI system ang mas masalimuot na problema sa pamamagitan ng paulit-ulit na paghahati-hati ng isang gawain sa mas maliliit na hakbang. Ipinapakita sa Talahanayan 1.3 ang isang halimbawa ng isang sistemang walang pangangatwiran at isang sistema ng pangangatwiran na lumulutas sa iisang problema.

Nakamit ng mga sistema ng pangangatwiran ang malalaking pagsulong sa mga kakayahan sa paglutas ng mahihirap na problema. Halimbawa, noong 2025, nalutas ng mga sistemang pangangatwirang espesyalisado sa paglutas ng mga suliraning matematikal, gaya ng Gemini Deep Think ng Google at isang hindi pa inilalabas na eksperimental na modelo mula sa OpenAI, ang mga problema sa International Mathematical Olympiad (sa isang nakabalangkas na kapaligiran ng pagsusulit) sa antas na katumbas ng pagganap ng mga taong nakakuha ng gintong medalya (‡75, ‡76). Nagpakita ang mga sistema ng pangangatwiran ng malaking pag-unlad sa mga pormal na larangan gaya ng matematika, mga palaisipang lohikal, at mga nakabalangkas na tanong sa agham, kung saan tahasang mabeberipika ang pangangatwiran sa bawat hakbang (‡77). Gayunman, maaari ring magkamali ang mga sistema ng pangangatwiran sa pamamagitan ng pagbuo ng mga sunod-sunod na pag-iisip na walang kaugnayan, hindi mabunga, o paulit-ulit (‡78, ‡79).

###@ Mga update sa mga pamamaraan ng pagsasanay

Mula nang ilathala ang huling Ulat (Enero 2025), lubhang napahusay ng isang paraan ng pagsasanay na tinatawag na ‘distilasyon’ ang kahusayan sa pag-fine-tune ng ilang modelo. Kasama sa distilasyon ang pagsasanay sa isang modelong ‘estudyante’ gamit ang mga output ng isang mas makapangyarihan (at karaniwan ay mas malaking) modelong ‘guro’, upang direktang magaya ng modelong estudyante ang mga output ng modelong guro (‡80). Halimbawa, bumuo ang DeepSeek ng isang malaking modelong tinatawag na DeepSeek-R1, na mahusay sa pangangatwirang chain-of-thought. Lumikha ang R1 ng mga output ng pangangatwiran na ginamit pagkaraan upang mag-fine-tune ng mas maliliit na modelong estudyante, kabilang ang DeepSeek-V3. Napanatili ng DeepSeek-V3 ang malaking bahagi ng mga kakayahan ng R1 sa matematika, pagko-code, at pagsusuri ng dokumento- at iniulat na na-fine- tune ito sa halagang humigit-kumulang $10,000 USD (bagaman hindi iniulat ang mga gastos sa paunang pagsasanay nito) (‡81). Malamang na mas mababa ito nang ilang order of magnitude kaysa sa gastos sa pag-fine-tune ng mas malalaking modelong may katulad na kakayahan.

![table1.3](images/table1.3_example_reasoning.png)

##### Talahanayan 1.3: Isang halimbawa ng sistemang hindi nangangatuwiran (kaliwa) kumpara sa sistemang nangangatuwiran (kanan)
>white|black||9|11|br Sa paglutas sa parehong bugtong, hinango ang mga halimbawang ito sa mga tunay na tugon ng AI. Mas matagal na naglalaan ng oras at kapangyarihang pangkompyutasyon ang sistema ng pangangatwiran sa “pag-iisip” sa pamamagitan ng pagbuo ng “kadena ng pag-iisip” bago ibigay ang pinal na sagot nito.

![figure.3](images/fig1.3_AI_agent.png)

##### Figure 1.3: Isang ilustratibong representasyon ng isang ahente ng AI
>white|black||9|11|br Isang modelo ng AI (gitna) na na-configure upang paulit-ulit na magplano, mangatwiran, at gumamit ng mga tool para maisagawa ang mga gawain sa totoong mundo. Pinagmulan: International AI Safety Report 2026.


Kaya maaaring maging mura at mahusay na paraan ang distilasyon upang magkaroon ang mga modelo ng mas makapangyarihang kakayahan (‡82). Gumamit ang ilang mananaliksik ng distilasyon upang i-fine-tune ang mga modelong may mataas na kakayahan gamit ang 1,000 halimbawa lamang na nalikha mula sa mga modelong state-of- the-art (‡83). Dahil nangangailangan ang distilasyon ng dati nang umiiral na modelong guro, hindi ito direktang magagamit upang isulong ang mga kakayahan ng mga modelong state-of-the-art. Gayunman, mapabibilis nito ang paglaganap ng mga advanced na kakayahan ng AI, kahit mula sa mga modelong closed-source (‡84*).

Kasabay ng mga pagsulong sa teknolohiyang ‘distributed compute’ at desentralisadong pagsasanay (mga pamamaraang gumagamit ang mga developer ng maraming processor, server, o data centre na nagtutulungan upang magsagawa ng pagsasanay o inference ng AI (‡85, ‡86, ‡87)), nabawasan ang antas ng pagdepende ng maraming proyekto sa pagpapaunlad ng AI sa malakihan at sentralisadong imprastraktura ng compute. Dahil dito, mas nagiging posible para sa mga aktor na may mas kakaunting mapagkukunan na bumuo at mag-deploy ng mahuhusay na sistema.

###@ Mga update sa mga ahente ng AI

Mula noong huling Ulat (Enero 2025), naging posible ang pagbuo ng mas makapangyarihang mga ahente ng AI dahil sa mga pagsulong sa paraan ng pagsasama ng mga developer ng mga modelo ng AI sa mga tool. Idinisenyo ang mga ahente ng AI upang magsikap na makamit ang mga layunin, na kadalasang tinutukoy ng mga user sa natural na wika. Upang makamit ang mga layuning ito, binibigyan sila ng access sa mga tool, gaya ng memorya, interface ng computer, at mga web browser. Tinatawag na ‘scaffolding’ ang mga tool na ito at ang code na ginagamit upang pagsamahin ang mga ito sa modelo. Tinutulungan ng mga ito ang mga ahente ng AI na kusang makipag-ugnayan sa mundo, gumawa ng mga plano, alalahanin ang mahahalagang detalye, at magsikap na makamit ang mga layunin (‡88*, ‡89) nang may mas kaunting pangangasiwa o tulong mula sa mga tao. Halimbawa, isang sikat na ahente ng AI ang Manus AI na kayang mag-automate ng iba't ibang gawain, kabilang ang paghahanap sa web, pagbuo ng software, at pagbili online (‡90). Inilalarawan sa Figure 1.3 ang isang simpleng halimbawa ng ahente ng AI na binubuo ng isang ‘utak’—isang pangkalahatang layuning modelo ng AI—na maaaring paulit-ulit na magplano, mangatwiran, at gumamit ng mga tool para sa memorya, pag-browse sa web, at paggamit ng computer.

Lumalawak ang digital na imprastraktura para sa mga ahente ng AI (‡91), at lalong nagiging karaniwan ang mga ito sa iba’t ibang industriya (‡92, ‡93, ‡94). Binuo ang mga ahente ng AI para sa mga gawaing tulad ng pananaliksik (‡37), inhinyeriya ng software (‡95), pagkontrol sa robot (‡96), at serbisyo sa kostumer (‡97). Dahil sa patuloy na pananaliksik at pagpapaunlad, unti-unting nagiging mas may kakayahan at mas nagsasarili ang mga ahente ng AI o mga sistemang may maraming ahente. Tinataya ng mga mananaliksik na humigit-kumulang kada pitong buwan ay nadodoble ang pagiging kumplikado ng mga gawaing pang-benchmark ng software na kayang gawin ng mga ahente ng AI (tingnan din ang §1.2. Mga kasalukuyang kakayahan) (‡98). Ipinapangatuwiran ng mga eksperto na ang mga ahente ng AI na patuloy na nagiging mas may kakayahan ay magdudulot ng kapwa malalaking oportunidad at panganib (‡99, ‡100*) (tingnan ang §2.2.1. Mga hamon sa pagiging maaasahan).

###@ Mga kakulangan sa ebidensya

Nagmumula ang mga pangunahing kakulangan sa ebidensya tungkol sa proseso ng pagbuo ng sistemang AI na pangkalahatang- layunin sa kakulangan ng impormasyong makukuha ng publiko  tungkol sa kung paano binubuo ang mga ito. Lubos na transparent ang ilang developer tungkol sa kung paano nila binubuo ang mga sistemang AI na pangkalahatang layunin (‡1, ‡101). Gayunman, sa pangkalahatan, limitado ang kaalaman ng publiko at mga gumagawa ng patakaran tungkol sa kung paano binubuo, nilalagyan ng mga pananggalang, sinusuri, at inilulunsad ang karamihan sa mga advanced na modelo. Lalo itong totoo para sa mga sistemang AI na inilulunsad at ginagamit sa loob ng mga kompanya ng AI, ngunit hindi ginagamit o nauunawaan ng mga panlabas na stakeholder (‡102, ‡103). Dahil limitado ang panlabas na kakayahang makita ang mga ito, nagiging mahirap ang transparency at pangangasiwa. Itinuro ng iba’t ibang mananaliksik ang limitado at hindi pare-parehong transparency tungkol sa datos ng pagsasanay (‡104, ‡105, ‡106), mga modelong AI na pangkalahatang layunin (‡107, ‡108), mga ahenteng AI (‡92), mga pagsusuri (‡109), mga pipeline ng pagbuo (‡110), at kaligtasan (‡111). Kung minsan, kinakailangan ang mga limitasyon sa pagsisiwalat sa labas upang maprotektahan ang mga lihim pangkalakalan at intelektuwal na ari-arian ng mga kompanya. Gayunpaman, dahil mababa ang antas ng transparency, mas nahihirapan ang mga independiyenteng mananaliksik at mga gumagawa ng patakaran na pag-aralan ang mga modelong at sistemang AI na pangkalahatang layunin.


