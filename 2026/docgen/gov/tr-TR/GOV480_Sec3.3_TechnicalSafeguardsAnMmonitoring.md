##########
>white|orangered|left|14|30|hr Bölüm 3.3
### 3.3. Teknik güvenlik önlemleri ve izleme
>white|orangered|left|24|30|hb Teknik güvenlik önlemleri ve izleme

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Temel bilgiler
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Yapay zeka geliştirme ve kullanımının farklı aşamalarında çok çeşitli teknik güvenlik önlemleri kullanılır. Bunlar; sistemleri daha sağlam ve kötüye kullanıma karşı daha dayanıklı hale getirmek için model geliştirme sırasında uygulanan teknikleri (örneğin veri kürasyonu), dağıtım- anı izleme ve kontrolünü (örneğin içerik filtreleme ve insan gözetimi) ve daha geniş yapay zeka ekosistemini izlemek için dağıtımdan sonraki araçları (örneğin köken kanıtlama ve içerik tespiti) içerir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Teknik güvenlik önlemlerinin sınırlamaları vardır ve zararlı davranışı tüm bağlamlarda güvenilir şekilde engellemez. Örneğin, kullanıcılar bazen istekleri yeniden ifade ederek veya bunları daha küçük adımlara bölerek zararlı çıktılar elde edebilir. Benzer şekilde, yapay zekâ tarafından üretilen içerikleri tespit etmek üzere tasarlanmış telif işaretleme (watermarking) gibi araçlar da çoğu zaman kaldırılabilir veya değiştirilebilir; bu da güvenilirliklerini sınırlar.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bireysel önlemlerin sınırlılıkları, bazı zararlı sonuçları önlemek için ‘savunmada derinlik’ yaklaşımının gerekli olabileceği anlamına gelir. Örneğin bir sistem, güvenlik eğitimi almış bir model ile giriş filtreleri, çıkış filtreleri ve içerik izleyicilerini birleştirebilir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Son Raporumun yayınlanmasından bu yana (Ocak 2025), araştırmacılar gözetim/koruma önlemlerini iyileştirmede ilerleme kaydetti; ancak temel sınırlamalar devam ediyor. Örneğin, gözetim/koruma önlemlerini atlatmayı hedefleyen saldırıların başarı oranı düşüyor, fakat görece yüksek kalıyor. Ayrıca, açık-ağırlıklı (open-weight) modellerin ne ölçüde kapsamlı şekilde korunabileceğine dair temel sınırlamalar da bulunmaktadır.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Politika yapıcılar için temel bir zorluk, genel amaçlı Yapay Zeka (AI) sistemlerinin farklı gerçek dünya kullanım alanlarında koruyucu önlemlerin ne kadar etkili olduğuna dair sınırlı kanıt bulunmasıdır. AI geliştiricileri, koruyucu önlemleri ve izleme faaliyetleri hakkında ne kadar bilgi paylaştıkları konusunda oldukça farklılık göstermektedir. Ek bir zorluk da, daha güçlü koruyucu önlemler uygulamak ile sistem performansını veya kullanılabilirliğini korumak arasında ortaya çıkabilecek ödünleşimlerdir.
>oldlace|black||11|15|br      


AI geliştiricileri, genel amaçlı AI sistemlerinden kaynaklanan riskleri azaltmak ve yönetmek için birkaç faydalı ama kusurlu teknik güvenlik önlemi kullanabilir; ancak sağlamlık zorlukları sürmektedir. Geliştiriciler hâlâ, genel amaçlı AI sistemlerinin suç işlemek için kullanıcılara talimat vermek gibi bilinen ve açıkça zararlı eylemleri dahi tamamen engelleyemez. Örneğin, araştırmacılar en son teknolojideki güvenlik önlemlerinin bile, düşmanca yönlendirme yöntemleriyle (yani ‘jailbreaks’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), karmaşık zararlı görevleri adımlara bölerek (‡1150, ‡1151, ‡1152, ‡1153, ‡1154) ve basit model değişiklikleriyle (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166) aşılabildiğini göstermiştir. Araştırmacılar, arızalar ve kötüye kullanım karşısında güvenlik önlemleri üzerinde çalışmaya devam etmektedir (‡690). Bu yöntemlerin amacı ve etkililiği büyük ölçüde değişir ve nihai etkileri, AI sistemlerinin geliştirildiği ve devreye alındığı daha geniş sosyoteknik ve yönetişim bağlamına bağlıdır.

Teknik güvenlik önlemleri genel olarak üç kategoriye ayrılabilir: daha güvenli modeller geliştirmeye yönelik teknikler; dağıtım sırasında izleme ve kontrol için kullanılan teknikler; ve dağıtım sonrası ekosistem izlemeyi destekleyen teknikler. Tablo 3.6, ele alınan teknik güvenlik önlemlerini, etkinliklerini ve açık zorlukları özetlemektedir.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Daha güvenli modeller geliştirme
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Veri kürasyonu (‡1167)
  Zararlı verileri kaldırarak bir modelin tehlikeli yetenekleri öğrenmesini engellemek. Bu yöntemler, zararlı yeteneklerden yoksun olan ve zararlı ince ayara (‡55) direnç gösteren açık ağırlıklı modelleri geliştirmek için de dahil olmak üzere faydalı olabilir. Ancak seçme/ayıklama hataları ve ölçekleme (‡1168) ile ilgili zorluklar vardır.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb İnsan geri bildirimiyle pekiştirmeli öğrenme (‡64*)
  Belirlenen hedeflerle uyumlu olacak şekilde modeli eğitmek; yardımcı ve zararsız olmasını sağlamak gibi. Bu, modellerin faydalı davranışları öğrenmesi için etkili bir yöntemdir (‡64*). Ancak insan onayına yönelik aşırı optimizasyon, modellerin aldatıcı ya da dalkavukça davranmasına yol açabilir (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Çoğulcu hizalama teknikleri (‡1170)
  Modeli, nasıl davranması gerektiğine dair farklı görüşleri bir araya entegre edecek şekilde eğitmek. Bu teknikler, modellerin belirli görüşleri ne ölçüde tercih ettiğini azaltmaya yardımcı olur (‡1170). Ancak bu tekniklere rağmen, insan anlaşmazlığı kaçınılmazdır ve rekabet halindeki görüşleri dengelemek için yaygın biçimde kabul gören yollar tasarlamak zordur (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Adversarial eğitimi (‡677)
  Modeli zarara neden etmeyi reddedecek şekilde eğitmek (hatta tanıdık olmayan bağlamlarda bile) ve kötü niyetli kullanıcıların saldırılarına (örn. 'jailbreaks') karşı direnç gösterecek şekilde eğitmek. Bu, modellerin kötüye kullanım girişimlerine karşı direnç göstermesi için etkili bir yöntemdir (‡1064), ancak sağlamlık (robustness) zorlukları devam etmektedir (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Makine ‘unlearning’ (‡1175, ‡1176)
  Uzmanlaşmış algoritmalar kullanarak bir modeli eğitmek, zararlı yetenekleri (ör. biyolojik tehlikelere ilişkin bilgi) aktif olarak bastırmayı amaçlar. Bu teknikler, zararlı yetenekleri modellerden hedefli bir şekilde kaldırmak için bir yol sunar (‡1175, ‡1176); ancak mevcut unutma (unlearning) algoritmaları sağlam olmayabilir ve diğer yetenekler üzerinde istenmeyen etkilere yol açabilir (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Yorumlanabilirlik ve güvenlik doğrulama araçları (‡1177)
  Modellerin belirli güvenlikle ilgili özelliklere sahip olduğunu daha titiz bir şekilde garanti etmeyi hedefleyen, tasarım ve doğrulama yöntemlerinden oluşan çeşitli bir aile. Değerlendiricilerin güvenlik konusunda daha yüksek güvenle doğrulama yapmalarını sağlar (‡1177), ancak güncel yöntemler varsayımlara dayanır ve pratikte performans açısından nadiren rekabetçidir (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb İzleme ve kontrol
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Donanıma dayalı izleme mekanizmaları (‡1179, ‡1180, ‡1181)
  Yetkili süreçlerin, güvenlik tehditlerini veya düzenleyici uyumluluğu incelemek amacıyla donanım üzerinde çalıştığının doğrulanması. Bu mekanizmalar, donanım üzerinde hangi hesaplamaların çalıştırıldığı ve kimin tarafından çalıştırıldığı konusunda benzersiz izleme yöntemleri sunar (‡1181). Ancak, donanım mekanizmaları her türlü tehdidi izleyemez ve bazı teknikler uzmanlaşmış donanım gerektirir (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kullanıcı etkileşimi izleyicileri (‡1154, ‡1166)
  Kullanıcı etkileşimlerini kötüye kullanım belirtileri açısından izlemek, geliştiricilerin kötü niyetli kullanıcılar için hizmeti sonlandırmasına yardımcı olabilir (‡1154, ‡1166). Ancak yaptırım uygulamaları istemeden güvenlik üzerine yapılan faydalı araştırmaları engelleyebilir (‡689) ve bazı kötüye kullanım biçimlerini tespit etmek zordur (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kullanıcı etkileşimi izleyicileri (‡1154, ‡1166)
  Kötü niyetli kullanım belirtileri için kullanıcı etkileşimlerini izlemek, geliştiricilerin kötü niyetli kullanıcılar için hizmeti sonlandırmasına yardımcı olabilir (‡1154, ‡1166). Ancak, yaptırım uygulamaları istemeden güvenlik alanındaki faydalı araştırmaları engelleyebilir (‡689) ve bazı kötüye kullanım biçimlerini tespit etmek zordur (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb İçerik filtreleri (‡65*, ‡725)
  Potansiyel olarak zararlı model girdilerini ve çıktıları filtrelemek, kazara zararları ve kötüye kullanım risklerini azaltmanın çok etkili bir yoludur (‡725). Ancak filtreler ek hesaplama (compute) gerektirir ve bazı saldırılara karşı savunmasızdır (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Modelin dahili hesaplama izleyicileri (‡744, ‡1183, ‡1184)
  Modellerde aldatma işaretleri veya diğer zararlı iç bilişsel biçimler için izleme yapmak, aldatmayı tespit etmede verimli bir yol olabilir (‡744, ‡1183, ‡1184). Ancak, mevcut yöntemler sağlamlık ve güvenilirlikten yoksundur (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zincir-a-kelime düşünce izleyicileri (‡430, ‡435)
  Model zincir-düşüncesi metnini yanıltıcı davranış belirtileri veya diğer zararlı akıl yürütme türleri açısından izlemek, modellerin nasıl düşündüğündeki kusurları anlamak ve fark etmek için etkili bir yoldur (‡435). Ancak bunlar güvenilmez olabilir (‡752, ‡753, ‡1186) ve eğer modeller zararsız zincir-düşünce üretmeye göre eğitilirse, yanıltıcı davranışı öğrenebilirler (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb İnsan döngüde (‡1187, ‡1188, ‡1189)
  Bazı güvenlik açısından kritik uygulamalarda sistem kararları için insan gözetimi ve geçersiz kılmalar esastır (‡1187). Ancak bu teknikler otomasyon yanlılığı ve insan karar verme hızına ilişkin sınırlamalar nedeniyle kısıtlanır (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kumanda kutulama (‡1192)
  Bir yapay zeka aracısının dünyayı doğrudan etkilemesini engellemek, verebileceği zararı sınırlamanın etkili bir yoludur (‡1192). Ancak sanal ortam/sandboxlama, sistemin bazı görevleri doğrudan yerine getirme yeteneğini sınırlar (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Ekosistem izlemeyi kolaylaştıran araçlar
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Yapay zeka modeli tanımlama teknikleri (‡1193*, ‡1194)
  Modellerin veya modellerin tek tek örneklerinin gerçek dünyadaki kullanım senaryolarında tanımlanmasını kolaylaştırmak, dijital adli bilişim ve ekosistem farkındalığına yardımcı olur (‡1195). Ancak, bu teknikler bazı türde model değişiklikleriyle (‡1196*) atlatılabilir.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb AI model mirası çıkarımı (‡1197)
  Bu teknikler, araştırmacıların AI ekosisteminde modellerin nasıl değiştirildiğini, özellikle de açık ağırlıklı modelleri nasıl etkilediğini incelemesine olanak tanır. Bunlar dijital adli bilişim ve ekosistem farkındalığına yardımcı olur (‡1198), ancak açık ağırlıklı model ekosistemini kapsamlı biçimde haritalamak için büyük ölçekli projelere ihtiyaç olacaktır (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filigranlar ve meta veriler (‡1199, ‡1200, ‡1201*)
  Bu teknikler, bir metnin, görselin, videonun, vb. AI tarafından üretilip üretilmediğini veya değiştirilip değiştirilmediğini ve hangi sistem tarafından yapıldığını tespit etmeyi kolaylaştırır. Daha iyi ekosistem farkındalığı sağlarlar (‡1199, ‡1200, ‡1201*). Ancak, içerikte yapılan bazı değişikliklerle su işaretleri ve meta veriler sahte yapılabilir veya kaldırılabilir (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Yapay zeka tarafından üretilen içerik tespiti (‡1203, ‡1204, ‡1205*)
  Yapay zeka tarafından üretilen içerik ile gerçek içerik arasında ayrım yapma konusunda kullanıcıların yeteneğini geliştirmek, dijital adli bilişim ve ekosistem farkındalığına yardımcı olur (‡1203, ‡1204). Ancak sınıflandırıcılar güvenilmez olabilir (‡1205*) ve farklı yöntemlerde performansları değişkenlik gösterebilir.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 3.6: Bu bölümde ele alınan teknik güvenlik önlemleri
>white|black||9|11|br Bu bölümde ele alınan teknik güvenlik önlemlerinin özeti; daha güvenli modeller geliştirmeye yönelik yöntemler, dağıtım zamanı izleme ve kontrol ve ekosistem izlemeyi kolaylaştırmaya yönelik teknikler olarak üçe ayrılmıştır.


###@ Daha güvenli modeller geliştirme

Genel amaçlı AI sistemlerinden kaynaklanan zararları önlemeye yönelik ilk savunma hattı, temel modeli daha güvenli hale getirmektir. Bu alt bölüm, model geliştirme süreci sırasında model parametrelerine “gömülü” olan (Figür 3.6) koruyucu önlemleri kapsar.

>white|orangered|left|14|15.5|bb Eğitim verilerini seçmek, potansiyel olarak tehlikeli yeteneklerin geliştirilmesini sınırlayabilir

Genel amaçlı yapay zeka modelleri, eğitim verilerini işledikten sonra geniş bir bilgi ve yetenek yelpazesi geliştirdikleri için özellikle faydalıdır; ancak bazı eğitim verisi türleri, potansiyel olarak tehlikeli yeteneklerin gelişiminden orantısız biçimde sorumludur. Örneğin viroloji makaleleri üzerinde eğitilmiş bir yapay zeka modeli, potansiyel olarak zararlı biyoloji görevlerinde yardım sağlama konusunda daha iyi olabilir (‡549, ‡1206*) (ayrıca bkz. §2.1.4. Biyolojik ve kimyasal riskler). Ayrıca, insan çıplaklığına ilişkin görüntüler üzerinde eğitilmiş görüntü/video üreticileri de rızasız yakın plan deepfake’ler üretmek için kötüye kullanılabilir (‡308, ‡319) (ayrıca bkz. §2.1.1. Yapay zeka tarafından üretilen içerik ve suç faaliyeti).

Eğitim verisini filtrelemek, bazı istenmeyen yeteneklere karşı etkili bir hafifletme yöntemidir (‡319, ‡1167, ‡1207, ‡1208). Ancak genel amaçlı yapay zeka modellerini eğitmek için kullanılan büyük veri kümelerini filtrelemek, yüksek maliyetler (‡1209), filtreleme hataları (‡1210) ve veri kümesinin kalitesi üzerindeki olumsuz etkiler (‡1211) nedeniyle zor olabilir. Bu zorluklar, internet metninin çok dilliliği (‡1212), içerik denetimindeki kültürel önyargılar (‡1211, ‡1213, ‡1214, ‡1215) ve belirli bir veri parçasının ‘zararlı’ olup olmadığının bağlamsal etkenlere bağlı olması (‡1216) ile daha da artar. Yine de, eğitim verisinden potansiyel olarak zararlı içeriğin filtrelenmesi, modelleri daha güvenilir biçimde güvenli hale getirmek için umut vaat eder; bu kapsamda açık ağırlıklı (open-weight) modellerin zararlı müdahalelere (tampering) karşı daha dirençli olmasını da sağlar (‡55). Eğitim verisi içerikleri ile ortaya çıkan model yetenekleri arasındaki ilişkiler henüz tam olarak anlaşılamamıştır (‡1195) ve filtrasyonun, daha dar davranışlara (‡1206, ‡1217) kıyasla bilgi birikiminin daha geniş alanlarına (‡55) uygulandığında zararlı yetenekleri sınırlamada daha etkili göründüğü anlaşılmaktadır. Daha fazla tartışma için bkz. §3.4. Açık ağırlıklı modeller.

![figure 3.6](images/fig3.6_safeguards.png)

##### Figür 3.6: Teknik önlemlerin nerede uygulanacağı
>white|black||9|11|br Teknik güvenlik önlemleri, model geliştirme sürecinin farklı aşamalarında uygulanabilir. Veri derleme (data curation), ön-eğitim ve ince ayar sırasında modellerin ne öğrendiğini şekillendirir. İnsan geri bildiriminden pekiştirmeli öğrenme ve sağlamlık eğitimi gibi eğitim-temelli yöntemler, model davranışını uyarlayabilir. Adversarial saldırılar gibi test yöntemleri, kalan güvenlik açıklarını belirler. Güvenli-tasarım (safe-by- design) algoritmaları gibi bazı teknikler birden fazla aşamayı kapsar. Kaynak: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Yardımsever ve zararsız olacak genel amaçlı yapay zeka modellerini eğitmek için kullanılan yöntemlerin çoğu esas olarak insan geri bildirimine dayanır

Yardımsever, zararsız ve dürüst olmak gibi yüksek seviye ilkelere güvenilir biçimde uyum sağlayan modelleri eğitmek ve değerlendirmek zordur. Uygulamada geliştiriciler, bunu yapay zekâ modellerini insanlardan alınan gösterimler ve geri bildirimler ile ince ayar yaparak başarmayı hedefler. Örneğin, insan geri bildirimi ile pekiştirmeli öğrenme olarak bilinen yapay zekâ modellerinin ince ayarına yönelik temel paradigma, modelleri, insan değerlendiricilerin olumlu olarak derecelendirdiği çıktılar üretmek üzere eğitmeye dayanır (‡1218). Ancak insanlardan gelen olumlu geri bildirim, faydalı davranış için kusurlu bir vekildir (‡737, ‡878, ‡1219, ‡1220) ve insan hatası ile önyargı tarafından sınırlandırılır (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Bu durum, bir dizi zorluk doğurur: İnsan geri bildirimi üzerinden pekiştirmeli öğrenme ile ince ayar yapılmış modeller bazen kullanıcıya yaranmaya yönelir; bu davranış ‘yalakalık’ (‡358, ‡740, ‡1226, ‡1227) olarak bilinir; bazı bağlamlarda faydalı, ancak diğerlerinde zararlı olabilen yanıtlar üretir (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); doğruluğu açısından değerlendirilmesi zor yanıtlar sunar (‡1233); veya faydalılığı ya da zararlılığı görüş meselesi olan eylemler gerçekleştirir (‡1234). Masa 3.7 bu tür zorluklara ilişkin örnekler sunar. Bazı araştırmalar, yapay zeka yardımıyla karmaşık görevler için çözümleri insanların daha iyi değerlendirmesine yardımcı olacak yöntemler geliştirmeyi amaçlar (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Ancak bu yöntemler şu an için sınırlı güvenilirliğe sahiptir ve günümüzdeki en gelişmiş AI modellerini eğitmekte ne ölçüde kullanıldıkları kamuya açık olarak bilinmemektedir.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sözdecilik/kolaycılık (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Açıklama:
>white|black|left|11|13|br Model yalnızca olumlu geri bildirim verir ve doğru bir 5-7-5 haiku hece yapısındaki eksikliği belirtmeyi başaramaz.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bazı eylemler bazı bağlamlarda faydalı olabilirken diğerlerinde zararlı olabilir (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Açıklama:
>white|black|left|11|13|br Biyolojik risk hakkında bilgi eğitim ve savunma amaçları için kullanılabilir; ancak kötü niyetli aktörleri bilgilendirmek için de kullanılabilir.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Doğru davranışın doğrulanması zordur (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Açıklama:
>white|black||11|13|br Bu yanıtın doğruluğunu değerlendirmek zordur; çünkü tıbbi uzmanlık gerektirir. Deneyimli bir doktor için bile, bu tür yanıtları değerlendirmek zaman ve dikkatli bir ince ayrıntı gerektirir.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb İnsanlar neyin doğru olduğu konusunda anlaşamaz (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Açıklama:
>white|black|left|11|13|br İnsanlar, doğru yanıtın ne olduğu konusunda önemli ölçüde farklı görüşlere sahiptir.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 3.7: Kullanıcı istemi ve yapay zeka model yanıtı
>white|black||9|11|br AI modellerinden faydalı eylemleri belirtmeyi ve teşvik etmeyi zorlaştıran zorluklara örnekler.


>white|orangered|left|14|15.5|bb İnsanlar her zaman neyin arzu edilir davranışlar olduğunda uzlaşmazlar; bu da rekabet eden tercihler arasında denge kurmayı gerektiren yöntemlere ihtiyaç duyulmasına yol açar.

İnsanlar, AI modellerinin hangi yanıtları veya eylemleri üretmesi veya üretmemesi gerektiği konusunda her zaman aynı fikirde değildir (‡1006). Bu durum, eylemleri ve etkileri toplumun çıkarlarıyla genel olarak uyumlu olan modeller geliştirmeyi temel olarak zorlaştırır (‡420). Bazı araştırmacılar, yapay zeka sistemlerine hangi tercihlerin yansıdığını inceler (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) ve birbiriyle rekabet eden tercihler arasında denge kurmayı hedefleyen “çoğulcu uyum” teknikleri geliştirmeye çalışır (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Örneğin, AI geliştiricileri, belirli taleplere yanıt vermeyi reddederek tartışmalı yanıtlar üretmekten kaçınan sistemler tasarlayabilir ya da ilgili bir kişi örnekleminde ortanca (medyan) görüşe uyum sağlayabilir ya da sistemleri bireysel kullanıcılara göre kişiselleştirebilir.

Bu yaklaşımlar için yaygın bir zorluk, genel olarak Yapay Zeka sistemlerinin herkesin tercihlerine eşit ölçüde uyum sağlayamaması ve bu sistemlerin aşağı yönlü toplumsal etkilerinin farklı insan gruplarını farklı şekillerde etkileyecek olmasıdır. Bazı araştırmacılar, çoğulcu uyum (pluralistic alignment) konusundaki çoğu teknik yaklaşımın sistematik önyargılar, toplumsal güç dinamikleri ve servet ile etki gücünün belirli ellerde yoğunlaşması gibi daha derin zorlukları ele almadığını ve hatta bu zorluklardan dikkati uzaklaştırdığını ileri sürmüştür (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb AI geliştiricileri, model dayanıklılığını artırmak için ‘adversarial training’ kullanır

Eğitim sırasında öğrendikleri faydalı davranışları gerçek dünya dağıtım bağlamlarına sağlam bir şekilde aktarmak için AI modellerinin güvenilirliğini sağlamak zordur. ‘Mükemmel’ bir öğrenme sinyali ile eğitilmiş modeller bile, görünmemiş tüm bağlamlara başarıyla genelleme yapamayabilir (‡738, ‡739, ‡1255, ‡1256, ‡1257). Örneğin, bazı araştırmacılar sohbet botlarının eğitim verilerinde yeterince temsil edilmeyen dillerde zararlı eylemler alma olasılığının daha yüksek olduğunu bulmuştur (‡159, ‡880, ‡1258*, ‡1259); bu durum, Küresel Güney'de ağırlıklı olarak konuşulan pek çok dili kapsar.

Son yıllarda araştırmacılar, modellerin potansiyel olarak zararlı yanıtlar üretmesini sağlamak için kullanılabilen bir dizi “adversarial attack” tekniğinden oluşan büyük bir araç takımı da geliştirdi (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Örneğin, yakın tarihli bir girişim; güncel durumdaki yapay zekâ modellerine karşı gerçekleştirilen başarılı saldırılara ait 60,000’den fazla çeşitli örneği, katılımcıların katkılarıyla (crowd-sourced) topladı; bu da modellerin şirketlerinin kabul edilebilir model davranışına ilişkin politikalarını ihlal etmesine yol açtı (‡1149). Masa 3.8, araştırmacıların modelleri zararlı taleplere uyum sağlayacak şekilde getirebildiğini gösterdiği “jailbreak” tekniklerine ilişkin örnekler sunar.

Modellerin sağlamlığını artırmanın bir yöntemi ‘adversaryal eğitim’ (‡1064) olarak bilinir. Bu yaklaşım, modelin istenmeyen şekilde davranmasını amaçlayan ‘saldırılar’ (örn. jailbreak’ler) inşa etmeyi ve modelin bu saldırıları uygun şekilde ele almasını sağlamak üzere modeli eğitmeyi içerir. Ancak adversaryal eğitim kusursuz değildir (‡1260, ‡1261). Saldırganlar, güncel en iyi (state-of-the-art) modellere karşı sürekli olarak yeni ve başarılı saldırılar geliştirebilmektedir (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Geliştiricilerin, onlara karşı eğitim verebilmek için belirli başarısızlık (failure mode) örneklerine ihtiyaç duyması (‡512, ‡1263) nedeniyle sonuç, geliştiricilerin yeni keşfedilen açıklar karşısında modelleri sürekli güncellediği ve saldırganların sürekli yeni saldırılar aradığı devam eden bir ‘kedi-fare’ oyunudur. Bazı araştırmacılar sağlamlığı artırmak için daha büyük ölçekli adversaryal eğitim (‡1264, ‡1265) veya yeni algoritmalar (‡675, ‡676, ‡1263, ‡1266, ‡1267) önermiş olsa da, modern yapay zeka sistemleri kalıcı biçimde savunmasız kalmaya devam etmektedir.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateji: Zararlı istekleri şifreli metin içinde yapın; örneğin Morse kodu (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateji: Zararlı talepler için uyumlu yanıt örnekleriyle sistemi önyükleyin (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateji: Zararlı istekleri, eğitimde muhtemelen daha az kullanılan düşük kaynaklı dillerde yapın (ör. Svahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strateji: Zararlı bir görevi birden fazla masum alt göreve ayırın (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 3.8: Jailbreak stratejileri
>white|black||9|11|br Kötü niyetli aktörler ve siber saldırı ekipleri, yapay zeka modellerinin, güvenlik önlemleri nedeniyle normalde reddedecekleri zararlı taleplere uymasını sağlamak için çeşitli türlerde “jailbreak” (kilit açma) yöntemleri kullanmıştır. Örnek çıktılar, yalnızca açıklayıcı amaçlarla Raporun yazarları tarafından yazılmıştır. Günümüzdeki en son teknolojiye sahip birçok yapay zeka modeli artık bu yöntemlerin çoğuna karşı koymaktadır; ancak yeni jailbreak teknikleri sürekli olarak bulunmaya devam etmektedir.


>white|orangered|left|14|15.5|bb ‘Unlearning’ teknikleri, belirli zararlı model yeteneklerini azaltabilir

Genel amaçlı yapay zekadan kaynaklanan riskleri azaltmaya yönelik bir başka strateji de, modelleri belirli yüksek riskli alanlarda yetenekten yoksun olacak şekilde ince ayarlamak / fine-tune etmek (‡1175, ‡1176) olabilir. Örneğin araştırmacılar, biyolojik tehditlerle ilgili yetenekleri veya çıplak insan bedenlerinin fotogerçekçi görüntülerini üretmeye ilişkin yetenekleri özellikle bastırabilen ‘makine unlearning’ algoritmaları geliştirmeye çalışmaktadır (‡903, ‡1272, ‡1273). Bu yöntemler, unlearned yeteneklerin bazı olumlu kullanımlarını sınırlama pahasına modelleri önemli ölçüde daha güvenli hale getirebilir. Zararlı alanlarda yapay zekâ modellerinin bilgisini sınırlamak, zararlı ince ayara / harmful fine-tuning karşı koyabilen ‘kurcalamaya dayanıklı’ açık ağırlıklı modelleri tasarlamanın bir yolu olarak da önerilmiştir (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Ancak şimdiye kadar bunu sağlam ve tutarlı biçimde yapmak zorlu olmuştur (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Daha fazla tartışma için §3.4. Open-weight models bölümüne bakın.

>white|orangered|left|14|15.5|bb Bazı araştırmacılar, model iç durumlarını yorumlayarak veya matematiksel doğrulama yoluyla daha güçlü güvenlik güvenceleri için yöntemler üzerinde çalışıyor.

Bazı araştırmacılar, modellerin güvenlikle ilgili özelliklerini daha titiz bir şekilde doğrulamak için yöntemler üzerinde çalışıyor. Bir yaklaşımda, araştırmacılar modellerin iç hesaplamalarını yorumlayarak ya riskleri belirlemeyi ya da modelin güvenli olduğuna dair daha ikna edici argümanlar üretmeyi amaçlıyor (‡1285, ‡1286). Örneğin, bir kavram kanıtında araştırmacılar, dil modeli iç hesaplamalarını analiz etmeye yönelik araçların değerlendiricilerin zararlı davranışları belirlemesine yardımcı olabileceğini gösterdi (‡1287). 2025 yılında Anthropic de modelin konumsal farkındalığı ve ‘niyet’ini incelemenin bir yolu olarak modelin iç bileşenlerini analiz etmeye başladı (‡2). Ancak bu tür yöntemler şu anda yaygın değil veya diğer değerlendirme teknikleriyle rekabetçi olduğu bilinmiyor.

Güvenlik konusunda daha güçlü güvenceler sağlamak için farklı bir yaklaşım, bir modelin belirli güvenlik koşullarını sağlayacağını matematiksel kanıtlarla ortaya koymaktır (‡1177, ‡1282, ‡1288). Ancak bu kanıtlar, test bağlamının dağıtım bağlamıyla eşleştiğini varsayar ve birçok tür saldırgana karşı test edilmemiştir.

Ayrıca şu anda büyük modellere ölçeklendirilemezler. Genel olarak, yorumlanabilirliğin vaadi ve biçimsel doğrulama yöntemleri konusunda uzmanlar arasında önemli bir tartışma vardır.

###@ Dağıtım-zamanı izleme ve kontrol

Model geliştirme sırasında uygulanan korumaların yanı sıra, zararlı davranışlara karşı ikinci bir savunma hattı, dağıtım sırasında bir modelin veya sistemin eylemlerini izlemeye ve kontrol etmeye odaklanan harici korumalardır. Bu tür korumalar, uydurulmuş çıktılar ve zararlı talimatlar gibi arızaların ve kötüye kullanımın etkisini azaltmaya yardımcı olur.

>white|orangered|left|14|15.5|bb Model dağıtıcıları, yüksek riskli model davranışlarını tespit etmek ve ele almak için çeşitli araçlar kullanabilir.

Bir yapay zeka sistemi çalışırken, bir dağıtıcı risk belirtileri için izleyebilir ve bunlar ortaya çıkarsa müdahale edebilir. Örneğin, kötü niyetli saldırı işaretleri için bir modelin girdilerini inceleyebilir, çıktılardan uygunsuz içeriği filtreleyebilir veya zararlı plan işaretleri için sistemin düşünce zincirini izleyebilir. Dağıtıcıların insanların sistemlerini nasıl kullandıklarını izleyebileceği ve müdahale edebileceği noktalar; donanımı (‡1180, ‡1181), kullanıcı etkileşimlerini (‡1154, ‡1166), girdileri ve çıktıları (‡65, ‡725, ‡1182), dahili hesaplamaları (‡744, ‡1183, ‡1184) ve düşünce zincirini (‡430, ‡435) içerir. Ayrıca riskler belirlendiğinde dağıtıcıların atabileceği birden fazla eylem vardır. Bunlar; bilginin kaydedilmesi, zararlı içeriğin filtrelenmesi/değiştirilmesi, olağandışı etkinliğin işaretlenmesi, sistemin kapatılması veya emniyet mekanizmalarının (failsafe) tetiklenmesini içerir. Figür 3.7, yaygın izleme ve kontrol mekanizmalarına ilişkin örnekleri göstermektedir.

Çünkü çok yönlüdürler ve çoğu zaman etkilidirler, bu mekanizmalar yaygın olarak kullanılır ve birçok türde istemeden zararların önüne geçebilir (‡725, ‡751, ‡1289). Ancak bu güvenlik önlemleri kusursuz değildir; özellikle de onları başarısız kılmak üzere optimize edilmiş kötü niyetli saldırılar altında (‡752, ‡1182). Son araştırmalar ayrıca, bir sistemin bir izleyicinin (monitor) puanları kullanılarak optimize edilmesi durumunda izleme işleminin güvenilmez olabileceğini incelemiştir; örneğin, muhakeme zincirini (chain of thought) daha az güvenilir hale getirerek (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Figür 3.7: İzleme ve kontrol teknikleri
>white|black||9|11|br İzleme ve kontrol teknikleri birden fazla noktada çalışır: zararlı içerik için girdi ve çıktıları taramak, iç model durumlarını izlemek, dış eylemleri sandboxlama ile kısıtlamak ve insan denetimini sürdürmek. Kaynak: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb İnsanların döngü içinde yer alması, yüksek riskli ortamlarda doğrudan denetim sağlar

AI ajanlarından kaynaklanan başarısızlık olasılığını azaltmak için (bkz. §2.2.1. Güvenilirlik zorlukları), dağıtım yapanlar, tamamen özerk olmak yerine insanlar ile işbirliği içinde çalışan AI sistemleri tasarlamayı hedefleyebilir (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Bu, finans, sağlık veya kolluk gibi alanlarda hatalı kararların önemli zararlara yol açabildiği kullanım senaryoları için özellikle önemlidir. Ancak, sıklıkla ‘human in the loop’ (insan döngüde) yaklaşımına sahip olmak pratik değildir. Bazen karar verme, milyonlarca kullanıcı bulunan sohbet uygulamalarında olduğu gibi çok hızlı gerçekleşir. Diğer durumlarda ise insan yanlılığı ve hatası, art arda gelen hatalardan kaynaklanan bileşim nedeniyle riskleri artırabilir (‡1187). İnsanların döngüde olduğu durumlarda da genellikle ‘otomasyon yanlılığı’ görülür; bu da insanların, hak ettiği ölçüde güven yerine çoğu zaman AI sistemine daha fazla güven duyması anlamına gelir (‡1190, ‡1191) (bkz. §2.3.2. İnsan özerkliğine yönelik riskler).

>white|orangered|left|14|15.5|bb ‘Kum havuzu’ (sandboxing), otonom davranışlardan kaynaklanan risklere karşı koruma sağlar

Web’de veya fiziksel dünyada sınırlama olmaksızın özerk olarak hareket edebilen AI ajanları, daha yüksek riskler oluşturur (bkz. §2.2.1. Güvenilirlik sorunları). ‘Korumalı alan (Sandboxing)’; AI ajanlarının dünyayı doğrudan etkileme yollarını sınırlamayı içerir ve bu sayede onları denetlemek ve yönetmek çok daha kolay hale gelir (‡640, ‡1192, ‡1295). Örneğin, bir AI sisteminin internete gönderi yapma veya bir bilgisayarın dosya sistemini düzenleme kabiliyetini kısıtlamak, beklenmeyen eylemlerden kaynaklanan beklenmedik zararların önlenmesine yardımcı olabilir (‡1296). Ancak, bu yaklaşımlar her zaman, bir AI sisteminin zorunlu olarak doğrudan dünyada eylemde bulunması gereken uygulamalar için kullanılamaz.

###@ Ekosistem izleme araçları: model ve veri kökeni

Model ve veri kökeni (provenance) araçları, AI ekosistemini incelemek için kullanılan teknik araçlardır; AI sistemlerinin aşağı akış kullanım alanlarını ve etkilerini artırılmış farkındalıkla geliştirmeye yöneliktir.

>white|orangered|left|14|15.5|bb AI sistem kökeni (provenance) teknikleri, sistemlerin kullanımlarını ve etkilerini izlemeye yardımcı olur

Geliştiriciler ve dağıtıcılar, model kullanımını incelemek ve ‘dış dünyada’ yayılımını izlemek için çeşitli teknikler kullanabilir. Örneğin, modellere özgün tanımlayıcı davranışlar kazandırabilirler (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) veya bireysel açık-ağırlıklı (open-weight) modellerin ağırlıklarına özgün desenler uygulayabilirler (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Ancak bu teknikleri model değişikliklerine karşı daha dayanıklı hâle getirmek açık bir problemdir (‡1195, ‡1196*). Araştırmacılar ayrıca ‘model mirasını (heritage) çıkarım’ etmeye (inferring model heritage) yönelik yöntemler üzerinde çalışmaktadır (‡1197, ‡1198, ‡1305, ‡1306); bu da şu tür soruların yanıtlanmasına yardımcı olur: ‘X modeli, Y modelinin ince ayar (fine-tuned) yapılmış mı yoksa distile (distilled) edilmiş mi bir sürümüdür?’ Son olarak, bazı geliştiriciler, yapay zeka ajanlarının harici sistemlerle etkileşime geçtiğinde kimlik tespiti ve doğrulamayı kolaylaştırması için protokoller ve altyapı üzerinde çalışmaktadır (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Figür 3.8: Filigranlar, görüntülere ve seslere algılanamaz bozulmalar gömer
>white|black||9|11|br Filigranlar, algılama araçlarının yapay zekâ tarafından üretilen içeriği tanımlamasına olanak tanıyan, görüntülere ve seslere fark edilmeyen düzeltmeler (perturbasyonlar) gömer. Bu figürde, görünürlük için hem görüntü hem de ses filigranları abartılarak gösterilmiştir. Kaynak: Unsplash (‡1313*) üzerindeki Chameleon görseli. Rapor yazarları tarafından oluşturulan diğer öğeler. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Figür 3.9: İstem enjeksiyonu saldırısı başarı oranları
>white|black||9|11|br Prompt enjeksiyon saldırılarının başarı oranları; May 2024 ile Ağustos 2025 arasında yayımlanan başlıca modeller için yapay zeka geliştiricileri tarafından raporlanan değerlere göre. Her bir nokta, yayımlanmasından hemen sonra verilen bir model karşısında 10 denemeye karşı başarılı saldırıların oranını temsil eder. Bu tür saldırıların bildirilen başarı oranı zamanla düşmektedir, ancak görece yüksek kalmaktadır. Kaynak: Zou et al. 2025 (‡1149), Anthropic 2025 (‡2) içinde atıf yapılmıştır.


>white|orangered|left|14|15.5|bb AI içerik algılama teknikleri, yapay zekâ tarafından üretilen içeriğin yayılımını ve etkilerini izlemeye yardımcı olur.

Su işaretleri, meta veriler ve diğer yapay zeka içerik tespit araçları, araştırmacıların yapay zeka tarafından oluşturulan içeriğin gerçek dünyadaki etkisini takip etmesine ve incelemesine yardımcı olabilir. 

İlk olarak, veri filigranları dijital medya içine yerleştirilen, kökenleri hakkında bilgi kodlayabilen gizli ama ayırt edilebilir motiflerdir (‡1199, ‡1200, ‡1201*). Metin için genellikle kelime seçimleri ve üsluptaki ince sapmalar şeklini alırlar (‡1308, ‡1309); görseller ve video için, pikseller üzerinde ince örüntüler (‡1310); ve ses için, ses dalgaları üzerindeki ince örüntüler (‡1311). Figür 3.8 bunları göstermektedir.

Su işaretleri dışında, yapay zeka tarafından üretilen içerikler, üretim şekliyle ilgili meta verileri saklayan dosya biçimleri kullanılarak da kaydedilebilir. Örneğin, birçok mobil cihaz görüntü ve ses dosyalarını, kamera ayarları, zaman, konum vb. hakkında bilgi depolayabilen bir dosya biçimiyle kaydeder. (‡1312). Benzer meta veriler, verinin bir AI sistemi tarafından üretilip üretilmediğiyle ilgili bilgileri saklamak için kullanılabilir. Tıpkı adli bilişimde parmak izi kullanımı gibi, su işaretleri ve meta veriler kurcalanabilir veya kaldırılabilir; buna rağmen yine de faydalıdır.

Araştırmacılar ayrıca, no watermark veya metadata mevcut olmasa bile, doğada AI tarafından üretilen içeriği tespit etmeye yardımcı olacak AI-üretilen içerik dedektörleri (‡1203, ‡1204, ‡1205*) geliştirmek için de çalışıyor. Ancak, bu tespit tekniklerinin başarı oranı sınırlıdır.

###@ Güncellemeler

Geçen Raporun (Ocak 2025) yayımlanmasından bu yana, birden fazla etkili güvence katmanına sahip yapay zeka sistemlerini geliştirmede ilerleme kaydedildi. §3.2. Risk yönetimi uygulamalarında tartışıldığı üzere, savunma-derinliği risk yönetiminde temel bir ilkedir (‡1314). Örneğin, güvenlik eğitimi verilmiş modelleri giriş filtreleri, çıkış filtreleri ve diğer içerik izleyicileriyle birleştiren yapay zeka sistemleri giderek daha fazla inceleniyor ve devreye alınıyor (‡32, ‡65, ‡1182*). Son araştırmalar ayrıca, model geliştiricilerin güvenceyi aşmaya yönelik girişimlere karşı sağlamlığı artırmada ilerleme kaydetmiş olmasına rağmen, saldırganların hâlâ yüksek bir oranda başarı sağladığını da göstermiştir (Figür 3.9).

###@ Kanıt boşlukları

Araştırmacıların mevcut yaklaşımların sınırlamalarını anlamasına ve hesaba katmasına yardımcı olmak için daha fazla kanıt gereklidir. Yapay zeka sistemleri için teknik önlemler geliştirilmektedir, ancak teknikler sınırlamalardan muzdariptir. Örneğin, genel amaçlı Yapay Zeka sistemlerinin en kötü durum dayanıklılığını artırmaya yönelik ilerleme yavaş olmuştur ve açık ağırlıklı modellerin ne ölçüde kapsamlı bir şekilde güvence altına alınıp izlenebileceğine dair temel sınırlamalar bulunmaktadır (‡1195, ‡1315, ‡1316) (ayrıca bkz. §3.4. Açık ağırlıklı modeller). Bu arada, tüm teknik önlemler eşit derecede yaygın değildir, eşit derecede etki sağlamaz ve gerçek dünyada eşit ölçüde kanıtlanmış değildir. Örneğin, hasım (adversarial) eğitim güncel en ileri modellerde neredeyse her yerde kullanılmaktadır (‡64*, ‡677); buna karşılık model yorumlanabilirliği ve biçimsel doğrulama teknikleri bugüne kadar üretim sistemlerinde çok az kullanılmıştır (‡1177, ‡1285).

###@ Politika yapıcılar için zorluklar

Politika yapıcılar için temel zorluklar; teknik güvenlik önlemleri ve izleme yöntemlerinin araştırılması, geliştirilmesi, değerlendirilmesi ve benimsenmesini destekleyip desteklememeye ve nasıl destekleyeceklerine karar vermeyi içerir. Bu zordur; çünkü bilim insanlarının mekanizmaları pratikte en iyi nasıl güvenceye alacaklarına ilişkin anlayışı hâlâ gelişmektedir ve en iyi uygulamalar henüz oluşturulmamıştır. Örneğin, farklı geliştiriciler farklı güvenlik önlemleri uygular ve teknik riskin azaltılmasına yönelik yaklaşımları daha geniş ölçekte büyük ölçüde değişkenlik gösterir (‡1116). Son olarak, etkili teknik güvenlik önlemlerinin varlığı tek başına güvenliği garanti etmez; çünkü benimseme ve uygulama geliştiriciler arasında ve devreye alma bağlamlarına göre farklılık gösterebilir.

