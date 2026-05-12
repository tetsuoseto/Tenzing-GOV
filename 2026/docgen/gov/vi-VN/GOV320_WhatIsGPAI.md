###@ Các hệ thống AI đa mục đích là gì?

Các hệ thống AI mục đích chung là các chương trình phần mềm học các mẫu từ lượng dữ liệu lớn, cho phép chúng thực hiện nhiều loại tác vụ thay vì được chuyên biệt cho chỉ một chức năng hoặc một lĩnh vực cụ thể (xem Bàn 1.1). Để tạo ra các hệ thống này, các nhà phát triển AI thực hiện một quy trình nhiều giai đoạn đòi hỏi nguồn lực tính toán đáng kể, các bộ dữ liệu lớn và chuyên môn chuyên biệt (xem Bàn 1.2). Nguồn lực tính toán (thường được rút gọn thành “compute”) là cần thiết cả để phát triển và triển khai các hệ thống AI, và bao gồm các chip máy tính chuyên dụng cũng như phần mềm và hạ tầng cần thiết để chạy chúng.† Do được huấn luyện trên các bộ dữ liệu lớn, đa dạng, các hệ thống AI mục đích chung có thể thực hiện nhiều tác vụ khác nhau, chẳng hạn như tóm tắt văn bản, tạo ảnh, hoặc viết mã máy tính. Phần này giải thích cách các hệ thống AI mục đích chung được tạo ra, các mô hình “reasoning” là gì, và các quyết định về chính sách định hình việc phát triển hệ thống AI mục đích chung như thế nào.

    Ghi chú † -- Thuật ngữ ‘compute’ cũng có thể đề cập đến một phép đo số lượng phép tính mà một bộ xử lý có thể thực hiện (thường được đo bằng phép toán dấu phẩy động trên giây) hoặc cụ thể là phần cứng (chẳng hạn như bộ xử lý đồ họa) thực hiện các phép tính đó.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Hệ thống ngôn ngữ
- Apertus (‡1)
- Claude Sonnet 4.5 (‡2*)
- Lệnh A (‡3*)
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
###@ Trình tạo hình ảnh
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Bộ tạo video
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Hệ thống robot và định vị
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Các yếu tố dự báo cho các lớp đa dạng của cấu trúc phân tử sinh học
- AlphaFold 3 (‡27)
- Tăng cường (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ tác nhân AI
- AlphaEvolve (‡31*)
- Tác nhân ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- Nhà khoa học AI-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 1.1: Các loại AI đa mục đích
>white|black||9|11|br Có nhiều loại AI đa dụng khác nhau. Trong Báo cáo này, các mô hình có thể dự đoán thông tin cấu trúc cho nhiều lớp phân tử khác nhau được xem là ‘AI đa dụng’ vì chúng có thể được điều chỉnh cho nhiều nhiệm vụ khác nhau. Ví dụ, các mô hình được huấn luyện để dự đoán cấu trúc protein có thể áp dụng cho nhiều nhiệm vụ khác, chẳng hạn như dự đoán tương tác protein, dự đoán các vị trí gắn kết phân tử nhỏ, và dự đoán và thiết kế peptide vòng (‡40).


>white|orangered|left|13|15|bb Học sâu là nền tảng cho trí tuệ nhân tạo đa mục đích

Các nhà nghiên cứu xây dựng các mô hình AI đa dụng bằng một quy trình gọi là ‘deep learning’ (học sâu), huấn luyện mô hình để học từ các ví dụ (‡41). Khác với kỹ thuật phần mềm, các mô hình học sâu học cách thực hiện các tác vụ từ dữ liệu thay vì dựa vào các chỉ dẫn viết tay. Bằng cách xử lý một lượng lớn dữ liệu, chẳng hạn như hình ảnh, văn bản hoặc âm thanh, các mô hình này khám phá các cách biểu diễn dữ liệu đó, tạo ra các biểu diễn nội bộ của các mẫu (như hình dạng, liên kết từ ngữ hoặc cấu trúc âm thanh) giúp mô hình nhận ra các mối quan hệ và tạo ra các đầu ra phù hợp với mục tiêu huấn luyện của nó. Sau đó, chúng sử dụng các biểu diễn nội bộ đã học được như các đặc trưng trừu tượng để phân tích dữ liệu mới, tương tự và tạo ra đầu ra theo cùng phong cách. Ví dụ, một mô hình AI đa dụng được huấn luyện trên đủ các ví dụ về thơ lãng mạn tiếng Anh thế kỷ 19 có thể nhận ra các bài thơ mới theo phong cách đó và tạo ra chất liệu mới theo phong cách tương tự.

Ở mức độ chi tiết hơn, học sâu hoạt động bằng cách xử lý dữ liệu thông qua nhiều lớp các nút xử lý thông tin được liên kết với nhau. Các nút này thường được gọi là ‘neuron’ vì chúng được lấy cảm hứng một cách lỏng lẻo từ các neuron trong bộ não sinh học (‘mạng lưới thần kinh’) (Nhân vật 1.1) (‡42). Khi thông tin chảy từ một lớp neuron sang lớp tiếp theo, mô hình sẽ dần dần biến đổi dữ liệu thành các biểu diễn trừu tượng hơn dưới dạng các nhóm đặc trưng đã được học - những mẫu mà mô hình tự động phát hiện trong dữ liệu, thay vì các mẫu được mã hóa thủ công. Ví dụ, trong một mô hình xử lý hình ảnh, các lớp đầu tiên có thể học cách phát hiện các đặc trưng đơn giản như cạnh hoặc các hình dạng cơ bản, trong khi các lớp sâu hơn sẽ kết hợp các đặc trưng này để nhận diện các mẫu phức tạp hơn như khuôn mặt hoặc các đối tượng.

Các đặc trưng ở tất cả các lớp được khám phá thông qua quá trình tối ưu hóa xác định quy trình huấn luyện. Trong quá trình huấn luyện, khi mô hình mắc lỗi, các thuật toán học sâu sẽ điều chỉnh cường độ của nhiều kết nối khác nhau giữa các nơ-ron để cải thiện hiệu năng của mô hình. Cường độ của từng kết nối giữa các nút thường được gọi là ‘weight’ (trọng số). Cách tiếp cận theo từng lớp này chính là lý do học sâu có tên gọi như vậy.

Học sâu đã chứng minh rất hiệu quả trong việc cho phép các hệ thống AI thực hiện các tác vụ trước đây được xem là khó đối với các hệ thống tính toán truyền thống được lập trình thủ công và các phương pháp AI biểu tượng hoặc dựa trên luật trước đó. Hầu hết các mô hình AI đa dụng trình độ hiện đại ngày nay đều dựa trên một kiến trúc mạng nơ-ron cụ thể được gọi là ‘transformer’ (‡43, ‡44). Transformers sử dụng cơ chế ‘attention’ (‡45) giúp mô hình tập trung vào những phần liên quan nhất của dữ liệu đầu vào khi xử lý thông tin, chẳng hạn như xác định những từ nào trong một câu quan trọng nhất để hiểu ý nghĩa của nó. Cách xây dựng mô hình đặc biệt này đã dẫn đến những cải tiến đáng kể trong dịch thuật (‡43), xử lý ngôn ngữ tự nhiên (‡46), nhận diện hình ảnh (‡47) và nhận diện giọng nói (‡48, ‡49), cuối cùng dẫn đến việc phát triển các mô hình tiên tiến nhất hiện nay.

![fig1.1](images/fig1.1_neural_network.png)

##### Nhân vật vật 1.1: Một biểu diễn minh họa của ‘mạng lưới thần kinh’
>white|black||9|11|br Các mô hình AI đa mục đích hiện nay được xây dựng dựa trên các mạng này, vốn được lấy cảm hứng một cách lỏng lẻo từ bộ não sinh học. Các mạng khác nhau có kích thước và kiến trúc khác nhau. Tuy nhiên, tất cả đều được cấu thành từ các đơn vị xử lý thông tin được kết nối với nhau, gọi là ‘neuron’ (nơ-ron), trong đó mức độ mạnh của các liên kết giữa các neuron được gọi là ‘weights’ (trọng số). Trọng số được cập nhật thông qua quá trình huấn luyện với lượng dữ liệu lớn. Nguồn: International AI Safety Report 2025 (‡50) (đã chỉnh sửa).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Nhân vật vật 1.2: Sơ đồ minh họa các giai đoạn phát triển trí tuệ nhân tạo đa mục đích
>white|black|left|9|11|br Báo cáo An toàn AI Quốc tế 2026.


>white|orangered|left|13|15|bb Trí tuệ nhân tạo đa mục đích được phát triển theo từng giai đoạn

Việc phát triển một hệ thống AI đa năng đòi hỏi nhiều giai đoạn, từ huấn luyện mô hình ban đầu đến giám sát sau khi triển khai và cập nhật (Nhân vật 1.2). Trên thực tế, các bước này thường chồng lấn và được thực hiện theo cách lặp lại. Mỗi giai đoạn yêu cầu các nguồn lực khác nhau (ví dụ: dữ liệu, nhân công, tài nguyên tính toán) và các kỹ thuật khác nhau, đồng thời đôi khi được thực hiện bởi những nhà phát triển khác nhau (Nhân vật 1.2 và Bàn 1.2).

Ví dụ, giai đoạn tiền huấn luyện mô hình nhìn chung đòi hỏi một lượng lớn tài nguyên tính toán và dữ liệu, do đó giai đoạn này đặc biệt nhạy cảm với các chính sách ảnh hưởng đến việc tiếp cận tài nguyên tính toán hoặc dữ liệu huấn luyện (‡51, ‡52). Tương tự, việc chọn lọc/chuẩn bị dữ liệu và một số phương pháp tinh chỉnh mô hình hiện nay có liên quan đến một lượng lớn lao động con người cho việc gán nhãn dữ liệu ban đầu (‡53). Vì vậy, giai đoạn này nhạy cảm với các thay đổi về chi phí lao động, chính sách nền tảng hoặc các quy định ảnh hưởng đến các thỏa thuận ký kết hợp đồng xuyên biên giới.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Thu thập và chuẩn hóa dữ liệu
> 
  Trước khi huấn luyện một mô hình AI đa mục đích, các nhà phát triển và nhân sự dữ liệu thu thập, làm sạch, tuyển chọn (curate) và chuẩn hoá (standardise) dữ liệu huấn luyện thô thành một định dạng mà mô hình có thể học từ đó. Đây có thể là một quy trình tốn nhiều công sức. Các bộ dữ liệu huấn luyện đứng sau các mô hình tiên tiến nhất (state-of-the-art) bao gồm một số lượng cực lớn các ví dụ từ khắp nơi trên internet.
  Các nhóm thường phát triển các phương pháp lọc phức tạp để giảm nội dung có hại, loại bỏ dữ liệu trùng lặp và cải thiện mức độ đại diện giữa các chủ đề và nguồn khác nhau (‡54, ‡55). Việc tinh tuyển dữ liệu cũng có thể giúp giảm vi phạm bản quyền và quyền riêng tư, loại bỏ các ví dụ chứa tri thức nguy hiểm, xử lý nhiều ngôn ngữ và cải thiện tài liệu hóa cho việc truy xuất nguồn gốc dữ liệu (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Huấn luyện trước (giai đoạn đầu của huấn luyện)

  Trong giai đoạn tiền huấn luyện, các nhà phát triển nạp cho mô hình một lượng lớn dữ liệu đa dạng để tạo nền tảng kiến thức rộng và khả năng hiểu ngữ cảnh. Quá trình này tạo ra một “mô hình nền”. Đây là một quy trình đòi hỏi dữ liệu và tài nguyên tính toán ở mức rất cao.

  Trong giai đoạn tiền huấn luyện, các mô hình được tiếp xúc với hàng tỷ hoặc hàng nghìn tỷ ví dụ về nội dung như hình ảnh, văn bản hoặc âm thanh. Thông qua việc tiếp xúc này, mô hình dần dần phát hiện các đặc trưng trừu tượng để biểu diễn dữ liệu và học cách các đặc trưng đó liên quan với nhau, từ đó cho phép mô hình hiểu được các đầu vào mới trong bối cảnh tương ứng. Quá trình tiền huấn luyện này kéo dài hàng tuần hoặc hàng tháng (‡59) và sử dụng từ hàng chục đến hàng trăm nghìn bộ xử lý đồ họa (GPU) hoặc bộ xử lý tensor (TPU) (‡60) – các chip máy tính chuyên dụng được thiết kế để xử lý nhanh chóng rất nhiều phép tính dạng này. Một số nhà phát triển tiến hành tiền huấn luyện bằng hạ tầng tính toán của riêng họ, trong khi những người khác sử dụng các tài nguyên do các nhà cung cấp dịch vụ tính toán chuyên biệt cung cấp.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Huấn luyện sau đào tạo và fine-tuning (giai đoạn đào tạo thứ hai)

  “Huấn luyện sau” tiếp tục tinh chỉnh mô hình cơ sở để tối ưu nó cho một ứng dụng cụ thể. Đây là một quy trình đòi hỏi mức độ tính toán ở mức vừa phải và mức độ lao động thủ công cao. Việc chuyển sang sử dụng “dữ liệu tổng hợp” – thông tin được tạo ra một cách nhân tạo nhằm bắt chước dữ liệu trong thế giới thực nhưng được tạo bằng thuật toán hoặc mô phỏng – đang giúp làm cho giai đoạn này ít tốn công lao động hơn.
  Sau huấn luyện bao gồm nhiều kỹ thuật fine-tuning và các sửa đổi khác. ‘Supervised fine-tuning’ liên quan đến việc tiếp tục huấn luyện một mô hình đã được huấn luyện trước đó trên các tập dữ liệu cụ thể để cải thiện hiệu suất của mô hình trong lĩnh vực đó (‡61, ‡62). Ví dụ, một mô hình đa mục đích có thể được tiếp tục huấn luyện trên một kho dữ liệu lớn các hình ảnh chẩn đoán hình ảnh y khoa. ‘Reinforcement learning’ (RL) liên quan đến việc cải thiện hiệu suất mô hình bằng cách ‘rewarding’ một mô hình (cung cấp phản hồi tích cực) cho các đầu ra mong muốn và ‘penalising’ một mô hình (cung cấp phản hồi tiêu cực) cho các đầu ra không mong muốn. Nó có hai nhóm con nổi bật. ‘Reinforcement learning from human feedback’ liên quan đến việc thưởng cho các đầu ra phù hợp với sở thích của con người và phạt những đầu ra không phù hợp, dựa trên phản hồi của con người (‡63, ‡64*). ‘Reinforcement learning with verifiable rewards’ (RLVR) được dùng để cải thiện hiệu suất mô hình trên các tác vụ đòi hỏi tính đúng đắn về mặt thực tế, như bài toán toán học hoặc sinh mã. Các nhà phát triển thường xen kẽ giữa việc áp dụng các kỹ thuật sau huấn luyện và chạy thử nghiệm cho đến khi kết quả cho thấy mô hình đáp ứng các yêu cầu kỹ thuật mong muốn.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Tích hợp hệ thống

  Các nhà phát triển kết hợp một hoặc nhiều mô hình AI đa dụng với các thành phần khác để tạo ra một ‘hệ thống AI’ sẵn sàng sử dụng. GPT-5 (ví dụ) là một mô hình AI đa dụng xử lý văn bản, hình ảnh và âm thanh, trong khi ChatGPT là một hệ thống AI đa dụng kết hợp nhiều mô hình với các kích thước và năng lực khác nhau, cùng với giao diện chat, xử lý nội dung, truy cập Web và tích hợp ứng dụng để tạo thành một sản phẩm hoạt động được.
  Ngoài việc làm cho các mô hình AI hoạt động được, các thành phần bổ sung trong một hệ thống AI còn hướng tới việc nâng cao năng lực, tính hữu ích và mức độ an toàn. Ví dụ, một hệ thống có thể đi kèm với một bộ lọc giúp phát hiện và chặn các đầu vào hoặc đầu ra của mô hình có chứa nội dung gây hại (‡65*). Các nhà phát triển cũng ngày càng sử dụng ‘scaffolding’ – phần mềm bổ sung được xây dựng xung quanh các mô hình AI đa năng nhằm cho phép họ lập kế hoạch trước, theo đuổi mục tiêu và tương tác với thế giới (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Triển khai và phát hành
  Triển khai là quá trình đưa hệ thống AI tích hợp vào trạng thái sẵn sàng để sử dụng theo mục đích. Các nhà phát triển và người triển khai tích hợp hệ thống AI vào các ứng dụng, sản phẩm hoặc dịch vụ trong thế giới thực. Các nhà phát triển có thể triển khai hệ thống AI nội bộ (để tự sử dụng) hoặc bên ngoài (cho khách hàng riêng tư hoặc cho mục đích công khai). Khi triển khai hệ thống AI bên ngoài, các công ty thường cung cấp cho người dùng quyền truy cập thông qua các giao diện người dùng trực tuyến hoặc giao diện lập trình ứng dụng (APIs) cho phép người dùng truy cập và chạy hệ thống. Ví dụ, một công ty có thể thiết kế một chatbot dịch vụ khách hàng tùy biến, được cung cấp năng lượng bởi một hệ thống AI đa mục đích của công ty khác.
  “triển khai hệ thống AI” đề cập đến việc đưa một mô hình sẵn sàng cho việc sử dụng trong thế giới thực với các công cụ và giao diện tích hợp, trong khi “phát hành mô hình” liên quan đến việc làm cho mô hình nền tảng có thể được chia sẻ với người khác – hoặc dưới dạng open-weight (các tham số có thể tải xuống) hoặc closed-weight (chỉ truy cập qua API). Xem §3.4. Mô hình open-weight.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Giám sát sau triển khai và cập nhật

  Các nhà phát triển thường thu thập và phân tích phản hồi của người dùng, theo dõi các chỉ số đo tác động và hiệu năng, đồng thời thực hiện các cải tiến lặp lại để giải quyết các vấn đề được phát hiện trong quá trình sử dụng thực tế (‡67). Các cải tiến được thực hiện bằng cách cập nhật các tích hợp của hệ thống, thường thông qua tinh chỉnh liên tục và cung cấp cho các mô hình quyền truy cập vào các cơ sở dữ liệu bên ngoài chứa các (sự kiện) gần đây. Điều này giúp các mô hình AI quy mô lớn luôn được cập nhật mà không cần lặp lại toàn bộ quá trình huấn luyện tiền (pre-training) (‡68*). Nhờ đó, các năng lực có thể tích lũy qua nhiều vòng huấn luyện kế tiếp trong khi vẫn duy trì được tính ổn định và giảm chi phí tính toán.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 1.2: Các giai đoạn phát triển AI đa dụng
>white|black||9|11|br Ở mỗi giai đoạn phát triển AI đa mục đích, mô hình AI được cải tiến để phục vụ các ứng dụng tiếp theo và cuối cùng được triển khai như một hệ thống AI tích hợp hoàn chỉnh, được giám sát và cập nhật.


>white|orangered|left|13|15|bb Các hệ thống suy luận tạo ra “chuỗi suy nghĩ” trong quá trình suy luận để cải thiện hiệu năng

Suy luận xảy ra khi ai đó sử dụng mô hình AI sau khi nó đã được huấn luyện. Ví dụ, suy luận diễn ra khi một người yêu cầu một hệ thống AI lên kế hoạch cho chuyến đi và mô hình đứng sau hệ thống đó dựa trên các khía cạnh liên quan của những gì nó đã học về địa lý, phương tiện di chuyển và ẩm thực để tạo ra một lịch trình.

Trong thập kỷ vừa qua, những tiến bộ về khả năng của AI chủ yếu đến từ các lần huấn luyện lớn hơn; nghĩa là, tăng lượng tài nguyên tính toán (compute) dùng để huấn luyện một mô hình AI. Gần đây, tuy nhiên, các nhà nghiên cứu đã đạt được nhiều cải tiến hơn bằng cách cho phép các mô hình xử lý thông tin trong thời gian dài hơn và huấn luyện chúng tạo ra các bước suy luận rõ ràng khi thực hiện một nhiệm vụ (‡69*, ‡70). Các hệ thống AI hoạt động theo cách như vậy được gọi là ‘hệ thống suy luận’, và các phần giải thích trung gian mà chúng đi qua trong khi giải quyết một vấn đề hoặc trả lời một câu hỏi được gọi là ‘chuỗi suy nghĩ’. Các hệ thống suy luận cần nhiều tài nguyên tính toán hơn tại thời điểm sử dụng để tạo ra các chuỗi suy nghĩ tinh vi này (‡71, ‡72, ‡73, ‡74), và cần nhiều tài nguyên hơn trong quá trình huấn luyện để chúng học suy luận tốt hơn. Trên thực tế, các khả năng suy luận này cho phép hệ thống AI giải các bài toán phức tạp hơn bằng cách lặp lại việc phân rã một nhiệm vụ thành các bước nhỏ hơn. Bàn 1.3 trình bày một ví dụ về hệ thống không suy luận và hệ thống suy luận cùng giải một bài toán.

Các hệ thống suy luận đã đạt được những bước đột phá lớn về năng lực trong các bài toán khó. Ví dụ, vào năm 2025, các hệ thống suy luận chuyên biệt cho việc giải quyết bài toán toán học, như Gemini Deep Think của Google và một mô hình thử nghiệm chưa được phát hành từ OpenAI, đã giải các bài toán của Kỳ thi Olympic Toán học Quốc tế (trong một môi trường kiểm thử có cấu trúc) ở mức tương đương với thành tích của con người đạt huy chương vàng (‡75, ‡76). Các hệ thống suy luận đã thể hiện sự tiến bộ đáng kể trong các lĩnh vực mang tính hình thức như toán học, câu đố logic và các câu hỏi khoa học có cấu trúc, nơi lập luận từng bước có thể được kiểm chứng một cách tường minh (‡77). Tuy nhiên, các hệ thống suy luận cũng có thể thất bại bằng cách tạo ra những chuỗi suy nghĩ không liên quan, thiếu hiệu quả hoặc lặp lại (‡78, ‡79).

###@ Cập nhật về các phương pháp huấn luyện

Kể từ khi Báo cáo trước đó được công bố (tháng 1 2025), một phương pháp huấn luyện có tên là ‘distillation’ đã làm tăng đáng kể hiệu suất mà một số mô hình có thể được fine-tuned. Distillation liên quan đến việc huấn luyện một mô hình ‘student’ trên các đầu ra của một mô hình ‘teacher’ mạnh hơn (và thường là lớn hơn), cho phép mô hình student bắt chước trực tiếp các đầu ra của mô hình teacher (‡80). Ví dụ, DeepSeek đã phát triển một mô hình lớn tên là DeepSeek-R1, nổi bật trong lập luận theo chain-of-thought. R1 tạo ra các đầu ra lập luận, sau đó được dùng để fine-tune các mô hình student nhỏ hơn, bao gồm DeepSeek-V3. DeepSeek-V3 duy trì phần lớn năng lực toán học, lập trình, và phân tích tài liệu của R1 và được cho là đã được fine-tune với khoảng $10,000 USD (mặc dù chi phí pre-training của nó không được công bố) (‡81). Khả năng cao, mức chi phí này thấp hơn theo nhiều bậc độ lớn so với chi phí fine-tuning các mô hình lớn hơn có năng lực tương tự.

![table1.3](images/table1.3_example_reasoning.png)

##### Bàn 1.3: Một ví dụ về hệ thống không suy luận (bên trái) so với hệ thống suy luận (bên phải)
>white|black||9|11|br Giải cùng một câu đố, các ví dụ này được chuyển thể từ các phản hồi AI thực tế. Hệ thống lý giải dành nhiều thời gian và sức mạnh tính toán hơn cho “tư duy” bằng cách xây dựng một “chuỗi suy nghĩ” trước khi cung cấp câu trả lời cuối cùng.

![figure.3](images/fig1.3_AI_agent.png)

##### Nhân vật vật 1.3: Biểu diễn minh họa về một AI agent
>white|black||9|11|br Một mô hình AI (trung tâm) đã được cấu hình để lập kế hoạch, suy luận và sử dụng công cụ một cách lặp đi lặp lại nhằm thực hiện các nhiệm vụ ngoài đời thực. Nguồn: International AI Safety Report 2026.


Do đó, chưng cất có thể là một cách rẻ và hiệu quả để các mô hình có được năng lực mạnh mẽ hơn (‡82). Một số nhà nghiên cứu đã sử dụng chưng cất để tinh chỉnh các mô hình có năng lực cao bằng chỉ 1,000 ví dụ được tạo ra từ các mô hình hiện đại (‡83). Vì chưng cất cần một mô hình giảng viên đã tồn tại trước, nên nó không thể được sử dụng trực tiếp để nâng cao năng lực của các mô hình hiện đại. Tuy nhiên, nó có thể làm tăng tốc sự lan truyền của các năng lực AI tiên tiến, kể cả từ các mô hình nguồn đóng (‡84*).

Cùng với những tiến bộ công nghệ trong “distributed compute” và huấn luyện phi tập trung (các phương pháp mà các nhà phát triển sử dụng nhiều bộ xử lý, máy chủ, hoặc trung tâm dữ liệu hoạt động cùng nhau để thực hiện huấn luyện hoặc suy luận AI (‡85, ‡86, ‡87)), mức độ mà nhiều dự án phát triển AI phụ thuộc vào hạ tầng tính toán lớn, tập trung đã được giảm đi. Điều này ngày càng cho phép các tác nhân có nguồn lực hạn chế hơn phát triển và triển khai các hệ thống mạnh mẽ.

###@ Cập nhật về tác nhân AI

Kể từ Báo cáo gần đây nhất (Tháng 1 năm 2025), những tiến bộ trong cách các nhà phát triển kết hợp các mô hình AI với công cụ đã cho phép phát triển các tác nhân AI ngày càng mạnh mẽ hơn. Các tác nhân AI được thiết kế để theo đuổi các mục tiêu, thường được người dùng chỉ định bằng ngôn ngữ tự nhiên. Để đạt được các mục tiêu đó, chúng được cung cấp quyền truy cập vào các công cụ, chẳng hạn như bộ nhớ, giao diện máy tính và trình duyệt web. Những công cụ này, cùng với mã được sử dụng để kết hợp chúng với mô hình, được gọi là ‘scaffolding’ (giàn dựng), và chúng giúp các tác nhân AI tương tác tự chủ với thế giới, lập kế hoạch, ghi nhớ các chi tiết quan trọng và theo đuổi các mục tiêu (‡88*, ‡89) với việc giám sát hoặc hỗ trợ của con người ít hơn nhiều. Ví dụ, Manus AI là một tác nhân AI phổ biến có thể tự động hóa nhiều tác vụ khác nhau, bao gồm tìm kiếm Web, phát triển phần mềm và mua hàng trực tuyến (‡90). Nhân vật 1.3 minh họa một ví dụ đơn giản về một tác nhân AI gồm một mô hình AI đa dụng ‘brain’ (bộ não) có thể lặp đi lặp lại quá trình lập kế hoạch, suy luận và sử dụng các công cụ cho bộ nhớ, duyệt web và sử dụng máy tính.

Cơ sở hạ tầng số cho các tác nhân AI đang mở rộng (‡91), và chúng ngày càng trở nên phổ biến trong nhiều ngành (‡92, ‡93, ‡94). Các tác nhân AI đã được phát triển cho các tác vụ như nghiên cứu (‡37), kỹ thuật phần mềm (‡95), điều khiển robot (‡96) và dịch vụ khách hàng (‡97). Nghiên cứu và phát triển liên tục đã dẫn đến việc các tác nhân AI hoặc các hệ đa tác nhân ngày càng có năng lực hơn và tự chủ hơn. Các nhà nghiên cứu đã ước tính rằng mức độ phức tạp của các tác vụ chuẩn (benchmark) phần mềm mà các tác nhân AI có thể thực hiện tăng gấp đôi xấp xỉ mỗi bảy tháng (xem thêm §1.2. Current capabilities) (‡98). Các chuyên gia cho rằng các tác nhân AI ngày càng có năng lực sẽ tạo ra cả cơ hội lớn lẫn rủi ro (‡99, ‡100*) (xem §2.2.1. Reliability challenges).

###@ Khoảng trống bằng chứng

Các khoảng trống bằng chứng chính xung quanh quy trình phát triển hệ thống AI đa năng (general- purpose AI) bắt nguồn từ việc thiếu thông tin công khai về cách chúng được phát triển. Một số nhà phát triển công khai cao về cách họ phát triển các hệ thống AI đa năng (‡1, ‡101). Tuy nhiên, nhìn chung, mức độ hiểu biết của công chúng và các nhà hoạch định chính sách về cách đa số mô hình tiên tiến được phát triển, được bảo đảm an toàn (safeguarded), được đánh giá, và được triển khai là có hạn. Điều này đặc biệt đúng với các hệ thống AI được triển khai nội bộ, được sử dụng trong các công ty AI nhưng không được bên liên quan ở bên ngoài sử dụng hoặc hiểu rõ (‡102, ‡103). Mức độ hiển thị bên ngoài hạn chế này tạo ra các thách thức cho tính minh bạch và giám sát. Nhiều nhà nghiên cứu đã chỉ ra tính minh bạch hạn chế và không nhất quán xoay quanh dữ liệu huấn luyện (‡104, ‡105, ‡106), các mô hình AI đa năng (‡107, ‡108), các tác nhân AI (AI agents) (‡92), các đánh giá (‡109), các đường ống phát triển (development pipelines) (‡110), và an toàn (safety) (‡111). Việc hạn chế công bố cho bên ngoài đôi khi là cần thiết để bảo vệ bí mật thương mại và quyền sở hữu trí tuệ của doanh nghiệp. Đồng thời, tính minh bạch thấp làm cho việc nghiên cứu độc lập của các nhà nghiên cứu và nhà hoạch định chính sách về các mô hình và hệ thống AI đa năng trở nên khó khăn hơn.


