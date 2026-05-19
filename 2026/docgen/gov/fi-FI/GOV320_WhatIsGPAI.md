###@ Mitä ovat yleiskäyttöiset tekoälyjärjestelmät?

Yleiskäyttöiset tekoälyjärjestelmät ovat ohjelmistoja, jotka oppivat malleja suurista datamääristä ja joiden avulla ne pystyvät suorittamaan monenlaisia tehtäviä sen sijaan, että ne olisi erikoistettu yhteen tiettyyn toimintaan tai toimialaan (katso Taulukko 1.1). Näiden järjestelmien luomiseksi tekoälykehittäjät toteuttavat monivaiheisen prosessin, joka vaatii huomattavia laskentaresursseja, suuria aineistoja ja erikoisosaamista (katso Taulukko 1.2). Laskentaresursseja (usein lyhennettynä muotoon ‘compute’) tarvitaan sekä tekoälyjärjestelmien kehittämiseen että niiden käyttöönottoon, ja ne sisältävät erikoistuneita tietokonelastuja sekä ohjelmistot ja infrastruktuurin, joita niiden ajaminen edellyttää.† Koska ne on koulutettu suurilla ja monipuolisilla aineistoilla, yleiskäyttöiset tekoälyjärjestelmät voivat suorittaa monia erilaisia tehtäviä, kuten tiivistää tekstiä, tuottaa kuvia tai kirjoittaa tietokonekoodia. Tässä osiossa selitetään, miten yleiskäyttöiset tekoälyjärjestelmät tehdään, mitä ‘päättely’ -malleilla tarkoitetaan, ja miten politiikkapäätökset muovaavat yleiskäyttöisten tekoälyjärjestelmien kehitystä.

    Huom † -- Termi ‘compute’ voi viitata myös joko prosessorin suorittamien laskutoimitusten määrän mittaamiseen (tyypillisesti mitattuna kelluvan pilkun operaatioina sekunnissa) tai erityisesti niihin laskutoimituksiin käytettävään laitteistoon (kuten näytönohjaimiin).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Kielijärjestelmät
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Komento A (‡3*)
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
###@ kuvageneraattorit
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Videogeneraattorit
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Näen 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotiikka- ja navigointijärjestelmät
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Ennustajat monimuotoisten biomolekyylirakenteiden luokille
- AlphaFold 3 (‡27)
- Laajenna (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ AI-agentit
- AlphaEvolve (‡31*)
- ChatGPT-agent (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 1.1: Yleiskäyttöiset tekoälytyypit
>white|black||9|11|br On olemassa useita erilaisia yleiskäyttöisiä AI-malleja. Tässä raportissa malleja, jotka pystyvät ennustamaan rakenteellista tietoa useille molekyyliluokille, pidetään ’yleiskäyttöisinä’ AI-malleina, koska niitä voidaan mukauttaa monenlaisiin tehtäviin. Esimerkiksi mallit, joita on koulutettu ennustamaan proteiinirakenne, soveltuvat moniin muihin tehtäviin, kuten proteiinien välisten vuorovaikutusten ennustamiseen, pienten molekyylien sitoutumiskohtien ennustamiseen sekä syklisien peptidien ennustamiseen ja suunnitteluun (‡40).


>white|orangered|left|13|15|bb Syväoppiminen on perusta yleiskäyttöiselle tekoälylle

Tutkijat rakentavat yleiskäyttöisiä tekoälymalleja prosessilla, jota kutsutaan nimellä ”syväoppiminen”, jossa mallit koulutetaan oppimaan esimerkeistä (‡41). Toisin kuin ohjelmistokehitys, syväoppimismallit oppivat suorittamaan tehtäviä datasta käsin sen sijaan, että ne nojaisivat käsin kirjoitettuihin ohjeisiin. Käsittelemällä suuria määriä dataa, kuten kuvia, tekstiä tai ääntä, nämä mallit löytävät tapoja esittää kyseinen data, jolloin ne muodostavat sisäisiä esityksiä malleista (kuten muodoista, sanayhteyksistä tai äänirakenteista), jotka auttavat mallia tunnistamaan suhteita ja tuottamaan tuloksia, jotka vastaavat sen koulutustavoitetta. Sen jälkeen ne käyttävät opittuja sisäisiä esityksiä abstrakteina piirteinä analysoidakseen uutta, samankaltaista dataa ja tuottaakseen tuloksia samassa tyylissä. Esimerkiksi yleiskäyttöinen tekoälymalli, jota on koulutettu riittävällä määrällä esimerkkejä 1800-luvun romanttisesta englantilaisesta runoudesta, voi tunnistaa uusia kyseiseen tyyliin kuuluvia runoja ja tuottaa uutta aineistoa samankaltaisessa tyylissä.

Yksityiskohtaisemmalla tasolla syväoppiminen toimii käsittelemällä dataa kerrosten läpi, joissa toisiinsa kytkeytyneet informaationkäsittelysolmut välittävät tietoa. Näitä solmuja kutsutaan usein “neuron(e)iksi”, koska ne ovat löyhästi inspiroituneet biologisten aivojen neuroneista (“neuroverkot”) (Kuva 1.1) (‡42). Kun informaatio virtaa neuronikerroksesta seuraavaan, malli muuntaa dataa asteittain yhä abstraktimmiksi esityksiksi opittujen ominaisuuksien ryhminä – malleille automaattisesti datasta löytyneinä kuvioina, eivät käsin koodattuina. Esimerkiksi kuvanprosessointimallissa ensimmäiset kerrokset voivat oppia tunnistamaan yksinkertaisia piirteitä, kuten reunoja tai perusmuotoja, kun taas syvemmät kerrokset yhdistävät nämä piirteet poimiakseen monimutkaisempia kuvioita, kuten kasvoja tai objekteja.

Kaikkien kerrosten ominaisuudet löydetään optimointiprosessin kautta, joka määrittelee koulutusmenettelyn. Koulutuksen aikana, kun malli tekee virheitä, syväoppimisen algoritmit säätävät neuronien välisten eri yhteyksien vahvuutta parantaakseen mallin suorituskykyä. Kunkin solmujen välisen yhteyden vahvuutta kutsutaan usein ”painoksi”. Tämä kerroksittainen lähestymistapa antaa syväoppimiselle sen nimen.

Syväoppiminen on osoittautunut erittäin tehokkaaksi mahdollistamaan AI-järjestelmien suorittamisen tehtäviä, jotka aiemmin katsottiin perinteisissä käsiohjelmoiduissa laskentajärjestelmissä sekä muissa varhaisemmissa symbolisissa tai sääntöihin perustuvissa AI-menetelmissä vaikeiksi. Suurin osa nykyisistä huipputason yleiskäyttöisistä AI-malleista perustuu nykyisin tiettyyn hermoverkkoarkkitehtuuriin, jota kutsutaan nimellä ”transformer” (‡43, ‡44). Transformerit käyttävät ”attention”-mekanismia (‡45), joka auttaa mallia kohdistamaan käsiteltäessä tietoa huomion kaikkein olennaisimpia osia kohti syötedatassa, kuten siihen, mitkä sanan lauseessa ovat merkityksen ymmärtämisen kannalta tärkeimpiä. Tämänkaltaisen mallien rakentamistavan ansiosta on saavutettu merkittäviä parannuksia käännöksissä (‡43), luonnollisen kielen käsittelyssä (‡46), kuvantunnistuksessa (‡47) sekä puheentunnistuksessa (‡48, ‡49), mikä on lopulta johtanut nykyisin kehittyneimpien mallien kehittämiseen.

![fig1.1](images/fig1.1_neural_network.png)

##### Kuva 1.1: Havainnollistava esitys 'neuroverkosta'
>white|black||9|11|br Nykyiset yleiskäyttöiset tekoälymallit perustuvat näihin verkkoihin, jotka ovat löyhästi inspiroituneita biologisista aivoista. Eri verkoilla on eri kokoja ja arkkitehtuureja. Kaikkia kuitenkin yhdistää se, että ne koostuvat toisiinsa kytkeytyneistä tietoa käsittelevistä yksiköistä, joita kutsutaan ”neuroneiksi”, ja yhteyksien vahvuuksia neuroinien välillä kutsutaan ”painoiksi”. Painoja päivitetään harjoittelussa suurilla tietomäärillä. Lähde: International AI Safety Report 2025 (‡50) (muokattu).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Kuva 1.2: Kaavioesitys yleiskäyttöisen tekoälyn kehitysvaiheista
>white|black|left|9|11|br Kansainvälinen tekoälyn turvallisuusraportti 2026.


>white|orangered|left|13|15|bb Yleiskäyttöistä tekoälyä kehitetään vaiheittain

Yleiskäyttöisen tekoälyjärjestelmän kehittäminen edellyttää useita vaiheita, aina mallin alkuperäisestä koulutuksesta käyttöönoton jälkeiseen seurantaan ja päivityksiin (Kuva 1.2). Käytännössä nämä vaiheet limittyvät usein iteratiivisesti. Jokainen vaihe vaatii erilaisia resurssipanoksia (esim. dataa, työvoimaa, laskentatehoa) ja erilaisia tekniikoita, ja niitä toteutetaan toisinaan eri kehittäjien toimesta (Kuva 1.2 ja Taulukko 1.2).

Esimerkiksi mallin esikoulutus yleensä edellyttää suuria määriä laskentatehoa ja dataa, minkä vuoksi tämä vaihe on erityisen herkkä politiikoille, jotka vaikuttavat pääsyyn laskentaresursseihin tai harjoitusdataan (‡51, ‡52). Samoin datan kuratointi ja jotkin mallin hienosäädön menetelmät edellyttävät tällä hetkellä suuria määriä inhimillistä työtä aloitusdatan merkitsemiseen (‡53). Tämän vuoksi tämä vaihe on herkkä muutoksille työvoimakustannuksissa, alustan käytäntöissä tai sellaisissa sääntelyissä, jotka vaikuttavat rajat ylittäviin sopimusjärjestelyihin.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Datan kerääminen ja kuratointi
> 
  Ennen yleiskäyttöisen tekoälymallin kouluttamista kehittäjät ja datan käsittelijät keräävät, puhdistavat, kokoavat ja standardoivat raakaa koulutusaineistoa mallin opittavaksi sopivaan muotoon. Tämä voi olla työläs prosessi. Huippumalleja taustalla olevat koulutusaineistot koostuvat valtavasta määrästä esimerkkejä kaikkialta internetistä.
  Tiimit kehittävät usein kehittyneitä suodatustapoja vähentääkseen haitallista sisältöä, poistaakseen kaksoiskappaleaineistoa ja parantaakseen edustavuutta eri aiheiden ja lähteiden välillä (‡54, ‡55). Tietoaineiston kuratointi voi myös auttaa vähentämään tekijänoikeus- ja yksityisyydensuojaloukkauksia, poistamaan esimerkkejä, jotka sisältävät vaarallista tietoa, käsittelemään useita kieliä ja parantamaan dokumentaatiota datan alkuperästä (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Esikoulutus (koulutuksen ensimmäinen vaihe)

  Ennakkokoulutuksen aikana kehittäjät syöttävät malleille valtavia määriä monimuotoista dataa, jotta niihin juurrutetaan laaja tietopohja ja kontekstuaalinen ymmärrys. Tämä prosessi tuottaa niin sanotun ”perusmallin”. Kyseessä on erittäin data- ja laskentaintensiivinen prosessi.

  Esikoulutuksen aikana mallit altistetaan miljardille tai biljoonalle esimerkille sisällöstä, kuten kuville, teksteille tai äänelle. Tämän altistumisen kautta malli vähitellen löytää abstrakteja ominaisuuksia edustamaan dataa ja oppii, miten nämä ominaisuudet liittyvät toisiinsa, mikä mahdollistaa sen, että se pystyy ymmärtämään uusia syötteitä kontekstissa. Tämä esikoulutusprosessi kestää viikkoja tai kuukausia (‡59) ja käyttää kymmeniä tai satoja tuhansia grafiikkaprosessoreita (GPU) tai tensoriprosessoreita (TPU) (‡60) – erikoistuneita tietokonesiruja, jotka on suunniteltu käsittelemään nopeasti monia tällaisia laskutoimituksia. Osa kehittäjistä tekee esikoulutusta omalla laskentakapasiteetillaan, kun taas toiset käyttävät erikoistuneiden laskentapalveluntarjoajien tarjoamia resursseja.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Jälkikoulutus ja hienosäätö (koulutuksen toinen vaihe)

  ’Jälkikoulutus’ tarkentaa edelleen perusmallia ja optimoi sen tiettyä käyttötarkoitusta varten. Se on kohtalaisen laskentatehoa vaativa mutta erittäin työvoimavaltainen prosessi. Siirtyminen ’synteettisen datan’ käyttöön – keinotekoisesti tuotetun tiedon, joka jäljittelee reaalimaailman dataa mutta joka luodaan algoritmeilla tai simuloinneilla – auttaa tekemään tästä vaiheesta vähemmän työvoimavaltaisen.
  Jälkikoulutus sisältää erilaisia hienosäätötekniikoita ja muita muutoksia. “Ohjattu hienosäätö” tarkoittaa koulutetun mallin jatkokouluttamista tietyillä tietojoukoilla mallin suorituskyvyn parantamiseksi kyseisessä osa-alueessa (‡61, ‡62). Esimerkiksi yleiskäyttöistä mallia voidaan kouluttaa edelleen suurella radiologisten kuvien aineistolla. “Vahvistusoppiminen” (RL) tarkoittaa mallin suorituskyvyn parantamista “palkitsemalla” mallia (antamalla positiivista palautetta) toivotuista tuotosista ja “rankaisemalla” mallia (antamalla negatiivista palautetta) ei-toivotuista tuotosista. Sillä on kaksi merkittävää alaluokkaa. “Vahvistusoppiminen ihmisen palautteen perusteella” tarkoittaa sellaisten tuotosvaihtoehtojen palkitsemista, jotka vastaavat ihmisen mieltymyksiä, ja sellaisten rankaisemista, jotka eivät, perustuen ihmisen antamaan palautteeseen (‡63, ‡64*). “Vahvistusoppiminen varmennettavilla palkkioilla” (RLVR) on käytössä mallin suorituskyvyn parantamiseksi tehtävissä, joissa vaaditaan tosiasiallista oikeellisuutta, kuten matematiikan tai koodin generoinnissa. Kehittäjät vuorottelevat tyypillisesti jälkikoulutustekniikoiden soveltamisen ja testien ajamisen välillä, kunnes tulokset osoittavat, että malli täyttää halutut vaatimukset.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Järjestelmäintegraatio

  Kehittäjät yhdistävät yhden tai useamman yleiskäyttöisen tekoälymallin muihin osiin luodakseen “tekoälyjärjestelmän”, joka on valmiina käyttöön. GPT-5 (esimerkiksi) on yleiskäyttöinen tekoälymalli, joka käsittelee tekstiä, kuvia ja ääntä, kun taas ChatGPT on yleiskäyttöinen tekoälyjärjestelmä, joka yhdistää useita eri kokoisia ja kyvykkyyksiltään erilaisia malleja sekä keskusteluliittymän, sisällön käsittelyn, Web-käytön ja sovellusten integraation tuottaakseen toimivan tuotteen.
  Lisäksi AI-mallien saattamiseen toimintaan järjestelmän muut osat pyrkivät myös parantamaan kyvykkyyttä, hyödyllisyyttä ja turvallisuutta. Esimerkiksi järjestelmä saattaa sisältää suodattimen, joka tunnistaa ja estää mallin syötteet tai ulostulot, jotka sisältävät haitallista sisältöä (‡65*). Kehittäjät käyttävät myös yhä useammin ‘telineytystä’ (scaffolding) – lisäohjelmistoa, joka rakennetaan yleiskäyttöisten AI-mallien ympärille ja jonka avulla ne voivat suunnitella etukäteen, tavoitella päämääriä ja olla vuorovaikutuksessa maailman kanssa (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Käyttöönotto ja julkaisu
  Käyttöönotto on prosessi, jossa integroidtu tekoälyjärjestelmä saatetaan sen käyttötarkoituksen mukaiseen käyttöön. Kehittäjät ja käyttöönotosta vastaavat ottavat tekoälyjärjestelmiä käyttöön todellisissa sovelluksissa, tuotteissa tai palveluissa. Kehittäjät voivat ottaa tekoälyjärjestelmiä käyttöön joko sisäisesti (omaa käyttöä varten) tai ulkoisesti (yksityisille asiakkaille tai julkiseen käyttöön). Kun tekoälyjärjestelmiä otetaan käyttöön ulkoisesti, yritykset tarjoavat usein käyttäjille pääsyn verkkokäyttöliittymien tai sovellusohjelmointirajapintojen (API) kautta, joiden avulla käyttäjät voivat käyttää ja suorittaa järjestelmää. Esimerkiksi yksi yritys saattaa suunnitella räätälöidyn asiakaspalvelubotn, jota käytetään toisen yrityksen yleiskäyttöisen tekoälyjärjestelmän avulla.
  ‘AI-järjestelmän käyttöönotto’ tarkoittaa sitä, että malli saatetaan saataville tosielämän käyttöön integroitujen työkalujen ja käyttöliittymien avulla, kun taas ‘mallin julkaisu’ tarkoittaa perusmallin saattamista muiden saataville – joko avoimilla painoilla (ladattavat parametrit) tai suljetuilla painoilla (vain API-käyttö). Katso §3.4. Avoimella painolla julkaistavat mallit.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Käyttöönoton jälkeinen seuranta ja päivitykset

  Kehittäjät keräävät usein käyttäjäpalautetta ja analysoivat sitä, seuraavat vaikutus- ja suorituskykymittareita sekä tekevät iteratiivisia parannuksia korjatakseen ongelmia, joita havaitaan tosielämän käytössä (‡67). Parannuksia tehdään päivittämällä järjestelmäintegraatioita, usein jatkuvalla hienosäädöllä ja tarjoamalla malleille pääsy ulkoisiin tietokantoihin, joissa on (tuoreita) tosiasioita. Näin suuret tekoälymallit pysyvät ajan tasalla toistamatta koko esikoulutusprosessia (‡68*). Tämä mahdollistaa kyvykkyyksien karttumisen peräkkäisissä koulutuskierroksissa säilyttäen samalla vakauden ja vähentäen laskennallisia kustannuksia.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 1.2: Yleiskäyttöisen tekoälyn kehitysvaiheet
>white|black||9|11|br Jokaisessa yleiskäyttöisen tekoälyn kehitysvaiheessa tekoälymallia parannetaan jatkokäyttöä varten, ja lopulta se otetaan käyttöön täysin integroituna tekoälyjärjestelmänä, jota valvotaan ja päivitetään.


>white|orangered|left|13|15|bb Päättelyjärjestelmät tuottavat päättelyketjuja (”chains of thought”) päätelmävaiheessa parantaakseen suorituskykyä

Päättely tapahtuu, kun joku käyttää tekoälymallia sen kouluttamisen jälkeen. Esimerkiksi päättelyä tapahtuu, kun henkilö pyytää tekoälyjärjestelmää suunnittelemaan matkan ja sen taustalla oleva malli hyödyntää oppimiaan, olennaisia näkökulmia maantieteestä, liikenteestä ja ruuasta laatiakseen matkasuunnitelman.

Viimeisen vuosikymmenen aikana tekoälyn kyvykkyyksien edistys on suurelta osin tullut suuremmista koulutusajoista; eli lisäämällä se määrä laskentaa (compute), jota käytetään tekoälymallin kouluttamiseen. Viime aikoina tutkijat ovat kuitenkin saaneet enemmän hyötyä siitä, että mallit saavat käsitellä tietoa pidempään ja että niitä koulutetaan tuottamaan tehtävän suorittaessaan eksplisiittisiä päättelyvaiheita (‡69*, ‡70). Tällaisen toiminnan omaavia tekoälyjärjestelmiä kutsutaan ‘päättelyjärjestelmiksi’, ja väliin jääviä selityksiä, joita ne käyvät läpi ratkaistessaan ongelmaa tai vastatessaan kysymykseen, kutsutaan ‘ajatusketjuiksi’ (chains of thought). Päättelyjärjestelmät vaativat enemmän laskennallisia resursseja käytön aikana, jotta ne voivat tuottaa nämä kehittyneet ajatusketjut (‡71, ‡72, ‡73, ‡74), ja enemmän resursseja koulutuksen aikana, jotta ne oppivat päättämään paremmin. Käytännössä nämä päättelykyvykkyydet mahdollistavat sen, että tekoälyjärjestelmät ratkaisevat monimutkaisempia ongelmia hajottamalla tehtävän iteratiivisesti pienempiin vaiheisiin. Taulukko 1.3 esittää esimerkin ei-päättelyjärjestelmästä ja päättelyjärjestelmästä, jotka ratkaisevat saman ongelman.

Päättelyjärjestelmät ovat saavuttaneet merkittäviä läpimurtoja kyvyissä vaikeissa ongelmissa. Esimerkiksi vuonna 2025 päättelyjärjestelmät, jotka on erikoistettu matemaattisten ongelmien ratkaisemiseen, kuten Googlen Gemini Deep Think ja julkaisematonta kokeellista mallia vastaava malli OpenAI:lta, ratkaisivat Kansainvälisen matemaattisten olympiadien tehtäviä (jäsennellyssä testiasetelmassa) tasolla, joka vastaa ihmisen kulta-mitalitason suoritusta (‡75, ‡76). Päättelyjärjestelmät ovat osoittaneet huomattavaa edistystä formaaleissa osa-alueissa, kuten matematiikassa, logiikkatehtävissä ja jäsennellyissä tieteellisissä kysymyksissä, joissa vaiheittainen päättely voidaan eksplisiittisesti todentaa (‡77). Toisaalta päättelyjärjestelmät voivat myös epäonnistua tuottamalla epäolennaisia, tuottamattomia tai toistuvia ajatusten ketjuja (‡78, ‡79).

###@ Päivityksiä koulutusmenetelmiin

Viimeisen raportin (tammikuu 2025) julkaisun jälkeen koulutusmenetelmä, jota kutsutaan nimellä ‘distillointi’, on huomattavasti parantanut joidenkin mallien hienosäädön tehokkuutta. Distillointi tarkoittaa, että ‘opiskelijamallia’ (student) koulutetaan tehokkaamman (ja yleensä suuremman) ‘opettajamallin’ (teacher) tuottamien tulosteiden perusteella, jolloin opiskelijamalli voi suoraan jäljitellä opettajan tuottamia tuloksia (‡80). Esimerkiksi DeepSeek kehitti suuren mallin nimeltä DeepSeek-R1, joka on erityisen hyvä ketjuajatteluun (chain-of-thought) perustuvassa päättelyssä. R1 tuotti päättelyyn liittyviä tulosteita, joita käytettiin sitten hienosäädön tekemiseen pienemmille opiskelijamalleille, mukaan lukien DeepSeek-V3. DeepSeek-V3 säilyttää suuren osan R1:n matemaattisista, koodaukseen liittyvistä ja dokumenttianalyysin kyvyistä, ja sen kerrottiin olevan hienosäädetty noin $10,000 USD:lla (vaikka sen esikoulutuksen kustannuksia ei raportoitu) (‡81). Tämä on todennäköisesti suuruusluokkaa pienempi kuin hienosäädön kustannus sellaisten samankaltaisesti kykenevien, suurempien mallien osalta.

![table1.3](images/table1.3_example_reasoning.png)

##### Taulukko 1.3: Esimerkki ei-päättelyjärjestelmästä (vasemmalla) verrattuna päättelyjärjestelmään (oikealla)
>white|black||9|11|br Ratkaisemme saman arvoituksen; nämä esimerkit on mukautettu todellisista AI-vastauksista. Päättelyjärjestelmä käyttää enemmän aikaa ja laskentatehoa “ajatteluun” rakentamalla “ajattelun ketjun” ennen lopullisen vastauksen antamista.

![figure.3](images/fig1.3_AI_agent.png)

##### Kuva 1.3: Havainnollistava esitys tekoälyagentista
>white|black||9|11|br AI-malli (keskellä), joka on määritetty iteratiivisesti suunnittelemaan, tekemään päättelyä ja käyttämään työkaluja reaalimaailman tehtävien suorittamiseksi. Lähde: International AI Safety Report 2026.


Näin ollen tislaus voi olla halpa ja tehokas tapa, jolla mallit saavat lisää voimakkaita ominaisuuksia (‡82). Jotkut tutkijat ovat käyttäneet tislauksen avulla mallien hienosäätöä erittäin kyvykkäillä malleilla käyttäen jopa vain 1,000 esimerkkiä, jotka on generoitu huipputason malleista (‡83). Koska tislaus edellyttää valmiiksi olemassa olevaa opettajamallia, sitä ei voi käyttää suoraan edistämään huipputason mallien ominaisuuksia. Se voi kuitenkin nopeuttaa kehittyneiden tekoälyominaisuuksien yleistymistä, myös suljetun lähdekoodin malleista (‡84*).

Yhdessä teknologisten edistysaskeleiden kanssa niin sanotussa “distributed compute” -laskennassa ja hajautetussa koulutuksessa (lähestymistavat, joissa kehittäjät käyttävät useita prosessoreita, palvelimia tai datakeskuksia, jotka toimivat yhdessä suorittaakseen AI-koulutusta tai -inferenssiä (‡85, ‡86, ‡87)), se, missä määrin monet AI-kehityshankkeet ovat riippuvaisia suurimittaisesta, keskitetystä laskenta-infrastruktuurista, on vähentynyt. Tämä mahdollistaa yhä useammin myös heikommin resursoitujen toimijoiden kehittää ja ottaa käyttöön tehokkaita järjestelmiä.

###@ Päivityksiä AI-agentteihin

Viimeisen raportin (tammikuu 2025) jälkeen edistysaskelia siinä, miten kehittäjät yhdistävät AI-malleja työkaluihin, on mahdollistanut yhä tehokkaampien AI-agenttien kehittämisen. AI-agentit on suunniteltu tavoittelemaan tavoitteita, jotka usein käyttäjät määrittelevät luonnollisella kielellä. Saavuttaakseen nämä tavoitteet niille annetaan pääsy työkaluihin, kuten muistiin, tietokäyttöliittymään ja verkkoselaimiin. Näitä työkaluja ja koodia, jota käytetään niiden yhdistämiseen mallin kanssa, kutsutaan nimellä ‘scaffolding’, ja ne auttavat AI-agentteja toimimaan maailmassa itsenäisesti, tekemään suunnitelmia, muistamaan tärkeitä yksityiskohtia ja tavoittelemaan tavoitteita (‡88*, ‡89) paljon vähäisemmällä ihmisten valvonnalla tai avustuksella. Esimerkiksi Manus AI on suosittu AI-agentti, joka pystyy automatisoimaan erilaisia tehtäviä, kuten verkkohakua, ohjelmistokehitystä ja verkkokauppoja (‡90). Kuva 1.3 havainnollistaa yksinkertaisen esimerkin AI-agentista, joka koostuu yleiskäyttöisestä AI-mallista ‘brain’, ja joka voi iteroiden suunnitella, päättellä ja käyttää työkaluja muistiin, verkkoselailuun ja tietokoneen käyttöön.

AI-agenttien digitaalinen infrastruktuuri laajenee (‡91), ja niistä on tullut yhä yleisempiä eri toimialoilla (‡92, ‡93, ‡94). AI-agenteille on kehitetty ratkaisuja muun muassa tutkimustehtäviin (‡37), ohjelmistokehitykseen (‡95), robottien ohjaukseen (‡96) ja asiakaspalveluun (‡97). Jatkuva tutkimus- ja kehitystyö on johtanut siihen, että AI-agentit tai monen agentin järjestelmät ovat koko ajan kyvykkäämpiä ja yhä autonomisempia. Tutkijat ovat arvioineet, että sellaisten ohjelmiston vertailutehtävien monimutkaisuus, joihin AI-agentit pystyvät, kaksinkertaistuu likimain joka seitsemäs kuukausi (katso myös §1.2. Nykyiset kyvykkyydet) (‡98). Asiantuntijat väittävät, että yhä kyvykkäämmät AI-agentit synnyttävät sekä merkittäviä mahdollisuuksia että riskejä (‡99, ‡100*) (katso §2.2.1. Luotettavuushaasteet).

###@ Todisteiden puutteet

Tärkeimmät näyttöä koskevat aukot yleiskäyttöisen tekoälyjärjestelmän kehitysprosessissa johtuvat siitä, että julkisesti saatavilla olevaa tietoa on niukasti siitä, miten niitä kehitetään. Jotkut kehittäjät ovat erittäin läpinäkyviä sen suhteen, miten ne kehittävät yleiskäyttöisiä tekoälyjärjestelmiä (‡1, ‡101). Yleisesti ottaen kuitenkin julkisten ja poliittisten päättäjien tietämys siitä, miten useimmat kehittyneet mallit kehitetään, suojataan, arvioidaan ja otetaan käyttöön, on rajallista. Tämä pitää erityisen hyvin paikkansa sellaisista yritysten sisäisesti käyttöönotetuista tekoälyjärjestelmistä, joita käytetään tekoälyyrityksissä mutta joita ulkopuoliset sidosryhmät eivät käytä tai ymmärrä (‡102, ‡103). Tämä vähäinen ulkoinen näkyvyys aiheuttaa haasteita läpinäkyvyydelle ja valvonnalle. Useat tutkijat ovat tuoneet esiin koulutusaineistoihin (‡104, ‡105, ‡106), yleiskäyttöisiin tekoälymalleihin (‡107, ‡108), tekoälyagentteihin (‡92), arviointeihin (‡109), kehityspolkuihin (‡110) ja turvallisuuteen (‡111) liittyvän rajallisen ja epäjohdonmukaisen läpinäkyvyyden. Rajoitukset ulkoiseen tiedonantoon ovat joskus tarpeen yritysten liikesalaisuuksien ja immateriaalioikeuksien suojaamiseksi. Samanaikaisesti vähäinen läpinäkyvyys vaikeuttaa riippumattomien tutkijoiden ja poliittisten päättäjien mahdollisuuksia tutkia yleiskäyttöisiä tekoälymalleja ja -järjestelmiä.


