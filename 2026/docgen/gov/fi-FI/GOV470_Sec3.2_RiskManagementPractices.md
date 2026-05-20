##########
>white|orangered|left|14|30|hr Luku 3.2
### 3.2. Riskienhallintakäytännöt
>white|orangered|left|24|30|hb Riskienhallintakäytännöt

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Tärkeimmät tiedot
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Yleistarkoitukseen tarkoitetun tekoälyn riskienhallinta sisältää joukon käytäntöjä, joilla tunnistetaan, arvioidaan ja vähennetään yleiskäyttöisen tekoälyn aiheuttamia riskejä. Näihin kuuluvat mallitasoinen testaus ja arviointi (kuten “red-teaming”), organisaatiotason prosessit, jotka ohjaavat kehitys- ja julkaisupäätöksiä, ehdolliset suojatoimet (kuten “if-then”-sitoumukset) sekä tapausraportointi.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Useat AI-kehittäjät ovat tuottaneet Frontier AI Safety -kehyksiä. Nämä kehykset sisältävät tietoa riskinarvioinneista ja määrittelevät ehdollisia toimenpiteitä, kuten pääsynrajoituksia, joita yritykset suunnittelevat toteuttavansa tehokkaammille malleille. Ne vaihtelevat sen mukaan, millaisia riskejä ne kattavat, miten ne määrittelevät kyvykkyyskynnysarvot ja millaisia toimia käynnistyy, kun kynnykset saavutetaan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Näyttö tekoälyn riskienhallintakäytäntöjen tosielämän vaikuttavuudesta on edelleen rajallista. Tapahtumista raportoimisen ja seurannan puute vaikeuttaa sen arviointia, kuinka hyvin nykyiset käytännöt vähentävät riskejä, tai kuinka johdonmukaisesti niitä toteutetaan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Viimeisimmän Raportin (tammikuu 2025) julkaisemisen jälkeen riskienhallinta on muuttunut jäsennellymmäksi uusien toimiala- ja hallinnointialoitteiden myötä. Uudet välineet, kuten EU:n yleiskäyttöistä tekoälyä koskeva käytännesääntö (General-Purpose AI Code of Practice), Kiinan tekoälyn turvallisuusjohtamisen kehikko 2.0 ja G7-maiden Hiroshiman tekoälyprosesseista raportoinnin kehikko, yhdessä yritysvetoisten aloitteiden kanssa, osoittavat suuntauksen kohti yhtenäisempiä toimintatapoja läpinäkyvyyden, arvioinnin ja tapausten raportoinnin osalta.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Markkinadynamiikka ja tekoälyn kehitysvauhti asettavat lisähaasteita. Kilpailupaineiden vuoksi tekoälyyritykset saattavat joutua tekemään valintoja nopeampien tuontijulkaisujen ja riskien vähentämiseen tehtävien investointien välillä. Monet tekoälyyn liittyvät haitat ulkoistetaan myös, ja niihin liittyvä oikeudellinen vastuu on edelleen epäselvä, ja hallinnointiprosessit voivat olla hitaita mukautumaan tekoälyympäristön muutoksiin.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Keskeisiä haasteita poliittisille päättäjille ovat muun muassa yleiskäyttöisen tekoälyn aiheuttamien moninaisten riskien priorisointi sekä sen selventäminen, mitkä toimijat tekoälyn arvoketjun eri vaiheissa ovat parhaiten asemassa niiden lieventämiseksi. Nämä haasteet korostuvat entisestään, koska käytännössä on rajallisesti näkyvyyttä siihen, miten riskejä tunnistetaan, arvioidaan ja hallitaan, sekä koska tietojen jakaminen on pirstoutunutta kehittäjien, käyttöönottajien ja infrastruktuuritoimittajien välillä.
>oldlace|black||11|15|br      


AI:n riskienhallinta käsittää joukon käytäntöjä, joiden tavoitteena on tunnistaa, arvioida ja vähentää AI-järjestelmiin liittyvien riskien todennäköisyyttä ja vakavuutta. Näitä käytäntöjä voivat toteuttaa AI-kehittäjät, käyttöönoton tekijät, arvioijat ja sääntelijät. Esimerkkejä ovat uhkamallinnus, riskiluokittelu, red-teaming, auditoinnit ja tapausraportointi. Tässä osiossa kuvataan nykyisiä riskienhallintakäytäntöjä, uusia kehityssuuntia ja jäljellä olevia rajoitteita.

Vuodesta 2025 alkaen on kehitetty useita uusia kansainvälisiä aloitteita yleiskäyttöisen tekoälyn riskienhallinnan tueksi, mukaan lukien organisaatiotason läpinäkyvyyttä ja riskiraportointia koskevat viitekehykset sekä sääntely- ja hallintoviitekehykset.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Kuva 3.4: Neljä riskienhallinnan komponenttia
>white|black||9|11|br Neljän yleiskäyttöisen tekoälyn riskienhallintamenetelmien kategoriaa: riskin tunnistaminen; riskin analysointi ja arviointi; riskin lieventäminen; ja riskien hallinnointi. Nämä muodostavat iteratiivisen ja syklisen prosessin. Keskellä esitetty riskien hallinnointi mahdollistaa muiden osien onnistumisen. Lähde: International AI Safety Report 2026.


Jäljellä olevia haasteita ovat muun muassa rajallinen standardointi, mikä vaikeuttaa vaatimustenmukaisuuden ja arvioinnin toteuttamista, sekä rajallinen näyttö siitä, kuinka tehokkaita nämä ratkaisut ovat tosielämässä. Lisäksi instituutio-, kulttuuri- ja poliittiset kontekstit vaihtelevat maailmanlaajuisesti, mikä tarkoittaa, että riskien tunnistamista ja hallintaa koskevat lähestymistavat, mukaan lukien hyväksyttävän riskitason kynnykset, voivat vaihdella eri alueilla. Tämän luvun käsittely riskienhallintalähestymistavoista on kuvailevaa: sen tarkoituksena on tiedottaa tekoälyekosysteemin toimijoille nykyisistä maailmanlaajuisista riskienhallinnan käytännöistä. Kun sellaista on saatavilla, käsitellään näyttöä näiden lähestymistapojen tehokkuudesta ja rajoituksista, mutta politiikkasuositukset eivät kuulu tämän työn piiriin.

###@ Riskienhallinnan osatekijät

Riskienhallinta on iteratiivinen prosessi, jossa on käytäntöjä ja menetelmiä, jotka ulottuvat koko AI:n kehittämis- ja käyttöönottojatsin ylle, mutta toimivat yhdessä johdonmukaisesti (‡969). Yleiskäyttöisen AI:n riskienhallinta voi sisältää rooleja laajalle joukolle toimijoita, kuten datatieteilijöitä, mallininsinöörejä, auditoijia, alan asiantuntijoita, johtoa, loppukäyttäjiä, vaikutuksen alaisia yhteisöjä, kolmansien osapuolten toimittajia, poliittisia päättäjiä, hallituksia, standardointiorganisaatioita ja kansalaisyhteiskunnan organisaatioita (‡970, ‡971, ‡972). Johtavat riskienhallinnan standardit ovat usein yhteentoimivia, mutta käyttävät eri terminologiaa kuvaamaan riskienhallinnan elementtejä (‡973, ‡974). Niissä on tyypillisesti neljä toisiinsa kytkeytyvää osaa (Kuva 3.4): riskien tunnistaminen; riskien analysointi ja arviointi; riskien lieventäminen; sekä riskien hallinnointi (‡970, ‡973, ‡975, ‡976). Alla olevat taulukot tarjoavat havainnollistavia esimerkkejä relevanteista menetelmistä, tekniikoista ja työkaluista. Käytännöt kehittyvät edelleen, joten taulukot eivät ole tyhjentäviä, ja sovellettavuus vaihtelee tilanteen mukaan.

###@ Riskien tunnistaminen

Riskien tunnistaminen on prosessi, jossa etsitään, tunnistetaan ja kuvataan riskejä. Kattava riskien tunnistaminen käsittää tyypillisesti kyvykkyyslähtöisiä arvioita, joissa testataan, onko malleilla tiettyjä vaarallisia kyvykkyyksiä (‡977), sekä riskimallinnusta (‡978) ja ennustamista (‡715*), joita käytetään tutkimaan olemassa olevia ja esiin tulevia riskejä. Taulukko 3.1 esittää erilaisia esimerkkejä riskien tunnistamisen käytännöistä. Riskien tunnistaminen hyödyntää myös vuorovaikutusta asiaankuuluvien asiantuntijoiden ja yhteisöjen kanssa, jotta ymmärretään laajempi konteksti siitä, miten riskit syntyvät (‡979, ‡980). Mekanismit, kuten bug bounty -ohjelmat, voivat tukea tätä prosessia kannustamalla sellaisten haavoittuvuuksien tunnistamiseen, joita ei aiemmin tunneta (‡981) (Taulukko 3.1). Riskien tunnistamisen keskeinen tavoite on ottaa huomioon sekä hyvin tunnetut ja hyvin ymmärretyt riskit että mahdolliset tulevat riskit, jotka ovat edelleen epävarmoja tai huonosti määriteltyjä (‡982). Tämä on erityisen tärkeää yleiskäyttöiselle tekoälylle, jossa monia riskejä ei välttämättä ole vielä täysin ymmärretty tai havaittavissa (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bounty-bug-ohjelmat
  Bug bounty -ohjelmat tai haavoittuvuuksien ilmoitusohjelmat kannustavat ihmisiä etsimään ja raportoimaan haavoittuvuuksia tekoälyjärjestelmissä. Useat kehittäjät ovat ottaneet käyttöön bug bounty -ohjelmia (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Asiantuntijaneuvonta
  Toimialan asiantuntijat, käyttäjät ja vaikutuksen alaiset yhteisöt tarjoavat näkemyksiä todennäköisistä riskeistä. Osallistuvaan ja inklusiiviseen tekoälyyn on tekeillä uusia ohjeistuksia (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kalanruotokaavio (Ishikawan kaavio)
  Kalanruotokaaviot ovat vakiintuneita juurisyiden analysointityökaluja, ja tutkijat ovat ehdottaneet niiden käyttämistä tekoälyyn liittyvien riskitapahtumien jäsenneltyyn analysointiin (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ennustaminen
  Ennustaminen on prosessi, jossa ennustetaan tulevia tapahtumia tai trendejä aiempien ja nykyisten tietojen analyysin perusteella. Sitä on käytetty vertailemaan eri taloudellisten lopputulosten suhteellista todennäköisyyttä, esimerkiksi edistyneen tekoälyn avulla (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskiluokittelu
  Riskitaksonomiat ovat tapa luokitella ja jäsentää riskejä useiden ulottuvuuksien kautta. On olemassa useita taksonomioita, jotka kuvaavat riskejä yleiskäyttöisestä tekoälystä (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Skenaariosuunnittelu
  Skenaariosuunnittelu edellyttää uskottavien tulevaisuuden skenaarioiden laatimista ja riskien realisoitumisen analysointia. Tätä on käytetty tutkimaan tekoälymallien riskejä ja vaikutuksia (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Uhkien mallintaminen
  Uhkien mallintaminen on prosessi, jossa tunnistetaan uhkia ja haavoittuvuuksia järjestelmään. Monet tekoälykehittäjät korostavat sen käyttöä ennakoidakseen tekoälyjärjestelmien mahdollisia väärinkäyttöskenaarioita (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.1: Riskien tunnistamisen esimerkkejä yleiskäyttöisen tekoälyn riskienhallinnassa
>white|black||9|11|br Esimerkkimenetelmät tekoälyriskien tunnistamiseksi lueteltuina aakkosjärjestyksessä. Menetelmät sisältyivät
on suunniteltu tukemaan riskien tunnistamista monenlaisille riskityypeille, mukaan lukien riskit haitallisesta käytöstä, riskit toimintahäiriöistä ja järjestelmätason riskit. Koska yleiskäyttöisen tekoälyn riskienhallinta on vielä varhaisessa vaiheessa, kaikki menetelmät eivät sovi jokaiseen tekoälykehittäjään tai käyttöönottoon.


>white|orangered|left|14|15.5|bb Uhkien mallintaminen ja riskitaksonomiat ovat merkittäviä riskien tunnistamismenetelmiä.

Kaksi keskeistä menetelmää yleiskäyttöisen tekoälyn aiheuttamien riskien tunnistamiseen ovat uhkamallinnus ja riskiluokitukset. International AI Safety Report 2026 -julkaisussa uhkamallinnus kuvataan jäsenneltynä prosessina, jossa kartoitetaan, miten tekoälyyn liittyvät riskit saattavat toteutua, ja riskiluokitukset tarjoavat luokitteluperustan. Meta, esimerkiksi, käyttää uhkamallinnusharjoituksia ennakoidakseen mahdollisia sen tekoälymallien väärinkäyttöskenaarioita (‡990), ja Anthropic sisällyttää uhkamallinnuksen osaksi ASL-3 Deployment Standard -standardiaan (‡991). Tekoälyn riskien ja vaarojen taksonomiat, jotka luettelevat riskiluokkia ja esimerkkejä, voivat yhtä lailla toimia lähtökohtana yleiskäyttöiseen tekoälyyn liittyvien olennaisten riskien käsitteellistämiselle, tunnistamiselle ja täsmentämiselle tietyillä sovellusalueilla (‡906, ‡988, ‡992, ‡993).

###@ Riskianalyysi ja arviointi

Riskianalyysi ja arviointi on prosessi, jossa määritetään tekoälymallin tai -järjestelmän riskin taso ja verrataan sitä vahvistettuihin kriteereihin, jotta voidaan arvioida hyväksyttävyys tai tarve lieventämistoimiin (‡994, ‡995, ‡996, ‡997). Se sisältää käytäntöjä, kuten mallin suorituskyvyn mittaamisen vertailuarvoissa (‡998) ja arvioinneissa (‡176, ‡715), punatiimiharjoitusten tekemisen (‡999*), vaikutusarvioinnit (‡1000) ja auditoinnit (‡1001, ‡1002). Katso Taulukko 3.2 esimerkkejä yleiskäyttöisen tekoälyn riskianalyysistä ja arvioinnista. Menetelmät on suunniteltu tukemaan analyysiä ja arviointia samanaikaisesti monentyyppisille riskeille.

Riskianalyysin ja arvioinnin keskeisiä tavoitteita ovat mallin kyvykkyyksien ja haavoittuvuuksien arviointien tekeminen (‡1003), hyödyntämällä vankkaa riskimallinnusta päätöksenteon tukemiseksi riskirajoista (‡1004, ‡1005) ja ymmärtämällä, miten tekoälyjärjestelmiä käytetään käytännössä, jotta voidaan arvioida välittömiä yhteiskunnallisia vaikutuksia (‡869, ‡904, ‡905, ‡1006). Riskianalyysi- ja arviointiprosesseja pidetään usein todennäköisempänä riskien tunnistamisessa silloin, kun ne sisältävät riippumattoman arvioinnin (‡1001, ‡1007), nojaavat eri toimialojen asiantuntemukseen (‡1008) ja ottavat mukaan erilaisia näkökulmia useilta aloilta ja tieteenaloilta sekä vaikutuksia kokevilta yhteisöiltä (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Auditoinnit
  Tarkastukset ovat muodollisia arvioita tekoälymallien suorituskyvystä ja vaikutuksista ja/ tai organisaation vaatimustenmukaisuudesta standardien, käytäntöjen ja menettelyjen osalta, ja ne toteutetaan joko organisaation sisäisesti tai ulkopuolisen tahon toimesta. Tekoälyn tarkastusala on kasvava, ja lukuisia työkaluja ja käytäntöjä on olemassa tekoälymallien ja tekoälymallien kehittäjien toimintatapojen tarkastamiseen (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vertailuarvot
  Vertailumittarit ovat standardoituja, usein kvantitatiivisia testejä tai mittareita, joita käytetään arvioimaan ja vertailemaan tekoälyjärjestelmien suorituskykyä kiinteällä joukon tehtäviä, jotka on suunniteltu edustamaan todellista käyttöä (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Jousisidontamenetelmä
  Joutsenensolmumenetelmää (bowtie) on hyvin tunnettu menetelmä havainnollistamaan, mihin ohjauksia voidaan lisätä riskitapahtumien lieventämiseksi. Se tarjoaa selkeän erottelun ennakoivan ja reagoivan riskienhallinnan välillä (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Delphi-menetelmä
  Delphi-menetelmä on ryhmäpäätöksentekotekniikka, joka käyttää sarjaa kyselylomakkeita yksimielisyyden keräämiseen asiantuntijapaneelilta (‡1020, ‡1021). Sitä on käytetty auttamaan mahdollisten tulevaisuuksien tutkimisessa kehittyneen tekoälyn avulla (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kenttätestaus
  Kenttäkokeissa arvioidaan tekoälyjärjestelmän suorituskykyä ja vaikutusta todellisessa, käytännön työympäristössä. Osa tutkimuksesta korostaa kenttäkokeita mallin arvioinnin täydentäjänä todellisten lopputulosten ja seurausten arvioinnissa (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vaikutusten arviointi
  Vaikutusarvioinneilla arvioidaan teknologian tai hankkeen mahdollisia vaikutuksia. Tämä voi sisältää vaikutusten määrällistämisen, yhteenlaskemisen ja priorisoinnin. EU:n tekoälyasetus edellyttää esimerkiksi, että korkean riskin tekoälyjärjestelmien kehittäjät tekevät perusoikeusvaikutusten arviointeja (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mallin arviointi
  Malliarvioinnit sisältävät prosesseja ja testejä, joilla arvioidaan ja mitataan AI-mallin suorituskykyä tietyssä tehtävässä. AI-arviointeja on lukuisia erilaisten kyvykkyyksien ja riskien arvioimiseksi, mukaan lukien turvallisuus, tietoturva ja sosiaalinen vaikutus (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Todennäköisyyspohjainen riskinarviointi
  Todennäköisyyspohjainen riskinarviointi on menetelmä, jolla arvioidaan monimutkaisiin järjestelmiin tai prosesseihin liittyviä riskejä ja joka ottaa huomioon epävarmuuden. Sitä on sovellettu edistyneisiin tekoälyjärjestelmiin (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-team-menetelmä
  Red-teaming on harjoitus, jossa ryhmä ihmisiä tai automatisoituja järjestelmiä teeskentelee olevansa hyökkääjä ja hyökkää organisaation teknisiin järjestelmiin haavoittuvuuksien tunnistamiseksi. Useilla AI-yrityksillä on sisäisiä käytäntöjä AI-järjestelmien red-teamingia varten (‡458, ‡1028). Red-teamingia voivat myös toteuttaa yritysten ulkopuoliset toimijat. Nämä tiimit kohtaavat haasteita, kuten rajallisen pääsyn, mutta ne voivat myös tuoda esiin erillisiä oivalluksia (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskimatriisit
  Riskimatriisit ovat visuaalinen työkalu, joka auttaa priorisoimaan riskejä niiden todennäköisen esiintymisen ja mahdollisen vaikutuksen perusteella (‡1027). Jotkin tekoälykehittäjät sisällyttävät perusmuotoisia riskimatriiseja Frontier AI Safety -turvallisuuskehyksiinsä (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskikynnykset/ riskiluokat
  Riskirajat tai -tasot ovat määrällisiä tai laadullisia raja-arvoja, jotka erottavat hyväksyttävät riskit ei-hyväksyttävistä riskeistä ja käynnistävät tiettyjä riskinhallintatoimia, kun niitä ylitetään. Yleiskäyttöiselle tekoälylle ne määritetään kyvykkyyksien, vaikutusten, laskennan (compute), leviämisen (reach) ja muiden tekijöiden yhdistelmällä (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskinsietokyky
  Riskinsietokyky tarkoittaa riskin tasoa, jonka organisaatio on valmis hyväksymään. Tekoälyssä riskinsietokyky asetetaan usein implisiittisesti yrityksen käytäntöjen ja toimintatapojen kautta, kun taas tietyissä sääntelyjärjestelmissä määritellään nimenomaisesti hyväksymättömät riskit ja liitetään niihin laillisia seuraamuksia (‡1032). Jotkin yritykset kuvaavat riskinsietokykyään uuden mallin marginaalisen riskin näkökulmasta; eli siinä määrin, missä uusi malli kontrafaktuaalisesti lisää riskiä jo olemassa oleviin malleihin tai muihin teknologioihin verrattuna (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Turvallisuustapaukset
  Turvallisuustapaus on jäsennelty argumentti, jota tukee näyttö ja jonka perusteella järjestelmä on hyväksyttävän turvallinen käyttää tietyssä toimintaympäristössä. Viimeaikaisessa kirjallisuudessa (‡1037, ‡1038, ‡1039) on tutkittu turvallisuustapauksia edistyneille AI-järjestelmille, ja tietyt Frontier AI Safety Framework -viitekehykset viittaavat niihin (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Järjestelmän turvallisuusanalyysi
  Järjestelmän turvallisuusanalyysi korostaa riippuvuuksia komponenttien ja niiden osana olevan järjestelmän välillä, jotta voidaan ennakoida, miten järjestelmätason vaarat voivat syntyä komponentti- tai prosessivirheistä tai alijärjestelmien välisistä vuorovaikutuksista, ihmistekijöistä ja ympäristöolosuhteista. AI-järjestelmiin sovellettuja lähestymistapoja kirjallisuudessa ovat järjestelmälähtöinen prosessianalyysi (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.2: Riskianalyysi-/arviointi yleiskäyttöisen tekoälyn riskienhallinnassa
>white|black||9|11|br Esimerkkimenetelmiä tekoälyriskien analysointiin/arviointiin, lueteltuna aakkosjärjestyksessä. Koska yleiskäyttöisen tekoälyn riskienhallinta on vasta kehittymässä, kaikki menetelmät eivät sovellu jokaiseen tekoälyn kehittäjään tai käyttöönottoorganisaatioon.


>white|orangered|left|14|15.5|bb Yleisiä riskianalyysityökaluja ovat vertailumittarit ja malliarvioinnit

Vertailuarvot ja malliarvioinnit ovat standardoituja testejä, joilla arvioidaan yleiskäyttöisten tekoälyjärjestelmien suorituskykyä tietyissä tehtävissä. Tutkijat ovat kehittäneet laajan valikoiman vertailuarvoja ja arviointeja, mukaan lukien joukot haastavia monivalintakysymyksiä, ohjelmistokehitysongelmia sekä työhön liittyviä tehtäviä simuloiduissa toimistoympäristöissä (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Haitallisia kyvykkyysarviointeja (‡715) käytetään arvioimaan, onko yleiskäyttöisellä tekoälymallilla tai -järjestelmällä erityisen vaarallista tietoa tai taitoja, kuten kykyä auttaa kyberhyökkäyksissä (katso §2.1.3. Kyberhyökkäykset).

Yritysten ja hallitusten erittäin merkitykselliset päätökset mallien julkaisuihin liittyen tukeutuvat osittain näihin arviointeihin (‡1050, ‡1051, ‡1052). Kuitenkin vertailuarvioinnit vaihtelevat huomattavasti laadultaan ja laajuudeltaan (‡998, ‡1003), ja niiden pätevyyttä voi olla vaikea arvioida lukuisien puutteiden vuoksi vertailukäytäntöihin liittyen (‡902, ‡909, ‡1003, ‡1053*). Esimerkiksi vertailuarvioinnit voivat muuttua ”kylläisiksi” – kun monien mallien pisteet lähestyvät ylintä pistemäärää – mikä tarkoittaa, etteivät ne enää erottele malleja selvästi toisistaan. Mallit ovat myös yhä todennäköisemmin kykeneviä tunnistamaan tietyt tehtävät arvioinneiksi ja näyttämään erilaisia käyttäytymismalleja kuin vastaavissa tehtävissä käyttöönoton yhteydessä niin sanotun ”tilannetietoisuuden” vuoksi (katso §2.2.2. Hallinnan menettäminen). Lopuksi vertailuarvioinneilla ja arvioinneilla on hyvin dokumentoidut rajoitukset: ne eivät erityisesti pysty kuvaamaan yleiskäyttöisen tekoälyn käytöstä uusissa ympäristöissä ja uusissa tehtävissä aiheutuvia riskejä, koska testiehtojen ja todellisen käytön välinen ero vaihtelee eri määrin (‡913) (katso §1.2. Nykyiset kyvykkyydet ja §3.1. Teknisiä ja institutionaalisia haasteita).

>white|orangered|left|14|15.5|bb Red-teaming mahdollistaa yksityiskohtaisemmat, toimialakohtaiset riskinarvioinnit

Toinen yleinen tapa arvioida riskejä on red-teaming. 'Red team' on arvioijien ryhmä, jonka tehtävänä on etsiä haavoittuvuuksia, rajoituksia tai väärinkäytön mahdollisuuksia. Red-teaming voi olla toimialakohtaista ja suorittaa toimialan asiantuntijat, tai se voi olla avoin tutkimaan uusia riskitekijöitä. Esimerkiksi red team saattaa tutkia 'jailbreaking'-hyökkäyksiä, jotka ohittavat mallin turvallisuusrajoitukset (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Toisin kuin vertailut (benchmarks), red-teamingin keskeinen etu on, että red teamit voivat mukauttaa arviointinsa testattavaan järjestelmään. Esimerkiksi red teamit voivat suunnitella mukautettuja syötteitä tunnistaakseen pahimmat mahdolliset toimintatavat, haitallisen käytön mahdollisuudet ja odottamattomat virheet. Toisaalta se voi edellyttää erityiskäyttöoikeuksia malleihin, ja se voi jäädä huomaamatta tärkeiltä riski-luokilta (‡999, ‡1028).

Tärkeää on, että tunnistettujen riskien puuttuminen ei tarkoita, että kyseiset riskit olisivat vähäisiä: aiempi työ osoittaa, että viat usein jäävät havaitsematta, erityisesti silloin kun hyökkäystiimeillä (red team) on rajallinen pääsy tai resurssit (‡1060). Tutkimuksissa on lisäksi kyseenalaistettu, voiko hyökkäystiimityö (red-teaming) tuottaa luotettavia ja toistettavia tuloksia (‡1061). Hyökkäystiimin kokoonpano ja hyökkäystiimiläisille annetut ohjeet (‡1062), hyökkäyskierrosten määrä (‡1063) sekä mallin pääsy työkaluihin (‡1064, ‡1065) voivat vaikuttaa merkittävästi lopputuloksiin, mukaan lukien se, millä riskialueella on katetta. Kattavat ohjeistukset hyökkäystiimityöhön (red-teaming) pyrkivät vastaamaan joihinkin näistä haasteista (‡1066).

###@ Riskienhallinta

Riskien lieventäminen on prosessi, jossa priorisoidaan, arvioidaan ja otetaan käyttöön hallintakeinoja ja vastatoimia tunnistettujen riskien pienentämiseksi. Esimerkkejä ovat pääsynhallinta (‡991), jatkuva seuranta (‡986) ja if-then-sitoumukset (‡700). Riskin lieventäminen nostaa esiin keskeisen kysymyksen: mikä on hyväksyttävä riskitaso? Viimeaikaiset viitekehykset ja yritysten käytännöt ovat alkaneet muodollistaa ”riskin hyväksymisen” kriteerejä (‡965, ‡1040). Asianmukaisten kynnysarvojen määrittäminen on kuitenkin edelleen haastavaa erityisesti riskien osalta, joilla on laaja-alaisia yhteiskunnallisia vaikutuksia (‡986, ‡1067). Vakiintunutta mekanismia ei ole tällä hetkellä olemassa sen varmistamiseksi, että kehittäjien ennen julkaisua tekemät riskin hyväksymispäätökset ovat oikein (‡1005).

Alla olevassa Taulukko 3.3 kuvatut riskienhallintamenetelmät ovat mukautettavia ja voivat lieventää useita riskejä, mukaan lukien joitakin odottamattomia riskejä. Taulukko ei sisällä teknisiä lieventämismenetelmiä, kuten vastakkaisten esimerkkien koulutusta, sisällönsuodattimia ja ketjupäättelyn (chain-of-thought) valvontaa. Nämä käsitellään kohdassa §3.3. Tekniset suojatoimet ja valvonta sekä koko raportissa kunkin riskin kohdalla kohdassa §2. Riskit, osioissa ”Mitigations”.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hyväksyttävän käytön käytännöt
  Hyväksyttävän käytön käytäntö on joukko sääntöjä ja ohjeita tekoälymallien vastuulliseen, eettiseen ja lailliseen käyttöön. On yleistä, että tekoälykehittäjät julkaisevat hyväksyttävän käytön käytäntöjä sekä kielletyn käytön käytäntöjä uusien mallijulkaisujen yhteydessä (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pääsynhallinta/käyttäjän hyväksynnän tarkastus
  Pääsynhallinta sisältää politiikkojen ja sääntöjen käytön rajoittamaan pääsyä AI-malleihin, dataan ja järjestelmiin käyttäjäroolien, attribuuttien ja muiden ehtojen perusteella, jotta voidaan estää luvaton käyttö, manipulointi tai tietomurrot. AI-yritykset poistavat usein tilit, joiden havaitaan harjoittavan rikollista toimintaa (‡486), ja sisällyttävät käyttäjien taustaselvitykset sekä Know-Your-Customer -tarkastukset varmistaakseen, että malleja käyttävät vain luotetut toimijat (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Käytös-/mallimääritys
  AI-käytöksen määrittely on dokumentti, joka määrittelee, miten AI-mallin tulisi käyttäytyä erilaisissa tilanteissa. Se toimii pohjana AI:n yhdenmukaistamiselle ja turvallisuudelle ja ohjaa mallin kehittämistä, koulutusta, arviointia sekä tuotosvaihetta. Useat AI-yritykset käyttävät mallin määrittelydokumentteja ja tekevät vähintään osan niistä julkisiksi (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Jatkuva seuranta
  Jatkuva seuranta on käytössä olevien tekoälyjärjestelmien jatkuva, automatisoitu prosessi, jossa havainnoidaan, analysoidaan ja ohjataan järjestelmiä. Seuraa suorituskykyä ja rajoita niiden toimintaa varmistaaksesi luotettavuuden, tehokkuuden ja turvallisuuden. Jatkuvaan seurantaan on saatavilla lukuisia työkaluja (‡1073*) sekä tekniikoita tukemaan
AI-havainnoitavuus (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Puolustuksen syvyyteen perustuva lähestymistapa
  Puolustus syvyyteen on ajatus siitä, että useita riippumattomia ja toisiaan täydentäviä puolustuskerroksia voidaan ottaa käyttöön niin, että jos yksi epäonnistuu, muut ovat silti tehokkaita (‡1075, ‡1076). Useat Frontier AI Safety -viitekehykset viittaavat siihen (esim. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Järjestelmän seuranta
  Tämä on prosessi, jossa seurataan laajempaa tekoälyekosysteemiä, mukaan lukien laskennan ja laitteiston seuranta, mallin alkuperän todennettavuus, datan alkuperän todennettavuus sekä käyttömallit. Tutkimuskirjallisuus käsittelee tällaista seurantaa suhteessa yleiskäyttöisen tekoälyn aiheuttamiin riskeihin (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Jos-sitovat sitoumukset
  Ehto–seuraamus-sitoumukset ovat joukko teknisiä ja organisatorisia menettelyjä sekä sitoumuksia, joiden avulla hallitaan riskejä, kun tekoälymallit muuttuvat yhä kykenevimmiksi. Useat tekoälyn kehittäjät käyttävät tällaisia sitoumuksia osana Frontier AI Safety Frameworks -kehyksiään (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Punaiset viivat tai kiellot
  Punaiset viivat ovat tiettyjä rajoja, jotka ilmaistaan kyvykkyyksinä, vaikutuksina tai käyttötapoina. Käsitettä esiintyy julkisissa kannanotoissa ja aloitteissa sekä sääntelyyn liittyvissä kieltomääräyksissä (‡1079, ‡1080, ‡1081). Kirjallisuudessa tuodaan myös esiin punaisen viivan lähestymistapojen rajoituksia, mukaan lukien haasteet liittyen yksimielisyyteen ja täytäntöönpanokelpoisuuteen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Julkaisu- ja käyttöönotto-strategiat
  Yleiskäyttöisen tekoälyn julkaisu- ja käyttöönottostrategioihin voi kuulua porrastettu julkaiseminen tai API-käyttö, jotta väärinkäytön tai odottamattoman haitan varalta on käytettävissä enemmän lievennysvaihtoehtoja (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.3: Riskien lieventäminen yleiskäyttöisen tekoälyn riskienhallinnassa
>white|black||9|11|br Esimerkkimenetelmät tekoälyn riskien pienentämiseksi on lueteltu aakkosjärjestyksessä. Mukana olevat menetelmät on suunniteltu tukemaan riskien pienentämistä samanaikaisesti monentyyppisissä riskeissä, mukaan lukien haitallisesta käytöstä aiheutuvat riskit, toimintahäiriöihin liittyvät riskit ja systeemiset riskit. Koska yleiskäyttöisen tekoälyn riskienhallinta on vielä alkuvaiheessa, kaikki menetelmät eivät sovellu jokaiseen tekoälyn kehittäjään tai käyttöönotto-organisaatioon.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Kuva 3.5: ’Juustoreikädiagrammi’, joka havainnollistaa puolustuksen kerroksittaisen toteutuksen lähestymistapaa
>white|black||9|11|br Useat puolustuskerrokset voivat korvata yksittäisten kerrosten puutteita. Nykyisissä tekoälyn riskienhallintatekniikoissa on puutteita, mutta niiden kerrostaminen voi tarjota huomattavasti vahvemman suojan riskejä vastaan. Lähde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Puolustus syvyyden periaatteen (defense-in-depth) ja julkaisu- eli release-strategiat ovat tärkeitä lieventämisen työkaluja

Puolustus- syvyydessä -malli voi tukea yleiskäyttöisen tekoälyn riskienhallintaa. Tässä yhteydessä puolustus- syvyydessä -mallilla tarkoitetaan yhdistelmää teknisiä, organisatorisia ja yhteiskunnallisia toimenpiteitä, joita sovelletaan eri kehitys- ja käyttöönoton vaiheissa (Kuva 3.5). Tämä tarkoittaa riippumattomien suojakerrosten luomista, jotta jos yksi kerros epäonnistuu, muut kerrokset voivat silti estää vahingon. Usein siteerattu esimerkki puolustus- syvyydessä -mallista on toimenpidevalikoima, jolla otetaan käyttöön ennaltaehkäiseviä toimenpiteitä tartuntatautien ehkäisemiseksi. Rokotteet, maskit ja käsienpesu, muiden toimenpiteiden ohella, voivat pienentää tartunnan riskiä huomattavasti yhdessä, vaikka mikään näistä menetelmistä ei ole yksinään 100% tehokas (‡1083*). Yleiskäyttöiselle tekoälylle puolustus- syvyydessä sisältää ohjauskeinoja, jotka eivät kohdistu itse tekoälimalliin, vaan laajempaan ekosysteemiin. Tähän sisältyy esimerkiksi ohjauksia niille materiaaleille, joita tarvitaan biologisen hyökkäyksen toteuttamiseen, kuten reagensseille (‡1084, ‡1085). Puolustus- syvyydessä -toimenpiteet käsittelevät kuitenkin ensisijaisesti onnettomuuksiin, toimintahäiriöihin ja haitalliseen käyttöön liittyviä riskejä, ja niillä voi olla pienempi rooli systeemisten riskien hallinnassa (katso §3.5. Yhteiskunnallisen sietokyvyn rakentaminen).

Yrityksen julkaisu- ja käyttöönotto- strategia on tärkeä osa riskienhallintaa. Päätökset siitä, miten mallit saatetaan käyttäjien saataville, voivat olennaisesti vaikuttaa riskialttiuteen (‡1082). Eri julkaisu- ja käyttöönotto-vaihtoehtoja ovat esimerkiksi vaiheittainen julkaisu rajatuille käyttäjäryhmille, pääsy hallittujen verkkopalvelujen kautta (kuten API-rajapintojen kautta) sekä lisenssisopimusten ja hyväksyttävän käytön käytäntöjen käyttö, joilla laillisesti kielletään tietyt haitalliset käyttötavat (‡176, ‡1086, ‡1087). §3.4. Open-weight-mallit käsittelee tarkemmin, miten mallipainojen julkaiseminen vaikuttaa riskeihin.

###@ Riskienhallinnan hallintomalli

Riskienhallinnan hallintotapa on prosessi, jossa riskienhallinnan arvioinnit, päätökset ja toimenpiteet kytketään organisaation tai muun toimijan strategiaan ja tavoitteisiin (‡1088, ‡1089). Taulukko 3.4 antaa yleiskuvan yleisistä riskienhallinnan hallintotavan tekniikoista. Kuten Kuvassa 3.4 on esitetty, riskienhallinnan hallintotapa voidaan ymmärtää riskienhallinnan ytimenä, sillä se mahdollistaa muiden riskienhallinnan osatekijöiden tehokkaan toiminnan. Se tarjoaa vastuunjakoa, läpinäkyvyyttä ja selkeyttä, jotka tukevat perusteltuja riskienhallinnan päätöksiä. Riskienhallinnan hallintotapa voi sisältää käytäntöjä, kuten poikkeamien ilmoittaminen (‡1090), riskivastuiden kohdentaminen (‡965) ja ilmiantajien suojelu (‡1091). Laajemmin riskienhallinnan hallintotapa voi käsittää ohjeistuksia, kehyksiä, lainsäädäntöä, sääntelyä, kansallisia ja kansainvälisiä standardeja sekä koulutus- ja opetusalotteita. Riskienhallinnan hallintotavan keskeinen tarkoitus on luoda organisaation politiikkoja ja mekanismeja, jotka selkeyttävät, miten riskienhallinnan vastuut kohdennetaan koko organisaation tai muun toimijan sisällä, jotta voidaan tukea asianmukaista valvontaa ja vastuullisuutta (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentaatio
  Dokumentointikäytännöt auttavat seuraamaan keskeisiä tietoja tekoälyjärjestelmistä, kuten harjoitustietoja, suunnitteluratkaisuja, käyttötarkoituksia, rajoituksia ja riskejä. ”Mallitietokortit” ja ”järjestelmätietokortit”, jotka tarjoavat tietoa siitä, miten AI-malli tai -järjestelmä on koulutettu ja arvioitu, ovat esimerkkejä tunnetuista tekoälyn dokumentointia koskevista parhaista käytännöistä (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tapahtumaraportointi
  Häiriö- tai poikkeamaraportointi on prosessi, jossa dokumentoidaan järjestelmällisesti ja jaetaan tapauksia, joissa kehittyvä tai käyttöönotettu tekoäly on aiheuttanut suoraa tai epäsuoraa vahinkoa. Useat alustat helpottavat tekoälyn häiriö- tai poikkeamaraportointia (‡1096, ‡1097), ja on myös viitekehyksiä, jotka helpottavat tehokkaampaa tekoälyn häiriö- tai poikkeamaraportointia (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskinhallintakehykset
  Riskienhallintakehykset ovat organisaatiotason suunnitelmia, joilla vähennetään puutteita riskien kattavuudessa, koordinoidaan erilaisia riskienhallinnan toimintoja ja otetaan käyttöön tarkastukset ja vastapainot. Yleisluonteiselle tekoälylle (‡986, ‡1098) erityiset kehykset viittaavat usein tässä jaksossa mainittuihin muihin toimenpiteisiin.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskirekisteri
  Riskirekisteri on eri riskien, niiden priorisoinnin, vastuuhenkilöiden ja lieventämissuunnitelmien kokoelma. Näitä esiintyy suhteellisen yleisesti monilla toimialoilla, mukaan lukien kyberturvallisuus (‡1099), ja niitä käytetään toisinaan sääntelynmukaisuuden vaatimusten täyttämiseen.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Riskin vastuunjako
  Roolien ja vastuiden kohdentaminen riskienhallinnassa organisaation sisällä voi jäsentää sisäistä valvontaa päätöksenteossa (‡1002, ‡1093). Tällaiset järjestelyt heijastuvat joissakin hallintokehikoissa, mukaan lukien EU:n yleiskäyttöisen tekoälyn käytäntökoodi (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Läpinäkyvyysraportit
  Läpinäkyvyysraportit kuvaavat tekoälyyrityksen riskienhallintakäytäntöjä julkistamalla tiettyjä tietoja tai jakamalla dokumentaatiota alan järjestöjen tai valtion elinten kanssa. Esimerkiksi monet tekoälyyritykset toimittavat Hiroshima AI Process (HAIP) -läpinäkyvyysraportteja (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ilmoittajansuojelu
  Koska suuri osa tekoälyn kehityksestä tapahtuu suljettujen ovien takana, joihinkin hallintokehyksiin sisältyy ilmoittajansuojelutoimia, jotta mahdollisista riskeistä voidaan ilmoittaa viranomaisille (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.4: Riskienhallinnan hallinnointi yleiskäyttöisen tekoälyn riskienhallinnassa
>white|black||9|11|br Esimerkkimenetelmät tekoälyriskien hallinnoinnin toteuttamiseksi on lueteltu aakkosjärjestyksessä. Menetelmät on tarkoitettu tukemaan riskien hallinnointia samanaikaisesti monentyyppisissä riskeissä, mukaan lukien haitallisesta käytöstä aiheutuvat riskit, toimintavikojen riskit ja järjestelmätason riskit. Koska yleiskäyttöisen tekoälyn riskienhallinta on vielä alkuvaiheessa, kaikki menetelmät eivät sovellu jokaiseen tekoälyn kehittäjään tai käyttöönotonomistajaan.


>white|orangered|left|14|15.5|bb Dokumentointi ja läpinäkyvyys ovat osa riskienhallintaa.

Dokumentaation ja institutionaalisen läpinäkyvyyden mekanismit sekä tiedonjakokäytännöt helpottavat ulkoista tarkastelua ja tukevat pyrkimyksiä hallita yleiskäyttöiseen tekoälyyn (‡1101, ‡1102) liittyviä riskejä. On tullut yleiseksi käytännöksi julkaista tuotantoa edeltävien testien tulokset ”model card” -mallikortissa tai ”system card” -järjestelmäkortissa yhdessä perustietojen kanssa mallista tai järjestelmästä, mukaan lukien se, miten se on koulutettu, ja mitkä sen mahdolliset rajoitteet ovat (‡1094, ‡1095). Jotkin kehittäjät julkaisevat myös läpinäkyvyysraportteja, jotka sisältävät yksityiskohtia riskienhallintakäytännöistä laajemmin (‡1103). Muita dokumentaation ja läpinäkyvyyden osatekijöitä ovat seuranta ja tapausten raportointi (‡176, ‡1083*, ‡1103) sekä tiedon jakaminen, jota voivat helpottaa kolmannet osapuolet, kuten Frontier Model Forum. Joissakin sääntelykehyksissä, kuten EU:n tekoälysäädöksessä tai Kalifornian Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), edellytetään tietyissä tapauksissa tietojen jakamista yleiskäyttöiseen tekoälyyn liittyvistä riskeistä.

>white|orangered|left|14|15.5|bb Johtajuuden sitoutuminen ja kannustimet muokkaavat riskienhallinnan käytäntöjä

Organisaatiokulttuuri, johtamisrakenne ja kannustimet vaikuttavat riskienhallinnan pyrkimyksiin monin eri tavoin (‡1105). Johtajien sitoutuminen ja kannustinjärjestelyt ovat usein olennaisia sen kannalta, miten riskienhallintapolitiikat toimivat käytännössä. Joillakin kehittäjillä on sisäisiä päätöksentekopaneeleja, jotka pohtivat, miten uusia tekoälyjärjestelmiä suunnitellaan, kehitetään ja arvioidaan turvallisesti ja vastuullisesti. Valvonta- ja neuvoa-antavat toimikunnat, luottamusrakenteet tai tekoälyn eettiset toimielimet voivat myös toimia mekanismeina riskienhallinnan ohjaukselle ja organisaation valvonnalle (‡1092*, ‡1106, ‡1107, ‡1108). Tutkijat ovat väittäneet, että vapaaehtoiseen itsehallintaan liittyvät haasteet tarkoittavat, että kolmannen osapuolen auditointi, todentaminen ja standardointi voisivat auttaa vahvistamaan yleiskäyttöisen tekoälyn riskienhallintaa (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Organisaation riskienhallinta, läpinäkyvyys ja riskiraportointikehykset

Useita uusia aloitteita keskittyy riskienhallintaprosesseihin, dokumentointiin ja läpinäkyvyyteen. Nykyisessä muodossaan EU:n yleiskäyttöisen tekoälyn käytäntöohje (Code of Practice) toimii vapaaehtoisena kehyksenä, joka ohjaa läpinäkyvyyttä, tekijänoikeuksia sekä turvallisuus- ja tietoturvakäytäntöjä tukemaan EU:n tekoälyasetuksen (AI Act) yleiskäyttöistä tekoälyä koskevien säännösten noudattamista (‡965). Joulukuusta 2025 alkaen yli kaksi tusinaa yritystä† on allekirjoittanut sopimuksen. G7 Hiroshima AI Processin (HAIP) raportointikehys (‡1100) on ensimmäinen kansainvälinen kehys vapaaehtoiseen julkiseen raportointiin organisaatioiden riskienhallintakäytännöistä kehittyneille tekoälyjärjestelmille. Ainakin 20 kehittäjää on julkaissut julkisia läpinäkyvyysraportteja, jotka kattavat riskien tunnistamisen, arviointimittarit, lieventämisstrategiat sekä datan tietoturvamenettelyt.

AI-kehittäjät ovat ottaneet käyttöön vapaaehtoisia läpinäkyvyyssitoumuksia. Kiinassa 17 kiinalaisen tekoälyyrityksen lupaukset, joita koordinoi Kiinan AI Industry Alliance, julkaistiin joulukuussa 2024 (‡1113) ja niitä päivitettiin vuonna 2025 (‡1114). Etelä-Koreassa 16. AI Seoul Summit -tapahtumassa toukokuussa 2024 16 tekoälykehittäjää useista eri maista allekirjoitti vapaaehtoisia sitoumuksia julkaista Frontier AI Safety Frameworks -puitteet kyvykkäimmille malleilleen ja järjestelmilleen sekä ottaa käyttöön riskienhallintakäytännöt mallikehityksen ja käyttöönoton vaiheissa (‡1052).

    Huom † -- Allekirjoittajat 12/2025 alkaen sisältävät: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing ja WRITER.

>white|orangered|left|14|15.5|bb Frontier AI -turvallisuuskehykset ovat nousseet merkittäväksi organisaatiotason lähestymistavaksi AI-riskien hallinnassa

Vuodesta 2023 lähtien useat johtavat tekoälyn kehittäjät ovat julkaisseet vapaaehtoisesti asiakirjoja, joissa ne kuvaavat, miten ne aikovat tunnistaa ja vastata vakaviin riskeihin kehittyneimmistä järjestelmistään. Nämä Frontier AI Safety Frameworks -kehykset kuvaavat, miten tekoälyn kehittäjä aikoo arvioida, valvoa ja hallita kehittyneimpiä tekoälymallejaan ja -järjestelmiään ennen käyttöönottoa ja sen aikana. Nämä kehykset ovat monilta osin samankaltaisia, mutta eroavat keskeisiltä osin (‡1115, ‡1116). Useimmat keskittyvät kemiallisten, biologisten, säteily- ja ydinhyökkäysten (CBRN) aiheuttamiin uhkiin, kehittyneisiin kyberturvallisuuskyvykkyyksiin sekä kehittyneeseen autonomiseen toimintaan (‡1115, ‡1117). Pieni osa kehyksistä käsittelee lisäksi muita riskialueita, kuten lainvastaista syrjintää mittakaavassa ja lapsiin kohdistuvaa seksuaalista hyväksikäyttöä.

Useat kehittäjät päivittivät kehyksiään vuonna 2025, ja lisäsivät uusia osioita haitallisesta manipuloinnista, virheellisestä kohdistumisesta aiheutuvasta riskistä sekä autonomisesta replikaatiosta ja adaptoitumisesta (‡1078, ‡1118). Vaikka monet kehykset kuvaavat samankaltaisia riskienhallintaa koskevia lähestymistapoja – mukaan lukien uhkamallinnus, red-teaming ja vaarallisten kyvykkyyksien arvioinnit – ne vaihtelevat riskitasojen ja kynnysten määritelmissään, arviointien tiheydessä, puskureissa arviointien ja kynnysten välillä sekä lieventämissitoumustensa kattavuudessa (esimerkiksi sisältyykö mallin painojen poistaminen vai vain kehityksen keskeyttäminen) (‡1115, ‡1119). Lisätietoja on Taulukko 3.5:ssä.

>white|orangered|left|14|15.5|bb Monet toimet Frontier AI Safety Frameworks -kehyksissä perustuvat siihen, toteutetaanko ne jos-niin-sitoumusten pohjalta.

Keskeinen osa Frontier AI Safety Frameworks -kehyksiä ovat "if-then sitoumukset" (jos–niin). Ne ovat ehdollisia toimintamalleja, jotka käynnistävät tiettyjä vasteita, kun tekoälymallit ja -järjestelmät saavuttavat ennalta määritetyt kyvykkyyskynnysarvot (‡1120). Esimerkiksi jos–niin-sitoumus voi määrittää, että jos mallin havaitaan kykenevän merkityksellisesti avustamaan aloittelijoita CBRN-aseiden luomisessa ja käyttöönotossa, kehittäjä toteuttaa tehostettuja turvatoimia, käyttöönoton ohjausmekanismeja ja reaaliaikaista valvontaa (‡991*).

Vuonna 2025 useat AI-kehittäjät ilmoittivat, että uudet mallit käynnistivät varhaisia varoitushälytyksiä, tai etteivät he pystyneet sulkemaan pois mahdollisuutta, että lisäarviointi osoittaisi mallien ylittäneen kyvykkyyskynnysarvot. Tämä sai heidät soveltamaan tehostettuja suojatoimia varotoimenpiteenä (‡7, ‡33, ‡1121*). Frontier AI Safety -kehyksissä vaaditaan usein kyvykkyyksien ensiarviointi ennen riskinhallintaa sekä jäljelle jäävän riskin analyysi tai turvallisuustapaus, joka on usein informoitu red-teaming-harjoituksilla, riskinhallinnan jälkeen. Katso Taulukko 3.5 tarkemmat tiedot.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Valmiuskehys 2 (‡1078*)
  Mahdolliset riskit:
1. Biologiset ja kemialliset valmiudet
2. Kyberturvallisuuden valmiudet
3. AI:n itseparantamisominaisuudet
  Riskitasot tai vastaava taso sekä niihin liittyvät suojatoimet:
- Korkea: Voisi vahvistaa olemassa olevia reittejä vakavaan haittaan (Vaatii turvatoimia ja suojatoimia)
- Kriittinen: Voi avata ennennäkemättömiä uusia reittejä vakavaan vahinkoon (Keskeytä lisäkehitys, kunnes määritellyt suojatoimet ja tietoturvakontrollien standardit täyttävät kriittisen tason vaatimukset)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Vastuullisen skaalauksen toimintaperiaate 2.2 (‡991*)
  Mahdolliset riskit:
1. CBRN-aseet
2. Autonominen tekoälytutkimus ja -kehitys (AI R&D)
3. Kyberoperaatiot (arvioitavana)
  Riskitasot tai vastaavat sekä niihin liittyvät suojatoimet:
  AI-turvallisuustasot (ASL)
- ASL-1: Ei merkittävää katastrofaalista riskiä
- ASL-2: Varhaiset merkit vaarallisista kyvykkyyksistä (mallien on täytettävä ASL-2:n käyttöönotto- ja tietoturvastandardit)
- ASL-3: Olennaisesti kasvanut katastrofaalisen väärinkäytön riski (Mallien on täytettävä ASL-3:n käyttöönotto- ja/tai tietoturvastandardit)
- ASL-4+: Tulevat luokittelut (ei vielä määritelty)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Mahdolliset riskit:
1. Väärinkäyttö
    a. CBRN
    b. Kyber
    c. Haitallinen manipulointi
2. Koneoppimisen tutkimus- ja kehitystyö
3. Virhekohdistuma/Instrumentaalinen päättely
  Riskitasot tai vastaava ja niihin liittyvät suojaustoimenpiteet:
  Kriittisen kyvykkyystason tasot
    Kyvykkyystasot, joilla ilman lieventäviä toimenpiteitä (käyttöönottoja koskevat turvallisuustapaukset ja turvallisuuslievennykset, jotka on kohdistettu RANDin turvallisuustasoihin 2, 3 tai 4 (‡1122)), tekoälymallit tai -järjestelmät voivat aiheuttaa korostuneen riskin vakavasta vahingosta. Kyvykkyystasot sisältävät ’ennakkovaroitusten arvioinnit’, joissa on tarkat ’hälytyskynnykset’
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Frontier AI Framework 1.1 (‡990*)
  Mahdolliset riskit:
1. Kyberturvallisuus
2. Kemialliset ja biologiset riskit
  Riskitasot tai vastaavat ja niihin liittyvät suojatoimet:
  Riskikynnystasot
- Kohtalainen (julkaisu asianmukaisilla turvatoimilla ja lievennyksillä)
- igh (älä vapauta)
- Kriittinen (lopeta kehitys)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Frontier-mallin turvallisuuskehys (‡1123*)
  Mahdolliset riskit:
1. CBRN-aseiden leviämisuhka
2. Haitalliset kybertoiminnot
3. Automaattinen AI:n T&K
  Riskiluokat tai vastaavat sekä niihin liittyvät suojatoimet:
  Kriittisen kyvykkyyden kynnykset
    Mallin ominaisuudet, jotka voivat aiheuttaa merkittävää haittaa yleisölle, jos niitä käytetään väärin. (Jos kynnysarvot täyttyvät tai ylittyvät, mallia ei oteta julkiseen käyttöön ilman asianmukaisia riskienhallintatoimenpiteitä)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Frontier Governance Framework (‡1124*)
  Mahdolliset riskit:
1. CBRN-aseet
2. Haitalliset kybertoiminnot
3. Pitkälle kehittynyt autonomisuus (mukaan lukien tekoälyn T&K)
  Riskitasot tai vastaava ja niihin liittyvät suojatoimet:
  Riskitasot
- Matala tai Keskitaso (Käyttöönotto sallittu Vastuu AI -ohjelman vaatimusten mukaisesti)
- Korkea tai Kriittinen (lisäarviointi ja lieventävät toimenpiteet)
vaadittu)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Frontier AI -riskinarviointi (‡1029*)
  Mahdolliset riskit:
1. Kyberrikos
2. CBRN
3. Vakuuttelu ja manipulointi
4. Laiton syrjintä mittakaavassa
  Riskitasot tai vastaavat ja niihin liittyvät suojatoimet:
  Riskikynnykset – malliriskin (MR) pisteet
- MR1 tai MR2 (arviointitulokset dokumentoivat tekniikkatiimit)
- MR3 (Vaarojen lieventämistoimenpiteet ja arviointitulokset on dokumentoitu tekniikkatiimeissä ja niitä tarkistetaan säännöllisesti)
- MR4 (Yksityiskohtainen riskinarviointi on suoritettava ja liiketoimintayksikön johtajan hyväksyntä vaaditaan)
- MR5 (Yksityiskohtainen riskinarviointi on saatettava valmiiksi ja hyväksytettävä riippumattomalla toimikunnalla, esim. NVIDIA:n tekoälyn eettisellä toimikunnalla)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Suojattu tekoälyn kehittyneen mallin kehys (‡1125*)
  Mahdolliset riskit:
1. Kielteinen käyttö (esim. haittaohjelmat, lapsiin kohdistuva seksuaalinen hyväksikäyttö)
2. Haitta tavallisessa, ei-kurittomassa käytössä, esim. tuotokset, jotka johtavat laittomaan syrjivään lopputulokseen tai turvattoman koodin generointiin
  Riskitasot tai vastaavat ja niihin liittyvät suojatoimet:
  Haittatyyppisen vahingon todennäköisyys ja vakavuus kontekstissa
- Matala
- Keskitasoinen
- Korkea
- Erittäin korkea
    (Riskienhallintatoimenpiteitä ja tietoturvakontrolleja on käytössä kaikissa järjestelmissä ja prosesseissa; lisäksi tarvittavat lievennykset on mukautettava tekoälyjärjestelmään ja käyttötapaukseen, johon malli on otettu käyttöön)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: AGI-valmiuskäytäntö (‡1127*)
  Mahdolliset riskit:
1. Kyberrikos
2. Automaattinen AI:n T&K
3. Autonominen replikointi ja mukautuminen
4. Biologisten aseiden avustaminen
  Riskitasot tai vastaavat ja niihin liittyvät turvatoimet:
  Kriittisen kyvykkyyden kynnykset
    Määrälliset kynnysarvot kyvykkyysvertailuissa (jos ylittyvät, suorita vaarallisten kyvykkyyksien arviointeja, tietoturvatoimenpiteitä ja käyttöönoton lievennyksiä, tai keskeytä kehitys)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: AGI-valmiuspolitiikka (‡1127*)
  Mahdolliset riskit:
1. Kyberrikos
2. Automaattinen AI:n T&K
3. Autonominen replikaatio ja sopeutuminen
4. Biologisten aseiden avustaminen
  Riskitasot tai vastaava ja niihin liittyvät suojatoimet:
  Kriittisen kyvykkyyden kynnykset
    Määrälliset kynnysarvot kyvykkyysvertailuissa (jos ne ylitetään, suorita vaarallisia kyvykkyyksiä koskevia arviointeja, tietoturvatoimia ja käyttöönoton lievennyksiä, tai keskeytä kehitys)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: tekoälyn turvallisuuskehys (‡1128*)
  Mahdolliset riskit:
1. Hallinnan menetys
2. Väärinkäyttö (esim. biokemiallisten aseiden valmistaminen)
  Riskitasot tai vastaavat ja niihin liittyvät suojatoimet:
  Riskitasot
- Pieni riski (Ota käyttöön tekoälyjärjestelmiä, mutta suorita valvontaa jälkikäteen riskien hallitsemiseksi)
- Riski tunnistettu (Joko avataan AI-järjestelmät vain valtuutetuille käyttäjille riskien lieventämiseksi, tai lykätään käyttöönottoa, kunnes lisäturvatoimenpiteet on toteutettu käyttötapauksen mukaan)
- Korkea riski (Älä ota käyttöön tekoälyjärjestelmiä)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Frontier AI:n turvallisuuskehys (‡1129*)
  Mahdolliset riskit:
1. Biologiset uhkat
2. Offensiivinen kyberturvallisuus
3. Autonominen toiminta ja kehittynyt manipulointi
  Riskiluokat tai vastaavat ja niihin liittyvät suojatoimenpiteet:
  Riskitasot
- Taso 1 (Perustason suojatoimet vähäisille riskeille ja mahdollisuus avata lähdekoodi)
- Taso 2 (reaaliaikainen seuranta, kehotteiden suodatus, käyttäytymisen poikkeavuuksien havaitseminen, käyttöoikeuksien hallinta, red-teaming ja hyökkääjäharjoitukset sekä vastakkaiset simulaatiot)
- Taso 3 (Edistyneet suojatoimet, mukaan lukien red teaming, vaiheistetut käyttöönotot, adverisaarinen testaus, salaus, monen osapuolen pääsynhallinta ja zero-trust-arkkitehtuuri)
- Taso 4 (Suurin turvallisuusprotokollat korkean riskin malleille ja enimmäissuojatoimet)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.5: Frontier AI Safety -kehykset
>white|black||9|11|br Ensimmäinen joukko Frontier AI Safety -kehyksiä, jotka on julkaistu niiden AI-kehittäjien osajoukon toimesta, jotka ovat allekirjoittaneet Frontier AI Safety -sitoumukset. Kehykset kattavat samankaltaisia riskejä (pienin vaihteluin) ja käyttävät erilaisia riskitasoja sekä riskienhallintatapoja.


>white|orangered|left|14|15.5|bb Frontier AI Safety Frameworks -kehysten tehokkuus on epävarma

Frontier AI Safety Frameworks -viitekehykset voivat toimia riskienhallintatyökaluina tietyissä olosuhteissa ja tiettyihin riskiluokkiin, joilla on uskottava polku haittaan (‡1117). Samanaikaisesti useat analyysit käsittelevät kysymyksiä niiden selkeydestä ja laajuudesta (‡111, ‡986) sekä tekoälyn kyvykkyyden ja riskikynnysten kestävyyttä (‡1031, ‡1130). Nykyiset viitekehykset keskittyvät tyypillisesti vain osaan riskialueista. Tämän seurauksena eräät merkittävät riskit, kuten lainvastainen valvonta (‡1131, ‡1132) ja suostumuksettomat intiimikuvat (‡287), saavat vähemmän painoarvoa. Toisin kuin muiden toimialojen riskienhallintamallit, kuten ilmailu tai ydinvoima (‡1133*), Frontier AI Safety Frameworks -viitekehykset eivät tyypillisesti käytä eksplisiittisiä määrällisiä riskikynnysten arvoja (‡1134).

Kehittäjien rajat ylittävän tekoälyn turvallisuuskehystensä noudattamista koskevat ulkoiset arvioinnit ovat toistaiseksi rajallisia, osin siksi, että useimmat kehykset ovat uusia, julkisesti saatavilla oleva tieto on niukkaa, eikä ole olemassa standardoituja ulkoisia arviointeja. Niiden tehokkuuteen vaikuttaa myös se, kuinka hyvin – ja missä määrin – sitoumukset toteutetaan käytännössä. Pelkästään nämä kehykset eivät välttämättä takaa tehokasta riskienhallintaa, sillä niiden käytännön vaikutus riippuu siitä, kuinka hyvin – ja missä määrin – ne toteutetaan. Toistaiseksi ne eivät täysin vastaa kansainvälisiä riskienhallinnan standardeja (‡1135). Aiemmista vapaaehtoisista sitoumuksista tehty tutkimus havaitsi epätasaista toteutumista eri toimenpiteissä, mikä viittaa siihen, että vapaaehtoisiin sitoumuksiin sitoutumisen taso todennäköisesti vaihtelee yritysten ja toimialojen välillä (‡1109).

Yhdessä tarkasteltuna Frontier AI Safety Frameworks edustavat nykyisin käytössä olevan vapaaehtoisen organisaatiotason riskienhallinnan yksityiskohtaisinta muotoa, mutta ne vaihtelevat huomattavasti laajuudeltaan, kynnysarvoiltaan ja täytäntöönpanokelpoisuudeltaan.

###@ Sääntely- ja hallinnointialoitteet

>white|orangered|left|14|15.5|bb Useat lainkäyttöalueet ovat ottaneet käyttöön lakeja, joihin sisältyy läpinäkyvyysvaatimuksia

Useat varhaiset sääntelyä koskevat lähestymistavat tuovat esiin lainsäädännöllisiä vaatimuksia, joiden tarkoituksena on lisätä standardointia ja läpinäkyvyyttä riskienhallinnassa. EU:n tekoälyasetus (AI Act), joka tuli voimaan vuonna 2024, määrittää yleiskäyttöisiä tekoälymalleja koskevia vaatimuksia, jotka liittyvät läpinäkyvyyteen, tekijänoikeuksiin ja turvallisuuteen. Vuonna 2025 julkaistiin EU:n yleiskäyttöisen tekoälyn käytännesääntöjä (General-Purpose AI Code of Practice) koskeva asiakirja, jonka tarkoituksena on tukea näiden velvoitteiden noudattamista antamalla ohjeita mallien dokumentoinnista ja tekijänoikeuksista sekä – kaikkein kehittyneimmille malleille – riskienhallintakäytännöistä, kuten arvioinneista, riskien arvioinnista ja lieventämisestä, tietoturvasta ja vakavien turvallisuuspoikkeamien ilmoittamisesta (‡965).

Muita esimerkkejä uusista sääntelyvaatimuksista ovat Etelä-Korean laki tekoälyn kehittämisestä ja luottamuksen perustamisesta (Framework Act on the Development of Artificial Intelligence and Establishment of Trust), joka tuo vaatimuksia ”korkean vaikutuksen” tekoälyjärjestelmille kriittisillä toimialoilla (‡1136), sekä Kalifornian SB 53, joka asettaa avoimuusvaatimuksia turvallisuuskehyksille ja tapausraportoinnille (‡1104). Koska nämä vaatimukset on otettu käyttöön vasta hiljattain, on liian aikaista arvioida yksityiskohtaisesti, miten ne vaikuttavat riskienhallintakäytäntöihin tai todellisiin riskitilanteisiin.

>white|orangered|left|14|15.5|bb Laajemmat hallinnointia koskevat aloitteet tarjoavat vapaaehtoista ohjeistusta

Useat alueelliset ja alueiden väliset hallintokehykset ilmaisevat nyt yhteisiä odotuksia yleiskäyttöisen tekoälyn aiheuttamien riskien hallinnasta tarjoamalla ei-sitovaa ohjeistusta päätöksentekijöille ja organisaatioille. Kiinan AI Safety Governance Framework 2.0, joka julkaistiin vuonna 2025, antaa jäsenneltyä ohjausta riskiluokittelusta ja vastatoimista tekoälyn kehittämisen ja käyttöönoton koko prosessin aikana (‡1137). ASEANin jäsenvaltiot julkaisivat ‘ASEAN Expanded Guide on AI Governance and Ethics (Generative AI)’, joka tarjoaa ohjeita yleiskäyttöisen tekoälyn hallinnosta ja eettisyydestä ja jonka tarkoituksena on tukea laajempaa politiikkayhteensopivuutta ASEANin jäsenvaltioiden välillä (‡1138). Lisäksi asiantuntijavetoiset aloitteet, kuten Singaporen konsensus, jonka ovat kehittäneet useista maista tulleet tekoälytutkijat, kuvaavat tutkimuksen painopistealueita yleiskäyttöisen tekoälyn turvallisuuden osalta riskinarvioinnissa, kehityksessä ja ohjauksessa (‡690).

###@ Päivitykset

Viimeisen raportin (tammikuu 2025) julkaisemisen jälkeen yleiskäyttöisen tekoälyn riskinhallinnan toimintaympäristö on kehittynyt. Uusia resursseja on julkaistu, kuten EU:n yleiskäyttöisen tekoälyn käytännesääntö (General-Purpose AI Code of Practice), G7:n HAIP-raportointikehys (G7 HAIP Reporting Framework), Kiinan kansallinen tekoälyn turvallisuus- ja hallintakehys 2.0 sekä useita eri tekoälykehittäjien Frontier AI Safety -kehyksiä. Nämä aloitteet kuvaavat lähestymistapoja ja käytäntöjä, joita tekoälykehittäjät käyttävät hallitakseen yleiskäyttöisiin tekoälyjärjestelmiin (‡1115) liittyviä riskejä. Frontier AI Safety -kehyksissä ja HAIP-läpinäkyvyysraporteissa (‡1103) on huomattavaa vaihtelua, mikä heijastaa eroja organisaation käytännöissä, riskien priorisoinnissa ja yleiskäyttöisen tekoälyn riskinhallinnan ekosysteemin varhaisessa kehitysvaiheessa. Luotettava ekosysteemi, jossa eri tekoälytoimijat osallistuvat toisiaan täydentäviin riskinhallinnan käytäntöihin koko elinkaaren ajan, voi edistää tehokasta riskinhallintaa (‡690).

###@ Todisteiden puutteet

On näyttöä puuttuu siitä, miten kehittyvien riskien vakavuus, yleisyys ja ajallinen ulottuvuus voidaan mitata; missä määrin näitä riskejä voidaan lieventää tosielämän toimintaympäristöissä; sekä miten lieventämisen käyttöönottoa voidaan kannustaa tai velvoittaa tehokkaasti eri toimijoiden keskuudessa. Lisää tutkimusta tarvitaan, jotta ymmärretään, kuinka yleisiä erilaiset riskit ovat ja kuinka paljon ne vaihtelevat eri puolilla maailmaa, erityisesti alueilla kuten Aasia, Afrikka ja Latinalainen Amerikka, jotka digitalisoituvat nopeasti. Kun tekoälymalleille annetaan yhä enemmän toimivaltaa ja auktoriteettia ja yleiskäyttöisen tekoälyn riskien tieteellinen tila edistyy, myös riskienhallintalähestymistapojen on kehittyttävä (‡639, ‡1139).

Tietyt riskien lieventämistoimet ovat kasvattaneet suosiotaan (‡690, ‡956), mutta tarvitaan lisää tutkimusta sen ymmärtämiseksi, kuinka kestäviä riskien lieventämistoimet ja turvatoimet ovat käytännössä eri yhteisöissä ja tekoälytoimijoiden keskuudessa (mukaan lukien pienet ja keskisuuret yritykset). Laajempi pääsy dataan tosielämän mallien käyttöönotosta ja käytöstä on olennaista tällaisissa arvioinneissa. Lisäksi riskinhallintatoimet vaihtelevat tällä hetkellä erittäin paljon johtavien tekoälyyritysten välillä. On esitetty, että kehittäjien kannustimet eivät ole hyvin linjassa perusteellisen riskinarvioinnin ja -hallinnan kanssa (‡934). Näyttöä koskeva aukko on edelleen olemassa sen suhteen, missä määrin eri vapaaehtoisia sitoumuksia täytetään, mitä esteitä yritykset kohtaavat sitoumusten täysimääräisessä noudattamisessa ja miten ne integroivat Frontier AI Safety Frameworks -kehyksiä laajempiin tekoälyn riskinhallintakäytäntöihin.

###@ Haasteet poliittisille päättäjille

Keskeisiä haasteita ovat sen määrittäminen, miten yleiskäyttöisen tekoälyn aiheuttamat monimuotoiset riskit tulisi priorisoida, sen selventäminen, mitkä toimijat ovat parhaiten kykeneviä lieventämään niitä, sekä sen ymmärtäminen, millaiset kannustimet ja rajoitteet muovaavat näiden toimijoiden toimintaa. Näyttö viittaa siihen, että päättäjillä on tällä hetkellä rajallinen pääsy tietoon siitä, miten tekoälyn kehittäjät ja hyödyntäjät testaavat, arvioivat ja seuraavat kehittyviä riskejä, sekä siitä, miten tehokkaita eri lieventämiskäytännöt ovat (‡1140). Tutkijat ja päättäjät ovat käsitelleet läpinäkyvyyttä ja aiempaa systemaattisempaa tapausraportointia mahdollisina keinoina, joilla voitaisiin tarjota tietoa riskien priorisointiin, edistää luottamusta ja kannustaa vastuulliseen kehittämiseen (‡957). Käytännössä riskienhallinta edellyttää useita toimijoita tekoälyn arvoketjussa – kuten data- ja pilvipalveluiden tarjoajia, mallien kehittäjiä ja mallien ylläpitopalveluja – joilla kullakin on erilaiset mahdollisuudet arvioida ja hallita erilaisia riskejä (‡1141). Rajallinen tiedon jakaminen näiden toimijoiden välillä vaikeuttaa sen määrittämistä, mitkä riskit ovat todennäköisimpiä tai vaikutuksiltaan merkittävimpiä, erityisesti silloin, kun tarkastellaan vaikutuksia yhteiskunnan tasolla.

