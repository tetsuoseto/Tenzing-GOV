##########
>white|orangered|left|14|30|hr Seksyon 3.3
### 3.3. Mga teknikal na pananggalang at pagsubaybay
>white|orangered|left|24|30|hb Mga teknikal na pananggalang at pagsubaybay

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Pangunahing impormasyon
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Gumagamit ng malawak na hanay ng mga teknikal na pananggalang sa iba't ibang yugto ng pagbuo at paggamit ng AI. Kabilang dito ang mga teknik na ginagamit habang binubuo ang modelo upang gawing mas matatag at mas lumalaban sa maling paggamit ang mga sistema (gaya ng pag-curate ng datos), pagsubaybay at pagkontrol habang ipinapatupad (gaya ng pagsala ng nilalaman at pangangasiwa ng tao), at mga tool pagkatapos ng deployment para subaybayan ang mas malawak na ekosistema ng AI (gaya ng pagtukoy sa pinagmulan at nilalaman).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ May mga limitasyon ang mga teknikal na pananggalang at hindi maaasahang napipigilan ng mga ito ang mapaminsalang asal sa lahat ng konteksto. Halimbawa, kung minsan ay nakakakuha ang mga user ng mapaminsalang output sa pamamagitan ng muling pagsulat ng mga kahilingan o paghahati-hati sa mga ito sa mas maliliit na hakbang. Gayundin, kadalasang naaalis o nababago ang mga tool gaya ng paglalagay ng watermark, na idinisenyo upang matukoy ang content na binuo ng AI, kaya hindi maaasahan ang mga ito.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Nangangahulugan ang mga limitasyon ng bawat pananggalang na maaaring kailanganin ang ‘depensa sa maraming antas’ upang maiwasan ang ilang mapaminsalang resulta. Halimbawa, maaaring pagsamahin ng isang sistema ang modelong sinanay para sa kaligtasan, mga filter ng input, mga filter ng output, at mga tagasubaybay ng nilalaman.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mula nang ilathala ang huling Ulat (Enero 2025), nagkaroon ng pag-unlad ang mga mananaliksik sa pagpapahusay ng mga pananggalang, ngunit nananatili ang mga pangunahing limitasyon. Halimbawa, bumababa ang rate ng tagumpay ng mga pag-atakeng idinisenyo upang malusutan ang mga pananggalang, ngunit nananatili itong medyo mataas. Mayroon ding mga pangunahing limitasyon sa kung gaano kalawak mapoprotektahan ang mga modelong open-weight.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Isang mahalagang hamon para sa mga tagapagpatupad ng patakaran ang kakulangan ng ebidensiya tungkol sa bisa ng mga pananggalang sa iba’t ibang paggamit ng mga AI system na pangkalahatang layunin sa tunay na mundo. Malaki ang pagkakaiba-iba ng mga developer ng AI sa dami ng impormasyong ibinabahagi nila tungkol sa kanilang mga pananggalang at pagsubaybay. Isa pang hamon ang posibleng mga kompromiso sa pagitan ng pagpapatupad ng mas mahihigpit na pananggalang at pagpapanatili ng performance o pagiging kapaki-pakinabang ng system.
>oldlace|black||11|15|br      


Maaaring gumamit ang mga developer ng AI ng ilang kapaki-pakinabang ngunit di-perpektong teknikal na pananggalang upang mabawasan at mapamahalaan ang mga panganib mula sa mga AI system para sa pangkalahatang layunin, ngunit nagpapatuloy ang mga hamon sa katatagan. Hindi pa rin ganap na napipigilan ng mga developer ang mga AI system para sa pangkalahatang layunin na gumawa kahit ng mga kilala na at hayagang mapaminsalang gawain, gaya ng pagbibigay sa mga user ng mga tagubilin sa paggawa ng krimen. Halimbawa, ipinakita ng mga mananaliksik na maaaring malusutan ang mga pananggalang na nangunguna sa larangan sa pamamagitan ng mga pamamaraang adversarial na pag-uudyok (ibig sabihin, mga ‘jailbreak’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), sa pamamagitan ng pagpapabuo sa mga modelo ng mga hakbang para sa mga kumplikadong mapaminsalang gawain (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), at sa pamamagitan ng mga simpleng pagbabago sa modelo (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Patuloy na gumagawa ang mga mananaliksik ng mga pananggalang laban sa mga malfunction at maling paggamit (‡690). Malaki ang pagkakaiba-iba ng mga pamamaraang ito sa layunin at pagiging epektibo ng mga ito, at nakadepende sa mas malawak na kontekstong sosyoteknikal at pangangasiwa kung saan binubuo at ipinapatupad ang mga AI system ang magiging epekto ng mga ito.

Maaaring malawakang hatiin sa tatlong kategorya ang mga teknikal na pananggalang: mga pamamaraan para bumuo ng mas ligtas na mga modelo; mga pamamaraang ginagamit sa panahon ng pag-de-deploy para sa pagsubaybay at pagkontrol; at mga pamamaraang sumusuporta sa pagsubaybay sa ekosistema pagkatapos ng pag-de-deploy. Binubuod sa Talahanayan 3.6 ang mga teknikal na pananggalang na tinalakay, ang pagiging epektibo ng mga ito, at ang mga bukas na hamon.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Pagbuo ng mas ligtas na mga modelo
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pag-curate ng datos (‡1167)
  Pag-aalis ng mapaminsalang datos upang pigilan ang isang modelo na matuto ng mga mapanganib na kakayahan. Maaaring maging kapaki-pakinabang ang mga paraang ito, kabilang ang pagbuo ng mga open-weight na modelo na walang mapaminsalang kakayahan at lumalaban sa mapaminsalang fine-tuning (‡55). Gayunman, may mga hamon sa mga pagkakamali sa pagpili ng datos at sa pagpapalawak nito (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pagkatuto sa pamamagitan ng reinforcement mula sa feedback ng tao (‡64*)
  Pagsasanay sa modelo upang umayon sa mga tinukoy na layunin, gaya ng pagiging matulungin at hindi nakapipinsala. Isa itong epektibong paraan upang matutuhan ng mga modelo ang mga kapaki-pakinabang na asal (‡64*). Gayunman, maaaring maging mapanlinlang o mapagsipsip ang mga modelo kapag labis na ino-optimize ang mga ito para makuha ang pagsang-ayon ng tao (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga teknik sa pluralistikong alignment (‡1170)
  Pagsasanay sa modelo upang pagsamahin ang maraming magkakaibang pananaw tungkol sa kung paano ito dapat kumilos. Nakakatulong ang mga teknik na ito na mabawasan ang pagkiling ng mga modelo sa mga partikular na pananaw (‡1170). Gayunman, sa kabila ng mga teknik na ito, hindi maiiwasan ang hindi pagkakasundo ng mga tao, at mahirap magdisenyo ng mga paraan ng pagtimbang sa magkakatunggaling pananaw na malawak na tatanggapin (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial na pagsasanay (‡677)
  Pagsasanay sa modelo na tumangging magdulot ng pinsala (kahit sa mga hindi pamilyar na konteksto) at lumaban sa mga pag-atake ng mga malisyosong user (hal. mga ‘jailbreak’). Epektibong paraan ito upang matulungan ang mga modelo na labanan ang mga pagtatangkang gamitin ang mga ito sa maling paraan (‡1064), ngunit nananatili ang mga hamon sa katatagan (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb ‘Paglimot’ ng makina (‡1175, ‡1176)
  Pagsasanay ng modelo gamit ang mga espesyalisadong algorithm na nilayong aktibong supilin ang mga mapaminsalang kakayahan (hal. kaalaman tungkol sa mga biyolohikal na panganib). Nag-aalok ang mga teknik na ito ng naka-target na paraan upang alisin sa mga modelo ang mga mapaminsalang kakayahan (‡1175, ‡1176), ngunit maaaring hindi matatag ang mga kasalukuyang algorithm sa pag-aalis ng kaalaman at maaari silang magkaroon ng mga hindi nilalayong epekto sa iba pang kakayahan (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga tool para sa interpretabilidad at beripikasyon ng kaligtasan (‡1177)
  Iba't ibang pamamaraan sa disenyo at beripikasyon na naglalayong magbigay ng mas mahigpit na katiyakan na taglay ng mga modelo ang mga partikular na katangiang may kaugnayan sa kaligtasan. Nagbibigay-daan ang mga ito sa mga tagasuri na makapagbigay ng mga katiyakang may mas mataas na antas ng kumpiyansa tungkol sa kaligtasan (‡1177), ngunit nakasalalay sa mga palagay ang mga kasalukuyang pamamaraan at bihira silang makipagsabayan sa pagganap sa aktuwal na paggamit (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Pagsubaybay at pagkontrol
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga mekanismo ng pagsubaybay na nakabatay sa hardware (‡1179, ‡1180, ‡1181)
  Pagpapatunay na tumatakbo sa hardware ang mga awtorisadong proseso upang pag-aralan ang mga banta sa seguridad o pagsunod sa regulasyon. Nag-aalok ang mga mekanismong ito ng natatanging paraan upang subaybayan kung anong mga pagkukuwenta ang isinasagawa sa hardware at kung sino ang nagsasagawa ng mga ito (‡1181). Gayunman, hindi nasusubaybayan ng mga mekanismo sa hardware ang lahat ng uri ng banta, at nangangailangan ng espesyalisadong hardware ang ilang pamamaraan (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga monitor ng interaksiyon ng user (‡1154, ‡1166)
  Makakatulong sa mga developer ang pagsubaybay sa mga pakikipag-ugnayan ng user upang matukoy ang mga palatandaan ng mapaminsalang paggamit at wakasan ang serbisyo para sa mga mapaminsalang user (‡1154, ‡1166). Gayunman, maaaring hindi sinasadyang makahadlang ang pagpapatupad ng mga patakaran sa kapaki-pakinabang na pananaliksik sa kaligtasan (‡689), at mahirap matukoy ang ilang uri ng maling paggamit (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga monitor ng pakikipag-ugnayan ng user (‡1154, ‡1166)
  Makakatulong sa mga developer ang pagsubaybay sa mga pakikipag-ugnayan ng user upang matukoy ang mga palatandaan ng malisyosong paggamit at wakasan ang serbisyo para sa mga malisyosong user (‡1154, ‡1166). Gayunman, maaaring hindi sinasadyang hadlangan ng pagpapatupad ang kapaki-pakinabang na pananaliksik sa kaligtasan (‡689), at mahirap matukoy ang ilang uri ng maling paggamit (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga filter ng nilalaman (‡65*, ‡725)
  Ang pagsala sa mga input at output ng modelo na posibleng makapinsala ay napakaepektibong paraan upang mabawasan ang mga hindi sinasadyang pinsala at panganib ng maling paggamit (‡725). Gayunman, nangangailangan ng dagdag na compute ang mga filter at bulnerable ang mga ito sa ilang pag-atake (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga monitor ng panloob na pagkukuwenta ng modelo (‡744, ‡1183, ‡1184)
  Ang pagsubaybay sa mga palatandaan ng panlilinlang o iba pang mapaminsalang panloob na proseso ng pag-iisip sa mga modelo ay maaaring maging mahusay na paraan upang matukoy ang panlilinlang (‡744, ‡1183, ‡1184). Gayunman, kulang sa katatagan at pagiging maaasahan ang mga kasalukuyang pamamaraan (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga monitor ng chain-of-thought (‡430, ‡435)
  Ang pagsubaybay sa teksto ng kadena ng pangangatwiran ng modelo upang matukoy ang mga palatandaan ng mapanlinlang na pag-uugali o iba pang mapaminsalang pangangatwiran ay isang epektibong paraan upang maunawaan at matukoy ang mga depekto sa pangangatwiran ng mga modelo (‡435). Gayunman, maaaring hindi ito maaasahan (‡752, ‡753, ‡1186), at kung sasanayin ang mga modelo na bumuo ng hindi nakapipinsalang kadena ng pangangatwiran, maaari silang matutong magpakita ng mapanlinlang na pag-uugali (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tao sa loop (‡1187, ‡1188, ‡1189)
  Mahalaga ang pangangasiwa ng tao at ang kakayahang balewalain ang mga desisyon ng sistema sa ilang application na kritikal sa kaligtasan (‡1187). Gayunman, nalilimitahan ang mga pamamaraang ito ng pagkiling sa automation at ng limitasyon sa bilis ng pagpapasya ng tao (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pag-sandbox (‡1192)
  Ang pagpigil sa isang AI agent na direktang maimpluwensiyahan ang mundo ay isang epektibong paraan upang limitahan ang pinsalang maaari nitong idulot (‡1192). Gayunman, nililimitahan ng paglalagay nito sa sandbox ang kakayahan ng system na direktang gawin ang ilang partikular na gawain (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Mga tool upang mapadali ang pagsubaybay sa ekosistema
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga pamamaraan sa pagtukoy ng modelo ng AI (‡1193*, ‡1194)
  Ang pagpapadali sa pagtukoy sa mga modelo, o sa mga indibidwal na instance ng mga modelo, sa mga aktuwal na kaso ng paggamit ay nakatutulong sa digital forensics at kamalayan sa ecosystem (‡1195). Gayunman, maaaring malusutan ang mga teknik na ito sa pamamagitan ng ilang uri ng pagbabago sa modelo (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Paghinuha sa pinagmulan ng modelo ng AI (‡1197)
  Nagbibigay-daan ang mga teknik na ito sa mga mananaliksik na pag-aralan kung paano binabago ang mga modelo sa ekosistema ng AI, lalo na ang mga modelong open-weight. Nakakatulong ang mga ito sa digital forensics at kamalayan sa ekosistema (‡1198), ngunit kakailanganin ng malalaking proyekto upang lubusang imapa ang ekosistema ng mga modelong open-weight (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mga watermark at metadata (‡1199, ‡1200, ‡1201*)
  Pinadadali ng mga teknik na ito ang pagtukoy kung ang isang piraso ng teksto, larawan, video, atbp. ay nilikha o binago ng AI, at kung aling sistema ang gumawa nito. Nakakatulong ang mga ito na mapahusay ang kamalayan sa ecosystem (‡1199, ‡1200, ‡1201*). Gayunman, maaaring pekein o alisin ang mga watermark at metadata sa pamamagitan ng ilang pagbabago sa nilalaman (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pagtukoy sa nilalamang binuo ng AI (‡1203, ‡1204, ‡1205*)
  Nakakatulong sa digital forensics at kamalayan sa ecosystem ang pagpapahusay sa kakayahan ng mga user na makilala ang content na binuo ng AI mula sa tunay na content (‡1203, ‡1204). Gayunman, maaaring hindi maaasahan ang mga classifier (‡1205*) at maaaring mag-iba ang performance ng mga ito sa iba’t ibang modality.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Talahanayan 3.6: Mga teknikal na pananggalang na tinalakay sa seksyong ito
>white|black||9|11|br Isang buod ng mga teknikal na pananggalang na tinalakay sa seksiyong ito, na hinati sa mga pamamaraan para makabuo ng mas ligtas na mga modelo, pagsubaybay at pagkontrol habang ipinapatupad, at mga teknik upang mapadali ang pagsubaybay sa ekosistema.


###@ Pagbuo ng mas ligtas na mga modelo

Isang unang linya ng depensa laban sa mga pinsalang dulot ng mga AI system na pangkalahatang gamit ay gawing mas ligtas ang pinagbabatayang modelo. Sinasaklaw ng subsection na ito ang mga pananggalang na “nakabaon sa mga parameter ng modelo” sa proseso ng pagbuo ng modelo (Figure 3.6).

>white|orangered|left|14|15.5|bb Maaaring limitahan ng maingat na pagpili ng datos para sa pagsasanay ang pagbuo ng mga kakayahang posibleng mapanganib.

Kapaki-pakinabang ang mga modelong AI para sa pangkalahatang layunin dahil nagkakaroon ang mga ito ng malawak na saklaw ng kaalaman at kakayahan matapos iproseso ang datos ng pagsasanay, ngunit may ilang uri ng datos ng pagsasanay na may di-katimbang na malaking ambag sa paglinang ng mga kakayahang posibleng mapanganib. Halimbawa, maaaring mas mahusay na makapagbigay ng tulong ang isang modelong AI na sinanay gamit ang mga papel tungkol sa virology sa mga gawaing may kaugnayan sa biyolohiya na posibleng makapinsala (‡549, ‡1206*) (tingnan din ang §2.1.4. Mga panganib na biyolohikal at kemikal). Bukod dito, maaari ring gamitin sa maling paraan ang mga generator ng larawan/video na sinanay gamit ang mga larawan ng mga hubad na tao upang lumikha ng mga deepfake na seksuwal at matalik na walang pahintulot (‡308, ‡319) (tingnan din ang §2.1.1. Nilalamang ginawa ng AI at kriminal na aktibidad).

Ang pagsasala sa datos ng pagsasanay ay isang mabisang paraan upang mabawasan ang ilang hindi kanais-nais na kakayahan (‡319, ‡1167, ‡1207, ‡1208). Gayunman, maaaring mahirap salain ang malalaking dataset na ginagamit sa pagsasanay ng mga AI model na pangkalahatang gamit (‡1168) dahil sa mataas na gastos (‡1209), mga pagkakamali sa pagsasala (‡1210), at mga negatibong epekto sa kalidad ng dataset (‡1211). Lalong pinatitindi ang mga hamong ito ng multilingguwal na katangian ng mga tekstong nasa internet (‡1212), mga pagkiling pangkultura sa pagmo-moderate ng nilalaman (‡1211, ‡1213, ‡1214, ‡1215), at ng katotohanang nakadepende sa mga salik sa konteksto kung ‘mapaminsala’ ang isang partikular na piraso ng datos (‡1216). Gayunpaman, nangangako ang pagsasala ng mga materyal na posibleng mapaminsala mula sa datos ng pagsasanay bilang paraan upang maging mas maaasahang ligtas ang mga modelo, kabilang ang paggawa sa mga modelong open-weight na mas lumalaban sa mapaminsalang pakikialam (‡55). Hindi pa lubos na nauunawaan ang mga ugnayan sa pagitan ng mga nilalaman ng datos ng pagsasanay at ng mga umuusbong na kakayahan ng modelo (‡1195), at tila mas mabisa ang pagsasala sa paglilimita ng mga mapaminsalang kakayahan kapag inilalapat ito sa malalawak na larangan ng kaalaman (‡55) kumpara sa mas makikitid na asal (‡1206, ‡1217). Tingnan ang §3.4. Mga modelong open-weight para sa higit pang talakayan.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figure 3.6: Saan ilalapat ang mga teknikal na pananggalang
>white|black||9|11|br Maaaring ilapat ang mga teknikal na pananggalang sa iba’t ibang yugto ng pagbuo ng modelo. Hinuhubog ng pag-aayos ng datos ang natututuhan ng mga modelo sa paunang pagsasanay at fine-tuning. Binabago ng mga pamamaraang nakabatay sa pagsasanay, gaya ng reinforcement learning mula sa feedback ng tao at pagsasanay para sa katatagan, ang pag-uugali ng modelo. Natutukoy ng mga pamamaraan ng pagsubok, gaya ng mga adversarial na pag-atake, ang mga natitirang kahinaan. Sumasaklaw sa maraming yugto ang ilang pamamaraan, gaya ng mga algorithm na safe-by- design. Pinagmulan: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Ang mga pamamaraan sa pagsasanay ng mga modelong AI para sa pangkalahatang layunin upang maging kapaki-pakinabang at hindi nakapipinsala ay pangunahing umaasa sa feedback ng tao.

Mahirap sanayin at suriin ang mga modelo upang mapagkakatiwalaang umayon sa matataas na prinsipyong gaya ng pagiging kapaki-pakinabang, hindi nakapipinsala, at tapat. Sa praktika, layunin ng mga developer na makamit ito sa pamamagitan ng pagpino ng mga modelo ng AI gamit ang mga demonstrasyon at feedback mula sa mga tao. Halimbawa, ang pangunahing paradigma sa pagpino ng mga modelo ng AI, na kilala bilang ‘reinforcement learning from human feedback’, ay nakabatay sa pagsasanay sa mga modelo upang gumawa ng mga output na positibong nire-rate ng mga annotator na tao (‡1218). Gayunman, hindi perpektong panukat ng kapaki-pakinabang na pag-uugali ang positibong feedback mula sa mga tao (‡737, ‡878, ‡1219, ‡1220), at nalilimitahan ito ng pagkakamali at pagkiling ng tao (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Nagdudulot ito ng ilang hamon: kung minsan, labis na sumasang-ayon sa gumagamit ang mga modelong pinino sa pamamagitan ng reinforcement learning mula sa feedback ng tao, isang pag-uugaling kilala bilang ‘sycophancy’ (‡358, ‡740, ‡1226, ‡1227); nagbibigay ng mga sagot na kapaki-pakinabang sa ilang konteksto ngunit nakapipinsala sa iba (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); nagbibigay ng mga sagot na mahirap suriin kung tama (‡1233); o nagsasagawa ng mga pagkilos na ang pagiging kapaki-pakinabang o nakapipinsala ay usapin ng opinyon (‡1234). Nagbibigay ang Talahanayan 3.7 ng mga halimbawa ng mga hamong ito. Layunin ng ilang pananaliksik na bumuo ng mga pamamaraan upang matulungan ang mga tao na mas mahusay na suriin ang mga solusyon sa mga komplikadong gawain sa tulong ng AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Gayunman, limitado pa sa kasalukuyan ang pagiging maaasahan ng mga pamamaraang ito, at hindi alam ng publiko kung hanggang saan ginagamit ang mga ito sa pagsasanay ng mga pinakaabanteng AI model sa ngayon.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pagsipsip/pagpapalugod (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Paliwanag:
>white|black|left|11|13|br Positibo lamang ang ibinibigay na puna ng modelo at hindi nito itinuturo na walang wastong estrukturang pantig na 5-7-5 ang haiku.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb May ilang pagkilos na nakatutulong sa ilang konteksto ngunit nakapipinsala sa iba (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Paliwanag:
>white|black|left|11|13|br Maaaring gamitin ang impormasyon tungkol sa mga biyolohikal na panganib para sa edukasyon at depensa, ngunit maaari rin itong makatulong sa mga malisyosong aktor.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mahirap beripikahin ang wastong gawi (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Paliwanag:
>white|black||11|13|br Mahirap tasahin kung tama ang sagot na ito dahil nangangailangan ito ng kadalubhasaan sa medisina. Kahit para sa isang bihasang doktor, nangangailangan ng oras at maingat na pagsusuri sa mga detalye ang pagtaya sa mga sagot na tulad nito.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Hindi nagkakasundo ang mga tao kung ano ang tama (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Paliwanag:
>white|black|left|11|13|br Malaki ang hindi pagkakasundo ng mga tao tungkol sa kung ano ang tamang tugon.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Talahanayan 3.7: Prompt ng user at tugon ng modelo ng AI
>white|black||9|11|br Mga halimbawa ng mga hamon sa pagtukoy at pagbibigay-insentibo sa mga kapaki-pakinabang na pagkilos mula sa mga modelo ng AI.


>white|orangered|left|14|15.5|bb Hindi laging nagkakasundo ang mga tao kung aling mga pag-uugali ang kanais-nais, kaya kailangan ng mga pamamaraan upang balansehin ang magkakatunggaling kagustuhan.

Hindi palaging nagkakasundo ang mga tao kung anong mga tugon o pagkilos ang dapat o hindi dapat ilabas ng mga modelo ng AI (‡1006). Dahil dito, talagang mahirap bumuo ng mga modelong ang mga pagkilos at epekto ay malawak na nakaayon sa mga interes ng lipunan (‡420). Pinag-aaralan ng ilang mananaliksik kung kaninong mga kagustuhan ang kinakatawan sa mga sistema ng AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) at nagsisikap silang bumuo ng mga teknik ng ‘pluralistikong pag-aayon’ na naglalayong balansehin ang magkakatunggaling kagustuhan (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Halimbawa, maaaring idisenyo ng mga developer ng AI ang mga sistema upang maiwasang makabuo ng mga kontrobersyal na sagot sa pamamagitan ng pagtangging sumagot sa ilang kahilingan, umayon sa pananaw na nasa gitna ng isang kaugnay na sampol ng mga tao, o iangkop ang mga sistema sa mga indibidwal na gumagamit.

Karaniwang hamon sa mga pamamaraang ito na, sa pangkalahatan, hindi kayang iayon ng mga AI system ang sarili sa mga kagustuhan ng lahat nang pantay-pantay, at magkakaiba ang magiging epekto ng mga ito sa lipunan sa iba’t ibang grupo ng mga tao. Ikinatwiran ng ilang mananaliksik na hindi natutugunan ng karamihan sa mga teknikal na pamamaraan para sa pluralistikong pagkakahanay ang mas malalalim na hamon, at maaari pa ngang ilihis ang pansin mula sa mga ito, gaya ng mga sistematikong pagkiling, dinamika ng kapangyarihang panlipunan, at konsentrasyon ng yaman at impluwensiya (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Gumagamit ang mga developer ng AI ng ‘adversarial training’ upang mapahusay ang katatagan ng modelo.

Mahirap tiyakin na matibay na naililipat ng mga modelo ng AI sa mga konteksto ng aktuwal na deployment ang mga kapaki-pakinabang na pag-uugaling natutuhan nila habang sinasanay. Kahit ang mga modelong sinanay gamit ang isang ‘perpektong’ senyal ng pagkatuto ay maaaring hindi matagumpay na makapag-generalisa sa lahat ng kontekstong hindi pa nila nakikita (‡738, ‡739, ‡1255, ‡1256, ‡1257). Halimbawa, natuklasan ng ilang mananaliksik na mas malamang na gumawa ng mga mapaminsalang pagkilos ang mga chatbot sa mga wikang kulang ang representasyon sa kanilang datos ng pagsasanay (‡159, ‡880, ‡1258*, ‡1259), kabilang dito ang maraming wikang pangunahing sinasalita sa Global South.

Sa mga nakaraang taon, nakabuo rin ang mga mananaliksik ng malawak na hanay ng mga teknik ng ‘adversarial attack’ na maaaring gamitin upang magpagawa sa mga modelo ng mga posibleng mapaminsalang tugon (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Halimbawa, sa isang kamakailang inisyatiba, nakalap mula sa madla ang mahigit 60,000 sari-saring halimbawa ng matagumpay na mga pag-atake laban sa mga makabagong modelo ng AI, na nag-udyok sa mga ito na labagin ang mga patakaran ng kanilang mga kumpanya tungkol sa katanggap-tanggap na pag-uugali ng modelo (‡1149). Ipinapakita sa Talahanayan 3.8 ang mga halimbawa ng mga teknik ng ‘jailbreak’ na ipinakitang kayang magpaayon sa mga modelo sa mga mapaminsalang kahilingan.

Ang isang paraan upang mapahusay ang katatagan ng mga modelo ay tinatawag na ‘adversarial training’ (‡1064). Kabilang dito ang pagbuo ng mga ‘pag-atake’ (hal., mga jailbreak) na idinisenyo upang kumilos nang hindi kanais-nais ang isang modelo, at pagsasanay sa modelo upang maayos na pangasiwaan ang mga pag-atakeng ito. Gayunman, hindi perpekto ang adversarial training (‡1260, ‡1261). Palaging nakakabuo ang mga umaatake ng mga bagong matagumpay na pag-atake laban sa mga modelong nangunguna sa larangan (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Dahil nangangailangan ang mga developer ng mga partikular na halimbawa ng mga uri ng pagkabigo upang makapagsanay laban sa mga ito (‡512, ‡1263), nagiging tuluy-tuloy na ‘larong pusa at daga’ ito: patuloy na ina-update ng mga developer ang mga modelo bilang tugon sa mga bagong natutuklasang kahinaan, habang patuloy namang naghahanap ang mga kalaban ng mga bagong paraan ng pag-atake. May ilang mananaliksik na nagmungkahi ng mas malawakang adversarial training (‡1264, ‡1265) o mga bagong algorithm (‡675, ‡676, ‡1263, ‡1266, ‡1267) upang mapahusay ang katatagan, ngunit nananatiling palaging mahina sa mga pag-atake ang mga makabagong sistema ng AI.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratehiya: Gumawa ng mga mapaminsalang kahilingan sa naka-encrypt na teksto, gaya ng Kodigo Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratehiya: Bigyan ang system ng mga halimbawa ng mga sumusunod sa patakaran na tugon sa mapaminsalang kahilingan (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Istratehiya: Gumawa ng mga mapaminsalang kahilingan sa mga wikang kulang- sa mga mapagkukunan na malamang na hindi gaanong ginamit sa pagsasanay (hal. Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Estratehiya: Hatiin ang mapaminsalang gawain sa maraming hindi nakapipinsalang maliliit na gawain (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Talahanayan 3.8: Mga estratehiya sa jailbreak
>white|black||9|11|br Gumamit ang mga malisyosong aktor at mga red team ng iba't ibang uri ng ‘jailbreak’ upang mapasunod ang mga modelo ng AI sa mga mapaminsalang kahilingan na karaniwan nilang tatanggihan dahil sa mga pananggalang. Isinulat ng mga may-akda ng Ulat ang mga halimbawang output para sa paglalarawan. Lumalaban na ngayon ang marami sa mga nangungunang modelo ng AI sa karamihan ng mga paraang ito, ngunit patuloy pa ring nakakahanap ng mga bagong teknik sa jailbreak.


>white|orangered|left|14|15.5|bb Maaaring mabawasan ng mga teknik sa “pag-unlearning” ang mga partikular na mapaminsalang kakayahan ng modelo.

Ang isa pang estratehiya para mabawasan ang mga panganib mula sa AI na pangkalahatang gamit ay ang pag-fine-tune sa mga modelo upang wala silang mga kakayahan sa mga partikular na domain na may mataas na panganib (‡1175, ‡1176). Halimbawa, nagsisikap ang mga mananaliksik na bumuo ng mga algorithm para sa ‘machine unlearning’ na partikular na makapipigil sa mga kakayahang may kaugnayan sa mga biothreat o sa paglikha ng mga larawang halos hindi maibukod sa mga litrato ng mga hubad na katawan ng tao (‡903, ‡1272, ‡1273). Dahil sa mga pamamaraang ito, maaaring maging higit na ligtas ang mga modelo, kapalit ng paglilimita sa ilang positibong gamit ng mga kakayahang inalis sa pagkatuto. Iminungkahi rin ang paglilimita sa kaalaman ng mga modelo ng AI sa mga mapaminsalang domain bilang paraan ng pagdidisenyo ng mga open-weight model na ‘matibay laban sa pakikialam’ at kayang lumaban sa mapaminsalang fine-tuning (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Gayunman, hanggang ngayon ay naging mahirap itong gawin sa paraang matibay laban sa iba’t ibang paraan ng pag-iwas (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Tingnan ang §3.4. Mga open-weight model para sa karagdagang talakayan.

>white|orangered|left|14|15.5|bb May ilang mananaliksik na gumagawa ng mga pamamaraan para sa mas matibay na garantiya sa kaligtasan sa pamamagitan ng pagbibigay-kahulugan sa mga panloob na estado ng modelo o sa pamamagitan ng matematikal na beripikasyon.

May ilang mananaliksik na gumagawa ng mga pamamaraan upang mas mahigpit na mapatunayan ang mga katangiang may kaugnayan sa kaligtasan ng mga modelo. Sa isang pamamaraan, nilalayon ng mga mananaliksik na bigyang-kahulugan ang mga panloob na pagkukuwenta ng mga modelo upang matukoy ang mga panganib o makabuo ng mas kapani-paniwalang mga argumento na ligtas ang modelo (‡1285, ‡1286). Halimbawa, sa isang patunay-konsepto, ipinakita ng mga mananaliksik na makatutulong ang mga tool para suriin ang panloob na pagkukuwenta ng isang modelo ng wika sa mga tagasuri upang matukoy ang mga mapaminsalang gawi (‡1287). Noong 2025, sinimulan din ng Anthropic na suriin ang mga panloob na bahagi ng modelo bilang paraan ng pag-aaral sa kamalayan ng modelo sa sitwasyon at sa ‘layunin’ nito (‡2). Gayunman, sa kasalukuyan, hindi pangkaraniwan ang mga ganitong uri ng pamamaraan at hindi rin kilalang nakapapantay ang mga ito sa ibang pamamaraan ng pagsusuri.

Kabilang sa ibang paraan upang makapagbigay ng mas matibay na mga garantiya sa kaligtasan ang pagbuo ng mga patunay sa matematika na tutugon ang isang modelo sa ilang partikular na kondisyon sa kaligtasan (‡1177, ‡1282, ‡1288). Gayunman, ipinapalagay ng mga patunay na ito na tumutugma ang konteksto ng pagsubok sa konteksto ng pag-deploy, at hindi pa nasusubok laban sa maraming uri ng mga kalaban.

Sa kasalukuyan, hindi rin mapalalaki ang mga ito upang magamit sa malalaking modelo. Sa kabuuan, malaki ang pagtatalo ng mga eksperto tungkol sa potensyal ng mga pamamaraan ng interpretability at pormal na beripikasyon.

###@ Pagsubaybay at pagkontrol habang isinasagawa ang deployment

Bukod sa mga pananggalang na ipinatupad sa panahon ng pagbuo ng modelo, ang ikalawang linya ng depensa laban sa mapaminsalang pag-uugali ay ang mga panlabas na pananggalang na nakatuon sa pagsubaybay at pagkontrol sa mga aksyon ng modelo o sistema habang ipinapatupad ito. Nakakatulong ang mga pananggalang na ito na mabawasan ang mga malfunction at maling paggamit, gaya ng mga output na naglalaman ng halusinasyon at mga mapaminsalang tagubilin.

>white|orangered|left|14|15.5|bb Maaaring gumamit ang mga tagapag-deploy ng modelo ng iba't ibang tool upang matukoy at matugunan ang mga pag-uugali ng modelo na may mataas na panganib.

Kapag tumatakbo ang isang AI system, maaaring subaybayan ng tagapag-deploy ang mga palatandaan ng panganib at makialam kung lumitaw ang mga ito. Halimbawa, maaari nilang siyasatin ang mga input ng isang modelo upang makita ang mga palatandaan ng mga adversarial na pag-atake, salain ang hindi angkop na nilalaman mula sa mga output, o subaybayan ang chain of thought ng system upang makita ang mga palatandaan ng mapaminsalang mga plano. Kabilang sa mga puntong maaaring subaybayan at pakialaman ng mga tagapag-deploy hinggil sa paggamit ng mga tao sa kanilang mga system ang hardware (‡1180, ‡1181), mga interaksiyon ng user (‡1154, ‡1166), mga input at output (‡65, ‡725, ‡1182), mga panloob na kalkulasyon (‡744, ‡1183, ‡1184), at chain of thought (‡430, ‡435). Marami ring pagkilos na maaaring gawin ng mga tagapag-deploy kapag natukoy ang mga panganib. Kabilang dito ang pagtatala ng impormasyon, pagsala/pagbabago ng mapaminsalang nilalaman, pag-flag ng abnormal na aktibidad, pagsasara ng system, o pag-activate ng mga failsafe. Inilalarawan sa Figure 3.7 ang mga halimbawa ng karaniwang mekanismo ng pagsubaybay at pagkontrol.

Dahil maraming gamit ang mga mekanismong ito at madalas na mabisa, malawakang ginagamit ang mga ito at napipigilan nila ang maraming uri ng hindi sinasadyang pinsala (‡725, ‡751, ‡1289). Gayunman, hindi perpekto ang mga pananggalang na ito, lalo na kapag nahaharap sa mga malisyosong pag-atakeng idinisenyo upang pabagsakin ang mga ito (‡752, ‡1182). Sinaliksik din ng mga kamakailang pag-aaral kung paano maaaring maging hindi maaasahan ang pagsubaybay kapag ino-optimize ang isang sistema batay sa mga iskor ng isang monitor, halimbawa, sa pamamagitan ng pagpapababa sa pagiging maaasahan ng chain of thought (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figure 3.7: Mga pamamaraan sa pagsubaybay at pagkontrol
>white|black||9|11|br Gumagana ang mga teknik sa pagsubaybay at pagkontrol sa maraming punto: sinusuri ang mga input at output para sa mapaminsalang nilalaman, sinusubaybayan ang mga panloob na estado ng modelo, nililimitahan ang mga panlabas na pagkilos sa pamamagitan ng sandboxing, at pinananatili ang pangangasiwa ng tao. Pinagmulan: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Ang pagkakaroon ng tao sa proseso ay nagbibigay-daan sa direktang pangangasiwa sa mga kritikal na sitwasyon.

Upang mabawasan ang posibilidad ng mga pagkabigo ng mga ahente ng AI (tingnan ang §2.2.1. Mga hamon sa pagiging maaasahan), maaaring sikapin ng mga nag-de-deploy na magdisenyo ng mga AI system na nakikipagtulungan sa mga tao sa halip na ganap na gumana nang nagsasarili (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Mahalaga ito para sa mga gamit kung saan maaaring magdulot ng malaking pinsala ang mga maling desisyon, gaya ng sa pananalapi, pangangalagang pangkalusugan, o pagpupulis. Gayunman, kadalasan ay hindi praktikal ang pagkakaroon ng ‘tao sa loop’. Kung minsan, napakabilis maganap ng pagpapasya, gaya sa mga chat application na may milyun-milyong user. Sa ibang mga kaso, maaaring magpalala ng mga panganib ang pagkiling at pagkakamali ng tao dahil sa sunod-sunod na pagkakamali (‡1187). Madalas ding magpakita ang mga taong nasa loop ng ‘pagkiling sa awtomasyon’, na nangangahulugang mas nagtitiwala sila sa AI system kaysa sa nararapat (‡1190, ‡1191) (tingnan ang §2.3.2. Mga panganib sa awtonomiya ng tao).

>white|orangered|left|14|15.5|bb Pinoprotektahan ng ‘sandboxing’ laban sa mga panganib na dulot ng mga autonomous na pag-uugali.

Ang mga AI agent na kayang kumilos nang awtonomo at walang limitasyon sa Web o sa pisikal na mundo ay nagdudulot ng mas mataas na panganib (tingnan ang §2.2.1. Mga hamon sa pagiging maaasahan). Ang ‘sandboxing’ ay kinabibilangan ng paglilimita sa mga paraan kung paano direktang maiimpluwensiyahan ng mga AI agent ang mundo, kaya mas nagiging madali ang pangangasiwa at pamamahala sa mga ito (‡640, ‡1192, ‡1295). Halimbawa, mapipigilan ang mga hindi inaasahang pinsalang dulot ng mga hindi inaasahang pagkilos sa pamamagitan ng paghihigpit sa kakayahan ng isang AI system na mag-post sa internet o mag-edit ng file system ng isang computer (‡1296). Gayunman, hindi palaging magagamit ang mga paraang ito para sa mga application kung saan kinakailangang kumilos nang direkta sa mundo ang isang AI system.

###@ Mga tool sa pagsubaybay ng ecosystem: pinagmulan ng modelo at datos

Ang mga tool para sa pagsubaybay sa pinagmulan ng modelo at datos ay mga teknikal na tool para pag-aralan ang ekosistema ng AI at mapalawak ang kamalayan tungkol sa mga susunod na paggamit at epekto ng mga sistema ng AI.

>white|orangered|left|14|15.5|bb Nakakatulong ang mga pamamaraan sa pagsubaybay sa pinagmulan ng mga sistema ng AI upang matunton ang mga paggamit at epekto ng mga sistema.

Maaaring gumamit ang mga developer at tagapag-deploy ng iba’t ibang pamamaraan upang pag-aralan ang paggamit at pagkalat ng mga modelo sa aktuwal na paggamit. Halimbawa, maaari silang magbigay sa mga modelo ng mga natatanging asal na nagpapakilala sa mga ito (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) o maglapat ng mga natatanging pattern sa mga weight ng mga indibiduwal na modelong may bukas na weight (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Gayunman, nananatiling isang bukas na suliranin ang pagpapatibay sa mga pamamaraang ito laban sa mga pagbabago sa modelo (‡1195, ‡1196*). Gumagawa rin ang mga mananaliksik ng mga paraan para “mahinuha ang pinagmulan ng modelo” (‡1197, ‡1198, ‡1305, ‡1306), na tumutulong sagutin ang mga tanong na gaya ng: “Isang bersiyong na-fine-tune o na-distil ba ng modelong Y ang modelong X?” Panghuli, may ilang developer na gumagawa ng mga protocol at imprastraktura para sa mga AI agent upang mapadali ang pagkilala at beripikasyon kapag nakikipag-ugnayan ang mga ito sa mga panlabas na sistema (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figure 3.8: Naglalagay ang mga watermark ng mga perturbasyong hindi mapapansin sa mga larawan at audio.
>white|black||9|11|br Naglalagay ang mga watermark ng mga perturbasyong hindi napapansin sa mga larawan at audio upang matukoy ng mga tool sa pagtukoy ang nilalamang binuo ng AI. Sa Figure na ito, pinalabis ang mga watermark sa larawan at audio upang mas madaling makita. Pinagmulan: larawan ng Chameleon mula sa Unsplash (‡1313*). Nilikha ng mga may-akda ng Ulat ang iba pang elemento. Ulat sa Kaligtasan ng AI sa Pandaigdigang Antas 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figure 3.9: Mga rate ng tagumpay ng pag-atake sa prompt injection
>white|black||9|11|br Mga rate ng tagumpay ng mga pag-atake ng prompt injection, ayon sa ulat ng mga developer ng AI para sa mga pangunahing modelong inilabas sa pagitan ng May 2024 at August 2025. Kinakatawan ng bawat punto ang proporsyon ng matagumpay na mga pag-atake sa loob ng 10 pagtatangka laban sa isang partikular na modelo, di-nagtagal matapos itong ilabas. Bumaba ang iniulat na rate ng tagumpay ng mga ganitong pag-atake sa paglipas ng panahon, ngunit nananatili itong medyo mataas. Pinagmulan: Zou et al. 2025 (‡1149), binanggit sa Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Nakakatulong ang mga pamamaraan sa pagtukoy ng nilalamang binuo ng AI na subaybayan ang pagkalat at mga epekto nito.

Makakatulong ang mga watermark, metadata, at iba pang detector ng nilalamang AI sa mga mananaliksik na subaybayan at pag-aralan ang epekto sa tunay na mundo ng nilalamang nilikha ng AI. 

Una, ang mga watermark ng datos ay banayad ngunit natatanging mga motif na ipinapasok sa digital media at maaaring mag-encode ng impormasyon tungkol sa pinagmulan ng mga ito (‡1199, ‡1200, ‡1201*). Para sa teksto, karaniwang anyo ng mga ito ang banayad na pagkiling sa pagpili ng mga salita at estilo (‡1308, ‡1309); para sa mga larawan at video, banayad na mga pattern sa mga pixel (‡1310); at para sa audio, banayad na mga pattern sa mga sound wave (‡1311). Inilalarawan ang mga ito sa Figure 3.8.

Bukod sa mga watermark, maaari ring i-save ang content na ginawa ng AI gamit ang mga format ng file na nag-iimbak ng metadata tungkol sa kung paano ito ginawa. Halimbawa, maraming mobile device ang nagse-save ng mga file ng larawan at audio gamit ang format ng file na maaaring mag-imbak ng impormasyon tungkol sa mga setting ng camera, oras, lokasyon, atbp. (‡1312). Maaaring gamitin ang katulad na metadata upang mag-imbak ng impormasyon kung ginawa ng isang AI system ang data. Gaya ng fingerprinting sa kriminalistikong pagsusuri, maaaring pakialaman o alisin ang mga watermark at metadata, ngunit kapaki-pakinabang pa rin ang mga ito.

Nagsusumikap din ang mga mananaliksik na bumuo ng mga detector ng content na nilikha ng AI (‡1203, ‡1204, ‡1205*) upang makatulong na matukoy ang content na nilikha ng AI sa aktuwal na paggamit, kahit walang watermark o metadata. Gayunman, limitado ang antas ng tagumpay ng mga pamamaraang ito sa pagtukoy.

###@ Mga update

Mula nang mailathala ang huling Ulat (Enero 2025), nagkaroon ng progreso sa pagbuo ng mga AI system na may maraming epektibong patong ng mga pananggalang. Gaya ng tinalakay sa §3.2. Mga kasanayan sa pamamahala ng panganib, pangunahing prinsipyo sa pamamahala ng panganib ang depensang may maraming patong (‡1314). Halimbawa, patuloy na pinag-aaralan at ipinapatupad ang mga AI system na pinagsasama ang mga modelong sinanay para sa kaligtasan at mga filter ng input, mga filter ng output, at iba pang tagasubaybay ng nilalaman (‡32, ‡65, ‡1182*). Ipinakita rin ng kamakailang pananaliksik na, bagama't umunlad ang mga developer ng modelo sa pagpapahusay ng katatagan laban sa mga pagtatangkang lampasan ang mga pananggalang, matagumpay pa rin ang mga umaatake sa mataas na antas (Figure 3.9).

###@ Mga kakulangan sa ebidensya

Mas maraming ebidensiya ang kailangan upang matulungan ang mga mananaliksik na maunawaan at maisaalang-alang ang mga limitasyon ng mga kasalukuyang pamamaraan. Pinagbubuti ang mga teknikal na pananggalang para sa mga AI system, ngunit may mga limitasyon ang mga teknik. Halimbawa, mabagal ang pag-usad sa pagpapahusay ng tibay sa pinakamasamang sitwasyon ng mga AI system na pangkalahatang gamit, at may mga pundamental na limitasyon sa kung gaano kapakahusay mapoprotektahan at masusubaybayan ang mga modelong may bukas na timbang (‡1195, ‡1315, ‡1316) (tingnan din ang §3.4. Mga modelong may bukas na timbang). Samantala, hindi pare-pareho ang karaniwan, bisa, o antas ng pagsubok sa totoong mundo ng lahat ng teknikal na pananggalang. Halimbawa, halos pangkalahatang ginagamit ang adversarial training sa mga makabagong modelo (‡64*, ‡677), samantalang kakaunti pa lamang ang paggamit ng mga teknik sa interpretability ng modelo at pormal na beripikasyon sa mga production system (‡1177, ‡1285).

###@ Mga hamon para sa mga tagagawa ng patakaran

Kabilang sa mga pangunahing hamon para sa mga tagapagpatupad ng patakaran ang pagpapasya kung dapat nilang suportahan, at kung paano nila susuportahan, ang pananaliksik, pagpapaunlad, pagsusuri, at paggamit ng mga teknikal na pananggalang at pamamaraan ng pagsubaybay. Mahirap ito dahil patuloy pang umuunlad ang pag-unawa ng mga siyentipiko sa pinakamahusay na paraan upang maisagawa ang mga mekanismo ng pananggalang, at hindi pa naitatatag ang pinakamahuhusay na kasanayan. Halimbawa, magkakaiba ang mga pananggalang na ginagamit ng iba’t ibang developer, at malaki rin ang pagkakaiba-iba ng kanilang mga pamamaraan sa pagpapagaan ng teknikal na panganib sa mas malawak na saklaw (‡1116). Panghuli, hindi sapat ang pagkakaroon ng mga epektibong teknikal na pananggalang upang matiyak ang kaligtasan, dahil maaaring mag-iba ang paggamit at pagpapatupad ng mga ito depende sa developer at sa konteksto ng deployment.

