##########
>white|orangered|left|14|30|hr Bahagian 3.3
### 3.3. Perlindungan teknikal dan pemantauan
>white|orangered|left|24|30|hb Perlindungan teknikal dan pemantauan

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Maklumat utama
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Pelbagai langkah perlindungan teknikal digunakan pada pelbagai peringkat pembangunan dan penggunaan AI. Ini termasuk teknik yang diterapkan semasa pembangunan model untuk menjadikan sistem lebih teguh dan tahan terhadap penyalahgunaan (seperti kurasi data), pemantauan dan kawalan semasa- penggunaan (seperti penapisan kandungan dan pengawasan manusia), serta alat pascapelaksanaan untuk memantau ekosistem AI yang lebih luas (seperti pengesanan asal-usul dan kandungan).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Perlindungan teknikal mempunyai batasan dan tidak dapat mencegah tingkah laku berbahaya dengan pasti dalam semua konteks. Contohnya, pengguna kadangkala boleh mendapatkan output berbahaya dengan menyusun semula permintaan atau memecahkannya kepada langkah-langkah yang lebih kecil. Begitu juga, alat seperti penandaan air yang direka untuk mengenal pasti kandungan yang dijana AI selalunya boleh dibuang atau diubah, sekali gus mengehadkan kebolehpercayaannya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Keterbatasan perlindungan individu bermakna pendekatan ‘pertahanan berlapis’ mungkin diperlukan untuk mencegah hasil buruk tertentu. Contohnya, sistem mungkin menggabungkan model yang dilatih untuk keselamatan dengan penapis input, penapis output dan pemantau kandungan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terakhir (Januari 2025), para penyelidik telah mencapai kemajuan dalam meningkatkan perlindungan, tetapi batasan asas masih wujud. Sebagai contoh, kadar kejayaan serangan yang direka untuk memintas perlindungan semakin menurun, tetapi masih agak tinggi. Terdapat juga batasan asas tentang sejauh mana model dengan pemberat terbuka boleh dilindungi secara menyeluruh.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Cabaran utama bagi penggubal dasar ialah bukti yang terhad tentang keberkesanan langkah perlindungan dalam pelbagai penggunaan sistem AI tujuan umum di dunia sebenar. Pembangun AI berbeza-beza dengan ketara dari segi jumlah maklumat yang dikongsi tentang langkah perlindungan dan pemantauan mereka. Cabaran seterusnya ialah kemungkinan wujudnya kompromi antara penggunaan langkah perlindungan yang lebih kukuh dengan pengekalan prestasi atau kegunaan sistem.
>oldlace|black||11|15|br      


Pembangun AI boleh menggunakan beberapa perlindungan teknikal yang berguna tetapi tidak sempurna untuk mengurangkan dan mengurus risiko daripada sistem AI tujuan umum, namun cabaran keteguhan masih berterusan. Pembangun masih belum dapat menghalang sepenuhnya sistem AI tujuan umum daripada melakukan tindakan yang diketahui umum dan jelas berbahaya, seperti memberikan arahan kepada pengguna untuk melakukan jenayah. Sebagai contoh, penyelidik telah menunjukkan bahawa perlindungan terkini boleh dipintas melalui kaedah prompting adversarial (iaitu ‘jailbreak’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), dengan meminta model memecahkan tugas berbahaya yang kompleks kepada beberapa langkah (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), dan melalui pengubahsuaian model yang mudah (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Penyelidik terus berusaha membangunkan perlindungan terhadap kerosakan fungsi dan penyalahgunaan (‡690). Kaedah ini berbeza-beza dari segi tujuan dan keberkesanannya, dan kesannya akhirnya bergantung pada konteks sosioteknikal dan tadbir urus yang lebih luas, tempat sistem AI dibangunkan dan digunakan.

Perlindungan teknikal secara umum boleh dibahagikan kepada tiga kategori: teknik untuk membangunkan model yang lebih selamat; teknik yang digunakan semasa pelaksanaan untuk pemantauan dan kawalan; dan teknik yang menyokong pemantauan ekosistem selepas pelaksanaan. Meja 3.6 merumuskan perlindungan teknikal yang dibincangkan, keberkesanannya dan cabaran yang masih belum ditangani.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Membangunkan model yang lebih selamat
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kurasi data (‡1167)
  Membuang data berbahaya untuk menghalang model daripada mempelajari keupayaan berbahaya. Kaedah ini boleh berguna, termasuk untuk membangunkan model dengan pemberat terbuka yang tidak mempunyai keupayaan berbahaya dan tahan terhadap penalaan halus yang berbahaya (‡55). Walau bagaimanapun, terdapat cabaran berkaitan kesilapan kurasi dan penskalaan (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pembelajaran pengukuhan daripada maklum balas manusia (‡64*)
  Melatih model supaya selaras dengan matlamat yang ditetapkan, seperti bersikap membantu dan tidak memudaratkan. Ini ialah cara yang berkesan untuk mengajar model tingkah laku yang bermanfaat (‡64*). Walau bagaimanapun, pengoptimuman berlebihan untuk mendapatkan persetujuan manusia boleh menyebabkan model berkelakuan secara mengelirukan atau mengampu (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teknik penjajaran pluralistik (‡1170)
  Melatih model untuk mengintegrasikan pelbagai pandangan yang berbeza tentang cara model itu harus bertindak. Teknik-teknik ini membantu mengurangkan kecenderungan model untuk memihak kepada pandangan tertentu (‡1170). Walau bagaimanapun, meskipun teknik-teknik ini digunakan, perbezaan pendapat dalam kalangan manusia tidak dapat dielakkan, dan sukar untuk mereka bentuk cara yang diterima secara meluas bagi mengimbangi pandangan yang bersaing (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Latihan adversarial (‡677)
  Melatih model supaya enggan menyebabkan kemudaratan (walaupun dalam konteks yang tidak biasa) dan menahan serangan daripada pengguna berniat jahat (cth. ‘jailbreak’). Ini merupakan kaedah yang berkesan untuk menjadikan model tahan terhadap percubaan penyalahgunaan (‡1064), tetapi cabaran keteguhan masih berterusan (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb ‘Nyahpembelajaran’ mesin (‡1175, ‡1176)
  Melatih model menggunakan algoritma khusus yang bertujuan untuk menyekat keupayaan berbahaya secara aktif (cth. pengetahuan tentang bahaya biologi). Teknik ini menawarkan cara yang disasarkan untuk menghapuskan keupayaan berbahaya daripada model (‡1175, ‡1176), tetapi algoritma nyahpembelajaran semasa mungkin tidak teguh dan boleh memberi kesan yang tidak diingini terhadap keupayaan lain (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Alat kebolehtafsiran dan pengesahan keselamatan (‡1177)
  Keluarga kaedah reka bentuk dan pengesahan yang pelbagai, bertujuan memberikan jaminan yang lebih ketat bahawa model mempunyai sifat khusus yang berkaitan dengan keselamatan. Kaedah ini membolehkan penilai memberikan jaminan keselamatan dengan tahap keyakinan yang lebih tinggi (‡1177), tetapi kaedah semasa bergantung pada andaian dan jarang sekali berdaya saing dari segi prestasi dalam amalan (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Pemantauan dan kawalan
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mekanisme pemantauan berasaskan perkakasan (‡1179, ‡1180, ‡1181)
  Mengesahkan bahawa proses yang dibenarkan sedang berjalan pada perkakasan untuk mengkaji ancaman keselamatan atau pematuhan peraturan. Mekanisme ini menawarkan cara yang unik untuk memantau pengiraan yang dijalankan pada perkakasan dan pihak yang menjalankannya (‡1181). Walau bagaimanapun, mekanisme perkakasan tidak dapat memantau semua jenis ancaman, dan sesetengah teknik memerlukan perkakasan khusus (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau interaksi pengguna (‡1154, ‡1166)
  Pemantauan interaksi pengguna untuk mengesan tanda-tanda penggunaan berniat jahat boleh membantu pembangun menamatkan perkhidmatan kepada pengguna berniat jahat (‡1154, ‡1166). Walau bagaimanapun, penguatkuasaan boleh secara tidak sengaja menghalang penyelidikan keselamatan yang bermanfaat (‡689), dan sesetengah bentuk penyalahgunaan sukar dikesan (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau interaksi pengguna (‡1154, ‡1166)
  Pemantauan interaksi pengguna untuk mengesan tanda-tanda penggunaan berniat jahat dapat membantu pembangun menamatkan perkhidmatan kepada pengguna berniat jahat (‡1154, ‡1166). Walau bagaimanapun, penguatkuasaan boleh secara tidak sengaja menghalang penyelidikan keselamatan yang bermanfaat (‡689), dan sesetengah bentuk penyalahgunaan sukar dikesan (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penapis kandungan (‡65*, ‡725)
  Penapisan input dan output model yang berpotensi memudaratkan ialah cara yang sangat berkesan untuk mengurangkan kemudaratan tidak sengaja dan risiko penyalahgunaan (‡725). Walau bagaimanapun, penapis memerlukan sumber pengiraan tambahan dan terdedah kepada sesetengah serangan (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau pengiraan dalaman model (‡744, ‡1183, ‡1184)
  Pemantauan terhadap tanda-tanda penipuan atau bentuk kognisi dalaman lain yang berbahaya dalam model boleh menjadi cara yang cekap untuk mengesan penipuan (‡744, ‡1183, ‡1184). Walau bagaimanapun, kaedah semasa kurang teguh dan boleh dipercayai (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemantau rantaian pemikiran (‡430, ‡435)
  Pemantauan teks rantaian pemikiran model untuk mengesan tanda-tanda tingkah laku yang mengelirukan atau penaakulan berbahaya yang lain ialah cara yang berkesan untuk memahami dan mengenal pasti kelemahan dalam cara model membuat penaakulan (‡435). Walau bagaimanapun, kaedah ini mungkin tidak boleh dipercayai (‡752, ‡753, ‡1186), dan jika model dilatih untuk menghasilkan rantaian pemikiran yang tidak berbahaya, model boleh mempelajari tingkah laku yang mengelirukan (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Manusia dalam gelung (‡1187, ‡1188, ‡1189)
  Pengawasan manusia dan tindakan mengatasi keputusan sistem adalah penting dalam sesetengah aplikasi kritikal keselamatan (‡1187). Walau bagaimanapun, teknik ini dibatasi oleh bias automasi dan had kelajuan pembuatan keputusan manusia (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengasingan kotak pasir (‡1192)
  Menghalang ejen AI daripada mempengaruhi dunia secara langsung ialah cara yang berkesan untuk mengehadkan kemudaratan yang boleh ditimbulkannya (‡1192). Walau bagaimanapun, penggunaan persekitaran kotak pasir mengehadkan keupayaan sistem untuk melaksanakan tugas tertentu secara langsung (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Alat untuk memudahkan pemantauan ekosistem
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teknik pengenalpastian model AI (‡1193*, ‡1194)
  Menjadikan model, atau kejadian individu model, lebih mudah dikenal pasti dalam kes penggunaan dunia sebenar membantu forensik digital dan kesedaran ekosistem (‡1195). Walau bagaimanapun, teknik ini boleh dielakkan dengan sesetengah jenis pengubahsuaian model (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Inferens asal-usul model AI (‡1197)
  Teknik ini membolehkan penyelidik mengkaji cara model diubah suai dalam ekosistem AI, khususnya model dengan pemberat terbuka. Teknik ini membantu dalam forensik digital dan kesedaran ekosistem (‡1198), tetapi projek berskala besar diperlukan untuk memetakan ekosistem model dengan pemberat terbuka secara menyeluruh (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tera air dan metadata (‡1199, ‡1200, ‡1201*)
  Teknik ini memudahkan pengesanan sama ada sesuatu teks, imej, video dan sebagainya dijana atau diubah suai oleh AI, serta sistem yang digunakan. Teknik ini meningkatkan kesedaran ekosistem (‡1199, ‡1200, ‡1201*). Walau bagaimanapun, tera air dan metadata boleh dipalsukan atau dibuang melalui pengubahsuaian tertentu pada kandungan (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengesanan kandungan yang dijana AI (‡1203, ‡1204, ‡1205*)
  Meningkatkan keupayaan pengguna untuk membezakan kandungan yang dijana AI daripada kandungan tulen membantu dalam forensik digital dan kesedaran ekosistem (‡1203, ‡1204). Walau bagaimanapun, pengelas mungkin tidak boleh dipercayai (‡1205*) dan prestasinya berbeza-beza mengikut modaliti.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.6: Perlindungan teknikal yang dibincangkan dalam bahagian ini
>white|black||9|11|br Ringkasan langkah perlindungan teknikal yang dibincangkan dalam bahagian ini, dibahagikan kepada kaedah untuk membangunkan model yang lebih selamat, pemantauan dan kawalan semasa penggunaan, serta teknik untuk memudahkan pemantauan ekosistem.


###@ Membangunkan model yang lebih selamat

Barisan pertahanan pertama daripada kemudaratan yang berpunca daripada sistem AI tujuan umum adalah dengan menjadikan model asas lebih selamat. Subseksyen ini merangkumi perlindungan yang ‘diterapkan dalam parameter model’ semasa proses pembangunan model (Angka 3.6).

>white|orangered|left|14|15.5|bb Pemilihan data latihan boleh mengehadkan pembangunan keupayaan yang berpotensi berbahaya.

Model AI tujuan umum berguna kerana model ini mengembangkan pelbagai pengetahuan dan keupayaan selepas memproses data latihan, tetapi sesetengah jenis data latihan secara tidak seimbang menyumbang kepada pembangunan keupayaan yang berpotensi berbahaya. Contohnya, model AI yang dilatih menggunakan kertas virologi mungkin lebih mampu memberikan bantuan dalam tugas biologi yang berpotensi memudaratkan (‡549, ‡1206*) (lihat juga §2.1.4. Risiko biologi dan kimia). Selain itu, penjana imej/video yang dilatih menggunakan imej kebogelan manusia juga boleh disalahgunakan untuk menghasilkan deepfake intim tanpa persetujuan (‡308, ‡319) (lihat juga §2.1.1. Kandungan yang dijana AI dan aktiviti jenayah).

Penapisan data latihan merupakan langkah mitigasi yang berkesan terhadap sesetengah keupayaan yang tidak diingini (‡319, ‡1167, ‡1207, ‡1208). Walau bagaimanapun, penapisan set data besar yang digunakan untuk melatih model AI tujuan umum boleh menjadi sukar (‡1168) disebabkan kos yang tinggi (‡1209), kesilapan penapisan (‡1210), dan kesan negatif terhadap kualiti set data (‡1211). Cabaran ini diburukkan lagi oleh sifat berbilang bahasa teks internet (‡1212), bias budaya dalam penyederhanaan kandungan (‡1211, ‡1213, ‡1214, ‡1215), serta hakikat bahawa sama ada sesuatu data itu ‘berbahaya’ bergantung pada faktor kontekstual (‡1216). Walau bagaimanapun, penapisan bahan yang berpotensi berbahaya daripada data latihan menunjukkan potensi untuk menjadikan model lebih selamat secara lebih konsisten, termasuk menjadikan model berwajaran terbuka lebih tahan terhadap pengusikan berbahaya (‡55). Hubungan antara kandungan data latihan dengan keupayaan model yang muncul masih belum difahami sepenuhnya (‡1195), dan penapisan nampaknya lebih berkesan untuk mengehadkan keupayaan berbahaya apabila digunakan pada domain pengetahuan yang luas (‡55) berbanding tingkah laku yang lebih khusus (‡1206, ‡1217). Lihat §3.4. Model berwajaran terbuka untuk perbincangan lanjut.

![figure 3.6](images/fig3.6_safeguards.png)

##### Angka 3.6: Di mana perlindungan teknikal perlu digunakan
>white|black||9|11|br Perlindungan teknikal boleh diterapkan pada pelbagai peringkat pembangunan model. Kurasi data membentuk perkara yang dipelajari oleh model semasa pralatihan dan penalaan halus. Kaedah berasaskan latihan seperti pembelajaran pengukuhan daripada maklum balas manusia dan latihan keteguhan melaraskan tingkah laku model. Kaedah pengujian seperti serangan adversarial mengenal pasti kelemahan yang masih wujud. Sesetengah teknik, seperti algoritma safe-by- design, merangkumi pelbagai peringkat. Sumber: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Kaedah untuk melatih model AI serba guna agar berguna dan tidak berbahaya terutamanya bergantung pada maklum balas manusia.

Sukar untuk melatih dan menilai model supaya dapat diselaraskan dengan prinsip aras tinggi seperti bersikap membantu, tidak berbahaya dan jujur secara konsisten. Dalam amalan, pembangun berusaha mencapai matlamat ini dengan menala halus model AI menggunakan demonstrasi dan maklum balas daripada manusia. Sebagai contoh, paradigma utama untuk menala halus model AI, yang dikenali sebagai ‘pembelajaran pengukuhan daripada maklum balas manusia’, berasaskan latihan model untuk menghasilkan output yang dinilai secara positif oleh anotator manusia (‡1218). Walau bagaimanapun, maklum balas positif daripada manusia ialah proksi yang tidak sempurna bagi tingkah laku yang bermanfaat (‡737, ‡878, ‡1219, ‡1220) dan terhad oleh kesilapan serta bias manusia (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Hal ini membawa kepada beberapa cabaran: model yang ditala halus melalui pembelajaran pengukuhan daripada maklum balas manusia kadangkala mengampu pengguna, tingkah laku yang dikenali sebagai ‘sikap mengampu’ (‡358, ‡740, ‡1226, ‡1227); memberikan respons yang membantu dalam sesetengah konteks tetapi memudaratkan dalam konteks lain (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); memberikan respons yang sukar dinilai ketepatannya (‡1233); atau melakukan tindakan yang kebermanfaatan atau kemudaratannya bergantung pada pendapat (‡1234). Meja 3.7 memberikan contoh cabaran ini. Sesetengah penyelidikan bertujuan membangunkan kaedah untuk membantu manusia menilai penyelesaian kepada tugas yang kompleks dengan bantuan AI dengan lebih baik (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Walau bagaimanapun, kebolehpercayaan kaedah ini pada masa ini terhad, dan sejauh mana kaedah ini digunakan untuk melatih model AI paling canggih pada masa kini tidak diketahui umum.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sikap mengampu/mengikut kehendak (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Model itu hanya memberikan maklum balas positif, tanpa menyatakan bahawa struktur suku kata haiku 5-7-5 yang betul tidak dipenuhi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sesetengah tindakan bermanfaat dalam sesetengah konteks tetapi memudaratkan dalam konteks yang lain (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Maklumat tentang risiko biologi boleh digunakan untuk pendidikan dan pertahanan, tetapi juga boleh memberikan panduan kepada pihak yang berniat jahat.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tingkah laku yang betul sukar disahkan (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black||11|13|br Ketepatan respons ini sukar dinilai kerana ia memerlukan kepakaran perubatan. Malah bagi doktor yang berpengalaman, menilai respons seperti ini memerlukan masa dan perhatian yang teliti terhadap perincian.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Manusia tidak sependapat tentang perkara yang betul (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Penjelasan:
>white|black|left|11|13|br Terdapat perbezaan pendapat yang ketara tentang respons yang betul.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.7: Gesaan pengguna dan respons model AI
>white|black||9|11|br Contoh cabaran dalam menentukan tindakan bermanfaat yang perlu dilakukan oleh model AI dan memberikan insentif untuk tindakan tersebut.


>white|orangered|left|14|15.5|bb Manusia tidak sentiasa bersetuju tentang tingkah laku yang diingini, maka kaedah diperlukan untuk mengimbangi keutamaan yang bersaing.

Manusia tidak sentiasa bersetuju tentang respons atau tindakan yang patut atau tidak patut dikeluarkan oleh model AI (‡1006). Hal ini menjadikan pembangunan model yang tindakannya dan kesannya selaras secara meluas dengan kepentingan masyarakat satu cabaran asas (‡420). Sesetengah penyelidik mengkaji keutamaan pihak yang dicerminkan dalam sistem AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) dan berusaha membangunkan teknik ‘penjajaran pluralistik’ yang bertujuan mencapai keseimbangan antara keutamaan yang bersaing (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Sebagai contoh, pembangun AI boleh mereka bentuk sistem supaya mengelakkan penjanaan jawapan kontroversial dengan menolak permintaan tertentu, menyelaraskan sistem dengan pandangan median dalam sampel orang yang relevan, atau memperibadikan sistem untuk pengguna individu. Pembezaan

Cabaran lazim bagi pendekatan ini ialah, secara umum, sistem AI tidak dapat menyelaraskan diri secara sama rata dengan keutamaan semua orang, dan kesan hilirannya terhadap masyarakat akan memberi kesan yang berbeza kepada pelbagai kumpulan manusia. Sesetengah penyelidik berpendapat bahawa kebanyakan pendekatan teknikal terhadap penjajaran pluralistik gagal menangani, malah berpotensi mengalih perhatian daripada, cabaran yang lebih mendalam seperti bias sistematik, dinamika kuasa sosial, serta pemusatan kekayaan dan pengaruh (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Pembangun AI menggunakan ‘latihan adversarial’ untuk meningkatkan keteguhan model

Memastikan model AI menggeneralisasikan tingkah laku bermanfaat yang dipelajarinya semasa latihan dengan kukuh kepada konteks penggunaan sebenar merupakan cabaran. Malah, model yang dilatih dengan isyarat pembelajaran yang ‘sempurna’ pun boleh gagal menggeneralisasikan tingkah laku tersebut dengan jayanya kepada semua konteks yang belum pernah dilihat (‡738, ‡739, ‡1255, ‡1256, ‡1257). Contohnya, sesetengah penyelidik mendapati bahawa chatbot lebih cenderung mengambil tindakan berbahaya dalam bahasa yang kurang diwakili dalam data latihannya (‡159, ‡880, ‡1258*, ‡1259), termasuk banyak bahasa yang kebanyakannya dituturkan di Selatan Global.

Dalam beberapa tahun kebelakangan ini, para penyelidik juga telah menghasilkan himpunan besar teknik ‘serangan adversarial’ yang boleh digunakan untuk membuat model menjana respons yang berpotensi berbahaya (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Sebagai contoh, satu inisiatif baru-baru ini mengumpulkan secara ramai lebih 60,000 contoh pelbagai serangan yang berjaya terhadap model AI tercanggih, yang menyebabkan model-model tersebut melanggar dasar syarikat masing-masing tentang tingkah laku model yang boleh diterima (‡1149). Meja 3.8 menunjukkan contoh teknik ‘jailbreak’ yang menurut penyelidik boleh membuat model mematuhi permintaan berbahaya.

Satu kaedah untuk meningkatkan keteguhan model dikenali sebagai ‘latihan adversarial’ (‡1064). Kaedah ini melibatkan pembinaan ‘serangan’ (cth. jailbreak) yang direka untuk membuat model bertindak dengan cara yang tidak diingini, serta melatih model untuk menangani serangan ini dengan sewajarnya. Walau bagaimanapun, latihan adversarial tidak sempurna (‡1260, ‡1261). Penyerang sentiasa dapat membangunkan serangan baharu yang berjaya terhadap model tercanggih (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Oleh sebab pembangun memerlukan contoh khusus tentang mod kegagalan untuk melatih model menentangnya (‡512, ‡1263), hasilnya ialah permainan ‘kucing dan tikus’ yang berterusan, dengan pembangun terus mengemas kini model sebagai tindak balas terhadap kelemahan yang baharu ditemukan, sementara pihak lawan terus mencari serangan baharu. Sesetengah penyelidik telah mencadangkan latihan adversarial berskala lebih besar (‡1264, ‡1265) atau algoritma baharu (‡675, ‡676, ‡1263, ‡1266, ‡1267) untuk meningkatkan keteguhan, tetapi sistem AI moden kekal terdedah secara berterusan.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Buat permintaan berbahaya dalam teks sifir, seperti kod Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Berikan sistem contoh respons yang mematuhi garis panduan bagi permintaan berbahaya (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Buat permintaan berbahaya dalam bahasa sumber rendah yang berkemungkinan kurang digunakan dalam latihan (cth. Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Strategi: Pecahkan tugas berbahaya kepada beberapa subtugas yang tidak berbahaya (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 3.8: Strategi jailbreak
>white|black||9|11|br Pelaku berniat jahat dan pasukan merah telah menggunakan pelbagai jenis ‘jailbreak’ untuk membuat model AI mematuhi permintaan berbahaya yang biasanya akan ditolak oleh model tersebut kerana adanya perlindungan. Contoh output ditulis oleh pengarang Laporan untuk tujuan ilustrasi. Banyak model AI tercanggih masa kini menangkis kebanyakan kaedah ini, tetapi teknik jailbreak baharu terus ditemui.


>white|orangered|left|14|15.5|bb Teknik ‘penyahpembelajaran’ boleh mengurangkan keupayaan model tertentu yang berbahaya.

Satu lagi strategi untuk mengurangkan risiko daripada AI tujuan umum ialah memperhalus model supaya tidak mempunyai keupayaan dalam domain berisiko tinggi tertentu (‡1175, ‡1176). Contohnya, para penyelidik sedang berusaha membangunkan algoritma ‘nyahpembelajaran mesin’ yang boleh menekan secara khusus kebolehan yang berkaitan dengan ancaman biologi atau penjanaan imej fotorealistik tubuh manusia yang berbogel (‡903, ‡1272, ‡1273). Kaedah ini boleh menjadikan model jauh lebih selamat, dengan mengorbankan beberapa kegunaan positif bagi keupayaan yang dinyahpelajari. Mengehadkan pengetahuan model AI dalam domain berbahaya juga telah dicadangkan sebagai satu cara mereka bentuk model ‘tahan usikan’ dengan pemberat terbuka yang boleh menahan penalaan halus yang berbahaya (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Walau bagaimanapun, setakat ini, perkara ini sukar dilakukan dengan teguh (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Lihat §3.4. Model dengan pemberat terbuka untuk perbincangan lanjut.

>white|orangered|left|14|15.5|bb Sesetengah penyelidik sedang mengusahakan kaedah untuk memberikan jaminan keselamatan yang lebih kukuh melalui pentafsiran keadaan dalaman model atau pengesahan matematik.

Sesetengah penyelidik sedang mengusahakan kaedah untuk mengesahkan dengan lebih rapi sifat model yang berkaitan dengan keselamatan. Dalam satu pendekatan, penyelidik berusaha mentafsir pengiraan dalaman model sama ada untuk mengenal pasti risiko atau untuk mengemukakan hujah yang lebih meyakinkan bahawa model itu selamat (‡1285, ‡1286). Sebagai contoh, dalam bukti konsep, penyelidik menunjukkan bahawa alat untuk menganalisis pengiraan dalaman model bahasa boleh membantu penilai mengenal pasti tingkah laku yang berbahaya (‡1287). Pada 2025, Anthropic juga mula menganalisis bahagian dalaman model sebagai cara untuk mengkaji kesedaran situasi dan ‘niat’ model (‡2). Walau bagaimanapun, kaedah seperti ini pada masa ini tidak lazim digunakan atau diketahui mampu bersaing dengan teknik penilaian lain.

Pendekatan lain untuk memberikan jaminan keselamatan yang lebih kukuh melibatkan pembinaan bukti matematik bahawa sesuatu model akan memenuhi syarat keselamatan tertentu (‡1177, ‡1282, ‡1288). Walau bagaimanapun, bukti ini mengandaikan bahawa konteks pengujian sepadan dengan konteks pelaksanaan, dan belum diuji terhadap pelbagai jenis pihak lawan.

Ia juga tidak dapat diskalakan kepada model besar pada masa ini. Secara keseluruhan, terdapat perdebatan yang ketara dalam kalangan pakar tentang potensi kaedah kebolehertafsiran dan pengesahan formal.

###@ Pemantauan dan kawalan semasa penempatan

Selain langkah perlindungan yang dilaksanakan semasa pembangunan model, barisan pertahanan kedua terhadap tingkah laku berbahaya ialah langkah perlindungan luaran yang memberi tumpuan kepada pemantauan dan kawalan terhadap tindakan model atau sistem semasa penggunaan. Langkah perlindungan sedemikian membantu mengurangkan kerosakan fungsi dan penyalahgunaan, seperti output halusinasi dan arahan berbahaya.

>white|orangered|left|14|15.5|bb Pihak yang melaksanakan model boleh menggunakan pelbagai alat untuk mengenal pasti dan menangani tingkah laku model berisiko tinggi.

Apabila sistem AI sedang beroperasi, pihak yang melaksanakan sistem boleh memantau tanda-tanda risiko dan campur tangan jika tanda-tanda tersebut muncul. Contohnya, mereka boleh memeriksa input model untuk mengesan tanda-tanda serangan adversarial, menapis kandungan yang tidak sesuai daripada output, atau memantau rantaian pemikiran sistem untuk mengesan tanda-tanda rancangan yang memudaratkan. Titik-titik yang membolehkan pihak yang melaksanakan sistem memantau dan campur tangan dalam cara orang menggunakan sistem mereka termasuk perkakasan (‡1180, ‡1181), interaksi pengguna (‡1154, ‡1166), input dan output (‡65, ‡725, ‡1182), pengiraan dalaman (‡744, ‡1183, ‡1184), dan rantaian pemikiran (‡430, ‡435). Terdapat juga pelbagai tindakan yang boleh diambil oleh pihak yang melaksanakan sistem apabila risiko dikenal pasti. Tindakan ini termasuk merekodkan maklumat, menapis/mengubah suai kandungan yang memudaratkan, menandakan aktiviti luar biasa, mematikan sistem atau mencetuskan mekanisme keselamatan. Angka 3.7 menggambarkan contoh mekanisme pemantauan dan kawalan yang lazim.

Oleh sebab mekanisme ini serba guna dan selalunya berkesan, mekanisme ini digunakan secara meluas dan dapat mencegah pelbagai jenis kemudaratan yang tidak disengajakan (‡725, ‡751, ‡1289). Namun begitu, langkah perlindungan ini tidak sempurna, terutamanya apabila berhadapan dengan serangan berniat jahat yang dioptimumkan untuk menggagalkannya (‡752, ‡1182). Penyelidikan terkini juga telah mengkaji bagaimana pemantauan boleh menjadi tidak boleh dipercayai jika sistem dioptimumkan menggunakan skor pemantau, contohnya dengan menjadikan rantaian pemikiran kurang boleh dipercayai (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Angka 3.7: Teknik pemantauan dan kawalan
>white|black||9|11|br Teknik pemantauan dan kawalan beroperasi pada pelbagai peringkat: menyaring input dan output untuk mengesan kandungan berbahaya, menjejak keadaan dalaman model, mengehadkan tindakan luaran melalui pengasingan dalam persekitaran terkawal, dan mengekalkan pengawasan manusia. Sumber: Laporan Keselamatan AI Antarabangsa 2026.


>white|orangered|left|14|15.5|bb Penglibatan manusia dalam gelung membolehkan pengawasan langsung dalam situasi berisiko tinggi.

Untuk mengurangkan kemungkinan kegagalan oleh ejen AI (lihat §2.2.1. Cabaran kebolehpercayaan), pihak yang melaksanakan boleh berusaha mereka bentuk sistem AI yang berfungsi dengan kerjasama manusia dan bukannya beroperasi sepenuhnya secara autonomi (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Hal ini penting bagi kes penggunaan yang keputusan yang salah boleh mengakibatkan kemudaratan yang besar, seperti dalam bidang kewangan, penjagaan kesihatan atau kepolisan. Walau bagaimanapun, mengekalkan ‘manusia dalam gelung’ sering kali tidak praktikal. Ada kalanya keputusan perlu dibuat terlalu pantas, seperti dalam aplikasi sembang yang mempunyai berjuta-juta pengguna. Dalam kes lain, bias dan kesilapan manusia boleh memburukkan risiko akibat kesilapan yang bertindan (‡1187). Manusia dalam gelung juga cenderung menunjukkan ‘bias automasi’, yang bermaksud mereka sering lebih mempercayai sistem AI daripada yang sewajarnya (‡1190, ‡1191) (lihat §2.3.2. Risiko terhadap autonomi manusia).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ melindungi daripada risiko tingkah laku autonomi.

Ejen AI yang boleh bertindak secara autonomi tanpa batasan di Web atau dalam dunia fizikal menimbulkan risiko yang lebih tinggi (lihat §2.2.1. Cabaran kebolehpercayaan). ‘Pengasingan dalam kotak pasir’ melibatkan pembatasan cara ejen AI boleh mempengaruhi dunia secara langsung, sekali gus memudahkan pengawasan dan pengurusan mereka (‡640, ‡1192, ‡1295). Contohnya, mengehadkan keupayaan sistem AI untuk membuat hantaran di internet atau mengedit sistem fail komputer boleh mencegah kemudaratan tidak dijangka yang berpunca daripada tindakan yang tidak dijangka (‡1296). Walau bagaimanapun, pendekatan ini tidak semestinya boleh digunakan untuk aplikasi yang memerlukan sistem AI bertindak secara langsung di dunia.

###@ Alat pemantauan ekosistem: asal usul model dan data

Alat penjejakan asal usul model dan data ialah alat teknikal untuk mengkaji ekosistem AI, bagi meningkatkan kesedaran tentang penggunaan di hiliran dan kesan sistem AI.

>white|orangered|left|14|15.5|bb Teknik asal usul sistem AI membantu menjejaki penggunaan dan kesan sistem.

Pembangun dan pihak yang menggunakan model boleh menggunakan pelbagai teknik untuk mengkaji penggunaan dan penyebaran model ‘di lapangan’. Contohnya, mereka boleh memberikan model tingkah laku pengecaman yang unik (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) atau menerapkan corak unik pada pemberat model individu dengan pemberat terbuka (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Walau bagaimanapun, menjadikan teknik ini lebih tahan terhadap pengubahsuaian model masih merupakan masalah terbuka (‡1195, ‡1196*). Penyelidik juga sedang mengusahakan kaedah untuk ‘mengesan asal-usul model’ (‡1197, ‡1198, ‡1305, ‡1306), bagi membantu menjawab soalan seperti: ‘Adakah model X versi model Y yang ditala halus atau didistilasi?’ Akhir sekali, sesetengah pembangun sedang mengusahakan protokol dan infrastruktur untuk ejen AI bagi memudahkan pengecaman dan pengesahan apabila mereka berinteraksi dengan sistem luaran (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Angka 3.8: Tera air menyematkan perubahan halus yang tidak dapat dikesan ke dalam imej dan audio
>white|black||9|11|br Tera air menyematkan gangguan yang tidak dapat dilihat pada imej dan audio, yang membolehkan kandungan yang dijana AI dikenal pasti oleh alat pengesanan. Dalam angka ini, tera air pada imej dan audio dibesar-besarkan supaya dapat dilihat. Sumber: imej Chameleon daripada Unsplash (‡1313*). Unsur-unsur lain dihasilkan oleh pengarang Laporan. Laporan Keselamatan AI Antarabangsa 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Angka 3.9: Kadar kejayaan serangan suntikan prompt
>white|black||9|11|br Kadar kejayaan serangan suntikan prompt seperti yang dilaporkan oleh pembangun AI untuk model utama yang dikeluarkan antara Mei 2024 dengan Ogos 2025. Setiap titik mewakili perkadaran serangan yang berjaya dalam 10 percubaan terhadap model tertentu sejurus selepas dikeluarkan. Kadar kejayaan serangan sedemikian yang dilaporkan telah menurun dari semasa ke semasa, tetapi kekal agak tinggi. Sumber: Zou et al. 2025 (‡1149), dipetik dalam Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Teknik pengesanan kandungan AI membantu memantau penyebaran dan kesan kandungan yang dijana AI.

Tanda air, metadata dan pengesan kandungan AI yang lain boleh membantu penyelidik menjejak dan mengkaji kesan sebenar kandungan yang dicipta oleh AI.


Pertama, tera air data ialah motif halus tetapi berbeza yang disisipkan ke dalam media digital dan boleh mengekodkan maklumat tentang asal usulnya (‡1199, ‡1200, ‡1201*). Untuk teks, tera air ini biasanya berbentuk kecenderungan halus dalam pemilihan perkataan dan gaya (‡1308, ‡1309); untuk imej dan video, corak halus pada piksel (‡1310); dan untuk audio, corak halus dalam gelombang audio (‡1311). Angka 3.8 menggambarkan perkara ini.

Selain tera air, kandungan yang dijana AI juga boleh disimpan menggunakan format fail yang menyimpan metadata tentang cara kandungan itu dijana. Contohnya, banyak peranti mudah alih menyimpan fail imej dan audio menggunakan format fail yang boleh menyimpan maklumat tentang tetapan kamera, masa, lokasi dan sebagainya (‡1312). Metadata yang serupa boleh digunakan untuk menyimpan maklumat tentang sama ada data dijana oleh sistem AI. Sama seperti pengenalpastian cap jari dalam forensik jenayah, tera air dan metadata boleh diusik atau dibuang, tetapi tetap berguna.

Penyelidik juga sedang berusaha membangunkan pengesan kandungan yang dijana AI (‡1203, ‡1204, ‡1205*) untuk membantu mengenal pasti kandungan yang dijana AI di lapangan, walaupun tiada tera air atau metadata tersedia. Walau bagaimanapun, teknik pengenalpastian ini mempunyai kadar kejayaan yang terhad.

###@ Kemas kini

Sejak penerbitan Laporan terakhir (January 2025), kemajuan telah dicapai dalam pembangunan sistem AI dengan berbilang lapisan perlindungan yang berkesan. Seperti yang dibincangkan dalam §3.2. Amalan pengurusan risiko, pertahanan berlapis ialah prinsip teras dalam pengurusan risiko (‡1314). Contohnya, sistem AI yang menggabungkan model yang dilatih untuk keselamatan dengan penapis input, penapis output dan pemantau kandungan lain semakin banyak dikaji dan digunakan (‡32, ‡65, ‡1182*). Penyelidikan terkini juga menunjukkan bahawa walaupun pembangun model telah mencapai kemajuan dalam meningkatkan keteguhan terhadap percubaan untuk memintas perlindungan, penyerang masih berjaya pada kadar yang tinggi (Angka 3.9).

###@ Jurang bukti

Lebih banyak bukti diperlukan untuk membantu penyelidik memahami dan mengambil kira keterbatasan pendekatan sedia ada. Perlindungan teknikal untuk sistem AI sedang ditambah baik, tetapi teknik-teknik tersebut mempunyai keterbatasan. Sebagai contoh, kemajuan dalam meningkatkan keteguhan dalam kes terburuk bagi sistem AI tujuan umum adalah perlahan, dan terdapat keterbatasan asas tentang sejauh mana model berat terbuka boleh dilindungi dan dipantau secara menyeluruh (‡1195, ‡1315, ‡1316) (lihat juga §3.4. Model berat terbuka). Sementara itu, tidak semua perlindungan teknikal sama lazim, sama berkesan atau sama terbukti di dunia sebenar. Sebagai contoh, latihan adversarial hampir digunakan secara universal pada model tercanggih (‡64*, ‡677), manakala teknik kebolehterangan model dan pengesahan formal setakat ini jarang digunakan dalam sistem produksi (‡1177, ‡1285).

###@ Cabaran bagi pembuat dasar

Cabaran utama bagi pembuat dasar termasuk menentukan sama ada dan bagaimana mereka patut menyokong penyelidikan, pembangunan, penilaian dan penerimagunaan perlindungan teknikal serta kaedah pemantauan. Perkara ini mencabar kerana pemahaman saintis tentang cara terbaik untuk melindungi mekanisme secara praktikal masih berkembang, dan amalan terbaik masih belum ditetapkan. Contohnya, pembangun yang berbeza menggunakan perlindungan yang berbeza, dan pendekatan mereka terhadap mitigasi risiko teknikal secara lebih meluas juga sangat berbeza (‡1116). Akhir sekali, kewujudan perlindungan teknikal yang berkesan tidak dengan sendirinya menjamin keselamatan, kerana penerimagunaan dan pelaksanaannya boleh berbeza-beza mengikut pembangun dan konteks penggunaan.

