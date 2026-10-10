##########
>white|orangered|left|14|30|hr Bagian 3.4
### 3.4. Model dengan bobot terbuka
>white|orangered|left|24|30|hb Model berbobot terbuka

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Informasi utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Tingkat akses yang diberikan perusahaan AI terhadap ‘bobot’ model mereka memengaruhi risiko yang ditimbulkan oleh model tersebut. Bobot adalah parameter matematis yang memungkinkan model AI memproses masukan dan menghasilkan keluaran. Untuk model apa pun, perusahaan dapat memilih untuk merahasiakan bobot sepenuhnya, memberikan akses terbatas kepada sebagian pengguna, atau mengizinkan siapa pun mengunduhnya secara penuh. Model yang bobotnya tersedia untuk umum disebut ‘model dengan bobot terbuka’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Model berbobot terbuka memfasilitasi penelitian dan inovasi, tetapi mekanisme pengamanannya lebih mudah dihilangkan. Di seluruh dunia, berbagai pihak – terutama mereka yang memiliki sumber daya lebih sedikit – dapat menggunakan model berbobot terbuka untuk tujuan penelitian dan komersial. Namun, dibandingkan dengan model berbobot tertutup, model berbobot terbuka lebih mudah dimodifikasi agar menunjukkan perilaku yang berpotensi membahayakan, dan  s lebih sulit.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Perilisan model dengan bobot terbuka tidak dapat dibatalkan. Setelah dirilis, bobot model tidak dapat ditarik kembali. Hal ini mempersulit mitigasi potensi bahaya yang timbul akibat perilisan model dengan kemampuan berbahaya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), sejumlah rilis model berbobot terbuka utama telah mempersempit kesenjangan kapabilitas dengan model tertutup terkemuka. Pengembang asal Tiongkok DeepSeek dan Alibaba masing-masing merilis model R1 dan Qwen, yang mencapai kinerja sebanding dengan model tertutup terkemuka, sementara OpenAI merilis model berbobot terbuka pertamanya sejak 2019. Kapabilitas model tertutup terkemuka kini diperkirakan hanya unggul kurang dari satu tahun dibandingkan model berbobot terbuka terkemuka pada tolok ukur AI yang menonjol.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br ■ Salah satu tantangan kebijakan utama adalah memperoleh manfaat yang ditawarkan model berbobot terbuka sembari mengelola risiko khasnya. Salah satu pendekatannya adalah menilai model berbobot terbuka berdasarkan ‘risiko marginal’: sejauh mana peluncurannya secara kontrafaktual meningkatkan risiko sosial di luar risiko yang sudah ditimbulkan oleh model yang ada atau teknologi lainnya. Namun, dalam praktiknya, hal ini rumit. Peningkatan kecil pada risiko marginal dari waktu ke waktu juga dapat terakumulasi menjadi peningkatan risiko keseluruhan yang signifikan.
>oldlace|black||11|15|br      


Model dengan bobot terbuka, yang parameternya tersedia secara publik untuk diunduh, memiliki implikasi tersendiri terhadap banyak tantangan yang dibahas di bagian sebelumnya. ‘Bobot’ model AI memuat informasi penting yang memungkinkannya menghasilkan respons yang bermanfaat bagi pengguna. Setelah dirilis, bobot ini tidak dapat ditarik kembali: siapa pun dapat mengunduh, mempelajari, memodifikasi, membagikan, dan menggunakannya di komputer atau akun cloud mereka sendiri. Ketika bobot tersedia secara terbuka, pihak lain dapat lebih mudah mengembangkan dan memodifikasi model tersebut untuk memenuhi beragam kebutuhan serta mendorong inovasi (‡1317). Namun, melalui mekanisme yang sama, pengguna dengan niat jahat juga dapat lebih mudah menghapus pengamanan dan memodifikasi model berbobot terbuka untuk penggunaan yang berbahaya (‡1122, ‡1160). Hal ini memunculkan pertanyaan apakah beberapa model berbobot terbuka harus tunduk pada persyaratan khusus (misalnya, pengujian yang lebih ketat sebelum dirilis) atau, sebaliknya, diberikan pengecualian khusus (misalnya, dari persyaratan pelaporan regulasi) (‡1033).

###@ Latar Belakang Model dengan Bobot Terbuka

>white|orangered||14|15.5|bb Model dengan bobot terbuka dapat merupakan model ‘sumber terbuka’, tetapi belum tentu demikian.

Meskipun sering disebut sebagai ‘sumber terbuka’, sebagian besar model yang dirilis ke publik lebih tepat disebut sebagai ‘bobot terbuka’. Hal ini karena, meskipun pengembang menyediakan bobot model, mereka tidak merilis kode pelatihan atau kumpulan data terkait. Selain itu, perangkat lunak sumber terbuka biasanya dicirikan oleh lisensi permisif yang menetapkan persyaratan minimal bagi pelaku hilir yang menggunakan atau memodifikasi perangkat lunak tersebut (‡1318). Sebagai contoh, model Llama dari Meta memiliki ketentuan lisensi yang ketat dan hanya menyertakan kode inferensi, bukan kode pelatihan, sehingga biasanya tidak dianggap sebagai perangkat lunak sumber terbuka (‡1319, ‡1320). Opsi perilisan model berada dalam suatu spektrum, dari sepenuhnya tertutup hingga sepenuhnya bersumber terbuka, dengan pertukaran risiko-manfaat yang berbeda pada setiap titik (‡1086*, ‡1320, ‡1321). Tabel 3.9 menjelaskan opsi-opsi ini.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Tertutup sepenuhnya
  Pengguna sama sekali tidak dapat berinteraksi langsung dengan model.
  Contoh: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Akses yang di-hosting
  Pengguna hanya dapat berinteraksi melalui aplikasi atau antarmuka tertentu, seperti aplikasi chatbot seluler.
  Contoh: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Akses API ke model
  Pengguna dapat mengirim permintaan ke model melalui kode, sehingga model dapat digunakan dalam aplikasi eksternal.
  Contoh: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Akses API untuk fine-tuning
  Pengguna dapat menyempurnakan model agar sesuai dengan kebutuhan spesifik mereka.
  Contoh: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Bobot terbuka: bobot tersedia untuk diunduh
  Pengguna dapat mengunduh dan menjalankan model di komputer mereka sendiri.
  Contoh: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Bobot, data, dan kode tersedia untuk diunduh dengan batasan penggunaan
  Pengguna dapat mengunduh dan menjalankan model serta kode inferensi dan pelatihan, tetapi terdapat pembatasan lisensi tertentu atas penggunaannya.
  Contoh: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Terbuka sepenuhnya: bobot model, data, dan kode tersedia untuk diunduh tanpa batasan penggunaan.
  Pengguna memiliki kebebasan penuh untuk mengunduh, menggunakan, dan memodifikasi model, kode lengkap, dan data.
  Contoh: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 3.9: Opsi berbagi model mulai dari sepenuhnya tertutup hingga sepenuhnya terbuka
>white|black||9|11|br Pilihan ilustratif untuk berbagi model, mulai dari model yang sepenuhnya tertutup (model bersifat privat dan hanya digunakan secara eksklusif) hingga model yang sepenuhnya terbuka dan bersumber terbuka (bobot model, data, dan kode tersedia secara bebas untuk publik tanpa pembatasan penggunaan, modifikasi, dan berbagi). Model yang termasuk dalam empat kategori pertama sering disebut sebagai model “tertutup”. Bagian ini berfokus pada tiga baris terbawah. Sumber: diadaptasi dari Bommasani, 2024 (‡1317).


###@ Manfaat dan risiko

>white|orangered|left|14|15.5|bb Model berbobot terbuka dapat lebih mudah disesuaikan dan dievaluasi.

Model dengan bobot terbuka menawarkan manfaat signifikan bagi penelitian, inovasi, dan akses. Sebagaimana dibahas dalam §1.1. Apa itu AI serbaguna?, pelatihan model AI serbaguna sangat mahal – biaya pengembangan model terkemuka mencapai ratusan juta dolar. Merilis bobot model secara terbuka memungkinkan pihak yang sumber dayanya lebih terbatas untuk mereplikasi, mempelajari, dan mengembangkan sistem yang sudah ada. Tanpa akses semacam itu, masyarakat di wilayah dengan sumber daya terbatas berisiko tidak dapat menikmati manfaat AI, sehingga bobot terbuka sangat penting untuk memungkinkan partisipasi mayoritas global dalam pengembangan AI (‡1322). Pengembang hilir dapat melakukan penyetelan halus pada model untuk beragam aplikasi, misalnya mengadaptasinya untuk bahasa minoritas yang kurang terlayani atau mengoptimalkan kinerjanya untuk tugas tertentu, seperti penyusunan dokumen hukum atau pencatatan medis (‡1323, ‡1324*). Dengan demikian, model berbobot terbuka dapat memungkinkan lebih banyak orang dan masyarakat menggunakan dan memperoleh manfaat dari AI daripada yang mungkin terjadi jika tidak demikian (‡1325). Untuk model yang tidak cukup mumpuni untuk menimbulkan bahaya, manfaat ini mungkin lebih besar daripada risiko tambahan akibat merilis bobot secara terbuka, meskipun hal ini bergantung pada toleransi risiko para pengambil- keputusan terkait.

Rilis model berbobot terbuka juga memperluas kelompok pengembang dan peneliti yang dapat mempelajari model tersebut, mengevaluasi kemampuannya, menguji kerentanannya, dan melakukan iterasi untuk menyempurnakannya (‡1326, ‡1327). Hal ini meningkatkan kemungkinan bahwa aplikasi yang bermanfaat dan kelemahan yang berbahaya dapat teridentifikasi, meskipun hal ini tidak dijamin (‡1328, ‡1329). Pengguna juga dapat menjalankan model berbobot terbuka di perangkat mereka sendiri, sehingga mereka dapat tetap mengendalikan data sensitif dan menghindari pengiriman data tersebut ke server pihak ketiga.

Ada manfaat tambahan ketika pengembang membagikan informasi seperti data pelatihan, kode, alat evaluasi, dan dokumentasi, selain bobot model (‡1320, ‡1330, ‡1331, ‡1332*). Dengan lebih banyak informasi, pengembang hilir dan peneliti lain dapat lebih memahami model dengan bobot terbuka dan menyesuaikannya untuk aplikasi baru.

>white|orangered|left|14|15.5|bb Mekanisme pengamanan pada model berbobot terbuka lebih mudah dihilangkan, sehingga berpotensi memungkinkan penggunaan untuk tujuan jahat.

Model dengan bobot terbuka juga menimbulkan risiko tambahan karena pengamanannya lebih mudah dihapus. Meskipun model dengan bobot terbuka maupun model tertutup dapat memiliki pengamanan untuk menolak permintaan pengguna yang berbahaya, pengamanan ini jauh lebih mudah dihapus pada model dengan bobot terbuka. Pelaku jahat dapat menyempurnakan model lebih lanjut agar kinerjanya optimal untuk aplikasi berbahaya, menghapus bagian kode yang dirancang untuk mencegah penggunaan berbahaya, atau membatalkan penyempurnaan keselamatan sebelumnya (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Akibatnya, bobot model terbuka dapat memperparah risiko penyalahgunaan yang dibahas di §2.1. Risiko dari penggunaan jahat dengan memungkinkan lebih banyak pelaku memanfaatkan dan meningkatkan kemampuan yang sudah ada untuk tujuan jahat tanpa pengawasan (‡1122, ‡1315). Meskipun banyak pengguna tidak memiliki keterampilan atau dorongan untuk menghapus pengamanan pada model dengan bobot terbuka, pelaku jahat yang sangat termotivasi tetap menjadi kekhawatiran. Selain itu, pelaku jahat mungkin juga dapat menggunakan model dengan bobot terbuka untuk mengidentifikasi kerentanan dalam model tertutup serupa (‡1055*). Cacat semacam itu lebih sulit ditemukan hanya dengan menjalankan model tertutup, karena penyedia model tertutup dapat menerapkan langkah-langkah pengendalian dan pemantauan yang lebih ketat.

>white|orangered|left|14|15.5|bb Berbagi bobot model tidak dapat dibatalkan.

Setelah bobot model tersedia untuk diunduh oleh publik, tidak ada cara untuk menarik kembali secara menyeluruh semua salinan yang sudah ada. Platform hosting internet seperti GitHub dan Hugging Face dapat menghapus model dari platform mereka. Hal ini dapat mempersulit sebagian pihak untuk menemukan salinan yang dapat diunduh, sekaligus menjadi penghalang yang signifikan bagi banyak pengguna jahat yang tidak terlalu gigih (‡1339). Namun, pihak yang gigih tetap dapat memperoleh salinan jika model tersebut telah diunduh dan dihosting ulang di tempat lain atau disimpan secara lokal. Selain itu, pengembang hilir yang mengintegrasikan model dengan bobot- terbuka ke dalam sistem mereka juga mewarisi kelemahan apa pun, seperti kerentanan terhadap serangan adversarial (‡1055) atau kemampuan model untuk menghindari sistem pemantauan (lihat §2.2.2. Hilangnya kendali) (‡1315). Tidak seperti model tertutup, yang penyedianya dapat menerapkan perbaikan secara universal, pengembang model dengan bobot terbuka tidak dapat menjamin bahwa pengguna akan menerapkan pembaruan.

###@ Pembaruan

Sejak penerbitan Laporan terakhir (Januari 2025), kesenjangan kemampuan antara model berbobot terbuka terkemuka dan model tertutup telah menyempit. Pengembang Tiongkok telah menjadi penyedia model berbobot terbuka yang sangat penting. Pada Januari 2025, DeepSeek merilis model R1, yang mencapai kinerja sebanding dengan o1 milik OpenAI pada sejumlah tolok ukur (‡1340). Model Qwen milik Alibaba juga semakin populer dan menduduki posisi teratas sebagai model berbobot terbuka di Chatbot Arena, tolok ukur kinerja yang banyak digunakan, per Agustus 2025 (‡1341, ‡1342*). Pada Agustus 2025, OpenAI merilis model berbobot terbuka pertamanya sejak peluncuran GPT-2 pada 2019, yaitu gpt-oss-120b dan gpt-oss-20b. Meta terus merilis model Llama dengan bobot terbuka. Kemampuan model tertutup terkemuka kini diperkirakan hanya unggul kurang dari satu tahun dibandingkan model berbobot terbuka terkemuka pada tolok ukur AI yang banyak digunakan (Gambar 3.10).

###@ Kesenjangan bukti

Kesenjangan bukti utama berkaitan dengan efektivitas solusi teknis di dunia nyata untuk mencegah penyalahgunaan model berbobot terbuka. Para peneliti telah mengusulkan berbagai pendekatan untuk membuat model tahan terhadap manipulasi. Pendekatan ini mencakup teknik pelatihan baru yang dirancang untuk membuat model tahan terhadap modifikasi berbahaya (‡1276), penyaringan konten berbahaya dari data pelatihan (‡55), dan pertahanan terhadap serangan jailbreak (‡675, ‡676). Teknik-teknik ini kini mulai diterapkan dalam peluncuran produk di dunia nyata oleh para pengembang besar. Sebagai contoh, OpenAI menggunakan beberapa teknik ini pada model gpt-oss mereka, dan melaporkan bahwa versi yang disetel dengan baik secara adversarial tidak mencapai ambang kapabilitas yang tinggi (‡1344*). Namun, penelitian menunjukkan bahwa pelaku kejahatan dapat menonaktifkan mekanisme perlindungan dengan melatih ulang model menggunakan contoh-contoh berbahaya (‡1345, ‡1346). Selain itu, evaluasi keandalan mekanisme perlindungan secara andal masih menjadi tantangan, sehingga efektivitasnya dalam menghadapi serangan di dunia nyata belum dapat dipastikan (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Gambar 3.10: Kesenjangan kemampuan antara model AI berbobot terbuka dan tertutup terkemuka
>white|black||9|11|br Skor Epoch Capabilities Index (ECI) untuk model berbobot terbuka (biru tua) dan model tertutup (biru muda) dengan kinerja terbaik dari waktu ke waktu. ECI menggabungkan skor dari 39 tolok ukur ke dalam satu skala kapabilitas umum. Model berbobot terbuka terbaik tertinggal sekitar satu tahun dari model tertutup. Sumber: Epoch AI, 2025 (‡1343).


###@ Mitigasi

Mitigasi teknis terhadap risiko model dengan bobot terbuka diterapkan di seluruh proses pengembangan dan penerapan AI (‡1141, ‡1195, ‡1347). Sebagai contoh, saat model sedang dikembangkan, pengembang dan pihak yang mengadaptasi model di hilir dapat menyaring konten sensitif dari data pelatihan untuk meminimalkan kapabilitas yang berbahaya. Menghapus contoh berbahaya dari data pelatihan model dapat mencegah penyetelan halus adversarial dengan efektivitas 10 kali lebih tinggi dibandingkan pertahanan yang ditambahkan setelah pelatihan, meskipun hal ini juga dapat berdampak pada kapabilitas yang bermanfaat (‡55). Penyedia aplikasi AI juga dapat menerapkan mekanisme pelaporan dan penanganan insiden (‡1348).

Selain itu, platform hosting seperti HuggingFace dan GitHub dapat menetapkan ketentuan layanan platform untuk menghapus model yang dimodifikasi untuk tujuan berbahaya (‡1141, ‡1324). Pengembang model dapat memberikan akses penuh kepada auditor sebelum peluncuran, atau memilih strategi peluncuran ‘bertahap’ – merilis model kepada kelompok yang semakin besar (‡1086). Hal ini dapat membantu mengidentifikasi potensi malafungsi atau kerentanan sebelum model tersedia secara luas (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Kolom 3.1: Keamanan bobot model
>oldlace|black|left|13|15|hb  Kolom 3.1: Keamanan bobot model
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Risiko yang dibahas di bagian ini mengasumsikan bahwa bobot model dirilis secara sengaja. Namun, bobot model tertutup juga dapat diakses melalui pencurian atau kebocoran. Pengembangan model tertutup menelan biaya ratusan juta dolar (§1.1. Apa itu AI serbaguna?) dan, secara rata-rata, model tersebut lebih cakap daripada model dengan bobot terbuka (‡1343). Hal ini menjadikannya sasaran menarik bagi berbagai pelaku, mulai dari peretas amatir hingga negara-bangsa yang berupaya memperoleh model AI terdepan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bobot model tertutup yang dicuri akan menimbulkan risiko serupa dengan risiko yang dijelaskan di atas untuk model dengan bobot terbuka, tetapi mungkin tanpa langkah mitigasi apa pun. Pelaku jahat dapat menghapus pengamanan dari model yang paling canggih. Tidak seperti pengembang yang sah, pelaku semacam itu tidak akan menghadapi kendala reputasi, hukum, atau komersial yang saat ini mendorong perusahaan AI terdepan untuk menerapkan model mereka dengan aman.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Tingkat keamanan saat ini bervariasi di seluruh industri dan mungkin tidak memadai untuk menghadapi penyerang canggih. Beberapa pengembang berkomitmen untuk mengamankan bobot model dari sindikat kejahatan siber dan ancaman orang dalam (‡582), sementara yang lain belum membuat komitmen keamanan apa pun kepada publik (‡1109, ‡1349). Penelitian menunjukkan bahwa pusat data AI mungkin tidak mampu menahan serangan dari aktor yang paling canggih dan memiliki sumber daya besar (‡582, ‡1350, ‡1351). Hingga Desember 2025, belum ada kasus pencurian bobot model yang terkonfirmasi dan didokumentasikan secara publik. Namun, pelanggaran keamanan lain di perusahaan AI terkemuka telah dilaporkan, termasuk penyusupan ke sistem email Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Menutup kesenjangan keamanan ini akan membutuhkan investasi besar dalam perangkat keras, perangkat lunak, personel, dan keamanan fasilitas. Beberapa peningkatan keamanan dapat diterapkan relatif cepat dengan upaya terkoordinasi (‡1122). Namun, langkah-langkah kritis lainnya, seperti mengamankan rantai pasok perangkat keras dan fasilitas, kemungkinan akan memerlukan waktu bertahun-tahun (‡1122). Perusahaan swasta mungkin juga tidak memiliki sumber daya atau informasi untuk mengembangkan perlindungan yang memadai secara mandiri. Sebagai contoh, pengembang AI tidak memiliki akses ke intelijen ancaman rahasia yang dimiliki pemerintah (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Tantangan bagi para pembuat kebijakan

Tantangan utama bagi pembuat kebijakan adalah mengamankan manfaat berbagi model berbobot terbuka tanpa meningkatkan risiko secara signifikan. Untuk menghindari bahaya katastrofik, pengembang model berbobot terbuka tidak boleh merilis model tanpa mengevaluasi risikonya, baik dengan menggunakan metode penilaian yang telah mapan dan digunakan untuk model tertutup maupun dengan melakukan pengujian tambahan, mengingat pelaku berniat jahat dapat melakukan fine-tuning pada model dan menghapus perlindungan keselamatannya. Dalam praktiknya, hal ini mungkin sulit karena perkembangan kapabilitas bisa sulit diprediksi, perilisan model berbobot terbuka tidak dapat dibatalkan, dan upaya evaluasi diperlukan untuk memprediksi kapan suatu perilisan berpotensi menimbulkan bahaya yang signifikan. Salah satu pendekatannya adalah mengevaluasi ‘risiko marginal’ dari perilisan model terbuka: sejauh mana perilisan tersebut secara kontrafaktual meningkatkan risiko sosial di luar risiko yang telah ditimbulkan oleh model lain atau teknologi lain yang sudah ada (‡556, ‡1033, ‡1354, ‡1355) (lihat §3.2. Praktik pengelolaan risiko). Namun, memperkirakan bagaimana suatu sistem akan meningkatkan atau menurunkan risiko hilir setelah diterapkan merupakan hal yang kompleks dan bergantung pada konteks. Peningkatan risiko secara bertahap pada perilisan yang berurutan dapat terakumulasi seiring waktu hingga menjadi peningkatan risiko total yang substansial, sekalipun risiko marginal yang terkait dengan setiap perilisan tampak dapat diterima (‡1356, ‡1357). Sifat kapabilitas AI yang dapat digunakan untuk tujuan ganda semakin mempersulit tata kelola: fitur yang memungkinkan penerapan bermanfaat di bidang kedokteran atau penelitian dapat dialihgunakan untuk menimbulkan bahaya, dan setelah bobot model tersedia untuk umum, membedakan penggunaan yang sah dari penggunaan yang berniat jahat bisa sulit dilakukan. Tidak jelas pula siapa yang seharusnya dimintai pertanggungjawaban ketika model berbobot terbuka dimodifikasi untuk tujuan yang merugikan.

