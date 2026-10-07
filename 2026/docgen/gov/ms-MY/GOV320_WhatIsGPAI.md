###@ Apakah sistem AI serba guna?

Sistem AI tujuan umum ialah program perisian yang mempelajari corak daripada sejumlah besar data, membolehkan sistem tersebut melaksanakan pelbagai tugas dan bukannya dikhususkan untuk satu fungsi atau domain tertentu (lihat Meja 1.1). Untuk mencipta sistem ini, pembangun AI menjalankan proses berbilang peringkat yang memerlukan sumber pengkomputeran yang banyak, set data yang besar dan kepakaran khusus (lihat Meja 1.2). Sumber pengkomputeran (sering dipendekkan kepada ‘compute’) diperlukan untuk membangunkan dan menggunakan sistem AI, serta merangkumi cip komputer khusus dan perisian serta infrastruktur yang diperlukan untuk menjalankannya.† Oleh sebab dilatih menggunakan set data yang besar dan pelbagai, sistem AI tujuan umum dapat melaksanakan pelbagai tugas, seperti meringkaskan teks, menjana imej atau menulis kod komputer. Bahagian ini menerangkan cara sistem AI tujuan umum dicipta, maksud model ‘penaakulan’ dan cara keputusan dasar membentuk pembangunan sistem AI tujuan umum.

    Nota † -- Istilah ‘compute’ juga boleh merujuk sama ada kepada ukuran bilangan pengiraan yang boleh dilakukan oleh pemproses (biasanya diukur dalam operasi titik terapung sesaat) atau khususnya perkakasan (seperti unit pemprosesan grafik) yang melakukan pengiraan tersebut.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistem bahasa
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Perintah A (‡3*)
- EXAONE 4.0 (‡4*)
- Gemini 3 Pro (‡5*)
- GLM-4.5 (‡6*)
- GPT-5(‡7*)
- Hunyuan-Large (‡8*)
- Kimi K2 (‡9*)
- Mistral 3.1 (‡10*)
- Qwen3 (‡11*)
- DeepSeek-V3.2 (‡12*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Penjana imej
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Penjana video
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Sistem robotik dan navigasi
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Peramal bagi pelbagai kelas struktur biomolekul
- AlphaFold 3 (‡27)
- Perkuat (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Ejen AI
- AlphaEvolve (‡31*)
- Ejen ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Saintis AI-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 1.1: Jenis AI Serba Guna
>white|black||9|11|br Terdapat beberapa jenis AI tujuan umum yang berbeza. Dalam Laporan ini, model yang boleh meramalkan maklumat struktur bagi pelbagai kelas molekul dianggap sebagai AI ‘tujuan umum’ kerana model tersebut boleh disesuaikan untuk pelbagai tugas. Contohnya, model yang dilatih untuk meramalkan struktur protein boleh digunakan untuk pelbagai tugas lain, seperti meramalkan interaksi protein, meramalkan tapak pengikatan molekul kecil, serta meramalkan dan mereka bentuk peptida siklik (‡40).


>white|orangered|left|13|15|bb  Pembelajaran mendalam merupakan asas kepada AI serba guna.

Penyelidik membina model AI serba- guna menggunakan proses yang dipanggil ‘pembelajaran mendalam’, yang melatih model untuk belajar daripada contoh (‡41). Tidak seperti kejuruteraan perisian, model pembelajaran mendalam belajar melaksanakan tugas daripada data dan bukannya bergantung pada arahan yang ditulis secara manual. Dengan memproses sejumlah besar data, seperti imej, teks atau audio, model ini menemui cara untuk mewakili data tersebut, lalu menghasilkan perwakilan dalaman bagi corak (seperti bentuk, perkaitan perkataan atau struktur bunyi) yang membantu model mengenali hubungan dan menjana output yang selaras dengan objektif latihannya. Model ini kemudian menggunakan perwakilan dalaman yang telah dipelajari sebagai ciri abstrak untuk menganalisis data baharu yang serupa dan menjana output dalam gaya yang sama. Contohnya, model AI serba- guna yang dilatih dengan contoh puisi romantik Inggeris abad ke-19 yang mencukupi dapat mengenali puisi baharu dalam gaya tersebut dan menghasilkan bahan baharu dengan gaya yang serupa.

Pada tahap yang lebih terperinci, pembelajaran mendalam berfungsi dengan memproses data melalui lapisan nod pemprosesan maklumat yang saling berhubung. Nod ini sering dipanggil ‘neuron’ kerana diinspirasikan secara longgar oleh neuron dalam otak biologi (‘rangkaian neural’) (Angka 1.1) (‡42). Apabila maklumat mengalir dari satu lapisan neuron ke lapisan seterusnya, model secara beransur-ansur mengubah data menjadi perwakilan yang lebih abstraksebagai kumpulan ciri yang dipelajari – corak yang ditemui secara automatik oleh model dalam data, bukannya corak yang dikodkan secara manual. Contohnya, dalam model pemprosesan imej, lapisan pertama mungkin belajar mengesan ciri mudah seperti tepi atau bentuk asas, manakala lapisan yang lebih dalam menggabungkan ciri ini untuk mengenal pasti corak yang lebih kompleks seperti wajah atau objek.

Ciri-ciri pada semua lapisan dikenal pasti melalui proses pengoptimuman yang mentakrifkan prosedur latihan. Semasa latihan, apabila model membuat kesilapan, algoritma pembelajaran mendalam melaraskan kekuatan pelbagai hubungan antara neuron untuk meningkatkan prestasi model. Kekuatan setiap hubungan antara nod sering dipanggil ‘pemberat’. Pendekatan berlapis ini memberikan nama pembelajaran mendalam.

Pembelajaran mendalam terbukti sangat berkesan dalam membolehkan sistem AI melaksanakan tugas yang sebelum ini dianggap sukar bagi sistem pengkomputeran tradisional yang diprogramkan secara manual dan kaedah AI simbolik atau berasaskan peraturan yang lebih awal. Kebanyakan model AI serba guna yang tercanggih kini berasaskan seni bina rangkaian neural khusus yang dikenali sebagai ‘transformer’ (‡43, ‡44). Transformer menggunakan mekanisme ‘perhatian’ (‡45) yang membantu model menumpukan perhatian pada bahagian data input yang paling relevan semasa memproses maklumat, seperti menentukan perkataan yang paling penting dalam sesuatu ayat untuk memahami maknanya. Cara khusus untuk membina model ini telah membawa kepada peningkatan yang ketara dalam penterjemahan (‡43), pemprosesan bahasa semula jadi (‡46), pengecaman imej (‡47) dan pengecaman pertuturan (‡48, ‡49), yang akhirnya membawa kepada pembangunan model tercanggih masa kini.

![fig1.1](images/fig1.1_neural_network.png)

##### Angka 1.1: Perwakilan ilustrasi bagi ‘rangkaian neural’
>white|black||9|11|br Model AI tujuan umum hari ini berasaskan rangkaian ini, yang diinspirasikan secara longgar oleh otak biologi. Rangkaian yang berbeza mempunyai saiz dan seni bina yang berbeza. Walau bagaimanapun, semuanya terdiri daripada unit pemprosesan maklumat yang saling berhubung, yang dipanggil ‘neuron’, manakala kekuatan hubungan antara neuron dipanggil ‘pemberat’. Pemberat dikemas kini melalui latihan menggunakan data dalam kuantiti yang besar. Sumber: Laporan Keselamatan AI Antarabangsa 2025 (‡50) (diubah suai).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Angka 1.2: Perwakilan skematik peringkat pembangunan AI tujuan umum
>white|black|left|9|11|br Sumber: Laporan Keselamatan AI Antarabangsa 2026.


>white|orangered|left|13|15|bb  AI tujuan umum dibangunkan secara berperingkat

Pembangunan sistem AI tujuan umum melibatkan pelbagai peringkat, daripada latihan model awal hingga pemantauan dan kemas kini selepas penggunaan (Angka 1.2). Dalam amalan, langkah-langkah ini sering bertindih secara berulang. Setiap peringkat memerlukan input sumber yang berbeza (cth. data, tenaga kerja, kuasa pengkomputeran) dan teknik yang berbeza, dan kadangkala dijalankan oleh pembangun yang berlainan (Angka 1.2 dan Meja 1.2).

Sebagai contoh, pralatihan model secara amnya memerlukan sumber pengkomputeran dan data yang banyak, menjadikan peringkat ini amat sensitif terhadap dasar yang menjejaskan akses kepada sumber pengkomputeran atau data latihan (‡51, ‡52). Begitu juga, penyusunan data dan beberapa kaedah penalaan halus model pada masa ini melibatkan penggunaan tenaga kerja manusia yang banyak untuk pelabelan data awal (‡53). Oleh itu, peringkat ini sensitif terhadap perubahan kos buruh, dasar platform atau peraturan yang menjejaskan aturan kontrak rentas sempadan.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Pengumpulan dan kurasi data
> 
  Sebelum melatih model AI serba guna, pembangun dan pekerja data mengumpul, membersihkan, memilih dan menyeragamkan data latihan mentah kepada format yang boleh dipelajari oleh model. Proses ini boleh memerlukan banyak tenaga kerja. Set data latihan di sebalik model tercanggih mengandungi sejumlah besar contoh daripada seluruh internet.
  Pasukan sering membangunkan kaedah penapisan yang canggih untuk mengurangkan kandungan berbahaya, menghapuskan data pendua dan menambah baik perwakilan merentas pelbagai topik dan sumber (‡54, ‡55). Kurasi data juga dapat membantu mengurangkan pelanggaran hak cipta dan privasi, mengalih keluar contoh yang mengandungi pengetahuan berbahaya, mengendalikan berbilang bahasa dan menambah baik dokumentasi asal-usul data (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Prap latihan (peringkat pertama latihan)

  Semasa latihan awal, pembangun membekalkan model dengan sejumlah besar data yang pelbagai untuk membina asas maklumat dan pemahaman kontekstual yang luas. Proses ini menghasilkan ‘model asas’. Proses ini memerlukan sumber data dan pengkomputeran yang sangat besar.

  Semasa pra-latihan, model didedahkan kepada berbilion-bilion atau trilion contoh kandungan seperti gambar, teks atau audio. Melalui pendedahan ini, model secara beransur-ansur menemui ciri abstrak untuk mewakili data dan mempelajari hubungan antara ciri-ciri ini, yang membolehkannya memahami input baharu dalam konteks. Proses pra-latihan ini mengambil masa berminggu-minggu atau berbulan-bulan (‡59) dan menggunakan puluhan ribu atau ratusan ribu unit pemprosesan grafik (GPU) atau unit pemprosesan tensor (TPU) (‡60) – cip komputer khusus yang direka untuk memproses banyak pengiraan sedemikian dengan pantas. Sesetengah pembangun menjalankan pra-latihan menggunakan sumber pengkomputeran mereka sendiri, manakala yang lain menggunakan sumber yang disediakan oleh penyedia pengkomputeran khusus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Latihan pasca dan penalaan halus (peringkat kedua latihan)

  ‘Latihan pasca’ memperhalus model asas dengan lebih lanjut untuk mengoptimumkannya bagi aplikasi tertentu. Proses ini memerlukan tahap pengkomputeran yang sederhana tinggi dan tenaga kerja yang banyak. Peralihan kepada penggunaan ‘data sintetik’ – maklumat yang dijana secara buatan dan meniru data dunia sebenar, tetapi dicipta menggunakan algoritma atau simulasi – membantu mengurangkan keperluan tenaga kerja dalam fasa ini.
  Pascapelatihan merangkumi pelbagai teknik penalaan halus dan pengubahsuaian lain. ‘Penalaan halus terselia’ melibatkan latihan lanjut terhadap model terlatih menggunakan set data khusus untuk meningkatkan prestasi model dalam domain tersebut (‡61, ‡62). Contohnya, model serba guna boleh dilatih lanjut menggunakan korpus besar imej radiologi. ‘Pembelajaran pengukuhan’ (RL) melibatkan peningkatan prestasi model dengan ‘memberikan ganjaran’ kepada model (memberikan maklum balas positif) untuk output yang diingini dan ‘mengenakan penalti’ kepada model (memberikan maklum balas negatif) untuk output yang tidak diingini. Pembelajaran ini mempunyai dua subkategori utama. ‘Pembelajaran pengukuhan daripada maklum balas manusia’ melibatkan pemberian ganjaran kepada output yang selaras dengan keutamaan manusia dan mengenakan penalti kepada output yang tidak selaras dengannya, berdasarkan maklum balas manusia (‡63, ‡64*). ‘Pembelajaran pengukuhan dengan ganjaran yang boleh disahkan’ (RLVR) digunakan untuk meningkatkan prestasi model bagi tugasan yang memerlukan ketepatan fakta, seperti matematik atau penjanaan kod. Pembangun biasanya berselang-seli antara penggunaan teknik pascapelatihan dengan pelaksanaan ujian sehingga hasilnya menunjukkan bahawa model memenuhi spesifikasi yang dikehendaki.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integrasi sistem

  Pembangun menggabungkan satu atau lebih model AI serba guna dengan komponen lain untuk mewujudkan ‘sistem AI’ yang sedia digunakan. GPT-5 (sebagai contoh) ialah model AI serba guna yang memproses teks, imej dan audio, manakala ChatGPT ialah sistem AI serba guna yang menggabungkan beberapa model dengan saiz dan keupayaan yang berbeza dengan antara muka sembang, pemprosesan kandungan, akses Web dan penyepaduan aplikasi untuk menghasilkan produk yang berfungsi.
  Selain menjadikan model AI beroperasi, komponen tambahan dalam sistem AI juga bertujuan meningkatkan keupayaan, kegunaan dan keselamatan. Contohnya, sesebuah sistem mungkin dilengkapi penapis yang mengesan dan menyekat input atau output model yang mengandungi kandungan berbahaya (‡65*). Pembangun juga semakin kerap menggunakan ‘perancah’ – perisian tambahan yang dibina di sekeliling model AI tujuan umum untuk membolehkannya merancang lebih awal, mencapai matlamat dan berinteraksi dengan dunia (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Pelaksanaan dan keluaran
  Pelaksanaan ialah proses menjadikan sistem AI bersepadu tersedia untuk kegunaan yang dimaksudkan. Pembangun dan pihak yang melaksanakan sistem AI menerapkannya dalam aplikasi, produk atau perkhidmatan dunia sebenar. Pembangun boleh melaksanakan sistem AI secara dalaman (untuk kegunaan mereka sendiri) atau secara luaran (untuk pelanggan persendirian atau kegunaan awam). Apabila melaksanakan sistem AI secara luaran, syarikat sering menyediakan akses kepada pengguna melalui antara muka pengguna dalam talian atau antara muka pengaturcaraan aplikasi (API) yang membolehkan pengguna mengakses dan menjalankan sistem tersebut. Sebagai contoh, sebuah syarikat mungkin mereka bentuk chatbot khidmat pelanggan tersuai yang dikuasakan oleh sistem AI tujuan umum milik syarikat lain.
  ‘Pelaksanaan sistem AI’ merujuk kepada penyediaan model untuk kegunaan dunia sebenar dengan alat dan antara muka yang disepadukan, manakala ‘pengeluaran model’ melibatkan penyediaan model asas kepada pihak lain – sama ada sebagai model dengan pemberat terbuka (parameter yang boleh dimuat turun) atau model dengan pemberat tertutup (akses API sahaja). Lihat §3.4. Model dengan pemberat terbuka.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Pemantauan dan kemas kini selepas pelaksanaan

  Pembangun sering mengumpulkan dan menganalisis maklum balas pengguna, menjejaki metrik impak dan prestasi, serta membuat penambahbaikan secara berulang untuk menangani isu yang ditemui semasa penggunaan di dunia sebenar (‡67). Penambahbaikan dilakukan dengan mengemas kini integrasi sistem, selalunya melalui penalaan halus berterusan dan dengan memberikan model akses kepada pangkalan data luaran yang mengandungi fakta (terkini). Langkah ini memastikan model AI yang besar sentiasa terkini tanpa mengulangi keseluruhan proses pralatihan (‡68*). Ini membolehkan keupayaan terkumpul melalui pusingan latihan berturut-turut sambil mengekalkan kestabilan dan mengurangkan kos pengiraan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Meja 1.2: Peringkat pembangunan AI tujuan umum
>white|black||9|11|br Pada setiap peringkat pembangunan AI tujuan umum, model AI ditambah baik untuk kegunaan hiliran dan akhirnya digunakan sebagai sistem AI bersepadu sepenuhnya yang dipantau dan dikemas kini.


>white|orangered|left|13|15|bb Sistem penaakulan menjana ‘rantaian pemikiran’ semasa inferens untuk meningkatkan prestasi.

Inferens berlaku apabila seseorang menggunakan model AI selepas model itu dilatih. Contohnya, inferens berlaku apabila seseorang meminta sistem AI merancang perjalanan dan model yang mendasarinya memanfaatkan aspek berkaitan yang telah dipelajarinya tentang geografi, pengangkutan dan masakan untuk menghasilkan jadual perjalanan.

Dalam dekad yang lalu, kemajuan keupayaan AI sebahagian besarnya berpunca daripada latihan berskala lebih besar; iaitu, peningkatan jumlah pengiraan yang digunakan untuk melatih model AI. Namun, baru-baru ini, penyelidik telah mencapai lebih banyak kemajuan dengan membolehkan model memproses maklumat untuk tempoh yang lebih lama dan melatihnya untuk menghasilkan langkah penaakulan yang jelas semasa melaksanakan sesuatu tugas (‡69*, ‡70). Sistem AI yang berfungsi dengan cara ini dipanggil ‘sistem penaakulan’, manakala penjelasan perantaraan yang dihasilkan semasa menyelesaikan masalah atau menjawab soalan dipanggil ‘rantaian pemikiran’. Sistem penaakulan memerlukan lebih banyak sumber pengkomputeran semasa digunakan untuk menjana rantaian pemikiran yang canggih ini (‡71, ‡72, ‡73, ‡74), serta lebih banyak sumber semasa latihan agar sistem ini belajar membuat penaakulan dengan lebih baik. Dalam amalan, keupayaan penaakulan ini membolehkan sistem AI menyelesaikan masalah yang lebih kompleks dengan menguraikan sesuatu tugas secara berulang kepada langkah-langkah yang lebih kecil. Meja 1.3 menunjukkan contoh sistem tanpa penaakulan dan sistem penaakulan yang menyelesaikan masalah yang sama.

Sistem penaakulan telah mencapai kemajuan besar dalam keupayaan menangani masalah yang mencabar. Sebagai contoh, pada 2025, sistem penaakulan yang dikhususkan untuk menyelesaikan masalah matematik, seperti Gemini Deep Think daripada Google dan model eksperimental yang belum dikeluarkan daripada OpenAI, menyelesaikan masalah Olimpik Matematik Antarabangsa (dalam tetapan ujian berstruktur) pada tahap yang setara dengan prestasi manusia yang memenangi pingat emas (‡75, ‡76). Sistem penaakulan telah menunjukkan kemajuan yang ketara dalam bidang formal seperti matematik, teka-teki logik dan soalan sains berstruktur, yang membolehkan penaakulan langkah demi langkah disahkan secara jelas (‡77). Walau bagaimanapun, sistem penaakulan juga boleh gagal dengan menghasilkan rantaian pemikiran yang tidak relevan, tidak produktif atau berulang-ulang (‡78, ‡79).

###@ Kemas kini tentang kaedah latihan

Sejak penerbitan Laporan terakhir (Januari 2025), kaedah latihan yang dipanggil ‘penyulingan’ telah meningkatkan kecekapan dengan ketara untuk memperhalus sesetengah model melalui penalaan halus. Penyulingan melibatkan latihan model ‘pelajar’ menggunakan output model ‘guru’ yang lebih berkuasa (dan biasanya lebih besar), sekali gus membolehkan model pelajar meniru output model guru secara langsung (‡80). Contohnya, DeepSeek membangunkan model besar yang dipanggil DeepSeek-R1, yang cemerlang dalam penaakulan rantaian pemikiran. R1 menghasilkan output penaakulan yang kemudiannya digunakan untuk memperhalus model pelajar yang lebih kecil, termasuk DeepSeek-V3. DeepSeek-V3 mengekalkan sebahagian besar keupayaan matematik, pengekodan dan analisis- dokumen R1, dan dilaporkan telah melalui penalaan- halus dengan kos kira-kira $10,000 USD (walaupun kos pra-latihannya tidak dilaporkan) (‡81). Kos ini berkemungkinan beberapa magnitud lebih rendah berbanding kos penalaan halus model yang lebih besar dengan keupayaan setanding.

![table1.3](images/table1.3_example_reasoning.png)

##### Meja 1.3: Contoh sistem tanpa penaakulan (kiri) berbanding sistem penaakulan (kanan)
>white|black||9|11|br Semasa menyelesaikan teka-teki yang sama, contoh-contoh ini diadaptasi daripada respons AI sebenar. Sistem penaakulan meluangkan lebih banyak masa dan kuasa pengkomputeran untuk ‘berfikir’ dengan membina ‘rantaian pemikiran’ sebelum memberikan jawapan akhirnya.

![figure.3](images/fig1.3_AI_agent.png)

##### Angka 1.3: Perwakilan ilustrasi bagi ejen AI
>white|black||9|11|br Model AI (tengah) yang telah dikonfigurasikan untuk merancang, menaakul dan menggunakan alat secara berulang bagi menyelesaikan tugasan dunia sebenar. Sumber: Laporan Keselamatan AI Antarabangsa 2026.


Oleh itu, penyulingan boleh menjadi cara yang murah dan cekap untuk membolehkan model memperoleh keupayaan yang lebih berkuasa (‡82). Sesetengah penyelidik telah menggunakan penyulingan untuk melakukan penalaan-halus terhadap model berkeupayaan tinggi dengan hanya 1,000 contoh yang dijana daripada model state-of- the-art (‡83). Oleh sebab penyulingan memerlukan model guru sedia ada, kaedah ini tidak boleh digunakan secara langsung untuk memajukan keupayaan model tercanggih. Walau bagaimanapun, kaedah ini boleh mempercepat penyebaran keupayaan AI termaju, malah daripada model sumber-tertutup (‡84*).

Bersama-sama dengan kemajuan teknologi dalam ‘pengkomputeran teragih’ dan latihan terdesentralisasi (pendekatan yang membolehkan pembangun menggunakan berbilang pemproses, pelayan atau pusat data yang bekerjasama untuk melaksanakan latihan atau inferens AI (‡85, ‡86, ‡87)), tahap kebergantungan banyak projek pembangunan AI pada infrastruktur pengkomputeran terpusat berskala besar telah berkurangan. Hal ini semakin membolehkan pihak yang mempunyai sumber lebih terhad membangunkan dan menggunakan sistem yang berkuasa.

###@ Kemas kini tentang ejen AI

Sejak Laporan terakhir (Januari 2025), kemajuan dalam cara pembangun menggabungkan model AI dengan alat telah membolehkan pembangunan ejen AI yang semakin berkuasa. Ejen AI direka untuk mencapai matlamat, yang sering dinyatakan oleh pengguna dalam bahasa semula jadi. Untuk mencapai matlamat ini, ejen tersebut diberikan akses kepada alat seperti memori, antara muka komputer dan pelayar web. Alat-alat ini serta kod yang digunakan untuk menggabungkannya dengan model dirujuk sebagai ‘perancah’, dan alat serta kod ini membantu ejen AI berinteraksi dengan dunia secara autonomi, membuat rancangan, mengingati butiran penting dan mencapai matlamat (‡88*, ‡89) dengan pengawasan atau bantuan manusia yang jauh lebih sedikit. Sebagai contoh, Manus AI ialah ejen AI popular yang boleh mengautomasikan pelbagai tugas, termasuk carian web, pembangunan perisian dan pembelian dalam talian (‡90). Angka 1.3 menggambarkan contoh mudah ejen AI yang terdiri daripada ‘otak’ model AI serba guna yang boleh merancang, menaakul dan menggunakan alat untuk memori, pelayaran web dan penggunaan komputer secara berulang.

Infrastruktur digital untuk ejen AI sedang berkembang (‡91), dan ejen AI semakin lazim merentas industri (‡92, ‡93, ‡94). Ejen AI telah dibangunkan untuk tugas seperti penyelidikan (‡37), kejuruteraan perisian (‡95), kawalan robotik (‡96) dan khidmat pelanggan (‡97). Penyelidikan dan pembangunan yang berterusan telah menghasilkan ejen AI atau sistem berbilang ejen yang semakin berkemampuan dan semakin autonomi. Para penyelidik menganggarkan bahawa kerumitan tugas penanda aras perisian yang mampu dilaksanakan oleh ejen AI meningkat dua kali ganda kira-kira setiap tujuh bulan (lihat juga §1.2. Keupayaan semasa) (‡98). Pakar berpendapat bahawa ejen AI yang semakin berkemampuan akan membawa kepada peluang besar serta risiko (‡99, ‡100*) (lihat §2.2.1. Cabaran kebolehpercayaan).

###@ Jurang bukti

Jurang bukti utama berkaitan proses pembangunan sistem AI tujuan- umum berpunca daripada kekurangan maklumat yang tersedia kepada umum tentang cara sistem tersebut dibangunkan. Sesetengah pembangun sangat telus tentang cara mereka membangunkan sistem AI tujuan umum (‡1, ‡101). Walau bagaimanapun, secara umum, pengetahuan orang awam dan pembuat dasar tentang cara kebanyakan model canggih dibangunkan, dilindungi, dinilai dan digunakan adalah terhad. Hal ini khususnya berlaku bagi sistem AI yang digunakan secara dalaman dalam syarikat AI tetapi tidak digunakan atau difahami oleh pihak berkepentingan luar (‡102, ‡103). Keterlihatan luaran yang terhad ini menimbulkan cabaran kepada ketelusan dan pengawasan. Pelbagai penyelidik telah menunjukkan bahawa ketelusan tentang data latihan (‡104, ‡105, ‡106), model AI tujuan umum (‡107, ‡108), ejen AI (‡92), penilaian (‡109), saluran paip pembangunan (‡110) dan keselamatan (‡111) adalah terhad dan tidak konsisten. Pendedahan luaran yang terhad kadangkala diperlukan untuk melindungi rahsia perdagangan dan harta intelek syarikat. Pada masa yang sama, ketelusan yang rendah menyukarkan penyelidik bebas dan pembuat dasar untuk mengkaji model dan sistem AI tujuan umum.


