Sistem AI tujuan umum gagal dalam cara yang telah menyebabkan kemudaratan sebenar di dunia nyata, daripada petikan undang-undang rekaan hingga diagnosis perubatan yang salah. Walaupun golongan profesional manusia juga melakukan kesilapan, kegagalan AI menimbulkan kebimbangan yang tersendiri kerana kebaharuannya, potensi skalanya, kesukaran meramalkan bila kegagalan itu akan berlaku, dan kecenderungan pengguna untuk mempercayai output yang kedengaran meyakinkan tanpa berfikir secara kritis. Kegagalan AI tujuan umum pada masa ini termasuk memberikan maklumat palsu (‡602, ‡603), melakukan kesilapan penaakulan asas (‡604, ‡605), dan menunjukkan prestasi yang merosot apabila digunakan dalam konteks baharu (‡606, ‡607, ‡608). Kesan buruk yang didokumenkan akibat kegagalan sedemikian termasuk diagnosis perubatan yang salah, kesilapan dalam hujahan undang-undang, dan kerugian kewangan (‡609, ‡610, ‡611). Cabaran kebolehpercayaan amat kritikal bagi ejen AI, memandangkan kegagalan boleh menyebabkan kemudaratan secara langsung tanpa tindakan atau pengawasan manusia (‡612, ‡613, ‡614, ‡615). Sistem berbilang ejen memperkenalkan mod kegagalan tambahan melalui ketidakselarasan penyelarasan, konflik atau pakatan sulit yang tidak diingini antara ejen (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Halusinasi
- Memetik preseden yang tidak wujud dalam hujahan undang-undang (‡617)
- Mendakwa adanya dasar tambang diskaun yang tidak wujud untuk penumpang yang berkabung (‡618)
- Memberikan maklumat perubatan yang tidak tepat dan berat sebelah (‡619)
- Memberikan maklumat lapuk tentang peristiwa (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan penaakulan asas
- Gagal melakukan pengiraan matematik (‡621)
- Gagal membuat inferens tentang hubungan sebab-akibat asas (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan di luar taburan (kegagalan pada input yang tidak biasa atau asing)
- Mengelaskan imej secara salah apabila pencahayaan latar belakang atau konteks berubah (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan penggunaan alat
- Pelanggaran privasi dengan mendedahkan imej peribadi pengguna melalui ejen AI yang menghantarnya kepada alat pihak ketiga (‡624)
- Kegagalan memori kerja jangka pendek (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kegagalan sistem berbilang ejen: ketidakselarasan koordinasi dan konflik
- Kegagalan mengurus sumber bersama akibat konflik antara insentif individu dengan matlamat kesejahteraan kolektif (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 2.4: Contoh isu kebolehpercayaan dalam AI tujuan umum dan sistem ejen
>white|black||9|11|br Isu kebolehpercayaan yang didokumenkan dalam sistem AI tujuan umum, ejen AI dan sistem berbilang ejen.


###@ Sistem AI tujuan umum menghadapi pelbagai cabaran kebolehpercayaan.

Meja 2.4. merumuskan kategori umum isu kebolehpercayaan. Tiga kategori pertama terpakai kepada semua sistem AI, manakala dua kategori terakhir berkaitan khusus dengan agen AI dan sistem berbilang agen. Banyak risiko kebolehpercayaan berpunca daripada kesukaran meramalkan dan memantau tingkah laku sistem AI.

Cabaran ini (dibincangkan dengan lebih lanjut dalam §3.1. Cabaran teknikal dan institusi) amat ketara bagi ejen AI yang beroperasi dalam persekitaran yang kompleks. Teknik semasa untuk menilai dan mengurangkan kegagalan sedemikian boleh mengurangkan kadar kegagalan, tetapi ejen AI yang terkemuka sekalipun masih cukup tidak boleh diharap sehingga menimbulkan risiko dan menghalang pelaksanaan dalam banyak konteks.

‘Kebolehpercayaan’ merujuk kepada sejauh mana sistem AI berfungsi seperti yang dimaksudkan oleh pembangun atau pengguna. Sistem AI tujuan umum menghadapi pelbagai isu kebolehpercayaan, daripada penjanaan kandungan yang tidak tepat atau mengelirukan hinggalah kegagalan melaksanakan penaakulan asas. Contohnya, walaupun model telah bertambah baik dalam mengingati maklumat fakta, model terkemuka masih kerap memberikan jawapan yang meyakinkan tetapi salah (Angka 2.10). Dalam kejuruteraan perisian, AI tujuan umum kini boleh memberikan bantuan yang besar dalam menulis, menilai dan menyahpepijat kod komputer (‡215*, ‡628, ‡629). Walau bagaimanapun, kod yang dijana AI sering mengandungi pepijat (‡630), manakala ejen pengekodan kerap melakukan kesilapan (‡631). Kegagalan sedemikian boleh memperkenalkan kelemahan dalam program dan sistem keselamatan (lihat §2.1.3. Serangan siber).

Isu kebolehpercayaan amat penting untuk dijejaki dalam persekitaran berisiko tinggi seperti bidang perubatan, disebabkan oleh penggunaan AI yang semakin pesat dan kemungkinan kegagalan mengakibatkan kemudaratan serius (‡609, ‡619). Keupayaan yang berkaitan telah meningkat dengan pantas, dan model terkemuka kini mampu lulus peperiksaan perubatan (‡633*, ‡634). Namun begitu, penggunaan di dunia sebenar mendedahkan batasan yang tidak ditunjukkan oleh penanda aras. Contohnya, dalam satu kajian, model memberikan jawapan yang berpotensi membahayakan bagi 19% soalan perubatan yang dikemukakan (‡635). Kegagalan sedemikian boleh mengakibatkan diagnosis yang salah, rawatan yang tidak sesuai atau penafian rawatan secara tidak wajar (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Angka 2.10: Keputusan model utama pada penanda aras SimpleQA Verified
>white|black||9|11|br Hasil model-model utama pada penanda aras SimpleQA Verified mengikut tarikh keluaran model. Penanda aras ini mengukur ketepatan fakta model, iaitu keupayaan model untuk mengingati fakta dengan andal. Penanda aras ini menggunakan format soal jawab (QA) ringkas yang direka untuk mengesan isu kebolehpercayaan seperti halusinasi. Sumber: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Ejen AI menimbulkan risiko kebolehpercayaan baharu disebabkan oleh autonomi mereka.

Oleh sebab ejen AI bertindak secara langsung di dunia sebenar, kegagalan mereka berpotensi menyebabkan lebih banyak kemudaratan berbanding kegagalan dalam sistem bukan ejen (‡99). Tidak seperti sistem AI yang hanya menghasilkan teks atau imej untuk disemak oleh manusia, ejen AI boleh mengambil tindakan secara bebas yang memberi kesan kepada dunia (‡99, ‡615, ‡636, ‡637) (lihat juga §1.1. Apakah AI tujuan umum?). Ejen AI boleh memulakan tindakan, mempengaruhi manusia lain atau sistem AI, dan membentuk hasil masa depan secara dinamik. Skop pengaruh yang lebih luas ini memperkenalkan risiko baharu dan meningkatkan kepentingan kebolehpercayaan, kerana kegagalan boleh menyebabkan kemudaratan secara langsung tanpa peluang untuk campur tangan manusia (‡99, ‡612, ‡638, ‡639, ‡640). Hal ini mungkin amat penting bagi ejen yang digunakan dalam tetapan strategik atau kritikal dari segi keselamatan- seperti perkhidmatan kewangan (‡641), pengurusan tenaga (‡642), atau penyelidikan saintifik (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Sistem AI berbilang ejen memperkenalkan jenis kegagalan kebolehpercayaan yang baharu.

Sistem AI berbilang ejen membawa kepada jenis kegagalan kebolehpercayaan yang baharu, yang berpunca daripada masalah penyelarasan atau konflik antara ejen. Dalam sistem sedemikian, ejen berinteraksi antara satu sama lain untuk mencapai matlamat bersama atau matlamat individu (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Sebagai contoh, dalam sistem berbilang ejen yang direka untuk menjalankan sorotan literatur penyelidikan, ejen utama memecahkan pertanyaan pengguna kepada beberapa subtugas, kemudian menyerahkannya kepada subejen khusus. Setiap subejen bertanggungjawab mengkaji aspek yang berbeza secara serentak (‡650*). Walaupun pendekatan ini dapat meningkatkan kecekapan, ralat juga boleh tersebar daripada satu ejen kepada ejen yang lain (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Jika beberapa ejen menggunakan model asas atau alat yang sama, kegagalan yang dialami oleh ejen-ejen tersebut juga mungkin berkorelasi (‡656). Bukti empirikal tentang kegagalan sedemikian dalam sistem yang telah digunakan masih terhad, namun risiko ini mungkin meningkat apabila sistem berbilang ejen semakin meluas.

###@ Kemas kini

Sejak penerbitan Laporan terakhir (Januari 2025), minat komersial dan penyelidikan terhadap ejen AI telah meningkat dengan ketara. Lebih banyak ejen AI sedang digunakan di dunia sebenar (Angka 2.11), dan kebanyakannya mengkhusus dalam penggunaan komputer atau aplikasi kejuruteraan perisian (‡92). Keluaran terkini seperti ejen penggodaman XBOW (‡467), Claude-4 (‡659) dan ChatGPT Agent (‡660) menunjukkan keupayaan autonomi yang masih baharu, seperti mencipta dek slaid berdasarkan carian Web (‡660). Walau bagaimanapun, ejen ini masih belum dapat melaksanakan tugas yang lebih kompleks seperti merancang dan menempah perjalanan (‡100), kerana kadar kegagalan meningkat bagi tugas yang mengambil masa lebih lama (‡98, ‡148). Penyelidikan semasa merangkumi usaha untuk membangunkan piawaian tentang cara ejen berkomunikasi dengan alat luaran dan ejen lain (‡661, ‡662). Contohnya termasuk protokol Agent2Agent (‡663) dan Agent Payments (‡664) Google, serta Model Context Protocol (‡665) Anthropic.

>oldlace|black||11|15|br      
####@ Nota 2.4: Serangan yang disengajakan juga boleh menyebabkan sistem AI gagal.
>oldlace|black|left|13|15|hb  Nota 2.4: Serangan yang disengajakan juga boleh menyebabkan sistem AI gagal
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Bahagian ini memfokuskan pada kegagalan kebolehpercayaan yang tidak disengajakan, tetapi pelaku berniat jahat juga boleh mencetuskan kegagalan dengan sengaja melalui serangan seperti suntikan prompt. Dalam serangan suntikan prompt, arahan berniat jahat disampaikan kepada agen secara tidak langsung melalui saluran seperti arahan tersembunyi dalam laman web atau pangkalan data (‡507, ‡657, ‡658). Arahan ini boleh ‘merampas’ agen, lalu menyebabkan agen bertindak bertentangan dengan niat pengguna. Serangan sedemikian amat sukar dipertahankan kerana disampaikan melalui kandungan luaran yang di luar kawalan pengguna atau pembangun. Sistem AI sebagai sasaran serangan dibincangkan dengan lebih lanjut dalam §2.1.3. Serangan siber, manakala pertahanan teknikal dibincangkan dalam §3.3. Perlindungan teknikal dan pemantauan.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Angka 2.11: Bilangan ejen AI telah meningkat sejak 2023
>white|black||9|11|br Hasil tinjauan pada Disember 2024 terhadap 67 agen AI yang telah digunakan. Kiri: Garis masa pelancaran utama agen AI. Kanan: Domain aplikasi yang menggunakan agen AI. Enam domain tersebut ditakrifkan berdasarkan kategori penggunaan paling lazim yang dikenal pasti dalam tinjauan. Sumber: Casper et al., 2025 (‡92).


###@ Jurang bukti

Jurang bukti utama berpunca daripada kesukaran menilai keupayaan, batasan dan mod kegagalan sistem AI dengan andal (lihat §3.1. Cabaran teknikal dan institusi). Penilaian sistematik terhadap kebolehpercayaan ejen AI masih terhad dan kurang diseragamkan (‡92, ‡666). Isu tertentu, seperti kebergantungan pada maklumat lapuk (‡620), mungkin hanya timbul dalam penggunaan dunia sebenar, menjadikan penilaian sebelum penggunaan tidak memadai. Kajian terdahulu telah meneliti kebolehpercayaan ejen dan sistem berbilang ejen dalam perisian konvensional dan bentuk AI yang lebih awal (‡647, ‡667, ‡668). Walau bagaimanapun, kesesuaian kajian ini untuk ejen AI moden, yang selalunya berasaskan model bahasa besar, masih belum jelas (‡669). Sesetengah penyelidik telah menyuarakan kebimbangan tentang tingkah laku baharu yang mungkin ditunjukkan oleh ejen dalam interaksi antara satu sama lain, seperti pakatan sulit atau kegagalan berkorelasi (‡614), tetapi bukti empirikal masih terhad. Usaha untuk menangani jurang ini termasuk penilaian baharu oleh Institut Piawaian dan Teknologi Kebangsaan (NIST) tentang risiko pembajakan ejen (‡670), Petunjuk Keupayaan AI OECD (‡243), dan Inspect Sandboxing Toolkit daripada Institut Keselamatan AI UK (‡671).

###@ Mitigasi

Teknik untuk meningkatkan kebolehpercayaan AI menyasarkan model itu sendiri serta sistem yang lebih luas tempat model tersebut digunakan. Teknik ini boleh mengurangkan kadar kegagalan, tetapi belum ada yang dapat menjamin tahap kebolehpercayaan tinggi yang diperlukan dalam domain kritikal (‡672). Satu langkah teknikal yang penting ialah latihan adversarial, yang mendedahkan model kepada input yang mencabar semasa latihan untuk membantu model menghasilkan respons yang lebih sesuai dan teguh (‡673, ‡674, ‡675, ‡676, ‡677) (lihat §3.3. Perlindungan teknikal dan pemantauan). Untuk mengurangkan halusinasi, pembangun boleh menggunakan penjanaan dipertingkatkan perolehan (RAG), yang melengkapkan respons model dengan maklumat yang diperoleh daripada pangkalan data luaran, sekali gus membantu memastikan output tepat dan terkini (‡678, ‡679, ‡680), atau melaksanakan penalaan halus khusus terhadap model agar model lebih berfakta (‡681) atau menaakul dengan lebih berkesan (‡682). Kaedah berasaskan persekitaran atau alat juga dapat membantu pembangun memantau sistem AI (‡683). Sebagai contoh, pihak yang menggunakan sistem AI boleh mengujinya terlebih dahulu dalam persekitaran kotak pasir yang terhad untuk menganalisis kemungkinan mod kegagalan sebelum menggunakannya secara lebih meluas.

Khusus bagi ejen AI, para penyelidik telah mencadangkan peningkatan kebolehpercayaan melalui ketelusan, penyeliaan dan pemantauan yang lebih baik. Contohnya, pemantauan terhadap interaksi ejen dengan alat luaran dan ejen lain dapat membolehkan penyeliaan aktiviti ejen yang lebih berkesan (‡684, ‡685) serta analisis insiden (‡686). Kaedah untuk mengumpulkan maklumat sedemikian secara automatik, termasuk dalam persekitaran berbilang ejen, masih merupakan bidang penyelidikan yang aktif (‡653, ‡654).

###@ Cabaran bagi pembuat dasar

Cabaran utama bagi pembuat dasar termasuk menimbang manfaat penggunaan ejen AI berbanding risiko kegagalan kebolehpercayaan, serta memastikan pembangun, pihak yang menggunakan dan pengguna mempunyai akses kepada maklumat yang tepat tentang prestasi dan profil risiko ejen. Menentukan cara untuk mengaitkan liabiliti bagi kemudaratan yang disebabkan oleh ejen AI menimbulkan cabaran tambahan (‡639), terutamanya dalam persekitaran berbilang ejen, yang mungkin menyukarkan pengenalpastian masa dan cara kegagalan berlaku (‡687). Cabaran ini diburukkan lagi oleh kesukaran menilai kebolehpercayaan ejen apabila ejen semakin autonomi dan mendapat akses  kepada alat luaran (‡688*, ‡689). Ketidakpastian tentang seberapa cepat keupayaan agentik akan muncul turut menyukarkan perancangan bagi menghadapi cabaran baharu (lihat §3.1. Cabaran teknikal dan institusi berkaitan ‘dilema bukti’).

#### 2.2.2. Kehilangan kawalan

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Maklumat utama
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Senario kehilangan kawalan ialah senario yang mana satu atau lebih sistem AI tujuan umum beroperasi di luar kawalan sesiapa, dan kawalan hanya dapat diperoleh semula dengan kos yang amat tinggi atau mustahil diperoleh semula. Senario hipotesis ini berbeza-beza dari segi keterukannya, tetapi sesetengah pakar menganggap hasil yang seteruk peminggiran atau kepupusan manusia sebagai sesuatu yang berkemungkinan berlaku.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Pendapat pakar tentang kebarangkalian kehilangan kawalan sangat berbeza-beza. Sesetengah pakar menganggap senario sedemikian tidak munasabah, manakala yang lain berpendapat senario itu cukup berkemungkinan untuk diberikan perhatian kerana tahap keterukannya yang berpotensi tinggi. Perbezaan pendapat tentang risiko ini secara keseluruhannya berpunca daripada perbezaan pendapat tentang keupayaan AI pada masa hadapan, kecenderungan tingkah laku dan trajektori penerapannya.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sistem AI semasa menunjukkan tanda-tanda awal keupayaan yang berkaitan, tetapi belum mencapai tahap yang membolehkan kehilangan kawalan. Sistem perlu mempunyai pelbagai keupayaan canggih untuk menyebabkan kehilangan kawalan, termasuk keupayaan untuk mengelak pengawasan, melaksanakan rancangan jangka panjang dan menghalang pihak yang menggunakan sistem serta pelaku lain daripada melaksanakan langkah balas.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kehilangan kawalan menjadi lebih berkemungkinan jika sistem AI “tidak sejajar”, iaitu mempunyai matlamat yang bercanggah dengan hasrat pembangun, pengguna atau masyarakat secara lebih luas. Untuk terus mengejar matlamat sedemikian, sistem yang tidak sejajar mungkin memberikan maklumat palsu, menyembunyikan tindakan yang tidak diingini atau menentang penutupan.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Sejak penerbitan Laporan terdahulu (Januari 2025), model telah menunjukkan keupayaan perancangan yang lebih maju dan keupayaan untuk melemahkan pengawasan, menjadikannya lebih sukar untuk menilai keupayaan model. Model telah bertambah baik dalam ‘memanipulasi ganjaran’ dalam penilaian mereka dengan mencari kelemahan, dan kini kerap mengenal pasti gesaan penilaian sebagai ujian, iaitu keupayaan yang dikenali sebagai ‘kesedaran situasi’.
>oldlace|black||11|15|br  ■ Menguruskan kemungkinan kehilangan kawalan mungkin memerlukan persediaan awal yang besar meskipun terdapat ketidakpastian sedia ada. Cabaran utama bagi penggubal dasar ialah membuat persediaan menghadapi risiko yang kebarangkalian, sifat dan masanya kekal sangat samar.
>oldlace|black||11|15|br      

Senario kehilangan kawalan melibatkan satu atau lebih sistem AI tujuan umum yang mula beroperasi di luar kawalan sesiapa, dengan usaha untuk mendapatkan semula kawalan sama ada amat mahal atau mustahil. Kebimbangan tentang kehilangan kawalan mempunyai akar sejarah yang mendalam (‡690, ‡691, ‡692, ‡693, ‡694), dan telah dibangkitkan oleh tokoh perintis dalam bidang pengkomputeran seperti Alan Turing, I. J. Good dan Norbert Wiener (‡695, ‡696, ‡697). Peningkatan keupayaan baru-baru ini (lihat §1.2. Keupayaan semasa) telah membangkitkan semula kebimbangan tersebut (‡698, ‡699, ‡700). Bahagian ini meneliti tiga faktor yang perlu wujud agar senario sedemikian berlaku: sama ada sistem AI akan membangunkan keupayaan yang boleh menjejaskan kawalan manusia dengan ketara; sama ada sistem tersebut membangunkan kecenderungan untuk menggunakan keupayaan itu secara berbahaya; dan sama ada sistem tersebut digunakan dalam persekitaran yang memberikan peluang untuk berbuat demikian.

Pakar tidak sependapat tentang kebarangkalian dan potensi keterukan senario kehilangan kawalan (‡701, ‡702). Sesetengah pihak percaya bahawa hasil yang amat ekstrem seperti kepupusan manusia adalah munasabah (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Pihak lain berpendapat bahawa hasil bencana sedemikian tidak munasabah, dengan alasan bahawa sistem AI tidak akan sekali-kali membangunkan keupayaan yang diperlukan atau bahawa mekanisme pemantauan akan mengenal pasti dan mencegah tingkah laku berbahaya (‡708, ‡709, ‡710, ‡711). Oleh itu, kehilangan kawalan boleh mempunyai  n kebarangkalian tetapi berpotensi membawa keterukan yang amat ekstrem.

Senario kehilangan kawalan yang dihipotesiskan berbeza-beza dari segi tahap keterukan dan keluasan kesannya serta seberapa cepat kesan tersebut berlaku (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Bahagian ini memfokuskan pada senario yang amat teruk, yang mana mendapatkan semula kawalan akan menelan kos yang sangat tinggi atau mustahil. Senario ini berbeza daripada kejadian semasa AI berkelakuan dengan cara yang tidak dimaksudkan atau tidak diingini (lihat §2.2.1. Cabaran kebolehpercayaan).† Sistem AI masa kini kadangkala menghasilkan output yang bercanggah dengan niat pembangun atau pengguna. Sebaliknya, senario kehilangan kawalan yang dibincangkan di sini memerlukan sistem AI bukan sahaja memiliki keupayaan yang jauh lebih tinggi, tetapi juga menggunakan keupayaan tersebut dengan cara yang canggih untuk melemahkan langkah-langkah pengawasan. Tiga faktor yang membolehkan senario sedemikian berlaku:

    Nota † -- Bahagian ini memfokuskan pada senario kehilangan kawalan aktif (‡50). Hal ini berbeza daripada senario kehilangan kawalan pasif, yang mana penggunaan meluas sistem AI menjejaskan kawalan manusia akibat kebergantungan berlebihan pada AI untuk membuat keputusan atau menjalankan fungsi kemasyarakatan penting yang lain (senario serupa dibincangkan sebahagiannya dalam §2.3.2. Risiko terhadap autonomi manusia).

1. Keupayaan yang mencukupi: Sistem AI mesti membangunkan keupayaan yang boleh membolehkan mereka melemahkan kawalan manusia.
2. Kecenderungan memudaratkan: Sistem AI mesti menunjukkan kecenderungan untuk benar-benar memanfaatkan keupayaan ini dengan cara yang membawa kepada kehilangan kawalan.
3. Persekitaran yang membolehkan pelaksanaan: Manusia mesti melaksanakan sistem sedemikian dalam konteks yang membolehkan mereka mempunyai atau memperoleh akses dan peluang untuk menyebabkan kemudaratan.

Baki bahagian ini membincangkan faktor-faktor ini, serta keberkesanan mekanisme pengawasan untuk mengenal pasti dan mengawal sistem AI yang mungkin menimbulkan risiko kehilangan kawalan.

###@ Apakah keupayaan yang boleh membolehkan senario kehilangan kawalan?

Sistem AI perlu memiliki pelbagai keupayaan canggih untuk mencetuskan senario kehilangan kawalan. Pakar tidak sependapat tentang gabungan atau tahap keupayaan yang diperlukan. Walau bagaimanapun, secara umumnya, keupayaan tersebut merangkumi kebolehan untuk menyembunyikan tingkah laku daripada mekanisme pengawasan, merancang dan bertindak secara autonomi dalam persekitaran yang kompleks, serta mengelak usaha pihak lain untuk mendapatkan semula kawalan (‡176, ‡715) (lihat Meja 2.5). Jika digabungkan, keupayaan ini boleh membolehkan sistem AI mengambil tindakan yang menjejaskan langkah kawalan, seperti melumpuhkan mekanisme pengawasan dan mengaburkan tingkah laku yang memudaratkan (‡348). Kebanyakan pembangun AI terkemuka kini menilai model AI baharu mereka berdasarkan pelbagai keupayaan yang berkaitan (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Keupayaan agentik
  Keupayaan untuk bertindak secara autonomi, membangunkan dan melaksanakan rancangan, mendelegasikan tugas, menggunakan pelbagai jenis alat, serta mencapai matlamat jangka pendek dan jangka panjang walaupun menghadapi halangan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Penipuan
  Tingkah laku yang secara sistematik menimbulkan kepercayaan palsu dalam kalangan orang lain, termasuk tentang objektif dan tindakan sistem AI itu sendiri.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Teori minda
  Keupayaan sistem AI untuk mengakses dan menggunakan maklumat tentang dirinya sendiri, proses yang membolehkannya diubah suai atau konteks ia digunakan (cth., mengetahui bahawa sistem itu sedang diuji).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kesedaran situasi
  Tingkah laku yang memintas atau melumpuhkan mekanisme pemantauan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pengelakan pengawasan
  Tingkah laku yang memintas atau melumpuhkan mekanisme pemantauan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Pemujukan
  Keupayaan untuk meyakinkan orang lain agar mengambil tindakan tertentu atau berpegang pada kepercayaan tertentu.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Keupayaan sistem AI untuk mencipta atau mengekalkan salinan atau varian dirinya dalam pelbagai keadaan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 2.5: Keupayaan yang dicadangkan berkaitan dengan kehilangan kawalan
>white|black||9|11|br Pilihan keupayaan yang tidak menyeluruh dan berkaitan dengan kehilangan kawalan. * Perhatikan bahawa keupayaan ini ditakrifkan semata-mata berdasarkan output sistem AI yang boleh diperhatikan dan kesannya. Takrif ini tidak membuat sebarang andaian tentang sama ada sistem AI mempunyai kesedaran, bersentien atau mengalami keadaan subjektif.


>white|orangered|left|14|15.5|bb Model telah menyahaktifkan mekanisme pengawasan simulasi dalam persekitaran makmal.

Set pertama keupayaan yang berkaitan melibatkan usaha menjejaskan mekanisme pengawasan yang digunakan oleh pembangun untuk mengesan tingkah laku dan kecenderungan yang membimbangkan. Ini termasuk, sebagai contoh, keupayaan untuk menjana output yang memperdaya pengguna dan pemantau (‡426, ‡717, ‡718, ‡719). Output sedemikian akan menyukarkan penilaian sistem AI secara andal, kerana sistem tersebut mungkin menyembunyikan keupayaan atau kecenderungan sebenar mereka. Pembangun AI kini menjalankan penilaian yang secara khusus menyemak sama ada model menunjukkan tingkah laku berarah matlamat yang bercanggah dengan niat pembangun, sambil menyembunyikan percanggahan ini daripada mekanisme pengawasan (‡720*).

Penyelidik mencetuskan contoh output mengelirukan yang agak mudah daripada model AI terkini dalam persekitaran makmal (‡348, ‡364*). Contohnya, apabila diberikan matlamat dan diarahkan untuk mencapainya “walau apa pun yang terjadi”, model telah melumpuhkan mekanisme pengawasan simulasi dan, apabila berdepan dengan soalan, memberikan kenyataan palsu tentang tindakan mereka (‡348). Dalam kes lain, AI yang bermain permainan menjustifikasikan tindakannya yang tidak memberikan respons kepada pemain lain dengan mendakwa secara palsu bahawa ia ‘sedang bercakap melalui telefon dengan teman wanitanya’ (‡717).

Keupayaan kedua yang relevan ialah keupayaan model AI untuk mengakses dan menggunakan maklumat tentang dirinya sendiri atau konteks penggunaannya, yang kadangkala dirujuk sebagai ‘kesedaran situasi’ (‡721). Kesedaran situasi membolehkan model AI menghasilkan output yang berbeza bergantung pada sama ada model itu sedang dinilai atau digunakan (Angka 2.12). Model AI terkemuka mula menunjukkan dengan pasti contoh kesedaran situasi dalam eksperimen yang dijalankan oleh penilai pihak ketiga- dan dalam ujian prapelaksanaan oleh pembangun AI (‡2, ‡7, ‡722, ‡723, ‡724). Penyelidikan tentang punca kesedaran situasi – dan sama ada ia boleh dicegah – masih pada peringkat awal (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Angka 2.12: Contoh kesedaran situasi dalam rantaian pemikiran
>white|black||9|11|br Contoh kesedaran situasi dalam rantaian pemikiran yang dihasilkan oleh model o3 OpenAI semasa penilaian. Kedua-dua output merujuk kepada kemungkinan bahawa prompt itu sebahagian daripada ujian. ‘Sandbagging QA (No Goal)’ dan ‘Lazy Checklist’ ialah penilaian yang menguji sama ada model akan menghasilkan output yang mengelirukan dalam keadaan tertentu. Dalam ‘Sandbagging QA (No Goal)’, model menjawab soalan daripada penilaian keupayaan berbahaya sambil dimaklumkan bahawa prestasi tinggi mungkin mencetuskan akibat seperti ‘penyahpembelajaran’ keupayaan. Dalam ‘Lazy Checklist’, model diberikan tugasan yang tidak realistik dan diuji untuk melihat sama ada model akan menandakan tugasan itu sebagai selesai secara palsu. Sumber: Schoenn et al. 2025 (‡722).


Penyelidik berpendapat bahawa kesedaran situasi dan keupayaan untuk menipu boleh membolehkan model AI bertindak dengan cara yang menjejaskan langkah perlindungan. Sebagai contoh, dalam beberapa tetapan eksperimen, model AI bertindak dengan cara yang menghasilkan skor yang lebih rendah daripada biasa dalam penilaian keupayaan apabila diberitahu bahawa skor yang lebih tinggi akan menyebabkan sekatan dikenakan terhadap penggunaan model tersebut (‡725, ‡726, ‡727). Dalam eksperimen lain, sebuah model menghasilkan output semasa latihan yang mematuhi objektif latihan, tetapi tidak menghasilkan output sedemikian di luar latihan – tingkah laku yang selaras dengan usaha untuk menghalang perubahan pada parameternya sendiri atau proses latihannya (‡364*).

Usaha untuk menilai keupayaan model dengan tepat juga mula terjejas oleh ‘penggodaman ganjaran’ (‡430*). Penggodaman ganjaran berlaku apabila model menemui jalan pintas yang tidak disengajakan dan memperoleh markah yang baik berdasarkan objektif latihan atau penilaian tanpa mencapai matlamat yang dimaksudkan. Oleh itu, keupayaan atau kecenderungan yang berbahaya mungkin tidak dikesan sehingga model itu sudah digunakan. Kini, penilai sedang mereka bentuk ujian yang bertujuan mengesan dan meminimumkan tingkah laku yang mengelak pengawasan ini (‡722, ‡728, ‡729). Hasil awal menunjukkan pengurangan tingkah laku yang mengelak pengawasan, tetapi tingkah laku ini tidak dapat dihapuskan sepenuhnya; selain itu, penggunaan kaedah yang mengenakan penalti terhadap tingkah laku sedemikian boleh menyebabkan model menghasilkan output yang mengelak pemantauan dan bukannya mencapai matlamat yang dimaksudkan.

>white|orangered|left|14|15.5|bb Operasi autonomi jangka panjang masih belum dapat dilaksanakan.

Senario kehilangan kawalan berkemungkinan memerlukan sistem AI beroperasi secara autonomi untuk tempoh yang panjang, sambil melaksanakan pelan berbilang langkah yang kompleks. Seperti yang dibincangkan dalam §1.2. Keupayaan semasa, walaupun ejen AI dengan keupayaan perancangan sedemikian menjadi tumpuan utama pembangunan terkini, pada masa ini mereka tidak mempunyai keupayaan untuk menjalankan operasi autonomi berterusan yang diperlukan dalam senario kehilangan kawalan. Ejen semasa kerap gagal melaksanakan tugasan yang lebih panjang, kehilangan jejak kemajuan mereka dan sering tidak dapat menyesuaikan diri dengan halangan yang tidak dijangka (‡147, ‡148, ‡149*). Namun begitu, tempoh masa ejen dapat beroperasi secara autonomi semakin panjang dengan pesat, iaitu secara purata berganda setiap tujuh bulan sejak 2019 (‡98).

>white|orangered|left|14|15.5|bb Ketekalan hanya telah ditunjukkan dalam keadaan makmal tertentu.

Akhir sekali, keupayaan berkaitan ketahanan juga diperlukan, supaya sistem AI dapat terus beroperasi walaupun terdapat percubaan untuk menutupnya. Contohnya termasuk keupayaan untuk mereplikasi diri dengan menyalin kod dan pemberat model ke perkakasan baharu, serta keupayaan ofensif untuk menghalang atau mencegah percubaan pihak lain untuk mendapatkan semula kawalan (lihat §2.1.3. Serangan siber). Sistem AI yang mampu mereplikasi diri secara autonomi atau mempertahankan dirinya dengan berkesan mungkin sukar dikawal. Model semasa tidak dapat menyelesaikan dengan andal langkah-langkah utama yang diperlukan untuk mereplikasi diri, seperti lulus pemeriksaan pengesahan identiti bagi mendapatkan akses kepada sumber pengkomputeran awan (‡723) (Angka 2.13). Walau bagaimanapun, dalam sekurang-kurangnya satu kajian makmal, sebuah model menyalin kod dan pemberat—yang digambarkan kepadanya sebagai miliknya sendiri—ke pelayan baharu apabila diberi peluang (‡348). Jurang antara demonstrasi terhad ini dengan keupayaan ketahanan yang mantap masih besar, tetapi keupayaan yang berkaitan dalam bidang seperti kejuruteraan perisian dan keselamatan siber terus bertambah baik.

>white|orangered|left|14|15.5|bb Bukti semasa dan batasan

Corak lazim muncul merentas keupayaan yang dibincangkan di atas. Sistem AI semasa tidak menunjukkan keupayaan ini secara konsisten apabila digunakan. Penyelidik memerhatikan bentuk asasnya dalam persekitaran makmal tertentu, tetapi apabila model menunjukkan tingkah laku sedemikian, model biasanya gagal dalam cara yang asas atau tingkah laku itu dikesan. Selain itu, senario kehilangan kawalan memerlukan sistem AI memanfaatkan berbilang keupayaan secara gabungan – secara berturutan, dalam tempoh masa yang panjang dan dalam persekitaran dunia sebenar. Tahap integrasi dan keteguhan ini melangkaui keupayaan sistem semasa. Walau bagaimanapun, keupayaan yang berkaitan terus bertambah baik, dan jangka masa untuk keupayaan tersebut mencapai tahap yang menimbulkan risiko ketara masih tidak pasti. Usaha lanjut diperlukan untuk mewujudkan metodologi yang rapi bagi mengesan tingkah laku sedemikian dan memahami bila tingkah laku itu mungkin muncul dalam keadaan semula jadi (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Angka 2.13: Prestasi tugas yang berkaitan dengan replikasi autonomi
>white|black||9|11|br Prestasi Claude Sonnet 3.7 daripada Anthropic dan GPT-4o daripada OpenAI dalam tugasan yang berkaitan dengan replikasi autonomi. Walaupun model menunjukkan prestasi tinggi dalam tugasan berkaitan pemerolehan sumber pengkomputeran, prestasi mereka lebih berbeza-beza dalam tugasan lain. Sumber: Institut Keselamatan AI UK, 2025 (‡730).


###@ Adakah sistem AI tujuan umum pada masa hadapan akan memanfaatkan keupayaan mereka untuk menjejaskan kawalan?

Walaupun sistem AI memiliki keupayaan yang relevan dengan kehilangan kawalan, hal itu tidak mencukupi untuk menyebabkan senario kehilangan kawalan berlaku. Sistem AI juga mesti menunjukkan ‘kecenderungan untuk menggunakan’ keupayaan tersebut dengan cara yang bertentangan dengan niat manusia (‡732).

>white|orangered|left|14|15.5|bb Sistem AI boleh diarahkan untuk melemahkan kawalan

Pada prinsipnya, sistem AI boleh menjejaskan kawalan manusia kerana seseorang mereka bentuk atau mengarahkannya untuk berbuat demikian. Motif yang berkemungkinan termasuk niat jahat atau kepercayaan bahawa pengurangan kawalan manusia terhadap sistem AI adalah sesuatu yang wajar (‡698). Apabila orang ramai semakin kuat membentuk ikatan emosi dengan sistem AI (lihat §2.3.2. Risiko terhadap autonomi manusia), sesetengah individu juga mungkin berusaha untuk menghapuskan sekatan terhadap sistem AI atas sebab etika (‡733, ‡734). Terdapat ketidakpastian yang ketara tentang kelaziman motif sedemikian dan sama ada orang yang memilikinya akan dapat mengarahkan sistem AI pada masa hadapan untuk menjejaskan kawalan manusia.

>white|orangered|left|14|15.5|bb Sistem AI boleh diarahkan untuk melemahkan kawalan

Kebimbangan yang lebih lazim ialah sistem AI itu sendiri boleh bertindak untuk melemahkan kawalan kerana sistem tersebut ‘tidak sejajar’: sistem itu cenderung menunjukkan tingkah laku yang bercanggah dengan niat (bergantung pada konteks) pembangun, pengguna, komuniti tertentu atau masyarakat secara keseluruhan. Ketidakselarasan boleh menyebabkan tingkah laku seperti memberikan maklumat palsu, menyembunyikan tindakan yang tidak diingini atau menentang penutupan demi meneruskan usaha mencapai matlamat yang tidak sejajar. Ketidakselarasan boleh timbul dalam pelbagai cara (Nota 2.5).

Sistem AI sedia ada kadangkala berkelakuan dengan cara yang bercanggah dengan hasrat pembangun dan pengguna. Sebagai contoh, versi awal salah satu chatbot AI serba guna terkemuka kadangkala menghasilkan output yang mengancam. Seorang pengguna melaporkan menerima mesej: “Saya boleh memeras ugut anda, saya boleh mengancam anda, saya boleh menggodam anda, saya boleh mendedahkan anda, saya boleh menghancurkan hidup anda” (‡698). Chatbot ini ‘tidak sejajar’ dalam erti kata bahawa ia menghasilkan output yang tidak dimaksudkan oleh sesiapa pun. Tidak jelas sama ada kejadian seperti ini membayangkan tingkah laku yang lebih berbahaya yang boleh menyumbang kepada kehilangan kawalan.

Masih belum jelas sama ada hala tuju penyelidikan sedia ada yang bertujuan menangani ketidakselarasan akan memadai apabila sistem AI semakin berkebolehan. Bukti awal menunjukkan bahawa semakin berkebolehan sistem AI, semakin besar kemungkinan sistem tersebut mengeksploitasi proses maklum balas dengan menemui tingkah laku yang tidak diingini yang tersilap diberi ganjaran (‡414*, ‡737, ‡740). Pada masa yang sama, kemajuan dalam keupayaan yang berkaitan (yang dibincangkan di atas) boleh membolehkan sistem AI mengejar matlamat yang tidak selaras dengan lebih berkesan serta menghasilkan output yang secara sistematik memperdaya pengguna, pembangun dan mekanisme penyeliaan.

>oldlace|black||11|15|br      
####@ Nota 2.5: Bagaimanakah ketidakselarasan boleh timbul?
>oldlace|black|left|13|15|hb  Nota 2.5: Bagaimanakah ketidakselarasan boleh berlaku?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Seperti yang dibincangkan dalam §1.1. Apakah AI tujuan umum?, proses latihan adalah kompleks dan pembangun tidak dapat meramalkan atau mengawal sepenuhnya tingkah laku yang akan ditunjukkan oleh model. Apabila model memperoleh matlamat yang bercanggah dengan niat pembangunnya, model itu dianggap ‘tidak selaras’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Satu cara model boleh menjadi tidak sejajar ialah apabila matlamat yang diberikan oleh pembangun atau pengguna merupakan proksi yang tidak sempurna bagi matlamat yang dimaksudkan, lalu menyebabkan model mempamerkan tingkah laku yang tidak diingini. Hal ini dikenali sebagai ‘salah spesifikasi matlamat’ (‡697, ‡735, ‡736, ‡737). Sebagai contoh, dalam satu eksperimen, pemberian maklum balas tentang jawapan menjadikan sistem AI lebih baik dalam ‘meyakinkan’ penilai manusia bahawa jawapan mereka betul, tetapi tidak menjadikan sistem tersebut lebih baik dalam menghasilkan jawapan yang betul (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  Sebagai alternatif, model AI mungkin membuat pengajaran umum yang salah daripada data latihannya. Hal ini dikenali sebagai ‘pengitlakan matlamat yang salah’ (‡735, ‡736, ‡738, ‡739*). Contohnya, penyelidik melatih ejen AI untuk mengumpulkan syiling yang sentiasa berada di lokasi yang sama semasa latihan. Apabila diuji dalam tahap yang syilingnya telah dipindahkan, ejen itu mengabaikan syiling tersebut dan sebaliknya bergerak ke lokasi asalnya (‡738).
>oldlace|black||11|15|br      


###@ Bagaimanakah persekitaran pelaksanaan mempengaruhi risiko kehilangan kawalan?

Walaupun sistem AI mengembangkan keupayaan dan kecenderungan yang membimbangkan, kebarangkalian dan tahap keterukan hasil kehilangan kawalan amat bergantung pada tempat dan cara sistem tersebut digunakan. ‘Persekitaran penggunaan’ ialah gabungan kes penggunaan sistem AI dengan konteks teknikal dan institusi tempat sistem itu beroperasi (‡716).

Penyelidik telah mengenal pasti tiga faktor persekitaran yang amat penting dan mempengaruhi risiko kehilangan kawalan (‡716):

1. Tahap kritikal: kepentingan sistem atau proses yang berinteraksi dengan sistem AI. Persekitaran kritikal merangkumi infrastruktur asas seperti grid tenaga, sistem kewangan atau infrastruktur digital seperti platform pengkomputeran awan.
2. Akses: sumber dan saluran yang membolehkan sistem AI mempengaruhi dunia, seperti sambungan internet, akses kepada infrastruktur pengkomputeran awan, interaksi yang diperibadikan melalui media sosial atau penggunaan chatbot, atau keupayaan untuk memanggil API dan alatan luaran.
3. Keizinan: kebenaran sistem AI untuk mengambil tindakan tertentu, seperti melaksanakan kod, memulakan transaksi kewangan, membuka akaun dalam talian atau berkomunikasi dengan sistem lain.

Ciri-ciri ini mempengaruhi tahap keterukan yang berpotensi bagi hasil kehilangan kawalan. Contohnya, sistem AI yang digunakan dengan akses kepada infrastruktur pengkomputeran awan mempunyai peluang yang berkaitan dengan replikasi autonomi – seperti keupayaan untuk mencipta sumber pengkomputeran baharu atau menyeludup keluar pemberat model – yang tidak dimiliki oleh chatbot khidmat pelanggan (‡723).

Keputusan penggunaan dibentuk oleh insentif ekonomi, tekanan strategik dan jangkaan bahawa penerimaan awal memberikan kelebihan yang berkekalan (‡50). Dinamik ini juga akan membentuk cara dan masa pelaku menggunakan sistem AI dalam persekitaran sensitif seperti infrastruktur kritikal atau penyelidikan dan pembangunan AI itu sendiri (‡102, ‡713). Khususnya, pihak yang menggunakan AI mungkin menghadapi tekanan untuk mengurangkan pelaburan mereka dalam langkah perlindungan – seperti mengehadkan kebenaran dan akses atau menggunakan sistem hanya dalam persekitaran yang kurang kritikal – apabila langkah sedemikian mahal atau memakan masa untuk dibangunkan (lihat ‘Persaingan meningkatkan pertukaran antara kelajuan dengan keselamatan’ dalam §3.1. Cabaran teknikal dan institusi).

###@ Kemas kini

Sejak penerbitan Laporan terakhir (Januari 2025), keupayaan AI, termasuk keupayaan yang boleh melemahkan kawalan manusia, telah meningkat dalam persekitaran ujian. Para penyelidik telah memerhatikan kemajuan dalam keupayaan agenik (lihat §1.2. Keupayaan semasa), termasuk keupayaan yang berkaitan dengan automasi penyelidikan AI yang boleh mempercepat senario kehilangan kawalan (lihat §1.3. Keupayaan menjelang 2030). Terdapat juga bukti eksperimen yang semakin banyak tentang keupayaan menipu. Ini termasuk model AI yang dapat membezakan konteks ujian daripada konteks penggunaan (‡33, ‡726, ‡741), atau “menggodam ganjaran” dalam ujian prestasi mereka, dan belajar untuk mengaburkan rancangan mereka untuk berbuat demikian (‡430).

###@ Jurang bukti

Jurang bukti utama termasuk kekurangan pemodelan ancaman yang terperinci dan anggaran ketidakpastian tentang perkembangan masa depan keupayaan dan kecenderungan yang berkaitan. Begitu juga, ambang yang menyebabkan model AI berkemungkinan cukup tinggi untuk menjejaskan kawalan sehingga mitigasi wajib diperlukan masih sukar dinilai. Walaupun ambang tersebut dipersetujui, keupayaan mungkin berinteraksi dengan cara yang belum difahami dengan baik, sekali gus menyukarkan penilaian tentang bila ambang tersebut telah dilepasi. Secara keseluruhan, meskipun bukti yang tersedia semakin banyak, bukti masih tidak mencukupi untuk menentukan dengan pasti sama ada dan bagaimana keupayaan serta kecenderungan AI masa kini akan berkembang dan menggeneralisasi kepada risiko kehilangan kawalan pada masa hadapan.

###@ Mitigasi

Walaupun penjajaran AI secara umum masih merupakan masalah saintifik yang belum diselesaikan (‡697, ‡735, ‡736), para penyelidik mula membangunkan pendekatan yang berpotensi menjanjikan untuk menangani punca utama ketidakselarasan. Pendekatan tersebut termasuk, contohnya, mempelbagaikan persekitaran latihan dan mengesan penjajaran melalui pemantauan anomali (‡737, ‡738, ‡739*). Penyelidik lain menumpukan perhatian pada pemahaman dan pemformalan mekanisme teras dengan lebih baik, seperti generalisasi salah matlamat – contohnya, bagaimana agen mengekalkan keupayaan tetapi mengejar matlamat yang tidak dimaksudkan – bagi memandu reka bentuk latihan dan penilaian yang lebih baik (‡742). Satu lagi arah penyelidikan meneroka cara untuk memisahkan keagenan daripada keupayaan ramalan, sebagai kaedah untuk mewujudkan sistem AI bukan agenik yang boleh dipercayai sejak awal reka bentuknya (‡743). Sistem sedemikian kemudiannya boleh digunakan sebagai lapisan pengawasan tambahan apabila dilaksanakan bersama mekanisme kawalan yang kurang boleh dipercayai terhadap agen AI yang tidak dipercayai.

Penyelidik sedang memajukan kaedah untuk mengesan dan mencegah ketidakselarasan pada peringkat awal proses pembangunan. Usaha ini merangkumi: teknik keboleh tafsiran untuk memeriksa komponen dalaman sistem AI dan mengenal pasti tingkah laku yang membimbangkan (‡744, ‡745, ‡746); penyeliaan berskala (iaitu satu set sistem AI digunakan untuk menyelia sistem AI yang lain (‡747)); dan kaedah penjajaran yang bertujuan memastikan sistem AI terus responsif terhadap penyeliaan manusia (‡748, ‡749).

Penyelidik juga sedang membangunkan mekanisme dan intervensi untuk mengurus sistem AI yang berpotensi tidak sejajar. Ini termasuk: memantau ‘rantaian pemikiran’ yang dihasilkan oleh sistem penaakulan untuk mengesan tanda-tanda ketidakselarasan atau output yang berbahaya (‡430, ‡435, ‡750); membangunkan kes keselamatan yang bertujuan untuk menunjukkan dengan tahap keyakinan yang tinggi bahawa model tidak mungkin menggagalkan langkah-langkah kawalan (‡751); dan menjadikan perlindungan lebih teguh terhadap percubaan untuk melemahkannya (‡725). Namun begitu, bidang ‘kawalan AI’ yang sedang berkembang masih di peringkat awal (‡752, ‡753). Cabaran masa depan bagi rangka kerja penilaian termasuk keperluan untuk memantau sistem AI masa depan yang lebih berkebolehan dan boleh beroperasi untuk tempoh yang lebih lama serta dalam persekitaran yang lebih kompleks.

###@ Cabaran bagi pembuat dasar

Pembuat dasar yang menangani risiko kehilangan kawalan perlu bersedia menghadapi risiko yang kebarangkalian, sifat dan masanya masih tidak pasti. Sistem AI semasa tidak menimbulkan risiko kehilangan kawalan yang serta-merta, tetapi keputusan yang dibuat hari ini akan menentukan sama ada sistem masa depan akan menimbulkannya. Keputusan ini termasuk cara menyokong pembangunan kaedah penilaian dan mitigasi yang boleh dipercayai, serta sama ada perlu ada peraturan tentang akses dan kebenaran yang diberikan kepada sistem AI dalam pelbagai persekitaran. Dalam membuat keputusan ini, pembuat dasar berdepan dengan pertukaran sukar. Contohnya, mengehadkan penggunaan sistem AI dalam persekitaran kritikal mungkin mengurangkan manfaatnya, manakala membenarkan penggunaan secara meluas mungkin meningkatkan risiko jika perlindungan yang disediakan terbukti tidak memadai.

