###@ Apa itu sistem AI serbaguna?

Sistem AI serbaguna adalah program perangkat lunak yang mempelajari pola dari sejumlah besar data, sehingga dapat melakukan beragam tugas, alih-alih dirancang khusus untuk satu fungsi atau ranah tertentu (lihat Tabel 1.1). Untuk membuat sistem ini, pengembang AI menjalankan proses bertahap yang membutuhkan sumber daya komputasi yang besar, kumpulan data yang besar, dan keahlian khusus (lihat Tabel 1.2). Sumber daya komputasi (sering disingkat menjadi ‘komputasi’) diperlukan baik untuk mengembangkan maupun menerapkan sistem AI, dan mencakup cip komputer khusus serta perangkat lunak dan infrastruktur yang dibutuhkan untuk menjalankannya.† Karena dilatih dengan kumpulan data yang besar dan beragam, sistem AI serbaguna dapat melakukan banyak tugas yang berbeda, seperti merangkum teks, menghasilkan gambar, atau menulis kode komputer. Bagian ini menjelaskan cara membuat sistem AI serbaguna, apa yang dimaksud dengan model ‘penalaran’, dan bagaimana keputusan kebijakan membentuk pengembangan sistem AI serbaguna.

    Catatan † -- Istilah ‘komputasi’ juga dapat merujuk pada pengukuran jumlah operasi yang dapat dilakukan prosesor (biasanya diukur dalam operasi titik-mengambang per detik) atau secara khusus pada perangkat keras (seperti unit pemrosesan grafis) yang melakukan operasi tersebut.

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
###@ Generator gambar
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Generator video
- Kosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Robotika dan sistem navigasi
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Prediktor untuk beragam kelas struktur biomolekuler
- AlphaFold 3 (‡27)
- Perkuat (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Agen AI
- AlphaEvolve (‡31*)
- Agen ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Ilmuwan AI-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 1.1: Jenis AI serbaguna
>white|black||9|11|br Ada beberapa jenis AI serbaguna. Dalam Laporan ini, model yang dapat memprediksi informasi struktural untuk beragam kelas molekul dianggap sebagai AI ‘serbaguna’ karena dapat diadaptasi untuk berbagai tugas. Sebagai contoh, model yang dilatih untuk memprediksi struktur protein dapat diterapkan pada berbagai tugas lain, seperti memprediksi interaksi protein, memprediksi lokasi pengikatan molekul kecil, serta memprediksi dan merancang peptida siklik (‡40).


>white|orangered|left|13|15|bb  Pembelajaran mendalam merupakan landasan bagi AI serbaguna.

Peneliti membangun model AI serbaguna menggunakan proses yang disebut ‘pembelajaran mendalam’, yang melatih model agar belajar dari contoh (‡41). Tidak seperti rekayasa perangkat lunak, model pembelajaran mendalam belajar menyelesaikan tugas dari data, alih-alih mengandalkan instruksi yang ditulis secara manual. Dengan memproses data dalam jumlah besar, seperti gambar, teks, atau audio, model-model ini menemukan cara untuk merepresentasikan data tersebut, sehingga menciptakan representasi internal dari pola (seperti bentuk, asosiasi kata, atau struktur suara) yang membantu model mengenali hubungan dan menghasilkan keluaran yang selaras dengan tujuan pelatihannya. Model-model tersebut kemudian menggunakan representasi internal yang telah dipelajari ini sebagai fitur abstrak untuk menganalisis data baru yang serupa dan menghasilkan keluaran dengan gaya yang sama. Sebagai contoh, model AI serbaguna yang dilatih dengan cukup banyak contoh puisi romantik Inggris abad ke-19 dapat mengenali puisi baru dengan gaya tersebut dan menghasilkan materi baru dengan gaya serupa.

Pada tingkat yang lebih terperinci, pembelajaran mendalam bekerja dengan memproses data melalui lapisan-lapisan simpul pemrosesan informasi yang saling terhubung. Simpul-simpul ini sering disebut ‘neuron’ karena terinspirasi secara longgar oleh neuron dalam otak biologis (‘jaringan saraf’) (Gambar 1.1) (‡42). Saat informasi mengalir dari satu lapisan neuron ke lapisan berikutnya, model secara bertahap mengubah data menjadi representasi yang lebih abstraksebagai kelompok fitur yang dipelajari – pola yang ditemukan model secara otomatis dalam data, bukan pola yang dikodekan secara manual. Sebagai contoh, dalam model pemrosesan gambar, lapisan pertama mungkin belajar mendeteksi fitur sederhana seperti tepi atau bentuk dasar, sedangkan lapisan yang lebih dalam menggabungkan fitur-fitur tersebut untuk mengenali pola yang lebih kompleks seperti wajah atau objek.

Fitur pada semua lapisan ditemukan melalui proses optimisasi yang mendefinisikan prosedur pelatihan. Selama pelatihan, ketika model membuat kesalahan, algoritma pembelajaran mendalam menyesuaikan kekuatan berbagai koneksi antar neuron untuk meningkatkan kinerja model. Kekuatan setiap koneksi antar simpul sering disebut ‘bobot’. Pendekatan berlapis ini menjadi asal nama pembelajaran mendalam.

Pembelajaran mendalam terbukti sangat efektif dalam memungkinkan sistem AI menyelesaikan tugas-tugas yang sebelumnya dianggap sulit bagi sistem komputasi tradisional yang diprogram secara manual serta metode AI simbolik atau berbasis aturan yang lebih awal. Sebagian besar model AI serbaguna tercanggih saat ini kini didasarkan pada arsitektur jaringan saraf tertentu yang dikenal sebagai ‘transformer’ (‡43, ‡44). Transformer menggunakan mekanisme ‘attention’ (‡45) yang membantu model berfokus pada bagian paling relevan dari data masukan saat memproses informasi, seperti menentukan kata-kata mana dalam sebuah kalimat yang paling penting untuk memahami maknanya. Cara khusus dalam membangun model ini telah menghasilkan peningkatan signifikan dalam penerjemahan (‡43), pemrosesan bahasa alami (‡46), pengenalan gambar (‡47), dan pengenalan suara (‡48, ‡49), yang pada akhirnya mengarah pada pengembangan model-model tercanggih saat ini.

![fig1.1](images/fig1.1_neural_network.png)

##### Gambar 1.1: Representasi ilustratif dari ‘jaringan saraf’
>white|black||9|11|br Model AI serbaguna saat ini didasarkan pada jaringan ini, yang terinspirasi secara longgar oleh otak biologis. Jaringan yang berbeda memiliki ukuran dan arsitektur yang berbeda. Namun, semuanya terdiri atas unit pemroses informasi yang saling terhubung dan disebut ‘neuron’, sedangkan kekuatan koneksi antar-neuron disebut ‘bobot’. Bobot diperbarui melalui pelatihan menggunakan data dalam jumlah besar. Sumber: International AI Safety Report 2025 (‡50) (dimodifikasi).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Gambar 1.2: Representasi skematis tahapan pengembangan AI tujuan umum
>white|black|left|9|11|br Sumber: Laporan Keselamatan AI Internasional 2026.


>white|orangered|left|13|15|bb AI tujuan umum dikembangkan secara bertahap

Pengembangan sistem AI serbaguna melibatkan beberapa tahap, mulai dari pelatihan model awal hingga pemantauan dan pembaruan setelah penerapan (Gambar 1.2). Dalam praktiknya, langkah-langkah ini sering kali saling tumpang tindih secara iteratif. Setiap tahap memerlukan masukan sumber daya yang berbeda (misalnya, data, tenaga kerja, komputasi) serta teknik yang berbeda, dan terkadang dilaksanakan oleh pengembang yang berbeda (Gambar 1.2 dan Tabel 1.2).

Sebagai contoh, pra-pelatihan model umumnya membutuhkan komputasi dan data dalam jumlah besar, sehingga tahap ini sangat sensitif terhadap kebijakan yang memengaruhi akses ke sumber daya komputasi atau data pelatihan (‡51, ‡52). Demikian pula, kurasi data dan beberapa metode penyetelan halus model saat ini melibatkan banyak tenaga kerja manusia untuk pelabelan data awal (‡53). Oleh karena itu, tahap ini sensitif terhadap perubahan biaya tenaga kerja, kebijakan platform, atau peraturan yang memengaruhi pengaturan kontrak lintas batas.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Pengumpulan dan kurasi data
> 
  Sebelum melatih model AI serbaguna, pengembang dan pekerja data mengumpulkan, membersihkan, mengkurasi, dan menstandarkan data pelatihan mentah ke dalam format yang dapat dipelajari model. Proses ini dapat membutuhkan banyak tenaga kerja. Dataset pelatihan di balik model-model tercanggih terdiri atas jumlah contoh yang sangat besar dari seluruh internet.
  Tim sering mengembangkan metode penyaringan yang canggih untuk mengurangi konten berbahaya, menghilangkan data duplikat, dan meningkatkan keterwakilan berbagai topik dan sumber (‡54, ‡55). Kurasi data juga dapat membantu mengurangi pelanggaran hak cipta dan privasi, menghapus contoh yang berisi pengetahuan berbahaya, menangani berbagai bahasa, dan meningkatkan dokumentasi asal-usul data (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Pra-pelatihan (tahap pertama pelatihan)

  Selama prapelatihan, pengembang memberikan model data beragam dalam jumlah besar untuk menanamkan dasar pengetahuan yang luas dan pemahaman kontekstual. Proses ini menghasilkan ‘model dasar’. Proses ini sangat intensif dalam penggunaan data dan komputasi.

  Selama prapelatihan, model dipaparkan pada miliaran atau triliunan contoh konten seperti gambar, teks, atau audio. Melalui paparan ini, model secara bertahap menemukan fitur abstrak untuk merepresentasikan data dan mempelajari hubungan antarfitur tersebut, sehingga model dapat memahami masukan baru dalam konteksnya. Proses prapelatihan ini berlangsung selama berminggu-minggu atau berbulan-bulan (‡59) dan menggunakan puluhan atau ratusan ribu unit pemrosesan grafis (GPUs) atau unit pemrosesan tensor (TPUs) (‡60) – chip komputer khusus yang dirancang untuk memproses banyak kalkulasi semacam itu dengan cepat. Sebagian pengembang melakukan prapelatihan menggunakan sumber daya komputasi mereka sendiri, sementara yang lain menggunakan sumber daya yang disediakan oleh penyedia komputasi khusus.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Pelatihan lanjutan dan penyetelan halus (tahap kedua pelatihan)

  ‘Pascapelatihan’ semakin menyempurnakan model dasar untuk mengoptimalkannya bagi aplikasi tertentu. Proses ini cukup intensif dari segi komputasi dan sangat padat karya. Peralihan ke penggunaan ‘data sintetis’ – informasi yang dibuat secara artifisial dan meniru data dunia nyata, tetapi dihasilkan menggunakan algoritme atau simulasi – membantu mengurangi kebutuhan tenaga kerja dalam tahap ini.
  Pelatihan pasca mencakup berbagai teknik penyempurnaan dan modifikasi lainnya. ‘Penyempurnaan terawasi’ melibatkan pelatihan lebih lanjut terhadap model yang telah dilatih menggunakan kumpulan data tertentu untuk meningkatkan kinerja model di bidang tersebut (‡61, ‡62). Sebagai contoh, model serbaguna dapat dilatih lebih lanjut menggunakan korpus besar citra radiologi. ‘Pembelajaran penguatan’ (RL) melibatkan peningkatan kinerja model dengan ‘memberi penghargaan’ kepada model (memberikan umpan balik positif) atas keluaran yang diinginkan dan ‘memberi penalti’ kepada model (memberikan umpan balik negatif) atas keluaran yang tidak diinginkan. Pembelajaran ini memiliki dua subkategori utama. ‘Pembelajaran penguatan dari umpan balik manusia’ melibatkan pemberian penghargaan atas keluaran yang selaras dengan preferensi manusia dan pemberian penalti atas keluaran yang tidak selaras, berdasarkan umpan balik manusia (‡63, ‡64*). ‘Pembelajaran penguatan dengan imbalan yang dapat diverifikasi’ (RLVR) digunakan untuk meningkatkan kinerja model pada tugas yang memerlukan kebenaran faktual, seperti matematika atau pembuatan kode. Pengembang biasanya bergantian menerapkan teknik pelatihan pasca dan menjalankan pengujian hingga hasilnya menunjukkan bahwa model memenuhi spesifikasi yang diinginkan.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Integrasi sistem

  Pengembang menggabungkan satu atau lebih model AI serbaguna dengan komponen lain untuk menciptakan ‘sistem AI’ yang siap digunakan. GPT-5 (misalnya) adalah model AI serbaguna yang memproses teks, gambar, dan audio, sedangkan ChatGPT adalah sistem AI serbaguna yang menggabungkan beberapa model dengan ukuran dan kemampuan berbeda dengan antarmuka obrolan, pemrosesan konten, akses Web, dan integrasi aplikasi untuk menciptakan produk fungsional.
  Selain membuat model AI dapat beroperasi, komponen tambahan dalam sistem AI juga bertujuan meningkatkan kemampuan, kegunaan, dan keamanannya. Sebagai contoh, suatu sistem mungkin dilengkapi filter yang mendeteksi dan memblokir masukan atau keluaran model yang mengandung konten berbahaya (‡65*). Pengembang juga semakin banyak menggunakan "scaffolding" – perangkat lunak tambahan yang dibangun di sekitar model AI serbaguna, yang memungkinkan model tersebut merencanakan ke depan, mengejar tujuan, dan berinteraksi dengan dunia (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Deployment dan rilis
  Deployment adalah proses menyediakan sistem AI terintegrasi agar dapat digunakan sesuai tujuan penggunaannya. Pengembang dan pihak yang menerapkan mengimplementasikan sistem AI ke dalam aplikasi, produk, atau layanan di dunia nyata. Pengembang dapat menerapkan sistem AI secara internal (untuk digunakan sendiri) atau secara eksternal (untuk pelanggan privat atau penggunaan publik). Saat menerapkan sistem AI secara eksternal, perusahaan sering kali memberi pengguna akses melalui antarmuka pengguna daring atau antarmuka pemrograman aplikasi (API) yang memungkinkan pengguna mengakses dan menjalankan sistem tersebut. Sebagai contoh, sebuah perusahaan mungkin merancang chatbot layanan pelanggan khusus yang ditenagai oleh sistem AI serbaguna milik perusahaan lain.
  ‘Penerapan sistem AI’ mengacu pada penyediaan model untuk digunakan di dunia nyata dengan alat dan antarmuka terintegrasi, sedangkan ‘perilisan model’ mencakup penyediaan akses kepada pihak lain ke model dasar – baik sebagai model berbobot terbuka (parameter yang dapat diunduh) maupun model berbobot tertutup (hanya akses API). Lihat §3.4. Model berbobot terbuka.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Pemantauan dan pembaruan pascapenerapan

  Pengembang sering mengumpulkan dan menganalisis umpan balik pengguna, melacak metrik dampak dan kinerja, serta melakukan perbaikan secara iteratif untuk mengatasi masalah yang ditemukan dalam penggunaan di dunia nyata (‡67). Perbaikan dilakukan dengan memperbarui integrasi sistem, sering kali melalui penyempurnaan berkelanjutan dan pemberian akses kepada model ke basis data eksternal yang berisi fakta (terkini). Hal ini menjaga model AI besar tetap mutakhir tanpa mengulangi seluruh proses prapelatihan (‡68*). Dengan demikian, kemampuan dapat terakumulasi dari satu putaran pelatihan ke putaran berikutnya, sekaligus menjaga stabilitas dan mengurangi biaya komputasi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Tabel 1.2: Tahapan pengembangan AI serbaguna
>white|black||9|11|br Pada setiap tahap pengembangan AI serbaguna, model AI disempurnakan untuk penggunaan hilir dan pada akhirnya diterapkan sebagai sistem AI yang terintegrasi penuh, dipantau, dan diperbarui.


>white|orangered|left|13|15|bb Sistem penalaran menghasilkan ‘rantai pemikiran’ selama inferensi untuk meningkatkan kinerja.

Inferensi terjadi ketika seseorang menggunakan model AI setelah model tersebut dilatih. Misalnya, inferensi terjadi ketika seseorang meminta sistem AI merencanakan perjalanan dan model di baliknya memanfaatkan aspek-aspek relevan dari hal-hal yang telah dipelajarinya tentang geografi, transportasi, dan kuliner untuk menghasilkan rencana perjalanan.

Dalam dekade terakhir, kemajuan kemampuan AI sebagian besar berasal dari proses pelatihan berskala lebih besar; yaitu, meningkatkan jumlah komputasi yang digunakan untuk melatih model AI. Namun, belakangan ini, para peneliti telah mencapai kemajuan yang lebih besar dengan memungkinkan model memproses informasi lebih lama dan melatihnya untuk menghasilkan langkah-langkah penalaran yang eksplisit saat menyelesaikan suatu tugas (‡69*, ‡70). Sistem AI yang bekerja seperti ini disebut ‘sistem penalaran’, dan penjelasan perantara yang dihasilkan saat sistem tersebut memecahkan masalah atau menjawab pertanyaan disebut ‘rantai pemikiran’. Sistem penalaran memerlukan lebih banyak sumber daya komputasi saat digunakan untuk menghasilkan rantai pemikiran yang canggih ini (‡71, ‡72, ‡73, ‡74), serta lebih banyak sumber daya selama pelatihan agar sistem tersebut belajar bernalar dengan lebih baik. Dalam praktiknya, kemampuan penalaran ini memungkinkan sistem AI memecahkan masalah yang lebih kompleks dengan menguraikan suatu tugas secara berulang menjadi langkah-langkah yang lebih kecil. Tabel 1.3 menunjukkan contoh sistem nonpenalaran dan sistem penalaran yang menyelesaikan masalah yang sama.

Sistem penalaran telah mencapai terobosan besar dalam kemampuannya menangani masalah yang menantang. Sebagai contoh, pada 2025, sistem penalaran yang dikhususkan untuk pemecahan masalah matematika, seperti Gemini Deep Think dari Google dan model eksperimental yang belum dirilis dari OpenAI, menyelesaikan soal-soal Olimpiade Matematika Internasional (dalam pengujian terstruktur) dengan tingkat kinerja setara peraih medali emas manusia (‡75, ‡76). Sistem penalaran telah menunjukkan kemajuan signifikan dalam ranah formal seperti matematika, teka-teki logika, dan pertanyaan ilmiah terstruktur, yang penalaran langkah demi langkahnya dapat diverifikasi secara eksplisit (‡77). Namun, sistem penalaran juga dapat gagal dengan menghasilkan rangkaian pemikiran yang tidak relevan, tidak produktif, atau berulang-ulang (‡78, ‡79).

###@ Pembaruan tentang metode pelatihan

Sejak penerbitan Laporan terakhir (Januari 2025), sebuah metode pelatihan yang disebut ‘distilasi’ telah sangat meningkatkan efisiensi penyetelan-halus beberapa model. Distilasi melibatkan pelatihan model ‘siswa’ dengan keluaran dari model ‘guru’ yang lebih canggih (dan biasanya lebih besar), sehingga model siswa dapat langsung meniru keluaran model guru (‡80). Sebagai contoh, DeepSeek mengembangkan model besar bernama DeepSeek-R1, yang unggul dalam penalaran rantai-pemikiran. R1 menghasilkan keluaran penalaran yang kemudian digunakan untuk menyetel-halus model siswa yang lebih kecil, termasuk DeepSeek-V3. DeepSeek-V3 mempertahankan sebagian besar kemampuan matematis, pemrograman, dan analisis dokumen- dari R1, dan kabarnya disetel- halus dengan biaya sekitar $10,000 USD (meskipun biaya pra-pelatihannya tidak dilaporkan) (‡81). Biaya ini kemungkinan beberapa orde magnitudo lebih rendah daripada biaya penyetelan-halus model yang lebih besar dengan kemampuan serupa.

![table1.3](images/table1.3_example_reasoning.png)

##### Tabel 1.3: Contoh sistem yang tidak melakukan penalaran (kiri) dibandingkan dengan sistem yang melakukan penalaran (kanan)
>white|black||9|11|br Dalam memecahkan teka-teki yang sama, contoh-contoh ini diadaptasi dari respons AI nyata. Sistem penalaran menghabiskan lebih banyak waktu dan daya komputasi untuk “berpikir” dengan menyusun “rantai pemikiran” sebelum memberikan jawaban akhirnya.

![figure.3](images/fig1.3_AI_agent.png)

##### Gambar 1.3: Representasi ilustratif dari agen AI
>white|black||9|11|br Model AI (tengah) yang telah dikonfigurasi untuk merencanakan, melakukan penalaran, dan menggunakan alat secara iteratif guna menyelesaikan tugas-tugas di dunia nyata. Sumber: Laporan Keselamatan AI Internasional 2026.


Dengan demikian, distilasi dapat menjadi cara yang murah dan efisien bagi model untuk memperoleh kemampuan yang lebih canggih (‡82). Sejumlah peneliti telah menggunakan distilasi untuk melakukan penyetelan halus pada model yang sangat cakap dengan hanya menggunakan 1,000 contoh yang dihasilkan dari model state-of- the-art (‡83). Karena distilasi memerlukan model guru yang sudah ada, teknik ini tidak dapat digunakan secara langsung untuk memajukan kemampuan model state-of-the-art. Namun, teknik ini dapat mempercepat penyebaran kemampuan AI canggih, bahkan dari model closed-source (‡84*).

Bersama dengan kemajuan teknologi dalam ‘komputasi terdistribusi’ dan pelatihan terdesentralisasi (pendekatan yang memungkinkan para pengembang menggunakan beberapa prosesor, server, atau pusat data yang bekerja sama untuk melakukan pelatihan atau inferensi AI (‡85, ‡86, ‡87)), tingkat ketergantungan banyak proyek pengembangan AI pada infrastruktur komputasi terpusat berskala besar telah berkurang. Hal ini semakin memungkinkan pihak-pihak yang memiliki sumber daya lebih terbatas untuk mengembangkan dan menerapkan sistem yang canggih.

###@ Pembaruan tentang agen AI

Sejak Laporan terakhir (Januari 2025), kemajuan dalam cara para pengembang menggabungkan model AI dengan alat telah memungkinkan pengembangan agen AI yang semakin canggih. Agen AI dirancang untuk mengejar tujuan, yang sering kali ditentukan oleh pengguna dalam bahasa alami. Untuk mencapai tujuan tersebut, agen diberi akses ke alat, seperti memori, antarmuka komputer, dan peramban web. Alat-alat ini beserta kode yang digunakan untuk menggabungkannya dengan model disebut ‘scaffolding’, dan membantu agen AI berinteraksi secara otonom dengan dunia, menyusun rencana, mengingat detail penting, dan mengejar tujuan (‡88*, ‡89) dengan jauh lebih sedikit pengawasan atau bantuan dari manusia. Sebagai contoh, Manus AI adalah agen AI populer yang dapat mengotomatiskan berbagai tugas, termasuk pencarian web, pengembangan perangkat lunak, dan pembelian daring (‡90). Gambar 1.3 mengilustrasikan contoh sederhana agen AI yang terdiri atas ‘otak’ berupa model AI serbaguna yang dapat secara iteratif menyusun rencana, bernalar, dan menggunakan alat untuk memori, penelusuran web, dan penggunaan komputer.

Infrastruktur digital untuk agen AI terus berkembang (‡91), dan agen AI semakin umum digunakan di berbagai industri (‡92, ‡93, ‡94). Agen AI telah dikembangkan untuk tugas-tugas seperti penelitian (‡37), rekayasa perangkat lunak (‡95), pengendalian robot (‡96), dan layanan pelanggan (‡97). Penelitian dan pengembangan yang berkelanjutan telah menghasilkan agen AI atau sistem multiagen yang semakin mampu dan semakin otonom. Para peneliti memperkirakan bahwa kompleksitas tugas tolok ukur perangkat lunak yang dapat diselesaikan oleh agen AI meningkat dua kali lipat kira-kira setiap tujuh bulan (lihat juga §1.2. Kemampuan saat ini) (‡98). Para ahli berpendapat bahwa agen AI yang semakin mampu akan menghadirkan peluang besar sekaligus risiko (‡99, ‡100*) (lihat §2.2.1. Tantangan keandalan).

###@ Kesenjangan bukti

Kesenjangan bukti utama terkait proses pengembangan sistem AI tujuan- umum bersumber dari kurangnya informasi yang tersedia untuk publik  mengenai cara sistem tersebut dikembangkan. Beberapa pengembang sangat transparan tentang cara mereka mengembangkan sistem AI tujuan umum (‡1, ‡101). Namun, secara umum, pengetahuan publik dan pembuat kebijakan tentang cara sebagian besar model canggih dikembangkan, dilindungi, dievaluasi, dan diterapkan masih terbatas. Hal ini terutama berlaku untuk sistem AI yang diterapkan secara internal dan digunakan di perusahaan AI, tetapi tidak digunakan atau dipahami oleh pemangku kepentingan eksternal (‡102, ‡103). Keterbatasan visibilitas eksternal ini menimbulkan tantangan bagi transparansi dan pengawasan. Berbagai peneliti telah menyoroti transparansi yang terbatas dan tidak konsisten terkait data pelatihan (‡104, ‡105, ‡106), model AI tujuan umum (‡107, ‡108), agen AI (‡92), evaluasi (‡109), alur kerja pengembangan (‡110), dan keselamatan (‡111). Pembatasan pengungkapan kepada pihak eksternal terkadang diperlukan untuk melindungi rahasia dagang dan kekayaan intelektual perusahaan. Pada saat yang sama, transparansi yang rendah semakin mempersulit peneliti independen dan pembuat kebijakan untuk mengkaji model dan sistem AI tujuan umum.


