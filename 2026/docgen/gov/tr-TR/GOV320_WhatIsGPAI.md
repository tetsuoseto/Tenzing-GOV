###@ Genel amaçlı yapay zeka sistemleri nedir?

Genel amaçlı AI sistemleri, büyük miktarlardaki verilerden örüntüler öğrenen ve tek bir belirli işlev veya alana özel olacak şekilde tasarlanmak yerine çeşitli görevleri yerine getirmelerini sağlayan yazılım programlarıdır (Bkz. Masa 1.1). Bu sistemleri oluşturmak için AI geliştiricileri, önemli miktarda hesaplama kaynağı, büyük veri kümeleri ve uzmanlaşmış uzmanlık gerektiren çok aşamalı bir süreç yürütür (Bkz. Masa 1.2). Hesaplama kaynakları (çoğu zaman ‘compute’ olarak kısaltılır), hem AI sistemlerini geliştirmek hem de devreye almak için gerekir; ayrıca onları çalıştırmak için gerekli olan yazılım ve altyapının yanı sıra özel bilgisayar çiplerini de içerir.† Büyük ve çeşitli veri kümeleri üzerinde eğitildikleri için genel amaçlı AI sistemleri, metin özetleme, görsel üretme veya bilgisayar kodu yazma gibi pek çok farklı görevi yerine getirebilir. Bu bölüm, genel amaçlı AI sistemlerinin nasıl üretildiğini, ‘akıl yürütme’ modellerinin ne olduğunu ve politika kararlarının genel amaçlı AI sistemlerinin geliştirilmesini nasıl şekillendirdiğini açıklar.

    Not † -- ‘compute’ terimi, bir işlemcinin gerçekleştirebileceği hesaplama sayısının ölçümünü (genellikle saniye başına kayan nokta işlemleri cinsinden ölçülür) ifade edebileceği gibi, bu hesaplamaları yapan donanımı (örneğin grafik işlem birimleri) da ifade edebilir.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Dil sistemleri
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Komut A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Büyük (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Görüntü üreteçleri
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Video oluşturucular
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Görüntüle 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotik ve navigasyon sistemleri
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Biyomoleküler yapıların çeşitli sınıfları için öngörücüler
- AlphaFold 3 (‡27)
- Amplify (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Yapay zeka ajanları
- AlphaEvolve (‡31*)
- ChatGPT Aracısı (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 1.1: Genel Amaçlı Yapay Zeka Türleri
>white|black||9|11|br Genel amaçlı AI’nin birkaç farklı türü vardır. Bu Rapor’da, farklı molekül sınıfları için yapısal bilgiyi tahmin edebilen modeller “genel amaçlı” AI olarak kabul edilir; çünkü çok çeşitli görevler için uyarlanabilirler. Örneğin, protein yapısını tahmin etmek üzere eğitilmiş modeller; protein etkileşimlerini tahmin etme, küçük moleküller için bağlanma bölgelerini tahmin etme ve siklik peptitleri (‡40) tahmin etme ile tasarlama gibi başka pek çok göreve uygulanabilir.


>white|orangered|left|13|15|bb Derin öğrenme genel amaçlı yapay zekanın temelini oluşturur

Araştırmacılar, ‘deep learning’ adı verilen bir süreçle genel amaçlı yapay zekâ modelleri geliştirir; bu süreç, modelleri örneklerden öğrenecek şekilde eğitir (‡41). Yazılım mühendisliğinden farklı olarak, deep learning modelleri görevleri baştan el yazımı talimatlara dayanarak değil; veriden öğrenerek yerine getirmeyi öğrenir. Görseller, metinler veya ses gibi büyük miktarda veriyi işleyerek, bu modeller o veriyi temsil etmenin yollarını keşfeder; böylece içeriye, kalıpları temsil eden yapılara (örneğin şekiller, kelime çağrışımları veya ses yapıları gibi) ilişkin iç temsiller geliştirir. Bu iç temsiller, modelin ilişkileri tanımasına ve eğitim hedefiyle uyumlu çıktılar üretmesine yardımcı olur. Daha sonra bu öğrenilmiş iç temsilleri, yeni ve benzer veriyi analiz etmek ve aynı üslupta çıktılar üretmek için soyut özellikler olarak kullanırlar. Örneğin, yeterli sayıda 19. yüzyıl İngiliz romantik şiiri örneğiyle eğitilmiş bir genel amaçlı yapay zekâ modeli, bu üsluptaki yeni şiirleri tanıyabilir ve benzer bir üslupta yeni içerik üretebilir.

Daha ayrıntılı bir seviyede, derin öğrenme, veriyi katmanlar halinde birbirine bağlı bilgi işleme düğümlerinden geçirerek çalışır. Bu düğümlere sıklıkla, biyolojik beyinlerdeki nöronlardan (biyolojik nöronlardan esinlenilerek) (''sinir ağları'' = ''neural networks'') gevşek bir şekilde esinlendiği için ''nöronlar'' denir (Figür 1.1) (‡42). Bilgi, bir nöron katmanından bir sonraki katmana akarken, model veriyi giderek daha soyut temsillere dönüştürür; bunlar, eldeki veride otomatik olarak keşfetmiş olduğu öğrenilmiş özellik gruplarıdır - yani elle kodlanmış olanlar değil. Örneğin bir görüntü işleme modelinde, ilk katmanlar kenarlar veya temel şekiller gibi basit özellikleri tespit etmeyi öğrenebilir; daha derin katmanlar ise bu özellikleri birleştirerek yüzler veya nesneler gibi daha karmaşık örüntüleri seçebilir.

Tüm katmanlardaki özellikler, eğitimi tanımlayan optimizasyon süreci aracılığıyla keşfedilir. Eğitim sırasında model hata yaptığında, derin öğrenme algoritmaları modelin performansını artırmak için nöronlar arasındaki çeşitli bağlantıların gücünü ayarlar. Düğümler arasındaki her bir bağlantının gücü çoğunlukla “weight” olarak adlandırılır. Bu katmanlı yaklaşım, derin öğrenmeye adını verir.

Derin öğrenme, yapay zeka sistemlerinin; daha önce geleneksel elle programlanmış hesaplama sistemleri ve diğer önceki sembolik veya kural tabanlı yapay zeka yöntemleri tarafından zor kabul edilen görevleri yerine getirmesini sağlayabilmede çok etkili olduğunu kanıtlamıştır. Günümüzde en ileri düzey genel amaçlı yapay zeka modellerinin çoğu, ‘dönüştürücü’ (‡43, ‡44) olarak bilinen belirli bir sinir ağı mimarisine dayanmaktadır. Dönüştürücüler, bilgiyi işlerken giriş verisinin en ilgili kısımlarına odaklanmaya yardımcı olan bir ‘dikkat’ mekanizması (‡45) kullanır; örneğin, bir cümlede anlamını anlamak için en önemli olan sözcüklerin hangileri olduğunu belirlemek gibi. Bu model kurma biçimi, çeviride (‡43), doğal dil işlemede (‡46), görüntü tanımada (‡47) ve konuşma tanımada (‡48, ‡49) önemli iyileştirmelere yol açmış; sonuçta bugünün en gelişmiş modellerinin geliştirilmesine giden yolu açmıştır.

![fig1.1](images/fig1.1_neural_network.png)

##### Figür 1.1: 'sinir ağı' için örnekleyici bir gösterim
>white|black||9|11|br Bugünün genel amaçlı yapay zeka modelleri, biyolojik beyinlerden esinlenen ancak gevşek bir şekilde uyarlanmış bu ağlara dayanmaktadır. Farklı ağların farklı boyutları ve mimarileri vardır. Bununla birlikte, hepsi ‘nöronlar’ adı verilen bağlı bilgi işleme birimlerinden oluşur; nöronlar arasındaki bağlantıların güçleri ise ‘ağırlıklar’ olarak adlandırılır. Ağırlıklar, büyük miktarda veriyi kullanan eğitim ile güncellenir. Kaynak: International AI Safety Report 2025 (‡50) (değiştirilmiştir).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Figür 1.2: Genel amaçlı yapay zekanın geliştirme aşamalarının şematik temsili
>white|black|left|9|11|br Uluslararası Yapay Zeka Güvenliği Raporu 2026.


>white|orangered|left|13|15|bb Genel amaçlı yapay zeka aşamalar halinde geliştirilir

Genel amaçlı bir AI sistemi geliştirmek, ilk model eğitiminden devreye aldıktan sonra izleme ve güncellemelere kadar birden fazla aşamayı içerir (Figür 1.2). Uygulamada, bu adımlar çoğu zaman yinelemeli bir biçimde örtüşür. Her aşama, farklı kaynak girdileri (örn. veri, emek, hesaplama) ve farklı teknikler gerektirir; ayrıca bazen farklı geliştiriciler tarafından yürütülür (Figür 1.2 ve Masa 1.2).

Örneğin, model ön-eğitimi genellikle büyük miktarda hesaplama gücü ve veri gerektirir; bu nedenle bu aşama, hesaplama kaynaklarına veya eğitim verilerine erişimi etkileyen politikalara karşı özellikle hassastır (‡51, ‡52). Benzer şekilde, veri derleme ve bazı model ince ayar yöntemleri şu anda başlangıç veri etiketleme için büyük miktarda insan emeği içerir (‡53). Bu nedenle bu aşama, emek maliyetlerindeki değişikliklere, platform politikalarına veya sınır ötesi sözleşme düzenlemelerini etkileyen düzenlemelere karşı hassastır.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Veri toplama ve kürasyon
> 
  Genel amaçlı bir yapay zeka modeli eğitmeye başlamadan önce, geliştiriciler ve veri çalışanları, ham eğitim verilerini toplayır, temizler, seçer ve standartlaştırır; böylece modelin öğrenebileceği bir formata dönüştürür. Bu süreç emek-yoğun olabilir. En güncel (state-of-the-art) modellerin arkasındaki eğitim veri setleri, internetin her yerinden gelen devasa sayıda örnekten oluşur.
  Ekipler, zararlı içeriği azaltmak, yinelenen verileri ortadan kaldırmak ve farklı konular ile kaynaklar arasında temsili geliştirmek için sıklıkla sofistike filtreleme yöntemleri geliştirir (‡54, ‡55). Veri kürasyonu ayrıca telif hakkı ve gizlilik ihlallerini azaltmaya, tehlikeli bilgiyi içeren örnekleri kaldırmaya, birden çok dili işlemeye ve veri soyağacına (data provenance) ilişkin dokümantasyonu iyileştirmeye yardımcı olabilir (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Ön eğitim (eğitimin ilk aşaması)

  Eğitim öncesinde, geliştiriciler modelleri büyük miktarlarda çeşitli verilerle besleyerek geniş bir bilgi tabanı ve bağlamsal anlayış kazandırır. Bu işlem bir ‘temel model’ üretir. Bu, son derece veri- ve hesaplama-yoğun bir süreçtir.

  Ön eğitim sırasında modeller, resimler, metinler veya ses gibi içeriklerden oluşan milyarlarca ya da trilyonlarca örneğe maruz bırakılır. Bu maruziyet sayesinde model, veriyi temsil edecek soyut özellikleri zamanla keşfeder ve bu özelliklerin birbirleriyle nasıl ilişkili olduğunu öğrenir; böylece bağlam içinde yeni girdilerin anlamını çıkarabilir. Bu ön eğitim süreci haftalar ya da aylar (‡59) sürer ve bu tür çok sayıda hesabı hızla işlemek üzere tasarlanmış, on binlerce ya da yüz binlerce grafik işlem birimi (GPU) veya tensör işlem birimi (TPU) (‡60) kullanır. Bazı geliştiriciler ön eğitimi kendi hesaplama kaynaklarıyla yaparken, diğerleri ise uzmanlaşmış hesaplama sağlayıcılarının sunduğu kaynakları kullanır.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Eğitim sonrası ve ince ayar (eğitimin ikinci aşaması)

  'Post-training', temel modeli daha spesifik bir uygulama için optimize etmek üzere daha da geliştirir. Bu işlem, orta düzeyde hesaplama yoğunluğuna sahip ve yüksek düzeyde emek-yoğun bir süreçtir. 'Sentetik veri' kullanımına yapılan bir kayma - algoritmalar veya simülasyonlar kullanılarak oluşturulan, gerçek dünya verisini taklit eden yapay olarak üretilmiş bilgi - bu aşamanın daha az emek-yoğun olmasına yardımcı oluyor.
  Son-öğrenme, çeşitli ince ayar teknikleri ve diğer değişiklikleri içerir. ‘Denetimli ince ayar’, eğitilmiş bir modelin, o alan içindeki performansını artırmak için belirli veri kümeleri üzerinde yeniden eğitilmesini ifade eder (‡61, ‡62). Örneğin genel amaçlı bir model, büyük bir radyolojik görüntü külliyatı üzerinde daha da eğitilebilir. ‘Pekiştirmeli öğrenme’ (RL), arzu edilen çıktılar için bir modeli ‘ödüllendirerek’ (olumlu geri bildirim sağlayarak) ve arzu edilmeyen çıktılar için bir modeli ‘cezalandırarak’ (olumsuz geri bildirim sağlayarak) model performansını artırmayı içerir. İki öne çıkan alt kategoriye sahiptir. ‘İnsan geri bildirimi ile pekiştirmeli öğrenme’, insan tercihleriyle uyumlu çıktıları ödüllendirmeyi ve insan geri bildirimine dayanarak uyumsuz olanları cezalandırmayı içerir (‡63, ‡64*). ‘Doğrulanabilir ödüllerle pekiştirmeli öğrenme’ (RLVR), matematik veya kod üretimi gibi olgusal doğruluk gerektiren görevlerde model performansını iyileştirmek için kullanılır. Geliştiriciler genellikle, sonuçlar modelin istenen özellikleri karşıladığını gösterene kadar, son-öğrenme tekniklerini uygulama ile testleri çalıştırma arasında dönüşümlü olarak ilerler.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Sistem entegrasyonu

  Geliştiriciler, kullanıma hazır bir ‘Yapay Zeka sistemi’ oluşturmak için bir veya daha fazla genel amaçlı AI (Yapay Zeka) modelini diğer bileşenlerle birleştirir. GPT-5 (örneğin) bir metin, görseller ve ses işleyen genel amaçlı bir AI modelidir; ChatGPT ise, farklı boyutlarda ve yeteneklerde birkaç modeli bir araya getirerek bir sohbet arayüzü, içerik işleme, Web erişimi ve uygulama entegrasyonu ile işlevsel bir ürün oluşturmuş genel amaçlı bir AI sistemidir.
  Yalnızca AI modellerini işler hale getirmekle kalmayıp, bir AI sistemindeki ek bileşenler de yetenek, kullanılabilirlik ve güvenliği artırmayı hedefler. Örneğin, bir sistem; zararlı içerik barındıran model girdilerini veya çıktıları tespit eden ve engelleyen bir filtreyle gelebilir (‡65*). Geliştiriciler ayrıca giderek artan şekilde ‘scaffolding’ kullanıyor; genel amaçlı AI modelleri etrafında inşa edilen, önceden plan yapmalarını, hedefleri izlemelerini ve dünya ile etkileşim kurmalarını sağlayan ek yazılımlar (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Dağıtım ve sürümleme
  Dağıtım, entegre Yapay Zekâ sisteminin amaçlanan kullanımı için erişilebilir hale getirilmesi sürecidir. Geliştiriciler ve dağıtım yapanlar Yapay Zekâ sistemlerini gerçek dünya uygulamalarına, ürünlere veya hizmetlere entegre eder. Geliştiriciler Yapay Zekâ sistemlerini dahili olarak (kendi kullanımları için) veya harici olarak (özel müşteriler ya da kamu kullanımı için) dağıtabilir. Yapay Zekâ sistemlerini harici olarak dağıtırken, şirketler genellikle kullanıcıların sisteme erişmesini ve sistemi çalıştırmasını sağlayan çevrimiçi kullanıcı arayüzleri veya Uygulama Programlama Arayüzleri (API) üzerinden erişim sunar. Örneğin, bir şirket başka bir şirketin genel amaçlı Yapay Zekâ sisteminden güç alan özel bir müşteri hizmetleri sohbet botu tasarlayabilir.
  ‘AI system deployment’ gerçek dünyada kullanım için, entegre araçlar ve arayüzlerle birlikte bir modelin erişilebilir hale getirilmesini ifade ederken, ‘model release’ temel modelin başkalarına sunulmasını içerir - ya açık ağırlık (indirilebilir parametreler) olarak ya da kapalı ağırlık (yalnızca API erişimi). Bkz. §3.4. Açık ağırlık modelleri.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Dağıtım sonrası izleme ve güncellemeler

  Geliştiriciler sıklıkla kullanıcı geri bildirimlerini toplar ve analiz eder, etki ve performans metriklerini izler ve gerçek dünya kullanımı sırasında keşfedilen sorunları gidermek için yinelemeli iyileştirmeler yapar (‡67). İyileştirmeler, sistem entegrasyonlarını güncelleyerek yapılır; çoğunlukla sürekli ince ayar yoluyla ve modellere (yakın tarihli) olguların harici veritabanlarına erişim sağlayarak gerçekleştirilir. Bu, büyük yapay zeka modellerinin tam ön eğitim sürecini tekrarlamadan güncel kalmasını sağlar (‡68*). Bu da, ardışık eğitim turları boyunca yeteneklerin birikmesine olanak tanırken istikrarı korur ve hesaplama maliyetlerini azaltır.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 1.2: Genel amaçlı yapay zeka geliştirme aşamaları
>white|black||9|11|br Her genel amaçlı yapay zeka geliştirme aşamasında, yapay zeka modeli alt kullanım için iyileştirilir ve sonunda, izlenen ve güncellenen tamamen entegre bir yapay zeka sistemi olarak dağıtılır.


>white|orangered|left|13|15|bb Muhakeme sistemleri, performansı artırmak için çıkarım sırasında “düşünce zincirleri” üretir

Çıkarım, birinin eğitimden sonra AI modelini kullanmasıyla gerçekleşir. Örneğin, bir kişi bir AI sisteminden bir seyahat planlamasını istediğinde ve bunun arkasındaki model, coğrafya, ulaşım ve yemek kültürüyle ilgili öğrendiği uygun yönlerden yararlanarak bir güzergah oluşturduğunda çıkarım gerçekleşir.

Son on yılda, Yapay Zeka (AI) yeteneklerindeki ilerlemelerin büyük kısmı daha büyük eğitim çalıştırmalarından kaynaklandı; yani bir AI modelini eğitmek için kullanılan hesaplama (compute) miktarını artırmak. Ancak yakın zamanda, araştırmacılar; modellerin daha uzun süre boyunca bilgi işlemesine izin vererek ve görevlerini yerine getirirken açık akıl yürütme adımları üretmeleri için onları eğiterek daha fazla kazanım elde etti (‡69*, ‡70). Bu şekilde çalışan AI sistemlerine ‘akıl yürütme sistemleri’ denir ve bir problemi çözerken ya da bir soruyu yanıtlarken üzerinden geçtikleri ara açıklamalara ‘thought chain’ (akıl yürütme zincirleri) denir. Akıl yürütme sistemleri, bu sofistike akıl yürütme zincirlerini üretmek için kullanım anında daha fazla hesaplama kaynağı gerektirir (‡71, ‡72, ‡73, ‡74) ve daha iyi akıl yürütmeyi öğrenebilmeleri için eğitim sırasında da daha fazla kaynak ister. Uygulamada, bu akıl yürütme yetenekleri; bir görevi daha küçük adımlara iteratif olarak ayırarak AI sistemlerinin daha karmaşık problemleri çözmesini sağlar. Masa 1.3, aynı problemi çözen akıl yürütme yapmayan bir sistem ile bir akıl yürütme sistemine ilişkin bir örnek göstermektedir.

Akıl yürütme sistemleri, zorlu problemler üzerinde yeteneklerinde önemli atılımlar gerçekleştirdi. Örneğin, 2025 yılında matematiksel problem çözmeye odaklanmış akıl yürütme sistemleri; Google’ın Gemini Deep Think’i ve OpenAI’den yayınlanmamış, deneysel bir model de dahil olmak üzere, Uluslararası Matematik Olimpiyatı problemlerini (yapılandırılmış bir test ortamında) insan altın madalya performansına eşdeğer bir düzeyde çözdü (‡75, ‡76). Akıl yürütme sistemleri; adım adım akıl yürütmenin açıkça doğrulanabildiği matematik, mantık bulmacaları ve yapılandırılmış bilimsel sorular gibi biçimsel alanlarda kayda değer ilerleme gösterdi (‡77). Bununla birlikte, akıl yürütme sistemleri alakasız, verimsiz veya tekrarlayıcı düşünce zincirleri üreterek de başarısız olabilir (‡78, ‡79).

###@ Eğitim yöntemlerine ilişkin güncellemeler

Son Yayınlanan Rapor’un (Ocak 2025) yayımlanmasından bu yana, ‘distillation’ (damıtma) adı verilen bir eğitim yöntemi, bazı modellerin ince ayarının (fine-tuning) verimini büyük ölçüde artırdı. Damıtma, daha güçlü (ve genellikle daha büyük) bir ‘teacher’ modelinin çıktıları üzerinde bir ‘student’ modelini eğitmeyi içerir; bu sayede student modeli, teacher modelinin çıktılarıni doğrudan taklit edebilir (‡80). Örneğin DeepSeek, zincir-of-thought (chain-of-thought) muhakemesinde üstün olan DeepSeek-R1 adında büyük bir model geliştirdi. R1, daha sonra DeepSeek-V3 de dahil olmak üzere daha küçük student modellerini ince ayar yapmak için kullanılan muhakeme çıktıları üretti. DeepSeek-V3, R1’in matematiksel, kodlama ve belge-analizi yeteneklerinin büyük bir kısmını koruyor ve yaklaşık $10,000 USD için (ön eğitim maliyetleri bildirilmemiş olsa da) ince ayar yapıldığı bildiriliyor (‡81). Bu durum, benzer derecede yetenekli daha büyük modellerin ince ayar maliyetinin muhtemelen büyüklük mertebeleri (orders of magnitude) daha düşüktür.

![table1.3](images/table1.3_example_reasoning.png)

##### Masa 1.3: Türetim yapmayan bir sisteme (sol) karşı bir akıl yürütme sisteminin (sağ) örneği
>white|black||9|11|br Aynı bilmecenin çözülmesiyle ilgili olarak, bu örnekler gerçek yapay zeka yanıtlarından uyarlanmıştır. Akıl yürütme sistemi, nihai yanıtını vermeden önce bir ‘düşünce zinciri’ oluşturarak ‘düşünmeye’ daha fazla zaman ve hesaplama gücü harcar.

![figure.3](images/fig1.3_AI_agent.png)

##### Figür 1.3: Yapay zeka aracısına ilişkin örnekleyici bir temsil
>white|black||9|11|br Gerçek dünyadaki görevleri yerine getirmek için araçları kullanıp araçlarla yinelemeli olarak plan yapma, muhakeme etme ve uygulama üzere yapılandırılmış bir yapay zeka modeli (merkez). Kaynak: International AI Safety Report 2026.


Bu nedenle, damıtma, modellerin daha güçlü yetenekler kazanması için ucuz ve verimli bir yol olabilir (‡82). Bazı araştırmacılar, damıtmayı kullanarak en güncel modellerden (state-of-the-art) üretilen yalnızca 1,000 örnekle, son derece yetenekli modelleri ince ayarlamak için kullanmıştır (‡83). Damıtma, önceden var olan bir öğretici (teacher) modele ihtiyaç duyduğundan, en güncel model yeteneklerini doğrudan ilerletmek için kullanılamaz. Ancak, kapalı kaynak modellerden bile (closed-source) (‡84*) gelişmiş yapay zeka yeteneklerinin yayılmasını hızlandırabilir.

‘dağıtık hesaplama’ alanındaki teknolojik ilerlemeler ve merkeziyetsiz eğitim (geliştiricilerin AI eğitimi veya çıkarımı gerçekleştirmek için birlikte çalışan birden fazla işlemciyi, sunucuyu veya veri merkezini kullandığı yaklaşımlar (‡85, ‡86, ‡87)) ile birlikte, birçok AI geliştirme projesinin büyük ölçekli, merkezî hesaplama altyapısına bağımlılık düzeyi azaltılmıştır. Bu durum giderek, kaynakları daha sınırlı aktörlerin güçlü sistemler geliştirmesine ve devreye almasına imkan tanımaktadır.

###@ Yapay zeka ajanları hakkındaki güncellemeler

Son Rapor (Ocak 2025) tarihinden bu yana, geliştiricilerin AI modellerini araçlarla nasıl birleştirdiğine dair ilerlemeler, giderek daha güçlü AI ajanlarının geliştirilmesini mümkün kılmıştır. AI ajanları, çoğu zaman kullanıcılar tarafından doğal dilde belirtilen hedefleri gerçekleştirmek üzere tasarlanır. Bu hedeflere ulaşmak için; bellek, bir bilgisayar arayüzü ve web tarayıcıları gibi araçlara erişim verilir. Bu araçlar ve bunları modelle birleştirmek için kullanılan kod, ‘scaffolding’ olarak adlandırılır ve AI ajanlarının dünyayla özerk biçimde etkileşime girmesine, plan yapmasına, önemli ayrıntıları hatırlamasına ve hedefleri daha az insan gözetimi veya yardımıyla (‡88*, ‡89) sürdürmesine yardımcı olur. Örneğin Manus AI, Web arama, yazılım geliştirme ve çevrimiçi satın alımlar da dahil olmak üzere çeşitli görevleri otomatikleştirebilen popüler bir AI ajandır (‡90). Şekil 1.3, bellek, web tarama ve bilgisayar kullanımı için araçları yinelemeli olarak planlama, akıl yürütme ve kullanabilen genel amaçlı bir AI modeli ‘brain’den oluşan basit bir AI ajan örneğini göstermektedir.

AI aracısılar için dijital altyapı genişliyor (‡91) ve çeşitli sektörlerde giderek daha yaygın hale geliyor (‡92, ‡93, ‡94). AI aracısılar; araştırma (‡37), yazılım mühendisliği (‡95), robotik kontrol (‡96) ve müşteri hizmetleri (‡97) gibi görevler için geliştirilmiştir. Süregelen araştırma ve geliştirme çalışmaları, giderek daha yetenekli ve daha özerk AI aracısılar ya da çoklu aracısı sistemleri ortaya çıkarmıştır. Araştırmacılar, AI aracısıların yerine getirebildiği yazılım kıyaslama görevlerinin karmaşıklığının yaklaşık her yedi ayda bir iki katına çıktığını tahmin etmiştir (bkz. §1.2. Mevcut yetenekler) (‡98). Uzmanlar, giderek daha yetenekli AI aracısıların hem önemli fırsatlara hem de risklere yol açacağını savunuyor (‡99, ‡100*) (bkz. §2.2.1. Güvenilirlik zorlukları).

###@ Kanıt boşlukları

Genel- amaçlı yapay zeka sistemi geliştirme süreci etrafındaki temel kanıt eksiklikleri, bu sistemlerin nasıl geliştirildiğine ilişkin kamuya açık bilgi eksikliğinden kaynaklanmaktadır. Bazı geliştiriciler, genel- amaçlı yapay zeka sistemlerini nasıl geliştirdikleri konusunda son derece şeffaftır (‡1, ‡101). Ancak genel olarak, en gelişmiş modellerin nasıl geliştirildiği, nasıl korunduğu, nasıl değerlendirildiği ve nasıl devreye alındığı konusunda kamu ve politika yapıcıların bilgisi sınırlı kalmaktadır. Bu durum, özellikle yapay zeka şirketleri içinde kullanılan ancak dış paydaşlar tarafından kullanılmayan veya anlaşılmayan, şirket içi olarak devreye alınmış yapay zeka sistemleri için geçerlidir (‡102, ‡103). Bu sınırlı dış görünürlük, şeffaflık ve gözetim açısından zorluklar yaratır. Çeşitli araştırmacılar, eğitim verisi (‡104, ‡105, ‡106), genel- amaçlı yapay zeka modelleri (‡107, ‡108), yapay zeka ajanları (‡92), değerlendirmeler (‡109), geliştirme hatları (‡110) ve güvenlik (‡111) etrafında sınırlı ve tutarsız şeffaflığa dikkat çekmiştir. Dışa açıklamaya getirilen sınırlamalar bazen şirketlerin ticari sırlarını ve fikri mülkiyetini korumak için gerekli olabilir. Bununla birlikte, düşük şeffaflık; bağımsız araştırmacıların ve politika yapıcıların genel- amaçlı yapay zeka modellerini ve sistemlerini incelemesini daha da zorlaştırır.


