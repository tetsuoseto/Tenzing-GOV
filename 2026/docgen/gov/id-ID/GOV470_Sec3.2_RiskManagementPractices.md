##########
>white|orangered|left|14|30|hr Bagian 3.2
### 3.2. Praktik manajemen risiko
>white|orangered|left|24|30|hb Praktik manajemen risiko

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informasi utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Manajemen risiko AI serbaguna mencakup berbagai praktik yang digunakan untuk mengidentifikasi, menilai, dan mengurangi risiko dari AI serbaguna. Praktik ini meliputi pengujian dan evaluasi tingkat model (seperti ‘red-teaming’), proses organisasi yang memandu keputusan pengembangan dan peluncuran, perlindungan bersyarat (seperti komitmen ‘jika-maka’), dan pelaporan insiden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejumlah pengembang AI telah menyusun Kerangka Kerja Keselamatan AI Frontier. Kerangka kerja ini mencakup informasi tentang penilaian risiko dan menetapkan langkah-langkah bersyarat, seperti pembatasan akses yang direncanakan perusahaan untuk diterapkan pada model yang lebih mampu. Kerangka kerja tersebut berbeda dalam hal risiko yang dicakup, cara mendefinisikan ambang batas kemampuan, dan tindakan yang dipicu ketika ambang batas tercapai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bukti mengenai efektivitas praktik manajemen risiko AI di dunia nyata masih terbatas. Kurangnya pelaporan dan pemantauan insiden menyulitkan penilaian tentang seberapa baik praktik saat ini mengurangi risiko atau seberapa konsisten praktik tersebut diterapkan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), manajemen risiko menjadi lebih terstruktur berkat inisiatif industri dan tata kelola yang baru. Instrumen baru seperti Kode Praktik AI Serbaguna Uni Eropa, Kerangka Tata Kelola Keselamatan AI Tiongkok 2.0, dan Kerangka Pelaporan Proses AI Hiroshima G7, bersama dengan inisiatif yang dipimpin perusahaan, menunjukkan tren menuju pendekatan yang lebih terstandardisasi terhadap transparansi, evaluasi, dan pelaporan insiden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dinamika pasar dan laju perkembangan AI menimbulkan tantangan tambahan. Tekanan persaingan dapat membuat perusahaan AI harus memilih antara merilis produk lebih cepat dan berinvestasi dalam upaya pengurangan risiko. Banyak dampak buruk terkait AI juga ditanggung oleh pihak eksternal, sementara tanggung jawab hukum atas dampak tersebut masih belum jelas, dan proses tata kelola dapat lambat beradaptasi dengan perubahan dalam lanskap AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tantangan utama bagi para pembuat kebijakan mencakup penentuan prioritas di antara beragam risiko yang ditimbulkan oleh AI serbaguna, serta penjelasan mengenai aktor mana di sepanjang rantai nilai AI yang paling mampu memitigasi risiko tersebut. Tantangan ini semakin besar karena terbatasnya visibilitas mengenai cara risiko diidentifikasi, dievaluasi, dan dikelola dalam praktik, serta berbagi informasi yang terfragmentasi antara pengembang, pihak penerap, dan penyedia infrastruktur.
>oldlace|black||11|15|br      


Manajemen risiko AI mencakup berbagai praktik yang bertujuan mengidentifikasi, menilai, dan mengurangi kemungkinan serta tingkat keparahan risiko yang terkait dengan sistem AI. Praktik-praktik ini dapat diterapkan oleh pengembang AI, pihak yang menerapkan AI, evaluator, dan regulator. Contohnya mencakup pemodelan ancaman, pengelompokan tingkat risiko, pengujian red team, audit, dan pelaporan insiden. Bagian ini menguraikan praktik manajemen risiko saat ini, perkembangan baru, dan keterbatasan yang masih ada.

Sejak awal 2025, sejumlah inisiatif internasional baru untuk manajemen risiko AI tujuan umum telah berkembang, termasuk kerangka kerja transparansi organisasi dan pelaporan risiko serta kerangka kerja regulasi dan tata kelola.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Gambar 3.4: Empat komponen manajemen risiko
>white|black||9|11|br Empat kategori metode untuk manajemen risiko AI serbaguna: identifikasi risiko; analisis dan evaluasi risiko; mitigasi risiko; dan tata kelola risiko. Semua ini membentuk proses iteratif dan siklis. Tata kelola risiko, yang ditampilkan di tengah, memfasilitasi keberhasilan komponen lainnya. Sumber: International AI Safety Report 2026.


Tantangan yang masih ada mencakup standardisasi yang terbatas, yang mempersulit kepatuhan dan penilaian, serta terbatasnya bukti mengenai efektivitas di dunia nyata. Selain itu, konteks kelembagaan, budaya, dan politik berbeda-beda di seluruh dunia, yang berarti bahwa pendekatan untuk mengidentifikasi dan mengelola risiko, termasuk ambang batas risiko yang dapat diterima, mungkin berbeda di berbagai wilayah. Pembahasan dalam bagian ini mengenai pendekatan pengelolaan risiko bersifat deskriptif: tujuannya adalah memberikan informasi kepada para pelaku dalam ekosistem AI mengenai pendekatan pengelolaan risiko yang saat ini diterapkan di seluruh dunia. Jika tersedia, bukti mengenai efektivitas dan keterbatasan pendekatan-pendekatan ini dibahas, tetapi rekomendasi kebijakan berada di luar cakupan karya ini.

###@ Komponen manajemen risiko

Manajemen risiko merupakan proses iteratif yang mencakup praktik dan metode di seluruh siklus pengembangan dan penerapan AI, yang bekerja bersama secara selaras (‡969). Manajemen risiko untuk AI serbaguna dapat melibatkan beragam peran, termasuk ilmuwan data, teknisi model, auditor, pakar bidang, eksekutif, pengguna akhir, komunitas terdampak, pemasok pihak ketiga, pembuat kebijakan, pemerintah, organisasi standardisasi, dan organisasi masyarakat sipil (‡970, ‡971, ‡972). Standar manajemen risiko terkemuka sering kali dapat dioperasikan bersama, tetapi menggunakan terminologi yang berbeda untuk menjelaskan elemen-elemen manajemen risiko (‡973, ‡974). Standar tersebut biasanya memiliki empat komponen yang saling terkait (Gambar 3.4): mengidentifikasi; menganalisis dan mengevaluasi; memitigasi; serta mengatur risiko (‡970, ‡973, ‡975, ‡976). Tabel-tabel di bawah ini memberikan contoh ilustratif tentang metode, teknik, dan alat yang relevan. Praktik terus berkembang, sehingga tabel-tabel tersebut tidak mencakup semuanya, dan penerapannya akan bervariasi di berbagai konteks.

###@ Identifikasi risiko

Identifikasi risiko adalah proses menemukan, mengenali, dan mendeskripsikan risiko. Identifikasi risiko yang komprehensif biasanya mencakup penilaian berbasis kapabilitas, yang menguji apakah model memiliki kapabilitas berbahaya tertentu (‡977), serta pemodelan risiko (‡978) dan peramalan (‡715*), yang digunakan untuk mengeksplorasi risiko yang ada dan yang sedang muncul. Tabel 3.1 menyajikan berbagai contoh praktik identifikasi risiko. Identifikasi risiko juga melibatkan para pakar dan komunitas terkait untuk memahami konteks yang lebih luas tentang bagaimana risiko muncul (‡979, ‡980). Mekanisme seperti program bug bounty dapat mendukung proses ini dengan memberikan insentif untuk mengidentifikasi kerentanan yang sebelumnya belum diketahui (‡981) (Tabel 3.1). Salah satu tujuan utama identifikasi risiko adalah mencakup risiko yang sudah dikenal dan dipahami dengan baik, serta potensi risiko masa depan yang masih tidak pasti atau belum dikarakterisasi dengan baik (‡982). Hal ini sangat penting untuk AI serbaguna, karena banyak risiko mungkin belum sepenuhnya dipahami atau dapat diamati (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Program bug bounty
  Program bug bounty atau pengungkapan kerentanan memberikan insentif kepada orang-orang untuk menemukan dan melaporkan kerentanan dalam sistem AI. Beberapa pengembang telah menerapkan program bug bounty (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Konsultasi ahli
  Pakar bidang, pengguna, dan komunitas terdampak memberikan wawasan tentang risiko yang mungkin terjadi. Pedoman untuk AI yang partisipatif dan inklusif mulai bermunculan (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Diagram tulang ikan (Ishikawa)
  Diagram tulang ikan merupakan alat analisis akar penyebab yang sudah mapan, dan para peneliti telah mengusulkan penggunaannya untuk menganalisis insiden risiko AI secara terstruktur (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Peramalan
  Peramalan adalah proses memprediksi peristiwa atau tren di masa depan berdasarkan analisis data masa lalu dan masa kini. Proses ini telah digunakan untuk membandingkan kemungkinan relatif dari, misalnya, berbagai dampak ekonomi akibat AI canggih (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Taksonomi risiko
  Taksonomi risiko merupakan cara untuk mengategorikan dan mengorganisasikan risiko berdasarkan berbagai dimensi. Ada beberapa taksonomi yang menguraikan risiko dari AI serbaguna (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perencanaan skenario
  Perencanaan skenario mencakup pengembangan skenario masa depan yang masuk akal dan analisis tentang bagaimana risiko terwujud. Pendekatan ini telah digunakan untuk mengeksplorasi risiko dan dampak model AI (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemodelan ancaman
  Pemodelan ancaman adalah proses untuk mengidentifikasi ancaman dan kerentanan pada suatu sistem. Banyak pengembang AI menyoroti penggunaan pemodelan ancaman untuk mengantisipasi skenario potensi penyalahgunaan sistem AI (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.1: Contoh identifikasi risiko dalam manajemen risiko AI serbaguna
>white|black||9|11|br Contoh metode untuk identifikasi risiko AI yang dicantumkan menurut urutan alfabet. Metode yang disertakan
dirancang untuk mendukung identifikasi berbagai jenis risiko, termasuk risiko akibat penggunaan berbahaya, malafungsi, dan risiko sistemik. Mengingat manajemen risiko AI serbaguna masih berada pada tahap awal, tidak semua metode akan sesuai untuk setiap pengembang atau penerap AI.


>white|orangered|left|14|15.5|bb Pemodelan ancaman dan taksonomi risiko merupakan metode identifikasi risiko yang utama.

Dua metode utama untuk mengidentifikasi risiko AI serbaguna adalah pemodelan ancaman International AI Safety Report 2026 (proses terstruktur untuk memetakan bagaimana risiko terkait AI dapat terwujud) dan taksonomi risiko. Meta, misalnya, menggunakan latihan pemodelan ancaman untuk mengantisipasi skenario potensi penyalahgunaan model AI-nya (‡990), dan Anthropic menyertakan pemodelan ancaman sebagai bagian dari Standar Penerapan ASL-3 (‡991). Taksonomi risiko dan bahaya AI, yang mencantumkan kategori risiko beserta contohnya, juga dapat menjadi titik awal untuk mengonseptualisasikan, mengidentifikasi, dan merinci risiko utama yang terkait dengan AI serbaguna dalam ranah penerapan tertentu (‡906, ‡988, ‡992, ‡993).

###@ Analisis dan evaluasi risiko

Analisis dan evaluasi risiko adalah proses menentukan tingkat risiko suatu model atau sistem AI dan membandingkannya dengan kriteria yang telah ditetapkan untuk menilai apakah risiko tersebut dapat diterima atau perlu dimitigasi (‡994, ‡995, ‡996, ‡997). Proses ini mencakup praktik seperti mengukur kinerja model pada tolok ukur (‡998) dan evaluasi (‡176, ‡715), melakukan latihan red teaming (‡999*), penilaian dampak (‡1000), dan audit (‡1001, ‡1002). Lihat Tabel 3.2 untuk contoh analisis dan evaluasi risiko AI serbaguna. Metode ini dirancang untuk mendukung analisis dan evaluasi berbagai jenis risiko secara bersamaan.

Tujuan utama analisis dan evaluasi risiko adalah melakukan evaluasi terhadap kapabilitas dan kerentanan model (‡1003), memanfaatkan pemodelan risiko yang kuat untuk menginformasikan keputusan tentang ambang batas risiko (‡1004, ‡1005), serta memahami bagaimana sistem AI digunakan dalam praktik guna menilai dampak sosial lanjutan (‡869, ‡904, ‡905, ‡1006). Proses analisis dan evaluasi risiko sering dianggap lebih mungkin mengidentifikasi risiko jika proses tersebut mencakup tinjauan independen (‡1001, ‡1007), memanfaatkan keahlian lintas sektor (‡1008), dan mencakup beragam perspektif dari berbagai bidang dan disiplin ilmu, serta dari komunitas yang terdampak (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audit
  Audit adalah tinjauan formal terhadap kinerja dan dampak model AI dan/ atau kepatuhan suatu organisasi terhadap standar, kebijakan, dan prosedur, yang dilakukan secara internal atau oleh pihak eksternal. Audit AI merupakan bidang yang terus berkembang, dan terdapat banyak alat serta praktik untuk mengaudit model AI dan praktik para pengembang model AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tolok ukur
  Tolok ukur adalah pengujian atau metrik standar, yang sering kali bersifat kuantitatif, dan digunakan untuk mengevaluasi serta membandingkan kinerja sistem AI pada serangkaian tugas tetap yang dirancang untuk merepresentasikan penggunaan di dunia nyata (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metode Bowtie
  Metode bowtie adalah metode yang dikenal luas untuk memvisualisasikan titik-titik tempat kontrol dapat ditambahkan guna memitigasi peristiwa risiko. Metode ini membedakan dengan jelas antara manajemen risiko proaktif dan reaktif (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Metode Delphi
  Metode Delphi adalah teknik pengambilan keputusan kelompok yang menggunakan serangkaian kuesioner untuk mengumpulkan konsensus dari panel ahli (‡1020, ‡1021). Metode ini telah digunakan untuk membantu mengeksplorasi kemungkinan masa depan dengan AI canggih (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengujian-lapangan
  Pengujian lapangan mengevaluasi kinerja dan dampak sistem AI dalam lingkungan operasional dunia- nyata. Beberapa penelitian menekankan pengujian lapangan sebagai pelengkap evaluasi model untuk menilai hasil dan konsekuensi di dunia nyata (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penilaian dampak
  Penilaian dampak menilai potensi dampak suatu teknologi atau proyek. Hal ini mungkin mencakup pengukuran, penggabungan, dan penentuan prioritas dampak. Sebagai contoh, EU AI Act mewajibkan pengembang sistem AI berisiko tinggi untuk melakukan Penilaian Dampak terhadap Hak-Hak Fundamental (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Evaluasi model
  Evaluasi model mencakup proses dan pengujian untuk menilai dan mengukur kinerja model AI dalam tugas tertentu. Ada banyak evaluasi AI untuk menilai berbagai kemampuan dan risiko, termasuk terkait keselamatan, keamanan, dan dampak sosial (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penilaian risiko probabilistik
  Penilaian risiko probabilistik adalah metodologi untuk mengevaluasi risiko yang terkait dengan sistem atau proses kompleks dengan memperhitungkan ketidakpastian. Metodologi ini telah diadaptasi untuk sistem AI tingkat lanjut (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengujian red-team
  Red-teaming adalah latihan ketika sekelompok orang atau sistem otomatis berpura-pura menjadi pihak lawan dan menyerang sistem teknologi suatu organisasi untuk mengidentifikasi kerentanan. Banyak perusahaan AI memiliki praktik internal untuk melakukan red-teaming terhadap sistem AI (‡458, ‡1028). Red-teaming juga dapat dilakukan oleh pihak di luar perusahaan. Tim-tim ini menghadapi tantangan seperti akses yang terbatas, tetapi juga dapat mengungkap wawasan yang berbeda (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Matriks risiko
  Matriks risiko adalah alat visual untuk membantu memprioritaskan risiko berdasarkan kemungkinan terjadinya dan potensi dampaknya (‡1027). Beberapa pengembang AI menyertakan matriks risiko dasar dalam Kerangka Kerja Keselamatan AI Frontier mereka (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ambang batas risiko/ tingkat risiko
  Ambang batas atau tingkatan risiko adalah batas kuantitatif atau kualitatif yang membedakan risiko yang dapat diterima dari yang tidak dapat diterima dan memicu tindakan manajemen risiko tertentu ketika terlampaui. Untuk AI tujuan umum, ambang batas atau tingkatan tersebut ditentukan berdasarkan kombinasi kemampuan, dampak, komputasi, jangkauan, dan faktor lainnya (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Toleransi risiko
  Toleransi risiko mengacu pada tingkat risiko yang bersedia diterima oleh suatu organisasi. Dalam AI, toleransi risiko sering kali ditetapkan secara implisit melalui kebijakan dan praktik perusahaan, sementara beberapa rezim regulasi secara eksplisit menetapkan risiko yang tidak dapat diterima dan mengaitkannya dengan konsekuensi hukum (‡1032). Beberapa perusahaan menjelaskan toleransi risiko mereka berdasarkan risiko marginal dari model baru; yaitu, sejauh mana suatu model secara kontrafaktual meningkatkan risiko di luar risiko yang telah ditimbulkan oleh model yang sudah ada atau teknologi lain (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kasus keselamatan
  Kasus keselamatan adalah argumen terstruktur, yang didukung oleh bukti, bahwa suatu sistem cukup aman untuk dioperasikan dalam konteks tertentu. Literatur terkini (‡1037, ‡1038, ‡1039) telah mengkaji kasus keselamatan untuk sistem AI terdepan, dan beberapa Kerangka Kerja Keselamatan AI Terdepan merujuknya (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Analisis keselamatan sistem
  Analisis keselamatan sistem menyoroti ketergantungan antara komponen dan sistem yang menjadi bagiannya, guna mengantisipasi bagaimana bahaya pada tingkat sistem dapat muncul akibat kegagalan komponen atau proses, maupun interaksi antara subsistem, faktor manusia, dan kondisi lingkungan. Pendekatan yang diterapkan pada sistem AI dalam literatur mencakup analisis proses teoretis sistem (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.2: Analisis/evaluasi risiko dalam manajemen risiko AI serbaguna
>white|black||9|11|br Contoh metode untuk analisis/evaluasi risiko AI, diurutkan menurut abjad. Mengingat manajemen risiko AI serbaguna masih dalam tahap awal, tidak semua metode akan sesuai untuk setiap pengembang atau penerap AI.


>white|orangered|left|14|15.5|bb Alat analisis risiko yang umum mencakup tolok ukur dan evaluasi model.

Tolok ukur dan evaluasi model adalah pengujian terstandardisasi untuk menilai kinerja sistem AI serbaguna pada tugas-tugas tertentu. Para peneliti telah mengembangkan beragam tolok ukur dan evaluasi, termasuk kumpulan soal pilihan ganda yang menantang, masalah rekayasa perangkat lunak, dan tugas terkait pekerjaan di lingkungan kantor simulasi (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Evaluasi kemampuan berbahaya (‡715) digunakan untuk menilai apakah model atau sistem AI serbaguna memiliki pengetahuan atau keterampilan yang sangat berbahaya, seperti kemampuan untuk membantu serangan siber (lihat §2.1.3. Serangan siber).

Keputusan yang sangat berdampak oleh perusahaan dan pemerintah mengenai perilisan model sebagian bergantung pada evaluasi ini (‡1050, ‡1051, ‡1052). Namun, tolok ukur sangat bervariasi dalam hal kualitas dan cakupan (‡998, ‡1003), dan validitasnya mungkin sulit dinilai karena berbagai kekurangan dalam praktik pembandingan (‡902, ‡909, ‡1003, ‡1053*). Sebagai contoh, tolok ukur dapat menjadi ‘jenuh’ – ketika skor banyak model mendekati skor tertinggi – yang berarti tolok ukur tersebut tidak lagi mampu membedakan model secara kuat. Model juga semakin mungkin mengidentifikasi tugas tertentu sebagai evaluasi dan menunjukkan perilaku yang berbeda dari perilaku mereka pada tugas serupa dalam konteks penerapan, karena ‘kesadaran situasional’ (lihat §2.2.2. Hilangnya kendali). Terakhir, keterbatasan tolok ukur dan evaluasi telah terdokumentasi dengan baik: khususnya, keduanya gagal menangkap risiko yang terkait dengan penggunaan AI serbaguna di ranah baru dan untuk tugas baru, karena kondisi pengujian berbeda-beda tingkatnya dari penggunaan di dunia nyata (‡913) (lihat §1.2. Kapabilitas saat ini dan §3.1. Tantangan teknis dan kelembagaan).

>white|orangered|left|14|15.5|bb Red-teaming memungkinkan penilaian risiko yang lebih domain- spesifik

Metode umum lainnya untuk menilai risiko adalah pengujian tim merah. ‘Tim merah’ adalah kelompok evaluator yang bertugas mencari kerentanan, keterbatasan, atau potensi penyalahgunaan. Pengujian tim merah dapat bersifat spesifik domain dan dilakukan oleh para ahli domain, atau terbuka untuk mengeksplorasi faktor risiko baru. Sebagai contoh, tim merah mungkin mengeksplorasi serangan ‘jailbreak’ yang mengakali pembatasan keselamatan model (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Berbeda dengan tolok ukur, keunggulan utama pengujian tim merah adalah bahwa tim merah dapat menyesuaikan evaluasi mereka dengan sistem spesifik yang sedang diuji. Sebagai contoh, tim merah dapat merancang masukan khusus untuk mengidentifikasi perilaku dalam skenario terburuk, peluang penyalahgunaan, dan kegagalan yang tidak terduga. Namun, metode ini mungkin memerlukan akses khusus ke model dan gagal mengungkap kelas risiko penting tertentu (‡999, ‡1028).

Yang penting, tidak ditemukannya risiko yang teridentifikasi tidak berarti bahwa risiko tersebut rendah: penelitian sebelumnya menunjukkan bahwa bug sering kali luput dari deteksi, khususnya ketika tim merah memiliki akses atau sumber daya yang terbatas (‡1060). Penelitian juga mempertanyakan apakah pengujian tim merah dapat menghasilkan temuan yang andal dan dapat direproduksi (‡1061). Komposisi tim merah dan instruksi yang diberikan kepada para penguji tim merah (‡1062), jumlah putaran serangan (‡1063), serta akses model ke alat (‡1064, ‡1065) dapat secara signifikan memengaruhi hasil, termasuk cakupan permukaan risiko. Pedoman komprehensif tentang pengujian tim merah bertujuan mengatasi beberapa tantangan ini (‡1066).

###@ Mitigasi risiko

Mitigasi risiko adalah proses memprioritaskan, mengevaluasi, dan menerapkan kontrol serta tindakan penanggulangan untuk mengurangi risiko yang telah diidentifikasi. Contohnya adalah kontrol akses (‡991), pemantauan berkelanjutan (‡986), dan komitmen jika-maka (‡700). Mitigasi risiko menimbulkan pertanyaan penting: tingkat risiko seperti apa yang dapat diterima? Kerangka kerja dan kebijakan perusahaan terbaru mulai merumuskan kriteria ‘penerimaan risiko’ (‡965, ‡1040). Namun, menetapkan ambang batas yang tepat masih menjadi tantangan, terutama untuk risiko yang berdampak luas pada masyarakat (‡986, ‡1067). Saat ini belum ada mekanisme yang mapan untuk memvalidasi keputusan penerimaan risiko yang dibuat oleh pengembang sebelum rilis (‡1005).

Metode mitigasi risiko yang dijelaskan dalam Tabel 3.3 di bawah ini dapat disesuaikan dan mampu memitigasi berbagai risiko, termasuk beberapa risiko yang tidak terduga. Tabel ini tidak mencakup metode mitigasi teknis seperti pelatihan adversarial, filter konten, dan pemantauan rantai pemikiran. Metode tersebut dibahas dalam §3.3. Perlindungan teknis dan pemantauan, serta di seluruh Laporan dalam paragraf ‘Mitigasi’ untuk setiap risiko di §2. Risiko.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kebijakan penggunaan yang dapat diterima
  Kebijakan penggunaan yang dapat diterima adalah serangkaian aturan dan panduan untuk penggunaan model AI yang bertanggung jawab, etis, dan legal. Para pengembang AI umumnya menerbitkan kebijakan penggunaan yang dapat diterima, serta kebijakan penggunaan yang dilarang, bersama peluncuran model baru (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kontrol akses/pemeriksaan pengguna
  Kontrol akses mencakup penggunaan kebijakan dan aturan untuk membatasi akses ke model AI, data, dan sistem berdasarkan peran pengguna, atribut, serta kondisi lainnya guna mencegah penggunaan tanpa izin, manipulasi, atau kebocoran data. Perusahaan AI sering menonaktifkan akun yang diketahui terlibat dalam aktivitas kriminal (‡486) dan melakukan pemeriksaan latar belakang pengguna serta pemeriksaan Know Your Customer untuk memastikan bahwa model hanya digunakan oleh pihak tepercaya (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Spesifikasi perilaku/model
  Spesifikasi perilaku AI adalah dokumen yang mendefinisikan bagaimana model AI seharusnya berperilaku dalam berbagai situasi. Dokumen ini berfungsi sebagai cetak biru untuk penyelarasan dan keselamatan AI, serta menjadi panduan dalam pengembangan, pelatihan, evaluasi, dan keluaran model. Beberapa perusahaan AI menggunakan dokumen spesifikasi model dan memublikasikan setidaknya sebagian isinya (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantauan berkelanjutan
  Pemantauan berkelanjutan adalah proses otomatis yang berlangsung terus-menerus untuk mengamati, menganalisis, dan mengendalikan sistem AI yang sedang digunakan, melacak kinerjanya, serta membatasi perilakunya guna memastikan keandalan, efektivitas, dan keamanan. Tersedia berbagai alat untuk pemantauan berkelanjutan (‡1073*) serta teknik untuk mendukung
Observabilitas AI (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pertahanan berlapis-lapis
  Pertahanan berlapis adalah gagasan bahwa beberapa lapisan pertahanan yang independen dan saling tumpang tindih dapat diterapkan sehingga jika salah satunya gagal, lapisan lainnya tetap efektif (‡1075, ‡1076). Beberapa Kerangka Kerja Keselamatan AI Frontier merujuk pada konsep ini (misalnya (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantauan ekosistem
  Ini adalah proses pemantauan ekosistem AI yang lebih luas, termasuk pelacakan komputasi dan perangkat keras, asal-usul model, asal-usul data, dan pola penggunaan. Literatur penelitian membahas pemantauan semacam ini dalam kaitannya dengan risiko dari AI serbaguna (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Komitmen jika-maka
  Komitmen jika-maka adalah serangkaian protokol teknis dan organisasional serta komitmen untuk mengelola risiko seiring meningkatnya kemampuan model AI. Beberapa pengembang AI menggunakan jenis komitmen ini sebagai bagian dari Kerangka Kerja Keselamatan AI Frontier mereka (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Batasan tegas atau larangan
  Garis merah adalah batasan spesifik yang dinyatakan dalam bentuk kemampuan, dampak, atau jenis penggunaan. Konsep ini muncul dalam pernyataan dan inisiatif publik, serta dalam larangan regulasi (‡1079, ‡1080, ‡1081). Literatur juga mencatat keterbatasan pendekatan garis merah, termasuk tantangan terkait konsensus dan keberlakuannya.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi rilis dan penerapan
  Strategi rilis dan penerapan AI serbaguna dapat mencakup penggunaan rilis bertahap atau akses API agar tersedia lebih banyak opsi mitigasi jika terjadi penyalahgunaan atau bahaya yang tidak terduga (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.3: Mitigasi risiko dalam manajemen risiko AI serbaguna
>white|black||9|11|br Contoh metode untuk mitigasi risiko AI yang diurutkan berdasarkan abjad. Metode yang disertakan dirancang untuk mendukung mitigasi berbagai jenis risiko secara bersamaan, termasuk risiko akibat penggunaan berbahaya, risiko akibat malfungsi, dan risiko sistemik. Mengingat manajemen risiko AI tujuan umum masih dalam tahap awal, tidak semua metode akan cocok untuk setiap pengembang atau pihak yang menerapkan AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Gambar 3.5: ‘Diagram keju Swiss’ yang menggambarkan pendekatan pertahanan berlapis
>white|black||9|11|br Beberapa lapisan pertahanan dapat mengimbangi kelemahan pada masing-masing lapisan. Teknik manajemen risiko AI saat ini memiliki kelemahan, tetapi menggabungkannya secara berlapis dapat memberikan perlindungan yang jauh lebih kuat terhadap risiko. Sumber: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Pertahanan berlapis dan strategi rilis merupakan alat mitigasi yang penting.

Model ‘pertahanan berlapis’ dapat mendukung manajemen risiko AI serbaguna. Dalam konteks ini, ‘pertahanan berlapis’ mengacu pada kombinasi langkah teknis, organisasional, dan sosial yang diterapkan di berbagai tahap pengembangan dan penerapan (Gambar 3.5). Artinya, menciptakan lapisan-lapisan perlindungan independen, sehingga jika satu lapisan gagal, lapisan lainnya tetap dapat mencegah bahaya. Contoh model pertahanan berlapis yang sering dikutip adalah beragam langkah pencegahan yang diterapkan untuk mencegah penyakit menular. Vaksin, masker, dan mencuci tangan, di antara langkah-langkah lainnya, jika dikombinasikan dapat mengurangi risiko infeksi secara signifikan, meskipun tidak satu pun metode ini 100% efektif jika digunakan sendiri (‡1083*). Untuk AI serbaguna, pertahanan- berlapis akan mencakup kontrol yang tidak diterapkan pada model AI itu sendiri, melainkan pada ekosistem yang lebih luas. Ini mencakup (misalnya) kontrol atas bahan yang diperlukan untuk melakukan serangan biologis, seperti reagen (‡1084, ‡1085). Namun, langkah pertahanan- berlapis terutama menangani risiko yang berkaitan dengan kecelakaan, malfungsi, dan penggunaan berbahaya, serta mungkin tidak terlalu berperan dalam mengelola risiko sistemik (lihat §3.5. Membangun ketahanan masyarakat).

Strategi rilis dan penerapan suatu perusahaan merupakan komponen penting dalam mitigasi risiko. Keputusan tentang cara model disediakan bagi pengguna dapat sangat memengaruhi paparan risiko (‡1082). Berbagai opsi rilis dan penerapan mencakup rilis bertahap kepada kelompok pengguna terbatas, akses melalui layanan daring yang terkontrol (seperti API), serta penggunaan perjanjian lisensi dan kebijakan penggunaan yang dapat diterima yang secara hukum melarang aplikasi berbahaya tertentu (‡176, ‡1086, ‡1087). §3.4. Model dengan bobot terbuka membahas secara lebih terperinci bagaimana perilisan bobot model memengaruhi risiko.

###@ Tata kelola risiko

Tata kelola risiko adalah proses yang menghubungkan evaluasi, keputusan, dan tindakan manajemen risiko dengan strategi dan tujuan suatu organisasi atau entitas lain (‡1088, ‡1089). Tabel 3.4 memberikan gambaran umum tentang teknik tata kelola risiko yang umum. Seperti yang ditunjukkan pada Gambar 3.4, tata kelola risiko dapat dipahami sebagai inti dari manajemen risiko karena tata kelola ini memfasilitasi pengoperasian komponen manajemen risiko lainnya secara efektif. Tata kelola risiko menyediakan akuntabilitas, transparansi, dan kejelasan yang mendukung pengambilan keputusan manajemen risiko berdasarkan informasi yang memadai. Tata kelola risiko dapat mencakup praktik seperti pelaporan insiden (‡1090), alokasi tanggung jawab risiko (‡965), dan perlindungan pelapor (‡1091). Secara lebih luas, tata kelola risiko dapat mencakup panduan, kerangka kerja, peraturan perundang-undangan, regulasi, standar nasional dan internasional, serta inisiatif pelatihan dan pendidikan. Salah satu tujuan utama tata kelola risiko adalah menetapkan kebijakan dan mekanisme organisasi yang memperjelas bagaimana tanggung jawab manajemen risiko dialokasikan di seluruh organisasi atau entitas lain, guna mendukung pengawasan dan akuntabilitas yang tepat (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentasi
  Praktik dokumentasi membantu melacak informasi penting tentang sistem AI, seperti data pelatihan, pilihan desain, penggunaan yang dimaksudkan, keterbatasan, dan risiko. ‘Kartu model’ dan ‘kartu sistem’, yang memberikan informasi tentang cara model atau sistem AI dilatih dan dievaluasi, merupakan contoh praktik terbaik dokumentasi AI yang menonjol (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pelaporan insiden
  Pelaporan insiden adalah proses mendokumentasikan dan membagikan secara sistematis kasus-kasus ketika pengembangan atau penerapan AI telah menyebabkan kerugian langsung atau tidak langsung. Terdapat beberapa platform yang memfasilitasi pelaporan insiden AI (‡1096, ‡1097), serta kerangka kerja untuk memfasilitasi pelaporan insiden AI yang lebih efektif (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kerangka kerja manajemen risiko
  Kerangka kerja manajemen risiko adalah rencana organisasi untuk mengurangi kesenjangan dalam cakupan risiko, mengoordinasikan berbagai aktivitas manajemen risiko, serta menerapkan mekanisme pengawasan dan keseimbangan. Kerangka kerja yang khusus untuk AI tujuan umum (‡986, ‡1098) sering merujuk pada langkah-langkah lain yang disebutkan di bagian ini.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Daftar risiko
  Daftar risiko adalah repositori berbagai risiko, prioritasnya, pemiliknya, dan rencana mitigasinya. Daftar ini relatif umum di banyak industri, termasuk keamanan siber (‡1099), dan terkadang digunakan untuk memenuhi persyaratan kepatuhan terhadap peraturan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alokasi tanggung jawab atas risiko
  Pembagian peran dan tanggung jawab untuk manajemen risiko dalam suatu organisasi dapat membentuk pengawasan internal terhadap pengambilan keputusan (‡1002, ‡1093). Pengaturan semacam itu tercermin dalam beberapa kerangka tata kelola, termasuk Kode Praktik AI Serbaguna Uni Eropa (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Laporan transparansi
  Laporan transparansi menjelaskan praktik manajemen risiko perusahaan AI dengan mengungkapkan informasi tertentu kepada publik atau membagikan dokumentasi kepada kelompok industri atau badan pemerintah. Sebagai contoh, banyak perusahaan AI menyerahkan laporan transparansi Hiroshima AI Process (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perlindungan bagi pelapor pelanggaran
  Karena sebagian besar pengembangan AI berlangsung secara tertutup, beberapa kerangka tata kelola mencakup perlindungan bagi pelapor pelanggaran agar mereka dapat mengungkapkan potensi risiko kepada pihak berwenang (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.4: Tata kelola risiko dalam manajemen risiko AI serbaguna
>white|black||9|11|br Contoh metode tata kelola risiko AI yang disusun menurut abjad. Metode yang tercantum dirancang untuk mendukung tata kelola berbagai jenis risiko secara bersamaan, termasuk risiko akibat penggunaan berbahaya, risiko akibat kegagalan fungsi, dan risiko sistemik. Mengingat manajemen risiko AI serbaguna masih berada pada tahap awal, tidak semua metode akan sesuai bagi setiap pengembang atau penerap AI.


>white|orangered|left|14|15.5|bb Dokumentasi dan transparansi merupakan komponen tata kelola risiko.

Mekanisme dokumentasi dan transparansi kelembagaan, bersama dengan praktik berbagi informasi, memfasilitasi pengawasan eksternal dan mendukung upaya untuk mengelola risiko yang terkait dengan AI serbaguna (‡1101, ‡1102). Menerbitkan hasil pengujian pra- penerapan dalam ‘kartu model’ atau ‘kartu sistem’, beserta detail dasar tentang model atau sistem tersebut, termasuk cara model atau sistem itu dilatih dan potensi keterbatasannya, telah menjadi praktik umum (‡1094, ‡1095). Beberapa pengembang juga menerbitkan laporan transparansi yang mencakup detail tentang praktik manajemen risiko mereka secara lebih luas (‡1103). Unsur dokumentasi dan transparansi lainnya mencakup pemantauan dan pelaporan insiden (‡176, ‡1083*, ‡1103) serta berbagi informasi, yang dapat difasilitasi oleh pihak ketiga seperti Frontier Model Forum. Beberapa kerangka peraturan, seperti EU AI Act atau Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) di California (‡1081, ‡1104), dalam kasus tertentu mewajibkan berbagi informasi tentang risiko AI serbaguna.

>white|orangered|left|14|15.5|bb Komitmen kepemimpinan dan insentif membentuk praktik manajemen risiko.

Budaya organisasi, struktur kepemimpinan, dan insentif memengaruhi upaya manajemen risiko dengan berbagai cara (‡1105). Komitmen kepemimpinan dan struktur insentif sering kali relevan terhadap penerapan kebijakan manajemen risiko dalam praktik. Beberapa pengembang memiliki panel pengambilan keputusan internal yang membahas cara merancang, mengembangkan, dan meninjau sistem AI baru secara aman dan bertanggung jawab. Komite pengawasan dan penasihat, lembaga perwalian, atau dewan etika AI juga dapat berfungsi sebagai mekanisme untuk memberikan panduan manajemen risiko dan melakukan pengawasan organisasi (‡1092*, ‡1106, ‡1107, ‡1108). Para peneliti berpendapat bahwa tantangan dalam tata kelola mandiri sukarela membuat audit, verifikasi, dan standardisasi oleh pihak ketiga berpotensi membantu memperkuat manajemen risiko AI tujuan umum (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Kerangka kerja manajemen risiko organisasi, transparansi, dan pelaporan risiko

Beberapa inisiatif baru berfokus pada proses manajemen risiko, dokumentasi, dan transparansi. Dalam bentuknya saat ini, Kode Praktik AI Serbaguna Uni Eropa berfungsi sebagai kerangka kerja sukarela untuk memandu praktik transparansi, hak cipta, keselamatan, dan keamanan guna mendukung kepatuhan terhadap ketentuan UU AI Uni Eropa untuk AI serbaguna (‡965). Per Desember 2025, lebih dari dua lusin perusahaan† telah menandatanganinya. Kerangka Pelaporan Proses AI Hiroshima G7 (HAIP) (‡1100) adalah kerangka kerja internasional pertama untuk pelaporan publik sukarela mengenai praktik manajemen risiko organisasi untuk sistem AI tingkat lanjut. Sedikitnya 20 pengembang telah menerbitkan laporan transparansi publik yang mencakup identifikasi risiko, metrik evaluasi, strategi mitigasi, dan proses keamanan data.

Para pengembang AI telah mengadopsi komitmen transparansi sukarela. Di Tiongkok, janji dari 17 perusahaan AI Tiongkok, yang dikoordinasikan oleh Aliansi Industri AI Tiongkok, dirilis pada Desember 2024 (‡1113) dan diperbarui pada 2025 (‡1114). Pada AI Seoul Summit Mei 2024 di Korea Selatan, 16 pengembang AI dari berbagai negara menandatangani komitmen sukarela untuk menerbitkan Kerangka Keselamatan AI Frontier bagi model dan sistem mereka yang paling mumpuni, serta menerapkan praktik manajemen risiko di seluruh tahap pengembangan dan penerapan model (‡1052).

    Catatan † -- Para penandatangan per December 2025 meliputi: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, dan WRITER.

>white|orangered|left|14|15.5|bb Kerangka Keselamatan AI Frontier telah menjadi pendekatan organisasi yang menonjol untuk pengelolaan risiko AI.

Sejak 2023, beberapa pengembang AI terdepan secara sukarela menerbitkan dokumen yang menjelaskan cara mereka berencana mengidentifikasi dan menanggapi risiko serius dari sistem mereka yang paling canggih. Kerangka Keselamatan AI Frontier ini menjelaskan rencana pengembang AI untuk mengevaluasi, memantau, dan mengendalikan model serta sistem AI mereka yang paling canggih sebelum dan selama penerapan. Kerangka-kerangka ini memiliki banyak kesamaan, tetapi berbeda dalam beberapa aspek penting (‡1115, ‡1116). Sebagian besar berfokus pada risiko yang terkait dengan ancaman kimia, biologis, radiologis, dan nuklir (CBRN), kemampuan siber tingkat lanjut, serta perilaku otonom tingkat lanjut (‡1115, ‡1117). Sebagian kecil kerangka membahas ranah risiko tambahan, seperti diskriminasi melanggar hukum dalam skala besar dan eksploitasi seksual anak.

Beberapa pengembang memperbarui kerangka kerja mereka pada 2025, dengan menambahkan bagian baru tentang manipulasi berbahaya, risiko ketidakselarasan, serta replikasi dan adaptasi otonom (‡1078, ‡1118). Meskipun banyak kerangka kerja menjelaskan pendekatan manajemen risiko yang serupa – termasuk pemodelan ancaman, red-teaming, dan evaluasi kemampuan berbahaya – pendekatan tersebut berbeda dalam definisi tingkat dan ambang batas risiko, frekuensi evaluasi, jarak antara evaluasi dan ambang batas, serta kelengkapan komitmen mitigasinya (misalnya, apakah komitmen tersebut mencakup penghapusan bobot model atau hanya penghentian sementara pengembangan) (‡1115, ‡1119). Lihat Tabel 3.5 untuk informasi lebih lanjut.

>white|orangered|left|14|15.5|bb Banyak tindakan dalam Kerangka Kerja Keselamatan AI Frontier didasarkan pada komitmen jika-maka.

Bagian penting dari Kerangka Keselamatan AI Frontier adalah ‘komitmen jika-maka’. Ini adalah protokol bersyarat yang memicu respons tertentu ketika model dan sistem AI mencapai ambang kemampuan yang telah ditetapkan sebelumnya (‡1120). Sebagai contoh, komitmen jika-maka dapat menyatakan bahwa jika suatu model terbukti mampu membantu pemula secara berarti dalam membuat dan mengerahkan senjata CBRN, maka pengembang akan menerapkan langkah-langkah keamanan yang lebih ketat, kontrol penerapan, dan pemantauan waktu nyata (‡991*).

Pada 2025, sejumlah pengembang AI mengumumkan bahwa model baru memicu peringatan dini atau bahwa mereka tidak dapat mengesampingkan kemungkinan bahwa evaluasi lebih lanjut akan menunjukkan bahwa model telah melampaui ambang kapabilitas. Hal ini mendorong mereka untuk menerapkan langkah-langkah perlindungan yang lebih ketat sebagai tindakan pencegahan (‡7, ‡33, ‡1121*). Kerangka Keselamatan AI Frontier umumnya mensyaratkan evaluasi kapabilitas awal sebelum mitigasi risiko, serta analisis risiko residual atau justifikasi keselamatan, yang sering kali didasarkan pada red teaming, setelah mitigasi. Lihat Tabel 3.5 untuk informasi terperinci.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Kerangka Kesiapsiagaan 2 (‡1078*)
  Risiko yang tercakup:
1. Kapabilitas biologis dan kimia
2. Kapabilitas keamanan siber
3. Kemampuan peningkatan diri AI
  Tingkat risiko atau yang setara serta langkah perlindungan terkait:
- Tinggi: Dapat memperkuat jalur yang sudah ada menuju bahaya serius (Memerlukan kontrol keamanan dan pengamanan)
- Kritis: Dapat memperkenalkan jalur baru yang belum pernah terjadi sebelumnya menuju bahaya parah (Hentikan pengembangan lebih lanjut sampai standar perlindungan dan kontrol keamanan yang ditentukan mencapai tingkat Kritis)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Kebijakan Penskalaan yang Bertanggung Jawab 2.2 (‡991*)
  Risiko yang tercakup:
1. senjata CBRN
2. Riset dan pengembangan AI otonom (AI R&D)
3. Operasi siber (sedang dalam penilaian)
  Tingkat risiko atau kategori yang setara dan langkah-langkah pengamanan terkait:
  Tingkat Keamanan AI (ASL)
- ASL-1: Tidak ada risiko katastrofik yang signifikan
- ASL-2: Tanda-tanda awal kemampuan berbahaya (Model harus memenuhi Standar Penerapan dan Keamanan ASL-2)
- ASL-3: Risiko penyalahgunaan katastrofik yang meningkat secara substansial (Model harus memenuhi Standar Penerapan dan/ atau Keamanan ASL-3)
- ASL-4+: Klasifikasi di masa mendatang (belum ditetapkan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Kerangka Keselamatan Frontier 3.0 (‡1040*)
  Risiko yang tercakup:
1. Penyalahgunaan
    a. CBRN
    b. Siber
    c. Manipulasi berbahaya
2. R&D pembelajaran mesin
3. Ketidakselarasan/ Penalaran instrumental
  Tingkat risiko atau kategori yang setara beserta perlindungan terkait:
  Tingkat Kapabilitas Kritis
    Tingkat kapabilitas yang pada tingkat tersebut, tanpa langkah mitigasi (kasus keselamatan untuk penerapan dan mitigasi keamanan yang selaras dengan tingkat keamanan RAND 2, 3, atau 4 (‡1122)), model atau sistem AI dapat menimbulkan risiko bahaya serius yang lebih tinggi. Tingkat kapabilitas tersebut mencakup ‘evaluasi peringatan dini’, dengan ‘ambang batas peringatan’ tertentu
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Kerangka Kerja AI Frontier 1.1 (‡990*)
  Risiko yang tercakup:
1. Keamanan siber
2. Risiko kimia dan biologis
  Tingkatan risiko atau yang setara dan langkah perlindungan terkait:
  Tingkat Ambang Risiko
- Sedang (rilis dengan langkah-langkah keamanan dan mitigasi yang sesuai)
- igh (jangan dirilis)
- Kritis (hentikan pengembangan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Kerangka Keselamatan Model Frontier (‡1123*)
  Risiko yang tercakup:
1. Proliferasi senjata CBRN
2. Operasi siber ofensif
3. R&D AI Otomatis
  Tingkat risiko atau yang setara beserta perlindungan terkait:
  Ambang Batas Kemampuan Kritis
    Kemampuan model yang berpotensi menyebabkan kerugian signifikan bagi masyarakat jika disalahgunakan. (Jika ambang batas terpenuhi atau terlampaui, model tidak akan diluncurkan ke publik tanpa langkah mitigasi risiko yang sesuai)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Kerangka Tata Kelola Frontier (‡1124*)
  Risiko yang tercakup:
1. senjata CBRN
2. Operasi siber ofensif
3. Otonomi tingkat lanjut (termasuk R&D AI)
  Tingkat risiko atau yang setara serta langkah perlindungan terkait:
  Tingkat Risiko
- Rendah atau Sedang (Penerapan diizinkan sesuai dengan persyaratan Program AI yang Bertanggung Jawab)
- Tinggi atau Kritis (Tinjauan lebih lanjut dan langkah mitigasi

diperlukan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Penilaian Risiko AI Frontier (‡1029*)
  Risiko yang tercakup:
1. Kejahatan siber
2. CBRN
3. Persuasi dan manipulasi
4. Diskriminasi yang melanggar hukum dalam skala besar
  Tingkat risiko atau yang setara beserta langkah-langkah pengamanan terkait:
  Ambang Batas Risiko – skor risiko model (MR)
- MR1 atau MR2 (Hasil evaluasi didokumentasikan oleh tim engineering)
- MR3 (Langkah-langkah mitigasi risiko dan hasil evaluasi didokumentasikan oleh tim rekayasa dan ditinjau secara berkala)
- MR4 (Penilaian risiko terperinci harus diselesaikan dan persetujuan pemimpin unit bisnis diperlukan)
- MR5 (Penilaian risiko yang terperinci harus diselesaikan dan disetujui oleh komite independen, misalnya komite etika AI NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Kerangka Kerja Model Frontier AI yang Aman (‡1125*)
  Risiko yang tercakup:
1. Penggunaan berbahaya (mis. malware, eksploitasi seksual anak)
2. Dampak merugikan dalam penggunaan biasa yang tidak bersifat jahat, misalnya keluaran yang mengakibatkan hasil diskriminatif ilegal atau pembuatan kode yang tidak aman

  Tingkat risiko atau yang setara beserta langkah pengamanan terkait:
  Kemungkinan dan Tingkat Keparahan Bahaya dalam Konteks
- Rendah
- Sedang
- Tinggi
- Sangat Tinggi
    (Mitigasi risiko dan kontrol keamanan telah diterapkan pada semua sistem dan proses; mitigasi tambahan perlu disesuaikan dengan sistem AI dan kasus penggunaan tempat model diterapkan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Kebijakan Kesiapan AGI (‡1127*)
  Risiko yang tercakup:
1. Kejahatan siber
2. R&D AI Otomatis
3. Replikasi dan adaptasi otonom
4. Bantuan terkait senjata biologis
  Tingkat risiko atau yang setara dan langkah-langkah perlindungan terkait:
  Ambang Batas Kemampuan Kritis
    Ambang kuantitatif pada tolok ukur kapabilitas (Jika terlampaui, lakukan evaluasi kapabilitas berbahaya, langkah-langkah keamanan informasi, dan mitigasi penerapan, atau hentikan pengembangan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: Kebijakan Kesiapan AGI (‡1127*)
  Risiko yang tercakup:
1. Kejahatan siber
2. R&D AI Otomatis
3. Replikasi dan adaptasi otonom
4. Bantuan terkait senjata biologis
  Tingkatan risiko atau yang setara beserta langkah perlindungan terkait:
  Ambang Batas Kemampuan Kritis
    Ambang kuantitatif pada tolok ukur kapabilitas (Jika terlampaui, lakukan evaluasi kapabilitas berbahaya, langkah-langkah keamanan informasi, dan mitigasi penerapan, atau hentikan pengembangan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Kerangka Keselamatan AI (‡1128*)
  Risiko yang tercakup:
1. Kehilangan kendali
2. Penyalahgunaan (misalnya, weaponisasi biokimia
  Tingkat risiko atau yang setara beserta langkah-langkah pengamanan terkait:
  Tingkat Risiko
- Risiko rendah (Terapkan sistem AI, tetapi lakukan pemantauan setelahnya untuk mengelola risiko)
- Risiko teridentifikasi (Buka sistem AI hanya bagi pengguna yang berwenang untuk memitigasi risiko, atau tunda penerapan hingga langkah-langkah keselamatan tambahan diterapkan, bergantung pada kasus penggunaan)
- Risiko tinggi (Jangan menerapkan sistem AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Kerangka Kerja Keselamatan AI Terdepan (‡1129*)
  Risiko yang tercakup:
1. Ancaman biologis
2. Keamanan siber ofensif
3. Operasi otonom dan manipulasi tingkat lanjut
  Tingkat risiko atau yang setara beserta langkah perlindungan terkait:
  Tingkat Risiko
- Level 1 (Perlindungan dasar untuk risiko minimal dan potensi dirilis sebagai sumber terbuka)
- Tingkat 2 (pemantauan waktu nyata, penyaringan prompt, deteksi anomali perilaku, kontrol akses, red-teaming, dan simulasi adversarial)
- Tingkat 3 (Pengamanan lanjutan termasuk red- teaming, peluncuran bertahap, pengujian adversarial, enkripsi, kontrol akses multipihak, dan arsitektur zero-trust)
- Level 4 (Protokol keselamatan maksimum untuk model berisiko tinggi dan langkah-langkah keamanan maksimum)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.5: Kerangka Kerja Keselamatan AI Frontier
>white|black||9|11|br Kerangka Kerja Keselamatan AI Frontier pertama yang telah dirilis oleh sebagian pengembang AI yang menandatangani Komitmen Keselamatan AI Frontier. Kerangka kerja tersebut mencakup risiko serupa (dengan sedikit variasi) dan menerapkan tingkatan risiko serta pendekatan manajemen risiko yang berbeda.


>white|orangered|left|14|15.5|bb Efektivitas Kerangka Kerja Keselamatan AI Frontier masih belum pasti.

Kerangka Keselamatan AI Frontier dapat berfungsi sebagai alat manajemen risiko dalam kondisi tertentu dan untuk kategori risiko tertentu yang memiliki jalur yang kredibel menuju bahaya (‡1117). Pada saat yang sama, beberapa analisis membahas pertanyaan mengenai kejelasan dan cakupannya (‡111, ‡986), serta ketangguhan ambang kemampuan AI dan risiko (‡1031, ‡1130). Kerangka yang ada cenderung berfokus pada sebagian ranah risiko. Akibatnya, beberapa risiko penting, seperti pengawasan yang melanggar hukum (‡1131, ‡1132) dan citra intim tanpa persetujuan (‡287), mendapat penekanan yang lebih sedikit. Berbeda dengan pendekatan manajemen risiko di sektor lain, seperti penerbangan atau tenaga nuklir (‡1133*), Kerangka Keselamatan AI Frontier biasanya tidak menggunakan ambang risiko kuantitatif yang eksplisit (‡1134).

Penilaian eksternal terhadap kepatuhan para pengembang terhadap Kerangka Keselamatan AI Frontier mereka sejauh ini masih terbatas, antara lain karena sebagian besar kerangka tersebut baru disusun, informasi yang tersedia untuk publik masih sedikit, dan belum ada audit eksternal yang terstandardisasi. Efektivitasnya juga akan dipengaruhi oleh seberapa baik dan sejauh mana komitmen tersebut diterapkan dalam praktik. Jika berdiri sendiri, kerangka-kerangka ini mungkin tidak dapat memastikan pengelolaan risiko yang efektif, karena dampak praktisnya bergantung pada seberapa baik dan sejauh mana kerangka tersebut diterapkan. Hingga saat ini, kerangka-kerangka tersebut belum sepenuhnya selaras dengan standar pengelolaan risiko internasional (‡1135). Sebuah studi tentang komitmen sukarela sebelumnya menemukan bahwa pemenuhan berbagai langkah tidak merata, yang menunjukkan bahwa kepatuhan terhadap komitmen sukarela kemungkinan akan berbeda-beda di antara perusahaan dan bidang (‡1109).

Jika dilihat secara keseluruhan, Kerangka Keselamatan AI Frontier merupakan bentuk manajemen risiko organisasi sukarela paling terperinci yang saat ini digunakan, tetapi sangat bervariasi dalam cakupan, ambang batas, dan daya penegakannya.

###@ Inisiatif regulasi dan tata kelola

>white|orangered|left|14|15.5|bb Beberapa yurisdiksi telah memberlakukan undang-undang dengan persyaratan transparansi.

Beberapa pendekatan regulasi awal memperkenalkan persyaratan hukum yang dimaksudkan untuk meningkatkan standardisasi dan transparansi dalam manajemen risiko. Undang-Undang AI Uni Eropa, yang mulai berlaku pada 2024, menetapkan persyaratan terkait transparansi, hak cipta, dan keselamatan untuk model AI tujuan umum. Pada 2025, Kode Praktik AI Tujuan Umum Uni Eropa diterbitkan untuk mendukung kepatuhan terhadap kewajiban ini dengan memberikan panduan tentang dokumentasi model dan hak cipta, serta – untuk model yang paling canggih – praktik manajemen risiko seperti evaluasi, penilaian dan mitigasi risiko, keamanan informasi, serta pelaporan insiden serius (‡965).

Contoh lain dari persyaratan regulasi baru mencakup Undang-Undang Kerangka Kerja Korea Selatan tentang Pengembangan Kecerdasan Buatan dan Pembentukan Kepercayaan, yang memperkenalkan persyaratan bagi sistem AI ‘berdampak tinggi’ di sektor-sektor kritis (‡1136), dan SB 53 California, yang menetapkan persyaratan transparansi terkait kerangka kerja keselamatan dan pelaporan insiden (‡1104). Mengingat persyaratan ini baru saja ditetapkan, masih terlalu dini untuk menilai secara terperinci bagaimana persyaratan tersebut akan memengaruhi praktik manajemen risiko atau hasil risiko yang sebenarnya.

>white|orangered|left|14|15.5|bb Inisiatif tata kelola yang lebih luas menawarkan panduan sukarela.

Sejumlah kerangka tata kelola regional dan antarregional kini merumuskan ekspektasi bersama untuk mengelola risiko AI serbaguna dengan memberikan panduan yang tidak mengikat bagi pembuat kebijakan dan organisasi. Kerangka Tata Kelola Keselamatan AI China 2.0, yang diterbitkan pada 2025, memberikan panduan terstruktur tentang kategorisasi risiko dan langkah penanggulangan di seluruh proses pengembangan dan penerapan AI (‡1137). Negara-Negara Anggota ASEAN menerbitkan ‘Panduan Perluasan ASEAN tentang Tata Kelola dan Etika AI (AI Generatif)’, yang memberikan panduan tentang tata kelola dan etika AI serbaguna serta ditujukan untuk mendukung penyelarasan kebijakan yang lebih besar di seluruh Negara-Negara Anggota ASEAN (‡1138). Selain itu, inisiatif yang dipimpin para pakar, seperti Konsensus Singapura, yang disusun oleh para ilmuwan AI dari berbagai negara, menguraikan prioritas penelitian untuk keselamatan AI serbaguna dalam bidang penilaian risiko, pengembangan, dan pengendalian (‡690).

###@ Pembaruan

Sejak penerbitan Laporan terakhir (Januari 2025), lanskap manajemen risiko untuk AI serbaguna telah berkembang, dengan diterbitkannya sumber daya baru seperti Kode Praktik AI Serbaguna Uni Eropa, Kerangka Kerja Pelaporan HAIP G7, Kerangka Kerja Tata Kelola Keselamatan AI Nasional Tiongkok 2.0, dan berbagai Kerangka Kerja Keselamatan AI Frontier dari pengembang AI. Inisiatif-inisiatif ini menjelaskan pendekatan dan praktik yang digunakan pengembang AI untuk mengelola risiko yang terkait dengan sistem AI serbaguna (‡1115). Terdapat variasi yang cukup besar di antara Kerangka Kerja Keselamatan AI Frontier dan laporan transparansi HAIP (‡1103), yang mencerminkan perbedaan dalam praktik organisasi, prioritas risiko, dan tahap awal ekosistem manajemen risiko AI serbaguna. Ekosistem tepercaya tempat berbagai pelaku AI menerapkan praktik manajemen risiko yang saling melengkapi di sepanjang siklus hidup dapat berkontribusi pada manajemen risiko yang efektif (‡690).

###@ Kesenjangan bukti

Masih kurang bukti mengenai cara mengukur tingkat keparahan, prevalensi, dan jangka waktu risiko yang muncul; sejauh mana risiko-risiko ini dapat dimitigasi dalam konteks dunia nyata; serta cara mendorong atau menegakkan penerapan mitigasi secara efektif di kalangan beragam pihak. Diperlukan lebih banyak penelitian untuk memahami seberapa umum berbagai risiko dan seberapa besar variasinya di berbagai wilayah dunia, terutama di wilayah seperti Asia, Afrika, dan Amerika Latin yang sedang mengalami digitalisasi dengan pesat. Seiring dengan semakin besarnya agensi dan kewenangan yang diberikan kepada model AI dan berkembangnya ilmu pengetahuan mengenai risiko AI serbaguna, pendekatan manajemen risiko juga perlu berkembang (‡639, ‡1139).

Langkah-langkah mitigasi risiko tertentu semakin populer (‡690, ‡956), tetapi diperlukan lebih banyak penelitian untuk memahami seberapa tangguh mitigasi risiko dan langkah pengamanan dalam praktiknya bagi berbagai komunitas dan aktor AI (termasuk usaha kecil dan menengah). Akses yang lebih luas terhadap data tentang penerapan dan penggunaan model di dunia nyata relevan untuk penilaian semacam itu. Selain itu, upaya manajemen risiko saat ini sangat bervariasi di antara perusahaan AI terkemuka. Ada anggapan bahwa insentif para pengembang tidak selaras dengan penilaian dan manajemen risiko yang menyeluruh (‡934). Masih terdapat kesenjangan bukti mengenai sejauh mana berbagai komitmen sukarela telah dipenuhi, kendala yang dihadapi perusahaan untuk mematuhi komitmen sepenuhnya, serta cara mereka mengintegrasikan Kerangka Kerja Keselamatan AI Frontier ke dalam praktik manajemen risiko AI yang lebih luas.

###@ Tantangan bagi para pembuat kebijakan

Tantangan utama mencakup menentukan cara memprioritaskan beragam risiko yang ditimbulkan oleh AI tujuan- umum, memperjelas pihak mana yang paling mampu memitigasi risiko tersebut, serta memahami insentif dan kendala yang membentuk tindakan mereka. Bukti menunjukkan bahwa saat ini pembuat kebijakan memiliki akses terbatas terhadap informasi tentang cara pengembang dan penerap AI menguji, mengevaluasi, dan memantau risiko baru, serta tentang efektivitas berbagai praktik mitigasi (‡1140). Peneliti dan pembuat kebijakan telah membahas upaya transparansi dan pelaporan insiden yang lebih sistematis sebagai cara yang mungkin untuk membantu menentukan prioritas risiko, mendorong kepercayaan, dan memberikan insentif bagi pengembangan yang bertanggung jawab (‡957). Dalam praktiknya, manajemen risiko melibatkan berbagai pihak di sepanjang rantai nilai AI – seperti penyedia data dan komputasi awan, pengembang model, serta platform hosting model – yang masing-masing memiliki peluang berbeda untuk menilai dan mengelola berbagai risiko (‡1141). Terbatasnya pertukaran informasi di antara para pihak ini menyulitkan penentuan risiko mana yang paling mungkin terjadi atau menimbulkan dampak terbesar, terutama jika dampak sosial di hilir turut dipertimbangkan.

