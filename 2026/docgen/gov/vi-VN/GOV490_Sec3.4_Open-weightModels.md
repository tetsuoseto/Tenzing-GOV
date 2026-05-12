##########
>white|orangered|left|14|30|hr Mục 3.4
### 3.4. Mô hình mã nguồn mở
>white|orangered|left|24|30|hb Các mô hình trọng lượng mở (open-weight models)

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mức độ truy cập mà các công ty AI cung cấp cho các ‘trọng số’ của mô hình của họ ảnh hưởng đến các rủi ro mà các mô hình này tạo ra. Trọng số là các tham số toán học cho phép các mô hình AI xử lý đầu vào và tạo ra đầu ra. Với bất kỳ mô hình nào, các công ty có thể chọn giữ trọng số hoàn toàn riêng tư, cấp cho một số người dùng một mức truy cập giới hạn, hoặc cho phép bất kỳ ai tải chúng về đầy đủ. Các mô hình mà trọng số của chúng sẵn có công khai được gọi là ‘open-weight models’.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Các mô hình trọng số mở tạo điều kiện cho nghiên cứu và đổi mới, nhưng các biện pháp bảo vệ của chúng dễ bị loại bỏ hơn. Trên khắp thế giới, nhiều chủ thể khác nhau – đặc biệt là những chủ thể có ít nguồn lực hơn – có thể sử dụng các mô hình trọng số mở cho mục đích nghiên cứu và thương mại. Tuy nhiên, so với các mô hình trọng số đóng, các mô hình trọng số mở dễ được chỉnh sửa hơn để thể hiện các hành vi có khả năng gây hại và  s khó hơn.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Việc phát hành mô hình open-weight là không thể thu hồi. Sau khi được phát hành, trọng số của mô hình không thể được hoàn lại. Điều này khiến việc giảm thiểu các tác hại tiềm ẩn do việc phát hành một mô hình có năng lực nguy hiểm trở nên khó khăn hơn.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi phát hành Báo cáo trước đó (tháng 1 năm 2025), các bản phát hành mã nguồn mở trọng số lớn đã thu hẹp khoảng cách về năng lực so với các mô hình đóng hàng đầu. Các nhà phát triển Trung Quốc DeepSeek và Alibaba đã phát hành lần lượt các mô hình R1 và Qwen, đạt hiệu suất tương đương với các mô hình đóng hàng đầu, trong khi OpenAI đã phát hành các mô hình mã nguồn mở trọng số đầu tiên của mình kể từ năm 2019. Năng lực của các mô hình đóng hàng đầu hiện được ước tính là thấp hơn không quá 1 năm so với các mô hình mã nguồn mở trọng số hàng đầu trên các bộ chuẩn AI nổi bật.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Một thách thức chính sách quan trọng là tiếp cận các lợi ích mà các mô hình open-weight (mở trọng số) mang lại, đồng thời quản lý các rủi ro riêng biệt của chúng. Một cách tiếp cận là đánh giá các mô hình open-weight theo “rủi ro cận biên”: mức độ mà việc phát hành chúng một cách phản thực (counterfactually) làm gia tăng rủi ro đối với xã hội so với rủi ro vốn đã tồn tại do các mô hình hiện có hoặc các công nghệ khác. Tuy nhiên, điều này rất phức tạp trong thực tiễn. Những gia tăng nhỏ về rủi ro cận biên theo thời gian cũng có thể tích lũy và dẫn đến những gia tăng đáng kể về tổng thể rủi ro.
>oldlace|black||11|15|br      


Các mô hình mã nguồn mở có tham số được công khai để tải xuống có những tác động khác biệt đối với nhiều thách thức được thảo luận ở các phần trước. “Các trọng số” của một mô hình AI chứa thông tin then chốt cho phép nó tạo ra các phản hồi hữu ích cho người dùng. Khi đã được phát hành, các trọng số này không thể được thu hồi: bất kỳ ai cũng có thể tải xuống, nghiên cứu, sửa đổi, chia sẻ và sử dụng chúng trên máy tính hoặc tài khoản đám mây của riêng mình. Khi các trọng số được công khai, những người khác có thể dễ dàng hơn để xây dựng và sửa đổi mô hình, đáp ứng nhiều nhu cầu khác nhau và thúc đẩy đổi mới (‡1317). Tuy nhiên, theo cùng cơ chế đó, người dùng với ý định xấu cũng có thể dễ dàng hơn để loại bỏ các cơ chế bảo vệ và sửa đổi các mô hình mã nguồn mở để phục vụ các trường hợp sử dụng gây hại (‡1122, ‡1160). Điều này đã đặt ra câu hỏi liệu một số mô hình mã nguồn mở có nên được áp dụng các yêu cầu đặc biệt (ví dụ: thử nghiệm nghiêm ngặt hơn trước khi phát hành) hay, ngược lại, được miễn trừ đặc biệt (ví dụ: miễn các yêu cầu báo cáo theo quy định) (‡1033).

###@ Bối cảnh về các mô hình trọng số mở

>white|orangered||14|15.5|bb Các mô hình trọng số mã nguồn mở có thể là, nhưng không nhất thiết phải là, các mô hình “mã nguồn mở”.

Mặc dù thường được gọi là ‘phần mềm nguồn mở’, phần lớn các mô hình được phát hành công khai chính xác hơn được mô tả là ‘nguồn mở trọng số’. Điều này là vì, mặc dù các nhà phát triển cung cấp các trọng số của mô hình, họ không phát hành mã huấn luyện hoặc các bộ dữ liệu tương ứng. Hơn nữa, phần mềm nguồn mở thường được đặc trưng bởi các giấy phép cho phép đặt ra các yêu cầu tối thiểu đối với các tác nhân ở phía sau (downstream) sử dụng hoặc chỉnh sửa phần mềm (‡1318). Ví dụ, các mô hình Llama của Meta có các điều kiện giấy phép mang tính hạn chế và chỉ bao gồm mã suy luận, không bao gồm mã huấn luyện; vì vậy, nhìn chung chúng không được xem là phần mềm nguồn mở (‡1319, ‡1320). Các lựa chọn phát hành mô hình tồn tại trên một phổ từ hoàn toàn đóng cho đến hoàn toàn là phần mềm nguồn mở, với các đánh đổi rủi ro - lợi ích khác nhau tại từng điểm (‡1086*, ‡1320, ‡1321). Bàn 3.9 mô tả các lựa chọn này.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>skyblue|black|left|12|15|bb Hoàn toàn đóng kín
  Người dùng không thể tương tác trực tiếp với mô hình theo bất kỳ cách nào
  Ví dụ: Flamingo (Google)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>paleturquoise|black|left|12|15|bb Truy cập được lưu trữ
  Người dùng chỉ có thể tương tác thông qua một ứng dụng hoặc giao diện cụ thể, chẳng hạn như một ứng dụng chatbot trên thiết bị di động
  Ví dụ: Midjourney v7 (Midjourney)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>powderblue|black|left|12|15|bb Truy cập API tới mô hình
  Người dùng có thể gửi yêu cầu đến mô hình thông qua mã lệnh, cho phép sử dụng trong các ứng dụng bên ngoài
  Ví dụ: Claude 4 (Anthropic)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightblue|black|left|12|15|bb Truy cập API để tinh chỉnh mô hình
  Người dùng có thể tinh chỉnh mô hình cho các nhu cầu cụ thể của họ
  Ví dụ: GPT-5 (OpenAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>lightcyan|black|left|12|15|bb Mở trọng số: trọng số có sẵn để tải xuống
  Người dùng có thể tải xuống và chạy mô hình trên máy tính của riêng họ
  Ví dụ: Llama 4 (Meta), DeepSeek R1 (DeepSeek)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>snow|black|left|12|15|bb Trọng số, dữ liệu và mã nguồn có sẵn để tải xuống kèm theo các hạn chế sử dụng
  Người dùng có thể tải xuống và chạy mô hình cũng như mã suy luận và huấn luyện, nhưng có một số hạn chế theo giấy phép đối với việc sử dụng của họ
  Ví dụ: BLOOM (BigScience)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mở hoàn toàn: có thể tải xuống trọng số, dữ liệu và mã nguồn mà không có bất kỳ hạn chế nào về sử dụng
  Người dùng có toàn quyền tải xuống, sử dụng và sửa đổi mô hình, toàn bộ mã nguồn và dữ liệu
  Ví dụ: GPT-NeoX (EleutherAI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.9: Các tùy chọn chia sẻ mô hình từ hoàn toàn đóng đến hoàn toàn mở
>white|black||9|11|br Một lựa chọn minh họa về các tùy chọn chia sẻ mô hình, trải dài từ các mô hình hoàn toàn đóng (mô hình riêng tư và chỉ được lưu giữ để sử dụng độc quyền) đến các mô hình hoàn toàn mở và mô hình mã nguồn mở (trọng số mô hình, dữ liệu và mã nguồn được cung cấp công khai và miễn phí, không bị hạn chế về việc sử dụng, sửa đổi và chia sẻ). Các mô hình thuộc bốn danh mục đầu tiên thường được gọi là ‘đóng’. Phần này tập trung vào ba hàng cuối. Nguồn: được chuyển thể từ Bommasani, 2024 (‡1317).


###@ Lợi ích và rủi ro

>white|orangered|left|14|15.5|bb Các mô hình open-weight có thể được tuỳ chỉnh và đánh giá dễ dàng hơn

Các mô hình mã nguồn mở (open-weight models) mang lại nhiều lợi ích đáng kể cho nghiên cứu, đổi mới và khả năng tiếp cận. Như đã thảo luận ở §1.1. AI đa năng (What is general-purpose AI?), việc huấn luyện các mô hình AI đa năng là vô cùng tốn kém – các mô hình hàng đầu có thể tốn hàng trăm triệu đô la để phát triển. Việc phát hành công khai trọng số mô hình cho phép các tác nhân có nguồn lực hạn chế hơn có thể sao chép, nghiên cứu và xây dựng trên các hệ thống hiện có. Nếu thiếu quyền truy cập như vậy, các cộng đồng ở các khu vực có nguồn lực thấp có nguy cơ bị loại khỏi những lợi ích mà AI mang lại, do đó trọng số mở là yếu tố quan trọng để tạo điều kiện cho sự tham gia trên phạm vi toàn cầu của đa số người dân trong quá trình phát triển AI (‡1322). Các nhà phát triển ở lớp ứng dụng tiếp theo (downstream developers) có thể tinh chỉnh các mô hình cho nhiều ứng dụng đa dạng, ví dụ, điều chỉnh chúng cho các ngôn ngữ thiểu số ít được hỗ trợ hoặc tối ưu hiệu năng cho các tác vụ cụ thể như soạn thảo văn bản pháp lý hoặc ghi chú y tế (‡1323, ‡1324*). Nhờ đó, các mô hình có trọng số mở có thể cho phép nhiều người và cộng đồng sử dụng và hưởng lợi từ AI hơn so với khả năng có thể đạt được nếu không có chúng (‡1325). Trong trường hợp các mô hình không đủ năng lực để gây nguy hiểm, những lợi ích này có thể lớn hơn rủi ro bổ sung của việc phát hành trọng số một cách công khai, mặc dù điều này còn tùy thuộc vào mức độ chịu rủi ro của các bên ra quyết định liên quan.

Việc phát hành mô hình mã nguồn mở cũng mở rộng nhóm các nhà phát triển và nhà nghiên cứu có khả năng nghiên cứu mô hình, đánh giá các năng lực của mô hình, kiểm thử các lỗ hổng và cải tiến theo vòng lặp (‡1326, ‡1327). Điều này làm tăng khả năng các ứng dụng có lợi và các khiếm khuyết gây hại được phát hiện, mặc dù điều đó không được đảm bảo (‡1328, ‡1329). Người dùng cũng có thể chạy các mô hình mã nguồn mở trên thiết bị của riêng họ, cho phép họ duy trì quyền kiểm soát đối với dữ liệu nhạy cảm và tránh phải gửi dữ liệu đó tới các máy chủ của bên thứ ba.

Có thêm các lợi ích khi các nhà phát triển chia sẻ thông tin như dữ liệu huấn luyện, mã nguồn, công cụ đánh giá và tài liệu cũng như trọng số của mô hình (‡1320, ‡1330, ‡1331, ‡1332*). Với nhiều thông tin hơn, các nhà phát triển ở phía sau và các nhà nghiên cứu khác có thể hiểu rõ hơn các mô hình mã nguồn mở và thích nghi chúng cho các ứng dụng mới.

>white|orangered|left|14|15.5|bb Các biện pháp bảo vệ của các mô hình open-weight dễ bị loại bỏ hơn, cho phép sử dụng sai mục đích tiềm ẩn

Các mô hình trọng số mở cũng đặt ra thêm rủi ro, vì các cơ chế bảo vệ của chúng dễ bị gỡ bỏ hơn. Mặc dù cả mô hình trọng số mở và mô hình trọng số đóng đều có thể có cơ chế bảo vệ để từ chối các yêu cầu gây hại từ người dùng, nhưng các cơ chế bảo vệ này dễ bị gỡ bỏ đối với mô hình trọng số mở hơn nhiều. Kẻ độc hại có thể tinh chỉnh một mô hình để tối ưu hiệu năng cho các ứng dụng gây hại, gỡ bỏ các phần của mã được thiết kế để ngăn việc sử dụng gây hại, hoặc hoàn tác việc tinh chỉnh an toàn trước đó (‡1156, ‡1160, ‡1161, ‡1333, ‡1334, ‡1335, ‡1336, ‡1337, ‡1338). Do đó, trọng số của mô hình mở có thể làm gia tăng các rủi ro bị lạm dụng đã được thảo luận trong §2.1. Rủi ro do bị sử dụng độc hại có thể tăng lên khi cho phép nhiều tác nhân hơn tận dụng và mở rộng các năng lực hiện có cho mục đích gây hại mà không có sự giám sát (‡1122, ‡1315). Mặc dù nhiều người dùng sẽ không có kỹ năng hoặc động lực để gỡ bỏ cơ chế bảo vệ trên các mô hình trọng số mở, nhưng các tác nhân độc hại có động cơ mạnh vẫn là một mối lo ngại. Ngoài ra, kẻ độc hại cũng có thể sử dụng các mô hình trọng số mở để xác định các lỗ hổng trong các mô hình trọng số đóng tương tự (‡1055*). Những khiếm khuyết này khó phát hiện hơn khi chỉ chạy các mô hình trọng số đóng, do các biện pháp kiểm soát và giám sát chặt chẽ hơn mà nhà cung cấp mô hình trọng số đóng có thể triển khai.

>white|orangered|left|14|15.5|bb Việc chia sẻ trọng số của mô hình là không thể đảo ngược

Khi trọng số mô hình đã có sẵn để tải xuống công khai, không còn cách nào để thực hiện một đợt hoàn toàn quay lui (rollback) cho tất cả các bản sao hiện có. Các nền tảng lưu trữ trên Internet như GitHub và Hugging Face có thể xóa mô hình khỏi nền tảng của họ, khiến một số tác nhân khó tìm các bản sao có thể tải xuống, đồng thời tạo ra một rào cản đáng kể đối với nhiều người dùng độc hại ngẫu nhiên (‡1339). Tuy nhiên, các tác nhân có động cơ vẫn có thể nhận được bản sao nếu mô hình đã được tải xuống và được lưu trữ lại (rehost) ở nơi khác hoặc được lưu cục bộ. Hơn nữa, các nhà phát triển tuyến dưới (downstream) tích hợp các mô hình có trọng số mở (open-weight) vào hệ thống của họ cũng sẽ thừa hưởng mọi khiếm khuyết, chẳng hạn như tính dễ bị tổn thương trước các cuộc tấn công đối kháng (adversarial attacks) (‡1055) hoặc khả năng của mô hình để vượt qua các hệ thống giám sát (xem §2.2.2. Loss of control) (‡1315). Khác với các mô hình đóng (closed models), nơi các máy chủ có thể triển khai các bản vá một cách phổ quát, các nhà phát triển mô hình có trọng số mở không thể đảm bảo rằng các bản cập nhật sẽ được người dùng chấp nhận.

###@ Cập nhật

Kể từ khi phát hành Báo cáo trước đó (tháng 1/2025), khoảng cách năng lực giữa các mô hình mã nguồn mở hàng đầu và các mô hình đóng đã thu hẹp. Các nhà phát triển Trung Quốc đặc biệt trở thành những nhà cung cấp quan trọng của các mô hình mã nguồn mở. Tháng 1/2025, DeepSeek đã phát hành mô hình R1 của mình, đạt hiệu năng tương đương với OpenAI’s o1 trên một số bộ đo điểm chuẩn (‡1340). Các mô hình Qwen của Alibaba cũng đã dần được đón nhận, chiếm vị trí số 1 cho một mô hình mã nguồn mở trên Chatbot Arena, một bộ đo hiệu năng được sử dụng rộng rãi, tính đến tháng 8/2025 (‡1341, ‡1342*). Tháng 8/2025, OpenAI đã phát hành các mô hình mã nguồn mở đầu tiên của mình kể từ khi phát hành GPT-2 vào năm 2019, gpt-oss-120b và gpt-oss-20b. Meta đã tiếp tục phát hành các mô hình Llama với trọng số mã nguồn mở. Hiện nay, năng lực của các mô hình đóng hàng đầu được ước tính là kém hơn chưa đầy 1 năm so với các mô hình mã nguồn mở hàng đầu trên các bộ đo điểm chuẩn AI nổi bật (Nhân vật 3.10).

###@ Khoảng trống bằng chứng

Một khoảng trống bằng chứng quan trọng liên quan đến hiệu quả trong thế giới thực của các giải pháp kỹ thuật nhằm ngăn chặn việc lạm dụng các mô hình trọng lượng mở. Các nhà nghiên cứu đã đề xuất nhiều cách tiếp cận khác nhau để làm cho các mô hình có khả năng chống can thiệp. Điều này bao gồm các kỹ thuật huấn luyện mới được thiết kế để khiến mô hình có khả năng chống lại việc chỉnh sửa gây hại (‡1276), lọc nội dung gây hại khỏi dữ liệu huấn luyện (‡55), và các biện pháp phòng vệ chống jailbreak (‡675, ‡676). Hiện nay, các kỹ thuật này đang được áp dụng trong các bản phát hành ngoài đời thực từ các nhà phát triển lớn. Chẳng hạn, OpenAI đã áp dụng một số kỹ thuật này trong các mô hình gpt-oss của họ, báo cáo rằng các phiên bản được fine-tune một cách đối kháng không đạt ngưỡng năng lực cao (‡1344*). Tuy nhiên, nghiên cứu đã chỉ ra rằng các đối tượng xấu có thể vô hiệu hóa các cơ chế bảo vệ bằng cách huấn luyện lại mô hình trên các ví dụ gây hại (‡1345, ‡1346). Hơn nữa, vẫn còn khó khăn để đánh giá một cách đáng tin cậy độ bền vững của các cơ chế bảo vệ, do đó tính hiệu quả của chúng trước các cuộc tấn công trong thế giới thực vẫn còn chưa chắc chắn (‡1159).

![figure 3.10](images/fig3.10_epoch_capabilities_index.png)

##### Nhân vật vật 3.10: Khoảng cách năng lực giữa các mô hình AI mã nguồn mở hàng đầu và các mô hình AI đóng
>white|black||9|11|br Điểm số chỉ số năng lực theo epoch (Epoch Capabilities Index - ECI) của các mô hình mã nguồn mở hiệu suất cao (màu xanh đậm) và các mô hình đóng (màu xanh nhạt) theo thời gian. ECI kết hợp điểm số từ 39 bộ chuẩn đánh giá thành một thang năng lực tổng quát. Các mô hình mã nguồn mở tốt nhất thua các mô hình đóng khoảng 1 năm. Nguồn: Epoch AI, 2025 (‡1343).


###@ Giảm thiểu

Các biện pháp giảm thiểu kỹ thuật cho rủi ro của các mô hình trọng số mở hoạt động xuyên suốt quá trình phát triển và triển khai AI (‡1141, ‡1195, ‡1347). Ví dụ, khi các mô hình đang được phát triển, các nhà phát triển và các bộ chuyển đổi (adapters) ở tuyến sau có thể lọc nội dung nhạy cảm khỏi dữ liệu huấn luyện để giảm thiểu các khả năng gây hại. Việc loại bỏ các ví dụ gây hại khỏi dữ liệu huấn luyện của một mô hình có thể ngăn chặn fine-tuning đối kháng (adversarial fine-tuning) hiệu quả hơn 10 lần so với các biện pháp phòng vệ được bổ sung sau huấn luyện, dù điều đó cũng có thể ảnh hưởng đến các khả năng có lợi (‡55). Các nhà cung cấp ứng dụng AI cũng có thể triển khai các cơ chế báo cáo sự cố và phản hồi (‡1348).

Ngoài ra, các nền tảng lưu trữ như HuggingFace và GitHub có thể thiết lập các điều khoản dịch vụ của nền tảng để loại bỏ các mô hình đã được sửa đổi cho mục đích gây hại (‡1141, ‡1324). Các nhà phát triển mô hình có thể cung cấp toàn bộ quyền truy cập cho các bên kiểm tra (auditors) trước khi phát hành, hoặc chọn một chiến lược phát hành “theo giai đoạn” – phát hành các mô hình cho các nhóm ngày càng lớn (‡1086). Điều này có thể giúp xác định các sự cố vận hành tiềm ẩn hoặc lỗ hổng bảo mật trước khi mô hình được phổ biến rộng rãi (‡1161, ‡1286).

>oldlace|black||11|15|br      
####@ Ghi chú vật 3.1: Bảo mật trọng số mô hình
>oldlace|black|left|13|15|hb Ghi chú vật 3.1: Bảo mật trọng số mô hình
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Những rủi ro được thảo luận trong phần này giả định rằng các trọng số của mô hình được phát hành một cách có chủ đích. Tuy nhiên, các trọng số mô hình dạng đóng cũng có thể trở nên sẵn có thông qua hành vi trộm cắp hoặc rò rỉ. Các mô hình đóng phải tốn hàng trăm triệu đô la để phát triển (§1.1. AI đa năng là gì?) và, trung bình, có năng lực cao hơn so với các mô hình trọng số mở (‡1343). Điều này khiến chúng trở thành mục tiêu hấp dẫn đối với các tác nhân trải dài từ tin tặc nghiệp dư cho đến các quốc gia tìm cách có được các mô hình AI hàng đầu.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Việc đánh cắp các trọng số mô hình đóng (closed model weights) sẽ gây ra những rủi ro tương tự như các rủi ro được mô tả ở trên đối với các mô hình trọng số mở (open-weight models), nhưng có thể là không có bất kỳ biện pháp giảm thiểu nào. Các tác nhân độc hại có thể loại bỏ các biện pháp bảo vệ khỏi những mô hình có năng lực cao nhất. Không giống như các nhà phát triển hợp pháp, những tác nhân như vậy sẽ không phải chịu các ràng buộc về uy tín, pháp lý hoặc thương mại mà hiện đang thúc đẩy các công ty AI ở tuyến đầu triển khai mô hình của họ một cách an toàn.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Mức độ bảo mật hiện tại khác nhau giữa các ngành, và có thể không đủ để chống lại các kẻ tấn công tinh vi. Một số nhà phát triển cam kết bảo vệ trọng số mô hình trước các tổ chức tội phạm mạng và các mối đe dọa từ nội bộ (‡582), trong khi những người khác không đưa ra bất kỳ cam kết bảo mật công khai nào (‡1109, ‡1349). Nghiên cứu cho thấy các trung tâm dữ liệu AI có thể không thể chịu được các cuộc tấn công từ những tác nhân tinh vi nhất và có nguồn lực dồi dào (‡582, ‡1350, ‡1351). Tính đến tháng 12 2025, chưa có trường hợp nào được xác nhận và có tài liệu công khai về việc đánh cắp trọng số mô hình. Tuy nhiên, các vụ vi phạm bảo mật khác tại các công ty AI hàng đầu đã được báo cáo, bao gồm việc xâm nhập vào hệ thống email của Microsoft (‡1352).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Việc đóng các lỗ hổng an ninh này sẽ đòi hỏi những khoản đầu tư đáng kể vào phần cứng, phần mềm, nhân sự và an ninh cơ sở vật chất. Một số biện pháp tăng cường an ninh có thể được triển khai tương đối nhanh với sự phối hợp đồng bộ (‡1122). Tuy nhiên, các biện pháp quan trọng khác, như bảo đảm chuỗi cung ứng phần cứng và các cơ sở vật chất, có thể sẽ mất nhiều năm (‡1122). Các công ty tư nhân cũng có thể thiếu nguồn lực hoặc thông tin để tự mình phát triển các biện pháp bảo vệ phù hợp. Ví dụ, các nhà phát triển AI không có quyền truy cập vào tình báo mối đe dọa đã được phân loại mà các chính phủ có (‡1349, ‡1353*).
>oldlace|black||11|15|br      


###@ Thách thức đối với các nhà hoạch định chính sách

Một thách thức then chốt đối với các nhà hoạch định chính sách là bảo đảm các lợi ích của việc chia sẻ mô hình trọng số công khai (open-weight) mà không làm tăng đáng kể rủi ro. Để tránh gây ra hậu quả thảm khốc, các nhà phát triển mô hình trọng số công khai không nên phát hành mô hình mà chưa đánh giá rủi ro, vừa sử dụng các phương pháp đánh giá đã được áp dụng cho mô hình đóng (closed models), vừa tiến hành thêm các thử nghiệm, trong bối cảnh các tác nhân xấu có thể tinh chỉnh (fine-tune) mô hình và loại bỏ các cơ chế bảo vệ an toàn. Trên thực tế, điều này có thể khó khăn vì các tiến bộ về năng lực có thể không đoán trước được, việc phát hành trọng số công khai là không thể đảo ngược, và cần có nỗ lực đánh giá để dự đoán thời điểm một lần phát hành có thể gây ra mức độ nguy hại tiềm tàng đáng kể. Một cách tiếp cận là đánh giá “rủi ro biên” (marginal risk) của các lần phát hành công khai: mức độ mà việc phát hành đó, trên cơ sở phảnfactual (counterfactually), làm gia tăng rủi ro đối với xã hội so với mức rủi ro vốn đã do các mô hình hiện có hoặc các công nghệ khác gây ra (‡556, ‡1033, ‡1354, ‡1355) (xem §3.2. Các thực hành quản lý rủi ro). Tuy nhiên, việc ước tính một hệ thống sẽ làm tăng hoặc giảm rủi ro ở các bước triển khai tiếp theo (downstream) như thế nào sau khi đã được triển khai là phức tạp và phụ thuộc mạnh vào bối cảnh. Những gia tăng rủi ro theo từng bước một qua các lần phát hành liên tiếp có thể tích lũy theo thời gian thành mức tăng đáng kể về tổng rủi ro, ngay cả khi rủi ro biên gắn với từng lần phát hành riêng lẻ có vẻ chấp nhận được (‡1356, ‡1357).

Tính hai mặt (dual-use) của năng lực AI còn làm phức tạp việc quản trị: các tính năng cho phép các ứng dụng có lợi trong y học hoặc nghiên cứu có thể bị chuyển hướng để gây hại, và khi trọng số đã được công khai, việc phân biệt sử dụng hợp pháp với sử dụng độc hại có thể trở nên khó khăn. Đồng thời, cũng chưa rõ ai nên chịu trách nhiệm giải trình khi các mô hình trọng số công khai được sửa đổi cho mục đích gây hại.

