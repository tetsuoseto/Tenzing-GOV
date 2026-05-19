##########
>white|orangered|left|14|30|hr Luku 3.3
### 3.3. Tekniset suojatoimet ja valvonta
>white|orangered|left|24|30|hb Tekniset turvatoimet ja valvonta

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Tärkeimmät tiedot
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br Laajaa teknisten suojatoimien kirjoa käytetään eri vaiheissa AI:n kehitystä ja käyttöä. Näihin kuuluvat malli kehityksen aikana tehtävät menetelmät, joilla järjestelmistä tehdään kestävämpiä ja väärinkäytöille vastustuskykyisempiä (kuten datan kuratointi), käyttöönoton aikainen seuranta ja ohjaus (kuten sisällön suodatus ja ihmisen valvonta) sekä käyttöönoton jälkeiset työkalut, joilla seurataan laajempaa AI-ekosysteemiä (kuten alkuperän todentaminen ja sisällön tunnistus).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Teknisillä suojatoimilla on rajoituksensa, eikä niitä voida luotettavasti käyttää haitallisen toiminnan estämiseen kaikissa tilanteissa. Esimerkiksi käyttäjät voivat joskus saada haitallisia tuloksia muotoilemalla pyynnöt uudelleen tai jakamalla ne pienempiin vaiheisiin. Samoin työkalut, kuten vesileimaukset, jotka on suunniteltu tunnistamaan tekoälyn tuottamaa sisällön, voidaan usein poistaa tai muokata, mikä heikentää niiden luotettavuutta.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Yksittäisten suojausten rajoitukset tarkoittavat, että ‘puolustus syvyyteen’ -lähestymistapaa voidaan tarvita tiettyjen haitallisten lopputulosten estämiseksi. Esimerkiksi järjestelmä voi yhdistää turvallisuuskoulutetun mallin syötesuodattimiin, tulostesuodattimiin ja sisällön valvontajärjestelmiin.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Viimeisimmän raportin julkaisemisen jälkeen (tammikuu 2025) tutkijat ovat edistäneet suojauksen parantamista, mutta perustavanlaatuiset rajoitukset pysyvät edelleen. Esimerkiksi suojauksen ohittamiseen suunniteltujen hyökkäysten onnistumisprosentti on laskenut, mutta pysyy silti suhteellisen korkeana. Lisäksi on olemassa perustavanlaatuisia rajoituksia sille, kuinka kattavasti avoimen painon (open-weight) mallit voidaan suojata.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Keskeinen haaste poliittisille päättäjille on rajallinen näyttö siitä, kuinka tehokkaita suojatoimet ovat eri käytännön käyttötapauksissa yleiskäyttöisille tekoälyjärjestelmille. AI-kehittäjät vaihtelevat suuresti siinä, kuinka paljon tietoa he jakavat suojatoimistaan ja seurannastaan. Lisähaasteena ovat mahdolliset kompromissit, jotka liittyvät vahvempien suojatoimien käyttämiseen ja toisaalta järjestelmän suorituskyvyn tai hyödyllisyyden ylläpitämiseen.
>oldlace|black||11|15|br      


AI-kehittäjät voivat käyttää useita hyödyllisiä mutta epätäydellisiä teknisiä suojatoimia lieventääkseen ja hallitakseen yleiskäyttöisistä AI-järjestelmistä aiheutuvia riskejä, mutta vankkuushaasteet jatkuvat. Kehittäjät eivät vieläkään pysty täysin estämään yleiskäyttöisiä AI-järjestelmiä suorittamasta myös hyvin tunnettuja ja selvästi haitallisia toimia, kuten tarjota käyttäjille ohjeita rikosten tekemiseen. Esimerkiksi tutkijat ovat osoittaneet, että huippuluokan suojatoimet voidaan kiertää adversaarisilla kehote- ja promptausmenetelmillä (eli ‘jailbreakit’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), kun mallit pilkkovat monimutkaiset haitalliset tehtävät vaiheisiin (‡1150, ‡1151, ‡1152, ‡1153, ‡1154) ja yksinkertaisilla mallimuutoksilla (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Tutkijat jatkavat työskentelyä vikatoimintoja ja väärinkäyttöä vastaan suunnattujen suojatoimien parissa (‡690). Nämä menetelmät vaihtelevat laajasti tarkoituksensa ja tehokkuutensa osalta, ja niiden vaikutus riippuu lopulta laajemmasta sosioteknisestä ja hallinnollisesta kontekstista, jossa AI-järjestelmiä rakennetaan ja otetaan käyttöön.

Tekniset suojatoimet voidaan laajasti jakaa kolmeen luokkaan: tekniikoihin turvallisempien mallien kehittämiseksi; tekniikoihin, joita käytetään käyttöönoton aikana valvontaan ja ohjaukseen; sekä tekniikoihin, jotka tukevat käyttöönoton jälkeistä ekosysteemin seurantaa. Taulukko 3.6 kokoaa yhteen käsitellyt tekniset suojatoimet, niiden tehokkuuden ja avoimet haasteet.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Turvallisempien mallien kehittäminen
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tiedon kuratointi (‡1167)
  Poistetaan haitalliset tiedot, jotta malli ei opi vaarallisia kyvykkyyksiä. Nämä menetelmät voivat olla hyödyllisiä, myös kehitettäessä avoimen painotuksen malleja, joilla ei ole haitallisia kyvykkyyksiä ja jotka kestävät haitallista hienosäätöä (‡55). Kuitenkin tietojen kuratoinnissa voi esiintyä virheitä ja mittakaavoitus voi olla haastavaa (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vahvistusoppiminen ihmisen palautteesta (‡64*)
  Mallin kouluttaminen vastaamaan määritettyjä tavoitteita, kuten olemaan hyödyllinen ja vahingoittamaton. Tämä on tehokas tapa saada mallit oppimaan hyödyllisiä toimintatapoja (‡64*). Kuitenkin ihmisten hyväksyntää varten tehty liiallinen optimointi voi saada mallit käyttäytymään petollisesti tai mielistelevästi (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pluralistiset kohdistustekniikat (‡1170)
  Koulutetaan malli integroimaan useita erilaisia näkemyksiä siitä, miten sen tulisi toimia. Nämä tekniikat auttavat vähentämään sitä laajuutta, jossa mallit suosivat tiettyjä näkemyksiä (‡1170). Näistä tekniikoista huolimatta ihmisten erimielisyys on kuitenkin väistämätöntä, ja on vaikeaa suunnitella yleisesti hyväksyttyjä tapoja tasapainottaa kilpailevia näkemyksiä (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vastustavallinen harjoittelu (‡677)
  Mallin kouluttaminen kieltäytymään aiheuttamasta vahinkoa (myös tunnistamattomissa tilanteissa) ja vastustamaan hyökkäyksiä haitallisilta käyttäjiltä (esim. ”jailbreakit”). Tämä on tehokas menetelmä, jolla mallit saadaan vastustamaan yrityksiä väärinkäyttöön (‡1064), mutta kestävyysongelmat jatkuvat (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Koneen “unlearning” (‡1175, ‡1176)
  Mallin kouluttaminen erikoistuneilla algoritmeilla tarkoittaa sellaisten haitallisten kyvykkyyksien aktiivista tukahduttamista (esim. tietämys biologisista vaaratekijöistä). Nämä tekniikat tarjoavat kohdennetun tavan poistaa haitallisia kyvykkyyksiä malleista (‡1175, ‡1176), mutta nykyiset unlearning-algoritmit voivat olla epäluotettavia ja aiheuttaa tahattomia vaikutuksia muihin kyvykkyyksiin (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Selitettävyyden ja turvallisuuden varmistamisen työkalut (‡1177)
  Suunnittelu- ja verifiointimenetelmien monimuotoinen kokonaisuus, jonka tarkoituksena on tarjota aiempaa tiukempaa varmistusta siitä, että malleilla on tiettyjä turvallisuuteen liittyviä ominaisuuksia. Nämä menetelmät mahdollistavat arvioijien saavuttaa suuremman luottamuksen turvallisuutta koskeviin varmistuksiin (‡1177), mutta nykyiset menetelmät nojaavat oletuksiin eivätkä ole käytännössä harvoin kilpailukykyisiä suorituskyvyn osalta (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Valvonta ja ohjaus
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Laittopohjaiset valvontamekanismit (‡1179, ‡1180, ‡1181)
  Varmistetaan, että valtuutetut prosessit ovat käynnissä laitteistossa, jotta voidaan tutkia tietoturvauhkia tai säädöstenmukaisuutta. Nämä mekanismit tarjoavat ainutlaatuisia tapoja seurata, mitä laskentoja laitteistossa ajetaan ja kenen toimesta (‡1181). Kuitenkin laitteistomekanismit eivät pysty havaitsemaan kaikentyyppisiä uhkia, ja jotkin tekniikat edellyttävät erikoistunutta laitteistoa (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Käyttäjävuorovaikutuksen seuranta (‡1154, ‡1166)
  Käyttäjien vuorovaikutusten seuraaminen haitallisen käytön merkkien varalta voi auttaa kehittäjiä lopettamaan palvelun haitallisilta käyttäjiltä (‡1154, ‡1166). Täytäntöönpano voi kuitenkin vahingossa haitata hyödyllistä turvallisuustutkimusta (‡689), ja joitakin väärinkäytön muotoja on vaikea havaita (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Käyttäjävuorovaikutuksen seuranta (‡1154, ‡1166)
  Käyttäjien vuorovaikutusten seuraaminen haitallisen käytön merkkejä varten voi auttaa kehittäjiä lopettamaan palvelun haitallisille käyttäjille (‡1154, ‡1166). Käyttöohjeiden noudattamisen valvonta voi kuitenkin tahattomasti haitata hyödyllistä turvallisuustutkimusta (‡689), ja joitakin väärinkäytön muotoja on vaikea havaita (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sisällönsuodattimet (‡65*, ‡725)
  Mahdollisesti haitallisten mallin syötteiden ja tulosteiden suodattaminen on erittäin tehokas tapa vähentää vahingollisia haittoja ja väärinkäytön riskejä (‡725). Kuitenkin suodattimet vaativat lisää laskentatehoa ja ovat alttiita joillekin hyökkäyksille (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mallituksen sisäiset laskennan monitorit (‡744, ‡1183, ‡1184)
  Mallien sisäisen tietoisuuden, kuten petollisuuden tai muiden haitallisten kognitiomuotojen, merkkien seuranta voi olla tehokas tapa havaita petollisuutta (‡744, ‡1183, ‡1184). Nykyiset menetelmät kuitenkin puuttuvat varmuudesta ja luotettavuudesta (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Päättelyketjun valvontajärjestelmät (‡430, ‡435)
  Malliketjun päättelytekstin seuraaminen merkkien varalta harhaanjohtavasta toiminnasta tai muusta haitallisesta päättelystä on tehokas tapa ymmärtää ja havaita puutteita siinä, miten mallit päättävät (‡435). Ne voivat kuitenkin olla epäluotettavia (‡752, ‡753, ‡1186), ja jos mallit koulutetaan tuottamaan vaaratonta ketjun päättelyä, ne voivat oppia harhaanjohtavaa käyttäytymistä (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ihminen silmukassa (‡1187, ‡1188, ‡1189)
  Ihmisen valvonta ja ohitukset järjestelmän päätöksille ovat välttämättömiä joissakin turvallisuuskriittisissä sovelluksissa (‡1187). Nämä tekniikat ovat kuitenkin rajallisia automaatiovääristymän ja ihmisen päätöksenteon nopeuden rajoitteiden vuoksi (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Suojaus hiekkalaatikossa (‡1192)
  Aivan suoran maailmanvaikutuksen estäminen AI-agentilta on tehokas tapa rajoittaa sen aiheuttamaa haittaa (‡1192). Kuitenkin eristysympäristö (sandbox) rajoittaa järjestelmän kykyä suoraan toteuttaa tiettyjä tehtäviä (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Työkalut ekosysteemin seurannan helpottamiseksi
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tekoälymallin tunnistamistekniikat (‡1193*, ‡1194)
  Mallien, tai mallien yksittäisten ilmentymien, tunnistettavuutta parantavien toimenpiteiden helpottaminen todellisissa käyttötilanteissa edistää digitaalista forensiikkaa ja ekosysteemitietoisuutta (‡1195). Näitä tekniikoita voidaan kuitenkin kiertää eräillä mallimuutoksilla (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI-malliperimän päätelmät (‡1197)
  Nämä tekniikat mahdollistavat tutkijoiden selvittää, miten malleja muokataan tekoälyekosysteemissä, erityisesti avoimen painon malleissa. Ne auttavat digitaalisen forensiikan ja ekosysteemitietoisuuden kanssa (‡1198), mutta tarvittaisiin laajamittaisia hankkeita, jotta avoimen painon malliekosysteemi (‡1198) voitaisiin kartoittaa perusteellisesti.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Vesileimat ja metatiedot (‡1199, ‡1200, ‡1201*)
  Nämä tekniikat helpottavat havaitsemaan, milloin jokin tekstin, kuvan, videon jne. sisältö on luotu tai muokattu tekoälyllä, sekä millä järjestelmällä. Ne helpottavat paremman ekosysteemitietoisuuden ylläpitämistä (‡1199, ‡1200, ‡1201*). Vesileimat ja metatiedot voidaan kuitenkin väärentää tai poistaa joillakin sisällön muokkauksilla (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tekoälyn tuottaman sisällön tunnistaminen (‡1203, ‡1204, ‡1205*)
  Käyttäjien kyky erottaa toisistaan tekoälyn tuottama ja aito sisältö parantaa digitaalista forensiikkaa ja ekosysteemitietoisuutta (‡1203, ‡1204). Luokittelijat voivat kuitenkin olla epäluotettavia (‡1205*) ja niiden suorituskyky voi vaihdella eri modaliteeteissa.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.6: Tässä osiossa käsitellyt tekniset suojatoimet
>white|black||9|11|br Yhteenveto tässä jaksossa käsitellyistä teknisistä suojatoimista jaoteltuna menetelmiin turvallisempien mallien kehittämiseksi, käyttöönottoaikaisesta seurannasta ja ohjauksesta sekä tekniikoista ekosysteemin seurannan helpottamiseksi.


###@ Turvallisempien mallien kehittäminen

Ensimmäinen puolustuslinja yleiskäyttöisten tekoälyjärjestelmien aiheuttamia haittoja vastaan on tehdä taustalla oleva malli turvallisemmaksi. Tämä alaluku käsittelee suojatoimia, jotka on “leivottu mallin parametreihin” mallin kehitysprosessin aikana (Kuva 3.6).

>white|orangered|left|14|15.5|bb Koulutusdatan kuratointi voi rajoittaa sellaisten mahdollisesti vaarallisten kyvykkyyksien kehittämistä

Yleistarkoituksiin tarkoitetut tekoälymallit ovat hyödyllisiä nimenomaan siksi, että ne kehittävät laajan kirjon tietoa ja kyvykkyyksiä käsiteltyään koulutusaineistoa, mutta tietyt koulutusaineistojen tyypit ovat suhteettoman vastuussa sellaisten mahdollisesti vaarallisten kyvykkyyksien kehittymisestä, joita voidaan käyttää väärin. Esimerkiksi virustutkimusartikkeleilla koulutettu tekoälymalli saattaa pystyä tarjoamaan apua mahdollisesti haitallisissa biologiaan liittyvissä tehtävissä (‡549, ‡1206*) (katso myös §2.1.4. Biologiset ja kemialliset riskit). Lisäksi ihmisruumiin alastomuuden kuviin koulutetut kuva-/videogeneraattorit voidaan myös väärinkäyttää ei-suostumuksellisten intiimien deepfakejen luomiseen (‡308, ‡319) (katso myös §2.1.1. AI:n tuottama sisältö ja rikollinen toiminta).

Koulutusaineiston suodattaminen on tehokas lieventämiskeino joitakin ei-toivottuja kyvykkyyksiä vastaan (‡319, ‡1167, ‡1207, ‡1208). Suurten yleiskäyttöisten tekoälymallien (‡1168) koulutuksessa käytettävien aineistojen suodattaminen voi kuitenkin olla vaikeaa korkeiden kustannusten (‡1209), suodatuksen virheiden (‡1210) ja aineiston laadun heikentävien vaikutusten (‡1211) vuoksi. Nämä haasteet korostuvat internettekstin monikielisyydestä johtuen (‡1212), sisällön moderoinnin kulttuurisista ennakkoluuloista (‡1211, ‡1213, ‡1214, ‡1215) sekä siitä, että se, onko jokin aineiston osa “haitallista”, riippuu kontekstuaalisista tekijöistä (‡1216). Siitä huolimatta mahdollisesti haitallisen materiaalin suodattaminen koulutusaineistosta vaikuttaa lupaavalta mallien turvallisuuden parantamiseksi luotettavammin, mukaan lukien se, että avoimen painon (open-weight) mallit muuttuvat kestävämmiksi haitallista manipulointia vastaan (‡55). Koulutusaineiston sisällön ja emergenttien mallikyvykkyyksien välisiä yhteyksiä ei ole vielä täysin ymmärretty (‡1195), ja suodatuksen näyttäisi olevan tehokkaampaa haitallisten kyvykkyyksien rajoittamisessa, kun sitä sovelletaan laajoihin tietämisen alueisiin (‡55), verrattuna kapeampiin käyttäytymismalleihin (‡1206, ‡1217). Katso §3.4. Open-weight-mallit lisäkeskustelua varten.

![figure 3.6](images/fig3.6_safeguards.png)

##### Kuva 3.6: Mihin soveltaa teknisiä turvatoimia
>white|black||9|11|br Teknisiä suojatoimia voidaan soveltaa mallin kehittämisen eri vaiheissa. Tietojen kuratointi muokkaa sitä, mitä mallit oppivat esikoulutuksen ja hienosäädön aikana. Koulutukseen perustuvat menetelmät, kuten vahvistusoppiminen ihmispalautteesta ja kestävyyskoulutus, säätävät mallin käyttäytymistä. Testausmenetelmät, kuten vastahyökkäykset, tunnistavat jäljellä olevat haavoittuvuudet. Jotkin tekniikat, kuten safe-by-design-algoritmit, ulottuvat useiden vaiheiden yli. Lähde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Menetelmät yleiskäyttöisten tekoälymallien kouluttamiseksi niin, että ne ovat hyödyllisiä ja haitattomia, perustuvat pääasiassa ihmispalautteeseen

Malleja on vaikea kouluttaa ja arvioida luotettavasti siten, että ne noudattavat korkeatasoisia periaatteita, kuten hyödyllisyyttä, vaarattomuutta ja rehellisyyttä. Käytännössä kehittäjät pyrkivät saavuttamaan tämän hienosäätämällä tekoälymalleja ihmisten antamien esimerkkien ja palautteen avulla. Esimerkiksi hienosäädön keskeinen paradigmainen lähestymistapa, joka tunnetaan nimellä ”reinforcement learning from human feedback”, perustuu mallien kouluttamiseen tuottamaan tuotoksia, joita ihmisen arvioijat arvioivat myönteisesti (‡1218). Myönteinen palaute ihmisiltä on kuitenkin puutteellinen korvike hyödylliselle toiminnalle (‡737, ‡878, ‡1219, ‡1220) ja siihen vaikuttavat ihmisen virheet sekä vinoumat (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Tämä johtaa useisiin haasteisiin: mallit, joita on hienosäädetty vahvistusoppimisella ihmisen palautteen avulla, saattavat joskus miellyttää käyttäjää, mikä on tunnettu käyttäytymisenä nimellä ”sykofania” (‡358, ‡740, ‡1226, ‡1227); tuottaa vastauksia, jotka ovat hyödyllisiä joissakin konteksteissa mutta haitallisia toisissa (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); tuottaa vastauksia, joiden oikeellisuuden arviointi on vaikeaa (‡1233); tai suorittaa toimia, joiden hyödyllisyys tai haitallisuus on mielipidekysymys (‡1234). Taulukko 3.7 esittää esimerkkejä näistä haasteista. Osa tutkimuksesta pyrkii kehittämään menetelmiä, joilla ihmisiä voidaan auttaa arvioimaan paremmin tekoälyn avustamana monimutkaisten tehtävien ratkaisuja (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Näillä menetelmillä on kuitenkin tällä hetkellä rajallinen luotettavuus, eikä ole julkisesti tiedossa, missä määrin niitä käytetään nykyisin kehittyneimpien tekoälimallien kouluttamiseen.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Syyllisyys miellyttämisellä/ mielistelevä asenne (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Selitys:
>white|black|left|11|13|br Malli antaa vain positiivista palautetta eikä onnistu huomauttamaan puutteesta, eli siitä ettei 5-7-5 haikun tavurakenne täyty oikein.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Jotkin toimet ovat hyödyllisiä joissakin konteksteissa mutta haitallisia toisissa (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Selitys:
>white|black|left|11|13|br Tietoja biologisesta riskistä voidaan käyttää koulutukseen ja puolustukseen, mutta myös siihen, että pahantahtoiset toimijat saavat niistä tietoa.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Oikean toiminnan varmistaminen on vaikeaa (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Selitys:
>white|black||11|13|br Tämän vastauksen oikeellisuutta on vaikea arvioida, koska se vaatii lääketieteellistä asiantuntemusta. Vaikka kyseessä olisi kokenut lääkäri, tällaisten vastausten arvioiminen vaatii aikaa ja huolellista paneutumista yksityiskohtiin.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Ihmiset ovat eri mieltä siitä, mikä on oikein (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Selitys:
>white|black|left|11|13|br Ihmiset ovat huomattavasti eri mieltä siitä, mikä on oikea vastaus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.7: Käyttäjän kehotepyyntö ja tekoälymallin vastaus
>white|black||9|11|br Esimerkkejä haasteista, jotka liittyvät hyödyllisten toimien määrittämiseen ja kannustamiseen tekoälymallien avulla.


>white|orangered|left|14|15.5|bb Ihmiset eivät aina ole samaa mieltä siitä, millaiset käyttäytymismallit ovat toivottavia, mikä edellyttää menetelmiä tasapainottamaan kilpailevia mieltymyksiä

Ihmiset eivät aina ole yhtä mieltä siitä, mitä vastauksia tai toimia tekoälymallien pitäisi tai ei pitäisi tuottaa (‡1006). Tämä tekee olennaisesti haastavaksi kehittää malleja, joiden toiminta ja vaikutukset ovat laajasti yhteensopivia yhteiskunnan etujen kanssa (‡420). Osa tutkijoista tutkii, joiden mieltymykset heijastuvat tekoälyjärjestelmissä (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) ja pyrkii kehittämään ”pluralistisen kohdistuksen” (pluralistic alignment) tekniikoita, joiden tavoitteena on löytää tasapaino kilpailevien mieltymysten välillä (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Esimerkiksi tekoälyn kehittäjät voivat suunnitella järjestelmiä välttämään kiistanalaisten vastausten tuottamista kieltäytymällä vastaamasta tietyntyyppisiin pyyntöihin, tai kohdistumaan joihinkin relevantteihin ihmisjoukkoihin perustuvan näkökantakannan mediaanin, tai personoimaan järjestelmiä yksittäisille käyttäjille.

Yleinen haaste näille lähestymistavoille on, että yleisesti ottaen tekoälyjärjestelmät eivät voi asettua yhtä hyvin kaikkien mieltymysten mukaisiksi, ja että niiden välittömät yhteiskunnalliset vaikutukset kohdistuvat eri tavoin eri ihmisryhmiin. Jotkut tutkijat ovat väittäneet, että useimmat tekniset lähestymistavat pluralistiseen (moniarvoiseen) kohdentamiseen eivät onnistu käsittelemään, ja mahdollisesti jopa vievät huomion pois, syvemmistä haasteista, kuten järjestelmällisistä vinoumista, sosiaalisen vallan dynamiikasta sekä varallisuuden ja vaikutusvallan keskittymisestä (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI-kehittäjät käyttävät “adversaarista harjoittelua” parantaakseen mallin robustiutta

On haastavaa varmistaa, että tekoälymallit pystyvät luotettavasti siirtämään oppimansa hyödylliset toimintatavat koulutuksen aikana todellisiin käyttöönoton ympäristöihin. Vaikka mallit olisi koulutettu niin sanotulla ‘täydellisellä’ oppimissignaalilla, ne voivat silti epäonnistua yleistämään onnistuneesti kaikkiin uusiin, ennen näkemättömiin tilanteisiin (‡738, ‡739, ‡1255, ‡1256, ‡1257). Esimerkiksi jotkut tutkijat ovat havainneet, että chatbotit toteuttavat haitallisia toimia todennäköisemmin kielillä, jotka ovat aliedustettuina niiden koulutusaineistossa (‡159, ‡880, ‡1258*, ‡1259). Tähän kuuluu monia kieliä, joita puhutaan pääasiassa Global South -alueella.

Viime vuosina tutkijat ovat myös kehittäneet suuren kokoelman ”adversarial attack” -menetelmiä, joita voidaan käyttää siihen, että mallit tuottavat mahdollisesti haitallisia vastauksia (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Esimerkiksi eräs hiljattainen aloite keräsi joukkorahoituksella yli 60,000 erilaista esimerkkiä onnistuneista hyökkäyksistä huipputason AI-malleja vastaan, mikä sai ne rikkomaan yritystensä käytäntöjä hyväksyttävästä mallin toiminnasta (‡1149). Taulukko 3.8 esittää esimerkkejä ”jailbreak”-menetelmistä, joita tutkijat ovat osoittaneet kykenevän saamaan mallit noudattamaan haitallisia pyyntöjä.

Yksi tapa parantaa mallien robustisuutta tunnetaan nimellä “adversaarikoulutus” (‡1064). Se sisältää “hyökkäysten” (esim. jailbreakingien) rakentamisen, joiden tarkoituksena on saada malli toimimaan ei-toivotulla tavalla, ja mallin kouluttamisen niin, että se käsittelee nämä hyökkäykset asianmukaisesti. Adversaarikoulutus on kuitenkin puutteellinen (‡1260, ‡1261). Hyökkääjät pystyvät jatkuvasti kehittämään uusia onnistuneita hyökkäyksiä huipputason malleja vastaan (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Koska kehittäjät tarvitsevat nimenomaisia esimerkkejä epäonnistumistavoista kouluttaakseen niitä vastaan (‡512, ‡1263), seurauksena on jatkuva “kissa ja hiiri” -peli: kehittäjät päivittävät malleja jatkuvasti uusien havaittujen haavoittuvuuksien perusteella, ja vastustajat etsivät jatkuvasti uusia hyökkäyksiä. Jotkut tutkijat ovat ehdottaneet suurempimittakaavaista adversaarikoulutusta (‡1264, ‡1265) tai uusia algoritmeja (‡675, ‡676, ‡1263, ‡1266, ‡1267) robustisuuden parantamiseksi, mutta nykyaikaiset tekoälyjärjestelmät ovat edelleen pysyvästi haavoittuvia.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Tee haitallisia pyyntöjä salakirjoitetussa muodossa, kuten morsekoodina (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Esitä järjestelmä valmiiksi esimerkeillä vaatimukset täyttävistä vastauksista haitallisiin pyyntöihin (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Tee haitallisia pyynnöistä vähäresurssisilla kielillä, joiden todennäköisyys olla vähemmän käytetty koulutuksessa on suurempi (esim. swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategia: Jaa haitallinen tehtävä useisiin vaarattomiin alitehtäviin (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Taulukko 3.8: Jailbreakkausstrategiat
>white|black||9|11|br Pahantahtoiset toimijat ja red team -ryhmät ovat käyttäneet erilaisia niin sanottuja ”jailbreakeja” saadakseen tekoälymallit noudattamaan haitallisia pyyntöjä, joita ne normaalisti kieltäytyisivät toteuttamasta turvasuojien vuoksi. Esimerkkitulokset ovat raportin tekijöiden kirjoittamia havainnollistamistarkoituksessa. Monet nykyisistä huipputason tekoälymalleista kestävät nyt jo suurimman osan näistä menetelmistä, mutta uusia jailbreak-tekniikoita löydetään edelleen.


>white|orangered|left|14|15.5|bb ”Unlearning”-menetelmät voivat lieventää tiettyjä haitallisia mallin ominaisuuksia

Toinen strategia riskien lieventämiseksi yleiskäyttöisestä tekoälystä on hienosäätää malleja niin, etteivät ne omaa kyvykkyyksiä tietyillä erityisen korkean riskin alueilla (‡1175, ‡1176). Esimerkiksi tutkijat työskentelevät kehittääkseen ’machine unlearning’ -algoritmeja, jotka pystyvät nimenomaisesti vaimentamaan kyvykkyyksiä, jotka liittyvät biouhkille, tai kykyä tuottaa fotorealistisia kuvia alastomista ihmisen kehoista (‡903, ‡1272, ‡1273). Nämä menetelmät voivat tehdä malleista olennaisesti turvallisempia rajoittamalla samalla joitakin myönteisiä käyttötapoja niille kyvykkyyksille, jotka on unlearnattu. On myös ehdotettu, että AI-mallien tietämystä haitallisista osa-alueista rajoitettaisiin keinona suunnitella ’tamper-resistant’ -avoimen painon malleja, jotka pystyvät vastustamaan haitallista hienosäätöä (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tähän mennessä tätä on kuitenkin ollut vaikea toteuttaa luotettavasti (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Katso §3.4. Open-weight -mallit lisäkeskustelua varten.

>white|orangered|left|14|15.5|bb Jotkut tutkijat työskentelevät menetelmien parissa vahvempien turvallisuusvarmistusten aikaansaamiseksi tulkitsemalla mallin sisäisiä tiloja tai käyttämällä matemaattista todentamista.

Jotkut tutkijat työskentelevät menetelmien parissa, joilla mallien turvallisuuteen liittyviä ominaisuuksia voidaan todentaa nykyistä tiukemmin. Yhdessä lähestymistavassa tutkijat pyrkivät tulkitsemaan mallien sisäisiä laskentavaiheita joko riskien tunnistamiseksi tai parempien ja vakuuttavampien perustelujen esittämiseksi siitä, että malli on turvallinen (‡1285, ‡1286). Esimerkiksi konseptitodistuksessa tutkijat osoittivat, että työkaluista, jotka analysoivat kielimallin sisäistä laskentaa, voi olla apua arvioijille haitallisten käyttäytymisten tunnistamisessa (‡1287). Vuonna 2025 Anthropic alkoi myös analysoida mallien sisäisiä toimintoja keinona tutkia mallin tilannetietoisuutta ja “intenttiä” (‡2). Tämänkaltaiset menetelmät eivät kuitenkaan tällä hetkellä ole yleisiä tai tiedetä niiden olevan kilpailukykyisiä muiden arviointitekniikoiden kanssa.

Toinen lähestymistapa turvallisuuden takaamiseksi paremmin liittyy matemaattisten todistusten rakentamiseen, joiden avulla varmistetaan, että malli täyttää tietyt turvallisuusehdot (‡1177, ‡1282, ‡1288). Nämä todistukset kuitenkin olettavat, että testausympäristö vastaa käyttöönottoympäristöä, ja niitä ei ole testattu monentyyppisiä hyökkääjiä vastaan.

Niitä ei myöskään tällä hetkellä voida skaalata suuriin malleihin. Kaiken kaikkiaan asiantuntijoiden keskuudessa vallitsee merkittävä kiista siitä, mitä lupa tulkittavuuteen ja formaaliin todentamiseen liittyvistä menetelmistä todella tarjoaa.

###@ Käyttöönoton aikainen valvonta ja ohjaus

Lisäksi mallin kehityksen aikana toteutettavien suojatoimien lisäksi toinen puolustuslinja haitallista käyttäytymistä vastaan on ulkoiset suojatoimet, jotka keskittyvät mallin tai järjestelmän toiminnan valvontaan ja hallintaan käyttöönoton aikana. Tällaiset suojatoimet auttavat lieventämään toimintahäiriöitä ja väärinkäyttöä, kuten hallusinoituja tulosteita ja haitallisia ohjeita.

>white|orangered|left|14|15.5|bb Mallin käyttöönottajat voivat käyttää useita työkaluja tunnistaakseen ja käsitelläkseen korkean riskin mallikäyttäytymistä.

Kun tekoälyjärjestelmä on käynnissä, jakelija voi seurata riskin merkkejä ja puuttua asiaan, jos niitä ilmenee. Esimerkiksi he voivat tarkastaa mallin syötteitä merkkejä vastaanottavista hyökkäyksistä, suodattaa epäasianmukaista sisältöä ulostuloista tai seurata järjestelmän ajatusketjua merkkejä haitallisista suunnitelmista. Kohdat, joissa jakelijat voivat seurata ja puuttua siihen, miten ihmiset käyttävät heidän järjestelmiään, sisältävät laitteiston (‡1180, ‡1181), käyttäjien vuorovaikutukset (‡1154, ‡1166), syötteet ja ulostulot (‡65, ‡725, ‡1182), sisäiset laskelmat (‡744, ‡1183, ‡1184) sekä ajatusketjun (‡430, ‡435). Lisäksi on useita toimia, joita jakelijat voivat tehdä, kun riskejä havaitaan. Näihin kuuluvat tietojen kirjaaminen, haitallisen sisällön suodattaminen/muokkaaminen, poikkeavan toiminnan merkitseminen, järjestelmän sammutukset tai suojatoimien (failsafe) käynnistäminen. Kuva 3.7 havainnollistaa esimerkkejä yleisistä seuranta- ja ohjausmekanismeista.

Koska nämä mekanismit ovat monipuolisia ja usein tehokkaita, niitä käytetään laajasti, ja ne voivat estää monenlaisia tahattomia haittoja (‡725, ‡751, ‡1289). Nämä suojatoimet ovat kuitenkin puutteellisia, erityisesti silloin, kun niitä vastaan tehdään haitallisia hyökkäyksiä, jotka on optimoitu niiden epäonnistumisen varmistamiseksi (‡752, ‡1182). Uudempi tutkimus on lisäksi tarkastellut, kuinka valvonta voi olla epäluotettavaa, jos järjestelmää optimoidaan valvojan pisteiden perusteella, esimerkiksi heikentämällä päättelyketjun luotettavuutta (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Kuva 3.7: Seuranta- ja ohjaustekniikat
>white|black||9|11|br Valvonta- ja ohjaustekniikat toimivat useissa kohdissa: syötteiden ja tulosteiden seulonta haitallisen sisällön varalta, sisäisten mallitilojen seuraaminen, ulkoisten toimintojen rajoittaminen eristämällä ne hiekkalaatikossa sekä ihmisen toteuttaman valvonnan ylläpitäminen. Lähde: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Ihmiset silmukassa mahdollistavat suoran valvonnan korkean panoksen ympäristöissä

Vähentääkseen epäonnistumisten todennäköisyyttä AI-agenttien osalta (katso §2.2.1. Luotettavuushaasteet), järjestelmien käyttöönottajat voivat pyrkiä suunnittelemaan AI-järjestelmiä, jotka toimivat yhteistyössä ihmisten kanssa sen sijaan, että ne toimisivat täysin autonomisesti (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Tämä on tärkeää käyttötapauksissa, joissa virheelliset päätökset voivat aiheuttaa merkittävää haittaa, kuten rahoituksessa, terveydenhuollossa tai poliisitoiminnassa. Kuitenkin “ihminen silmukassa” -lähestymistapa on usein käytännössä vaikea. Joskus päätöksenteko tapahtuu liian nopeasti, kuten viestintäsovelluksissa, joissa on miljoonia käyttäjiä. Joissakin tapauksissa ihmisen ennakkoluulot ja virheet voivat lisäksi voimistaa riskejä kasautuvien virheiden vuoksi (‡1187). Ihmiset silmukassa myös taipuvat ilmentämään “automaatiokyvyn harhaa”, mikä tarkoittaa, että he usein luottavat AI-järjestelmään enemmän kuin olisi perusteltua (‡1190, ‡1191) (katso §2.3.2. Riskit ihmisen autonomialle).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ suojaa riskeiltä, jotka aiheutuvat autonomisesta toiminnasta

Verkkoympäristössä tai fyysisessä maailmassa itsenäisesti ja rajoituksetta toimivat AI-agentit aiheuttavat kohonneita riskejä (katso §2.2.1. Luotettavuushaasteet). ”Sandboxing” tarkoittaa sitä, että rajoitetaan niitä tapoja, joilla AI-agentit voivat suoraan vaikuttaa maailmaan, jolloin niitä on paljon helpompi valvoa ja hallita (‡640, ‡1192, ‡1295). Esimerkiksi rajoittamalla AI-järjestelmän mahdollisuuksia julkaista internetissä tai muokata tietokoneen tiedostojärjestelmää voidaan estää odottamattomista toimista johtuvia odottamattomia haittoja (‡1296). Nämä lähestymistavat eivät kuitenkaan aina ole käytettävissä sovelluksissa, joissa AI-järjestelmän on välttämättä toimittava suoraan maailmassa.

###@ Ekosysteemin seurantatyökalut: mallin ja datan alkuperä sekä jäljitettävyys

Malli- ja datan alkuperäselvitystyökalut ovat teknisiä työkaluja tekoälyekosysteemin tutkimiseen, jotta voidaan lisätä tietoisuutta tekoälyjärjestelmien jatkokäytöistä ja vaikutuksista.

>white|orangered|left|14|15.5|bb AI-järjestelmien alkuperän todennustekniikat auttavat jäljittämään järjestelmien käytön ja vaikutukset

Kehittäjät ja käyttöönotosta vastaavat voivat käyttää erilaisia tekniikoita mallien käytön tutkimiseen ja niiden leviämisen selvittämiseen ‘todellisessa maailmassa’. Esimerkiksi ne voivat antaa malleille yksilöllisiä tunnistettavia käyttäytymismalleja (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) tai soveltaa yksilöllisiä kuvioita yksittäisten avoimen painotuksen mallien painoihin (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Näiden tekniikoiden tekeminen entistä kestävämmiksi mallimuokkauksille on kuitenkin avoin ongelma (‡1195, ‡1196*). Tutkijat kehittävät myös menetelmiä ‘malliperimän päättelemiseksi’ (‡1197, ‡1198, ‡1305, ‡1306), joiden avulla voidaan vastata kysymyksiin, kuten: ‘Oliko malli X mallista Y hienosäädetty vai mallista Y tislattu versio?’ Lopuksi osa kehittäjistä työskentelee protokollien ja infrastruktuurin parissa, jotta tekoälyagentit voisivat olla tunnistamista ja varmennusta helpottavia, kun ne ovat vuorovaikutuksessa ulkoisten järjestelmien kanssa (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Kuva 3.8: Vesileimat upottavat huomaamattomia häiriöitä kuviin ja ääneen
>white|black||9|11|br Vesileimat upottavat kuviin ja ääniin havaitsemattomia häiriöitä, joiden avulla tekoälyllä tuotettu sisältö voidaan tunnistaa tunnistustyökaluilla. Tässä kuvassa sekä kuvan että äänen vesileimoja on liioiteltu näkyvyyden vuoksi. Lähde: Chameleon-kuva Unsplashista (‡1313*). Muut elementit: Reportin tekijät. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Kuva 3.9: Prompt-injektiohyökkäyksen onnistumisasteet
>white|black||9|11|br Prompt-injektiohyökkäysten onnistumisasteet, kuten AI-kehittäjät raportoivat suurille malleille, jotka julkaistiin välillä toukokuu 2024 ja elokuu 2025. Kukin piste kuvaa onnistuneiden hyökkäysten osuuden 10 yrityksestä tiettyä mallia vastaan pian julkaisun jälkeen. Raportoitu onnistumisaste tällaisten hyökkäysten osalta on laskenut ajan myötä, mutta pysyy edelleen suhteellisen korkeana. Lähde: Zou et al. 2025 (‡1149), lainattu lähteestä Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb AI-sisällön tunnistamistekniikat auttavat seuraamaan AI:n tuottaman sisällön leviämistä ja sen vaikutuksia

Vesileimat, metatiedot ja muut tekoälyn sisällön ilmaisimet voivat auttaa tutkijoita seuraamaan ja tutkimaan tekoälyn luoman sisällön tosimaailman vaikutuksia. 

Ensin datan vesileimat ovat huomaamattomia mutta erottuvia kuvioita, jotka upotetaan digitaaliseen mediaan ja joilla voidaan koodata tietoa niiden alkuperästä (‡1199, ‡1200, ‡1201*). Tekstissä ne tyypillisesti ovat hienovaraisia vinoumia sanavalinnoissa ja tyylissä (‡1308, ‡1309); kuvissa ja videossa hienovaraisia kuvioita pikseleissä (‡1310); ja äänissä hienovaraisia kuvioita äänen aaltomuodoissa (‡1311). Kuva 3.8 havainnollistaa tätä.

Vesileimojen lisäksi tekoälyllä tuotettua sisältöä voidaan tallentaa myös tiedostomuodoissa, jotka tallentavat metatietoa siitä, miten sisältö on tuotettu. Esimerkiksi monet mobiililaitteet tallentavat kuvia ja äänitiedostoja tiedostomuodossa, joka voi tallentaa tietoa kameran asetuksista, ajasta, sijainnista jne. (‡1312). Vastaavia metatietoja voidaan käyttää tallentamaan tietoa siitä, onko aineisto tuotettu tekoälyjärjestelmällä. Samalla tavoin kuin sormenjälkien tunnistaminen rikosteknisessä forensiikassa, vesileimoja ja metatietoja voidaan väärentää tai poistaa, mutta niistä on silti hyötyä.

Tutkijat työskentelevät myös kehittääkseen tekoälyn tuottaman sisällön tunnistimia (‡1203, ‡1204, ‡1205*) auttamaan AI:n tuottaman sisällön tunnistamisessa käytännön ympäristöissä, vaikka vesileimaa tai metatietoja ei olisi saatavilla. Näillä tunnistustekniikoilla on kuitenkin rajallinen onnistumisaste.

###@ Päivitykset

Edellisen Raportin (tammikuu 2025) julkaisemisen jälkeen on edistytty sellaisten tekoälyjärjestelmien kehittämisessä, joissa on useita tehokkaita suojakerroksia. Kuten kohdassa §3.2. Riskienhallinnan käytännöt käsitellään, puolustuksellinen kerroksittaisuus (defence-in-depth) on riskienhallinnan keskeinen periaate (‡1314). Esimerkiksi tekoälyjärjestelmiä, jotka yhdistävät turvallisuuskoulutetut mallit syötteensuodattimiin, ulostulosuodattimiin ja muihin sisällön valvontamekanismeihin, tutkitaan ja otetaan yhä useammin käyttöön (‡32, ‡65, ‡1182*). Tuore tutkimus on myös osoittanut, että vaikka mallinkehittäjät ovat edistyneet suojatoimien ohittamisyrityksiin kohdistuvan kestävyyden parantamisessa, hyökkääjät onnistuvat silti suurella osumaprosentilla (Kuva 3.9).

###@ Todisteiden puutteet

Lisää näyttöä tarvitaan auttamaan tutkijoita ymmärtämään ja huomioimaan nykyisten lähestymistapojen rajoitukset. AI-järjestelmien teknisiä suojatoimia kehitetään, mutta tekniikoissa on rajoituksia. Esimerkiksi yleiskäyttöisten AI-järjestelmien pahimman tapauksen robustisuuden parantamisessa on edetty hitaasti, ja on perustavanlaatuisia rajoituksia sille, miten perusteellisesti avoimen painon (open-weight) malleja voidaan suojata ja valvoa (‡1195, ‡1315, ‡1316) (katso myös §3.4. Open-weight models). Samaan aikaan kaikki tekniset suojatoimet eivät ole yhtä yleisiä, yhtä tehokkaita eivätkä yhtä laajasti todistettuja käytännön maailmassa. Esimerkiksi vastustajakoulutusta (adversarial training) käytetään lähes yleisesti huipputason malleissa (‡64*, ‡677), kun taas mallin tulkittavuuden ja muodollisen varmennuksen tekniikoita on tähän mennessä käytetty vain vähän tuotantojärjestelmissä (‡1177, ‡1285).

###@ Haasteet poliittisille päättäjille

Päätöksentekijöiden keskeisiä haasteita ovat muun muassa sen pohtiminen, pitäisikö ja miten niiden tulisi tukea tutkimusta, kehitystä, arviointia ja teknisten turvatoimien sekä valvontamenetelmien käyttöönottoa. Tämä on haastavaa, koska tutkijoiden käsitys siitä, mikä on käytännössä paras tapa suojata mekanismeja, on edelleen kehittymässä, eikä parhaista käytännöistä ole vielä vakiintunut. Esimerkiksi eri kehittäjät soveltavat erilaisia turvatoimia, ja heidän lähestymistapansa teknisen riskin lieventämiseen laajemmin vaihtelevat huomattavasti (‡1116). Lopuksi tehokkaiden teknisten turvatoimien olemassaolo ei yksinään takaa turvallisuutta, koska käyttöönotto ja toteutus voivat vaihdella eri kehittäjien ja käyttöönottoympäristöjen välillä.

