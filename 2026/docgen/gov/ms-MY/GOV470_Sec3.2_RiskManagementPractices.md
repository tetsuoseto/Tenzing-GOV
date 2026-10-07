##########
>white|orangered|left|14|30|hr Bahagian 3.2
### 3.2. Amalan pengurusan risiko
>white|orangered|left|24|30|hb Amalan pengurusan risiko

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Maklumat utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pengurusan risiko AI tujuan umum merangkumi pelbagai amalan yang digunakan untuk mengenal pasti, menilai dan mengurangkan risiko daripada AI tujuan umum. Amalan ini termasuk pengujian dan penilaian pada peringkat model- (seperti ‘ujian pasukan merah’), proses organisasi yang membimbing keputusan pembangunan dan pelancaran, langkah perlindungan bersyarat (seperti komitmen ‘jika-maka’), serta pelaporan insiden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Beberapa pembangun AI telah menghasilkan Kerangka Keselamatan AI Barisan Hadapan. Kerangka ini merangkumi maklumat tentang penilaian risiko dan menetapkan langkah bersyarat seperti sekatan akses yang dirancang untuk dilaksanakan oleh syarikat bagi model yang lebih berkemampuan. Kerangka ini berbeza dari segi risiko yang diliputinya, cara ambang keupayaan ditakrifkan dan tindakan yang dicetuskan apabila ambang tersebut dicapai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bukti tentang keberkesanan amalan pengurusan risiko AI di dunia sebenar masih terhad. Kekurangan pelaporan insiden dan pemantauan menyukarkan penilaian tentang sejauh mana amalan semasa mengurangkan risiko atau dilaksanakan secara konsisten.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), pengurusan risiko menjadi lebih tersusun melalui inisiatif industri dan tadbir urus yang baharu. Instrumen baharu seperti Kod Amalan AI Tujuan Umum EU, Rangka Kerja Tadbir Urus Keselamatan AI China 2.0 dan Rangka Kerja Pelaporan Proses AI Hiroshima G7, bersama-sama inisiatif yang diterajui syarikat, menggambarkan trend ke arah pendekatan yang lebih piawai terhadap ketelusan, penilaian dan pelaporan insiden.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Dinamik pasaran dan kepantasan pembangunan AI menimbulkan cabaran tambahan. Disebabkan tekanan persaingan, syarikat AI mungkin perlu membuat pertukaran antara pelancaran produk yang lebih pantas dengan pelaburan dalam usaha mengurangkan risiko. Banyak kemudaratan berkaitan AI juga ditanggung oleh pihak luar, manakala liabiliti undang-undang bagi kemudaratan tersebut masih tidak jelas, dan proses tadbir urus mungkin lambat menyesuaikan diri dengan perubahan dalam landskap AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Cabaran utama bagi pembuat dasar termasuk menentukan keutamaan antara pelbagai risiko yang ditimbulkan oleh AI tujuan umum, serta menjelaskan pihak yang berada pada kedudukan terbaik untuk menguruskannya merentas rantaian nilai AI. Cabaran ini diburukkan lagi oleh keterlihatan yang terhad tentang cara risiko dikenal pasti, dinilai dan diuruskan dalam amalan, serta perkongsian maklumat yang tidak bersepadu antara pembangun, pihak yang menggunakan AI dan penyedia infrastruktur.
>oldlace|black||11|15|br      


Pengurusan risiko AI merangkumi pelbagai amalan yang bertujuan untuk mengenal pasti, menilai dan mengurangkan kebarangkalian serta tahap keterukan risiko yang berkaitan dengan sistem AI. Amalan ini boleh dilaksanakan oleh pembangun AI, pihak yang menerapkan AI, penilai dan pengawal selia. Contohnya termasuk pemodelan ancaman, pengelasan tahap risiko, ujian pasukan merah, pengauditan dan pelaporan insiden. Bahagian ini menggariskan amalan pengurusan risiko semasa, perkembangan baharu dan batasan yang masih wujud.

Sejak awal 2025, beberapa inisiatif antarabangsa baharu untuk pengurusan risiko AI tujuan umum telah dibangunkan, termasuk rangka kerja ketelusan organisasi dan pelaporan risiko serta rangka kerja kawal selia dan tadbir urus.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Angka 3.4: Empat komponen pengurusan risiko
>white|black||9|11|br Empat kategori kaedah untuk pengurusan risiko AI tujuan umum: pengenalpastian risiko; analisis dan penilaian risiko; mitigasi risiko; dan tadbir urus risiko. Semua ini membentuk proses yang berulang dan bersifat kitaran. Tadbir urus risiko, yang ditunjukkan di tengah, memudahkan kejayaan komponen lain. Sumber: International AI Safety Report 2026.


Cabaran yang masih wujud termasuk penyeragaman yang terhad, yang menyukarkan pematuhan dan penilaian, serta bukti yang terhad tentang keberkesanan dalam keadaan sebenar. Selain itu, konteks institusi, budaya dan politik berbeza di seluruh dunia, yang bermaksud pendekatan untuk mengenal pasti dan mengurus risiko, termasuk ambang risiko yang boleh diterima, mungkin berbeza mengikut rantau. Perbincangan dalam bahagian ini tentang pendekatan pengurusan risiko bersifat deskriptif: tujuannya adalah untuk memaklumkan pihak dalam ekosistem AI tentang pendekatan global semasa terhadap pengurusan risiko. Jika tersedia, bukti tentang keberkesanan dan batasan pendekatan ini turut dibincangkan, tetapi cadangan dasar berada di luar skop kerja ini.

###@ Komponen pengurusan risiko

Pengurusan risiko ialah proses berulang yang merangkumi amalan dan kaedah sepanjang kitaran pembangunan dan penggunaan AI, yang berfungsi bersama secara koheren (‡969). Pengurusan risiko untuk AI tujuan umum boleh melibatkan peranan pelbagai pihak, termasuk saintis data, jurutera model, juruaudit, pakar bidang, eksekutif, pengguna akhir, komuniti yang terkesan, pembekal pihak ketiga, penggubal dasar, kerajaan, organisasi piawaian dan organisasi masyarakat sivil (‡970, ‡971, ‡972). Piawaian pengurusan risiko terkemuka selalunya saling boleh kendali, tetapi menggunakan istilah yang berbeza untuk menerangkan elemen pengurusan risiko (‡973, ‡974). Lazimnya, piawaian tersebut mempunyai empat komponen yang saling berkaitan (Angka 3.4): mengenal pasti; menganalisis dan menilai; mengurangkan; dan mentadbir risiko (‡970, ‡973, ‡975, ‡976). Jadual di bawah memberikan contoh ilustrasi kaedah, teknik dan alat yang berkaitan. Amalan terus berkembang, maka jadual tersebut tidak merangkumi semuanya dan kesesuaiannya berbeza-beza mengikut konteks.

###@ Pengenalpastian risiko

Pengenalpastian risiko ialah proses mencari, mengenali dan menghuraikan risiko. Pengenalpastian risiko yang menyeluruh lazimnya merangkumi penilaian dipacu keupayaan, yang menguji sama ada model mempunyai keupayaan berbahaya tertentu (‡977), serta pemodelan risiko (‡978) dan peramalan (‡715*), yang digunakan untuk meneroka risiko sedia ada dan risiko yang sedang muncul. Meja 3.1 memberikan pelbagai contoh amalan pengenalpastian risiko. Pengenalpastian risiko juga melibatkan kerjasama dengan pakar dan komuniti yang berkaitan untuk memahami konteks yang lebih luas tentang bagaimana risiko timbul (‡979, ‡980). Mekanisme seperti program ganjaran pepijat boleh menyokong proses ini dengan memberikan insentif untuk mengenal pasti kelemahan yang belum diketahui sebelum ini (‡981) (Meja 3.1). Matlamat utama pengenalpastian risiko adalah untuk mengambil kira risiko yang diketahui umum dan difahami dengan baik, serta potensi risiko masa hadapan yang masih tidak menentu atau kurang dicirikan (‡982). Hal ini amat penting bagi AI tujuan umum, yang risikonya mungkin masih belum difahami sepenuhnya atau belum dapat diperhatikan (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Program ganjaran pepijat
  Program ganjaran pepijat atau program pendedahan kerentanan memberikan insentif kepada orang ramai untuk mencari dan melaporkan kerentanan dalam sistem AI. Beberapa pembangun telah melaksanakan program ganjaran pepijat (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perundingan pakar
  Pakar bidang, pengguna dan komuniti yang terjejas memberikan pandangan tentang risiko yang mungkin timbul. Garis panduan untuk AI yang bersifat partisipatif dan inklusif sedang berkembang (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rajah Tulang Ikan (Ishikawa)
  Rajah tulang ikan ialah alat analisis punca akar yang telah lama digunakan, dan para penyelidik telah mencadangkan penggunaannya untuk analisis berstruktur terhadap insiden risiko AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Peramalan
  Peramalan ialah proses meramalkan peristiwa atau trend pada masa hadapan berdasarkan analisis data masa lalu dan masa kini. Proses ini telah digunakan untuk membandingkan kemungkinan relatif, contohnya, pelbagai hasil ekonomi akibat AI lanjutan (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Taksonomi risiko
  Taksonomi risiko ialah cara untuk mengkategorikan dan menyusun risiko merentas pelbagai dimensi. Terdapat beberapa taksonomi yang menghuraikan risiko daripada AI tujuan umum (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perancangan senario
  Perancangan senario melibatkan pembangunan senario masa depan yang munasabah dan analisis tentang cara risiko menjadi kenyataan. Pendekatan ini telah digunakan untuk meneroka risiko dan impak model AI (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemodelan ancaman
  Pemodelan ancaman ialah proses mengenal pasti ancaman dan kelemahan dalam sesuatu sistem. Ramai pembangun AI menekankan penggunaan pemodelan ancaman untuk menjangkakan kemungkinan senario penyalahgunaan sistem AI (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.1: Contoh pengenalpastian risiko dalam pengurusan risiko AI tujuan umum
>white|black||9|11|br Contoh kaedah pengenalpastian risiko AI yang disenaraikan mengikut abjad. Kaedah yang disertakan
direka untuk menyokong pengenalpastian pelbagai jenis risiko, termasuk risiko daripada penggunaan berniat jahat, kerosakan fungsi dan risiko sistemik. Memandangkan pengurusan risiko AI tujuan umum masih di peringkat awal, tidak semua kaedah sesuai untuk setiap pembangun atau pihak yang menggunakan AI.


>white|orangered|left|14|15.5|bb Pemodelan ancaman dan taksonomi risiko ialah kaedah utama untuk mengenal pasti risiko.

Dua kaedah utama untuk mengenal pasti risiko daripada AI tujuan umum ialah pemodelan ancaman International AI Safety Report 2026 (proses berstruktur untuk memetakan cara risiko berkaitan AI mungkin berlaku) dan taksonomi risiko. Meta, sebagai contoh, menggunakan latihan pemodelan ancaman untuk menjangkakan senario penyalahgunaan yang berpotensi melibatkan model AInya (‡990), dan Anthropic menyertakan pemodelan ancaman sebagai sebahagian daripada ASL-3 Deployment Standard (‡991). Taksonomi risiko dan bahaya AI, yang menyenaraikan kategori risiko berserta contoh, juga boleh menjadi titik permulaan untuk mengkonseptualisasikan, mengenal pasti dan menentukan risiko utama yang berkaitan dengan AI tujuan umum dalam domain aplikasi tertentu (‡906, ‡988, ‡992, ‡993).

###@ Analisis dan penilaian risiko

Analisis dan penilaian risiko ialah proses menentukan tahap risiko model atau sistem AI dan membandingkannya dengan kriteria yang ditetapkan untuk menilai kebolehterimaan atau keperluan untuk mengurangkan risiko (‡994, ‡995, ‡996, ‡997). Proses ini merangkumi amalan seperti mengukur prestasi model berdasarkan penanda aras (‡998) dan penilaian (‡176, ‡715), menjalankan latihan red teaming (‡999*), penilaian impak (‡1000) dan audit (‡1001, ‡1002). Lihat Meja 3.2 untuk contoh analisis dan penilaian risiko AI tujuan umum. Kaedah ini direka untuk menyokong analisis dan penilaian bagi pelbagai jenis risiko yang berbeza secara serentak.

Matlamat utama analisis dan penilaian risiko ialah menjalankan penilaian terhadap keupayaan dan kerentanan model (‡1003), memanfaatkan pemodelan risiko yang mantap untuk memaklumkan keputusan tentang ambang risiko (‡1004, ‡1005), dan memahami cara sistem AI digunakan dalam amalan bagi menilai kesan hiliran terhadap masyarakat (‡869, ‡904, ‡905, ‡1006). Proses analisis dan penilaian risiko sering dianggap lebih berkemungkinan mengenal pasti risiko apabila proses tersebut melibatkan semakan bebas (‡1001, ‡1007), memanfaatkan kepakaran merentas sektor (‡1008), dan merangkumi pelbagai perspektif daripada berbilang bidang dan disiplin, serta daripada komuniti yang terjejas (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Audit
  Audit ialah semakan rasmi terhadap prestasi dan impak model AI dan/ atau pematuhan sesebuah organisasi terhadap piawaian, dasar dan prosedur, yang dijalankan secara dalaman atau oleh pihak luar. Pengauditan AI ialah bidang yang semakin berkembang, dan terdapat pelbagai alat dan amalan untuk mengaudit model AI serta amalan pembangun model AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penanda aras
  Penanda aras ialah ujian atau metrik piawai, yang selalunya bersifat kuantitatif, dan digunakan untuk menilai serta membandingkan prestasi sistem AI pada set tugas tetap yang direka untuk mewakili penggunaan dunia sebenar (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kaedah Bowtie
  Kaedah bowtie ialah kaedah yang terkenal untuk menggambarkan tempat kawalan boleh ditambah bagi mengurangkan peristiwa risiko. Kaedah ini membezakan dengan jelas antara pengurusan risiko proaktif dengan reaktif (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kaedah Delphi
  Kaedah Delphi ialah teknik membuat keputusan berkumpulan yang menggunakan siri soal selidik untuk mendapatkan konsensus daripada panel pakar (‡1020, ‡1021). Kaedah ini telah digunakan untuk membantu meneroka kemungkinan masa depan dengan AI termaju (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengujian lapangan
  Ujian lapangan menilai prestasi dan impak sistem AI dalam persekitaran operasi dunia- sebenar. Sesetengah penyelidikan menekankan ujian lapangan sebagai pelengkap kepada penilaian model untuk menilai hasil dan akibat dunia sebenar (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penilaian impak
  Penilaian impak menilai potensi impak sesuatu teknologi atau projek. Ini mungkin merangkumi pengkuantitian, pengagregatan dan pengutamaan impak. Sebagai contoh, Akta AI EU menghendaki pembangun sistem AI berisiko tinggi menjalankan Penilaian Impak Hak Asasi (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penilaian model
  Penilaian model merangkumi proses dan ujian untuk menilai dan mengukur prestasi model AI dalam tugasan tertentu. Terdapat banyak penilaian AI untuk menilai pelbagai keupayaan dan risiko, termasuk aspek keselamatan, sekuriti dan impak sosial (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penilaian risiko probabilistik
  Penilaian risiko probabilistik ialah metodologi untuk menilai risiko yang berkaitan dengan sistem atau proses kompleks dengan mengambil kira ketidakpastian. Metodologi ini telah disesuaikan untuk sistem AI canggih (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ujian pasukan merah
  Red-teaming ialah latihan yang melibatkan sekumpulan orang atau sistem automatik yang berpura-pura menjadi pihak lawan dan menyerang sistem teknologi sesebuah organisasi untuk mengenal pasti kelemahan. Banyak syarikat AI mempunyai amalan dalaman untuk menjalankan red-teaming terhadap sistem AI (‡458, ‡1028). Red-teaming juga boleh dijalankan oleh pihak di luar syarikat. Pasukan ini menghadapi cabaran seperti akses yang terhad, tetapi juga dapat mendedahkan pandangan yang berbeza (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Matriks risiko
  Matriks risiko ialah alat visual untuk membantu mengutamakan risiko berdasarkan kebarangkalian berlakunya risiko tersebut dan potensi impaknya (‡1027). Sesetengah pembangun AI menyertakan matriks risiko asas dalam Kerangka Kerja Keselamatan AI Frontier mereka (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ambang risiko/ tahap risiko
  Ambang atau tahap risiko ialah had kuantitatif atau kualitatif yang membezakan risiko yang boleh diterima daripada risiko yang tidak boleh diterima, serta mencetuskan tindakan pengurusan risiko tertentu apabila had tersebut dilampaui. Bagi AI tujuan umum, had ini ditentukan berdasarkan gabungan keupayaan, impak, sumber pengkomputeran, jangkauan dan faktor lain (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Toleransi risiko
  Toleransi risiko merujuk kepada tahap risiko yang sanggup diterima oleh sesebuah organisasi. Dalam AI, toleransi risiko sering ditetapkan secara tersirat melalui dasar dan amalan syarikat, manakala sesetengah rejim kawal selia mentakrifkan risiko yang tidak boleh diterima secara jelas dan mengenakan akibat undang-undang (‡1032). Sesetengah syarikat menghuraikan toleransi risiko mereka dari segi risiko marginal model baharu; iaitu sejauh mana model tersebut secara kontrafaktual meningkatkan risiko melebihi risiko yang telah ditimbulkan oleh model sedia ada atau teknologi lain (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kes keselamatan
  Kes keselamatan ialah hujah berstruktur, yang disokong oleh bukti, bahawa sesuatu sistem cukup selamat untuk dikendalikan dalam konteks tertentu. Literatur terkini (‡1037, ‡1038, ‡1039) telah meneroka kes keselamatan untuk sistem AI barisan hadapan, dan beberapa Rangka Kerja Keselamatan AI Barisan Hadapan merujuk kepadanya (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Analisis keselamatan sistem
  Analisis keselamatan sistem menonjolkan kebergantungan antara komponen dengan sistem yang merangkuminya, untuk menjangkakan bagaimana bahaya peringkat sistem boleh timbul daripada kegagalan komponen atau proses, atau interaksi antara subsistem, faktor manusia dan keadaan persekitaran. Pendekatan yang digunakan untuk sistem AI dalam literatur termasuk analisis proses teori sistem (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.2: Analisis/penilaian risiko dalam pengurusan risiko AI tujuan umum
>white|black||9|11|br Contoh kaedah untuk analisis/penilaian risiko AI, disenaraikan mengikut abjad. Memandangkan pengurusan risiko AI tujuan umum masih di peringkat awal, tidak semua kaedah sesuai untuk setiap pembangun atau pihak yang menggunakan AI.


>white|orangered|left|14|15.5|bb Alat analisis risiko yang lazim termasuk penanda aras dan penilaian model.

Penanda aras dan penilaian model ialah ujian piawai untuk menilai prestasi sistem AI tujuan umum dalam tugasan tertentu. Penyelidik telah membangunkan pelbagai penanda aras dan penilaian, termasuk set soalan aneka pilihan yang mencabar, masalah kejuruteraan perisian dan tugasan berkaitan kerja dalam persekitaran pejabat simulasi (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Penilaian keupayaan berbahaya (‡715) digunakan untuk menilai sama ada model atau sistem AI tujuan umum mempunyai pengetahuan atau kemahiran yang amat berbahaya, seperti keupayaan untuk membantu dalam serangan siber (lihat §2.1.3. Serangan siber).

Keputusan berimpak tinggi oleh syarikat dan kerajaan tentang pelancaran model sebahagiannya bergantung pada penilaian ini (‡1050, ‡1051, ‡1052). Walau bagaimanapun, penanda aras sangat berbeza dari segi kualiti dan skop (‡998, ‡1003), dan kesahihannya mungkin sukar dinilai disebabkan pelbagai kelemahan dalam amalan penandaarasan (‡902, ‡909, ‡1003, ‡1053*). Sebagai contoh, penanda aras boleh menjadi ‘tepu’ – apabila markah banyak model menghampiri markah tertinggi – yang bermakna penanda aras itu tidak lagi dapat membezakan model dengan jelas. Model juga semakin cenderung untuk mengenal pasti tugas tertentu sebagai penilaian dan menunjukkan tingkah laku yang berbeza daripada tingkah laku yang akan ditunjukkannya pada tugas serupa dalam konteks pelaksanaan, disebabkan oleh ‘kesedaran situasi’ (lihat §2.2.2. Kehilangan kawalan). Akhir sekali, batasan penanda aras dan penilaian telah didokumenkan dengan baik: khususnya, kedua-duanya gagal menangkap risiko yang berkaitan dengan penggunaan AI tujuan umum dalam domain baharu dan untuk tugas baharu, kerana keadaan ujian berbeza-beza daripada penggunaan dunia sebenar (‡913) (lihat §1.2. Keupayaan semasa dan §3.1. Cabaran teknikal dan institusi).

>white|orangered|left|14|15.5|bb Red-teaming membolehkan penilaian risiko yang lebih khusus mengikut domain- 

Kaedah lazim lain untuk menilai risiko ialah ujian pasukan merah. ‘Pasukan merah’ ialah sekumpulan penilai yang ditugaskan untuk mencari kerentanan, batasan atau potensi penyalahgunaan. Ujian pasukan merah boleh khusus kepada domain dan dijalankan oleh pakar domain, atau bersifat terbuka untuk meneroka faktor risiko baharu. Contohnya, pasukan merah mungkin meneroka serangan ‘jailbreak’ yang memintas sekatan keselamatan model (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Berbeza dengan penanda aras, kelebihan utama ujian pasukan merah ialah pasukan merah boleh menyesuaikan penilaian mereka dengan sistem khusus yang sedang diuji. Contohnya, pasukan merah boleh mereka bentuk input tersuai untuk mengenal pasti tingkah laku kes terburuk, peluang penggunaan berniat jahat dan kegagalan yang tidak dijangka. Walau bagaimanapun, kaedah ini mungkin memerlukan akses khas kepada model dan mungkin gagal mendedahkan kelas risiko yang penting (‡999, ‡1028).

Yang penting, ketiadaan risiko yang dikenal pasti tidak bermakna risiko tersebut rendah: kajian terdahulu menunjukkan bahawa pepijat kerap terlepas daripada pengesanan, terutamanya apabila pasukan merah mempunyai akses atau sumber yang terhad (‡1060). Penyelidikan juga mempersoalkan sama ada ujian pasukan merah dapat menghasilkan keputusan yang boleh dipercayai dan dihasilkan semula (‡1061). Komposisi pasukan merah dan arahan yang diberikan kepada penguji pasukan merah (‡1062), bilangan pusingan serangan (‡1063), serta akses model kepada alat (‡1064, ‡1065) boleh mempengaruhi hasil dengan ketara, termasuk permukaan risiko yang diliputi. Garis panduan komprehensif tentang ujian pasukan merah bertujuan menangani sebahagian daripada cabaran ini (‡1066).

###@ Mitigasi risiko

Mitigasi risiko ialah proses mengutamakan, menilai dan melaksanakan kawalan serta tindakan balas untuk mengurangkan risiko yang dikenal pasti. Contohnya termasuk kawalan akses (‡991), pemantauan berterusan (‡986) dan komitmen jika-maka (‡700). Mitigasi risiko menimbulkan persoalan penting: apakah tahap risiko yang boleh diterima? Rangka kerja terkini dan dasar syarikat telah mula memformalkan kriteria ‘penerimaan risiko’ (‡965, ‡1040). Walau bagaimanapun, menetapkan ambang yang sesuai masih mencabar, terutamanya bagi risiko yang mempunyai impak sosial yang meluas (‡986, ‡1067). Pada masa ini, tiada mekanisme yang mantap untuk mengesahkan keputusan penerimaan risiko yang dibuat oleh pembangun sebelum keluaran dilancarkan (‡1005).

Kaedah mitigasi risiko yang diterangkan dalam Meja 3.3 di bawah boleh disesuaikan dan dapat mengurangkan pelbagai risiko, termasuk sesetengah risiko yang tidak dijangka. Meja ini tidak merangkumi kaedah mitigasi teknikal seperti latihan adversarial, penapis kandungan dan pemantauan rantaian pemikiran. Kaedah ini dibincangkan dalam §3.3. Perlindungan dan pemantauan teknikal, serta di seluruh Laporan dalam perenggan ‘Mitigasi’ bagi setiap risiko dalam §2. Risiko.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dasar penggunaan yang boleh diterima
  Polisi penggunaan yang boleh diterima ialah satu set peraturan dan garis panduan untuk penggunaan model AI yang bertanggungjawab, beretika dan sah di sisi undang-undang. Lazimnya, pembangun AI menerbitkan polisi penggunaan yang boleh diterima, serta polisi penggunaan yang dilarang, bersama-sama keluaran model baharu (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kawalan akses/saringan pengguna
  Kawalan akses merangkumi penggunaan dasar dan peraturan untuk mengehadkan akses kepada model AI, data dan sistem berdasarkan peranan pengguna, atribut dan syarat lain bagi mencegah penggunaan tanpa kebenaran, manipulasi atau pelanggaran data. Syarikat AI kerap menyahaktifkan akaun yang didapati terlibat dalam kegiatan jenayah (‡486) dan menjalankan tapisan pengguna serta saringan Kenali-Pelanggan-Anda bagi memastikan model hanya digunakan oleh pihak yang dipercayai (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Spesifikasi tingkah laku/model
  Spesifikasi tingkah laku AI ialah dokumen yang mentakrifkan cara model AI harus berkelakuan dalam pelbagai situasi. Dokumen ini berfungsi sebagai pelan untuk penjajaran dan keselamatan AI, serta membimbing pembangunan, latihan, penilaian dan output model. Beberapa syarikat AI menggunakan dokumen spesifikasi model dan menerbitkan sekurang-kurangnya sebahagian daripadanya (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantauan berterusan
  Pemantauan berterusan ialah proses berterusan dan automatik untuk memerhati, menganalisis dan mengawal sistem AI yang sedang digunakan, menjejak prestasinya dan mengehadkan tingkah lakunya bagi memastikan kebolehpercayaan, keberkesanan dan keselamatan. Terdapat pelbagai alat yang tersedia untuk pemantauan berterusan (‡1073*) serta teknik untuk menyokong
Kebolehcerapan AI (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pertahanan berlapis
  Pertahanan berlapis ialah konsep bahawa beberapa lapisan pertahanan yang bebas dan bertindih boleh dilaksanakan supaya jika satu lapisan gagal, lapisan lain masih berkesan (‡1075, ‡1076). Beberapa Rangka Kerja Keselamatan AI Frontier merujuk konsep ini (cth. (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantauan ekosistem
  Ini ialah proses memantau ekosistem AI yang lebih luas, termasuk penjejakan pengkomputeran dan perkakasan, asal usul model, asal usul data dan corak penggunaan. Literatur penyelidikan membincangkan pemantauan sedemikian berkaitan dengan risiko daripada AI tujuan umum (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Komitmen jika-maka
  Komitmen jika-maka ialah satu set protokol dan komitmen teknikal serta organisasi untuk mengurus risiko apabila model AI menjadi semakin berkebolehan. Beberapa pembangun AI menggunakan jenis komitmen ini sebagai sebahagian daripada Kerangka Keselamatan AI Termaju mereka (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Garis merah atau larangan
  Garis merah ialah sempadan khusus yang dinyatakan dari segi keupayaan, impak atau jenis penggunaan. Konsep ini muncul dalam kenyataan awam dan inisiatif, serta dalam larangan kawal selia (‡1079, ‡1080, ‡1081). Literatur juga menyatakan keterbatasan pendekatan garis merah, termasuk cabaran untuk mencapai konsensus dan memastikan kebolehkuatkuasaan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi keluaran dan penggunaan
  Strategi keluaran dan penggunaan AI kegunaan umum boleh merangkumi keluaran berperingkat atau akses API supaya lebih banyak pilihan mitigasi tersedia sekiranya berlaku penyalahgunaan atau kemudaratan yang tidak dijangka (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.3: Pengurangan risiko dalam pengurusan risiko AI tujuan umum
>white|black||9|11|br Contoh kaedah untuk mitigasi risiko AI yang disenaraikan mengikut abjad. Kaedah yang disertakan direka untuk menyokong mitigasi pelbagai jenis risiko secara serentak, termasuk risiko daripada penggunaan berniat jahat, risiko daripada kerosakan fungsi dan risiko sistemik. Memandangkan pengurusan risiko AI serba guna masih di peringkat awal, tidak semua kaedah sesuai untuk setiap pembangun atau pihak yang melaksanakan AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Angka 3.5: ‘Gambar rajah keju Swiss’ yang menggambarkan pendekatan pertahanan berlapis
>white|black||9|11|br Pelbagai lapisan pertahanan boleh mengimbangi kelemahan dalam setiap lapisan. Teknik pengurusan risiko AI yang digunakan pada masa ini mempunyai kelemahan, tetapi menggabungkannya secara berlapis boleh memberikan perlindungan yang jauh lebih kukuh daripada risiko. Sumber: Laporan Keselamatan AI Antarabangsa 2026.


>white|orangered|left|14|15.5|bb Strategi pertahanan berlapis dan strategi pelepasan ialah alat mitigasi yang penting.

Model ‘pertahanan berlapis’ boleh menyokong pengurusan risiko AI tujuan- umum. Dalam konteks ini, ‘pertahanan berlapis’ merujuk kepada gabungan langkah teknikal, organisasi dan kemasyarakatan yang diterapkan merentasi pelbagai peringkat pembangunan dan penggunaan (Angka 3.5). Ini bermakna mewujudkan lapisan perlindungan bebas, supaya jika satu lapisan gagal, lapisan lain masih dapat mencegah kemudaratan. Contoh model pertahanan berlapis yang sering disebut ialah pelbagai langkah pencegahan yang digunakan untuk mencegah penyakit berjangkit. Vaksin, pelitup muka dan amalan mencuci tangan, antara langkah-langkah lain, boleh mengurangkan risiko jangkitan dengan ketara apabila digabungkan, walaupun tiada satu pun kaedah ini berkesan 100% jika digunakan secara berasingan (‡1083*). Bagi AI tujuan umum, pertahanan- berlapis akan merangkumi kawalan yang bukan pada model AI itu sendiri, tetapi pada ekosistem yang lebih luas. Ini termasuk (contohnya) kawalan terhadap bahan yang diperlukan untuk melancarkan serangan biologi seperti reagen (‡1084, ‡1085). Walau bagaimanapun, langkah pertahanan- berlapis terutamanya menangani risiko yang berkaitan dengan kemalangan, kegagalan fungsi dan penggunaan berniat jahat, dan mungkin memainkan peranan yang lebih kecil dalam mengurus risiko sistemik (lihat §3.5. Membina daya tahan masyarakat).

Strategi keluaran dan pelaksanaan sesebuah syarikat merupakan komponen penting dalam mitigasi risiko. Keputusan tentang cara model disediakan kepada pengguna boleh mempengaruhi pendedahan risiko dengan ketara (‡1082). Pilihan keluaran dan pelaksanaan yang berbeza termasuk keluaran berperingkat kepada kumpulan pengguna yang terhad, akses melalui perkhidmatan dalam talian terkawal (seperti API), serta penggunaan perjanjian pelesenan dan dasar penggunaan yang boleh diterima yang melarang aplikasi berbahaya tertentu dari segi undang-undang (‡176, ‡1086, ‡1087). §3.4. Model pemberat terbuka membincangkan dengan lebih terperinci bagaimana pengeluaran pemberat model mempengaruhi risiko.

###@ Tadbir urus risiko

Tadbir urus risiko ialah proses yang menghubungkan penilaian, keputusan dan tindakan pengurusan risiko dengan strategi dan objektif sesebuah organisasi atau entiti lain (‡1088, ‡1089). Meja 3.4 memberikan gambaran keseluruhan tentang teknik tadbir urus risiko yang lazim. Seperti yang ditunjukkan dalam Angka 3.4, tadbir urus risiko boleh difahami sebagai teras pengurusan risiko kerana ia memudahkan pengoperasian komponen pengurusan risiko yang lain dengan berkesan. Tadbir urus risiko menyediakan akauntabiliti, ketelusan dan kejelasan yang menyokong keputusan pengurusan risiko berdasarkan maklumat yang mencukupi. Tadbir urus risiko boleh merangkumi amalan seperti pelaporan insiden (‡1090), pengagihan tanggungjawab risiko (‡965) dan perlindungan pemberi maklumat (‡1091). Secara lebih luas, tadbir urus risiko boleh merangkumi panduan, rangka kerja, perundangan, peraturan, piawaian kebangsaan dan antarabangsa, serta inisiatif latihan dan pendidikan. Tujuan utama tadbir urus risiko adalah untuk menetapkan dasar dan mekanisme organisasi yang menjelaskan cara tanggungjawab pengurusan risiko diagihkan di seluruh organisasi atau entiti lain, bagi menyokong penyeliaan dan akauntabiliti yang sewajarnya (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dokumentasi
  Amalan dokumentasi membantu menjejak maklumat penting tentang sistem AI, seperti data latihan, pilihan reka bentuk, kegunaan yang dimaksudkan, batasan dan risiko. ‘Kad model’ dan ‘kad sistem’, yang memberikan maklumat tentang cara model atau sistem AI dilatih dan dinilai, ialah contoh amalan terbaik dokumentasi AI yang utama (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pelaporan insiden
  Pelaporan insiden ialah proses mendokumentasikan dan berkongsi secara sistematik kes apabila pembangunan atau penggunaan AI telah menyebabkan kemudaratan secara langsung atau tidak langsung. Terdapat beberapa platform yang memudahkan pelaporan insiden berkaitan AI (‡1096, ‡1097), serta rangka kerja untuk menjadikan pelaporan insiden AI lebih berkesan (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Rangka kerja pengurusan risiko
  Rangka kerja pengurusan risiko ialah pelan organisasi untuk mengurangkan jurang dalam liputan risiko, menyelaraskan pelbagai aktiviti pengurusan risiko dan melaksanakan mekanisme semak dan imbang. Rangka kerja khusus untuk AI tujuan umum (‡986, ‡1098) sering merujuk kepada langkah-langkah lain yang disebut dalam bahagian ini.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Daftar risiko
  Daftar risiko ialah repositori yang mengandungi pelbagai risiko, keutamaan risiko tersebut, pemiliknya dan pelan mitigasi. Daftar seperti ini agak lazim dalam banyak industri, termasuk keselamatan siber (‡1099), dan kadangkala digunakan untuk memenuhi keperluan pematuhan kawal selia.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengagihan tanggungjawab risiko
  Pembahagian peranan dan tanggungjawab bagi pengurusan risiko dalam sesebuah organisasi boleh menstrukturkan pengawasan dalaman terhadap pembuatan keputusan (‡1002, ‡1093). Pengaturan sedemikian tercermin dalam sesetengah rangka kerja tadbir urus, termasuk Kod Amalan AI Tujuan Umum EU (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Laporan ketelusan
  Laporan ketelusan menerangkan amalan pengurusan risiko syarikat AI dengan mendedahkan maklumat tertentu kepada orang ramai atau berkongsi dokumentasi dengan kumpulan industri atau badan kerajaan. Contohnya, banyak syarikat AI menyerahkan laporan ketelusan Proses AI Hiroshima (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Perlindungan pemberi maklumat
  Memandangkan sebahagian besar pembangunan AI berlaku secara tertutup, sesetengah rangka kerja tadbir urus merangkumi perlindungan pemberi maklumat bagi membolehkan pendedahan risiko yang berpotensi kepada pihak berkuasa (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.4: Tadbir urus risiko dalam pengurusan risiko AI tujuan umum
>white|black||9|11|br Contoh kaedah untuk tadbir urus risiko AI yang disenaraikan mengikut abjad. Kaedah yang disertakan direka untuk menyokong tadbir urus risiko bagi pelbagai jenis risiko secara serentak, termasuk risiko daripada penggunaan berniat jahat, risiko daripada kerosakan fungsi dan risiko sistemik. Memandangkan pengurusan risiko AI tujuan umum masih di peringkat awal, tidak semua kaedah sesuai untuk setiap pembangun atau penerap AI.


>white|orangered|left|14|15.5|bb Dokumentasi dan ketelusan ialah komponen tadbir urus risiko.

Mekanisme dokumentasi dan ketelusan institusi, bersama-sama dengan amalan perkongsian maklumat, memudahkan penelitian luaran dan menyokong usaha untuk mengurus risiko yang berkaitan dengan kecerdasan buatan tujuan umum (‡1101, ‡1102). Amalan menerbitkan hasil ujian prapelancaran dalam ‘kad model’ atau ‘kad sistem’, berserta butiran asas tentang model atau sistem itu, termasuk cara model atau sistem itu dilatih dan potensi batasannya, kini menjadi kebiasaan (‡1094, ‡1095). Sesetengah pembangun juga menerbitkan laporan ketelusan yang merangkumi butiran tentang amalan pengurusan risiko mereka secara lebih meluas (‡1103). Unsur dokumentasi dan ketelusan yang lain termasuk pemantauan dan pelaporan insiden (‡176, ‡1083*, ‡1103) serta perkongsian maklumat, yang boleh difasilitasi oleh pihak ketiga seperti Frontier Model Forum. Sesetengah rangka kerja kawal selia, seperti Akta AI EU atau California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53) (‡1081, ‡1104), mewajibkan perkongsian maklumat tentang risiko kecerdasan buatan tujuan umum dalam sesetengah keadaan.

>white|orangered|left|14|15.5|bb Komitmen kepimpinan dan insentif membentuk amalan pengurusan risiko.

Budaya organisasi, struktur kepimpinan dan insentif mempengaruhi usaha pengurusan risiko dalam pelbagai cara (‡1105). Komitmen kepimpinan dan struktur insentif sering mempengaruhi cara dasar pengurusan risiko dilaksanakan dalam amalan. Sesetengah pembangun mempunyai panel dalaman untuk membuat keputusan yang membincangkan cara mereka bentuk, membangunkan dan menyemak sistem AI baharu dengan selamat dan bertanggungjawab. Jawatankuasa penyeliaan dan penasihat, amanah atau lembaga etika AI juga boleh berfungsi sebagai mekanisme untuk memberikan panduan pengurusan risiko dan melaksanakan penyeliaan organisasi (‡1092*, ‡1106, ‡1107, ‡1108). Para penyelidik berhujah bahawa cabaran dalam tadbir urus kendiri secara sukarela bermakna pengauditan, pengesahan dan penyeragaman oleh pihak ketiga dapat membantu memperkukuh pengurusan risiko AI tujuan umum (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Pengurusan risiko organisasi, ketelusan dan rangka kerja pelaporan risiko

Beberapa inisiatif baharu memberi tumpuan kepada proses pengurusan risiko, dokumentasi dan ketelusan. Dalam bentuknya yang terkini, Kod Amalan AI Tujuan Umum EU berfungsi sebagai rangka kerja sukarela untuk membimbing amalan ketelusan, hak cipta, keselamatan dan sekuriti bagi menyokong pematuhan terhadap peruntukan Akta AI EU untuk AI tujuan umum (‡965). Setakat Disember 2025, lebih daripada dua puluh syarikat† telah menandatanganinya. Rangka Kerja Pelaporan Proses AI Hiroshima G7 (HAIP) (‡1100) ialah rangka kerja antarabangsa pertama untuk pelaporan awam secara sukarela tentang amalan pengurusan risiko organisasi bagi sistem AI lanjutan. Sekurang-kurangnya 20 pembangun telah menerbitkan laporan ketelusan awam yang meliputi pengenalpastian risiko, metrik penilaian, strategi mitigasi dan proses keselamatan data.

Pembangun AI telah menerima pakai komitmen ketelusan sukarela. Di China, ikrar oleh 17 syarikat AI China, yang diselaraskan oleh AI Industry Alliance of China, diumumkan pada Disember 2024 (‡1113) dan dikemas kini pada 2025 (‡1114). Pada Sidang Kemuncak AI Seoul Mei 2024 di Korea Selatan, 16 pembangun AI dari pelbagai negara menandatangani komitmen sukarela untuk menerbitkan Kerangka Keselamatan AI Frontier bagi model dan sistem mereka yang paling berkeupayaan, serta menerima pakai amalan pengurusan risiko merentas peringkat pembangunan dan pelaksanaan model (‡1052).

    Nota † -- Penandatangan setakat Disember 2025 termasuk: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, dan WRITER.

>white|orangered|left|14|15.5|bb Kerangka Keselamatan AI Termaju telah menjadi pendekatan organisasi yang menonjol untuk pengurusan risiko AI.

Sejak 2023, beberapa pembangun AI barisan hadapan telah menerbitkan dokumen secara sukarela yang menerangkan cara mereka merancang untuk mengenal pasti dan menangani risiko serius daripada sistem mereka yang paling canggih. Rangka Kerja Keselamatan AI Barisan Hadapan ini menerangkan cara pembangun AI merancang untuk menilai, memantau dan mengawal model serta sistem AI mereka yang paling canggih sebelum dan semasa penggunaan. Rangka kerja ini mempunyai banyak persamaan, tetapi berbeza dalam beberapa aspek penting (‡1115, ‡1116). Kebanyakannya menumpukan pada risiko yang berkaitan dengan ancaman kimia, biologi, radiologi dan nuklear (CBRN), keupayaan siber lanjutan dan tingkah laku autonomi lanjutan (‡1115, ‡1117). Sebilangan kecil rangka kerja menangani domain risiko tambahan seperti diskriminasi yang menyalahi undang-undang pada skala besar dan eksploitasi seksual kanak-kanak.

Beberapa pembangun mengemas kini kerangka kerja mereka pada 2025, dengan menambah bahagian baharu tentang manipulasi berbahaya, risiko ketidakselarasan, serta replikasi dan penyesuaian autonomi (‡1078, ‡1118). Walaupun banyak kerangka kerja menerangkan pendekatan pengurusan risiko yang serupa – termasuk pemodelan ancaman, ujian red-team dan penilaian keupayaan berbahaya – kerangka kerja tersebut berbeza dari segi takrif tahap dan ambang risiko, kekerapan penilaian, jurang penampan antara penilaian dengan ambang, serta kelengkapan komitmen mitigasi masing-masing (contohnya, sama ada komitmen itu merangkumi pemadaman pemberat model atau sekadar penggantungan pembangunan) (‡1115, ‡1119). Lihat Meja 3.5 untuk maklumat lanjut.

>white|orangered|left|14|15.5|bb Banyak tindakan dalam Rangka Kerja Keselamatan AI Frontier berasaskan komitmen jika-maka.

Bahagian penting dalam Rangka Kerja Keselamatan AI Frontier ialah ‘komitmen jika-maka’. Ini ialah protokol bersyarat yang mencetuskan tindak balas khusus apabila model dan sistem AI mencapai ambang keupayaan yang telah ditetapkan (‡1120). Contohnya, komitmen jika-maka mungkin menyatakan bahawa jika didapati sesuatu model berupaya membantu orang baharu dengan ketara dalam mencipta dan menggunakan senjata CBRN, maka pembangun akan melaksanakan langkah keselamatan yang dipertingkat, kawalan penggunaan dan pemantauan masa nyata (‡991*).

Pada 2025, beberapa pembangun AI mengumumkan bahawa model baharu mencetuskan amaran awal atau bahawa mereka tidak dapat menolak kemungkinan bahawa penilaian lanjut akan menunjukkan model telah melepasi ambang keupayaan. Hal ini mendorong mereka melaksanakan perlindungan yang dipertingkatkan sebagai langkah berjaga-jaga (‡7, ‡33, ‡1121*). Kerangka Keselamatan AI Frontier lazimnya memerlukan penilaian keupayaan awal sebelum mitigasi risiko, serta analisis risiko baki atau kes keselamatan, yang selalunya dimaklumkan oleh aktiviti red-teaming, selepas mitigasi. Lihat Meja 3.5 untuk maklumat terperinci.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Kerangka Kesiapsiagaan 2 (‡1078*)
  Risiko yang dilindungi:
1. Keupayaan biologi dan kimia
2. Keupayaan keselamatan siber
3. Keupayaan AI untuk memperbaik dirinya sendiri
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
- Tinggi: Boleh memperkuat laluan sedia ada yang membawa kepada kemudaratan serius (Memerlukan kawalan keselamatan dan perlindungan)
- Kritikal: Boleh memperkenalkan laluan baharu yang belum pernah berlaku sebelum ini kepada kemudaratan serius (Hentikan pembangunan selanjutnya sehingga piawaian perlindungan dan kawalan keselamatan yang ditetapkan memenuhi tahap Kritikal)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Dasar Penskalaan Bertanggungjawab 2.2 (‡991*)
  Risiko yang dilindungi:
1. senjata CBRN
2. Penyelidikan dan pembangunan AI autonomi (AI R&D)
3. Operasi siber (sedang dinilai)
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Tahap Keselamatan AI (ASL)
- ASL-1: Tiada risiko malapetaka yang ketara
- ASL-2: Tanda awal keupayaan berbahaya (Model mesti memenuhi Piawaian Penerapan dan Keselamatan ASL-2)
- ASL-3: Risiko penyalahgunaan yang membawa bencana meningkat dengan ketara (Model mesti memenuhi Piawaian Penerapan dan/ atau Keselamatan ASL-3)
- ASL-4+: Pengelasan masa hadapan (belum ditakrifkan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Rangka Kerja Keselamatan AI Frontier 3.0 (‡1040*)
  Risiko yang dilindungi:
1. Penyalahgunaan
    a. CBRN
    b. Siber
    c. Manipulasi berbahaya
2. R&D pembelajaran mesin
3. Ketidakselarasan/ Penaakulan instrumental
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Tahap Keupayaan Kritikal
    Tahap keupayaan yang, tanpa langkah mitigasi (keselamatan untuk penggunaan dan mitigasi keselamatan yang sejajar dengan tahap keselamatan RAND 2, 3 atau 4 (‡1122)), model atau sistem AI mungkin menimbulkan risiko bahaya serius yang lebih tinggi. Tahap keupayaan tersebut merangkumi ‘penilaian amaran awal’, dengan ‘ambang amaran’ khusus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Kerangka Kerja AI Frontier 1.1 (‡990*)
  Risiko yang dilindungi:
1. Keselamatan siber
2. Risiko kimia dan biologi
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Tahap Ambang Risiko
- Sederhana (keluarkan dengan langkah keselamatan dan mitigasi yang sesuai)
- igh (jangan keluarkan)
- Kritikal (hentikan pembangunan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Rangka Kerja Keselamatan Model Frontier (‡1123*)
  Risiko yang dilindungi:
1. Proliferasi senjata CBRN
2. Operasi siber ofensif
3. Penyelidikan dan Pembangunan AI Automatik
  Tahap risiko atau yang setara serta langkah perlindungan berkaitan:
  Ambang Keupayaan Kritikal
    Keupayaan model yang berpotensi menyebabkan kemudaratan besar kepada orang awam jika disalahgunakan. (Jika ambang dipenuhi atau dilebihi, model tidak akan dilancarkan kepada umum tanpa langkah mitigasi risiko yang sewajarnya)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Rangka Kerja Tadbir Urus Sempadan Hadapan (‡1124*)
  Risiko yang dilindungi:
1. senjata CBRN
2. Operasi siber ofensif
3. Autonomi lanjutan (termasuk R&D AI)
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Tahap Risiko
- Rendah atau Sederhana (Penggunaan dibenarkan selaras dengan keperluan Program AI Bertanggungjawab)
- Tinggi atau Kritikal (Semakan lanjut dan langkah mitigasi

(diperlukan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Penilaian Risiko AI Barisan Hadapan (‡1029*)
  Risiko yang dilindungi:
1. Kesalahan siber
2. CBRN
3. Pujukan dan manipulasi
4. Diskriminasi yang menyalahi undang-undang secara besar-besaran

  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Ambang Risiko – skor risiko model (MR)
- MR1 atau MR2 (Keputusan penilaian didokumenkan oleh pasukan kejuruteraan)
- MR3 (Langkah mitigasi risiko dan hasil penilaian didokumenkan oleh pasukan kejuruteraan dan disemak secara berkala)
- MR4 (Penilaian risiko terperinci perlu dilengkapkan dan kelulusan ketua unit perniagaan diperlukan)
- MR5 (Penilaian risiko terperinci hendaklah diselesaikan dan diluluskan oleh jawatankuasa bebas, contohnya jawatankuasa etika AI NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Rangka Kerja Model Frontier AI Selamat (‡1125*)
  Risiko yang dilindungi:
1. Penggunaan berniat jahat (cth. perisian hasad, eksploitasi seksual kanak-kanak)
2. Kemudaratan dalam penggunaan biasa yang tidak berniat jahat, contohnya output yang mengakibatkan hasil diskriminasi yang menyalahi undang-undang atau penjanaan kod yang tidak selamat.
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Kebarangkalian dan Keterukan Kemudaratan dalam Konteks
- Rendah
- Sederhana
- Tinggi
- Sangat Tinggi
    (Langkah mitigasi risiko dan kawalan keselamatan telah dilaksanakan untuk semua sistem dan proses; langkah mitigasi tambahan perlu disesuaikan dengan sistem AI dan kes penggunaan model tersebut)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Dasar Kesediaan AGI (‡1127*)
  Risiko yang dilindungi:
1. Kesalahan siber
2. Penyelidikan dan Pembangunan AI Automatik
3. Replikasi dan penyesuaian autonomi
4. Bantuan senjata biologi
  Tahap risiko atau yang setara dan langkah perlindungan yang berkaitan:
  Ambang Keupayaan Kritikal
    Ambang kuantitatif pada penanda aras keupayaan (Jika dilepasi, jalankan penilaian keupayaan berbahaya, langkah keselamatan maklumat dan mitigasi penggunaan, atau hentikan pembangunan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: Dasar Kesediaan AGI (‡1127*)
  Risiko yang dilindungi:
1. Kesalahan siber
2. Penyelidikan dan Pembangunan AI Automatik
3. Replikasi dan penyesuaian autonomi
4. Bantuan senjata biologi
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Ambang Keupayaan Kritikal
    Ambang kuantitatif pada penanda aras keupayaan (Jika dilampaui, jalankan penilaian keupayaan berbahaya, langkah keselamatan maklumat dan mitigasi penggunaan, atau hentikan pembangunan)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Rangka Kerja Keselamatan AI (‡1128*)
  Risiko yang dilindungi:
1. Kehilangan kawalan
2. Penyalahgunaan (cth. persenjataan biokimia

  Peringkat risiko atau yang setara serta langkah perlindungan berkaitan:
  Tahap Risiko
- Risiko rendah (Gunakan sistem AI, tetapi lakukan pemantauan selepas itu untuk menguruskan risiko)
- Risiko dikenal pasti (Sama ada buka sistem AI hanya kepada pengguna yang dibenarkan untuk mengurangkan risiko, atau tangguhkan pelaksanaan sehingga langkah keselamatan tambahan diambil, bergantung pada kes penggunaan)
- Risiko tinggi (Jangan gunakan sistem AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Rangka Kerja Keselamatan AI Barisan Hadapan (‡1129*)
  Risiko yang dilindungi:
1. Ancaman biologi
2. Keselamatan siber ofensif
3. Operasi autonomi dan manipulasi lanjutan
  Tahap risiko atau yang setara serta langkah perlindungan yang berkaitan:
  Tahap Risiko
- Tahap 1 (Perlindungan asas untuk risiko minimum dan potensi untuk keluaran sumber terbuka)
- Tahap 2 (Pemantauan masa nyata, penapisan prompt, pengesanan anomali tingkah laku, kawalan akses, red-teaming dan simulasi adversarial)
- Tahap 3 (perlindungan lanjutan termasuk red- teaming, pelancaran berfasa, pengujian adversarial, penyulitan, kawalan akses berbilang pihak dan seni bina sifar kepercayaan)
- Tahap 4 (Protokol keselamatan maksimum untuk model berisiko tinggi dan langkah sekuriti maksimum)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.5: Kerangka Keselamatan AI Barisan Hadapan
>white|black||9|11|br Set pertama Rangka Kerja Keselamatan AI Frontier yang telah diterbitkan oleh sebahagian daripada pembangun AI yang menandatangani Komitmen Keselamatan AI Frontier. Rangka kerja ini merangkumi risiko yang serupa (dengan sedikit variasi) dan menggunakan peringkat risiko serta pendekatan pengurusan risiko yang berbeza.


>white|orangered|left|14|15.5|bb Keberkesanan Kerangka Keselamatan AI Barisan Hadapan masih tidak pasti.

Rangka Kerja Keselamatan AI Barisan Hadapan boleh berfungsi sebagai alat pengurusan risiko dalam keadaan tertentu dan bagi kategori risiko tertentu yang mempunyai laluan kepada bahaya yang boleh dipercayai (‡1117). Pada masa yang sama, beberapa analisis membincangkan persoalan berkaitan kejelasan dan skopnya (‡111, ‡986), serta keteguhan ambang keupayaan dan risiko AI (‡1031, ‡1130). Rangka kerja sedia ada cenderung menumpukan pada subset domain risiko. Akibatnya, beberapa risiko utama, seperti pengawasan yang menyalahi undang-undang (‡1131, ‡1132) dan imej intim tanpa persetujuan (‡287), kurang diberi penekanan. Tidak seperti pendekatan pengurusan risiko daripada sektor lain, seperti penerbangan atau kuasa nuklear (‡1133*), Rangka Kerja Keselamatan AI Barisan Hadapan biasanya tidak menggunakan ambang risiko kuantitatif yang jelas (‡1134).

Penilaian luaran terhadap pematuhan pembangun kepada Rangka Kerja Keselamatan AI Termaju mereka setakat ini masih terhad, sebahagiannya kerana kebanyakan rangka kerja tersebut masih baharu, maklumat yang tersedia kepada umum adalah terhad, dan tiada audit luaran yang standard. Keberkesanannya juga akan dipengaruhi oleh sejauh mana – dan sebaik mana – komitmen dilaksanakan dalam amalan. Dengan sendirinya, rangka kerja ini mungkin tidak menjamin pengurusan risiko yang berkesan, kerana impak praktikalnya bergantung pada sejauh mana dan sebaik mana rangka kerja ini dilaksanakan. Setakat ini, rangka kerja tersebut belum sejajar sepenuhnya dengan piawaian pengurusan risiko antarabangsa (‡1135). Satu kajian tentang komitmen sukarela terdahulu mendapati bahawa pemenuhan langkah-langkah berbeza-beza, yang menunjukkan bahawa pematuhan terhadap komitmen sukarela mungkin berbeza-beza antara syarikat dan domain (‡1109).

Secara keseluruhannya, Rangka Kerja Keselamatan AI Termaju merupakan bentuk pengurusan risiko organisasi secara sukarela yang paling terperinci yang sedang digunakan pada masa ini, tetapi berbeza dengan ketara dari segi skop, ambang dan kebolehkuatkuasaan.

###@ Inisiatif kawal selia dan tadbir urus

>white|orangered|left|14|15.5|bb Beberapa bidang kuasa telah memperkenalkan undang-undang yang menetapkan keperluan ketelusan.

Beberapa pendekatan kawal selia awal memperkenalkan keperluan undang-undang yang bertujuan meningkatkan penyeragaman dan ketelusan dalam pengurusan risiko. Akta AI EU, yang mula berkuat kuasa pada 2024, menetapkan keperluan berkaitan ketelusan, hak cipta dan keselamatan untuk model AI tujuan umum. Pada 2025, Kod Amalan AI Tujuan Umum EU diterbitkan untuk menyokong pematuhan terhadap kewajipan ini dengan memberikan panduan tentang dokumentasi model dan hak cipta, serta – bagi model yang paling canggih – amalan pengurusan risiko seperti penilaian, pentaksiran dan mitigasi risiko, keselamatan maklumat dan pelaporan insiden serius (‡965).

Contoh lain keperluan kawal selia baharu termasuk Akta Kerangka Korea Selatan mengenai Pembangunan Kecerdasan Buatan dan Pembentukan Kepercayaan, yang memperkenalkan keperluan bagi sistem AI ‘berimpak tinggi’ dalam sektor kritikal (‡1136), serta SB 53 California, yang menetapkan keperluan ketelusan berhubung rangka kerja keselamatan dan pelaporan insiden (‡1104). Memandangkan keperluan ini baru sahaja diwujudkan, masih terlalu awal untuk menilai secara terperinci bagaimana keperluan tersebut akan mempengaruhi amalan pengurusan risiko atau hasil risiko sebenar.

>white|orangered|left|14|15.5|bb Inisiatif tadbir urus yang lebih luas menawarkan panduan sukarela

Beberapa rangka kerja tadbir urus serantau dan antara rantau kini menggariskan jangkaan bersama untuk mengurus risiko daripada AI tujuan umum dengan menyediakan panduan tidak mengikat kepada pembuat dasar dan organisasi. Rangka Kerja Tadbir Urus Keselamatan AI China 2.0, yang diterbitkan pada 2025, menyediakan panduan berstruktur tentang pengelasan risiko dan langkah balas sepanjang proses pembangunan dan pelaksanaan AI (‡1137). Negara Anggota ASEAN menerbitkan ‘Panduan Lanjutan ASEAN tentang Tadbir Urus dan Etika AI (AI Generatif)’, yang menyediakan panduan tentang tadbir urus dan etika AI tujuan umum serta bertujuan menyokong penyelarasan dasar yang lebih baik merentas Negara Anggota ASEAN (‡1138). Selain itu, inisiatif yang dipimpin oleh pakar seperti Konsensus Singapura, yang dibangunkan oleh saintis AI dari pelbagai negara, menggariskan keutamaan penyelidikan bagi keselamatan AI tujuan umum merangkumi penilaian risiko, pembangunan dan kawalan (‡690).

###@ Kemas kini

Sejak penerbitan Laporan terakhir (Januari 2025), landskap pengurusan risiko bagi AI tujuan umum telah berkembang, dengan penerbitan sumber baharu seperti Kod Amalan AI Tujuan Umum EU, Rangka Kerja Pelaporan HAIP G7, Rangka Kerja Tadbir Urus Keselamatan AI Kebangsaan China 2.0 dan pelbagai Kerangka Keselamatan AI Termaju oleh pembangun AI. Inisiatif-inisiatif ini menerangkan pendekatan dan amalan yang digunakan oleh pembangun AI untuk mengurus risiko yang berkaitan dengan sistem AI tujuan umum (‡1115). Terdapat variasi yang ketara merentas Kerangka Keselamatan AI Termaju dan laporan ketelusan HAIP (‡1103), yang mencerminkan perbezaan dalam amalan organisasi, keutamaan risiko dan peringkat awal ekosistem pengurusan risiko AI tujuan umum. Ekosistem yang dipercayai, yang membolehkan pelbagai pihak AI menyumbang amalan pengurusan risiko yang saling melengkapi sepanjang kitar hayat, boleh menyumbang kepada pengurusan risiko yang berkesan (‡690).

###@ Jurang bukti

Terdapat kekurangan bukti tentang cara mengukur tahap keterukan, kelaziman dan jangka masa risiko yang muncul; sejauh mana risiko ini boleh dikurangkan dalam konteks dunia sebenar; dan cara menggalakkan atau menguatkuasakan penggunaan langkah mitigasi secara berkesan dalam kalangan pelbagai pihak. Lebih banyak penyelidikan diperlukan untuk memahami sejauh mana pelbagai risiko ini berleluasa dan sejauh mana risikonya berbeza-beza di pelbagai rantau dunia, khususnya rantau seperti Asia, Afrika dan Amerika Latin yang sedang mengalami pendigitalan pesat. Apabila model AI diberikan autonomi dan kuasa yang semakin besar, dan pengetahuan saintifik tentang risiko AI tujuan umum terus berkembang, pendekatan pengurusan risiko juga perlu berubah (‡639, ‡1139).

Langkah mitigasi risiko tertentu semakin popular (‡690, ‡956), tetapi lebih banyak penyelidikan diperlukan untuk memahami sejauh mana langkah mitigasi risiko dan perlindungan berkesan dalam amalan bagi komuniti dan pelaku AI yang berbeza (termasuk perusahaan kecil dan sederhana). Akses yang lebih luas kepada data tentang penggunaan dan pelaksanaan model dalam kehidupan sebenar adalah penting untuk penilaian sedemikian. Selain itu, usaha pengurusan risiko pada masa ini sangat berbeza-beza dalam kalangan syarikat AI terkemuka. Terdapat hujah bahawa insentif pembangun tidak sejajar dengan penilaian dan pengurusan risiko yang menyeluruh (‡934). Masih terdapat jurang bukti tentang sejauh mana pelbagai komitmen sukarela dipenuhi, halangan yang dihadapi syarikat dalam mematuhi komitmen sepenuhnya, dan cara mereka mengintegrasikan Rangka Kerja Keselamatan AI Frontier ke dalam amalan pengurusan risiko AI yang lebih luas.

###@ Cabaran bagi pembuat dasar

Cabaran utama termasuk menentukan cara mengutamakan pelbagai risiko yang ditimbulkan oleh AI tujuan umum, menjelaskan pihak yang paling berupaya mengurangkannya, dan memahami insentif serta kekangan yang membentuk tindakan mereka. Bukti menunjukkan bahawa pembuat dasar pada masa ini mempunyai akses terhad kepada maklumat tentang cara pembangun dan pelaksana AI menguji, menilai dan memantau risiko yang baru muncul, serta tentang keberkesanan pelbagai amalan mitigasi (‡1140). Penyelidik dan pembuat dasar telah membincangkan usaha ketelusan dan pelaporan insiden yang lebih sistematik sebagai cara yang mungkin untuk memaklumkan pengutamaan risiko, memupuk kepercayaan dan memberikan insentif bagi pembangunan yang bertanggungjawab (‡957). Dalam amalan, pengurusan risiko melibatkan pelbagai pihak merentasi rantaian nilai AI – seperti penyedia data dan awan, pembangun model dan platform pengehosan model – yang masing-masing mempunyai peluang tersendiri untuk menilai dan mengurus pelbagai risiko (‡1141). Perkongsian maklumat yang terhad antara pihak-pihak ini menyukarkan penentuan risiko yang paling berkemungkinan berlaku atau memberikan impak terbesar, khususnya apabila kesan hiliran terhadap masyarakat dipertimbangkan.

