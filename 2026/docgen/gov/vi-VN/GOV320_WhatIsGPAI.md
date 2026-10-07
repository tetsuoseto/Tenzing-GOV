###@ Các hệ thống AI đa dụng là gì?

Các hệ thống AI đa dụng là những chương trình phần mềm học các quy luật từ lượng dữ liệu lớn, cho phép chúng thực hiện nhiều loại tác vụ thay vì được chuyên biệt hóa cho một chức năng hoặc lĩnh vực cụ thể (xem Bàn 1.1). Để tạo ra các hệ thống này, các nhà phát triển AI tiến hành một quy trình gồm nhiều giai đoạn, đòi hỏi nguồn lực tính toán đáng kể, các tập dữ liệu lớn và chuyên môn chuyên sâu (xem Bàn 1.2). Nguồn lực tính toán (thường được gọi tắt là “compute”) cần thiết cho cả quá trình phát triển lẫn triển khai các hệ thống AI, bao gồm các chip máy tính chuyên dụng cũng như phần mềm và cơ sở hạ tầng cần thiết để vận hành chúng.† Vì được huấn luyện trên các tập dữ liệu lớn và đa dạng, các hệ thống AI đa dụng có thể thực hiện nhiều tác vụ khác nhau, chẳng hạn như tóm tắt văn bản, tạo hình ảnh hoặc viết mã máy tính. Phần này giải thích cách tạo ra các hệ thống AI đa dụng, “mô hình suy luận” là gì và các quyết định chính sách định hình quá trình phát triển hệ thống AI đa dụng như thế nào.

    Lưu ý † -- Thuật ngữ ‘compute’ cũng có thể chỉ một phép đo số lượng phép tính mà bộ xử lý có thể thực hiện (thường được đo bằng số phép toán dấu phẩy động mỗi giây) hoặc cụ thể là phần cứng (chẳng hạn như bộ xử lý đồ họa) thực hiện các phép tính đó.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Các hệ thống ngôn ngữ
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
###@ Các trình tạo ảnh
- DALL-E 3 (‡13*)
- Gemini 2.5 Flash (‡14*)
- Midjourney v7 (‡15*)
- Qwen-Image (‡16*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Các trình tạo video
- Cosmos (‡17*)
- Sora (‡18*)
- Pika (‡19)
- Runway (‡19)
- Veo 3 (‡20*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Hệ thống robot và định vị đường đi
- Gemini Robotics (‡21*)
- Gr00t N1 (‡22*)
- MobileAloha (‡23)
- OctoAI (‡24*)
- OpenVLA (‡25*)
- PaLM-E (‡26)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Các công cụ dự đoán cho nhiều lớp cấu trúc phân tử sinh học
- AlphaFold 3 (‡27)
- Khuếch đại (‡28)
- CellFM (‡29)
- Evo 2 (‡30)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
###@ Các tác nhân AI
- AlphaEvolve (‡31*)
- Tác nhân ChatGPT (‡32*)
- Claude Code (‡33*)
- Doubao-1.5 (34*)
- Magentic-One (‡35*)
- OpenScholar (‡36*)
- AI Scientist-v2 (‡37, ‡38, ‡39*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 1.1: Các loại AI đa dụng
>white|black||9|11|br Có một số loại AI đa dụng khác nhau. Trong Báo cáo này, các mô hình có thể dự đoán thông tin cấu trúc cho nhiều lớp phân tử khác nhau được xem là AI “đa dụng” vì chúng có thể được điều chỉnh cho nhiều nhiệm vụ. Ví dụ, các mô hình được huấn luyện để dự đoán cấu trúc protein có thể được ứng dụng vào nhiều nhiệm vụ khác, chẳng hạn như dự đoán tương tác protein, dự đoán vị trí liên kết của các phân tử nhỏ, cũng như dự đoán và thiết kế peptide vòng (‡40).


>white|orangered|left|13|15|bb  Học sâu là nền tảng của AI đa dụng

Các nhà nghiên cứu xây dựng các mô hình AI đa năng bằng một quy trình gọi là ‘học sâu’, trong đó mô hình được huấn luyện để học từ các ví dụ (‡41). Khác với kỹ thuật phần mềm, các mô hình học sâu học cách hoàn thành nhiệm vụ từ dữ liệu thay vì dựa vào các chỉ dẫn được viết thủ công. Bằng cách xử lý lượng lớn dữ liệu, chẳng hạn như hình ảnh, văn bản hoặc âm thanh, các mô hình này khám phá cách biểu diễn dữ liệu đó, tạo ra các biểu diễn nội bộ về những mẫu (chẳng hạn như hình dạng, mối liên hệ giữa các từ hoặc cấu trúc âm thanh) giúp mô hình nhận diện các mối quan hệ và tạo ra đầu ra phù hợp với mục tiêu huấn luyện. Sau đó, chúng sử dụng các biểu diễn nội bộ đã học này làm đặc trưng trừu tượng để phân tích dữ liệu mới tương tự và tạo ra đầu ra theo cùng phong cách. Ví dụ, một mô hình AI đa- năng được huấn luyện với đủ ví dụ về thơ lãng mạn Anh thế kỷ 19 có thể nhận diện những bài thơ mới theo phong cách đó và tạo ra nội dung mới có phong cách tương tự.

Ở cấp độ chi tiết hơn, học sâu hoạt động bằng cách xử lý dữ liệu qua các lớp gồm những nút xử lý thông tin được kết nối với nhau. Những nút này thường được gọi là ‘nơ-ron’ vì chúng phần nào lấy cảm hứng từ các nơ-ron trong não bộ sinh học (‘mạng nơ-ron’) (Nhân vật 1.1) (‡42).Khi thông tin truyền từ lớp nơ-ron này sang lớp tiếp theo, mô hình dần biến đổi dữ liệu thành các biểu diễn trừu tượng hơnthông qua các nhóm đặc trưng đã học – những mẫu hình mà mô hình tự động phát hiện trong dữ liệu, thay vì được lập trình thủ công. Ví dụ, trong một mô hình xử lý hình ảnh, các lớp đầu tiên có thể học cách phát hiện những đặc trưng đơn giản như cạnh hoặc hình dạng cơ bản, trong khi các lớp sâu hơn kết hợp những đặc trưng này để nhận diện các mẫu hình phức tạp hơn như khuôn mặt hoặc đồ vật.

Các đặc trưng ở mọi lớp được phát hiện thông qua quá trình tối ưu hóa xác định quy trình huấn luyện. Trong quá trình huấn luyện, khi mô hình mắc lỗi, các thuật toán học sâu điều chỉnh độ mạnh của nhiều liên kết giữa các nơ-ron để cải thiện hiệu suất của mô hình. Độ mạnh của mỗi liên kết giữa các nút thường được gọi là ‘trọng số’. Cách tiếp cận phân lớp này là nguồn gốc tên gọi học sâu.

Học sâu đã chứng minh hiệu quả vượt trội trong việc giúp các hệ thống AI thực hiện những nhiệm vụ từng được xem là khó đối với các hệ thống tính toán được lập trình thủ công truyền thống và các phương pháp AI biểu tượng hoặc dựa trên quy tắc trước đây. Hầu hết các mô hình AI đa dụng tiên tiến nhất hiện nay đều dựa trên một kiến trúc mạng nơ-ron cụ thể có tên là ‘transformer’ (‡43, ‡44). Transformer sử dụng cơ chế ‘chú ý’ (‡45), giúp mô hình tập trung vào những phần dữ liệu đầu vào liên quan nhất khi xử lý thông tin, chẳng hạn như xác định những từ nào trong câu quan trọng nhất để hiểu ý nghĩa của câu. Cách xây dựng mô hình này đã mang lại những cải tiến đáng kể trong dịch thuật (‡43), xử lý ngôn ngữ tự nhiên (‡46), nhận dạng hình ảnh (‡47) và nhận dạng giọng nói (‡48, ‡49), cuối cùng dẫn đến sự phát triển của những mô hình tiên tiến nhất hiện nay.

![fig1.1](images/fig1.1_neural_network.png)

##### Nhân vật vật 1.1: Hình minh họa về một ‘mạng nơ-ron’
>white|black||9|11|br Các mô hình AI đa dụng hiện nay dựa trên những mạng lưới này, vốn được lấy cảm hứng một cách khái quát từ bộ não sinh học. Các mạng lưới khác nhau có kích thước và kiến trúc khác nhau. Tuy nhiên, tất cả đều gồm các đơn vị xử lý thông tin được kết nối với nhau, gọi là ‘nơ-ron’, trong đó độ mạnh của các kết nối giữa các nơ-ron được gọi là ‘trọng số’. Trọng số được cập nhật thông qua quá trình huấn luyện với lượng dữ liệu lớn. Nguồn: Báo cáo An toàn AI Quốc tế 2025 (‡50) (đã chỉnh sửa).

![fig1.2](images/fig1.2_GAI_dev_stages.png)

##### Nhân vật vật 1.2: Sơ đồ minh họa các giai đoạn phát triển AI đa dụng
>white|black|left|9|11|br Nguồn: Báo cáo An toàn AI Quốc tế 2026.


>white|orangered|left|13|15|bb  AI đa dụng được phát triển theo từng giai đoạn

Việc phát triển một hệ thống AI đa dụng bao gồm nhiều giai đoạn, từ huấn luyện mô hình ban đầu đến giám sát và cập nhật sau triển khai (Nhân vật 1.2). Trên thực tế, các bước này thường chồng lấn theo cách lặp đi lặp lại. Mỗi giai đoạn đòi hỏi các nguồn lực đầu vào khác nhau (ví dụ: dữ liệu, nhân lực, năng lực tính toán) và các kỹ thuật khác nhau, đồng thời đôi khi do những nhà phát triển khác nhau thực hiện (Nhân vật 1.2 và Bàn 1.2).

Ví dụ, quá trình tiền huấn luyện mô hình thường đòi hỏi lượng lớn tài nguyên tính toán và dữ liệu, khiến giai đoạn này đặc biệt nhạy cảm với các chính sách ảnh hưởng đến quyền tiếp cận tài nguyên tính toán hoặc dữ liệu huấn luyện (‡51, ‡52). Tương tự, hiện nay, việc tuyển chọn dữ liệu và một số phương pháp tinh chỉnh mô hình đòi hỏi nhiều lao động con người để gán nhãn dữ liệu ban đầu (‡53). Do đó, giai đoạn này nhạy cảm với những thay đổi về chi phí lao động, chính sách nền tảng hoặc quy định ảnh hưởng đến các thỏa thuận thuê ngoài xuyên biên giới.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 1. Thu thập và tuyển chọn dữ liệu
> 
  Trước khi huấn luyện một mô hình AI đa năng, các nhà phát triển và nhân viên xử lý dữ liệu thu thập, làm sạch, tuyển chọn và chuẩn hóa dữ liệu huấn luyện thô thành định dạng mà mô hình có thể học. Quá trình này có thể đòi hỏi nhiều công sức. Các bộ dữ liệu huấn luyện đứng sau những mô hình tiên tiến nhất bao gồm số lượng ví dụ khổng lồ từ khắp internet.
  Các nhóm thường phát triển những phương pháp lọc tinh vi để giảm nội dung có hại, loại bỏ dữ liệu trùng lặp và cải thiện mức độ đại diện cho các chủ đề và nguồn khác nhau (‡54, ‡55). Việc tuyển chọn dữ liệu cũng có thể giúp giảm các vi phạm bản quyền và quyền riêng tư, loại bỏ các ví dụ chứa kiến thức nguy hiểm, xử lý nhiều ngôn ngữ và cải thiện tài liệu về nguồn gốc dữ liệu (‡56, ‡57, ‡58).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 2. Tiền huấn luyện (giai đoạn đầu tiên của quá trình huấn luyện)

  Trong quá trình tiền huấn luyện, các nhà phát triển cung cấp cho mô hình lượng dữ liệu đa dạng khổng lồ để trang bị cho mô hình nền tảng kiến thức rộng và khả năng hiểu ngữ cảnh. Quá trình này tạo ra một “mô hình nền”. Đây là một quá trình đòi hỏi lượng dữ liệu và năng lực tính toán rất lớn.

  Trong quá trình tiền huấn luyện, các mô hình được tiếp xúc với hàng tỷ hoặc hàng nghìn tỷ mẫu nội dung như hình ảnh, văn bản hoặc âm thanh. Qua quá trình tiếp xúc này, mô hình dần khám phá ra các đặc trưng trừu tượng để biểu diễn dữ liệu và học được mối liên hệ giữa các đặc trưng đó, nhờ vậy có thể hiểu các đầu vào mới trong ngữ cảnh. Quá trình tiền huấn luyện này kéo dài hàng tuần hoặc hàng tháng (‡59) và sử dụng hàng chục hoặc hàng trăm nghìn bộ xử lý đồ họa (GPU) hoặc bộ xử lý tensor (TPU) (‡60) – các chip máy tính chuyên dụng được thiết kế để nhanh chóng thực hiện nhiều phép tính như vậy. Một số nhà phát triển tiến hành tiền huấn luyện bằng năng lực tính toán của riêng mình, trong khi những nhà phát triển khác sử dụng tài nguyên do các nhà cung cấp năng lực tính toán chuyên biệt cung cấp.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 3. Hậu huấn luyện và tinh chỉnh (giai đoạn huấn luyện thứ hai)

  ‘Hậu huấn luyện’ tiếp tục tinh chỉnh mô hình nền tảng để tối ưu hóa mô hình cho một ứng dụng cụ thể. Đây là một quy trình đòi hỏi mức năng lực tính toán vừa phải và rất nhiều nhân lực. Xu hướng chuyển sang sử dụng ‘dữ liệu tổng hợp’ – thông tin được tạo ra một cách nhân tạo, mô phỏng dữ liệu trong thế giới thực nhưng được tạo bằng thuật toán hoặc mô phỏng – đang giúp giai đoạn này bớt đòi hỏi nhiều nhân lực hơn.
  Huấn luyện hậu kỳ bao gồm nhiều kỹ thuật tinh chỉnh và các sửa đổi khác. ‘Tinh chỉnh có giám sát’ bao gồm việc tiếp tục huấn luyện một mô hình đã được huấn luyện trên các tập dữ liệu cụ thể để cải thiện hiệu suất của mô hình trong lĩnh vực đó (‡61, ‡62). Ví dụ: một mô hình đa dụng có thể được huấn luyện thêm trên một kho ảnh X quang lớn. ‘Học tăng cường’ (RL) bao gồm việc cải thiện hiệu suất mô hình bằng cách ‘thưởng’ cho mô hình (đưa ra phản hồi tích cực) khi tạo ra đầu ra mong muốn và ‘phạt’ mô hình (đưa ra phản hồi tiêu cực) khi tạo ra đầu ra không mong muốn. Phương pháp này có hai phân nhóm nổi bật. ‘Học tăng cường từ phản hồi của con người’ bao gồm việc thưởng cho những đầu ra phù hợp với sở thích của con người và phạt những đầu ra không phù hợp, dựa trên phản hồi của con người (‡63, ‡64*). ‘Học tăng cường với phần thưởng có thể xác minh’ (RLVR) được sử dụng để cải thiện hiệu suất mô hình đối với các tác vụ đòi hỏi tính chính xác về mặt sự thật, chẳng hạn như toán học hoặc tạo mã. Các nhà phát triển thường luân phiên áp dụng các kỹ thuật huấn luyện hậu kỳ và chạy thử nghiệm cho đến khi kết quả cho thấy mô hình đáp ứng các thông số kỹ thuật mong muốn.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 4. Tích hợp hệ thống

  Các nhà phát triển kết hợp một hoặc nhiều mô hình AI đa dụng với các thành phần khác để tạo ra một ‘hệ thống AI’ sẵn sàng sử dụng. Chẳng hạn, GPT-5 là một mô hình AI đa dụng xử lý văn bản, hình ảnh và âm thanh, trong khi ChatGPT là một hệ thống AI đa dụng kết hợp một số mô hình có kích thước và năng lực khác nhau với giao diện trò chuyện, khả năng xử lý nội dung, truy cập Web và tích hợp ứng dụng để tạo ra một sản phẩm hoàn chỉnh.
  Ngoài việc đưa các mô hình AI vào vận hành, các thành phần bổ sung trong một hệ thống AI còn nhằm nâng cao năng lực, tính hữu ích và độ an toàn. Ví dụ, một hệ thống có thể đi kèm bộ lọc phát hiện và chặn các đầu vào hoặc đầu ra của mô hình chứa nội dung có hại (‡65*). Các nhà phát triển cũng ngày càng sử dụng “lớp phần mềm hỗ trợ” – phần mềm bổ sung được xây dựng xung quanh các mô hình AI đa dụng, cho phép chúng lập kế hoạch trước, theo đuổi mục tiêu và tương tác với thế giới (‡66).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 5. Triển khai và phát hành
  Triển khai là quá trình đưa hệ thống AI tích hợp vào trạng thái sẵn sàng để sử dụng theo mục đích đã định. Các nhà phát triển và bên triển khai đưa hệ thống AI vào các ứng dụng, sản phẩm hoặc dịch vụ trong thế giới thực. Các nhà phát triển có thể triển khai hệ thống AI nội bộ (để sử dụng cho riêng mình) hoặc bên ngoài (cho khách hàng cá nhân hoặc phục vụ công chúng). Khi triển khai hệ thống AI bên ngoài, các công ty thường cung cấp cho người dùng quyền truy cập thông qua giao diện người dùng trực tuyến hoặc giao diện lập trình ứng dụng (API), cho phép người dùng truy cập và chạy hệ thống. Ví dụ, một công ty có thể thiết kế riêng một chatbot dịch vụ khách hàng được vận hành bằng hệ thống AI đa dụng của một công ty khác.
  ‘Triển khai hệ thống AI’ là việc cung cấp một mô hình để sử dụng trong thực tế cùng với các công cụ và giao diện được tích hợp, trong khi ‘phát hành mô hình’ là việc cung cấp mô hình nền cho người khác truy cập – theo dạng trọng số mở (có thể tải xuống các tham số) hoặc trọng số đóng (chỉ truy cập qua API). Xem §3.4. Các mô hình trọng số mở.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb 6. Giám sát sau triển khai và cập nhật

  Các nhà phát triển thường thu thập và phân tích phản hồi của người dùng, theo dõi tác động và các chỉ số hiệu suất, đồng thời thực hiện các cải tiến lặp đi lặp lại để giải quyết những vấn đề được phát hiện trong quá trình sử dụng thực tế (‡67). Các cải tiến được thực hiện bằng cách cập nhật các tích hợp hệ thống, thường thông qua việc tinh chỉnh liên tục và cung cấp cho mô hình quyền truy cập vào các cơ sở dữ liệu bên ngoài chứa những thông tin thực tế (mới đây). Nhờ vậy, các mô hình AI lớn luôn được cập nhật mà không cần lặp lại toàn bộ quá trình tiền huấn luyện (‡68*). Điều này cho phép các năng lực được tích lũy qua những vòng huấn luyện liên tiếp, đồng thời duy trì tính ổn định và giảm chi phí tính toán.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 1.2: Các giai đoạn phát triển AI đa dụng
>white|black||9|11|br Ở mỗi giai đoạn phát triển AI đa dụng, mô hình AI được cải thiện để phục vụ các ứng dụng tiếp theo và cuối cùng được triển khai thành một hệ thống AI tích hợp hoàn chỉnh, được giám sát và cập nhật.


>white|orangered|left|13|15|bb Các hệ thống suy luận tạo ra ‘chuỗi suy nghĩ’ trong quá trình suy luận để cải thiện hiệu suất

Suy luận diễn ra khi ai đó sử dụng mô hình AI sau khi mô hình đã được huấn luyện. Ví dụ, suy luận xảy ra khi một người yêu cầu hệ thống AI lập kế hoạch cho chuyến đi và mô hình đứng sau hệ thống đó vận dụng những kiến thức liên quan đã học về địa lý, giao thông và ẩm thực để tạo ra lịch trình.

Trong thập kỷ qua, những tiến bộ về năng lực AI phần lớn đến từ các đợt huấn luyện quy mô lớn hơn; tức là tăng lượng tài nguyên tính toán được sử dụng để huấn luyện một mô hình AI. Tuy nhiên, gần đây, các nhà nghiên cứu đã đạt được nhiều tiến bộ hơn bằng cách cho phép các mô hình xử lý thông tin trong thời gian dài hơn và huấn luyện chúng tạo ra các bước lập luận tường minh khi thực hiện một nhiệm vụ (‡69*, ‡70). Các hệ thống AI hoạt động theo cách này được gọi là ‘hệ thống suy luận’, còn những lời giải thích trung gian mà chúng đưa ra khi giải quyết một vấn đề hoặc trả lời một câu hỏi được gọi là ‘chuỗi suy nghĩ’. Hệ thống suy luận cần nhiều tài nguyên tính toán hơn trong quá trình sử dụng để tạo ra những chuỗi suy nghĩ phức tạp này (‡71, ‡72, ‡73, ‡74), và cần nhiều tài nguyên hơn trong quá trình huấn luyện để học cách suy luận tốt hơn. Trên thực tế, những năng lực suy luận này cho phép các hệ thống AI giải quyết các vấn đề phức tạp hơn bằng cách liên tục chia một nhiệm vụ thành các bước nhỏ hơn. Bàn 1.3 đưa ra ví dụ về một hệ thống không có khả năng suy luận và một hệ thống suy luận cùng giải quyết một vấn đề.

Các hệ thống suy luận đã đạt được những bước đột phá lớn về năng lực giải quyết các vấn đề khó. Ví dụ, vào năm 2025, các hệ thống suy luận chuyên giải toán, chẳng hạn như Gemini Deep Think của Google và một mô hình thử nghiệm chưa được phát hành của OpenAI, đã giải được các bài toán của Kỳ thi Olympic Toán học Quốc tế (trong một môi trường kiểm tra có cấu trúc) với kết quả tương đương thành tích giành huy chương vàng của con người (‡75, ‡76). Các hệ thống suy luận đã cho thấy tiến bộ đáng kể trong những lĩnh vực hình thức như toán học, câu đố logic và các câu hỏi khoa học có cấu trúc, nơi có thể xác minh tường minh quá trình suy luận từng bước (‡77). Tuy nhiên, các hệ thống suy luận cũng có thể thất bại khi tạo ra những chuỗi suy nghĩ không liên quan, không hiệu quả hoặc lặp đi lặp lại (‡78, ‡79).

###@ Cập nhật về các phương pháp huấn luyện

Kể từ khi Báo cáo gần nhất được công bố (tháng 1 năm 2025), một phương pháp huấn luyện có tên là ‘chưng cất’ đã giúp tăng đáng kể hiệu quả tinh chỉnh một số mô hình. Chưng cất là phương pháp huấn luyện một mô hình ‘học sinh’ dựa trên đầu ra của một mô hình ‘giáo viên’ mạnh hơn (và thường lớn hơn), cho phép mô hình học sinh trực tiếp bắt chước đầu ra của mô hình giáo viên (‡80). Ví dụ, DeepSeek đã phát triển một mô hình lớn có tên DeepSeek-R1, vượt trội về khả năng suy luận chuỗi suy nghĩ. R1 tạo ra các đầu ra suy luận, sau đó được dùng để tinh chỉnh các mô hình học sinh nhỏ hơn, bao gồm DeepSeek-V3. DeepSeek-V3 duy trì phần lớn khả năng toán học, lập trình và phân tích tài liệu của R1, và được cho là đã được tinh chỉnh với chi phí khoảng $10,000 USD (mặc dù chi phí tiền huấn luyện không được công bố) (‡81). Con số này có khả năng thấp hơn nhiều bậc độ lớn so với chi phí tinh chỉnh các mô hình lớn hơn có năng lực tương đương.

![table1.3](images/table1.3_example_reasoning.png)

##### Bàn 1.3: Ví dụ về hệ thống không suy luận (bên trái) so với hệ thống suy luận (bên phải)
>white|black||9|11|br Để giải cùng một câu đố, các ví dụ này được phỏng theo những phản hồi thực tế của AI. Hệ thống suy luận dành nhiều thời gian và năng lực tính toán hơn cho việc ‘suy nghĩ’ bằng cách xây dựng một ‘chuỗi suy nghĩ’ trước khi đưa ra câu trả lời cuối cùng.

![figure.3](images/fig1.3_AI_agent.png)

##### Nhân vật vật 1.3: Minh họa về một tác nhân AI
>white|black||9|11|br Một mô hình AI (ở giữa) đã được cấu hình để lập kế hoạch, suy luận và sử dụng công cụ theo từng bước nhằm hoàn thành các nhiệm vụ trong thế giới thực. Nguồn: Báo cáo An toàn AI Quốc tế 2026.


Do đó, chưng cất tri thức có thể là một cách ít tốn kém và hiệu quả để giúp các mô hình đạt được những năng lực mạnh mẽ hơn (‡82). Một số nhà nghiên cứu đã sử dụng phương pháp chưng cất tri thức để tinh chỉnh các mô hình có năng lực cao bằng chỉ 1,000 ví dụ được tạo ra từ các mô hình state-of- the-art (‡83). Vì chưng cất tri thức đòi hỏi phải có sẵn một mô hình giáo viên, phương pháp này không thể được sử dụng trực tiếp để nâng cao năng lực của các mô hình state-of-the-art. Tuy nhiên, phương pháp này có thể đẩy nhanh sự phổ biến của các năng lực AI tiên tiến, kể cả từ các mô hình có mã nguồn đóng (‡84*).

Cùng với những tiến bộ công nghệ trong lĩnh vực ‘tính toán phân tán’ và đào tạo phi tập trung (các phương pháp trong đó nhà phát triển sử dụng nhiều bộ xử lý, máy chủ hoặc trung tâm dữ liệu phối hợp với nhau để thực hiện đào tạo hoặc suy luận AI (‡85, ‡86, ‡87)), mức độ phụ thuộc của nhiều dự án phát triển AI vào cơ sở hạ tầng điện toán tập trung, quy mô lớn- đã giảm. Điều này ngày càng tạo điều kiện cho các tác nhân có ít nguồn lực hơn phát triển và triển khai các hệ thống mạnh mẽ.

###@ Cập nhật về các tác nhân AI

Kể từ Báo cáo gần nhất (January 2025), những tiến bộ trong cách các nhà phát triển kết hợp mô hình AI với công cụ đã cho phép phát triển các tác nhân AI ngày càng mạnh mẽ. Các tác nhân AI được thiết kế để theo đuổi mục tiêu, thường do người dùng chỉ định bằng ngôn ngữ tự nhiên. Để đạt được những mục tiêu này, chúng được cấp quyền truy cập vào các công cụ như bộ nhớ, giao diện máy tính và trình duyệt web. Những công cụ này cùng mã được sử dụng để kết hợp chúng với mô hình được gọi là ‘giàn giáo’, giúp các tác nhân AI tự chủ tương tác với thế giới, lập kế hoạch, ghi nhớ các chi tiết quan trọng và theo đuổi mục tiêu (‡88*, ‡89) với ít sự giám sát hoặc hỗ trợ của con người hơn nhiều. Ví dụ, Manus AI là một tác nhân AI phổ biến có thể tự động hóa nhiều tác vụ, bao gồm tìm kiếm trên Web, phát triển phần mềm và mua hàng trực tuyến (‡90). Nhân vật 1.3 minh họa một ví dụ đơn giản về tác nhân AI gồm một ‘bộ não’ là mô hình AI đa dụng, có thể lập kế hoạch, suy luận và sử dụng lặp đi lặp lại các công cụ để ghi nhớ, duyệt web và sử dụng máy tính.

Cơ sở hạ tầng số dành cho các tác nhân AI đang mở rộng (‡91), và chúng ngày càng phổ biến trong nhiều ngành (‡92, ‡93, ‡94). Các tác nhân AI đã được phát triển để thực hiện những nhiệm vụ như nghiên cứu (‡37), kỹ thuật phần mềm (‡95), điều khiển robot (‡96) và dịch vụ khách hàng (‡97). Các hoạt động nghiên cứu và phát triển liên tục đã giúp các tác nhân AI hoặc hệ thống đa tác nhân ngày càng có năng lực cao hơn và tự chủ hơn. Các nhà nghiên cứu ước tính rằng độ phức tạp của các nhiệm vụ trong các bài kiểm tra tiêu chuẩn về phần mềm mà tác nhân AI có thể hoàn thành tăng gấp đôi khoảng mỗi bảy tháng (xem thêm §1.2. Năng lực hiện tại) (‡98). Các chuyên gia cho rằng các tác nhân AI ngày càng có năng lực cao sẽ mang lại cả những cơ hội lớn lẫn rủi ro (‡99, ‡100*) (xem §2.2.1. Thách thức về độ tin cậy).

###@ Những khoảng trống về bằng chứng

Những khoảng trống bằng chứng chính xung quanh quy trình phát triển hệ thống AI đa dụng bắt nguồn từ việc thiếu thông tin được công khai  về cách chúng được phát triển. Một số nhà phát triển rất minh bạch về cách họ phát triển các hệ thống AI đa dụng (‡1, ‡101). Tuy nhiên, nhìn chung, công chúng và các nhà hoạch định chính sách còn biết rất hạn chế về cách phần lớn các mô hình tiên tiến được phát triển, bảo vệ, đánh giá và triển khai. Điều này đặc biệt đúng với các hệ thống AI được triển khai nội bộ, được sử dụng trong các công ty AI nhưng không được các bên liên quan bên ngoài sử dụng hoặc hiểu rõ (‡102, ‡103). Khả năng quan sát từ bên ngoài hạn chế này gây khó khăn cho tính minh bạch và hoạt động giám sát. Nhiều nhà nghiên cứu đã chỉ ra mức độ minh bạch hạn chế và thiếu nhất quán về dữ liệu huấn luyện (‡104, ‡105, ‡106), các mô hình AI đa dụng (‡107, ‡108), tác tử AI (‡92), hoạt động đánh giá (‡109), quy trình phát triển (‡110) và vấn đề an toàn (‡111). Đôi khi cần hạn chế công khai thông tin ra bên ngoài để bảo vệ bí mật thương mại và tài sản trí tuệ của các công ty. Đồng thời, mức độ minh bạch thấp khiến các nhà nghiên cứu độc lập và nhà hoạch định chính sách khó nghiên cứu các mô hình và hệ thống AI đa dụng hơn.


