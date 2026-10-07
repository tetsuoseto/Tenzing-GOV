##########
>white|orangered|left|14|30|hr Seksyen 3.4
### 3.4. Model dengan pemberat terbuka
>white|orangered|left|24|30|hb Model dengan pemberat terbuka

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Maklumat utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tahap akses yang diberikan oleh syarikat AI kepada ‘pemberat’ model mereka mempengaruhi risiko yang ditimbulkan oleh model tersebut. Pemberat ialah parameter matematik yang membolehkan model AI memproses input dan menjana output. Bagi mana-mana model, syarikat boleh memilih untuk merahsiakan pemberat sepenuhnya, memberikan akses terhad kepada sesetengah pengguna, atau membenarkan sesiapa sahaja memuat turunnya sepenuhnya. Model yang pemberatnya tersedia kepada umum dipanggil ‘model berpemberat terbuka’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Model dengan pemberat terbuka memudahkan penyelidikan dan inovasi, tetapi langkah perlindungannya lebih mudah digugurkan. Di seluruh dunia, pelbagai pihak – terutamanya mereka yang mempunyai sumber yang lebih terhad – boleh menggunakan model dengan pemberat terbuka untuk tujuan penyelidikan dan komersial. Walau bagaimanapun, berbanding model dengan pemberat tertutup, model dengan pemberat terbuka lebih mudah diubah suai agar mempamerkan tingkah laku yang berpotensi memudaratkan, dan  s lebih sukar.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pelepasan model dengan pemberat terbuka tidak dapat dibatalkan. Setelah dilepaskan, pemberat model tidak boleh ditarik balik. Hal ini menyukarkan usaha mengurangkan potensi bahaya yang timbul akibat pelepasan model dengan keupayaan berbahaya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), keluaran utama model berpemberat terbuka telah merapatkan jurang keupayaan dengan model tertutup terkemuka. Pembangun dari China, DeepSeek dan Alibaba, masing-masing telah mengeluarkan model R1 dan Qwen, yang mencapai prestasi setanding dengan model tertutup terkemuka, manakala OpenAI telah mengeluarkan model berpemberat terbuka pertamanya sejak 2019. Keupayaan model tertutup terkemuka kini dianggarkan mendahului model berpemberat terbuka terkemuka kurang daripada satu tahun dalam penanda aras AI utama.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Cabaran dasar utama ialah mengakses manfaat yang diberikan oleh model berat terbuka sambil mengurus risiko tersendirinya. Salah satu pendekatan ialah menilai model berat terbuka dari segi ‘risiko marginal’: sejauh mana pelepasannya secara kontrafaktual meningkatkan risiko masyarakat melampaui risiko yang telah ditimbulkan oleh model sedia ada atau teknologi lain. Walau bagaimanapun, hal ini rumit dalam amalan. Peningkatan kecil dalam risiko marginal dari semasa ke semasa juga boleh terkumpul sehingga menyebabkan peningkatan besar dalam risiko keseluruhan.
>oldlace|black||11|15|br      


Model dengan pemberat terbuka, yang parameternya tersedia kepada orang ramai untuk dimuat turun, mempunyai implikasi tersendiri terhadap banyak cabaran yang dibincangkan dalam bahagian terdahulu. ‘Pemberat’ model AI mengandungi maklumat penting yang membolehkannya menjana respons yang berguna kepada pengguna. Setelah dikeluarkan, pemberat ini tidak dapat ditarik balik: sesiapa sahaja boleh memuat turun, mengkaji, mengubah suai, berkongsi dan menggunakannya pada komputer atau akaun awan mereka sendiri. Apabila pemberat tersedia secara terbuka, pihak lain dapat membina berdasarkan model itu dan mengubah suainya dengan lebih mudah, sekali gus memenuhi pelbagai keperluan dan mendorong inovasi (‡1317). Namun, melalui mekanisme yang sama, pengguna yang berniat jahat juga dapat menyingkirkan perlindungan dan mengubah suai model dengan pemberat terbuka dengan lebih mudah untuk kegunaan yang berbahaya (‡1122, ‡1160). Hal ini menimbulkan persoalan sama ada sesetengah model dengan pemberat terbuka patut tertakluk pada keperluan khas (cth. ujian yang lebih ketat sebelum dikeluarkan) atau, sebaliknya, diberikan pengecualian khas (cth. daripada keperluan pelaporan kawal selia) (‡1033).

###@ Latar belakang model dengan pemberat terbuka

>white|orangered||14|15.5|bb Model dengan pemberat terbuka boleh jadi, tetapi tidak semestinya, model ‘sumber terbuka’

Walaupun sering dirujuk sebagai ‘sumber terbuka’, kebanyakan model yang dikeluarkan kepada umum lebih tepat digambarkan sebagai ‘berat terbuka’. Hal ini kerana, walaupun pembangun menyediakan berat model, mereka tidak mengeluarkan kod latihan atau set data yang berkaitan. Tambahan pula, perisian sumber terbuka biasanya dicirikan oleh lesen permisif yang mengenakan keperluan minimum terhadap pihak hiliran yang menggunakan atau mengubah suai perisian tersebut (‡1318). Sebagai contoh, model Llama Meta mempunyai syarat lesen yang ketat dan hanya menyertakan kod inferens, bukannya kod latihan, maka model tersebut biasanya tidak dianggap sebagai sumber terbuka (‡1319, ‡1320). Pilihan pengeluaran model wujud dalam suatu spektrum daripada tertutup sepenuhnya hingga sumber terbuka sepenuhnya, dengan pertukaran antara risiko dan manfaat yang berbeza pada setiap titik (‡1086*, ‡1320, ‡1321). Meja 3.9 menerangkan pilihan ini.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Tertutup sepenuhnya
  Pengguna tidak boleh berinteraksi langsung dengan model sama sekali.
  Contoh: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Akses yang dihoskan
  Pengguna hanya boleh berinteraksi melalui aplikasi atau antara muka tertentu, seperti aplikasi chatbot mudah alih.
  Contoh: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Akses API kepada model
  Pengguna boleh menghantar permintaan kepada model melalui kod, membolehkannya digunakan dalam aplikasi luaran.
  Contoh: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Akses API kepada penalaan halus
  Pengguna boleh memperhalus model mengikut keperluan khusus mereka.
  Contoh: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Pemberat terbuka: pemberat tersedia untuk dimuat turun
  Pengguna boleh memuat turun dan menjalankan model tersebut pada komputer mereka sendiri.
  Contoh: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Pemberat, data dan kod tersedia untuk dimuat turun dengan sekatan penggunaan
  Pengguna boleh memuat turun dan menjalankan model serta kod inferens dan latihan, tetapi terdapat sekatan lesen tertentu terhadap penggunaannya.
  Contoh: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Terbuka sepenuhnya: pemberat, data dan kod tersedia untuk dimuat turun tanpa sekatan penggunaan
  Pengguna mempunyai kebebasan sepenuhnya untuk memuat turun, menggunakan dan mengubah suai model, kod penuh dan data.
  Contoh: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.9: Pilihan perkongsian model daripada tertutup sepenuhnya hingga terbuka sepenuhnya
>white|black||9|11|br Pilihan perkongsian model sebagai ilustrasi, daripada model yang tertutup sepenuhnya (model bersifat persendirian dan hanya digunakan secara proprietari) hingga model yang terbuka sepenuhnya dan sumber terbuka (pemberat model, data dan kod tersedia secara bebas kepada umum tanpa sekatan terhadap penggunaan, pengubahsuaian dan perkongsian). Model dalam empat kategori pertama sering dirujuk sebagai ‘tertutup’. Bahagian ini memfokuskan pada tiga baris paling bawah. Sumber: diadaptasi daripada Bommasani, 2024 (‡1317).


###@ Manfaat dan risiko

>white|orangered|left|14|15.5|bb Model berwajaran terbuka boleh disesuaikan dan dinilai dengan lebih mudah.

Model berpemberat terbuka menawarkan manfaat yang besar untuk penyelidikan, inovasi dan akses. Seperti yang dibincangkan dalam §1.1. Apakah AI tujuan umum?, latihan model AI tujuan umum amat mahal – model terkemuka menelan kos ratusan juta dolar untuk dibangunkan. Penerbitan pemberat model secara terbuka membolehkan pihak yang mempunyai sumber yang lebih terhad meniru, mengkaji dan membangunkan sistem sedia ada. Tanpa akses sedemikian, komuniti di wilayah yang kurang sumber berisiko tersisih daripada manfaat AI, menjadikan pemberat terbuka penting untuk membolehkan penyertaan majoriti global dalam pembangunan AI (‡1322). Pembangun hiliran boleh menala halus model untuk pelbagai aplikasi, contohnya, menyesuaikannya untuk bahasa minoriti yang kekurangan sumber atau mengoptimumkan prestasi bagi tugasan tertentu seperti penggubalan dokumen undang-undang atau pencatatan nota perubatan (‡1323, ‡1324*). Dengan cara ini, model berpemberat terbuka dapat membolehkan lebih ramai orang dan komuniti menggunakan AI dan mendapat manfaat daripadanya berbanding jika model sedemikian tidak tersedia (‡1325). Bagi model yang tidak cukup berkebolehan untuk mendatangkan bahaya, manfaat ini mungkin melebihi risiko tambahan akibat pemberatan model diterbitkan secara terbuka, walaupun hal ini bergantung pada toleransi risiko pihak pembuat keputusan yang berkaitan.

Pelepasan model dengan berat terbuka turut memperluas kumpulan pembangun dan penyelidik yang dapat mengkaji model tersebut, menilai keupayaannya, menguji kelemahannya dan mengulang penambahbaikan (‡1326, ‡1327). Hal ini meningkatkan kemungkinan aplikasi yang bermanfaat dan kelemahan yang memudaratkan dikenal pasti, walaupun perkara ini tidak terjamin (‡1328, ‡1329). Pengguna juga boleh menjalankan model dengan berat terbuka pada peranti mereka sendiri, sekali gus membolehkan mereka mengekalkan kawalan terhadap data sensitif dan mengelakkan penghantaran data tersebut ke pelayan pihak ketiga.

Terdapat manfaat tambahan apabila pembangun berkongsi maklumat seperti data latihan, kod, alat penilaian dan dokumentasi, selain pemberat model (‡1320, ‡1330, ‡1331, ‡1332*). Dengan lebih banyak maklumat, pembangun hiliran dan penyelidik lain dapat memahami model berpemberat terbuka dengan lebih baik dan menyesuaikannya untuk aplikasi baharu.

>white|orangered|left|14|15.5|bb Langkah perlindungan pada model dengan pemberat terbuka lebih mudah dibuang, sekali gus membuka peluang kepada penggunaan berniat jahat.

Model dengan pemberat terbuka juga menimbulkan risiko tambahan kerana perlindungannya lebih mudah dihapuskan. Walaupun model dengan pemberat terbuka dan model tertutup boleh mempunyai perlindungan untuk menolak permintaan pengguna yang berbahaya, perlindungan ini jauh lebih mudah dihapuskan daripada model dengan pemberat terbuka. Pelaku berniat jahat boleh melakukan penalaan halus pada model untuk mengoptimumkan prestasinya bagi aplikasi berbahaya, menghapuskan bahagian kod yang direka untuk mencegah penggunaan berbahaya, atau membatalkan penalaan halus keselamatan yang dilakukan sebelum ini (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Akibatnya, pemberat model terbuka boleh memburukkan risiko penyalahgunaan yang dibincangkan dalam §2.1. Risiko daripada penggunaan berniat jahat meningkat apabila lebih ramai pelaku dapat memanfaatkan dan menambah baik keupayaan sedia ada untuk tujuan berniat jahat tanpa pengawasan (‡1122, ‡1315). Walaupun ramai pengguna tidak mempunyai kemahiran atau dorongan untuk menghapuskan perlindungan pada model dengan pemberat terbuka, pelaku berniat jahat yang sangat bermotivasi tetap menimbulkan kebimbangan. Selain itu, pelaku berniat jahat juga mungkin dapat menggunakan model dengan pemberat terbuka untuk mengenal pasti kelemahan dalam model tertutup yang serupa (‡1055*). Kelemahan sedemikian lebih sukar ditemui dengan hanya menjalankan model tertutup, kerana penyedia model tertutup dapat melaksanakan langkah kawalan dan pemantauan yang lebih ketat.

>white|orangered|left|14|15.5|bb Perkongsian pemberat model tidak boleh ditarik balik.

Sebaik sahaja pemberat model tersedia untuk dimuat turun secara umum, tiada cara untuk melaksanakan penarikan balik secara menyeluruh bagi semua salinan sedia ada. Platform pengehosan Internet seperti GitHub dan Hugging Face boleh mengalih keluar model daripada platform mereka, sekali gus menyukarkan sesetengah pihak untuk mencari salinan yang boleh dimuat turun dan menjadi penghalang yang besar kepada ramai pengguna berniat jahat yang bertindak secara sambil lewa (‡1339). Walau bagaimanapun, pihak yang bersungguh-sungguh masih boleh mendapatkan salinan jika model itu telah dimuat turun dan dihoskan semula di tempat lain atau disimpan secara setempat. Selain itu, pembangun hiliran yang menyepadukan model pemberat terbuka ke dalam sistem mereka turut mewarisi sebarang kelemahan, seperti kerentanan terhadap serangan adversarial (‡1055) atau keupayaan model untuk memintas sistem pemantauan (lihat §2.2.2. Kehilangan kawalan) (‡1315). Tidak seperti model tertutup, yang hosnya boleh melancarkan pembaikan secara menyeluruh, pembangun model pemberat terbuka tidak dapat menjamin bahawa pengguna akan menggunakan kemas kini.

###@ Kemas kini

Sejak penerbitan Laporan terakhir (Januari 2025), jurang keupayaan antara model berpemberat terbuka terkemuka dengan model tertutup semakin mengecil. Pembangun dari China telah menjadi penyedia model berpemberat terbuka yang amat penting. Pada Januari 2025, DeepSeek mengeluarkan model R1, yang mencapai prestasi setanding dengan o1 keluaran OpenAI dalam beberapa penanda aras (‡1340). Model Qwen keluaran Alibaba juga semakin mendapat sambutan, menduduki tempat teratas bagi model berpemberat terbuka di Chatbot Arena, penanda aras prestasi yang digunakan secara meluas, setakat Ogos 2025 (‡1341, ‡1342*). Pada Ogos 2025, OpenAI mengeluarkan model berpemberat terbuka pertamanya sejak pengeluaran GPT-2 pada 2019, iaitu gpt-oss-120b dan gpt-oss-20b. Meta terus mengeluarkan model Llama dengan pemberat terbuka. Keupayaan model tertutup terkemuka kini dianggarkan mendahului model terbuka terkemuka kurang daripada setahun dalam penanda aras AI utama (Angka 3.10).

###@ Jurang bukti

Jurang bukti utama berkaitan keberkesanan penyelesaian teknikal dalam dunia sebenar untuk mencegah penyalahgunaan model dengan pemberat terbuka. Para penyelidik telah mencadangkan pelbagai pendekatan untuk menjadikan model tahan terhadap pengubahan. Ini termasuk teknik latihan baharu yang direka untuk menjadikan model tahan terhadap pengubahsuaian berbahaya (‡1276), menapis kandungan berbahaya daripada data latihan (‡55), dan pertahanan terhadap serangan jailbreak (‡675, ‡676). Teknik ini kini diterapkan dalam keluaran dunia sebenar daripada pembangun utama. Sebagai contoh, OpenAI menggunakan beberapa teknik ini dalam model gpt-oss mereka, dan melaporkan bahawa versi yang ditala halus secara adversarial tidak mencapai ambang keupayaan yang tinggi (‡1344*). Walau bagaimanapun, penyelidikan menunjukkan bahawa pihak berniat jahat boleh melumpuhkan perlindungan dengan melatih semula model menggunakan contoh berbahaya (‡1345, ‡1346). Tambahan pula, penilaian kebolehpercayaan perlindungan secara konsisten masih mencabar, menjadikan keberkesanannya terhadap serangan dunia sebenar tidak menentu (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Angka 3.10: Jurang keupayaan antara model AI berpemberat terbuka dan model AI tertutup terkemuka
>white|black||9|11|br Skor Indeks Keupayaan Epoch (ECI) bagi model berwajaran terbuka berprestasi terbaik (biru tua) dan model tertutup (biru muda) dari semasa ke semasa. ECI menggabungkan skor daripada 39 penanda aras ke dalam satu skala keupayaan umum. Model berwajaran terbuka terbaik ketinggalan kira-kira setahun berbanding model tertutup. Sumber: Epoch AI, 2025 (‡1343).


###@ Mitigasi

Mitigasi teknikal bagi risiko model dengan pemberat terbuka dilaksanakan sepanjang proses pembangunan dan penggunaan AI (‡1141, ‡1195, ‡1347). Sebagai contoh, semasa model dibangunkan, pembangun dan penyesuai hiliran boleh menapis kandungan sensitif daripada data latihan untuk meminimumkan keupayaan yang berbahaya. Membuang contoh berbahaya daripada data latihan model boleh mencegah penalaan halus adversarial dengan keberkesanan 10 kali ganda berbanding pertahanan yang ditambah selepas latihan, walaupun hal ini juga boleh menjejaskan keupayaan yang bermanfaat (‡55). Penyedia aplikasi AI juga boleh melaksanakan mekanisme pelaporan dan tindak balas terhadap insiden (‡1348).

Selain itu, platform pengehosan seperti HuggingFace dan GitHub boleh menetapkan syarat perkhidmatan platform untuk mengalih keluar model yang diubah suai bagi tujuan berbahaya (‡1141, ‡1324). Pembangun model boleh memberikan akses penuh kepada juruaudit sebelum pelancaran, atau memilih strategi pelancaran ‘berperingkat’ – dengan melancarkan model kepada kumpulan yang semakin besar (‡1086). Langkah ini dapat membantu mengenal pasti kemungkinan kerosakan fungsi atau kelemahan sebelum model tersedia secara meluas (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Nota 3.1: Keselamatan pemberat model
>oldlace|black|left|13|15|hb  Nota 3.1: Keselamatan pemberat model
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Risiko yang dibincangkan dalam bahagian ini mengandaikan bahawa pemberat model dikeluarkan dengan sengaja. Walau bagaimanapun, pemberat model tertutup juga boleh diakses melalui kecurian atau kebocoran. Pembangunan model tertutup menelan belanja ratusan juta dolar (§1.1. Apakah AI tujuan umum?) dan, secara purata, model ini lebih berkebolehan berbanding model berpemberat terbuka (‡1343). Hal ini menjadikannya sasaran yang menarik bagi pelaku, daripada penggodam amatur hingga negara berdaulat yang berusaha mendapatkan model AI terkemuka.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Pemberat model tertutup yang dicuri akan menimbulkan risiko yang serupa dengan risiko yang diterangkan di atas bagi model berpemberat terbuka, tetapi mungkin tanpa sebarang langkah mitigasi. Pelaku berniat jahat boleh menyingkirkan perlindungan daripada model yang paling berkebolehan. Tidak seperti pembangun yang sah, pelaku sedemikian tidak akan tertakluk pada kekangan reputasi, undang-undang atau komersial yang kini mendorong syarikat AI termaju untuk menggunakan model mereka dengan selamat.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Tahap keselamatan semasa berbeza-beza di seluruh industri, dan mungkin tidak mencukupi untuk menghadapi penyerang yang canggih. Sesetengah pembangun berikrar untuk melindungi pemberat model daripada sindiket jenayah siber dan ancaman orang dalam (‡582), manakala yang lain tidak membuat sebarang komitmen keselamatan secara terbuka (‡1109, ‡1349). Penyelidikan menunjukkan bahawa pusat data AI mungkin tidak mampu menahan serangan daripada pihak yang paling canggih dan mempunyai sumber yang mencukupi (‡582, ‡1350, ‡1351). Setakat Disember 2025, tiada kes kecurian pemberat model yang disahkan dan didokumenkan secara terbuka. Walau bagaimanapun, pelanggaran keselamatan lain di syarikat AI terkemuka telah dilaporkan, termasuk pencerobohan sistem e-mel Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Menutup jurang keselamatan ini memerlukan pelaburan besar dalam perkakasan, perisian, kakitangan dan keselamatan kemudahan. Sesetengah penambahbaikan keselamatan boleh dilaksanakan dengan agak cepat melalui usaha yang diselaraskan (‡1122). Namun, langkah kritikal yang lain, seperti mengamankan rantaian bekalan perkakasan dan kemudahan, mungkin mengambil masa bertahun-tahun (‡1122). Syarikat swasta juga mungkin kekurangan sumber atau maklumat untuk membangunkan perlindungan yang mencukupi secara bersendirian. Contohnya, pembangun AI tidak mempunyai akses kepada maklumat risikan ancaman terperingkat seperti yang dimiliki oleh kerajaan (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Cabaran bagi pembuat dasar

Cabaran utama bagi pembuat dasar ialah mendapatkan manfaat daripada perkongsian model berpemberat terbuka tanpa meningkatkan risiko dengan ketara. Untuk mengelakkan kemudaratan dahsyat, pembangun model berpemberat terbuka tidak sepatutnya mengeluarkan model tanpa menilai risikonya, menggunakan kaedah penilaian mapan yang digunakan untuk model tertutup serta ujian tambahan, memandangkan pelaku berniat jahat boleh memperhalus model dan menghapuskan perlindungan keselamatan. Dalam amalan, hal ini mungkin sukar kerana perkembangan keupayaan boleh menjadi tidak menentu, pengeluaran model berpemberat terbuka tidak boleh dipulihkan, dan usaha penilaian diperlukan untuk meramalkan bila sesuatu keluaran akan menimbulkan potensi kemudaratan yang ketara. Salah satu pendekatan ialah menilai ‘risiko marginal’ bagi keluaran terbuka: sejauh mana keluaran itu secara kontrafaktual meningkatkan risiko masyarakat melebihi risiko yang telah ditimbulkan oleh model sedia ada atau teknologi lain (‡556, ‡1033, ‡1354, ‡1355) (lihat §3.2. Amalan pengurusan risiko). Walau bagaimanapun, menganggarkan bagaimana sesuatu sistem akan meningkatkan atau mengurangkan risiko hiliran selepas digunakan adalah rumit dan bergantung pada konteks. Peningkatan risiko secara beransur-ansur melalui keluaran berturutan boleh terkumpul dari semasa ke semasa sehingga menyebabkan peningkatan besar dalam jumlah risiko, walaupun risiko marginal yang dikaitkan dengan setiap keluaran kelihatan boleh diterima (‡1356, ‡1357). Sifat dwiguna keupayaan AI turut merumitkan tadbir urus: ciri yang membolehkan aplikasi bermanfaat dalam bidang perubatan atau penyelidikan boleh digunakan semula untuk tujuan berbahaya, dan sebaik sahaja pemberat diterbitkan kepada umum, membezakan penggunaan yang sah daripada penggunaan berniat jahat mungkin sukar. Turut tidak jelas siapa yang patut dipertanggungjawabkan apabila model berpemberat terbuka diubah suai untuk tujuan berbahaya.

