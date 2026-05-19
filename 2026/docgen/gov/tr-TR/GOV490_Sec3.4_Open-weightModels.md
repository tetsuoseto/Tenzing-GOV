##########
>white|orangered|left|14|30|hr Bölüm 3.4
### 3.4. Açık ağırlıklı modeller
>white|orangered|left|24|30|hb Açık ağırlıklı modeller

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Temel bilgiler
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ AI şirketlerinin modellerinin ‘ağırlıklarına’ sağladığı erişim düzeyi, bu modellerin oluşturduğu riskleri etkiler. Ağırlıklar, AI modellerinin girdileri işleyip çıktılar üretmesini sağlayan matematiksel parametrelerdir. Belirli bir model için şirketler, ağırlıkları tamamen özel tutmayı, bazı kullanıcılara sınırlı erişim vermeyi ya da herkesin bunları eksiksiz olarak indirebilmesine izin vermeyi seçebilir. Ağırlıkları kamuya açık olan modeller ‘open-weight modeller’ olarak adlandırılır.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Açık ağırlıklı modeller araştırma ve inovasyonu kolaylaştırır, ancak güvenlik önlemleri daha kolay kaldırılabilir. Dünyanın dört bir yanında, çeşitli aktörler – özellikle de daha az kaynağa sahip olanlar – araştırma ve ticari amaçlarla açık ağırlıklı modelleri kullanabilir. Ancak, kapalı ağırlıklı modellere kıyasla açık ağırlıklı modeller, potansiyel olarak zararlı davranışlar sergileyecek şekilde daha kolay değiştirilebilir ve  daha zordur.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Açık-ağırlık model yayınları geri alınamaz. Yayınlandıktan sonra model ağırlıkları geri çağırılamaz. Bu, tehlikeli yeteneklere sahip bir modelin yayınlanmasından kaynaklanabilecek olası zararları azaltmayı zorlaştırır.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Son Rapor’un yayınlanmasından (Ocak 2025) bu yana, büyük açık-ağırlık (open-weight) sürümler, önde gelen kapalı (closed) modellere karşı olan yetenek farkını daralttı. Çinli geliştiriciler DeepSeek ve Alibaba sırasıyla R1 ve Qwen modellerini yayınladı; bu modeller, önde gelen kapalı modellere benzer performans elde etti. Bu arada OpenAI, 2019’dan bu yana ilk açık-ağırlık modellerini yayınladı. Önde gelen kapalı modellerin yeteneklerinin, önde gelen açık-ağırlık modellerden başlıca AI kıyaslamalarında (benchmarks) bir yıldan daha az bir süre ileride olduğu tahmin ediliyor.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Temel politika zorluklarından biri, açık-ağırlıklı (open-weight) modellerin sağladığı faydalara erişimi sağlarken, kendine özgü risklerini yönetebilmektir. Yaklaşımlardan biri, açık-ağırlıklı modelleri ‘marjinal risk’ açısından değerlendirmektir: onların yayımlanmasının, halihazırda var olan modellerin ya da diğer teknolojilerin zaten oluşturduğu toplumsal riske kıyasla toplumsal riski karşı-olgusal (counterfactually) olarak ne ölçüde artırdığı. Ancak bu uygulamada karmaşıktır. Zaman içinde marjinal riskteki küçük artışlar da genel riskte zamanla önemli artışlara dönüşebilir.
>oldlace|black||11|15|br      


Açık ağırlıklı modeller; parametreleri indirmeye sunulduğu için pek çok, önceki bölümlerde ele alınan zorluklar açısından ayırt edici sonuçlar doğurur. Bir yapay zeka modelinin “ağırlıkları”, kullanıcılar için faydalı yanıtlar üretmesini sağlayan kritik bilgiyi içerir. Yayınlandıktan sonra bu ağırlıklar geri çağrılamaz: herkes kendi bilgisayarlarında veya bulut hesaplarında indirip inceleyebilir, değiştirebilir, paylaşabilir ve kullanabilir. Ağırlıklar açık olduğunda, başkaları modelin üzerine daha kolay inşa edebilir ve onu değiştirebilir; böylece çeşitli ihtiyaçlara hizmet edilir ve inovasyon hızlanır (‡1317). Bununla birlikte, aynı mekanizma kötü niyetli kullanıcıların da güvenlik önlemlerini kaldırmasını ve açık ağırlıklı modelleri zararlı kullanım senaryoları için değiştirmesini daha kolay hale getirir (‡1122, ‡1160). Bu da, bazı açık ağırlıklı modellerin özel gereksinimlere (örn. yayından önce daha katı testler) tabi tutulup tutulmaması gerektiği ya da tersine özel muafiyetler (örn. düzenleyici raporlama gerekliliklerinden muafiyet) verilmesi gerekip gerekmediği sorusunu gündeme getirmiştir (‡1033).

###@ Açık ağırlıklı modellere ilişkin arka plan

>white|orangered||14|15.5|bb Açık-ağırlıklı modeller açık kaynak olabilir, ancak mutlaka açık kaynak olmak zorunda değildir.

‘Açık kaynak’ olarak sıkça anılsa da, kamuya açık şekilde yayımlanan çoğu model daha doğru bir ifadeyle ‘açık ağırlık (open-weight)’ olarak tanımlanır. Bunun nedeni, geliştiricilerin model ağırlıklarını sağlasına karşın, ilişkili eğitim kodunu veya veri kümelerini yayımlamamasıdır. Ayrıca, açık kaynak yazılımı genellikle, yazılımı kullanan veya değiştiren alt aktörler üzerinde asgari düzeyde gereklilikler getiren izin verilebilir lisanslara sahip olmasıyla karakterize edilir (‡1318). Örneğin Meta’nın Llama modelleri kısıtlayıcı lisans koşullarına sahiptir ve yalnızca çıkarım (inference) kodunu içerir; eğitim kodunu içermez. Bu nedenle genellikle açık kaynak olarak değerlendirilmez (‡1319, ‡1320). Model yayımlama seçenekleri, tamamen kapalıdan tamamen açık kaynağa kadar bir spektrum üzerinde yer alır; her noktada farklı risk-fayda dengelemeleri bulunur (‡1086*, ‡1320, ‡1321). Masa 3.9 bu seçenekleri açıklar.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Tamamen kapalı
  Kullanıcılar modele hiç doğrudan etkileşime giremez
  Örnekler: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Barındırılan erişim
  Kullanıcılar yalnızca belirli bir uygulama veya arayüz üzerinden etkileşime girebilir; örneğin bir mobil chatbot uygulaması gibi
  Örnekler: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Modele API erişimi
  Kullanıcılar, kod aracılığıyla modele istek gönderebilir; bu da harici uygulamalarda kullanılmasına olanak tanır.
  Örnekler: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb İnce ayar için API erişimi
  Kullanıcılar, modeli kendi ihtiyaçlarına göre ince ayar yapabilir
  Örnekler: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Açık ağırlık: indirilebilir ağırlıklar mevcuttur
  Kullanıcılar modeli kendi bilgisayarlarında indirebilir ve çalıştırabilir
  Örnekler: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb İndirilebilir ağırlıklar, veriler ve kod; kullanım kısıtlamaları ile birlikte
  Kullanıcılar modeli indirebilir ve çalıştırabilir; ayrıca çıkarım ve eğitim kodlarını da indirebilir ve çalıştırabilir, ancak kullanımlarına ilişkin bazı lisans kısıtlamaları vardır
  Örnekler: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tamamen açık: ağırlıklar, veriler ve kod indirmeye hazır ve herhangi bir kullanım kısıtlaması yok
  Kullanıcıların modelin, tam kodun ve verinin tamamını indirme, kullanma ve değiştirme konusunda tam özgürlüğü vardır
  Örnekler: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 3.9: Tamamen kapalıdan tamamen açıkya kadar uzanan model paylaşım seçenekleri
>white|black||9|11|br Model paylaşım seçeneklerinin örnek bir seçimi; tamamen kapalı modellerden (modeller özel tutulur ve yalnızca tescilli kullanım için elde bulundurulur) tamamen açık ve açık kaynaklı modellere (model ağırlıkları, veri ve kod; kullanım, değiştirme ve paylaşım kısıtlaması olmaksızın serbest ve kamusal olarak mevcuttur) kadar uzanır. İlk dört kategoride yer alan modeller çoğunlukla ‘kapalı’ olarak adlandırılır. Bu bölüm, en alttaki üç satıra odaklanır. Kaynak: Bommasani, 2024 (‡1317) uyarlanmıştır.


###@ Faydalar ve riskler

>white|orangered|left|14|15.5|bb Açık ağırlıklı modeller daha kolay özelleştirilebilir ve değerlendirilebilir

Açık-ağırlıklı modeller, araştırma, yenilik ve erişim açısından önemli faydalar sunar. §1.1’de tartışıldığı gibi Genel amaçlı yapay zeka nedir? genel amaçlı yapay zeka modellerini eğitmek son derece pahalıdır – önde gelen modellerin geliştirilmesi için yüz milyonlarca dolar gerekir. Model ağırlıklarını açık şekilde yayımlamak, daha az kaynağa sahip aktörlerin mevcut sistemleri kopyalamasına, incelemesine ve bunların üzerine inşa etmesine olanak tanır. Böyle bir erişim olmadan, düşük kaynaklı bölgelerdeki topluluklar AI’nin faydalarından dışlanma riskiyle karşı karşıya kalır; bu nedenle, AI geliştiriminde küresel çoğunluğun katılımını mümkün kılmak için açık ağırlıklar kritik önemdedir (‡1322). İleri seviye geliştiriciler, modelleri çeşitli uygulamalar için ince ayar yapabilir; örneğin, onları az kaynaklı azınlık dillerine uyarlamak veya hukuki metin taslağı hazırlama ya da tıbbi not alma gibi belirli görevler için performansı optimize etmek (‡1323, ‡1324*). Bu sayede, açık-ağırlıklı modeller, aksi mümkün olmayacak olandan daha fazla insanın ve topluluğun AI’yi kullanmasını ve ondan faydalanmasını sağlayabilir (‡1325). Tehlikeli olacak kadar yeterli olmayan modeller söz konusu olduğunda, bu faydalar ağırlıkların açık şekilde yayımlanmasına ilişkin ek riski dengeleyebilir; ancak bu, ilgili karar vericilerin risk toleransına bağlıdır.

Açık-ağırlık sürümü, modeli inceleyebilen, yeteneklerini değerlendirebilen, güvenlik açıklarına test edebilen ve iyileştirmeler üzerinde yineleme yapabilen geliştirici ve araştırmacı havuzunu da genişletir (‡1326, ‡1327). Bu, faydalı uygulamaların ve zararlı kusurların belirlenme olasılığını artırır; ancak bu garanti değildir (‡1328, ‡1329). Kullanıcılar ayrıca açık-ağırlıklı modelleri kendi cihazlarında çalıştırabilir; böylece hassas veriler üzerinde kontrolü korur ve bunu üçüncü taraf sunuculara göndermekten kaçınır.

Geliştiricilerin eğitim verileri, kod, değerlendirme araçları ve dokümantasyonun yanı sıra model ağırlıklarını da (‡1320, ‡1330, ‡1331, ‡1332*) paylaşması durumunda ek faydalar vardır. Daha fazla bilgiyle, sonraki geliştiriciler ve diğer araştırmacılar açık ağırlıklı modelleri daha iyi anlayabilir ve onları yeni uygulamalara uyarlayabilir.

>white|orangered|left|14|15.5|bb Açık ağırlıklı modellerin güvenlik önlemleri daha kolay kaldırılabilir, bu da potansiyel kötü niyetli kullanıma olanak tanır

Açık-ağırlıklı (open-weight) modeller ayrıca, güvenlik önlemlerinin kaldırılmasının daha kolay olması nedeniyle ek riskler doğurur. Hem açık-ağırlıklı hem de kapalı modeller zararlı kullanıcı isteklerini reddetmek için güvenlik önlemleri içerebilir; ancak bu güvenlik önlemleri açık-ağırlıklı modellerde çok daha kolay kaldırılır. Kötü niyetli aktörler, zararlı uygulamalar için performansını optimize edecek şekilde bir modeli ince ayar (fine-tune) yapabilir, zararlı kullanımları önlemek üzere tasarlanmış kod bölümlerini kaldırabilir veya önceki güvenlik ince ayarını geri alabilir (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Sonuç olarak, açık model ağırlıkları, §2.1’de tartışılan kötüye kullanım risklerini daha da artırabilir. Kötü niyetli kullanım kaynaklı riskler; gözetim olmaksızın daha fazla aktörün mevcut yeteneklerden yararlanmasını ve onları kötü amaçlı kullanım için geliştirmesini mümkün kılarak artar (‡1122, ‡1315). Birçok kullanıcının açık-ağırlıklı modellerdeki güvenlik önlemlerini kaldıracak beceriye veya teşvike sahip olmayacağı doğru olsa da, yüksek motivasyonlu kötü niyetli aktörler bir endişe kaynağıdır. Ayrıca kötü niyetli aktörler, açık-ağırlıklı modelleri kullanarak benzer kapalı modellerdeki zafiyetleri tespit edebilme imkanına da sahip olabilir (‡1055*). Bu tür kusurlar, yalnızca kapalı modelleri çalıştırmaya kıyasla daha zor bulunur; çünkü kapalı-model sağlayıcılarının uygulayabildiği daha fazla kontrol ve izleme tedbirleri vardır.

>white|orangered|left|14|15.5|bb Model ağırlıklarının paylaşılması geri alınamaz

Model ağırlıkları kamuya açık olarak indirilebilir hale getirildikten sonra, tüm mevcut kopyaların tamamına yönelik toplu bir geri alma (rollback) işlemini uygulamanın bir yolu yoktur. GitHub ve Hugging Face gibi internet barındırma platformları, modelleri platformlarından kaldırabilir; bu da bazı aktörlerin indirilebilir kopyaları bulmasını zorlaştırır ve birçok gündelik kötü niyetli kullanıcı için önemli bir engel oluşturur (‡1339). Ancak model indirilmiş ve başka bir yerde yeniden barındırılmış ya da yerel olarak saklanmışsa, kararlı aktörler yine de kopyalara ulaşabilir. Ayrıca açık-ağırlık modellerini sistemlerine entegre eden alt seviye (downstream) geliştiriciler de, örneğin düşmanca saldırılara (adversarial attacks) karşı savunmasızlık gibi (‡1055) veya izleme sistemlerini atlatmaya yönelik model yetenekleri gibi (bkz. §2.2.2. Kontrol kaybı) kusurları devralır (‡1315). Evrilmiş (kapalı) modellerde barındırıcılar düzeltmeleri evrensel olarak devreye sokabilse de, açık-ağırlık modeli geliştiricileri güncellemelerin kullanıcılar tarafından benimseneceğini garanti edemez.

###@ Güncellemeler

Son önceki Raporun (Ocak 2025) yayımlanmasından bu yana, önde gelen açık-ağırlıklı ve kapalı modeller arasındaki yetenek açığı daraldı. Çinli geliştiriciler, özellikle açık-ağırlıklı model sağlayıcıları açısından giderek daha önemli hale geldi. Ocak 2025’te DeepSeek, bir dizi kıyaslamada (‡1340) OpenAI’ın o1’iyle benzer performans sergileyen R1 modelini yayımladı. Alibaba’nın Qwen modelleri de benzer şekilde ivme kazandı; Chatbot Arena’da, yaygın olarak kullanılan bir performans kıyaslamasında, Ağustos 2025 itibarıyla açık-ağırlıklı bir model için ilk sırayı aldı (‡1341, ‡1342*). Ağustos 2025’te OpenAI, 2019’da GPT-2’nin yayımlanmasından bu yana ilk kez gpt-oss-120b ve gpt-oss-20b olmak üzere açık-ağırlıklı modellerini yayımladı. Meta, açık ağırlıklarla Llama modellerini yayımlamaya devam etti. Önde gelen kapalı modellerin yeteneklerinin, önde gelen açık modellere kıyasla önde gelen yapay zeka kıyaslamalarında artık bir yıldan daha az bir süre geride olduğu tahmin ediliyor (Figür 3.10).

###@ Kanıt boşlukları

Önemli bir kanıt boşluğu, açık-ağırlık modellerinin kötüye kullanılmasını önlemeye yönelik teknik çözümlerin gerçek dünyadaki etkinliğine ilişkindir. Araştırmacılar, modelleri kurcalamaya (tamper) karşı dayanıklı hale getirmek için çeşitli yaklaşımlar önermiştir. Bu; zararlı değişikliklere karşı dirençli olacak şekilde tasarlanan yeni eğitim tekniklerini (‡1276), eğitim verisinden zararlı içeriğin filtrelenmesini (‡55) ve jailbreak’lere yönelik savunmaları (‡675, ‡676) içerir. Bu teknikler artık büyük geliştiricilerin gerçek dünya sürümlerinde benimsenmektedir. Örneğin OpenAI, gpt-oss modellerinde bu yaklaşımlardan bazılarını kullanmış; düşmanca (adversarial) şekilde ince ayar yapılan sürümlerin yüksek yetenek eşiğine ulaşmadığını bildirmiştir (‡1344*). Ancak araştırmalar, kötü niyetli kişilerin zararlı örnekler üzerinde yeniden eğiterek güvenlik önlemlerini devre dışı bırakabildiğini göstermiştir (‡1345, ‡1346). Ayrıca, güvenlik önlemlerinin dayanıklılığını güvenilir biçimde değerlendirmek hâlâ zordur; bu da gerçek dünyadaki saldırılara karşı etkinliklerinin belirsiz olmasına yol açar (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Figür 3.10: Önde gelen açık-ağırlıklı ve kapalı yapay zeka modelleri arasındaki yetenek açığı
>white|black||9|11|br  Epoch Yetenekler Endeksi (ECI) puanları, en iyi performans gösteren açık-ağırlıklı (koyu mavi) ve kapalı (açık mavi) modellerin zaman içindeki değişimini gösterir. ECI, 39 ölçütten gelen puanları tek bir genel yetenek ölçeğinde birleştirir. En iyi açık-ağırlıklı modeller, kapalı modellerin yaklaşık bir yıl gerisindedir. Kaynak: Epoch AI, 2025 (‡1343).


###@ Azaltımlar

Açık ağırlıklı model risklerine yönelik teknik azaltımlar, Yapay Zeka geliştirme ve devreye alma süreci boyunca işler (‡1141, ‡1195, ‡1347). Örneğin modeller geliştirilirken geliştiriciler ve aşağı akım uyarlayıcılar, zararlı yetenekleri en aza indirmek için eğitim verisinden hassas içerikleri filtreleyebilir. Bir modelin eğitim verisinden zararlı örneklerin kaldırılması, eğitim sonrasında eklenen savunmalardan 10 kat daha etkili biçimde düşmanca ince ayarı engelleyebilir; ancak bu, faydalı yetenekleri de etkileyebilir (‡55). Yapay zeka uygulama sağlayıcıları ayrıca olay bildirim ve yanıt mekanizmaları uygulayabilir (‡1348).

Ayrıca HuggingFace ve GitHub gibi barındırma platformları, zararlı amaçlarla değiştirilmiş modelleri kaldırmak için platform hizmet şartları oluşturabilir (‡1141, ‡1324). Model geliştiricileri, yayından önce denetçilere tam erişim sağlayabilir veya bir “kademeli” yayın stratejisi seçebilir; modelleri giderek daha büyük gruplara kademeli olarak yayınlarlar (‡1086). Bu, bir model yaygın olarak erişilebilir hale gelmeden önce olası arızaları veya güvenlik açıklarını tespit etmeye yardımcı olabilir (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Not 3.1: Model ağırlık güvenliği
>oldlace|black|left|13|15|hb Not 3.1: Model ağırlık güvenliği
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bu bölümde ele alınan riskler, model ağırlıklarının kasıtlı olarak yayıtıldığını varsayar. Ancak kapalı model ağırlıkları, hırsızlık veya sızıntı yoluyla da erişilebilir hale gelebilir. Kapalı modellerin geliştirilmesi yüzlerce milyon dolar maliyet gerektirir (§1.1. What is general-purpose AI?) ve ortalama olarak, açık-ağırlıklı modellere (‡1343) göre daha yeteneklidir. Bu durum, lider AI modellerini elde etmek isteyen amatör bilgisayar korsanlarından devlet aktörlerine kadar uzanan çeşitli aktörler için onları cazip hedefler haline getirir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Çalınmış kapalı model ağırlıkları, açık ağırlıklı modeller için yukarıda açıklananlarla benzer riskler doğurur; ancak olasılıkla bu risklere karşı uygulanan herhangi bir önlem bulunmadan. Kötü niyetli aktörler, en yetenekli modellerden güvenlik önlemlerini kaldırabilir. Meşru geliştiricilerin aksine, bu tür aktörler; şu anda sınırda yapay zeka şirketlerini modellerini güvenli şekilde dağıtmaya yönelten itibar, hukuki veya ticari kısıtlarla karşı karşıya kalmaz.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Mevcut güvenlik seviyeleri sektöre göre değişir ve gelişmiş saldırganlara karşı yetersiz kalabilir. Bazı geliştiriciler, siber suç şebekelerine ve içeriden tehditlere karşı model ağırlıklarını güvence altına almaya (‡582) kararlıyken, diğerleri herhangi bir kamuya açık güvenlik taahhüdünde bulunmamıştır (‡1109, ‡1349). Araştırmalar, yapay zeka veri merkezlerinin en gelişmiş ve yeterli kaynaklara sahip aktörlerin saldırılarına karşı koyamayabileceğini göstermektedir (‡582, ‡1350, ‡1351). Aralık 2025 itibarıyla, model ağırlığı hırsızlığına dair doğrulanmış ve kamuya açık şekilde belgelenmiş hiçbir olay bulunmamaktadır. Bununla birlikte, önde gelen yapay zeka şirketlerinde raporlanan başka güvenlik ihlalleri de vardır; bunlar arasında Microsoft’un e-posta sistemlerine yapılan bir sızma da yer almaktadır (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bu güvenlik açıklarını kapatmak; donanım, yazılım, personel ve tesis güvenliği için önemli yatırımlar gerektirecektir. Bazı güvenlik iyileştirmeleri, koordineli bir çabayla nispeten hızlı bir şekilde uygulanabilir (‡1122). Ancak diğer bazı kritik önlemler; donanım tedarik zincirlerinin ve tesislerin güvence altına alınması gibi, büyük olasılıkla yıllar alacaktır (‡1122). Özel şirketler ayrıca tek başına yeterli korumaları geliştirmek için kaynaklara veya bilgilere sahip olmayabilir. Örneğin, yapay zeka geliştiricileri; hükümetlerin sahip olduğu (‡1349, ‡1353*) sınıflandırılmış tehdit istihbaratına erişime sahip değildir.
>oldlace|black||11|15|br      


###@ Politika yapıcılar için zorluklar

Politika yapıcılar için temel bir zorluk, önemli ölçüde riski artırmadan açık-ağırlık model paylaşımının faydalarını güvence altına almaktır. Yıkıcı zararları önlemek için açık-ağırlık modellerin geliştiricileri, kötü niyetli aktörlerin modelleri ince ayar yapıp güvenlik korumalarını kaldırabilmesi nedeniyle, kapalı modeller için kullanılan yerleşik değerlendirme yöntemlerini kullanarak değerlendirmenin yanı sıra ek testler yapmadan modelleri yayımlamamalıdır. Uygulamada bu durum zor olabilir; çünkü yetenek geliştirmeleri öngörülemez olabilir, açık-ağırlık yayımları geri alınamaz ve bir yayımlamanın önemli düzeyde potansiyel zarara yol açıp açmayacağını öngörebilmek için değerlendirme çabaları gerekir.

Bir yaklaşım, açık yayımların ‘marjinal risk’ini değerlendirmektir: yayımlamanın, halihazırda var olan modellerin veya diğer teknolojilerin oluşturduğu toplumsal riskin ötesinde toplumsal riski karşı-olgusal olarak (counterfactually) ne ölçüde artırdığı. (‡556, ‡1033, ‡1354, ‡1355) (bkz. §3.2. Risk yönetimi uygulamaları). Ancak bir sistem devreye alındıktan sonra, aşağı akışta (downstream) riski nasıl artırıp azaltacağını tahmin etmek karmaşık ve duruma bağlıdır (context- dependent). Ardışık yayımlarla birlikte riskteki kademeli artışlar, her bir yayıma ilişkin marjinal risk kabul edilebilir görünse bile, zaman içinde toplam riskte önemli artışlara dönüşecek şekilde bileşebilir (compound). (‡1356, ‡1357).

Yapay zekâ yeteneklerinin çift-kullanımlı (dual-use) niteliği, yönetişimi daha da karmaşıklaştırır: tıpta veya araştırmada faydalı uygulamaları mümkün kılan özellikler zarara yönelik olarak yeniden amaçlandırılabilir ve ağırlıklar (weights) kamuya açık hale geldiğinde meşru kullanım ile kötü niyetli kullanımı ayırt etmek zorlaşabilir. Ayrıca, açık-ağırlık modellerin zararlı amaçlarla değiştirildiğinde kimin sorumlu tutulacağı da belirsizdir.

