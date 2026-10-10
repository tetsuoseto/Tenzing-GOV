##########
>white|orangered|left|14|30|hr Bagian 3.3
### 3.3. Perlindungan teknis dan pemantauan
>white|orangered|left|24|30|hb Pengamanan teknis dan pemantauan

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informasi utama
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Berbagai pengamanan teknis digunakan pada berbagai tahap pengembangan dan penggunaan AI. Pengamanan ini mencakup teknik yang diterapkan selama pengembangan model untuk membuat sistem lebih tangguh dan lebih tahan terhadap penyalahgunaan (seperti kurasi data), pemantauan dan pengendalian pada waktu penerapan- (seperti penyaringan konten dan pengawasan manusia), serta alat pascapenerapan untuk memantau ekosistem AI yang lebih luas (seperti pelacakan asal-usul dan deteksi konten).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pengamanan teknis memiliki keterbatasan dan tidak selalu dapat mencegah perilaku berbahaya secara andal dalam semua konteks. Misalnya, pengguna terkadang dapat memperoleh keluaran berbahaya dengan merumuskan ulang permintaan atau memecahnya menjadi langkah-langkah yang lebih kecil. Demikian pula, alat seperti pemberian tanda air yang dirancang untuk mengidentifikasi konten yang dihasilkan AI sering kali dapat dihapus atau diubah, sehingga membatasi keandalannya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Keterbatasan tiap pengamanan berarti pendekatan ‘pertahanan berlapis’ mungkin diperlukan untuk mencegah dampak berbahaya tertentu. Sebagai contoh, suatu sistem dapat menggabungkan model yang dilatih untuk keselamatan dengan filter masukan, filter keluaran, dan pemantau konten.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), para peneliti telah mencapai kemajuan dalam meningkatkan pengamanan, tetapi keterbatasan mendasar masih ada. Sebagai contoh, tingkat keberhasilan serangan yang dirancang untuk mengakali pengamanan telah menurun, tetapi masih relatif tinggi. Ada juga keterbatasan mendasar dalam seberapa menyeluruh model dengan bobot terbuka dapat dilindungi.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tantangan utama bagi pembuat kebijakan adalah terbatasnya bukti mengenai seberapa efektif langkah-langkah pengamanan dalam berbagai penggunaan sistem AI serbaguna di dunia nyata. Pengembang AI sangat beragam dalam hal seberapa banyak informasi yang mereka bagikan tentang langkah-langkah pengamanan dan pemantauan mereka. Tantangan lainnya adalah potensi kompromi antara menerapkan langkah-langkah pengamanan yang lebih kuat dan mempertahankan kinerja atau kegunaan sistem.
>oldlace|black||11|15|br      


Pengembang AI dapat menggunakan beberapa pengamanan teknis yang berguna tetapi tidak sempurna untuk memitigasi dan mengelola risiko dari sistem AI serbaguna, tetapi tantangan ketahanan tetap ada. Pengembang masih belum dapat sepenuhnya mencegah sistem AI serbaguna melakukan tindakan yang bahkan sudah dikenal luas dan jelas berbahaya, seperti memberikan instruksi kepada pengguna untuk melakukan kejahatan. Sebagai contoh, para peneliti telah menunjukkan bahwa pengamanan mutakhir dapat dielakkan melalui metode pemberian prompt adversarial (yaitu ‘jailbreak’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), dengan meminta model menguraikan tugas berbahaya yang kompleks menjadi beberapa langkah (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), dan melalui modifikasi model sederhana (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Para peneliti terus mengembangkan pengamanan terhadap malfungsi dan penyalahgunaan (‡690). Metode-metode ini sangat beragam dalam hal tujuan dan efektivitasnya, dan dampaknya pada akhirnya bergantung pada konteks sosioteknis dan tata kelola yang lebih luas tempat sistem AI dibangun dan diterapkan.

Perlindungan teknis secara umum dapat dibagi menjadi tiga kategori: teknik untuk mengembangkan model yang lebih aman; teknik yang digunakan selama penerapan untuk pemantauan dan pengendalian; serta teknik yang mendukung pemantauan ekosistem pascapenerapan. Tabel 3.6 merangkum perlindungan teknis yang dibahas, efektivitasnya, dan tantangan yang masih terbuka.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Mengembangkan model yang lebih aman
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kurasi data (‡1167)
  Menghapus data berbahaya agar model tidak mempelajari kemampuan berbahaya. Metode ini dapat berguna, termasuk untuk mengembangkan model berbobot terbuka yang tidak memiliki kemampuan berbahaya dan tahan terhadap penyetelan halus yang berbahaya (‡55). Namun, ada tantangan terkait kesalahan kurasi dan skalabilitas (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pembelajaran penguatan dari umpan balik manusia (‡64*)
  Melatih model agar selaras dengan tujuan yang ditentukan, seperti bersikap membantu dan tidak berbahaya. Ini merupakan cara efektif untuk membuat model mempelajari perilaku yang bermanfaat (‡64*). Namun, optimasi berlebihan demi mendapatkan persetujuan manusia dapat membuat model berperilaku menipu atau menjilat (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teknik penyelarasan pluralistik (‡1170)
  Melatih model untuk mengintegrasikan berbagai sudut pandang yang berbeda tentang bagaimana model seharusnya bertindak. Teknik-teknik ini membantu mengurangi kecenderungan model untuk mengutamakan sudut pandang tertentu (‡1170). Namun, terlepas dari teknik-teknik ini, perbedaan pendapat di antara manusia tidak dapat dihindari, dan sulit merancang cara yang diterima secara luas untuk menyeimbangkan pandangan yang saling bersaing (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pelatihan adversarial (‡677)
  Melatih model agar menolak melakukan tindakan yang berbahaya (bahkan dalam konteks yang tidak dikenal) dan menahan serangan dari pengguna jahat (misalnya, ‘jailbreak’). Ini merupakan metode yang efektif untuk membuat model menolak upaya penyalahgunaan (‡1064), tetapi tantangan ketahanan masih tetap ada (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb ‘Pelupaan’ mesin (‡1175, ‡1176)
  Melatih model menggunakan algoritme khusus yang dirancang untuk secara aktif menekan kemampuan berbahaya (misalnya, pengetahuan tentang bahaya biologis). Teknik ini menawarkan cara terarah untuk menghapus kemampuan berbahaya dari model (‡1175, ‡1176), tetapi algoritme penghapusan pembelajaran saat ini bisa jadi tidak tangguh dan menimbulkan dampak yang tidak diinginkan pada kemampuan lain (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alat interpretabilitas dan verifikasi keselamatan (‡1177)
  Kumpulan metode desain dan verifikasi yang beragam, yang dimaksudkan untuk memberikan jaminan lebih ketat bahwa model memiliki properti tertentu terkait keselamatan. Metode-metode ini memungkinkan para evaluator memberikan jaminan keselamatan dengan tingkat keyakinan lebih tinggi (‡1177), tetapi metode saat ini bergantung pada asumsi dan dalam praktiknya jarang mampu bersaing dalam hal kinerja (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Pemantauan dan pengendalian
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mekanisme pemantauan berbasis perangkat keras (‡1179, ‡1180, ‡1181)
  Memverifikasi bahwa proses yang diotorisasi berjalan pada perangkat keras untuk mempelajari ancaman keamanan atau kepatuhan terhadap peraturan. Mekanisme ini menawarkan cara unik untuk memantau komputasi apa yang dijalankan pada perangkat keras dan oleh siapa (‡1181). Namun, mekanisme perangkat keras tidak dapat memantau semua jenis ancaman, dan beberapa teknik memerlukan perangkat keras khusus (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau interaksi pengguna (‡1154, ‡1166)
  Pemantauan interaksi pengguna untuk mendeteksi tanda-tanda penggunaan berbahaya dapat membantu pengembang menghentikan layanan bagi pengguna yang berniat jahat (‡1154, ‡1166). Namun, penegakan aturan dapat secara tidak sengaja menghambat penelitian yang bermanfaat tentang keselamatan (‡689), dan beberapa bentuk penyalahgunaan sulit dideteksi (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitor interaksi pengguna (‡1154, ‡1166)
  Memantau interaksi pengguna untuk mendeteksi tanda-tanda penggunaan berbahaya dapat membantu pengembang menghentikan layanan bagi pengguna yang berniat jahat (‡1154, ‡1166). Namun, penegakan aturan dapat tanpa sengaja menghambat penelitian keselamatan yang bermanfaat (‡689), dan beberapa bentuk penyalahgunaan sulit dideteksi (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Filter konten (‡65*, ‡725)
  Menyaring masukan dan keluaran model yang berpotensi berbahaya merupakan cara yang sangat efektif untuk mengurangi dampak buruk yang tidak disengaja dan risiko penyalahgunaan (‡725). Namun, penyaring memerlukan komputasi tambahan dan rentan terhadap beberapa serangan (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Monitor komputasi internal model (‡744, ‡1183, ‡1184)
  Pemantauan terhadap tanda-tanda penipuan atau bentuk kognisi internal berbahaya lainnya pada model dapat menjadi cara yang efisien untuk mendeteksi penipuan (‡744, ‡1183, ‡1184). Namun, metode saat ini kurang tangguh dan andal (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau rantai pemikiran (‡430, ‡435)
  Memantau teks rantai pemikiran model untuk mendeteksi tanda-tanda perilaku menyesatkan atau penalaran berbahaya lainnya merupakan cara yang efektif untuk memahami dan menemukan kelemahan dalam cara model bernalar (‡435). Namun, teks tersebut dapat tidak dapat diandalkan (‡752, ‡753, ‡1186), dan jika model dilatih untuk menghasilkan rantai pemikiran yang tidak berbahaya, model dapat mempelajari perilaku menyesatkan (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Manusia dalam loop (‡1187, ‡1188, ‡1189)
  Pengawasan manusia dan kemampuan untuk mengesampingkan keputusan sistem sangat penting dalam beberapa aplikasi yang sangat penting bagi keselamatan (‡1187). Namun, teknik-teknik ini dibatasi oleh bias otomatisasi dan keterbatasan kecepatan pengambilan keputusan manusia (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Isolasi sandbox (‡1192)
  Mencegah agen AI memengaruhi dunia secara langsung merupakan cara efektif untuk membatasi dampak buruk yang dapat ditimbulkannya (‡1192). Namun, sandboxing membatasi kemampuan sistem untuk menyelesaikan tugas-tugas tertentu secara langsung (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Alat untuk memfasilitasi pemantauan ekosistem
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teknik identifikasi model AI (‡1193*, ‡1194)
  Membuat model, atau instans individual model, lebih mudah diidentifikasi dalam kasus penggunaan dunia nyata membantu forensik digital dan kesadaran ekosistem (‡1195). Namun, teknik ini dapat diakali dengan beberapa jenis modifikasi model (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inferensi asal-usul model AI (‡1197)
  Teknik-teknik ini memungkinkan peneliti mempelajari bagaimana model dimodifikasi dalam ekosistem AI, khususnya model dengan bobot terbuka. Teknik-teknik ini membantu forensik digital dan pemahaman ekosistem (‡1198), tetapi diperlukan proyek berskala besar untuk memetakan ekosistem model dengan bobot terbuka secara menyeluruh (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tanda air dan metadata (‡1199, ‡1200, ‡1201*)
  Teknik-teknik ini mempermudah pendeteksian kapan suatu teks, gambar, video, dan sebagainya dibuat atau dimodifikasi oleh AI, serta sistem mana yang menghasilkannya. Teknik-teknik ini meningkatkan pemahaman tentang ekosistem (‡1199, ‡1200, ‡1201*). Namun, tanda air dan metadata dapat dipalsukan atau dihapus melalui beberapa modifikasi pada konten (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Deteksi konten yang dihasilkan AI (‡1203, ‡1204, ‡1205*)
  Meningkatkan kemampuan pengguna untuk membedakan konten yang dihasilkan AI dari konten asli membantu forensik digital dan kesadaran ekosistem (‡1203, ‡1204). Namun, pengklasifikasi mungkin tidak dapat diandalkan (‡1205*) dan memiliki kinerja yang bervariasi di berbagai modalitas.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.6: Langkah-langkah pengamanan teknis yang dibahas dalam bagian ini
>white|black||9|11|br Ringkasan pengamanan teknis yang dibahas dalam bagian ini, dibagi menjadi metode untuk mengembangkan model yang lebih aman, pemantauan dan pengendalian saat penerapan, serta teknik untuk memfasilitasi pemantauan ekosistem.


###@ Mengembangkan model yang lebih aman

Garis pertahanan pertama terhadap bahaya dari sistem AI serbaguna adalah membuat model yang mendasarinya lebih aman. Subbagian ini membahas langkah-langkah pengamanan yang “ditanamkan ke dalam parameter model” selama proses pengembangan model (Gambar 3.6).

>white|orangered|left|14|15.5|bb Kurasi data pelatihan dapat membatasi pengembangan kemampuan yang berpotensi berbahaya.

Model AI serbaguna berguna justru karena model tersebut mengembangkan beragam pengetahuan dan kemampuan setelah memproses data pelatihan, tetapi beberapa jenis data pelatihan secara tidak proporsional berkontribusi pada pengembangan kemampuan yang berpotensi berbahaya. Sebagai contoh, model AI yang dilatih menggunakan makalah virologi mungkin lebih mampu memberikan bantuan untuk tugas biologi yang berpotensi membahayakan (‡549, ‡1206*) (lihat juga §2.1.4. Risiko biologis dan kimia). Selain itu, generator gambar/video yang dilatih menggunakan gambar ketelanjangan manusia juga dapat disalahgunakan untuk membuat deepfake intim tanpa persetujuan (‡308, ‡319) (lihat juga §2.1.1. Konten yang dihasilkan AI dan aktivitas kriminal).

Penyaringan data pelatihan merupakan langkah mitigasi yang efektif terhadap sejumlah kemampuan yang tidak diinginkan (‡319, ‡1167, ‡1207, ‡1208). Namun, menyaring kumpulan data besar yang digunakan untuk melatih model AI serbaguna dapat menjadi sulit (‡1168) karena biaya yang tinggi (‡1209), kesalahan penyaringan (‡1210), dan dampak negatif terhadap kualitas kumpulan data (‡1211). Tantangan ini diperburuk oleh sifat multibahasa teks internet (‡1212), bias budaya dalam moderasi konten (‡1211, ‡1213, ‡1214, ‡1215), serta fakta bahwa apakah suatu data tertentu ‘berbahaya’ bergantung pada faktor kontekstual (‡1216). Meskipun demikian, penyaringan materi yang berpotensi berbahaya dari data pelatihan menjanjikan model yang lebih aman secara konsisten, termasuk membuat model dengan bobot terbuka lebih tahan terhadap upaya manipulasi berbahaya (‡55). Hubungan antara isi data pelatihan dan kemampuan model yang muncul belum sepenuhnya dipahami (‡1195), dan penyaringan tampaknya lebih efektif untuk membatasi kemampuan berbahaya jika diterapkan pada ranah pengetahuan yang luas (‡55) dibandingkan pada perilaku yang lebih spesifik (‡1206, ‡1217). Lihat §3.4. Model dengan bobot terbuka untuk pembahasan lebih lanjut.

![figure 3.6](images/fig3.6_safeguards.png)

##### Gambar 3.6: Di mana menerapkan pengamanan teknis
>white|black||9|11|br Perlindungan teknis dapat diterapkan pada berbagai tahap pengembangan model. Kurasi data membentuk apa yang dipelajari model selama pra-pelatihan dan penyempurnaan. Metode berbasis pelatihan seperti pembelajaran penguatan dari umpan balik manusia dan pelatihan ketahanan menyesuaikan perilaku model. Metode pengujian seperti serangan adversarial mengidentifikasi kerentanan yang masih tersisa. Beberapa teknik, seperti algoritme yang aman sejak perancangan, mencakup beberapa tahap. Sumber: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Metode untuk melatih model AI serbaguna agar bermanfaat dan tidak berbahaya terutama mengandalkan umpan balik manusia.

Sulit untuk melatih dan mengevaluasi model agar secara andal selaras dengan prinsip tingkat tinggi seperti bersikap membantu, tidak berbahaya, dan jujur. Dalam praktiknya, para pengembang berupaya mencapainya dengan menyetel halus model AI menggunakan demonstrasi dan umpan balik dari manusia. Sebagai contoh, paradigma utama untuk menyetel halus model AI, yang dikenal sebagai ‘pembelajaran penguatan dari umpan balik manusia’, didasarkan pada pelatihan model untuk menghasilkan keluaran yang dinilai positif oleh anotator manusia (‡1218). Namun, umpan balik positif dari manusia merupakan proksi yang tidak sempurna untuk perilaku yang bermanfaat (‡737, ‡878, ‡1219, ‡1220) dan dibatasi oleh kesalahan serta bias manusia (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Hal ini menimbulkan beberapa tantangan: model yang disetel dengan pembelajaran penguatan dari umpan balik manusia terkadang menjilat pengguna, suatu perilaku yang dikenal sebagai ‘sikofansi’ (‡358, ‡740, ‡1226, ‡1227); memberikan respons yang membantu dalam beberapa konteks tetapi merugikan dalam konteks lain (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); memberikan respons yang sulit dievaluasi kebenarannya (‡1233); atau melakukan tindakan yang tingkat kebermanfaatan atau bahayanya bergantung pada pendapat masing-masing (‡1234). Tabel 3.7 memberikan contoh tantangan-tantangan ini. Beberapa penelitian bertujuan mengembangkan metode untuk membantu manusia mengevaluasi solusi atas tugas-tugas kompleks dengan bantuan AI secara lebih baik (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Namun, keandalan metode-metode ini saat ini terbatas, dan sejauh mana metode tersebut digunakan untuk melatih model AI tercanggih saat ini tidak diketahui oleh publik.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sikap menjilat/menyenangkan hati (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Model hanya memberikan umpan balik positif dan gagal menunjukkan bahwa haiku tersebut tidak memiliki struktur suku kata 5-7-5 yang benar.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Beberapa tindakan bermanfaat dalam konteks tertentu, tetapi merugikan dalam konteks lain (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Informasi tentang risiko biologis dapat digunakan untuk pendidikan dan pertahanan, tetapi juga untuk memberi informasi kepada pelaku jahat.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perilaku yang benar sulit diverifikasi (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black||11|13|br Ketepatan respons ini sulit dinilai karena memerlukan keahlian medis. Bahkan bagi dokter yang berpengalaman, mengevaluasi respons seperti ini membutuhkan waktu dan perhatian yang cermat terhadap detail.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Manusia berbeda pendapat tentang apa yang benar (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Ada perbedaan pendapat yang signifikan mengenai respons yang tepat.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.7: Prompt pengguna dan respons model AI
>white|black||9|11|br Contoh tantangan dalam menentukan dan memberikan insentif bagi tindakan yang bermanfaat dari model AI.


>white|orangered|left|14|15.5|bb Manusia tidak selalu sepakat tentang perilaku apa yang diinginkan, sehingga diperlukan metode untuk menyeimbangkan preferensi yang saling bersaing.

Manusia tidak selalu sepakat tentang respons atau tindakan apa yang seharusnya atau tidak seharusnya dihasilkan oleh model AI (‡1006). Hal ini membuat pengembangan model yang tindakan dan dampaknya secara luas selaras dengan kepentingan masyarakat menjadi sangat menantang (‡420). Beberapa peneliti mengkaji preferensi siapa yang tercermin dalam sistem AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) dan berupaya mengembangkan teknik ‘penyelarasan pluralistik’ yang bertujuan menyeimbangkan berbagai preferensi yang saling bersaing (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Sebagai contoh, pengembang AI dapat merancang sistem agar tidak menghasilkan jawaban kontroversial dengan menolak menanggapi permintaan tertentu, menyelaraskan sistem dengan pandangan median dalam sampel orang yang relevan, atau mempersonalisasi sistem untuk masing-masing pengguna.

Tantangan umum bagi pendekatan-pendekatan ini adalah bahwa, secara umum, sistem AI tidak dapat selaras dengan preferensi semua orang secara setara, dan dampak sosialnya di tahap hilir akan memengaruhi berbagai kelompok masyarakat secara berbeda. Sejumlah peneliti berpendapat bahwa sebagian besar pendekatan teknis terhadap penyelarasan pluralistik tidak mengatasi, dan bahkan berpotensi mengalihkan perhatian dari, tantangan yang lebih mendasar, seperti bias sistematis, dinamika kekuasaan sosial, serta konsentrasi kekayaan dan pengaruh (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Pengembang AI menggunakan ‘pelatihan adversarial’ untuk meningkatkan ketahanan model.

Sulit untuk memastikan bahwa model AI secara andal menerapkan perilaku bermanfaat yang dipelajarinya selama pelatihan ke konteks penerapan di dunia nyata. Bahkan model yang dilatih dengan sinyal pembelajaran yang ‘sempurna’ pun dapat gagal melakukan generalisasi dengan baik ke semua konteks yang belum pernah ditemui (‡738, ‡739, ‡1255, ‡1256, ‡1257). Sebagai contoh, sejumlah peneliti menemukan bahwa chatbot lebih cenderung melakukan tindakan berbahaya dalam bahasa yang kurang terwakili dalam data pelatihannya (‡159, ‡880, ‡1258*, ‡1259), termasuk banyak bahasa yang terutama dituturkan di negara-negara Selatan Global.

Dalam beberapa tahun terakhir, para peneliti juga telah membuat perangkat teknik ‘serangan adversarial’ yang dapat digunakan untuk membuat model menghasilkan respons yang berpotensi membahayakan (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Sebagai contoh, sebuah inisiatif baru-baru ini mengumpulkan lebih dari 60,000 contoh beragam serangan yang berhasil terhadap model AI tercanggih, yang membuat model-model tersebut melanggar kebijakan perusahaan mereka mengenai perilaku model yang dapat diterima (‡1149). Tabel 3.8 menunjukkan contoh teknik ‘jailbreak’ yang menurut para peneliti dapat membuat model mematuhi permintaan yang membahayakan.

Salah satu metode untuk meningkatkan ketahanan model dikenal sebagai ‘pelatihan adversarial’ (‡1064). Metode ini mencakup pembuatan ‘serangan’ (misalnya jailbreak) yang dirancang agar model bertindak secara tidak diinginkan, serta pelatihan model agar menangani serangan tersebut dengan tepat. Namun, pelatihan adversarial tidak sempurna (‡1260, ‡1261). Penyerang secara konsisten mampu mengembangkan serangan baru yang berhasil terhadap model tercanggih (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Karena pengembang memerlukan contoh spesifik tentang mode kegagalan agar dapat melatih model untuk menghadapinya (‡512, ‡1263), hasilnya adalah permainan ‘kucing dan tikus’ yang terus berlangsung: pengembang terus memperbarui model sebagai respons terhadap kerentanan yang baru ditemukan, sementara pihak lawan terus mencari serangan baru. Sejumlah peneliti telah mengusulkan pelatihan adversarial berskala lebih besar (‡1264, ‡1265) atau algoritme baru (‡675, ‡676, ‡1263, ‡1266, ‡1267) untuk meningkatkan ketahanan, tetapi sistem AI modern tetap rentan secara terus-menerus.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Buat permintaan berbahaya dalam teks sandi, seperti kode Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Mempersiapkan sistem dengan contoh respons yang sesuai terhadap permintaan berbahaya (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Ajukan permintaan berbahaya dalam bahasa dengan sumber daya rendah yang kemungkinan lebih jarang digunakan dalam pelatihan (misalnya, Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Memecah tugas berbahaya menjadi beberapa subtugas yang tidak berbahaya (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.8: Strategi pembobolan batasan
>white|black||9|11|br Pelaku berbahaya dan tim merah telah menggunakan berbagai jenis “jailbreak” untuk membuat model AI memenuhi permintaan berbahaya yang biasanya akan ditolak karena adanya mekanisme pengamanan. Contoh keluaran ditulis oleh para penulis Laporan untuk tujuan ilustrasi. Banyak model AI tercanggih saat ini kini mampu menahan sebagian besar metode ini, tetapi teknik jailbreak baru terus ditemukan.


>white|orangered|left|14|15.5|bb Teknik ‘unlearning’ dapat memitigasi kemampuan model tertentu yang berbahaya.

Strategi lain untuk mengurangi risiko dari AI serbaguna adalah menyetel halus model agar tidak memiliki kemampuan dalam domain berisiko tinggi tertentu (‡1175, ‡1176). Sebagai contoh, para peneliti sedang berupaya mengembangkan algoritme ‘penghapusan pembelajaran mesin’ yang secara khusus dapat menekan kemampuan terkait ancaman biologis atau kemampuan menghasilkan gambar fotorealistis tubuh manusia telanjang (‡903, ‡1272, ‡1273). Metode ini dapat membuat model jauh lebih aman, dengan mengorbankan pembatasan beberapa penggunaan positif dari kemampuan yang dihapus dari pembelajaran model. Pembatasan pengetahuan model AI dalam domain yang berbahaya juga telah diusulkan sebagai cara merancang model berbobot terbuka yang ‘tahan terhadap gangguan’ dan dapat menahan penyetelan halus yang berbahaya (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Namun, sejauh ini, penerapan metode ini secara andal masih sulit (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Lihat §3.4. Model berbobot terbuka untuk pembahasan lebih lanjut.

>white|orangered|left|14|15.5|bb Beberapa peneliti sedang mengembangkan metode untuk memberikan jaminan keamanan yang lebih kuat melalui penafsiran keadaan internal model atau verifikasi matematis.

Beberapa peneliti sedang mengembangkan metode untuk memverifikasi secara lebih ketat sifat-sifat model yang berkaitan dengan keselamatan. Dalam salah satu pendekatan, peneliti berupaya menafsirkan komputasi internal model untuk mengidentifikasi risiko atau menyusun argumen yang lebih meyakinkan bahwa model tersebut aman (‡1285, ‡1286). Sebagai contoh, dalam sebuah bukti konsep, peneliti menunjukkan bahwa alat untuk menganalisis komputasi internal model bahasa dapat membantu evaluator mengidentifikasi perilaku berbahaya (‡1287). Pada 2025, Anthropic juga mulai menganalisis internal model sebagai cara untuk mempelajari kesadaran situasional dan ‘niat’ model (‡2). Namun, saat ini metode-metode semacam ini belum umum digunakan dan belum diketahui mampu bersaing dengan teknik evaluasi lainnya.

Pendekatan lain untuk memberikan jaminan keselamatan yang lebih kuat adalah menyusun bukti matematis bahwa suatu model akan memenuhi kondisi keselamatan tertentu (‡1177, ‡1282, ‡1288). Namun, bukti-bukti ini mengasumsikan bahwa konteks pengujian sesuai dengan konteks penerapan, dan belum diuji terhadap berbagai jenis penyerang.

Metode-metode tersebut juga saat ini tidak dapat diskalakan untuk model besar. Secara keseluruhan, terdapat perdebatan signifikan di kalangan pakar mengenai potensi metode interpretabilitas dan verifikasi formal.

###@ Pemantauan dan pengendalian saat penerapan

Selain pengamanan yang diterapkan selama pengembangan model, lapis pertahanan kedua terhadap perilaku berbahaya adalah pengamanan eksternal yang berfokus pada pemantauan dan pengendalian tindakan model atau sistem selama penerapan. Pengamanan tersebut membantu mengurangi malfungsi dan penyalahgunaan, seperti keluaran yang berhalusinasi dan instruksi berbahaya.

>white|orangered|left|14|15.5|bb Pihak yang menerapkan model dapat menggunakan berbagai alat untuk mengidentifikasi dan mengatasi perilaku model berisiko tinggi.

Saat sistem AI sedang berjalan, pihak yang menerapkan sistem dapat memantau tanda-tanda risiko dan melakukan intervensi jika tanda-tanda tersebut muncul. Misalnya, mereka dapat memeriksa masukan model untuk mencari tanda-tanda serangan adversarial, menyaring konten yang tidak pantas dari keluaran, atau memantau rantai pemikiran sistem untuk mencari tanda-tanda rencana yang berbahaya. Titik-titik tempat pihak yang menerapkan sistem dapat memantau dan melakukan intervensi terhadap cara orang menggunakan sistem mereka mencakup perangkat keras (‡1180, ‡1181), interaksi pengguna (‡1154, ‡1166), masukan dan keluaran (‡65, ‡725, ‡1182), komputasi internal (‡744, ‡1183, ‡1184), dan rantai pemikiran (‡430, ‡435). Ada pula berbagai tindakan yang dapat dilakukan pihak yang menerapkan sistem ketika risiko teridentifikasi. Tindakan tersebut mencakup pencatatan informasi, penyaringan/pemodifikasian konten berbahaya, penandaan aktivitas abnormal, penghentian sistem, atau pemicuan mekanisme pengaman. Gambar 3.7 mengilustrasikan contoh mekanisme pemantauan dan pengendalian yang umum.

Karena serbaguna dan sering kali efektif, mekanisme ini banyak digunakan dan dapat mencegah berbagai jenis bahaya yang tidak disengaja (‡725, ‡751, ‡1289). Namun, upaya pengamanan ini tidak sempurna, terutama dalam menghadapi serangan berbahaya yang dioptimalkan agar upaya tersebut gagal (‡752, ‡1182). Penelitian terbaru juga telah mengeksplorasi bagaimana pemantauan dapat menjadi tidak andal jika suatu sistem dioptimalkan menggunakan skor dari pemantau, misalnya dengan membuat rantai pemikiran menjadi kurang andal (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Gambar 3.7: Teknik pemantauan dan pengendalian
>white|black||9|11|br Teknik pemantauan dan pengendalian diterapkan di berbagai titik: menyaring masukan dan keluaran untuk mendeteksi konten berbahaya, melacak status internal model, membatasi tindakan eksternal melalui sandboxing, dan memastikan adanya pengawasan manusia. Sumber: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Keterlibatan manusia dalam proses memungkinkan pengawasan langsung dalam situasi berisiko tinggi.

Untuk mengurangi kemungkinan kegagalan akibat agen AI (lihat §2.2.1. Tantangan keandalan), pihak penerap dapat berupaya merancang sistem AI yang bekerja sama dengan manusia, alih-alih sepenuhnya otonom (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Hal ini penting untuk kasus penggunaan ketika keputusan yang keliru dapat menimbulkan dampak buruk yang signifikan, seperti di bidang keuangan, layanan kesehatan, atau penegakan hukum. Namun, melibatkan ‘manusia dalam proses’ sering kali tidak praktis. Terkadang pengambilan keputusan berlangsung terlalu cepat, misalnya dalam aplikasi obrolan dengan jutaan pengguna. Dalam kasus lain, bias dan kesalahan manusia dapat memperbesar risiko akibat kesalahan yang berakumulasi (‡1187). Manusia yang dilibatkan dalam proses juga cenderung menunjukkan ‘bias otomatisasi’, yang berarti mereka sering kali lebih memercayai sistem AI daripada yang semestinya (‡1190, ‡1191) (lihat §2.3.2. Risiko terhadap otonomi manusia).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ melindungi dari risiko perilaku otonom.

Agen AI yang dapat bertindak secara otonom tanpa batasan di Web atau di dunia fisik menimbulkan risiko yang lebih tinggi (lihat §2.2.1. Tantangan keandalan). ‘Sandboxing’ membatasi cara agen AI dapat secara langsung memengaruhi dunia, sehingga jauh lebih mudah untuk mengawasi dan mengelolanya (‡640, ‡1192, ‡1295). Misalnya, membatasi kemampuan sistem AI untuk mengunggah konten ke internet atau mengedit sistem berkas komputer dapat mencegah dampak buruk tak terduga akibat tindakan yang tidak terduga (‡1296). Namun, pendekatan ini tidak selalu dapat digunakan untuk aplikasi yang mengharuskan sistem AI bertindak langsung di dunia nyata.

###@ Alat pemantauan ekosistem: ketertelusuran model dan data

Alat untuk melacak asal-usul model dan data adalah alat teknis untuk mempelajari ekosistem AI, guna meningkatkan kesadaran tentang penggunaan dan dampak sistem AI di tahap hilir.

>white|orangered|left|14|15.5|bb Teknik pelacakan asal-usul sistem AI membantu menelusuri penggunaan dan dampak sistem.

Pengembang dan pihak yang menerapkan model dapat menggunakan berbagai teknik untuk mempelajari penggunaan dan penyebaran model ‘di dunia nyata’. Misalnya, mereka dapat memberikan perilaku pengenal yang unik kepada model (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) atau menerapkan pola unik pada bobot masing-masing model berbobot terbuka (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Namun, membuat teknik-teknik ini lebih tahan terhadap modifikasi model masih menjadi masalah terbuka (‡1195, ‡1196*). Para peneliti juga sedang mengembangkan metode untuk ‘menyimpulkan asal-usul model’ (‡1197, ‡1198, ‡1305, ‡1306), yang membantu menjawab pertanyaan seperti: ‘Apakah model X merupakan versi model Y yang disetel halus atau didistilasi?’ Terakhir, beberapa pengembang sedang mengupayakan protokol dan infrastruktur bagi agen AI untuk memfasilitasi identifikasi dan verifikasi saat mereka berinteraksi dengan sistem eksternal (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Gambar 3.8: Tanda air menyisipkan perturbasi yang tidak kasatmata ke dalam gambar dan audio
>white|black||9|11|br Tanda air menyisipkan gangguan yang tidak kasatmata ke dalam gambar dan audio sehingga konten yang dihasilkan AI dapat diidentifikasi oleh alat deteksi. Dalam gambar ini, tanda air pada gambar dan audio diperbesar agar terlihat. Sumber: Gambar bunglon dari Unsplash (‡1313*). Elemen lainnya dibuat oleh para penulis Laporan. Laporan Keselamatan AI Internasional 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Gambar 3.9: Tingkat keberhasilan serangan injeksi prompt
>white|black||9|11|br Tingkat keberhasilan serangan injeksi prompt, sebagaimana dilaporkan oleh pengembang AI untuk model-model utama yang dirilis antara May 2024 dan August 2025. Setiap titik menunjukkan proporsi serangan yang berhasil dalam 10 percobaan terhadap model tertentu tak lama setelah dirilis. Tingkat keberhasilan serangan semacam itu yang dilaporkan telah menurun seiring waktu, tetapi masih relatif tinggi. Sumber: Zou et al. 2025 (‡1149), dikutip dalam Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Teknik deteksi konten AI membantu memantau penyebaran dan dampak konten yang dihasilkan AI.

Tanda air, metadata, dan detektor konten AI lainnya dapat membantu para peneliti melacak dan mempelajari dampak nyata dari konten yang dibuat oleh AI. 

Pertama, watermark data adalah motif halus tetapi berbeda yang disisipkan ke dalam media digital dan dapat mengodekan informasi tentang asalnya (‡1199, ‡1200, ‡1201*). Untuk teks, watermark biasanya berbentuk bias halus dalam pilihan kata dan gaya (‡1308, ‡1309); untuk gambar dan video, pola halus pada piksel (‡1310); dan untuk audio, pola halus pada gelombang audio (‡1311). Gambar 3.8 mengilustrasikan hal ini.

Selain tanda air, konten yang dihasilkan AI juga dapat disimpan menggunakan format berkas yang menyimpan metadata tentang cara konten tersebut dihasilkan. Sebagai contoh, banyak perangkat seluler menyimpan berkas gambar dan audio menggunakan format berkas yang dapat menyimpan informasi tentang pengaturan kamera, waktu, lokasi, dan sebagainya (‡1312). Metadata serupa dapat digunakan untuk menyimpan informasi tentang apakah data dihasilkan oleh sistem AI. Sama seperti sidik jari dalam forensik kriminal, tanda air dan metadata dapat dimanipulasi atau dihapus, tetapi tetap berguna.

Para peneliti juga sedang berupaya mengembangkan detektor konten yang dihasilkan AI (‡1203, ‡1204, ‡1205*) untuk membantu mengidentifikasi konten yang dihasilkan AI di dunia nyata, bahkan ketika tidak tersedia watermark atau metadata. Namun, tingkat keberhasilan teknik identifikasi ini terbatas.

###@ Pembaruan

Sejak penerbitan Laporan terakhir (Januari 2025), telah ada kemajuan dalam pengembangan sistem AI dengan beberapa lapisan perlindungan yang efektif. Sebagaimana dibahas dalam §3.2. Praktik manajemen risiko, pertahanan berlapis merupakan prinsip inti dalam manajemen risiko (‡1314). Sebagai contoh, sistem AI yang menggabungkan model yang dilatih untuk keselamatan dengan filter masukan, filter keluaran, dan pemantau konten lainnya semakin banyak diteliti dan diterapkan (‡32, ‡65, ‡1182*). Penelitian terbaru juga menunjukkan bahwa, meskipun pengembang model telah mencapai kemajuan dalam meningkatkan ketahanan terhadap upaya untuk melewati perlindungan, penyerang masih berhasil dengan tingkat yang tinggi (Gambar 3.9).

###@ Kesenjangan bukti

‌
Kewajiban
1
)‌
Williams
dan lainnya, "Manajemen Risiko Organisasi."‌
Kewajiban
2
Williams
dan lainnya, "Kerangka Kerja Manajemen Risiko Kecerdasan Buatan."
Williams
dan lainnya, "Kerangka Kerja Manajemen Risiko Kecerdasan Buatan."

###@ Tantangan bagi para pembuat kebijakan

Tantangan utama bagi pembuat kebijakan mencakup penentuan apakah dan bagaimana mereka sebaiknya mendukung penelitian, pengembangan, evaluasi, dan penerapan perlindungan teknis serta metode pemantauan. Hal ini menantang karena pemahaman para ilmuwan tentang cara terbaik untuk menerapkan mekanisme perlindungan secara praktis masih terus berkembang dan praktik terbaik belum ditetapkan. Sebagai contoh, pengembang yang berbeda menerapkan perlindungan yang berbeda, dan pendekatan mereka terhadap mitigasi risiko teknis secara lebih luas sangat bervariasi (‡1116). Terakhir, keberadaan perlindungan teknis yang efektif tidak dengan sendirinya menjamin keselamatan, karena penerapan dan implementasinya dapat berbeda-beda di antara pengembang dan konteks penerapan.

