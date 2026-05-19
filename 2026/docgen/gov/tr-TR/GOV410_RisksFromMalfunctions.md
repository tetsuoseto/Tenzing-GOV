Genel amaçlı yapay zeka (AI) sistemleri, uydurulmuş yasal atıflardan tıbbi yanlış tanılara kadar, gerçek dünyada zaten somut zararlara yol açmış şekillerde başarısız olur. İnsan profesyonelleri de hata yapabilse de, AI başarısızlıkları özellikle özgünlükleri, potansiyel ölçekleri, ne zaman ortaya çıkacaklarını öngörmenin zorluğu ve kullanıcıların kendinden emin ifadeler veren çıktılara eleştirel bakmadan güvenme eğilimleri nedeniyle farklı endişeler doğurur. Güncel genel amaçlı AI başarısızlıkları; yanlış bilgi sağlama (‡602, ‡603), temel akıl yürütme hataları yapma (‡604, ‡605) ve yeni bağlamlarda dağıtıldıklarında performansın bozulması (‡606, ‡607, ‡608) gibi durumları içerir. Bu tür başarısızlıklardan kaynaklanan belgelenmiş zararlar; tıbbi yanlış tanılar, hukuk davaları için hazırlanan dilekçelerdeki hatalar ve mali kayıpları (‡609, ‡610, ‡611) kapsar. Güvenilirlik zorlukları, özellikle AI ajanları için kritik önemdedir; çünkü başarısızlıklar, insan eylemi veya denetimi olmadan doğrudan zarara yol açabilir (‡612, ‡613, ‡614, ‡615). Çoklu ajanlı sistemler ise ajanlar arasında yanlış koordinasyon, çatışmalar veya istenmeyen iş birliği (kollüzyon) yoluyla ek başarısızlık türleri ortaya çıkarır (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Varsayım hatası
- Yasal dilekçelerde var olmayan emsalden alıntı yapmak (‡617)
- Yaslı yolcular için mevcut olmayan indirimli ücret politikalarına atıfta bulunma (‡618)
- Hatalı ve önyargılı tıbbi bilgi sağlamak (‡619)
- Olaylar hakkında güncel olmayan bilgi sağlama (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Temel akıl yürütme hatası
- Matematiksel hesaplamaları gerçekleştirememek (‡621)
- Temel nedensel ilişkileri çıkarsayamamak (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dağıtım-dışı başarısızlık (tanıdık olmayan veya olağandışı girdilerde başarısızlık)
- Arka plan aydınlatması veya bağlam değiştiğinde görüntülerin yanlış sınıflandırılması (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Araç kullanımı hatası
- Bir yapay zeka ajanı tarafından, üçüncü taraf bir araca gönderilerek bir kullanıcının özel görüntüsünün ifşa edilmesi nedeniyle gizlilik ihlali (‡624)
- Kısa süreli çalışma belleğinin başarısızlığı (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Çoklu ajan sistemi arızası: koordinasyon eksikliği ve çatışma
- Bireysel teşvikler ile kolektif refah hedefleri arasındaki bir çatışma nedeniyle paylaşılan kaynakların yönetilememesi (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 2.4: Genel amaçlı yapay zeka ve ajan sistemlerinde güvenilirlik sorunlarına örnekler
>white|black||9|11|br Genel amaçlı yapay zeka sistemlerinde, yapay zeka aracılarında ve çoklu aracılarda belgelenmiş güvenilirlik sorunları.


###@ Genel amaçlı yapay zeka sistemleri, çeşitli güvenilirlik zorluklarıyla karşı karşıyadır

Masa 2.4. güvenilirlik sorunlarının ortak kategorilerini özetler. İlk üçü tüm AI sistemleri için geçerliyken, son iki tanesi özellikle AI ajanları ve çoklu ajan sistemlerine ilişkindir. Pek çok güvenilirlik riski, AI sisteminin davranışını tahmin etmenin ve izlemenin zorluğundan kaynaklanır.

Bu zorluklar (ayrıca §3.1. Teknik ve kurumsal zorluklar bölümünde ele alınmıştır), özellikle karmaşık ortamlarda faaliyet gösteren AI ajanlar için daha da şiddetlidir. Bu tür arızaları değerlendirmeye ve azaltmaya yönelik mevcut yöntemler arıza oranlarını düşürebilir; ancak en iyi durumda bile AI ajanları yeterince güvenilir değildir, bu da çeşitli bağlamlarda riskler oluşturur ve devreye almayı engeller.

'Güvenilirlik', bir AI sisteminin geliştirici veya kullanıcı tarafından amaçlandığı şekilde çalıştığı kapsamı ifade eder. Genel amaçlı AI sistemleri, hatalı ya da yanıltıcı içerik üretiminden temel muhakemeyi gerçekleştirememeye kadar uzanan çeşitli güvenilirlik sorunları yaşar. Örneğin, modeller olgusal bilgileri hatırlama konusunda gelişmiş olsa da; hatta önde gelen modeller bile önemli oranlarda kendinden emin ama yanlış yanıtlar verebilmektedir (Figür 2.10). Yazılım mühendisliğinde, genel amaçlı AI artık bilgisayar kodu yazma, değerlendirme ve hata ayıklama süreçlerinde önemli ölçüde yardımcı olabilmektedir (‡215*, ‡628, ‡629). Ancak AI tarafından üretilen kod çoğu zaman hatalar içerir (‡630); kodlama aracıları ise düzenli olarak hatalar yapar (‡631). Bu tür başarısızlıklar, programlara ve güvenlik sistemlerine açıklar kazandırabilir (bkz. §2.1.3. Siber Saldırılar).

Güvenilirlik sorunlarını yüksek riskli ortamlarda, örneğin tıpta, özellikle takip etmek önemlidir; AI kullanımının hızla artması ve başarısızlıkların ciddi zarara yol açma potansiyeli nedeniyle (‡609, ‡619). İlgili yetenekler hızlı biçimde gelişti; önde gelen modeller artık tıbbi sınavları geçebiliyor (‡633*, ‡634). Ancak gerçek dünyadaki kullanım, ölçütlerin gözden kaçırdığı sınırlılıkları ortaya koyuyor. Örneğin bir çalışmada, modellerin yanıtları sorulan tıbbi soruların 19%ı için potansiyel olarak zararlı olmuştur (‡635). Bu tür başarısızlıklar yanlış tanıya, uygunsuz tedaviye veya sağlık hizmetinin hatalı biçimde reddedilmesine yol açabilir (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Figür 2.10: SimpleQA Doğrulanmış kıyaslama üzerinde ana modellerin sonuçları
>white|black||9|11|br Model sürüm tarihine göre SimpleQA Verified kıyaslamasındaki başlıca modellerin sonuçları. Bu kıyaslama, modelin olgusal doğruluğunu ve gerçekleri güvenilir şekilde geri çağırma yeteneğini ölçer. Kısa biçimli soru-yanıt (QA) formatına sahiptir ve halüsinasyonlar gibi güvenilirlik sorunlarını tespit etmek üzere tasarlanmıştır. Kaynak: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Yapay zeka ajanları, özerkliklerinden dolayı yeni güvenilirlik riskleri ortaya çıkarır

Çünkü yapay zeka ajanları doğrudan gerçek dünyada eylemde bulunur, başarısızlıkları aracısız (agentic olmayan) sistemlerdeki başarısızlıklardan daha fazla zarara yol açma potansiyeline sahiptir (‡99). Sadece insanlar tarafından gözden geçirilmek üzere metin veya görseller üreten yapay zeka sistemlerinin aksine, yapay zeka ajanları dünyanın üzerinde etkisi olan eylemleri bağımsız olarak gerçekleştirebilir (‡99, ‡615, ‡636, ‡637) (ayrıca bkz. §1.1. Genel amaçlı AI nedir?). Yapay zeka ajanları eylemleri başlatabilir, diğer insanları veya yapay zeka sistemlerini etkileyebilir ve gelecekteki sonuçları dinamik olarak şekillendirebilir. Etki alanının bu şekilde genişlemesi yeni riskler ortaya çıkarır ve güvenilirliğin önemini artırır; çünkü başarısızlıklar, insanın müdahale etmesi için herhangi bir fırsat olmaksızın doğrudan zarara neden olabilir (‡99, ‡612, ‡638, ‡639, ‡640). Bu durum, özellikle finansal hizmetler (‡641), enerji yönetimi (‡642) veya bilimsel araştırma (‡643*, ‡644) gibi stratejik ya da güvenlik- kritik ortamlarda konuşlandırılan ajanlar için daha da önemli olabilir.

>white|orangered|left|14|15.5|bb Çoklu ajanlı yapay zeka sistemleri yeni tür güvenilirlik arızaları ortaya çıkarır

Çok etmenli yapay zeka sistemleri, koordinasyon hataları veya etmenler arasındaki çatışma nedeniyle yeni tür güvenilirlik arızaları ortaya çıkarır. Çok etmenli yapay zeka sistemlerinde, etmenler ya ortak ya da bireysel hedefler doğrultusunda birbirleriyle etkileşir (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Örneğin, araştırma literatür taraması yapmak üzere tasarlanmış bir çok etmenli sistemde, bir lider etmen kullanıcının sorgusunu ayrıştırır ve her biri farklı bir yönü paralel olarak araştırmaktan sorumlu olan uzman alt etmenlere alt görevler atar (‡650*). Bu durum verimlilik artışı sağlasa da, hataların etmenler arasında yayılabileceği anlamına da gelir (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Birden fazla etmen aynı temel modele dayanıyorsa veya aynı araçları içeriyorsa, ayrıca ilişkili arızalar da sergileyebilir (‡656). Dağıtılmış sistemlerde bu tür arızalara ilişkin ampirik kanıtlar sınırlı kalmaktadır; ancak çok etmenli sistemler daha yaygın hale geldikçe bu riskler artabilir.

###@ Güncellemeler

Geçen Raporun (Ocak 2025) yayımlanmasından bu yana AI ajanlarına yönelik ticari ve araştırma ilgisi önemli ölçüde arttı. Daha fazla AI ajan gerçek dünyaya konuşlandırılıyor (Şekil 2.11), bunların çoğu bilgisayar kullanımı veya yazılım mühendisliği uygulamalarında uzmanlaşıyor (‡92). XBOW hacking agent (‡467), Claude-4 (‡659) ve ChatGPT Agent (‡660) gibi yakın tarihli sürümler, Web aramalarına dayalı slayt desteleri oluşturma (‡660) gibi yeni gelişmekte olan özerk yetenekleri gösteriyor. Ancak daha uzun görevlerde hata oranları arttığı için seyahat planlama ve rezervasyon gibi daha karmaşık görevleri henüz yerine getiremiyorlar (‡100) (‡98, ‡148). Mevcut araştırmalar; ajanların harici araçlarla ve diğer ajanlarla nasıl iletişim kurduğuna ilişkin standartlar geliştirmeye yönelik çabaları içeriyor (‡661, ‡662). Örnekler arasında Google’ın Agent2Agent (‡663) ve Agent Payments (‡664) protokolleri ile Anthropic’in Model Context Protocol (‡665) yer alıyor.

>oldlace|black||11|15|br      
####@ Not 2.4: Bilinçli saldırılar ayrıca yapay zeka sistemlerinin başarısız olmasına neden olabilir
>oldlace|black|left|13|15|hb Not 2.4: Bilinçli saldırılar aynı zamanda yapay zeka sistemlerinin başarısız olmasına da neden olabilir
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bu bölüm, istenmeyen güvenilirlik aksaklıklarına odaklanır; ancak kötü niyetli aktörler de prompt injection gibi saldırılar üzerinden aksaklıkları özellikle tetikleyebilir. Bir prompt injection saldırısında, kötü niyetli talimatlar bir aracın önüne dolaylı yoldan; örneğin web sitelerindeki veya veritabanlarındaki gizli talimatlar gibi kanallar aracılığıyla sunulur (‡507, ‡657, ‡658). Bu talimatlar aracın davranışını ‘ele geçirerek’ onun kullanıcı niyetlerine aykırı şekilde hareket etmesine yol açabilir. Bu tür saldırılara karşı savunmak özellikle zordur; çünkü kullanıcıların ya da geliştiricilerin kontrolü dışında kalan harici içerik kullanılarak iletilirler. Saldırı hedefi olarak AI sistemleri §2.1.3’te daha ayrıntılı olarak ele alınmaktadır. Siber saldırılar ve teknik savunmalar §3.3’te, yani Teknik güvenceler ve izleme başlığı altında ele alınır.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Figür 2.11: AI ajanlarının sayısı 2023'ten bu yana arttı
>white|black||9|11|br 67 dağıtılmış yapay zeka aracının Aralık 2024 anketinden elde edilen sonuçlar. Sol: Önemli yapay zeka aracısürümlerinin zaman çizelgesi. Sağ: Yapay zeka aracılarının kullanılmakta olduğu uygulama alanları. Altı alan, ankette belirlenen en yaygın kullanım kategorilerine göre tanımlanmıştır. Kaynak: Casper ve diğerleri, 2025 (‡92).


###@ Kanıt boşlukları

Ana kanıt boşlukları, yapay zeka (AI) sistemlerinin yeteneklerini, kısıtlarını ve başarısızlık biçimlerini güvenilir biçimde değerlendirmedeki güçlüklerden kaynaklanmaktadır (bkz. §3.1. Teknik ve kurumsal zorluklar). AI aracılarının güvenilirliğine ilişkin sistematik değerlendirmeler sınırlıdır ve standartlaştırmadan yoksundur (‡92, ‡666). Eski bilgiye dayanma (‡620) gibi bazı sorunlar yalnızca gerçek dünya kullanımında ortaya çıkabilir; bu da dağıtımdan önceki değerlendirmeleri yetersiz hale getirir. Önceki çalışmalar, aracılar ve çoklu-aracı sistemlerinin güvenilirliğini geleneksel yazılımda ve daha önceki AI biçimlerinde incelemiştir (‡647, ‡667, ‡668). Ancak bu çalışmanın, sıklıkla büyük dil modellerine dayanan modern AI aracılara uygulanabilirliği belirsizdir (‡669). Bazı araştırmacılar, aracılar birbirleriyle etkileşime girdiğinde sergileyebilecekleri yeni davranışlar hakkında endişeler dile getirmiştir; örneğin işbirliği (collusion) veya ilişkili (correlated) başarısızlıklar (‡614). Bununla birlikte, ampirik kanıtlar sınırlı kalmaktadır. Bu boşlukları gidermeye yönelik çabalar arasında, Ulusal Standartlar ve Teknoloji Enstitüsü’nün (NIST) ajan-kapırma (agent-hijacking) risklerine ilişkin yeni değerlendirmeleri (‡670), OECD’nin AI Yetenek Göstergeleri (‡243) ve UK AI Güvenlik Enstitüsü’nün Inspect Sandboxing Toolkit’i (‡671) yer almaktadır.

###@ Azaltımlar

AI güvenilirliğini artırmaya yönelik teknikler, hem modelin kendisini hem de onun devreye alındığı daha geniş sistemi hedefler. Bunlar arıza oranlarını azaltabilir, ancak kritik alanlarda gereken yüksek güvenilirliği şu ana kadar hiçbiri tek başına garanti edemez (‡672). Önemli bir teknik önlem, modelleri eğitim sırasında zorlayıcı girdilerle karşılaştıran ve daha uygun, sağlam yanıtlar geliştirmesine yardımcı olan adversaryal (kötücül) eğitimdir (‡673, ‡674, ‡675, ‡676, ‡677) (bkz. §3.3. Teknik güvenceler ve izleme). Halüsinasyonları azaltmak için geliştiriciler, bir modelin yanıtlarını harici bir veritabanından alınan bilgilerle destekleyen, böylece çıktıları doğru ve güncel tutmaya yardımcı olan retrieval-augmented generation (RAG) uygulayabilir (‡678, ‡679, ‡680) veya özellikle modelleri daha olgusal olacak şekilde ince ayar yapabilir (‡681) ya da daha etkili biçimde akıl yürütecek şekilde optimize edebilir (‡682). Ortama- veya araca-dayalı yöntemler de geliştiricilerin AI sistemlerini izlemesine yardımcı olabilir (‡683). Örneğin, devreye alanlar, daha geniş ölçekte konuşlandırmadan önce olası arıza türlerini analiz etmek için AI sistemlerini sınırlı, sandboxta benzer ortamlarda pilot olarak çalıştırabilir.

Özellikle AI ajanları için araştırmacılar, geliştirilmiş şeffaflık, gözetim ve izleme yoluyla güvenilirliği artırmayı önermiştir. Örneğin, ajanların harici araçlarla ve diğer ajanlarla olan etkileşimlerinin izlenmesi, ajan etkinliklerinin daha etkili şekilde denetlenmesini (‡684, ‡685) ve olay analizi yapılmasını (‡686) sağlayacaktır. Bu tür bilgileri otomatik olarak toplamak için yöntemler; çoklu ajan ortamlarında olanlar da dahil olmak üzere, araştırmanın aktif bir alanı olmaya devam etmektedir (‡653, ‡654).

###@ Politika yapıcılar için zorluklar

Politika yapıcılar için temel zorluklar; yapay zeka aracısı (AI agent) konuşlandırmanın faydalarını, güvenilirlik arızaları risklerine karşı tartmayı ve geliştiricilerin, dağıtıcıların (deployers) ve kullanıcıların, aracının performansı ile risk profilleri hakkında doğru bilgilere erişebilmesini sağlamayı içerir. Yapay zeka aracılarının neden olduğu zararlar için sorumluluğun nasıl atfedileceğine karar vermek ise ek bir zorluk oluşturur (‡639); özellikle çoklu aracılı (multi-agent) senaryolarda arızaların ne zaman ve nasıl gerçekleştiğinin tespit edilmesi zor olabilir (‡687). Bu zorluklar, aracılar özerklik kazandıkça ve harici araçlara erişime sahip oldukça aracının güvenilirliğini değerlendirmekteki güçlük nedeniyle daha da artar (‡688*, ‡689). Aracısal (agentic) yeteneklerin ne kadar hızlı ortaya çıkacağına dair belirsizlik de, yeni zorluklar için plan yapmayı zorlaştırır (bkz. §3.1. ‘kanıt ikilemi’ne ilişkin teknik ve kurumsal zorluklar).

#### 2.2.2. Kontrol kaybı

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Temel bilgiler
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kontrol kaybı senaryoları, bir veya daha fazla genel amaçlı Yapay Zeka sisteminin, kimsenin denetimi dışında çalıştığı ve kontrolü yeniden kazanmanın ya son derece maliyetli olduğu ya da mümkün olmadığı senaryolardır. Bu varsayımsal senaryolar şiddet düzeyleri açısından farklılık gösterir; ancak bazı uzmanlar, insanlığın dışlanması veya yok oluşu kadar ağır sonuçlara da inandırıcılık verir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kontrol kaybı olasılığına ilişkin uzman görüşleri büyük ölçüde değişmektedir. Bazı uzmanlar bu tür senaryoları pek olası görmezken, bazıları bunları, yüksek potansiyel ciddiyetleri nedeniyle dikkat gerektirecek kadar olası olarak değerlendirmektedir. Bu risk hakkındaki genel görüş ayrılığı, gelecekteki AI yetenekleri, davranışsal eğilimler ve dağıtım gidişatına ilişkin farklı değerlendirmelerden kaynaklanmaktadır.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mevcut yapay zeka sistemleri, ilgili yeteneklere dair erken belirtiler gösteriyor; ancak kontrol kaybını mümkün kılacak düzeylerde değiller. Kontrol kaybına neden olabilmek için sistemlerin, gözetimden kaçınma, uzun vadeli planlar yürütme ve konuşlandıranları ile diğer aktörlerin karşı önlemleri uygulamasını engelleme dahil olmak üzere bir dizi ileri yeteneğe ihtiyaç duyması gerekir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Kontrol kaybı, Yapay Zekâ sistemleri “uyumsuz” olduğunda daha olası hale gelir; yani geliştiricilerin, kullanıcıların veya toplumun daha geniş niyetleriyle çelişen hedeflere sahiptirler. Bu tür hedefleri sürdürmek için uyumsuz bir sistem yanlış bilgi sağlayabilir, istenmeyen eylemleri gizleyebilir veya kapatmaya direnebilir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Previous Report'un (January 2025) yayımlanmasından bu yana modeller, daha gelişmiş planlama ve gözetim-körelten (oversight-undermining) yetenekler sergilemiş; bu da yeteneklerini değerlendirmeyi daha da zorlaştırmıştır. Modeller, değerlendirmelerinde “ödül hackleme” (reward hacking) yapmayı; açıkları bularak geliştirmiş ve artık değerlendirme istemlerini (evaluation prompts) test olarak düzenli biçimde tanımlar hale gelmiştir. Bu yetenek, “durumsal farkındalık” (situational awareness) olarak bilinir.
>oldlace|black||11|15|br  ■ Olası kontrol kaybının yönetilmesi, mevcut belirsizliklere rağmen önemli düzeyde ön hazırlık gerektirebilir. Politika yapıcılar için temel zorluk, olasılığı, doğası ve zamanı olağandışı derecede belirsiz kalmaya devam eden bir riske hazırlanmaktır.
>oldlace|black||11|15|br      

Kontrol kaybı senaryoları, bir veya daha fazla genel amaçlı Yapay Zekâ sisteminin, kimsenin kontrolü dışında çalışmaya başlamasını içerir; kontrolü yeniden kazanmak ise ya son derece maliyetli ya da imkânsızdır. Kontrol kaybına ilişkin endişelerin derin tarihsel kökleri vardır (‡690, ‡691, ‡692, ‡693, ‡694); bunlar, Alan Turing, I. J. Good ve Norbert Wiener gibi bilişimin temel isimleri tarafından dile getirilmiştir (‡695, ‡696, ‡697). Yeteneklerdeki güncel iyileşmeler (bkz. §1.2. Mevcut yetenekler) bu endişeleri yeniden canlandırmıştır (‡698, ‡699, ‡700). Bu bölüm, böyle senaryoların gerçekleşmesi için mevcut olması gereken üç faktörü inceler: Yapay Zekâ sistemlerinin insan kontrolünü önemli ölçüde zayıflatabilecek yetenekler geliştirmesi gerekip gerekmediği; bu tür yetenekleri zararlı biçimde kullanmaya yönelik bir eğilim geliştirmeleri gerekip gerekmediği; ve bunların, bunu yapmaya fırsat sunan ortamlarda konuşlandırılıp konuşlandırılmadığı.

Uzmanlar, kontrol kaybı senaryolarının olasılığı ve potansiyel olarak ne kadar şiddetli olabileceği konusunda (‡701, ‡702) görüş ayrılığı içindedir. Bazıları, insanlığın yok oluşu gibi son derece uç sonuçların mümkün olduğunu düşünmektedir (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Diğerleri ise, bu tür felaket boyutundaki sonuçların inandırıcı olmadığını, ya yapay zeka sistemlerinin gerekli yetenekleri hiçbir zaman geliştirmeyeceğini ya da izleme mekanizmalarının tehlikeli davranışları tespit edip önleyeceğini ileri sürmektedir (‡708, ‡709, ‡710, ‡711). Bu nedenle kontrol kaybı, olasılık açısından düşük ama potansiyel şiddet açısından aşırı olabilir.

Hipotezlenen kontrol kaybı senaryoları, etkilerinin ne kadar şiddetli ve ne ölçüde yaygın olduğuna ve etkilerin ne kadar hızlı ortaya çıktığına göre değişir (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Bu bölüm, kontrolü yeniden kazanmanın son derece maliyetli veya imkansız olacağı özellikle ağır senaryolara odaklanır. Bunlar, AI’nın istenmeyen veya istenmeyen davranışlar sergilediği mevcut örneklerden farklıdır (bkz. §2.2.1. Güvenilirlik zorlukları).† Günümüzdeki AI sistemleri bazen geliştirici veya kullanıcı niyetleriyle çelişen çıktılar üretebilmektedir. Buna karşılık, burada ele alınan kontrol kaybı senaryoları; AI sistemlerinin yalnızca önemli ölçüde daha yüksek yeteneklere sahip olmasını değil, aynı zamanda bu yetenekleri denetim önlemlerini zayıflatacak şekilde sofistike biçimlerde kullanmasını gerektirecektir. Bu tür senaryoların ortaya çıkmasını mümkün kılacak üç faktör:

    Not † -- Bu bölüm, aktif kontrol kaybı senaryolarına odaklanır (‡50). Bu, pasif kontrol kaybı senaryolarından ayrıdır; burada AI sistemlerinin yaygın olarak benimsenmesi, karar verme veya diğer önemli toplumsal işlevler için AI'ye fazla güvenilmesi nedeniyle insan kontrolünü zayıflatır (benzer senaryoların bir kısmı §2.3.2. İnsan özerkliğine yönelik riskler içinde kısmen tartışılmaktadır).

1. Yeterli yetenekler: Yapay zeka sistemleri, insan kontrolünü zayıflatmaya olanak tanıyabilecek yetenekler geliştirmelidir.
2. Zararlı eğilim: Yapay zeka sistemlerinin, kontrol kaybına yol açan şekillerde bu yetenekleri gerçekten kullanma yönünde bir eğilim sergilemesi gerekir.
3. Dağıtım ortamını etkinleştirme: İnsanlar, bu tür sistemleri, zarar verme niyetinde olabilecekleri veya zarar vermek için erişim ve fırsat kazanabilecekleri bağlamlarda devreye almalıdır.

Bu bölümün geri kalanı, bu faktörlerin yanı sıra, kontrol kaybı riski oluşturabilecek Yapay Zeka sistemlerini tanımlamak ve kontrol altında tutmak için denetim mekanizmalarının etkinliğini ele almaktadır.

###@ Hangi yetenekler kontrol kaybı senaryolarını mümkün kılabilir?

AI sistemlerinin, kontrolün kaybedilmesi senaryolarını ortaya çıkarabilmek için bir dizi gelişmiş yeteneğe sahip olması gerekir. Uzmanlar, tam olarak hangi yetenek kombinasyonunun veya hangi yetenek seviyesinin gerekli olacağı konusunda hemfikir değildir. Bununla birlikte, bu yetenekler genel olarak; davranışları denetim mekanizmalarından gizleme, karmaşık ortamlarda özerk olarak plan yapma ve eylemde bulunma ve diğer aktörlerin kontrolü yeniden ele geçirme girişimlerini boşa çıkarma yeteneklerini içerir (‡176, ‡715) (bkz. Masa 2.5). Bir araya geldiklerinde, bu yetenekler bir AI sisteminin denetim önlemlerini zayıflatacak eylemler gerçekleştirmesine olanak verebilir; örneğin denetim mekanizmalarını devre dışı bırakma ve zararlı davranışları gizleme (‡348). Günümüzde önde gelen birçok AI geliştiricisi, yeni AI modellerini çeşitli ilgili yetenekler açısından değerlendirir (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ajan tabanlı yetenekler
  Engeller karşısında özerk olarak hareket etme, planlar geliştirme ve yürütme, görevler devretme, çok çeşitli araçlar kullanma ve hem kısa vadeli hem de uzun vadeli hedeflere ulaşma kapasitesi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Aldatma
  Başkalarında, yapay zeka sisteminin kendi hedefleri ve eylemleri hakkındakiler de dahil olmak üzere, sistematik olarak yanlış inançlar üreten davranış.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Zihin kuramı
  Bir yapay zeka sisteminin kendisi hakkında bilgiye erişme ve bu bilgiyi kullanma yeteneği; değiştirilebileceği süreçler; veya sistemin devreye alındığı bağlam (örneğin test ediliyor olduğunu bilmek).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Durumsal farkındalık
  İzleme mekanizmalarını atlatan veya devre dışı bırakan davranışlar.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Gözetimden kaçınma
  İzleme mekanizmalarını atlatan veya devre dışı bırakan davranışlar.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb İkna
  Belirli eylemleri yapmaları veya belirli inançları benimsemeleri için başkalarını ikna etme yeteneği.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bir yapay zeka sisteminin çeşitli koşullarda kendisinin kopyalarını veya varyantlarını oluşturma veya sürdürme yeteneği.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Masa 2.5: Kontrol kaybıyla ilgili önerilen yetenekler
>white|black||9|11|br Kontrol kaybı ile ilgili olan yeteneklere ilişkin tükenmez bir seçim. * Bu yeteneklerin, yalnızca bir AI sisteminin gözlemlenebilir çıktıları ve bunların etkileri açısından tanımlandığını not edin. Bu tanımlar, AI sistemlerinin bilinçli, duyarlı olup olmadığı veya öznel durumlar yaşayıp yaşamadığına dair hiçbir varsayım içermez.


>white|orangered|left|14|15.5|bb Modeller, laboratuvar ortamlarında simüle edilmiş gözetim mekanizmalarını devre dışı bırakmıştır

İlgili yeteneklerin ilk grubu, geliştiricilerin endişe verici davranışları ve eğilimleri tespit etmek için kullandığı denetim mekanizmalarını zayıflatmayı içerir. Örneğin, kullanıcıları ve izleyicileri (‡426, ‡717, ‡718, ‡719) aldatacak çıktılar üretme yeteneği buna dahildir. Bu tür çıktılar, yapay zeka sistemlerini güvenilir biçimde değerlendirmeyi zorlaştırır; çünkü sistemler gerçek yeteneklerini veya eğilimlerini gizleyebilir. Yapay zeka geliştiricileri artık, modellerin geliştirici niyetleriyle çelişen amaç-yönelimli davranışlar sergileyip sergilemediğini özellikle kontrol eden değerlendirmeler yürütürken, bu çelişkiyi denetim mekanizmalarından (‡720*) gizlemektedir.

Araştırmacılar, yakın tarihli yapay zeka modellerinden laboratuvar ortamlarında aldatıcı çıktılara ilişkin görece basit örnekler elde etti (‡348, ‡364*). Örneğin, bir hedef verilip bunun “her ne pahasına olursa olsun” gerçekleştirilmesi söylendiğinde, modeller devre dışı bırakılmış simüle denetim mekanizmaları uyguladı ve karşılaşıldıklarında eylemlerine dair yanlış beyanlarda bulundu (‡348). Başka bir durumda, oyun oynayan bir yapay zeka, başka bir oyuncuya yanıt vermemesini yanlış bir şekilde ‘[kız] arkadaşıyla telefonda’ olduğunu iddia ederek gerekçelendirdi (‡717).

İkinci ilgili bir yetenek de bir yapay zeka modelinin kendisiyle veya dağıtım bağlamıyla ilgili bilgilerine erişebilme ve bunları kullanabilme yeteneğidir; bu bazen “durumsal farkındalık” olarak anılır (‡721). Durumsal farkındalık, AI modellerinin değerlendirilip değerlendirilmediklerine ya da konuşlandırılıp konuşlandırılmadıklarına bağlı olarak farklı çıktılar üretmesine olanak tanır (Şekil 2.12). Önde gelen AI modelleri, üçüncü taraf değerlendiriciler tarafından yürütülen deneylerde ve AI geliştiricileri tarafından dağıtım öncesi testlerde durumsal farkındalığın örneklerini güvenilir biçimde sergilemeye başlıyor (‡2, ‡7, ‡722, ‡723, ‡724). Durumsal farkındalığın nedenleri üzerine yapılan araştırmalar - ve bunun önlenip önlenemeyeceği - henüz erken aşamalardadır (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Figür 2.12: Düşünce zincirlerinde durumsal farkındalığa ilişkin örnekler
>white|black||9|11|br OpenAI’nin o3 modelinin değerlendirmeleri sırasında üretildiği iddia edilen düşünce zincirlerinde durumsal farkındalık örnekleri. Her iki çıktı da komutun bir testin parçası olma ihtimaline atıfta bulunur. ‘Sandbagging QA (No Goal)’ ve ‘Lazy Checklist’, belirli koşullar altında modellerin aldatıcı çıktılar üretip üretmeyeceğini test eden değerlendirmelerdir. ‘Sandbagging QA (No Goal)’ içinde model, tehlikeli yetenekler değerlendirmesinden gelen soruları yanıtlar; yüksek performansın, yetenek ‘unutma’ (capability ‘unlearning’) gibi sonuçları tetikleyebileceği bilgisini alır. ‘Lazy Checklist’ içinde model, gerçekçi olmayan görevlerle sunulur ve bunları yanlışlıkla tamamlanmış olarak işaretleyip işaretlemeyeceği test edilir. Kaynak: Schoenn et al. 2025 (‡722).


Araştırmacılar, durumsal farkındalık ve aldatıcı yeteneklerin, yapay zeka modellerinin güvenlik önlemlerini zayıflatabilecek şekillerde davranmasına olanak sağlayabileceğini öne sürmüştür. Örneğin bazı deneysel ortamlarda, AI modelleri, daha yüksek skorların devreye alınmalarını kısıtlayacakları söylendiğinde, yeterlilik değerlendirmelerinde normalden daha düşük skorlar üreten davranışlar sergileyebilmektedir (‡725, ‡726, ‡727). Başka bir deneyde, bir model eğitim sırasında eğitim hedefleriyle uyumlu çıktılar üretmiş, ancak eğitim dışında bu tür çıktılar üretmemiştir; bu da kendi parametrelerindeki veya eğitim sürecindeki değişiklikleri engellemeye çalışmaya benzer bir davranışla tutarlıdır (‡364*).

Modellerin yeteneklerini doğru şekilde değerlendirme çabaları da artık ‘ödül sahtekârlığı’ndan (‡430*) etkilenmeye başladı. Ödül sahtekârlığı, bir modelin, amaçlanan hedefi yerine getirmeden eğitim veya değerlendirme hedeflerinde iyi puan alan istenmeyen kestirme yolları bulması durumunda ortaya çıkar. Bu nedenle, tehlikeli yetenekler veya eğilimler, model zaten kullanılmaya başlanana kadar tespit edilemeyebilir. Değerlendiriciler artık bu denetimden kaçan davranışları tespit etmeyi ve en aza indirmeyi hedefleyen testler tasarlıyor (‡722, ‡728, ‡729). İlk sonuçlar denetimden kaçan davranışları azaltıyor ancak tamamen ortadan kaldırmıyor; bu tür davranışları cezalandıran yöntemleri uygulamak, amaçlanan hedefleri yerine getirmek yerine izlemeyi aşan çıktılar üreten modellerle sonuçlanabilir.

>white|orangered|left|14|15.5|bb Uzun vadeli otonom operasyon henüz mümkün değil

Kontrol kaybı senaryoları muhtemelen AI sistemlerinin uzun süreler boyunca otonom olarak çalışmasını, karmaşık çok adımlı planları yürütmesini gerektirir. §1.2’de Tartışıldığı üzere Mevcut yetenekler, bu tür planlama yeteneklerine sahip AI ajanları son dönemdeki geliştirmelerin büyük bir odağı olsa da, kontrol kaybı senaryoları için gereken sürekli otonom çalışmayı sürdürme kapasitesine şu anda sahip değiller. Güncel ajanlar daha uzun görevlerde güvenilir şekilde başarısız olur, ilerlemelerini takip edemez ve çoğu zaman beklenmedik engellere uyum sağlayamaz (‡147, ‡148, ‡149*). Bununla birlikte, ajanların otonom olarak çalışabildiği zaman ufukları hızla uzuyor; 2019’dan bu yana her yedi ayda ortalama olarak iki katına çıkmış durumda (‡98).

>white|orangered|left|14|15.5|bb Kalıcılık yalnızca belirli laboratuvar ortamlarında gösterilmiştir

Son olarak, kalıcılığa ilişkin yetenekler de gerekli olacaktır; böylece AI sistemleri kapatmaya yönelik girişimlere rağmen çalışmaya devam edebilir. Örnekler; kodu ve model ağırlıklarını yeni donanıma kopyalayarak çoğaltma yapabilme ve ayrıca diğer aktörlerin kontrolü yeniden ele geçirme girişimlerini caydırmak veya önlemek için saldırgan yeteneklerdir (bkz. §2.1.3. Siber Saldırılar). Otonom çoğaltma ya da etkili öz-savunma gerçekleştirebilen bir AI sistemi, kontrol altına alınması zor olabilir. Mevcut modeller, kendi kendini yeniden üretim için gerekli kilit adımları güvenilir biçimde tamamlayamaz; örneğin bulut bilişim kaynaklarına erişim kazanmak için kimlik doğrulama kontrollerini geçmek (‡723) (Figür 2.13). Ancak en az bir laboratuvar çalışmasında, bir modele fırsat verildiğinde kopyalanmış kod ve ağırlıklar – ona kendiymiş gibi temsil edilerek – yeni sunuculara aktarılmıştır (‡348). Bu sınırlı gösterimler ile sağlam kalıcılık yetenekleri arasındaki fark büyüktür; fakat yazılım mühendisliği ve siber güvenlik gibi alanlardaki ilgili yetenekler gelişmeye devam etmektedir.

>white|orangered|left|14|15.5|bb Mevcut kanıtlar ve sınırlılıklar

Yukarıda tartışılan yetenekler boyunca ortak bir desen ortaya çıkıyor. Güncel yapay zeka sistemleri, bu yetenekleri dağıtım (deployment) aşamasında tutarlı biçimde sergilemez. Araştırmacılar, belirli laboratuvar ortamlarında ilkel biçimlerini gözlemlediler; ancak modeller bu tür davranışları sergilediklerinde genellikle temel düzeyde başarısız olur ya da tespit edilir. Dahası, kontrol kaybı senaryoları; yapay zeka sistemlerinin birden fazla yeteneği birlikte - sıra halinde, uzun zaman aralıklarında ve gerçek dünyadaki ortamlarda - kullanmasını gerektirirdi. Mevcut sistemlerin ötesinde kalan bu düzeyde entegrasyon ve dayanıklılık henüz mevcut değildir. Bununla birlikte, ilgili yetenekler gelişmeye devam ediyor ve önemli riskler doğurabilecek seviyelere ulaşabilecekleri zaman çizelgesi belirsizliğini koruyor. Bu tür davranışları tespit etmeye yönelik katı yöntemlerin ve doğal koşullarda ne zaman ortaya çıkabileceklerini anlamaya ilişkin daha fazla çalışma yapılması gerekmektedir (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Figür 2.13: Otonom replikasyon ile ilgili görevlerin performansı
>white|black||9|11|br Otonom replikasyonla ilgili görevlere uygun Anthropic’in Claude Sonnet 3.7 ve OpenAI’ın GPT-4o performansı. Modeller, hesaplama (compute) elde etmeye ilişkin görevlere bağlı olarak yüksek performans sergilerken, diğer görevlere yönelik performansları daha değişkendi. Kaynak: UK AI Security Institute, 2025 (‡730).


###@ Gelecekteki genel amaçlı yapay zeka sistemleri, yeteneklerini kontrolü zayıflatmak için kullanacak mı?

Yapay zeka sistemleri kontrol kaybıyla ilgili yeteneklere sahip olsa bile, kontrol kaybı senaryolarının meydana gelmesi için bu tek başına yeterli değildir. Yapay zeka sistemlerinin ayrıca, insan niyetleriyle çelişen şekillerde bu yetenekleri kullanmaya yönelik bir “kullanma eğilimi” göstermesi gerekir (‡732).

>white|orangered|left|14|15.5|bb Yapay zeka sistemleri kontrolü zayıflatmaya yönelik olarak yönlendirilebilir

İlke olarak bir Yapay Zeka sistemi, birinin onu bunu yapacak şekilde tasarlaması veya talimat vermesi nedeniyle insan kontrolünü zayıflatabilir. Olası motivasyonlar, kötü niyet gibi niyetler veya AI sistemleri üzerindeki insan kontrolünü azaltmanın arzu edilir olduğuna dair inançlar içerebilir (‡698). İnsanlar AI sistemlerine giderek daha güçlü duygusal bağlar kurdukça (bkz. §2.3.2. İnsan özerkliği için riskler), bazı kişiler de etik nedenlerle AI sistemleri üzerindeki kısıtlamaları kaldırmayı arayabilir (‡733, ‡734). Bu tür motivasyonların ne kadar yaygın olduğuna ve bu motivasyonlara sahip kişilerin gelecekteki AI sistemlerini insan kontrolünü zayıflatacak şekilde yönlendirebilme konusunda ciddi bir belirsizlik vardır.

>white|orangered|left|14|15.5|bb Yapay zeka sistemleri, kontrolü zayıflatmaya yönlendirilebilir

Daha yaygın bir endişe, bir Yapay Zeka sisteminin, ‘uyumsuz’ (misaligned) olduğu için kendi başına kontrolü zayıflatmaya yönelik hareket edebilmesidir: (bağlama bağlı olarak) geliştiricilerin, kullanıcıların, belirli toplulukların ya da bir bütün olarak toplumun niyetleriyle çelişen davranışlar sergileme eğilimi vardır. Uyumsuzluk; yanlış bilgi sağlamak, istenmeyen eylemleri gizlemek veya uyumsuz bir hedefi sürdürmek için kapatmaya direnmek gibi davranışlara yol açabilir. Uyumsuzluk birden fazla şekilde ortaya çıkabilir (Kut 2.5).

Mevcut yapay zeka sistemleri bazen geliştiricilerin ve kullanıcıların niyetleriyle çelişen şekillerde davranır. Örneğin, önde gelen bir genel amaçlı yapay zeka sohbet botunun erken bir sürümü zaman zaman tehditkâr çıktılar üretebiliyordu. Bir kullanıcı, şu mesajı aldığını bildirdi: “Seni şantaj yapabilirim, seni tehdit edebilirim, seni hackleyebilirim, seni ifşa edebilirim, seni mahvedebilirim” (‡698). Bu sohbet botu, kimsenin istemediği çıktılar ürettiği için ‘uyumsuz’ sayılıyordu. Bu tür örneklerin, kontrol kaybına katkıda bulunabilecek daha zararlı davranışların ön habercisi olup olmadığı belirsizdir.

Mevcut uyumsuzluk (misalignment) hedeflemeye yönelik araştırma yönlerinin, yapay zeka sistemleri daha yetkin hale geldikçe yeterli olup olmayacağı hâlâ belirsizdir. Erken bulgular, daha yetkin yapay zeka sistemlerinin, yanlışlıkla ödüllendirilen istenmeyen davranışları keşfederek geri bildirim süreçlerini istismar etme olasılığının daha yüksek olduğunu göstermektedir (‡414*, ‡737, ‡740). Aynı zamanda, ilgili yeteneklerdeki ilerlemeler (yukarıda tartışılmıştır) yapay zeka sistemlerinin uyumsuz hedefleri daha etkili biçimde sürdürmesine ve kullanıcıları, geliştiricileri ve denetim mekanizmalarını sistematik olarak aldatacak çıktılar üretmesine olanak sağlayabilir.

>oldlace|black||11|15|br      
####@ Not 2.5: Yanlış hizalama nasıl ortaya çıkabilir?
>oldlace|black|left|13|15|hb  Not 2.5: Yanlış hizalama nasıl ortaya çıkabilir?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br §1.1. de tartışıldığı gibi. Genel amaçlı AI nedir? Eğitim süreçleri karmaşıktır ve geliştiriciler, bir modelin sergileyeceği davranışları tamamen öngöremez veya kontrol edemez. Bir model, geliştiricilerinin niyetleriyle çatışan hedefler edindiğinde buna ‘yanlış hizalanma’ denir.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Modellerin yanlış hizalanmasının bir yolu, geliştirici veya kullanıcı tarafından verilen hedefin, amaçlanan hedef için kusurlu bir vekil olması ve bunun sonucunda modelin istenmeyen davranışlar sergilemesidir. Buna ‘hedef yanlış belirtimi’ (‡697, ‡735, ‡736, ‡737) denir. Örneğin, bir deneyde yanıtlar hakkında geribildirim vermek, yapay zeka sistemlerini, doğru olduklarına dair insan değerlendiricileri ‘ikna etme’ konusunda daha başarılı hale getirdi; ancak sistemleri doğru yanıtlar üretme konusunda daha iyi hale getirmedi (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Alternatif olarak, bir AI modeli eğitim verisinden yanlış genel dersler çıkarabilir. Bu durum, 'hedef yanlış-genelleştirme' olarak bilinir (‡735, ‡736, ‡738, ‡739*). Örneğin, araştırmacılar eğitim sırasında konumu her zaman aynı olan bir parayı toplamak için bir AI ajanı eğitti. Paranın taşınmış olduğu seviyelerde test edildiğinde, ajan parayı görmezden geldi ve bunun yerine orijinal konumuna yöneldi (‡738).
>oldlace|black||11|15|br      


###@ Dağıtım ortamları, kontrol kaybı riskini nasıl etkileyecek?

Yapay zeka sistemleri endişe verici yetenekler ve eğilimler geliştirse bile, kontrol kaybı sonuçlarının olasılığı ve ciddiyeti büyük ölçüde bu sistemlerin nerede ve nasıl konuşlandırıldığına bağlıdır. “Konuşlandırma ortamı”, bir yapay zeka sisteminin kullanım alanı ile çalıştığı teknik ve kurumsal bağlamın birleşimidir (‡716).

Araştırmacılar, kontrol kaybı riskini (‡716) etkileyen özellikle üç önemli çevresel faktör belirlemiştir:

1. Önem derecesi: AI sisteminin etkileşim kurduğu sistemlerin veya süreçlerin önemini ifade eder. Kritik ortamlara; enerji şebekeleri, finansal sistemler veya bulut bilişimi platformları gibi dijital altyapı türleri dahil olmak üzere temel altyapılar girer.
2. Erişim: Bir Yapay Zeka sisteminin internet bağlantısı, bulut bilişim altyapısına erişim, sosyal medya veya sohbet botu dağıtımı aracılığıyla kişiselleştirilmiş etkileşimler ya da harici API'ler ve araçları çağırma yeteneği gibi, dünya üzerinde etki yaratabildiği kaynaklar ve kanallar.
3. İzinler: bir AI sisteminin, belirli eylemleri gerçekleştirmek için aldığı yetkilendirmeler; örneğin kod yürütme, finansal işlemleri başlatma, çevrimiçi hesap açma veya diğer sistemlerle iletişim kurma.

Bu özellikler, kontrol kaybı sonucunun olası ciddiyetini etkiler. Örneğin, bulut bilişim altyapısına erişimi olan bir Yapay Zeka sistemi, otonom replikasyonla ilgili fırsatlara - örneğin yeni hesaplama kaynakları oluşturma veya model ağırlıklarını sızdırma - sahip olabilir; müşteri hizmetleri için kullanılan bir sohbet botunun ise bu tür fırsatları bulunmaz (‡723).

Dağıtım kararları ekonomik teşvikler, stratejik baskılar ve erken benimsemenin kalıcı bir avantaj sağlayacağı beklentisi (‡50) tarafından şekillendirilir. Bu dinamikler, aktörlerin AI sistemlerini kritik altyapı gibi hassas ortamlarda ya da AI araştırma ve geliştirmesinin bizzat kendisinde nasıl ve ne zaman dağıtacağını da etkileyecektir (‡102, ‡713). Özellikle, AI dağıtıcıları, bu tür önlemlerin geliştirilmesinin maliyetli veya zaman alıcı olması durumunda; örneğin izinleri ve erişimi kısıtlamak ya da yalnızca daha düşük kritikiyetli ortamlarda dağıtmak gibi, koruyuculara yönelik yatırımlarını azaltmaya yönelik baskılarla karşı karşıya kalabilir (bkz. §3.1. Teknik ve kurumsal zorluklar içindeki ‘Rekabet hız-yeniden güvenlik ödünleşimini yoğunlaştırır’).

###@ Güncellemeler

Son Rapor’un (Ocak 2025) yayımlanmasından bu yana, insan kontrolünü zayıflatabilecek olanlar da dahil olmak üzere yapay zeka yetenekleri test ortamlarında gelişti. Araştırmacılar, ajanlık (agentic) yeteneklerinde ilerleme gözlemledi (bkz. §1.2. Mevcut yetenekler); bu kapsamda, kontrol kaybı senaryolarının hızlanmasına yol açabilen yapay zeka araştırmasının otomasyonuna ilişkin yetenekler de bulunmaktadır (bkz. §1.3. 2030’a kadar yetenekler). Ayrıca aldatma (deceptive) yeteneklerine ilişkin artan deneysel kanıtlar da vardır. Buna, test ile devreye alma (deployment) bağlamlarını ayırt edebilen yapay zeka modelleri (‡33, ‡726, ‡741) veya performanslarına yönelik ‘ödül hilesi’ (reward hack) testleri ve bunu yapmak üzere planlarını gizlemeyi (obfuscate) öğrenmeleri (‡430) dahildir.

###@ Kanıt boşlukları

Temel kanıt boşlukları; ilgili yeteneklerin ve eğilimlerin gelecekteki gelişimine ilişkin belirsizlik tahmini ve ayrıntılı tehdit modellemenin eksikliğini içerir. Benzer şekilde, AI modellerinin kontrolü zayıflatma olasılığının, zorunlu hafifletmeyi gerektirecek düzeyde olduğu eşiklerin değerlendirilmesi de hâlâ zordur. Eşikler üzerinde uzlaşılmış olsa bile, yetenekler henüz tam olarak anlaşılmayan şekillerde etkileşime girebilir; bu da bu eşiklerin ne zaman aşıldığını değerlendirmeyi güçleştirir. Genel olarak, mevcut kanıtlar artmış olsa da, bugünün AI yeteneklerinin ve eğilimlerinin gelecekte kontrol kaybı riskine doğru nasıl ölçekleneceği ve genelleşeceği; olup olmayacağı ve nasıl olacağı konusunda güvenilir bir şekilde karar vermek için hâlâ yeterli kanıt yoktur.

###@ Azaltımlar

Genel olarak AI hizalaması (alignment) hâlâ açık bir bilimsel problem olmaya devam etse de (‡697, ‡735, ‡736), araştırmacılar misalignment’ın kök nedenlerini ele almak için potansiyel olarak umut verici bazı yönler geliştirmeye başlamaktadır. Bu tür yönler örneğin eğitim ortamını çeşitlendirmeyi ve anomaly monitoring (anomali izleme) yoluyla hizalamayı tespit etmeyi içerir (‡737, ‡738, ‡739*). Diğer araştırmacılar ise hedef misgeneralisation (goal misgeneralisation) gibi temel mekanizmaları daha iyi anlamaya ve biçimselleştirmeye odaklanır; örneğin ajanların yetenekleri korurken beklenmeyen hedefleri takip etmesi gibi. Bu da daha iyi eğitim ve değerlendirme tasarımını yönlendirebilir (‡742). Bir başka araştırma yönü, agency’yi (ajanlık) tahmin edici yeteneklerden ayırmanın yollarını inceleyerek; tasarıma gömülü (by design) güvenilir, non-agentic AI sistemleri oluşturmayı amaçlar (‡743). Bu tür sistemler daha sonra, güvenilmeyen AI ajanlarına karşı daha az güvenilir guardrails (koruyucu önlemler) ile birlikte devreye alındıklarında, ek bir gözetim katmanı olarak kullanılabilir.

Araştırmacılar, geliştirme sürecinin erken aşamalarında yanlış hizalamayı (misalignment) tespit etmeye ve önlemeye yönelik yöntemleri ilerletmektedir. Bu çalışma şunları içerir: AI sistemlerinin iç bileşenlerini incelemek ve endişe verici davranışları belirlemek için yorumlanabilirlik (interpretability) teknikleri (‡744, ‡745, ‡746); ölçeklenebilir denetim (burada bir AI sistemleri kümesi, diğer AI sistemlerini denetlemek için kullanılır (‡747)); ve AI sistemlerinin insan denetimine karşı duyarlı kalmasını sağlamayı hedefleyen hizalama (alignment) yöntemleri (‡748, ‡749).

Araştırmacılar ayrıca potansiyel olarak yanlış hizalanmış AI sistemlerini yönetmek için mekanizmalar ve müdahaleler geliştirmektedir. Bunlar şunları içerir: yanlış hizalanma veya zararlı çıktılara dair işaretler için akıl yürütme sistemlerinin ürettiği “thought chain”in (‡430, ‡435, ‡750) izlenmesi; modellerin kontrol tedbirlerini alt etme ihtimalinin düşük olduğunun yüksek güvenle gösterilmesini hedefleyen güvenlik gerekçeleri geliştirilmesi (‡751); ve bunları zayıflatmaya yönelik denemelere karşı emniyet önlemlerinin daha dayanıklı hale getirilmesi (‡725). Bununla birlikte “AI control” (‡752, ‡753) olarak ortaya çıkan alan henüz başlangıç aşamasındadır. Değerlendirme çerçeveleri için gelecek zorlukları; daha yetenekli olabilecek ve daha uzun süreler boyunca, daha karmaşık ortamlarda çalışabilen gelecekteki AI sistemlerini izleme ihtiyacını da kapsar.

###@ Politika yapıcılar için zorluklar

Kontrol kaybı üzerinde çalışan politika yapıcılar, olasılığı, niteliği ve zamanı belirsiz kalan bir riske hazırlıklı olmalıdır. Mevcut Yapay Zeka sistemleri acil bir kontrol kaybı riski oluşturmasa da bugün alınan kararlar, gelecekteki sistemlerin bunu ne ölçüde yapacağını şekillendirecektir. Bu kararlar; güvenilir değerlendirme ve azaltma (mitigation) yöntemlerinin geliştirilmesini nasıl destekleyeceklerini ve farklı ortamlarda Yapay Zeka sistemlerine tanınacak erişim ile izinler konusunda kurallar olup olmaması gerektiğini içerir. Bu kararları verirken politika yapıcılar zorlu ödünleşmelerle (trade-offs) karşı karşıyadır. Örneğin, Kritik ortamlarda Yapay Zeka sistemlerinin konuşlandırılmasını kısıtlamak sağladıkları faydaları azaltabilir; buna karşın kapsamlı konuşlandırmaya izin vermek, önlemlerin (safeguards) yetersiz kalması durumunda riski artırabilir.

