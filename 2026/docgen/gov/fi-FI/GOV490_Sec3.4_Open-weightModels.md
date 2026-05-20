##########
>white|orangered|left|14|30|hr Luku 3.4
### 3.4. Avoimen painon mallit
>white|orangered|left|24|30|hb Avoimen lähdekoodin mallit

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Tärkeimmät tiedot
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tietotaso, jonka AI-yritykset tarjoavat mallien ‘painoille’, vaikuttaa näiden mallien aiheuttamiin riskeihin. Painot ovat matemaattisia parametreja, joiden avulla AI-mallit käsittelevät syötteitä ja tuottavat tulosteita. Minkä tahansa yksittäisen mallin kohdalla yritykset voivat valita, että painot pidetään täysin yksityisinä, antaa joillekin käyttäjille rajatun pääsyn tai sallia kenen tahansa ladata ne kokonaisuudessaan. Mallit, joiden painot ovat julkisesti saatavilla, kutsutaan ‘open-weight-malleiksi’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Avoimen painotuksen mallit helpottavat tutkimusta ja innovointia, mutta niiden suojatoimet voidaan poistaa helpommin. Maailmanlaajuisesti erilaiset toimijat – erityisesti ne, joilla on vähemmän resursseja – voivat käyttää avoimen painotuksen malleja tutkimus- ja kaupallisiin tarkoituksiin. Kuitenkin verrattuna suljetun painotuksen malleihin avoimen painotuksen malleja on helpompi muokata osoittamaan mahdollisesti haitallista käyttäytymistä, ja se on vaikeampaa.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Avoimen lähdekoodin mallien julkaisujen vaikutusta ei voi peruuttaa. Kun mallit on julkaistu, mallien painoja ei voi enää noutaa takaisin. Tämä tekee mahdollisten haittojen lieventämisestä vaikeampaa, kun vaarallisia ominaisuuksia sisältävä malli julkaistaan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Viimeisen raportin julkaisemisen (tammikuu 2025) jälkeen merkittävät avoimen painon mallijulkaisut ovat kaventaneet osaamiseroa johtaviin suljettuihin malleihin. Kiinalaiset kehittäjät DeepSeek ja Alibaba julkaisivat vastaavasti R1- ja Qwen-mallinsa, joiden suorituskyky on saavuttanut tasavertaista tulosta johtavien suljettujen mallien kanssa, kun taas OpenAI julkaisi ensimmäiset avoimen painon mallinsa vuoden 2019 jälkeen. Johtavien suljettujen mallien kyvykkyyksien arvioidaan nyt olevan alle vuoden edellä johtavia avoimen painon malleja useilla merkittävillä tekoälyn vertailuilla.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Keskeinen politiikkahaaste on päästä käsiksi avoimen painon (open-weight) mallien tarjoamiin hyötyihin samalla kun hallitaan niiden ominaisia riskejä. Yksi lähestymistapa on arvioida avoimen painon malleja niiden ”marginaaliriskin” näkökulmasta: siinä määrin, missä niiden julkaisu kontrafaktuaalisesti lisää yhteiskunnallista riskiä verrattuna riskiin, jota jo olemassa olevat mallit tai muut teknologiat aiheuttavat. Tämä on kuitenkin käytännössä monimutkaista. Pienet marginaaliriskin lisäykset ajan myötä voivat myös kasautua merkittäviksi lisäyksiksi kokonaisriskiin.
>oldlace|black||11|15|br      


Avoimen lähdekoodin painotetut mallit, joiden parametrit ovat julkisesti saatavilla latausta varten, vaikuttavat selvästi moniin edellä käsitellyissä jaksoissa esiin tuotuihin haasteisiin. Tekoälymallin ”painot” sisältävät ratkaisevan tiedon, jonka avulla se voi tuottaa käyttäjille hyödyllisiä vastauksia. Kun painot on julkaistu, niitä ei voi enää peruuttaa: kuka tahansa voi ladata, tutkia, muokata, jakaa ja käyttää niitä omilla tietokoneillaan tai pilvitileillään. Kun painot ovat avoimesti saatavilla, muut voivat helpommin rakentaa niiden päälle ja muokata mallia, palvella erilaisia tarpeita ja vauhdittaa innovointia (‡1317). Samalla mekanismilla myös pahantahtoiset käyttäjät voivat kuitenkin helpommin poistaa suojatoimia ja muokata avoimen painomallin malleja haitallisiin käyttötarkoituksiin (‡1122, ‡1160). Tämä on herättänyt kysymyksen siitä, tulisiko joidenkin avoimen painotettujen mallien kohdalla noudattaa erityisvaatimuksia (esim. perusteellisempi testaus ennen julkaisua) vai päinvastoin myöntää niille erityisiä poikkeuksia (esim. sääntelyraportointia koskevista vaatimuksista) (‡1033).

###@ Tausta avopainotteisista malleista

>white|orangered||14|15.5|bb Avoimen painon mallit voivat olla, mutta eivät välttämättä ole, ”avoimen lähdekoodin” malleja

Vaikka niitä kutsutaan usein “open source” -lähdekoodiksi, useimmat julkisesti julkaistut mallit kuvaillaan tarkemmin “open-weight”-malleina. Tämä johtuu siitä, että vaikka kehittäjät tarjoavat mallin painot, he eivät julkaise niihin liittyvää koulutuskoodia tai aineistoja. Lisäksi avoimen lähdekoodin ohjelmistoa yleensä luonnehtivat lisenssit, jotka asettavat vähäisiä vaatimuksia jatkotoimijoille, jotka käyttävät tai muokkaavat ohjelmistoa (‡1318). Esimerkiksi Metan Llama-malleilla on rajoittavat lisenssiehdot, ja ne sisältävät vain päätelmöintikoodin eivätkä koulutuskoodia, minkä vuoksi niitä ei tyypillisesti pidetä avoimen lähdekoodin ohjelmistona (‡1319, ‡1320). Mallien julkaisuvaihtoehdot sijoittuvat janalle täysin suljetusta täysin avoimeen lähdekoodiin, ja kussakin kohdassa tehdään erilaisia riski-hyöty -tasapainoon liittyviä kompromisseja (‡1086*, ‡1320, ‡1321). Taulukko 3.9 kuvaa nämä vaihtoehdot.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Täysin suljettu
  Käyttäjät eivät voi olla suorassa vuorovaikutuksessa mallin kanssa lainkaan.
  Esimerkit: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Isännöity käyttöoikeus
  Käyttäjät voivat olla vuorovaikutuksessa vain tietyn sovelluksen tai käyttöliittymän kautta, kuten esimerkiksi mobiilin chatbot-sovelluksen
  Esimerkit: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Pääsy mallin API:hin
  Käyttäjät voivat lähettää mallille pyyntöjä koodin kautta, mikä mahdollistaa käytön ulkoisissa sovelluksissa
  Esimerkit: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Pääsy API:n kautta hienosäätöön
  Käyttäjät voivat hienosäätää mallia omiin erityistarpeisiinsa
  Esimerkkejä: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Avoimet painot: painot saatavilla ladattavaksi
  Käyttäjät voivat ladata mallin ja suorittaa sen omilla tietokoneillaan
  Esimerkit: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Painot, data ja koodi saatavilla ladattavaksi käyttörajoituksin
  Käyttäjät voivat ladata ja ajaa mallin sekä päätellä ja kouluttaa koskevaa koodia, mutta niiden käyttöön liittyy joitakin lisenssirajoituksia
  Esimerkit: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Täysin avoin: painot, data ja koodi ovat ladattavissa ilman käyttörajoituksia
  Käyttäjillä on täydellinen vapaus ladata, käyttää ja muokata mallia, koko koodia ja dataa
  Esimerkkejä: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.9: Mallin jakamisvaihtoehdot täysin suljetusta täysin avoimeen
>white|black||9|11|br Havainnollistava valikoima mallin jakamisen vaihtoehtoja, aina täysin suljetuista malleista (mallit ovat yksityisiä ja niitä pidetään vain omistusoikeudelliseen käyttöön) täysin avoimiin ja avoimen lähdekoodin malleihin (mallin painot, data ja koodi ovat vapaasti ja julkisesti saatavilla ilman rajoituksia käytön, muokkaamisen ja jakamisen osalta). Ensimmäisiin neljään luokkaan kuuluvia malleja kutsutaan usein nimellä ”suljetut”. Tämä osio keskittyy kolmeen alimpaan riviin. Lähde: muokattu lähteestä Bommasani, 2024 (‡1317).


###@ Hyödyt ja riskit

>white|orangered|left|14|15.5|bb Avoimen painon mallit voidaan mukauttaa ja arvioida helpommin

Avoimen painoasetelman mallit tarjoavat merkittäviä hyötyjä tutkimukselle, innovoinnille ja saavutettavuudelle. Kuten jaksossa §1.1 käsitellään: Mikä on yleiskäyttöinen tekoäly?, yleiskäyttöisten tekoälymallien kouluttaminen on erittäin kallista – johtavien mallien kehittäminen maksaa satoja miljoonia dollareita. Mallin painoasetelmien julkaiseminen avoimesti mahdollistaa vähemmän resursoitujen toimijoiden mallien toistamisen, tutkimisen ja olemassa olevien järjestelmien päälle rakentamisen. Ilman tällaista pääsyä matalan resurssitason alueiden yhteisöt vaarantavat jäävänsä tekoälyn hyötyjen ulkopuolelle, mikä tekee avoimista painoasetelmista kriittisiä, jotta tekoälyn kehittämiseen saadaan mukaan globaali enemmistö (‡1322). Jatkuvan kehityksen kehittäjät voivat hienosäätää malleja erilaisiin käyttötarkoituksiin, esimerkiksi mukauttamalla niitä aliresursoitujen vähemmistökielten tarpeisiin tai optimoimalla suorituskykyä tiettyihin tehtäviin, kuten oikeudellisten asiakirjojen luonnosteluun tai lääkärimerkintöjen tekemiseen (‡1323, ‡1324*). Näin avoimen painoasetelman mallit voivat mahdollistaa useammille ihmisille ja yhteisöille tekoälyn käyttämisen ja hyötyminen siitä enemmän kuin muuten olisi mahdollista (‡1325). Niiden mallien tapauksessa, jotka eivät ole riittävän kyvykkäitä ollakseen vaarallisia, nämä hyödyt voivat ylittää painoasetelmien avoimeen julkaisemiseen liittyvän lisäriskin, vaikka tämä riippuu asianomaisten päätöksentekijöiden riskinsietokyvystä.

Avoimen mallipainotuksen julkaisu laajentaa lisäksi niiden kehittäjien ja tutkijoiden joukkoa, jotka pystyvät tutkimaan mallia, arvioimaan sen kyvykkyyksiä, testaamaan haavoittuvuuksia ja tekemään parannuksia iteratiivisesti (‡1326, ‡1327). Tämä tekee todennäköisemmäksi, että hyödylliset sovellukset ja haitalliset virheet tunnistetaan, vaikka sitä ei taata (‡1328, ‡1329). Käyttäjät voivat myös ajaa avoimen painotuksen malleja omilla laitteillaan, jolloin he voivat säilyttää kontrollin arkaluonteiseen dataan ja välttää sen lähettämisen kolmannen osapuolen palvelimille.

Kehittäjien jakaessa tietoa, kuten harjoitusaineistoa, koodia, arviointityökaluja ja dokumentaatiota sekä mallipainoja (‡1320, ‡1330, ‡1331, ‡1332*), on lisäetuja. Kun tietoa on enemmän, jatkokehittäjät ja muut tutkijat voivat paremmin ymmärtää avoimien mallipainojen malleja ja mukauttaa niitä uusiin käyttökohteisiin.

>white|orangered|left|14|15.5|bb Avoimen painon mallien suojatoimet on helpompi poistaa, mikä mahdollistaa mahdollisen haitallisen käytön

Avoimen painotuksen mallit aiheuttavat myös lisäriskejä, koska niiden suojatoimet on helpompi poistaa. Sekä avoimen painotuksen että suljetut mallit voivat sisältää suojatoimia, joilla torjutaan haitallisia käyttäjäpyyntöjä, mutta nämä suojatoimet ovat paljon helpompia poistaa avoimen painotuksen malleista. Haitalliset toimijat voivat hienosäätää mallia optimoimaan sen suorituskyvyn haitallisiin käyttötarkoituksiin, poistaa osia koodista, jotka on suunniteltu estämään haitallista käyttöä, tai peruuttaa aiemman turvallisuuteen liittyvän hienosäädön (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Tämän seurauksena avoimen mallin painot voivat pahentaa kohdassa §2.1 käsiteltyjä väärinkäytösriskejä. Riskit kasvavat, koska useammat toimijat voivat hyödyntää ja laajentaa olemassa olevia valmiuksia haitallisiin tarkoituksiin ilman valvontaa (‡1122, ‡1315). Vaikka monet käyttäjät eivät poista suojatoimia avoimen painotuksen malleista, koska heiltä puuttuu taito tai motiivi, erityisen motivoituneet haitalliset toimijat ovat huolenaihe. Lisäksi haitalliset toimijat saattavat pystyä käyttämään avoimen painotuksen malleja myös sellaisten haavoittuvuuksien tunnistamiseen, jotka ovat samanlaisia suljetuissa malleissa (‡1055*). Tällaisia puutteita on vaikeampi löytää pelkästään ajamalla suljettuja malleja, koska suljetun mallin tarjoajat voivat toteuttaa enemmän kontrolli- ja valvontatoimenpiteitä.

>white|orangered|left|14|15.5|bb Mallin painojen jakaminen on peruuttamatonta

Kun mallin painot ovat saatavilla julkiseen lataukseen, ei ole mitään tapaa toteuttaa kaikkien olemassa olevien kopioiden täydellistä takaisinvetoa. Internetin ylläpitopalvelut, kuten GitHub ja Hugging Face, voivat poistaa malleja alustoiltaan, mikä vaikeuttaa joidenkin toimijoiden löytää ladattavia kopioita ja asettaa merkittävän kynnyksen monille satunnaisille haitallisille käyttäjille (‡1339). Motivoituneet toimijat voivat kuitenkin edelleen saada kopioita, jos malli on ladattu ja uudelleenjulkaistu muualla tai tallennettu paikallisesti. Lisäksi jatkokehittäjät, jotka integroivat avoimen painon malleja omiin järjestelmiinsä, perivät myös kaikki mahdolliset puutteet, kuten haavoittuvuudet vastakkaisille hyökkäyksille (‡1055) tai mallin kyvyt kiertää valvontajärjestelmiä (katso §2.2.2. Ohjauksen menetys) (‡1315). Toisin kuin suljetuissa malleissa, joissa ylläpitäjät voivat laajasti ottaa käyttöön korjauksia, avoimen painon mallien kehittäjät eivät voi varmistaa, että käyttäjät ottavat päivitykset käyttöön.

###@ Päivitykset

Viimeisimmän raportin (tammikuu 2025) julkaisemisen jälkeen ero johtavien open-weight- ja closed-mallien kyvykkyyksissä on kaventunut. Kiinalaisista kehittäjistä on tullut erityisen tärkeitä open-weight-mallien tarjoajia. Tammikuussa 2025 DeepSeek julkaisi R1-mallinsa, joka saavutti useilla vertailumittareilla (‡1340) OpenAI:n o1:n tasoa vastaavan suorituskyvyn. Alicloudan Qwen-mallit ovat samoin saaneet lisää jalansijaa ja ovat elokuuhun 2025 mennessä (‡1341, ‡1342*) vallanneet Chatbot Arenalla, laajasti käytetyllä suorituskykymittarilla, ykköspaikan open-weight-mallien joukossa. Elokuussa 2025 OpenAI julkaisi ensimmäiset open-weight-mallinsa sen jälkeen, kun GPT-2 julkaistiin vuonna 2019: gpt-oss-120b ja gpt-oss-20b. Meta on jatkanut Llama-mallien julkaisemista open weight -painotuksilla. Johtavien closed-mallien kyvykkyyksien arvioidaan nyt olevan alle vuoden johtavien open-mallien edellä merkittävissä tekoälyvertailuissa (Kuva 3.10).

###@ Todisteiden puutteet

Keskeinen näyttöaukko koskee teknisten ratkaisujen tosielämän tehokkuutta sen estämisessä, että avoimen painon malleja käytetään väärin. Tutkijat ovat ehdottaneet erilaisia lähestymistapoja, joilla malleja voitaisiin tehdä manipuloinnin kestäviksi. Tähän kuuluu uusia koulutustekniikoita, jotka on suunniteltu tekemään malleista vastustuskykyisiä haitalliselle muokkaukselle (‡1276), haitallisen sisällön suodatusta harjoitusaineistosta (‡55) sekä puolustautumiskeinoja jailbreak-hyökkäyksiä vastaan (‡675, ‡676). Näitä tekniikoita otetaan nyt käyttöön tosielämän julkaisuissa suurilta kehittäjiltä. Esimerkiksi OpenAI hyödynsi joitakin näistä tekniikoista gpt-oss-malleissaan ja raportoi, että haitallisesti hienosäädetyillä versioilla ei saavutettu korkeita kyvykkyyskynnysarvoja (‡1344*). Tutkimus on kuitenkin osoittanut, että pahantahtoiset toimijat voivat poistaa suojaukset käytöstä kouluttamalla malleja uudelleen haitallisilla esimerkeillä (‡1345, ‡1346). Lisäksi suojauksen kestävyyttä on edelleen vaikeaa arvioida luotettavasti, mikä tekee niiden tehokkuudesta tosielämän hyökkäyksiä vastaan epävarmaa (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Kuva 3.10: Kyvykkyysvaje johtavien avoimen painon ja suljettujen tekoälymallien välillä
>white|black||9|11|br Huippusuoriutuvien avoimen painon (tummansininen) ja suljettujen (vaaleansininen) mallien Epoch Capabilities Index (ECI) -pisteet ajan myötä. ECI yhdistää 39 vertailuarvion pisteet yhdeksi yleisen kyvykkyyden asteikoksi. Parhaat avoimen painon mallit jäävät noin vuoden jälkeen suljetuista malleista. Lähde: Epoch AI, 2025 (‡1343).


###@ Lievitykset

Avoimen mallin riskeihin liittyvät tekniset lieventämistoimet toimivat koko tekoälyn kehitys- ja käyttöönottoprosessin ajan (‡1141, ‡1195, ‡1347). Esimerkiksi kun malleja kehitetään, kehittäjät ja jatkokehityksen sovittimet voivat suodattaa arkaluonteisen sisällön harjoitusdatasta haitallisten kykyjen minimoimiseksi. Haitallisten esimerkkien poistaminen mallin harjoitusdatasta voi estää vihamielisen jatkohienosäädön 10 kertaa tehokkaammin kuin harjoittelun jälkeen lisättävät puolustukset, vaikka se voi samalla vaikuttaa hyödyllisiin kykyihin (‡55). Tekoälysovellusten tarjoajat voivat myös ottaa käyttöön tapausraportointi- ja vasteen toteutusmekanismeja (‡1348).

Lisäksi alustoja kuten HuggingFace ja GitHub käyttävät alustojensa käyttöehtoja poistamaan malleja, joita on muokattu haitallisiin tarkoituksiin (‡1141, ‡1324). Mallikehittäjät voivat tarjota auditoijille täyden pääsyn ennen julkaisua tai valita niin sanotun vaiheistetun julkaisustrategian – julkaista malleja asteittain yhä suuremmille ryhmille (‡1086). Tämä voi auttaa tunnistamaan mahdollisia toimintahäiriöitä tai haavoittuvuuksia ennen kuin malli on laajalti saatavilla (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Huom 3.1: Mallin painojen tietoturva
>oldlace|black|left|13|15|hb Huom 3.1: Mallin painojen tietoturva
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Tässä osiossa käsitellyt riskit olettavat, että mallin painot julkaistaan tarkoituksella. Suljetut mallin painot voivat kuitenkin tulla saataville myös varkauden tai vuodon kautta. Suljettujen mallien kehittäminen maksaa satoja miljoonia dollareita (§1.1. Mitä yleiskäyttöinen tekoäly on?) ja ovat keskimäärin kyvykkäämpiä kuin avoimen painon mallit (‡1343). Tämä tekee niistä houkuttelevia kohteita toimijoille aina harrastelaisista hakkereista nation-state-toimijoihin, jotka pyrkivät saamaan käyttöönsä johtavia tekoälymalleja.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Varastetut suljetun mallin painot aiheuttaisivat riskejä, jotka ovat samanlaisia kuin edellä avoimia painoja koskevissa malleissa, mutta mahdollisesti ilman mitään niistä lieventävistä toimista. Haitalliset toimijat voisivat poistaa suojamekanismeja kaikkein kyvykkäimmistä malleista. Toisin kuin lailliset kehittäjät, tällaiset toimijat eivät joutuisi reputaatioriskejä, oikeudellisia tai kaupallisia rajoitteita koskevien vaikutusten piiriin, jotka tällä hetkellä kannustavat edelläkävijöitä edustavia tekoälyyrityksiä ottamaan mallinsa käyttöön turvallisesti.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Nykyiset suojaustasot vaihtelevat toimialalla, ja ne saattavat olla riittämättömiä kehittyneitä hyökkääjiä vastaan. Osa kehittäjistä sitoutuu suojaamaan mallien painot kyberrikollisryhmiä ja sisäpiirintuhkia vastaan (‡582), kun taas toiset ovat tehneet mitään julkisia suojaussitoumuksia (‡1109, ‡1349). Tutkimusten mukaan tekoälydata-asemat eivät ehkä pysty kestämään hyökkäyksiä kaikkein kehittyneimmiltä ja hyvin resursoiduilta toimijoilta (‡582, ‡1350, ‡1351). Joulukuuhun 2025 mennessä ei ole vahvistettuja, julkisesti dokumentoituja tapauksia mallien painojen varkaudesta. Muista suojausloukkauksista johtavissa tekoälyyrityksissä on kuitenkin raportoitu, mukaan lukien Microsoftin sähköpostijärjestelmien tunkeutuminen (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Näiden tietoturva-aukkojen korjaaminen edellyttäisi huomattavia investointeja laitteistoon, ohjelmistoon, henkilöstöön ja toimitilojen tietoturvaan. Jotkin tietoturvaparannukset voitaisiin toteuttaa suhteellisen nopeasti koordinoidulla toiminnalla (‡1122). Muut kriittiset toimenpiteet, kuten laitteistotoimitusketjujen ja toimitilojen suojaaminen, vaatisivat kuitenkin todennäköisesti vuosia (‡1122). Lisäksi yksityisillä yrityksillä ei välttämättä ole resursseja tai tietoa riittävien suojatoimien kehittämiseen yksin. Esimerkiksi tekoälykehittäjillä ei ole sellaista pääsyä luokiteltuun uhka-analytiikkaan kuin hallituksilla (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Haasteet poliittisille päättäjille

Keskeinen haaste päättäjille on turvata avoin- painomallien jakamisen hyödyt ilman, että riskiä lisätään merkittävästi. Jotta katastrofaalinen haitta voitaisiin välttää, avoin- painomallien kehittäjien ei tulisi julkaista malleja arvioimatta riskejä, sekä hyödyntäen vakiintuneita arviointimenetelmiä, joita käytetään suljetuille malleille, että tekemällä lisäksi testausta, kun otetaan huomioon, että pahantahtoiset toimijat voivat hienosäätää malleja ja poistaa turvatoimia. Käytännössä tämä voi olla vaikeaa, koska kyvykkyyksien kehittyminen voi olla arvaamatonta, avoin- painon julkaisut ovat peruuttamattomia ja tarvitaan arviointityötä sen ennakoimiseksi, milloin julkaisu aiheuttaisi merkittävän mahdollisen haitan. Yksi lähestymistapa on arvioida avoimien julkaisujen ”marginaaliriski”: se, missä määrin julkaisu kontrafaktuaalisesti lisäisi yhteiskunnallista riskiä jo olemassa olevien mallien tai muiden teknologioiden aiheuttaman riskin lisäksi (‡556, ‡1033, ‡1354, ‡1355) (katso §3.2. Riskinhallinnan käytännöt). Kuitenkin monimutkaista on arvioida, miten järjestelmä muuttaa alavirran riskiä sen jälkeen, kun se on otettu käyttöön, ja arviointi on kontekstisidonnaista. Riskin asteittaiset kasvu erät peräkkäisten julkaisujen myötä voivat kumuloitua ajan myötä merkittäviksi kokonaisriskin lisäyksiksi, vaikka kunkin julkaisun marginaaliriski vaikuttaisi hyväksyttävältä (‡1356, ‡1357). AI-kyvykkyyksien kaksoiskäyttöluonne vaikeuttaa lisäksi hallintaa: piirteet, jotka mahdollistavat hyödyllisiä sovelluksia lääketieteessä tai tutkimuksessa, voidaan muuntaa haitaksi, ja kun painot ovat julkisia, laillisten ja haitallisten käyttötapojen erottaminen voi olla vaikeaa. Myös on epäselvää, kuka olisi vastuussa, kun avoin- painomalleja muokataan haitallisiin tarkoituksiin.

