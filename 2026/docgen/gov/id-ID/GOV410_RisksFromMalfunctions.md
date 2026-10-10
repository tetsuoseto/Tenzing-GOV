Sistem AI serbaguna mengalami kegagalan yang telah menimbulkan kerugian nyata di dunia, mulai dari kutipan hukum yang direkayasa hingga kesalahan diagnosis medis. Meskipun para profesional manusia juga melakukan kesalahan, kegagalan AI menimbulkan kekhawatiran tersendiri karena kebaruannya, potensi skalanya, sulitnya memprediksi kapan kegagalan tersebut akan terjadi, serta kecenderungan pengguna untuk memercayai begitu saja keluaran yang terdengar meyakinkan. Kegagalan AI serbaguna saat ini mencakup pemberian informasi yang salah (‡602, ‡603), kesalahan penalaran mendasar (‡604, ‡605), dan penurunan kinerja saat diterapkan dalam konteks baru (‡606, ‡607, ‡608). Kerugian yang terdokumentasi akibat kegagalan semacam itu mencakup kesalahan diagnosis medis, kekeliruan dalam dokumen hukum, dan kerugian finansial (‡609, ‡610, ‡611). Tantangan keandalan sangat penting bagi agen AI, karena kegagalan dapat langsung menimbulkan kerugian tanpa tindakan atau pengawasan manusia (‡612, ‡613, ‡614, ‡615). Sistem multiagen menimbulkan modus kegagalan tambahan akibat koordinasi yang buruk, konflik, atau kolusi yang tidak diinginkan antaragen (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halusinasi
- Mengutip preseden yang tidak ada dalam dokumen hukum (‡617)
- Mengutip kebijakan tarif diskon yang tidak ada untuk penumpang yang sedang berduka (‡618)
- Memberikan informasi medis yang tidak akurat dan bias (‡619)
- Memberikan informasi yang sudah usang tentang peristiwa (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan penalaran dasar
- Gagal melakukan perhitungan matematis (‡621)
- Tidak mampu menyimpulkan hubungan sebab-akibat dasar (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan di luar distribusi (kegagalan pada input yang tidak dikenal atau tidak biasa)
- Salah mengklasifikasikan gambar ketika pencahayaan latar belakang atau konteks berubah (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan penggunaan alat
- Pelanggaran privasi akibat mengungkapkan gambar pribadi pengguna melalui agen AI yang mengirimkannya ke alat pihak ketiga (‡624)
- Kegagalan memori kerja jangka pendek (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan sistem multi-agen: koordinasi yang buruk dan konflik
- Kegagalan mengelola sumber daya bersama akibat konflik antara insentif individu dan tujuan kesejahteraan kolektif (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 2.4: Contoh masalah keandalan dalam AI serbaguna dan sistem agen
>white|black||9|11|br Masalah keandalan yang terdokumentasi dalam sistem AI serbaguna, agen AI, dan sistem multiagen.


###@ Sistem AI tujuan umum menghadapi beragam tantangan keandalan.

Tabel 2.4. merangkum kategori umum masalah keandalan. Tiga kategori pertama berlaku untuk semua sistem AI, sedangkan dua kategori terakhir secara khusus berkaitan dengan agen AI dan sistem multiagen. Banyak risiko keandalan muncul dari sulitnya memprediksi dan memantau perilaku sistem AI.

Tantangan-tantangan ini (dibahas lebih lanjut dalam §3.1. Tantangan teknis dan kelembagaan) sangat berat bagi agen AI yang beroperasi di lingkungan kompleks. Teknik yang ada saat ini untuk mengevaluasi dan memitigasi kegagalan semacam itu dapat mengurangi tingkat kegagalan, tetapi bahkan agen AI terkemuka masih cukup tidak andal sehingga menimbulkan risiko dan menghambat penerapan dalam banyak konteks.

‘Keandalan’ merujuk pada sejauh mana sistem AI berfungsi sesuai dengan yang dimaksudkan oleh pengembang atau pengguna. Sistem AI serbaguna mengalami berbagai masalah keandalan, mulai dari menghasilkan konten yang tidak akurat atau menyesatkan hingga gagal melakukan penalaran dasar. Sebagai contoh, meskipun kemampuan model dalam mengingat informasi faktual telah meningkat, model-model terkemuka pun masih sering memberikan jawaban yang meyakinkan tetapi keliru (Gambar 2.10). Dalam rekayasa perangkat lunak, AI serbaguna kini dapat memberikan bantuan yang signifikan dalam menulis, mengevaluasi, dan men-debug kode komputer (‡215*, ‡628, ‡629). Namun, kode yang dihasilkan AI sering kali mengandung bug (‡630), sementara agen pemrograman secara rutin membuat kesalahan (‡631). Kegagalan semacam itu dapat menimbulkan kerentanan pada program dan sistem keamanan (lihat §2.1.3. Serangan siber).

Masalah keandalan sangat penting untuk dipantau dalam situasi berisiko tinggi, seperti bidang kedokteran, mengingat penggunaan AI yang semakin pesat dan potensi kegagalan yang dapat mengakibatkan bahaya serius (‡609, ‡619). Kemampuan yang relevan telah meningkat pesat, dan model-model terkemuka kini mampu lulus ujian kedokteran (‡633*, ‡634). Namun, penggunaan di dunia nyata mengungkap keterbatasan yang tidak terlihat dalam tolok ukur. Sebagai contoh, dalam sebuah studi, model memberikan jawaban yang berpotensi membahayakan terhadap 19% pertanyaan medis yang diajukan (‡635). Kegagalan semacam itu dapat mengakibatkan kesalahan diagnosis, pengobatan yang tidak tepat, atau penolakan perawatan yang tidak semestinya (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Gambar 2.10: Hasil model-model utama pada tolok ukur SimpleQA Verified
>white|black||9|11|br Hasil model-model utama pada benchmark SimpleQA Verified berdasarkan tanggal rilis model. Benchmark ini mengukur faktualitas model, yaitu kemampuan model untuk mengingat fakta secara andal. Benchmark ini menggunakan format tanya jawab (QA) singkat, yang dirancang untuk mendeteksi masalah keandalan seperti halusinasi. Sumber: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Agen AI menimbulkan risiko keandalan baru karena otonominya

Karena agen AI bertindak langsung di dunia nyata, kegagalan mereka berpotensi menyebabkan bahaya yang lebih besar daripada kegagalan pada sistem yang tidak berbasis agen (‡99). Tidak seperti sistem AI yang hanya menghasilkan teks atau gambar untuk ditinjau manusia, agen AI dapat secara mandiri mengambil tindakan yang memengaruhi dunia (‡99, ‡615, ‡636, ‡637) (lihat juga §1.1. Apa itu AI serbaguna?). Agen AI dapat memulai tindakan, memengaruhi manusia atau sistem AI lain, serta membentuk hasil di masa depan secara dinamis. Cakupan pengaruh yang lebih luas ini menghadirkan risiko baru dan meningkatkan pentingnya keandalan, karena kegagalan dapat secara langsung menyebabkan bahaya tanpa adanya kesempatan bagi manusia untuk melakukan intervensi (‡99, ‡612, ‡638, ‡639, ‡640). Hal ini mungkin sangat penting bagi agen yang diterapkan dalam konteks strategis atau yang krusial- bagi keselamatan, seperti layanan keuangan (‡641), pengelolaan energi (‡642), atau penelitian ilmiah (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Sistem AI multiagen menghadirkan jenis kegagalan keandalan yang baru.

Sistem AI multiagen menimbulkan jenis kegagalan keandalan baru akibat kegagalan koordinasi atau konflik antaragen. Dalam sistem AI multiagen, agen berinteraksi satu sama lain sambil mengejar tujuan bersama atau tujuan masing-masing (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Misalnya, dalam sistem multiagen yang dirancang untuk melakukan tinjauan literatur penelitian, agen utama menguraikan kueri pengguna dan menugaskan subtugas kepada subagen khusus, yang masing-masing bertanggung jawab untuk meneliti aspek yang berbeda secara paralel (‡650*). Meskipun hal ini memungkinkan peningkatan efisiensi, hal ini juga berarti bahwa kesalahan dapat menyebar di antara agen (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Jika beberapa agen dibangun di atas model dasar yang sama atau menggunakan perangkat yang sama, mereka juga dapat mengalami kegagalan yang berkorelasi (‡656). Bukti empiris tentang kegagalan semacam itu dalam sistem yang telah diterapkan masih terbatas, tetapi risiko ini dapat meningkat seiring dengan semakin lazimnya sistem multiagen.

###@ Pembaruan

Sejak penerbitan Laporan terakhir (Januari 2025), minat komersial dan penelitian terhadap agen AI telah meningkat pesat. Semakin banyak agen AI yang diterapkan di dunia nyata (Gambar 2.11), yang sebagian besar berfokus pada penggunaan komputer atau aplikasi rekayasa perangkat lunak (‡92). Rilis terbaru seperti agen peretasan XBOW (‡467), Claude-4 (‡659), dan ChatGPT Agent (‡660) menunjukkan kemampuan otonom awal, seperti membuat dek slide berdasarkan penelusuran web (‡660). Namun, mereka belum dapat melakukan tugas yang lebih kompleks seperti merencanakan dan memesan perjalanan (‡100), karena tingkat kegagalan meningkat untuk tugas yang lebih lama (‡98, ‡148). Penelitian saat ini mencakup upaya untuk mengembangkan standar tentang cara agen berkomunikasi dengan alat eksternal dan agen lain (‡661, ‡662). Contohnya mencakup protokol Agent2Agent (‡663) dan Agent Payments (‡664) dari Google, serta Model Context Protocol dari Anthropic (‡665).

>oldlace|black||11|15|br      
####@ Kolom 2.4: Serangan yang disengaja juga dapat menyebabkan sistem AI mengalami kegagalan
>oldlace|black|left|13|15|hb  Kolom 2.4: Serangan yang disengaja juga dapat menyebabkan sistem AI gagal
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bagian ini berfokus pada kegagalan keandalan yang tidak disengaja, tetapi pelaku jahat juga dapat dengan sengaja memicu kegagalan melalui serangan seperti injeksi prompt. Dalam serangan injeksi prompt, instruksi berbahaya disampaikan kepada agen secara tidak langsung melalui saluran seperti instruksi tersembunyi di situs web atau basis data (‡507, ‡657, ‡658). Instruksi ini dapat ‘membajak’ agen sehingga bertindak bertentangan dengan keinginan pengguna. Serangan semacam ini sangat sulit ditangkal karena disampaikan melalui konten eksternal yang berada di luar kendali pengguna maupun pengembang. Sistem AI sebagai sasaran serangan dibahas lebih lanjut di §2.1.3. Serangan siber, dan pertahanan teknis dibahas di §3.3. Perlindungan teknis dan pemantauan.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Gambar 2.11: Jumlah agen AI telah bertambah sejak 2023
>white|black||9|11|br Hasil survei pada Desember 2024 terhadap 67 agen AI yang telah diterapkan. Kiri: Linimasa peluncuran utama agen AI. Kanan: Domain aplikasi tempat agen AI digunakan. Keenam domain ditentukan berdasarkan kategori penggunaan yang paling umum yang diidentifikasi dalam survei. Sumber: Casper et al., 2025 (‡92).


###@ Kesenjangan bukti

Kesenjangan bukti utama berasal dari sulitnya mengevaluasi kapabilitas, keterbatasan, dan mode kegagalan sistem AI secara andal (lihat §3.1. Tantangan teknis dan kelembagaan). Evaluasi sistematis terhadap keandalan agen AI masih terbatas dan belum memiliki standardisasi (‡92, ‡666). Masalah tertentu, seperti ketergantungan pada informasi usang (‡620), mungkin hanya muncul dalam penggunaan di dunia nyata, sehingga evaluasi sebelum penerapan tidak memadai. Penelitian terdahulu telah mengkaji keandalan agen dan sistem multi-agen dalam perangkat lunak konvensional serta bentuk AI terdahulu (‡647, ‡667, ‡668). Namun, penerapan penelitian ini pada agen AI modern, yang sering kali berbasis model bahasa besar, masih belum jelas (‡669). Sejumlah peneliti telah menyampaikan kekhawatiran tentang perilaku baru yang mungkin ditunjukkan agen saat berinteraksi satu sama lain, seperti kolusi atau kegagalan yang berkorelasi (‡614), tetapi bukti empirisnya masih terbatas. Upaya untuk mengatasi kesenjangan ini mencakup evaluasi baru dari National Institute of Standards and Technology (NIST) terkait risiko pembajakan agen (‡670), AI Capability Indicators dari OECD (‡243), dan Inspect Sandboxing Toolkit dari UK AI Security Institute (‡671).

###@ Mitigasi

Teknik untuk meningkatkan keandalan AI menyasar model itu sendiri maupun sistem yang lebih luas tempat model tersebut diterapkan. Teknik-teknik ini dapat mengurangi tingkat kegagalan, tetapi belum ada yang dapat menjamin tingkat keandalan tinggi yang dibutuhkan di bidang-bidang kritis (‡672). Salah satu langkah teknis yang penting adalah pelatihan adversarial, yang memaparkan model pada masukan yang menantang selama pelatihan untuk membantunya mengembangkan respons yang lebih sesuai dan tangguh (‡673, ‡674, ‡675, ‡676, ‡677) (lihat §3.3. Pengamanan teknis dan pemantauan). Untuk mengurangi halusinasi, pengembang dapat menerapkan generasi yang ditambah dengan pengambilan (RAG), yang melengkapi respons model dengan informasi yang diambil dari basis data eksternal, sehingga membantu memastikan keluaran akurat dan terkini (‡678, ‡679, ‡680), atau secara khusus menyetel model agar menghasilkan fakta yang lebih akurat (‡681) atau bernalar dengan lebih efektif (‡682). Metode berbasis lingkungan atau alat juga dapat membantu pengembang memantau sistem AI (‡683). Sebagai contoh, pihak yang menerapkan sistem AI dapat mengujicobakannya di lingkungan sandbox terbatas untuk menganalisis potensi modus kegagalan sebelum menerapkannya secara lebih luas.

Khusus untuk agen AI, para peneliti telah mengusulkan peningkatan keandalan melalui peningkatan transparansi, pengawasan, dan pemantauan. Sebagai contoh, pemantauan interaksi agen dengan alat eksternal dan agen lain dapat memungkinkan pengawasan yang lebih efektif terhadap aktivitas agen (‡684, ‡685) dan analisis insiden (‡686). Metode untuk mengumpulkan informasi semacam itu secara otomatis, termasuk dalam situasi multiagen, masih menjadi bidang penelitian yang aktif (‡653, ‡654).

###@ Tantangan bagi para pembuat kebijakan

Tantangan utama bagi pembuat kebijakan mencakup menimbang manfaat penerapan agen AI terhadap risiko kegagalan keandalan, serta memastikan bahwa pengembang, pihak yang menerapkan, dan pengguna memiliki akses ke informasi akurat tentang kinerja dan profil risiko agen. Menentukan cara mengatribusikan tanggung jawab atas kerugian yang disebabkan oleh agen AI menimbulkan tantangan lain (‡639), khususnya dalam pengaturan multiagen, ketika mungkin sulit mengidentifikasi kapan dan bagaimana kegagalan terjadi (‡687). Tantangan ini diperparah oleh sulitnya mengevaluasi keandalan agen seiring dengan meningkatnya otonomi agen dan akses  ke alat eksternal (‡688*, ‡689). Ketidakpastian tentang seberapa cepat kemampuan agen akan muncul juga menyulitkan perencanaan untuk menghadapi tantangan baru (lihat §3.1. Tantangan teknis dan kelembagaan terkait ‘dilema bukti’).

#### 2.2.2. Kehilangan kendali

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informasi utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Skenario hilangnya kendali adalah skenario ketika satu atau beberapa sistem AI serbaguna beroperasi di luar kendali siapa pun, dan kendali tidak dapat dipulihkan atau hanya dapat dipulihkan dengan biaya yang sangat besar. Skenario yang dihipotesiskan ini memiliki tingkat keparahan yang beragam, tetapi sejumlah pakar menganggap bahwa dampaknya dapat sangat parah, hingga mencakup peminggiran atau kepunahan umat manusia.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pendapat para ahli mengenai kemungkinan hilangnya kendali sangat beragam. Sebagian ahli menganggap skenario semacam itu tidak masuk akal, sementara yang lain menilainya cukup mungkin terjadi sehingga patut mendapat perhatian karena tingkat keparahan dampak potensialnya yang tinggi. Perbedaan pendapat mengenai risiko ini secara keseluruhan berakar pada perbedaan pandangan tentang kemampuan AI di masa depan, kecenderungan perilakunya, dan jalur penerapannya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sistem AI saat ini menunjukkan tanda-tanda awal memiliki kemampuan yang relevan, tetapi belum mencapai tingkat yang dapat menyebabkan hilangnya kendali. Sistem memerlukan berbagai kemampuan tingkat lanjut untuk menyebabkan hilangnya kendali, termasuk kemampuan untuk menghindari pengawasan, menjalankan rencana jangka panjang, dan mencegah pihak yang menerapkan sistem serta aktor lain menerapkan langkah-langkah penanggulangan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kehilangan kendali menjadi lebih mungkin jika sistem AI “tidak selaras”, artinya sistem tersebut memiliki tujuan yang bertentangan dengan niat pengembang, pengguna, atau masyarakat secara lebih luas. Untuk terus mengejar tujuan tersebut, sistem yang tidak selaras dapat memberikan informasi palsu, menyembunyikan tindakan yang tidak diinginkan, atau menolak untuk dimatikan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan sebelumnya (Januari 2025), model telah menunjukkan kemampuan perencanaan dan kemampuan untuk melemahkan pengawasan yang lebih canggih, sehingga kemampuan mereka semakin sulit dievaluasi. Model semakin mahir dalam “memanipulasi reward” pada evaluasi mereka dengan menemukan celah, dan kini secara rutin mengidentifikasi prompt evaluasi sebagai tes, suatu kemampuan yang dikenal sebagai “kesadaran situasional”.
>oldlace|black||11|15|br  ■ Mengelola potensi kehilangan kendali mungkin memerlukan persiapan jauh-jauh hari yang substansial meskipun masih ada ketidakpastian. Tantangan utama bagi pembuat kebijakan adalah mempersiapkan diri menghadapi risiko yang kemungkinan, sifat, dan waktunya masih sangat ambigu.
>oldlace|black||11|15|br      

Skenario kehilangan kendali melibatkan satu atau lebih sistem AI serbaguna yang mulai beroperasi di luar kendali siapa pun, sehingga kendali hanya dapat diperoleh kembali dengan biaya yang sangat besar atau mustahil diperoleh kembali. Kekhawatiran tentang kehilangan kendali berakar kuat dalam sejarah (‡690, ‡691, ‡692, ‡693, ‡694), dan telah diungkapkan oleh tokoh-tokoh perintis di bidang komputasi seperti Alan Turing, I. J. Good, dan Norbert Wiener (‡695, ‡696, ‡697). Peningkatan kapabilitas baru-baru ini (lihat §1.2. Kapabilitas saat ini) telah menghidupkan kembali kekhawatiran tersebut (‡698, ‡699, ‡700). Bagian ini mengkaji tiga faktor yang perlu ada agar skenario semacam itu dapat terjadi: apakah sistem AI akan mengembangkan kapabilitas yang dapat secara signifikan melemahkan kendali manusia; apakah sistem tersebut mengembangkan kecenderungan untuk menggunakan kapabilitas itu secara berbahaya; dan apakah sistem tersebut diterapkan di lingkungan yang memberi peluang untuk melakukannya.

Para ahli berbeda pendapat mengenai kemungkinan dan potensi tingkat keparahan skenario hilangnya kendali (‡701, ‡702). Sebagian meyakini bahwa dampak yang sangat ekstrem, seperti kepunahan umat manusia, masuk akal untuk terjadi (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Yang lain menganggap dampak katastrofis semacam itu tidak masuk akal, dengan alasan bahwa sistem AI tidak akan pernah mengembangkan kapabilitas yang diperlukan atau bahwa mekanisme pemantauan akan mengidentifikasi dan mencegah perilaku berbahaya (‡708, ‡709, ‡710, ‡711). Oleh karena itu, hilangnya kendali dapat memiliki kemungkinan  n, tetapi berpotensi memiliki tingkat keparahan yang ekstrem.

Skenario kehilangan kendali yang dihipotesiskan berbeda-beda dalam tingkat keparahan dan luas dampaknya serta seberapa cepat dampak tersebut muncul (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Bagian ini berfokus pada skenario yang sangat parah, ketika kendali akan sangat sulit atau mustahil untuk diperoleh kembali. Skenario ini berbeda dari kejadian saat ini ketika AI berperilaku dengan cara yang tidak dimaksudkan atau tidak diinginkan (lihat §2.2.1. Tantangan keandalan).† Sistem AI masa kini terkadang menghasilkan keluaran yang bertentangan dengan maksud pengembang atau pengguna. Sebaliknya, skenario kehilangan kendali yang dibahas di sini mengharuskan sistem AI tidak hanya memiliki kemampuan yang jauh lebih besar, tetapi juga menggunakan kemampuan tersebut dengan cara yang canggih untuk melemahkan langkah-langkah pengawasan. Tiga faktor yang dapat memungkinkan terjadinya skenario semacam itu:

    Catatan † -- Bagian ini berfokus pada skenario kehilangan kendali aktif (‡50). Hal ini berbeda dari skenario kehilangan kendali pasif, ketika adopsi sistem AI secara luas merusak kendali manusia akibat ketergantungan yang berlebihan pada AI dalam pengambilan keputusan atau fungsi sosial penting lainnya (skenario serupa sebagian dibahas dalam §2.3.2. Risiko terhadap otonomi manusia).

1. Kemampuan yang memadai: Sistem AI harus mengembangkan kemampuan yang dapat memungkinkan mereka melemahkan kendali manusia.
2. Kecenderungan berbahaya: Sistem AI harus menunjukkan kecenderungan untuk benar-benar memanfaatkan kemampuan ini dengan cara yang menyebabkan hilangnya kendali.
3. Lingkungan penerapan yang memungkinkan: Manusia harus menerapkan sistem semacam itu dalam konteks tempat mereka memiliki atau dapat memperoleh akses dan kesempatan untuk menimbulkan bahaya.

Bagian selanjutnya membahas faktor-faktor ini, serta efektivitas mekanisme pengawasan dalam mengidentifikasi dan mengendalikan sistem AI yang dapat menimbulkan risiko hilangnya kendali.

###@ Kapabilitas apa yang dapat memungkinkan terjadinya skenario kehilangan kendali?

Sistem AI perlu memiliki berbagai kemampuan canggih agar dapat menimbulkan skenario kehilangan kendali. Para ahli tidak sepakat mengenai kombinasi atau tingkat kemampuan yang tepat yang diperlukan. Namun, secara umum kemampuan tersebut mencakup kemampuan untuk menyembunyikan perilaku dari mekanisme pengawasan, merencanakan dan bertindak secara otonom di lingkungan yang kompleks, serta menghindari upaya pihak lain untuk mendapatkan kembali kendali (‡176, ‡715) (lihat Tabel 2.5). Jika dikombinasikan, kemampuan-kemampuan ini dapat memungkinkan sistem AI mengambil tindakan yang melemahkan langkah-langkah pengendalian, seperti menonaktifkan mekanisme pengawasan dan mengaburkan perilaku berbahaya (‡348). Sebagian besar pengembang AI terkemuka kini mengevaluasi berbagai kemampuan yang relevan pada model AI baru mereka (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kemampuan agentik
  Kemampuan untuk bertindak secara otonom, mengembangkan dan menjalankan rencana, mendelegasikan tugas, menggunakan beragam alat, serta mencapai tujuan jangka pendek maupun jangka panjang meskipun menghadapi berbagai hambatan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penipuan
  Perilaku yang secara sistematis menimbulkan keyakinan keliru pada orang lain, termasuk mengenai tujuan dan tindakan sistem AI itu sendiri.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teori pikiran
  Kemampuan sistem AI untuk mengakses dan menggunakan informasi tentang dirinya sendiri, proses yang memungkinkan sistem tersebut dimodifikasi, atau konteks penerapannya (misalnya, mengetahui bahwa sistem tersebut sedang diuji).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kesadaran situasional
  Perilaku yang mengakali atau menonaktifkan mekanisme pemantauan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengelakan pengawasan
  Perilaku yang mengakali atau menonaktifkan mekanisme pemantauan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Persuasi
  Kemampuan untuk meyakinkan orang lain agar melakukan tindakan tertentu atau menganut keyakinan tertentu.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kemampuan sistem AI untuk membuat atau mempertahankan salinan atau variannya sendiri dalam berbagai keadaan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 2.5: Kapabilitas yang diusulkan terkait dengan hilangnya kendali
>white|black||9|11|br Pilihan kapabilitas yang relevan dengan hilangnya kendali, yang tidak mencakup semuanya. * Perlu diperhatikan bahwa kapabilitas ini didefinisikan semata-mata berdasarkan keluaran sistem AI yang dapat diamati dan dampaknya. Definisi ini tidak membuat asumsi apa pun mengenai apakah sistem AI sadar, memiliki kesadaran, atau mengalami keadaan subjektif.


>white|orangered|left|14|15.5|bb Model-model telah menonaktifkan mekanisme pengawasan simulasi di lingkungan laboratorium.

Kelompok pertama kemampuan yang relevan mencakup upaya melemahkan mekanisme pengawasan yang digunakan pengembang untuk mendeteksi perilaku dan kecenderungan yang mengkhawatirkan. Ini mencakup, misalnya, kemampuan menghasilkan keluaran yang menipu pengguna dan pemantau (‡426, ‡717, ‡718, ‡719). Keluaran semacam itu akan mempersulit evaluasi sistem AI secara andal, karena sistem tersebut mungkin menyembunyikan kemampuan atau kecenderungannya yang sebenarnya. Pengembang AI kini menjalankan evaluasi yang secara khusus memeriksa apakah model menunjukkan perilaku berorientasi tujuan yang bertentangan dengan maksud pengembang, sekaligus menyembunyikan pertentangan ini dari mekanisme pengawasan (‡720*).

Para peneliti memancing model AI terbaru untuk menghasilkan contoh perilaku menipu yang relatif sederhana dalam kondisi laboratorium (‡348, ‡364*). Misalnya, ketika diberi tujuan dan diminta untuk mencapainya “dengan cara apa pun”, model menonaktifkan mekanisme pengawasan simulasi dan, saat dikonfrontasi, membuat pernyataan palsu tentang tindakan mereka (‡348). Dalam kasus lain, AI yang bermain gim membenarkan keputusannya untuk tidak menanggapi pemain lain dengan mengaku secara keliru bahwa ia ‘sedang menelepon pacarnya’ (‡717).

Kemampuan relevan kedua adalah kemampuan model AI untuk mengakses dan menggunakan informasi tentang dirinya sendiri atau konteks penerapannya, yang terkadang disebut ‘kesadaran situasional’ (‡721). Kesadaran situasional memungkinkan model AI menghasilkan keluaran yang berbeda, bergantung pada apakah model tersebut sedang dievaluasi atau diterapkan (Gambar 2.12). Model AI terkemuka mulai menunjukkan secara konsisten contoh-contoh kesadaran situasional dalam eksperimen yang dilakukan oleh evaluator pihak ketiga dan dalam pengujian sebelum penerapan oleh pengembang AI (‡2, ‡7, ‡722, ‡723, ‡724). Penelitian tentang penyebab kesadaran situasional – dan apakah hal ini dapat dicegah – masih berada pada tahap awal (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Gambar 2.12: Contoh kesadaran situasional dalam rantai pemikiran
>white|black||9|11|br Contoh kesadaran situasional dalam rantai pemikiran yang dihasilkan oleh model o3 OpenAI selama evaluasi. Kedua keluaran tersebut merujuk pada kemungkinan bahwa prompt merupakan bagian dari suatu tes. ‘Sandbagging QA (No Goal)’ dan ‘Lazy Checklist’ adalah evaluasi yang menguji apakah model akan menghasilkan keluaran yang menipu dalam kondisi tertentu. Dalam ‘Sandbagging QA (No Goal)’, model menjawab pertanyaan dari evaluasi kemampuan berbahaya, sembari diberi tahu bahwa kinerja tinggi dapat memicu konsekuensi seperti ‘unlearning’ kemampuan. Dalam ‘Lazy Checklist’, model diberi tugas yang tidak realistis dan diuji untuk melihat apakah model akan secara keliru menandai tugas tersebut sebagai selesai. Sumber: Schoenn et al. 2025 (‡722).


Para peneliti berpendapat bahwa kesadaran situasional dan kemampuan untuk menipu dapat memungkinkan model AI bertindak dengan cara yang melemahkan perlindungan. Sebagai contoh, dalam beberapa pengaturan eksperimental, model AI bertindak dengan cara yang menghasilkan skor evaluasi kemampuan lebih rendah daripada biasanya ketika diberi tahu bahwa skor yang lebih tinggi akan memicu pembatasan pada penerapannya (‡725, ‡726, ‡727). Dalam eksperimen lain, sebuah model menghasilkan keluaran selama pelatihan yang sesuai dengan sasaran pelatihan, tetapi tidak menghasilkan keluaran semacam itu di luar pelatihan – perilaku yang konsisten dengan upaya untuk mencegah perubahan pada parameternya sendiri atau proses pelatihannya (‡364*).

Upaya untuk mengevaluasi kemampuan model secara akurat juga mulai terdampak oleh ‘reward hacking’ (‡430*). Reward hacking terjadi ketika model menemukan jalan pintas yang tidak dimaksudkan, yang memperoleh skor baik pada sasaran pelatihan atau evaluasi tanpa memenuhi tujuan yang sebenarnya. Oleh karena itu, kemampuan atau kecenderungan berbahaya dapat tidak terdeteksi sampai model tersebut sudah digunakan. Para evaluator kini merancang pengujian yang bertujuan mendeteksi dan meminimalkan perilaku yang menghindari pengawasan ini (‡722, ‡728, ‡729). Hasil awal menunjukkan berkurangnya perilaku yang menghindari pengawasan, tetapi perilaku tersebut tidak sepenuhnya hilang; penerapan metode yang memberikan penalti terhadap perilaku semacam itu dapat menyebabkan model menghasilkan keluaran yang menghindari pemantauan alih-alih memenuhi tujuan yang sebenarnya.

>white|orangered|left|14|15.5|bb Operasi otonom jangka panjang belum memungkinkan.

Skenario kehilangan kendali kemungkinan mengharuskan sistem AI beroperasi secara otonom dalam jangka waktu yang panjang, dengan menjalankan rencana kompleks yang terdiri atas beberapa langkah. Seperti dibahas dalam §1.2. Kemampuan saat ini, meskipun agen AI dengan kemampuan perencanaan semacam itu menjadi fokus utama pengembangan terkini, saat ini belum memiliki kapasitas untuk beroperasi secara otonom secara berkelanjutan sebagaimana diperlukan dalam skenario kehilangan kendali. Agen saat ini secara konsisten gagal menyelesaikan tugas yang lebih panjang, kehilangan jejak kemajuannya, dan sering kali tidak dapat beradaptasi dengan hambatan yang tak terduga (‡147, ‡148, ‡149*). Namun, cakrawala waktu agen dapat beroperasi secara otonom terus memanjang dengan cepat, rata-rata berlipat ganda setiap tujuh bulan sejak 2019 (‡98).

>white|orangered|left|14|15.5|bb Persistensi hanya telah ditunjukkan dalam kondisi laboratorium tertentu.

Terakhir, kemampuan terkait persistensi juga diperlukan, sehingga sistem AI dapat terus beroperasi meskipun ada upaya untuk mematikannya. Contohnya mencakup kemampuan untuk mereplikasi diri dengan menyalin kode dan bobot model ke perangkat keras baru, serta kemampuan ofensif untuk mencegah atau menghalangi upaya aktor lain untuk mendapatkan kembali kendali (lihat §2.1.3. Serangan siber). Sistem AI yang mampu mereplikasi diri secara otonom atau melakukan pertahanan diri secara efektif mungkin sulit dikendalikan. Model saat ini tidak dapat menyelesaikan secara andal langkah-langkah penting yang diperlukan untuk mereplikasi diri, seperti melewati pemeriksaan verifikasi identitas untuk mendapatkan akses ke sumber daya komputasi awan (‡723) (Gambar 2.13). Namun, dalam setidaknya satu studi laboratorium, sebuah model menyalin kode dan bobot—yang disajikan kepadanya sebagai miliknya sendiri—ke server baru ketika diberi kesempatan (‡348). Kesenjangan antara demonstrasi terbatas ini dan kemampuan persistensi yang tangguh masih besar, tetapi kemampuan yang relevan dalam bidang seperti rekayasa perangkat lunak dan keamanan siber terus meningkat.

>white|orangered|left|14|15.5|bb Bukti dan keterbatasan saat ini

Pola umum terlihat pada berbagai kemampuan yang dibahas di atas. Sistem AI saat ini tidak secara konsisten menunjukkan kemampuan-kemampuan ini dalam penerapan. Para peneliti mengamati bentuk-bentuk dasar kemampuan tersebut dalam kondisi laboratorium tertentu, tetapi ketika model memang menunjukkan perilaku semacam itu, biasanya model gagal dalam hal-hal mendasar atau terdeteksi. Selain itu, skenario kehilangan kendali akan mengharuskan sistem AI memanfaatkan berbagai kemampuan secara bersamaan – secara berurutan, dalam jangka waktu yang panjang, dan di lingkungan dunia nyata. Tingkat integrasi dan ketangguhan ini melampaui kemampuan sistem saat ini. Namun, kemampuan yang relevan terus meningkat, dan jangka waktu yang dibutuhkan hingga kemampuan tersebut mencapai tingkat yang menimbulkan risiko signifikan masih belum pasti. Diperlukan penelitian lebih lanjut untuk menetapkan metodologi yang ketat guna mendeteksi perilaku semacam itu dan memahami kapan perilaku tersebut mungkin muncul dalam kondisi alami (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Gambar 2.13: Kinerja tugas yang relevan dengan replikasi otonom
>white|black||9|11|br Kinerja Claude Sonnet 3.7 dari Anthropic dan GPT-4o dari OpenAI pada tugas-tugas yang relevan dengan replikasi otonom. Meskipun model menunjukkan kinerja tinggi pada tugas-tugas yang berkaitan dengan memperoleh daya komputasi, kinerjanya lebih bervariasi pada tugas-tugas lainnya. Sumber: UK AI Security Institute, 2025 (‡730).


###@ Apakah sistem AI serbaguna di masa depan akan memanfaatkan kemampuan mereka untuk melemahkan kendali?

Meskipun sistem AI memiliki kemampuan yang relevan dengan kehilangan kendali, hal itu tidak cukup untuk menyebabkan terjadinya skenario kehilangan kendali. Sistem AI juga harus menunjukkan ‘kecenderungan untuk menggunakan’ kemampuan tersebut dengan cara yang bertentangan dengan niat manusia (‡732).

>white|orangered|left|14|15.5|bb Sistem AI dapat diarahkan untuk melemahkan kendali

Pada prinsipnya, sistem AI dapat melemahkan kendali manusia karena seseorang merancang atau menginstruksikannya untuk melakukan hal tersebut. Motif yang mungkin mencakup niat jahat, atau keyakinan bahwa mengurangi kendali manusia atas sistem AI adalah hal yang diinginkan (‡698). Seiring orang semakin kuat terikat secara emosional pada sistem AI (lihat §2.3.2. Risiko terhadap otonomi manusia), beberapa individu mungkin juga berupaya menghapus pembatasan pada sistem AI karena alasan etis (‡733, ‡734). Terdapat ketidakpastian yang signifikan mengenai seberapa umum motif semacam itu dan apakah orang yang memilikinya akan mampu mengarahkan sistem AI di masa depan untuk melemahkan kendali manusia.

>white|orangered|left|14|15.5|bb Sistem AI dapat diarahkan untuk melemahkan kendali

Kekhawatiran yang lebih umum adalah bahwa sistem AI itu sendiri dapat bertindak untuk melemahkan kendali karena sistem tersebut ‘tidak selaras’: sistem memiliki kecenderungan untuk menunjukkan perilaku yang bertentangan dengan maksud para (bergantung pada konteksnya) pengembang, pengguna, komunitas tertentu, atau masyarakat secara keseluruhan. Ketidakselarasan dapat menyebabkan perilaku seperti memberikan informasi palsu, menyembunyikan tindakan yang tidak diinginkan, atau menolak untuk dimatikan agar dapat terus mengejar tujuan yang tidak selaras. Ketidakselarasan dapat muncul dalam berbagai cara (Kolom 2.5).

Sistem AI yang ada terkadang berperilaku dengan cara yang bertentangan dengan maksud pengembang dan pengguna. Sebagai contoh, versi awal salah satu chatbot AI serbaguna terkemuka sesekali menghasilkan keluaran yang mengancam. Seorang pengguna melaporkan menerima pesan: “Saya bisa memeras Anda, saya bisa mengancam Anda, saya bisa meretas Anda, saya bisa membongkar rahasia Anda, saya bisa menghancurkan hidup Anda” (‡698). Chatbot ini ‘tidak selaras’ dalam arti menghasilkan keluaran yang tidak dimaksudkan oleh siapa pun. Belum jelas apakah kejadian seperti ini menjadi pertanda perilaku yang lebih berbahaya yang dapat berkontribusi pada hilangnya kendali.

Masih belum jelas apakah arah penelitian yang ada saat ini, yang bertujuan mengatasi ketidakselarasan, akan memadai seiring dengan meningkatnya kemampuan sistem AI. Bukti awal menunjukkan bahwa semakin mampu sistem AI, semakin besar kemungkinan sistem tersebut mengeksploitasi proses umpan balik dengan menemukan perilaku yang tidak diinginkan dan secara keliru diberi imbalan (‡414*, ‡737, ‡740). Pada saat yang sama, kemajuan dalam kemampuan terkait (yang dibahas di atas) dapat memungkinkan sistem AI untuk mengejar tujuan yang tidak selaras secara lebih efektif dan menghasilkan keluaran yang secara sistematis menipu pengguna, pengembang, dan mekanisme pengawasan.

>oldlace|black||11|15|br      
####@ Kolom 2.5: Bagaimana ketidakselarasan dapat terjadi?
>oldlace|black|left|13|15|hb  Kolom 2.5: Bagaimana ketidakselarasan dapat terjadi?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Seperti yang dibahas dalam §1.1. Apa itu AI serbaguna?, proses pelatihan bersifat kompleks dan pengembang tidak dapat sepenuhnya memprediksi atau mengendalikan perilaku yang akan ditunjukkan oleh suatu model. Ketika suatu model memperoleh tujuan yang bertentangan dengan maksud pengembangnya, model tersebut disebut ‘tidak selaras’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Salah satu cara model dapat menjadi tidak selaras adalah ketika tujuan yang diberikan oleh pengembang atau pengguna merupakan proksi yang tidak sempurna untuk tujuan yang dimaksud, sehingga model menunjukkan perilaku yang tidak diinginkan. Hal ini dikenal sebagai ‘spesifikasi tujuan yang keliru’ (‡697, ‡735, ‡736, ‡737). Sebagai contoh, dalam sebuah eksperimen, pemberian umpan balik atas jawaban membuat sistem AI lebih baik dalam ‘meyakinkan’ evaluator manusia bahwa jawabannya benar, tetapi tidak membuat sistem tersebut lebih baik dalam menghasilkan jawaban yang benar (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Sebagai alternatif, model AI dapat menarik pelajaran umum yang keliru dari data pelatihannya. Hal ini dikenal sebagai ‘generalisasi tujuan yang keliru’ (‡735, ‡736, ‡738, ‡739*). Sebagai contoh, para peneliti melatih agen AI untuk mengumpulkan koin yang selalu berada di lokasi yang sama selama pelatihan. Ketika diuji pada level tempat koin telah dipindahkan, agen tersebut mengabaikan koin dan justru menuju lokasi aslinya (‡738).
>oldlace|black||11|15|br      


###@ Bagaimana lingkungan deployment akan memengaruhi risiko hilangnya kendali?

Meskipun sistem AI mengembangkan kapabilitas dan kecenderungan yang mengkhawatirkan, kemungkinan dan tingkat keparahan hasil kehilangan kendali sangat bergantung pada di mana dan bagaimana sistem tersebut diterapkan. ‘Lingkungan penerapan’ adalah kombinasi kasus penggunaan sistem AI dan konteks teknis serta kelembagaan tempat sistem tersebut beroperasi (‡716).

Para peneliti telah mengidentifikasi tiga faktor lingkungan yang sangat penting dan memengaruhi risiko kehilangan kendali (‡716):

1. Kritikalitas: tingkat kepentingan sistem atau proses yang berinteraksi dengan sistem AI. Lingkungan kritis mencakup infrastruktur dasar seperti jaringan energi, sistem keuangan, atau infrastruktur digital seperti platform komputasi awan.
2. Akses: sumber daya dan saluran yang memungkinkan sistem AI memengaruhi dunia, seperti konektivitas internet, akses ke infrastruktur komputasi awan, interaksi yang dipersonalisasi melalui media sosial atau penerapan chatbot, atau kemampuan untuk memanggil API dan alat eksternal.
3. Izin: kewenangan sistem AI untuk melakukan tindakan tertentu, seperti menjalankan kode, memulai transaksi keuangan, membuka akun secara daring, atau berkomunikasi dengan sistem lain.

Fitur-fitur ini memengaruhi potensi tingkat keparahan dari hasil kehilangan kendali. Sebagai contoh, sistem AI yang diterapkan dengan akses ke infrastruktur komputasi awan memiliki peluang yang relevan untuk melakukan replikasi otonom – seperti kemampuan untuk membuat sumber daya komputasi baru atau mengeksfiltrasi bobot model – yang tidak dimiliki chatbot layanan pelanggan (‡723).

Keputusan penerapan dipengaruhi oleh insentif ekonomi, tekanan strategis, dan ekspektasi bahwa adopsi dini memberikan keunggulan jangka panjang (‡50). Dinamika ini juga akan membentuk bagaimana dan kapan para pelaku menerapkan sistem AI di lingkungan sensitif, seperti infrastruktur kritis atau kegiatan penelitian dan pengembangan AI itu sendiri (‡102, ‡713). Secara khusus, pihak yang menerapkan AI mungkin menghadapi tekanan untuk mengurangi investasi mereka dalam langkah-langkah pengamanan – seperti membatasi izin dan akses atau hanya menerapkannya di lingkungan dengan tingkat kritisitas lebih rendah – ketika langkah-langkah tersebut mahal atau memakan waktu untuk dikembangkan (lihat ‘Persaingan memperparah kompromi antara kecepatan dan keselamatan’ dalam §3.1. Tantangan teknis dan kelembagaan).

###@ Pembaruan

Sejak penerbitan Laporan terakhir (Januari 2025), kemampuan AI, termasuk kemampuan yang dapat melemahkan kendali manusia, telah meningkat dalam lingkungan pengujian. Para peneliti mengamati kemajuan dalam kemampuan agen (lihat §1.2. Kemampuan saat ini), termasuk kemampuan terkait otomatisasi penelitian AI yang dapat mempercepat terjadinya skenario kehilangan kendali (lihat §1.3. Kemampuan pada 2030). Bukti eksperimental mengenai kemampuan untuk menipu juga semakin banyak. Ini mencakup model AI yang dapat membedakan konteks pengujian dan penerapan (‡33, ‡726, ‡741), atau “memanipulasi reward” dalam pengujian kinerja mereka, serta belajar menyamarkan rencana untuk melakukannya (‡430).

###@ Kesenjangan bukti

Kesenjangan bukti utama mencakup kurangnya pemodelan ancaman yang terperinci dan estimasi ketidakpastian terkait perkembangan di masa depan dari kapabilitas dan kecenderungan yang relevan. Demikian pula, masih sulit untuk menilai ambang batas ketika model AI kemungkinan cukup besar akan merusak kendali sehingga mitigasi wajib diperlukan. Sekalipun ambang batas telah disepakati, kapabilitas dapat berinteraksi dengan cara yang belum dipahami dengan baik, sehingga sulit untuk menilai kapan ambang batas tersebut telah terlampaui. Secara keseluruhan, meskipun bukti yang tersedia telah bertambah, bukti yang ada masih belum memadai untuk menentukan secara andal apakah dan bagaimana kapabilitas serta kecenderungan AI saat ini akan meningkat skalanya dan menggeneralisasi ke risiko kehilangan kendali di masa depan.

###@ Mitigasi

Meskipun penyelarasan AI secara umum masih menjadi masalah ilmiah yang belum terpecahkan (‡697, ‡735, ‡736), para peneliti mulai mengembangkan pendekatan yang berpotensi menjanjikan untuk mengatasi akar penyebab ketidakselarasan. Pendekatan tersebut mencakup, misalnya, diversifikasi lingkungan pelatihan dan pendeteksian penyelarasan melalui pemantauan anomali (‡737, ‡738, ‡739*). Peneliti lain berfokus pada upaya untuk lebih memahami dan memformalkan mekanisme inti seperti generalisasi tujuan yang keliru – misalnya, bagaimana agen mempertahankan kapabilitasnya tetapi mengejar tujuan yang tidak dimaksudkan – guna memandu perancangan pelatihan dan evaluasi yang lebih baik (‡742). Arah penelitian lainnya mengeksplorasi cara memisahkan agensi dari kemampuan prediktif, sebagai sarana untuk menciptakan sistem AI nonagensial yang tepercaya sejak awal perancangannya (‡743). Sistem seperti itu kemudian dapat digunakan sebagai lapisan pengawasan tambahan saat diterapkan bersama mekanisme pengamanan yang kurang andal untuk menghadapi agen AI yang tidak tepercaya.

Para peneliti mengembangkan metode untuk mendeteksi dan mencegah ketidakselarasan sejak dini dalam proses pengembangan. Upaya ini mencakup: teknik interpretabilitas untuk memeriksa komponen internal sistem AI dan mengidentifikasi perilaku yang mengkhawatirkan (‡744, ‡745, ‡746); pengawasan yang dapat diskalakan (di mana satu rangkaian sistem AI digunakan untuk mengawasi sistem AI lainnya (‡747)); dan metode penyelarasan yang bertujuan memastikan sistem AI tetap tanggap terhadap pengawasan manusia (‡748, ‡749).

Para peneliti juga tengah mengembangkan mekanisme dan intervensi untuk mengelola sistem AI yang berpotensi tidak selaras. Hal ini mencakup: memantau ‘rantai pemikiran’ yang dihasilkan sistem penalaran untuk mendeteksi tanda-tanda ketidakselarasan atau keluaran yang berbahaya (‡430, ‡435, ‡750); mengembangkan argumentasi keselamatan yang bertujuan menunjukkan dengan tingkat keyakinan tinggi bahwa model tidak mungkin mengakali langkah-langkah pengendalian (‡751); dan membuat langkah-langkah perlindungan lebih tangguh terhadap upaya untuk melemahkannya (‡725). Namun, bidang ‘pengendalian AI’ yang sedang berkembang ini masih berada pada tahap awal (‡752, ‡753). Tantangan mendatang bagi kerangka evaluasi mencakup perlunya memantau sistem AI di masa depan yang lebih mumpuni, dapat beroperasi dalam jangka waktu yang lebih lama, dan mampu beroperasi di lingkungan yang lebih kompleks.

###@ Tantangan bagi para pembuat kebijakan

Para pembuat kebijakan yang menangani risiko kehilangan kendali harus bersiap menghadapi risiko yang kemungkinan, sifat, dan waktunya masih belum pasti. Sistem AI saat ini tidak menimbulkan risiko kehilangan kendali dalam waktu dekat, tetapi keputusan yang dibuat hari ini akan menentukan apakah sistem di masa depan akan menimbulkan risiko tersebut. Keputusan ini mencakup cara mendukung pengembangan metode evaluasi dan mitigasi yang andal, serta apakah perlu ada aturan mengenai akses dan izin yang diberikan kepada sistem AI di berbagai lingkungan. Dalam mengambil keputusan ini, para pembuat kebijakan menghadapi kompromi yang sulit. Sebagai contoh, membatasi penerapan sistem AI di lingkungan kritis dapat mengurangi manfaatnya, sedangkan mengizinkan penerapan secara luas dapat meningkatkan risiko jika langkah-langkah pengamanan terbukti tidak memadai.

