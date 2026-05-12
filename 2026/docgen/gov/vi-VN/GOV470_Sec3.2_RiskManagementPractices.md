##########
>white|orangered|left|14|30|hr Mục 3.2
### 3.2. Các thực hành quản lý rủi ro
>white|orangered|left|24|30|hb Các thực hành quản lý rủi ro

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Quản lý rủi ro AI đa mục đích bao gồm nhiều hoạt động được sử dụng để xác định, đánh giá và giảm thiểu rủi ro từ AI đa mục đích. Chúng bao gồm kiểm thử và đánh giá ở cấp độ mô hình (chẳng hạn như “red-teaming”), các quy trình của tổ chức hướng dẫn các quyết định phát triển và phát hành, các cơ chế bảo vệ mang tính điều kiện (chẳng hạn như các cam kết “if-then”), và báo cáo sự cố.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Một số nhà phát triển AI đã xây dựng các Khung An toàn AI Cạnh tranh. Các khung này bao gồm thông tin về đánh giá rủi ro và nêu các biện pháp mang tính điều kiện như các hạn chế truy cập mà các công ty dự định triển khai đối với các mô hình có năng lực cao hơn. Chúng khác nhau về các rủi ro mà chúng bao phủ, cách chúng xác định các ngưỡng năng lực, và những hành động nào được kích hoạt khi đạt đến các ngưỡng đó.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bằng chứng về hiệu quả thực tế của các thực hành quản lý rủi ro AI vẫn còn hạn chế. Việc thiếu báo cáo sự cố và giám sát khiến việc đánh giá xem các thực hành hiện tại có giảm rủi ro tốt đến mức nào, hoặc chúng có được triển khai một cách nhất quán hay không, trở nên khó khăn.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi phát hành Báo cáo gần đây nhất (tháng 1 năm 2025), quản lý rủi ro đã trở nên có cấu trúc hơn thông qua các sáng kiến mới về ngành và quản trị. Các công cụ mới như Bộ quy tắc thực hành về AI đa mục đích của EU, Khung quản trị An toàn AI của Trung Quốc 2.0, và Khung Báo cáo Quy trình AI Hiroshima của G7, cùng với các sáng kiến do công ty dẫn dắt, cho thấy xu hướng chuyển dịch sang các cách tiếp cận được chuẩn hoá hơn đối với tính minh bạch, đánh giá và báo cáo sự cố.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Động lực thị trường và tốc độ phát triển AI đặt ra thêm các thách thức. Do sức ép cạnh tranh, các công ty AI có thể phải cân nhắc đánh đổi giữa việc phát hành sản phẩm nhanh hơn và việc đầu tư cho các nỗ lực giảm thiểu rủi ro. Nhiều tác hại liên quan đến AI cũng bị chuyển ra bên ngoài, và trách nhiệm pháp lý đối với các tác hại này vẫn chưa rõ ràng; đồng thời các quy trình quản trị có thể chậm thích nghi với những thay đổi trong bối cảnh AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Những thách thức chính đối với các nhà hoạch định chính sách bao gồm việc ưu tiên giữa các rủi ro đa dạng do AI đa năng (general-purpose AI) gây ra, và làm rõ các chủ thể trong chuỗi giá trị AI (AI value chain) nào được định vị tốt nhất để giảm thiểu chúng. Những thách thức này còn bị gia tăng bởi tầm nhìn hạn chế về cách các rủi ro được nhận diện, đánh giá và quản lý trong thực tiễn, cũng như việc chia sẻ thông tin bị phân mảnh giữa các nhà phát triển, đơn vị triển khai và các nhà cung cấp hạ tầng.
>oldlace|black||11|15|br      


Quản lý rủi ro AI bao gồm một loạt các hoạt động nhằm xác định, đánh giá và giảm thiểu khả năng xảy ra cũng như mức độ nghiêm trọng của các rủi ro liên quan đến các hệ thống AI. Các hoạt động này có thể được triển khai bởi các nhà phát triển AI, đơn vị triển khai, bên đánh giá và các cơ quan quản lý. Ví dụ bao gồm mô hình hóa mối đe dọa, phân tầng rủi ro, red-teaming, kiểm toán, và báo cáo sự cố. Phần này trình bày các thực hành quản lý rủi ro hiện tại, các phát triển mới và các hạn chế còn tồn tại.

Kể từ đầu năm 2025, một số sáng kiến quốc tế mới về quản lý rủi ro AI đa mục đích đã được phát triển, bao gồm các khuôn khổ về minh bạch tổ chức và báo cáo rủi ro, cũng như các khuôn khổ về quy định và quản trị.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Nhân vật vật 3.4: Bốn thành phần của quản lý rủi ro
>white|black||9|11|br Bốn nhóm phương pháp quản lý rủi ro cho AI đa mục đích: xác định rủi ro; phân tích và đánh giá rủi ro; giảm thiểu rủi ro; và quản trị rủi ro. Các nhóm này tạo thành một quá trình lặp đi lặp lại và mang tính chu kỳ. Quản trị rủi ro, được thể hiện ở trung tâm, giúp đảm bảo sự thành công của các thành phần khác. Nguồn: International AI Safety Report 2026.


Những thách thức còn lại bao gồm việc thiếu chuẩn hoá ở mức độ nhất định, gây khó khăn cho việc tuân thủ và đánh giá, cũng như thiếu bằng chứng về hiệu quả trong thế giới thực. Hơn nữa, bối cảnh thể chế, văn hoá và chính trị khác nhau trên toàn cầu, điều này hàm ý rằng các phương pháp xác định và quản lý rủi ro, bao gồm cả ngưỡng rủi ro chấp nhận được, có thể thay đổi giữa các khu vực. Phần này mô tả các cách tiếp cận quản lý rủi ro: nhằm cung cấp thông tin cho các chủ thể trong hệ sinh thái AI về các cách tiếp cận toàn cầu hiện tại đối với quản lý rủi ro. Khi có sẵn, các bằng chứng về hiệu quả và những hạn chế của các cách tiếp cận này sẽ được thảo luận, nhưng các khuyến nghị chính sách nằm ngoài phạm vi của công việc này.

###@ Thành phần của quản lý rủi ro

Quản lý rủi ro là một quá trình lặp đi lặp lại với các hoạt động và phương pháp trải suốt toàn bộ vòng đời phát triển và triển khai AI, nhưng chúng hoạt động phối hợp với nhau một cách nhất quán (‡969). Quản lý rủi ro cho AI mục đích chung có thể bao gồm vai trò của nhiều nhóm tác nhân khác nhau, bao gồm các nhà khoa học dữ liệu, kỹ sư mô hình, kiểm toán viên, chuyên gia lĩnh vực, lãnh đạo, người dùng cuối, các cộng đồng bị ảnh hưởng, nhà cung cấp bên thứ ba, các nhà hoạch định chính sách, chính phủ, các tổ chức tiêu chuẩn, và các tổ chức xã hội dân sự (‡970, ‡971, ‡972). Các chuẩn mực hàng đầu về quản lý rủi ro thường có khả năng tương tác với nhau, nhưng sử dụng các thuật ngữ khác nhau để mô tả các thành phần của quản lý rủi ro (‡973, ‡974). Thông thường, chúng có bốn thành phần liên kết với nhau (Nhân vật 3.4): xác định; phân tích và đánh giá; giảm thiểu; và quản trị rủi ro (‡970, ‡973, ‡975, ‡976). Các bảng bên dưới cung cấp các ví dụ minh họa về các phương pháp, kỹ thuật và công cụ liên quan. Các hoạt động tiếp tục được phát triển, do đó các bảng không phải là đầy đủ, và mức độ áp dụng sẽ khác nhau tùy theo bối cảnh.

###@ Nhận diện rủi ro

Nhận diện rủi ro là quá trình tìm kiếm, nhận biết, và mô tả các rủi ro. Nhận diện rủi ro toàn diện thường bao gồm các đánh giá dựa trên năng lực, trong đó kiểm tra xem các mô hình có hay không các năng lực nguy hiểm cụ thể (‡977), cũng như mô hình hoá rủi ro (‡978) và dự báo (‡715*), được dùng để khám phá các rủi ro hiện có và rủi ro mới nổi. Bàn 3.1 cung cấp nhiều ví dụ khác nhau về các thực hành nhận diện rủi ro. Nhận diện rủi ro cũng dựa trên việc trao đổi với các chuyên gia và cộng đồng liên quan để hiểu bối cảnh rộng hơn về cách các rủi ro hình thành (‡979, ‡980). Các cơ chế như chương trình săn lỗi có thưởng (bug bounty programmes) có thể hỗ trợ quá trình này bằng cách tạo động lực để phát hiện các lỗ hổng chưa từng được biết đến trước đó (‡981) (Bàn 3.1). Một mục tiêu then chốt của nhận diện rủi ro là tính đến cả những rủi ro đã được biết rõ, đã được hiểu rõ lẫn các rủi ro tiềm năng trong tương lai mà vẫn chưa chắc chắn hoặc chưa được mô tả đầy đủ (‡982). Điều này đặc biệt quan trọng đối với AI đa dụng, nơi nhiều rủi ro có thể vẫn chưa được hiểu hoàn toàn hoặc chưa thể quan sát được (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chương trình bug bounty
  Các chương trình thưởng lỗi (bug bounties) hoặc công bố lỗ hổng (vulnerability disclosure) khuyến khích mọi người tìm và báo cáo các lỗ hổng trong các hệ thống AI. Một số nhà phát triển đã triển khai các chương trình thưởng lỗi (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tư vấn chuyên gia
  Các chuyên gia trong lĩnh vực, người dùng và các cộng đồng bị ảnh hưởng cung cấp thông tin chi tiết về các rủi ro có khả năng xảy ra. Có các hướng dẫn mới nổi cho AI tham gia và hòa nhập (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sơ đồ xương cá (Ishikawa)
  Biểu đồ xương cá là các công cụ phân tích nguyên nhân gốc rễ đã được thiết lập tốt, và các nhà nghiên cứu đã đề xuất sử dụng chúng để phân tích có cấu trúc các sự cố rủi ro AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dự báo
  Dự báo là quá trình dự đoán các sự kiện hoặc xu hướng trong tương lai dựa trên việc phân tích dữ liệu trong quá khứ và hiện tại. Nó đã được sử dụng để so sánh mức độ có khả năng tương đối của, ví dụ, các kết quả kinh tế khác nhau nhờ AI tiên tiến (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phân loại rủi ro
  Các phân loại rủi ro là một cách để phân nhóm và tổ chức các rủi ro theo nhiều chiều khác nhau. Có một số phân loại đưa ra rủi ro từ AI đa mục đích (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lập kế hoạch theo kịch bản
  Lập kế hoạch theo kịch bản bao gồm việc xây dựng các kịch bản tương lai khả dĩ và phân tích cách thức các rủi ro hình thành. Điều này đã được sử dụng để khám phá các rủi ro và tác động của các mô hình AI (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lập mô hình mối đe dọa
  Mô hình hóa mối đe dọa là một quy trình nhằm xác định các mối đe dọa và lỗ hổng đối với một hệ thống. Nhiều nhà phát triển AI nhấn mạnh việc sử dụng mô hình hóa mối đe dọa để dự đoán các kịch bản lạm dụng tiềm ẩn của các hệ thống AI (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.1: Ví dụ nhận diện rủi ro trong quản lý rủi ro AI đa mục đích
>white|black||9|11|br Các phương pháp mẫu để nhận diện rủi ro AI được liệt kê theo thứ tự bảng chữ cái. Các phương pháp bao gồm
được thiết kế để hỗ trợ việc xác định rủi ro cho nhiều loại rủi ro khác nhau, bao gồm rủi ro do sử dụng với mục đích độc hại, rủi ro do trục trặc và rủi ro mang tính hệ thống. Do tính còn sơ khai của quản lý rủi ro đối với trí tuệ nhân tạo đa mục đích nói chung, không phải mọi phương pháp đều phù hợp với mọi nhà phát triển hoặc bên triển khai AI.


>white|orangered|left|14|15.5|bb Mô hình hóa mối đe dọa và các phân loại rủi ro là các phương pháp nhận diện rủi ro nổi bật

Hai phương pháp nổi bật để xác định các rủi ro từ AI đa mục đích là mô hình hoá mối đe doạ trong International AI Safety Report 2026 (một quy trình có cấu trúc để lập bản đồ cách các rủi ro liên quan đến AI có thể hiện thực hoá) và các phân loại rủi ro (risk taxonomies). Ví dụ, Meta sử dụng các buổi thực hành mô hình hoá mối đe doạ để dự đoán các kịch bản lạm dụng tiềm năng của các mô hình AI của mình (‡990), và Anthropic đưa mô hình hoá mối đe doạ vào như một phần của ASL-3 Deployment Standard (‡991). Các phân loại rủi ro và nguy hại của AI, vốn liệt kê các nhóm rủi ro và ví dụ, cũng có thể đóng vai trò như một điểm khởi đầu để khái niệm hoá, nhận diện và xác định các rủi ro then chốt gắn với AI đa mục đích trong các lĩnh vực ứng dụng cụ thể (‡906, ‡988, ‡992, ‡993).

###@ Phân tích và đánh giá rủi ro

Phân tích và đánh giá rủi ro là quá trình xác định mức độ rủi ro của một mô hình hoặc hệ thống AI và so sánh nó với các tiêu chí đã được thiết lập để đánh giá tính chấp nhận được hoặc sự cần thiết phải có biện pháp giảm thiểu (‡994, ‡995, ‡996, ‡997). Nó bao gồm các hoạt động như đo lường hiệu năng mô hình trên các bộ chuẩn (‡998) và các đánh giá (‡176, ‡715), tiến hành các bài kiểm thử đỏ (‡999*), đánh giá tác động (‡1000) và kiểm toán (‡1001, ‡1002). Xem Bàn 3.2 để biết các ví dụ về phân tích và đánh giá rủi ro AI đa mục đích. Các phương pháp được thiết kế để hỗ trợ phân tích và đánh giá đồng thời cho nhiều loại rủi ro khác nhau.

Các mục tiêu chính của phân tích và đánh giá rủi ro là thực hiện các đánh giá về năng lực và các lỗ hổng của mô hình (‡1003), sử dụng mô hình hóa rủi ro vững chắc để đưa ra quyết định về các ngưỡng rủi ro (‡1004, ‡1005), và hiểu cách các hệ thống AI được sử dụng trong thực tế nhằm đánh giá các tác động xã hội tiếp diễn (‡869, ‡904, ‡905, ‡1006). Các quy trình phân tích và đánh giá rủi ro thường được xem là có khả năng xác định rủi ro cao hơn khi chúng tích hợp việc xem xét độc lập (‡1001, ‡1007), dựa trên chuyên môn liên ngành (‡1008), và bao gồm các quan điểm đa dạng từ nhiều lĩnh vực và ngành học, cũng như từ các cộng đồng bị ảnh hưởng (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kiểm toán
  Các cuộc kiểm toán là các đánh giá chính thức về hiệu suất và tác động của các mô hình AI và/hoặc về việc một tổ chức tuân thủ các tiêu chuẩn, chính sách và quy trình, được thực hiện nội bộ hoặc bởi một bên bên ngoài. Kiểm toán AI là một lĩnh vực đang phát triển, và có nhiều công cụ và thực hành tồn tại để kiểm toán các mô hình AI cũng như các thực hành của các nhà phát triển mô hình AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chuẩn đánh giá
  Các benchmark được tiêu chuẩn hóa, thường là các bài kiểm tra hoặc chỉ số định lượng dùng để đánh giá và so sánh hiệu suất của các hệ thống AI trên một tập tác vụ cố định được thiết kế để phản ánh việc sử dụng trong thế giới thực (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phương pháp Bowtie
  Phương pháp bowtie là một phương pháp nổi tiếng để trực quan hóa nơi có thể thêm các biện pháp kiểm soát nhằm giảm thiểu các sự kiện rủi ro. Nó cung cấp sự phân biệt rõ ràng giữa quản lý rủi ro chủ động và quản lý rủi ro phản ứng (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phương pháp Delphi
  Phương pháp Delphi là một kỹ thuật ra quyết định theo nhóm sử dụng một chuỗi bảng câu hỏi để thu thập sự đồng thuận từ một nhóm chuyên gia (‡1020, ‡1021). Nó đã được sử dụng để giúp khám phá các kịch bản tương lai có thể xảy ra với AI tiên tiến (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Thử nghiệm thực địa
  Thử nghiệm thực địa đánh giá hiệu suất và tác động của một hệ thống AI trong môi trường vận hành thực tế. Một số nghiên cứu nhấn mạnh thử nghiệm thực địa như một sự bổ sung cho việc đánh giá mô hình nhằm xem xét các kết quả và hậu quả trong thế giới thực (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá tác động
  Đánh giá tác động đánh giá các tác động tiềm ẩn của một công nghệ hoặc dự án. Điều này có thể bao gồm việc định lượng, tổng hợp và ưu tiên các tác động. Chẳng hạn, Đạo luật AI của EU yêu cầu các nhà phát triển hệ thống AI có rủi ro cao thực hiện Đánh giá tác động về các quyền cơ bản (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá mô hình
  Đánh giá mô hình bao gồm các quy trình và bài kiểm tra nhằm đánh giá và đo lường hiệu suất của một mô hình AI trên một tác vụ cụ thể. Có rất nhiều đánh giá AI để đánh giá các năng lực và rủi ro khác nhau, bao gồm về an toàn, an ninh và tác động xã hội (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá rủi ro theo phương pháp xác suất
  Đánh giá rủi ro theo xác suất là một phương pháp luận để đánh giá các rủi ro liên quan đến các hệ thống hoặc quy trình phức tạp, có tính đến bất định. Nó đã được điều chỉnh cho các hệ thống AI tiên tiến (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Red-teaming
  Red-teaming là một hoạt động trong đó một nhóm người hoặc các hệ thống tự động đóng vai đối thủ và tấn công các hệ thống công nghệ của một tổ chức nhằm xác định các lỗ hổng. Nhiều công ty AI có các thực hành nội bộ để red-teaming các hệ thống AI (‡458, ‡1028). Red-teaming cũng có thể được thực hiện bởi các tác nhân bên ngoài công ty. Các đội này gặp thách thức như quyền truy cập hạn chế, nhưng cũng có thể làm lộ ra những hiểu biết khác biệt (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ma trận rủi ro
  Ma trận rủi ro là một công cụ trực quan để giúp ưu tiên các rủi ro dựa trên khả năng xảy ra và mức độ tác động tiềm ẩn (‡1027). Một số nhà phát triển AI bao gồm các ma trận rủi ro cơ bản trong Các Khung An toàn Frontier AI (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ngưỡng rủi ro/ cấp bậc rủi ro
  Ngưỡng rủi ro hoặc các hạng là các giới hạn định lượng hoặc định tính dùng để phân biệt rủi ro chấp nhận được với không chấp nhận được và kích hoạt các hành động quản lý rủi ro cụ thể khi các ngưỡng này bị vượt quá. Đối với AI đa mục đích, chúng được xác định dựa trên sự kết hợp của các năng lực, mức độ tác động, năng lực tính toán (compute), mức độ lan tỏa/tiếp cận (reach) và các yếu tố khác (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mức chịu đựng rủi ro
  Khả năng chịu rủi ro là mức độ rủi ro mà một tổ chức sẵn sàng chấp nhận. Trong AI, mức chịu rủi ro thường được thiết lập một cách ngầm thông qua các chính sách và thực tiễn của doanh nghiệp, trong khi một số chế độ quản lý quy định rõ ràng các rủi ro không thể chấp nhận được và gắn với các hậu quả pháp lý (‡1032). Một số công ty mô tả khả năng chịu rủi ro của mình theo thuật ngữ rủi ro biên của một mô hình mới; nghĩa là, mức độ mà một mô hình, một cách phản thực (counterfactually), làm gia tăng rủi ro vượt quá mức rủi ro vốn đã do các mô hình hiện có hoặc các công nghệ khác gây ra (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hồ sơ an toàn
  Hồ sơ an toàn (safety case) là một lập luận có cấu trúc, được hỗ trợ bởi bằng chứng, nhằm khẳng định rằng một hệ thống có thể được vận hành một cách chấp nhận được về mức độ an toàn trong một bối cảnh cụ thể. Các tài liệu gần đây (‡1037, ‡1038, ‡1039) đã nghiên cứu hồ sơ an toàn cho các hệ thống AI tiên phong và một số Khung An toàn AI Tiên phong (Frontier AI Safety Frameworks) có tham chiếu đến chúng (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb phân tích an toàn hệ thống
  Phân tích an toàn hệ thống làm nổi bật sự phụ thuộc giữa các thành phần và hệ thống mà chúng thuộc về, nhằm dự đoán cách các mối nguy cấp độ hệ thống có thể phát sinh từ lỗi của thành phần hoặc quy trình, hoặc từ các tương tác giữa các phân hệ, các yếu tố con người và điều kiện môi trường. Các cách tiếp cận được áp dụng cho các hệ thống AI trong tài liệu bao gồm phân tích quy trình theo lý thuyết hệ thống (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.2: Phân tích/đánh giá rủi ro trong quản lý rủi ro AI đa mục đích
>white|black||9|11|br Ví dụ về các phương pháp phân tích/đánh giá rủi ro AI, được liệt kê theo thứ tự bảng chữ cái. Do tính còn non trẻ của quản lý rủi ro AI đa năng, không phải mọi phương pháp đều phù hợp với mọi nhà phát triển hoặc bên triển khai AI.


>white|orangered|left|14|15.5|bb Các công cụ phân tích rủi ro phổ biến bao gồm bộ chuẩn (benchmarks) và đánh giá mô hình

Các chuẩn điểm và đánh giá mô hình là các bài kiểm tra chuẩn hoá để đánh giá hiệu năng của các hệ thống AI đa mục đích trên các tác vụ cụ thể. Các nhà nghiên cứu đã phát triển nhiều loại chuẩn điểm và đánh giá, bao gồm các bộ câu hỏi trắc nghiệm nhiều lựa chọn khó, các bài toán về kỹ thuật phần mềm, và các tác vụ liên quan đến công việc trong môi trường văn phòng mô phỏng (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Các đánh giá năng lực gây hại (‡715) được dùng để đánh giá liệu một mô hình hay hệ thống AI đa mục đích có kiến thức hoặc kỹ năng đặc biệt nguy hiểm hay không, chẳng hạn như khả năng hỗ trợ trong các cuộc tấn công mạng (xem §2.1.3. Cyberattacks).

Các quyết định có tác động đặc biệt quan trọng của các công ty và chính phủ về việc phát hành mô hình một phần dựa trên các đánh giá này (‡1050, ‡1051, ‡1052). Tuy nhiên, các bộ chuẩn thường khác nhau đáng kể về chất lượng và phạm vi (‡998, ‡1003), và có thể khó đánh giá tính hợp lệ của chúng do nhiều hạn chế trong thực hành đánh chuẩn (‡902, ‡909, ‡1003, ‡1053*). Ví dụ, các bộ chuẩn có thể trở nên “bão hòa” – khi điểm của nhiều mô hình tiến sát điểm cao nhất – nghĩa là chúng không còn phân biệt mạnh giữa các mô hình. Các mô hình cũng ngày càng có khả năng nhận diện một số tác vụ như là các phép đánh giá và thể hiện các hành vi khác so với các hành vi mà chúng sẽ thể hiện trên các tác vụ tương tự trong bối cảnh triển khai do “nhận thức theo tình huống” (xem §2.2.2. Mất kiểm soát). Cuối cùng, các bộ chuẩn và các đánh giá có các hạn chế đã được ghi nhận rõ ràng: đặc biệt, chúng không nắm bắt được các rủi ro liên quan đến việc sử dụng AI đa mục đích trong các miền mới và cho các tác vụ mới, vì các điều kiện thử nghiệm khác nhau so với việc sử dụng trong thực tế ở những mức độ khác nhau (‡913) (xem §1.2. Current capabilities và §3.1. Technical and institutional challenges).

>white|orangered|left|14|15.5|bb Red-teaming cho phép đánh giá rủi ro cụ thể theo từng miền tốt hơn

Một phương pháp phổ biến khác để đánh giá rủi ro là red-teaming. “red team” là một nhóm người đánh giá được giao nhiệm vụ tìm kiếm các lỗ hổng, hạn chế, hoặc khả năng bị lạm dụng. Red-teaming có thể mang tính chuyên theo lĩnh vực và được thực hiện bởi các chuyên gia trong lĩnh vực đó, hoặc mở rộng để khám phá các yếu tố rủi ro mới. Ví dụ, một red team có thể khám phá các cuộc tấn công “jailbreaking” nhằm vượt qua các ràng buộc an toàn của mô hình (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). Trái ngược với benchmarks, một lợi thế quan trọng của red-teaming là các red team có thể điều chỉnh việc đánh giá cho đúng hệ thống cụ thể đang được kiểm thử. Ví dụ, red team có thể thiết kế các đầu vào tùy chỉnh để nhận diện các hành vi theo kịch bản xấu nhất, cơ hội sử dụng độc hại, và các lỗi bất ngờ. Tuy nhiên, phương pháp này có thể đòi hỏi quyền truy cập đặc biệt tới mô hình và có thể không phát hiện được các nhóm rủi ro quan trọng (‡999, ‡1028).

Quan trọng là việc không xác định được rủi ro không có nghĩa rằng các rủi ro đó ở mức thấp: các công trình trước cho thấy các lỗi thường xuyên né tránh việc phát hiện, đặc biệt khi nhóm red team có quyền truy cập hoặc nguồn lực hạn chế (‡1060). Nghiên cứu cũng đã đặt vấn đề về việc liệu red-teaming có thể tạo ra các kết quả đáng tin cậy và có thể lặp lại hay không (‡1061). Thành phần của red team và các hướng dẫn được cung cấp cho người thực hiện red-team (‡1062), số lượng vòng tấn công (‡1063), và mức độ mô hình được truy cập các công cụ (‡1064, ‡1065) có thể ảnh hưởng đáng kể đến các kết quả, bao gồm cả bề mặt rủi ro được bao phủ. Các hướng dẫn toàn diện về red-teaming nhằm giải quyết một số thách thức này (‡1066).

###@ Giảm thiểu rủi ro

Giảm thiểu rủi ro là quá trình ưu tiên, đánh giá và triển khai các biện pháp kiểm soát và biện pháp đối phó để giảm các rủi ro đã nhận diện. Ví dụ gồm các biện pháp kiểm soát truy cập (‡991), giám sát liên tục (‡986) và các cam kết if-then (‡700). Việc giảm thiểu rủi ro đặt ra một câu hỏi quan trọng: mức độ rủi ro nào là chấp nhận được? Các khuôn khổ gần đây và chính sách của công ty đã bắt đầu chính thức hóa các tiêu chí “chấp nhận rủi ro” (‡965, ‡1040). Tuy nhiên, việc thiết lập các ngưỡng phù hợp vẫn còn thách thức, đặc biệt đối với những rủi ro có tác động rộng đến xã hội (‡986, ‡1067). Hiện chưa có cơ chế được thiết lập nào để xác thực các quyết định chấp nhận rủi ro mà các nhà phát triển đưa ra trước khi phát hành (‡1005).

Các biện pháp giảm thiểu rủi ro được mô tả trong Bàn 3.3 dưới đây có thể thích ứng và có khả năng giảm thiểu nhiều loại rủi ro, bao gồm cả một số rủi ro bất ngờ. Bàn này không bao gồm các biện pháp giảm thiểu kỹ thuật như huấn luyện đối kháng, bộ lọc nội dung và giám sát chuỗi suy nghĩ. Các nội dung này được trình bày trong §3.3. Các biện pháp bảo vệ kỹ thuật và giám sát, cũng như xuyên suốt Báo cáo trong các đoạn “Giảm thiểu” cho từng rủi ro trong §2. Rủi ro.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chính sách sử dụng chấp nhận được
  Chính sách sử dụng chấp nhận được là một tập hợp các quy tắc và hướng dẫn cho việc sử dụng có trách nhiệm, mang tính đạo đức và tuân thủ pháp luật đối với các mô hình AI. Việc này thường thấy ở các nhà phát triển AI khi công bố các chính sách sử dụng chấp nhận được, cũng như các chính sách sử dụng bị cấm, cùng với các bản phát hành mô hình mới (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kiểm soát truy cập/đánh giá người dùng
  Các biện pháp kiểm soát truy cập bao gồm việc sử dụng các chính sách và quy tắc để hạn chế truy cập vào các mô hình AI, dữ liệu và hệ thống dựa trên vai trò người dùng, thuộc tính và các điều kiện khác nhằm ngăn chặn việc sử dụng trái phép, thao túng hoặc rò rỉ dữ liệu. Các công ty AI thường vô hiệu hóa các tài khoản được phát hiện là đang tham gia hoạt động tội phạm (‡486) và triển khai thẩm định người dùng cũng như sàng lọc Know-Your-Customer để đảm bảo rằng các mô hình chỉ được sử dụng bởi các bên đáng tin cậy (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đặc tả hành vi/mô hình
  Một đặc tả hành vi AI là một tài liệu xác định cách một mô hình AI nên hành xử trong nhiều tình huống khác nhau. Nó đóng vai trò như một bản thiết kế cho căn chỉnh và an toàn AI, hướng dẫn việc phát triển mô hình, huấn luyện, đánh giá và các đầu ra của mô hình. Một số công ty AI sử dụng các tài liệu đặc tả mô hình và công khai ít nhất một phần của chúng (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát liên tục
  Giám sát liên tục là quá trình diễn ra thường xuyên, tự động để quan sát, phân tích và kiểm soát các hệ thống AI đang được sử dụng, theo dõi hiệu suất của chúng và giới hạn hành vi của chúng nhằm đảm bảo độ tin cậy, hiệu quả và an toàn. Có rất nhiều công cụ phục vụ cho giám sát liên tục (‡1073*) cũng như các kỹ thuật để hỗ trợ
khả sát (AI) khả năng quan sát (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phòng thủ theo chiều sâu
  Phòng thủ theo chiều sâu là ý tưởng rằng có thể triển khai nhiều lớp phòng vệ độc lập và chồng lấn nhau sao cho nếu một lớp thất bại, thì các lớp khác vẫn còn hiệu quả (‡1075, ‡1076). Nhiều Khung An toàn AI cho Biên giới (Frontier) tham chiếu đến ý tưởng này (ví dụ (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát hệ sinh thái
  Đây là quy trình giám sát hệ sinh thái AI rộng hơn, bao gồm theo dõi năng lực tính toán và phần cứng, nguồn gốc của mô hình, nguồn gốc dữ liệu và các mẫu sử dụng. Tài liệu nghiên cứu thảo luận về việc giám sát như vậy liên quan đến các rủi ro từ AI đa năng (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cam kết dạng nếu-thì
  Các cam kết if-then là một tập hợp các giao thức kỹ thuật và tổ chức cùng với các cam kết nhằm quản lý rủi ro khi các mô hình AI ngày càng trở nên mạnh mẽ hơn. Một số nhà phát triển AI sử dụng các loại cam kết này như một phần của các Khung An toàn AI Frontier của họ (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các đường kẻ đỏ hoặc các lệnh cấm
  Các đường màu đỏ là các ranh giới cụ thể được biểu đạt dưới dạng năng lực, mức độ tác động hoặc loại hình sử dụng. Khái niệm này xuất hiện trong các tuyên bố và sáng kiến công khai, cũng như trong các lệnh cấm theo quy định (‡1079, ‡1080, ‡1081). Tài liệu học thuật cũng ghi nhận các hạn chế của các cách tiếp cận dựa trên đường màu đỏ, bao gồm các thách thức liên quan đến việc đạt được sự đồng thuận và khả năng thực thi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược phát hành và triển khai
  Các chiến lược phát hành và triển khai cho AI đa mục đích có thể bao gồm việc sử dụng phát hành theo giai đoạn hoặc truy cập API để có thêm các phương án giảm thiểu trong trường hợp bị lạm dụng hoặc gây hại ngoài dự kiến (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.3: Giảm thiểu rủi ro trong quản lý rủi ro của AI mục đích chung
>white|black||9|11|br Các phương pháp ví dụ để giảm thiểu rủi ro AI được liệt kê theo thứ tự chữ cái. Các phương pháp được đưa vào nhằm hỗ trợ giảm thiểu rủi ro cho nhiều loại rủi ro khác nhau một cách đồng thời, bao gồm rủi ro từ việc sử dụng với mục đích độc hại, rủi ro từ trục trặc và rủi ro mang tính hệ thống. Do tính còn sơ khai của việc quản lý rủi ro AI đa mục đích nói chung, không phải tất cả các phương pháp đều phù hợp với mọi nhà phát triển hoặc đơn vị triển khai AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Nhân vật vật 3.5: Sơ đồ “pho mát Thụy Sĩ” minh họa phương pháp phòng thủ theo chiều sâu
>white|black||9|11|br Nhiều lớp phòng vệ có thể bù đắp các khiếm khuyết trong từng lớp riêng lẻ. Các kỹ thuật quản lý rủi ro hiện tại cho AI có những điểm yếu, nhưng việc xếp chồng (layering) chúng có thể mang lại sự bảo vệ mạnh mẽ hơn nhiều trước các rủi ro. Nguồn: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Chiến lược phòng thủ theo chiều sâu và chiến lược phát hành là các công cụ giảm thiểu quan trọng

Một mô hình “defence-in-depth” có thể hỗ trợ quản lý rủi ro AI đa mục đích. Trong bối cảnh này, “defence-in-depth” đề cập đến sự kết hợp giữa các biện pháp kỹ thuật, tổ chức và xã hội được áp dụng qua các giai đoạn khác nhau của quá trình phát triển và triển khai (Figure 3.5). Điều này có nghĩa là tạo ra nhiều lớp các biện pháp bảo vệ độc lập, sao cho nếu một lớp thất bại thì các lớp khác vẫn có thể ngăn chặn gây hại. Một ví dụ thường được viện dẫn về mô hình defence-in-depth là phạm vi các biện pháp phòng ngừa được triển khai để ngăn ngừa bệnh truyền nhiễm. Vắc-xin, khẩu trang và rửa tay, cùng với các biện pháp khác, có thể giảm đáng kể nguy cơ lây nhiễm khi kết hợp với nhau, dù không có một phương pháp nào trong số đó đạt hiệu quả 100% khi đứng một mình (‡1083*).

Đối với AI đa mục đích, defence-in-depth sẽ bao gồm các biện pháp kiểm soát không nằm ngay trên bản thân mô hình AI, mà nằm trong hệ sinh thái rộng hơn. Điều này bao gồm (ví dụ) các kiểm soát đối với các vật liệu cần thiết để thực hiện một cuộc tấn công sinh học như các thuốc thử (‡1084, ‡1085). Tuy nhiên, các biện pháp defence-in-depth chủ yếu giải quyết các rủi ro liên quan đến tai nạn, trục trặc và sử dụng với mục đích độc hại, và có thể đóng vai trò ít hơn trong việc quản lý các rủi ro mang tính hệ thống (see §3.5. Building societal resilience).

Chiến lược phát hành và triển khai của một công ty là một thành phần quan trọng trong việc giảm thiểu rủi ro. Các quyết định về cách các mô hình được cung cấp cho người dùng có thể ảnh hưởng đáng kể đến mức độ phơi nhiễm rủi ro (‡1082). Các lựa chọn khác nhau về phát hành và triển khai bao gồm phát hành theo giai đoạn cho các nhóm người dùng giới hạn, cung cấp thông qua các dịch vụ trực tuyến được kiểm soát (chẳng hạn như các API), và việc sử dụng các thỏa thuận cấp phép cùng với các chính sách sử dụng chấp nhận được nhằm hợp pháp ngăn cấm một số ứng dụng gây hại (‡176, ‡1086, ‡1087). §3.4. Các mô hình trọng số mở (open-weight models) thảo luận chi tiết hơn về cách việc phát hành trọng số mô hình ảnh hưởng đến rủi ro.

###@ Quản trị rủi ro

Quản trị rủi ro là quá trình mà qua đó các đánh giá, quyết định và hành động của quản lý rủi ro được gắn kết với chiến lược và các mục tiêu của một tổ chức hoặc một thực thể khác (‡1088, ‡1089). Bảng 3.4 cung cấp một cái nhìn tổng quan về các kỹ thuật quản trị rủi ro phổ biến. Như thể hiện trong Nhân vật 3.4, quản trị rủi ro có thể được hiểu như cốt lõi của quản lý rủi ro vì nó tạo điều kiện cho các bộ phận khác của quản lý rủi ro vận hành hiệu quả. Nó cung cấp trách nhiệm giải trình, tính minh bạch và sự rõ ràng nhằm hỗ trợ các quyết định quản lý rủi ro dựa trên thông tin. Quản trị rủi ro có thể bao gồm các thực hành như báo cáo sự cố (‡1090), phân bổ trách nhiệm về rủi ro (‡965) và bảo vệ người tố giác (‡1091). Một cách rộng hơn, quản trị rủi ro có thể bao gồm các hướng dẫn, khuôn khổ, luật pháp, quy định, các tiêu chuẩn quốc gia và quốc tế, cũng như các sáng kiến đào tạo và giáo dục. Mục đích trọng yếu của quản trị rủi ro là thiết lập các chính sách và cơ chế của tổ chức nhằm làm rõ cách phân bổ các trách nhiệm quản lý rủi ro trong toàn tổ chức hoặc một thực thể khác, để hỗ trợ việc giám sát phù hợp và trách nhiệm giải trình (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tài liệu
  Các thực tiễn tài liệu hóa giúp theo dõi thông tin quan trọng về các hệ thống AI, chẳng hạn như dữ liệu huấn luyện, các lựa chọn thiết kế, mục đích sử dụng dự kiến, các hạn chế và rủi ro. ‘Phiếu mô hình’ và ‘phiếu hệ thống’, cung cấp thông tin về việc một mô hình AI hoặc một hệ thống AI đã được huấn luyện và đánh giá như thế nào, là các ví dụ về các thực hành tài liệu hóa AI nổi bật (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Báo cáo sự cố
  Báo cáo sự cố là quá trình ghi nhận một cách có hệ thống và chia sẻ các trường hợp mà việc phát triển hoặc triển khai AI đã gây ra tác hại trực tiếp hoặc gián tiếp. Có một số nền tảng hỗ trợ báo cáo sự cố cho AI (‡1096, ‡1097) và các khung (framework) để hỗ trợ báo cáo sự cố AI hiệu quả hơn (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Khung quản lý rủi ro
  Các khung quản lý rủi ro là các kế hoạch ở cấp tổ chức nhằm giảm các khoảng trống trong phạm vi quản lý rủi ro, phối hợp các hoạt động quản lý rủi ro khác nhau và triển khai các cơ chế kiểm tra - giám sát. Các khung dành riêng cho AI mục đích chung (‡986, ‡1098) thường tham chiếu đến các biện pháp khác được nêu trong phần này.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sổ đăng ký rủi ro
  Sổ đăng ký rủi ro là một kho lưu trữ các rủi ro khác nhau, mức độ ưu tiên của chúng, người chịu trách nhiệm và kế hoạch giảm thiểu. Các nội dung này khá phổ biến trong nhiều ngành, bao gồm an ninh mạng (‡1099), và đôi khi được sử dụng để đáp ứng các yêu cầu tuân thủ quy định.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phân bổ trách nhiệm rủi ro
  Việc phân bổ vai trò và trách nhiệm cho quản lý rủi ro trong một tổ chức có thể cấu trúc việc giám sát nội bộ đối với hoạt động ra quyết định (‡1002, ‡1093). Những sắp xếp như vậy được phản ánh trong một số khung quản trị, bao gồm Bộ quy tắc thực hành về AI đa mục đích của EU (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Báo cáo minh bạch
  Báo cáo minh bạch mô tả các thực tiễn quản lý rủi ro của một công ty AI bằng cách công khai tiết lộ một số thông tin hoặc chia sẻ tài liệu với các nhóm trong ngành hoặc cơ quan chính phủ. Ví dụ, nhiều công ty AI nộp các báo cáo minh bạch Quy trình AI Hiroshima (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bảo vệ người tố giác
  Vì phần lớn việc phát triển AI diễn ra trong khuất cửa, một số khung quản trị bao gồm các biện pháp bảo vệ người tố giác để cho phép việc công bố các rủi ro tiềm ẩn với các cơ quan có thẩm quyền (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.4: Quản trị rủi ro trong quản lý rủi ro AI đa mục đích
>white|black||9|11|br Các phương pháp mẫu để quản trị rủi ro AI được liệt kê theo thứ tự alphabet. Các phương pháp được bao gồm nhằm hỗ trợ quản trị rủi ro cho đồng thời nhiều loại rủi ro khác nhau, bao gồm rủi ro từ việc sử dụng với mục đích độc hại, rủi ro từ sự cố/malfunction, và rủi ro mang tính hệ thống. Do tính còn non trẻ của quản lý rủi ro AI đa mục đích, không phải tất cả các phương pháp đều phù hợp cho mọi nhà phát triển hoặc đơn vị triển khai AI.


>white|orangered|left|14|15.5|bb Tài liệu hóa và tính minh bạch là các thành phần của quản trị rủi ro

Các cơ chế minh bạch trong tài liệu và thể chế, cùng với các thông lệ chia sẻ thông tin, tạo điều kiện cho việc giám sát từ bên ngoài và hỗ trợ các nỗ lực nhằm quản lý các rủi ro liên quan đến trí tuệ nhân tạo đa năng (‡1101, ‡1102). Hiện nay, việc công bố kết quả các bài kiểm tra trước khi triển khai theo một “model card” hoặc “system card”, kèm theo các thông tin cơ bản về mô hình hoặc hệ thống, bao gồm cách thức nó đã được huấn luyện và các hạn chế tiềm ẩn của nó, đã trở thành thông lệ phổ biến (‡1094, ‡1095). Một số nhà phát triển cũng công bố các báo cáo minh bạch, trong đó có các chi tiết về thực tiễn quản lý rủi ro của họ ở phạm vi rộng hơn (‡1103). Các yếu tố khác của tài liệu và minh bạch bao gồm giám sát và báo cáo sự cố (‡176, ‡1083*, ‡1103) và chia sẻ thông tin, có thể được hỗ trợ bởi các bên thứ ba như Frontier Model Forum. Một số khuôn khổ quy định, chẳng hạn như Đạo luật AI của EU hoặc “California’s Transparency in Frontier Artificial Intelligence Act - Senate Bill No. 53 (SB 53)” (‡1081, ‡1104), trong một số trường hợp yêu cầu chia sẻ thông tin về các rủi ro của trí tuệ nhân tạo đa năng.

>white|orangered|left|14|15.5|bb Cam kết lãnh đạo và các biện pháp khuyến khích định hình các thực hành quản lý rủi ro

Văn hoá tổ chức, cơ cấu lãnh đạo và các cơ chế khuyến khích ảnh hưởng đến các nỗ lực quản lý rủi ro theo nhiều cách khác nhau (‡1105). Sự cam kết của lãnh đạo và các cấu trúc khuyến khích thường liên quan đến cách các chính sách quản lý rủi ro vận hành trong thực tiễn. Một số nhà phát triển có các hội đồng ra quyết định nội bộ để cân nhắc cách thiết kế, phát triển và rà soát các hệ thống AI mới một cách an toàn và có trách nhiệm. Các cơ chế giám sát và uỷ ban tư vấn, quỹ tín thác (trusts), hoặc các hội đồng đạo đức AI cũng có thể đóng vai trò như các cơ chế để cung cấp hướng dẫn quản lý rủi ro và giám sát của tổ chức (‡1092*, ‡1106, ‡1107, ‡1108). Các nhà nghiên cứu đã lập luận rằng những thách thức của cơ chế tự quản trị tự nguyện cho thấy bên thứ ba thực hiện kiểm toán, thẩm định và tiêu chuẩn hoá có thể giúp củng cố quản lý rủi ro cho AI mục đích chung (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Quản lý rủi ro trong tổ chức, tính minh bạch và các khung báo cáo rủi ro

Một số sáng kiến mới tập trung vào các quy trình quản lý rủi ro, tài liệu hóa và tính minh bạch. Trong hình thức hiện tại, Bộ Quy tắc Thực hành về AI đa mục đích của EU đóng vai trò như một khuôn khổ tự nguyện để hướng dẫn các hoạt động về minh bạch, bản quyền, và an toàn cùng an ninh nhằm hỗ trợ việc tuân thủ các quy định của Đạo luật AI của EU đối với AI đa mục đích (‡965). Tính đến tháng 12/2025, đã có hơn hai chục công ty† tham gia ký kết. Khung báo cáo của Quy trình AI Hiroshima của G7 (HAIP) (‡1100) là khuôn khổ quốc tế đầu tiên cho việc báo cáo công khai tự nguyện các thực hành quản lý rủi ro của các hệ thống AI tiên tiến. Ít nhất 20 nhà phát triển đã công bố các báo cáo minh bạch công khai, bao gồm việc xác định rủi ro, các chỉ số đánh giá, các chiến lược giảm thiểu, và các quy trình bảo mật dữ liệu.

Các nhà phát triển AI đã áp dụng các cam kết minh bạch tự nguyện. Tại Trung Quốc, các cam kết của 17 công ty AI của Trung Quốc, được phối hợp bởi Liên minh Công nghiệp AI của Trung Quốc, đã được công bố vào tháng 12 năm 2024 (‡1113) và được cập nhật vào năm 2025 (‡1114). Tại Hội nghị thượng đỉnh AI Seoul tháng 5 năm 2024 ở Hàn Quốc, 16 nhà phát triển AI từ nhiều quốc gia đã ký các cam kết tự nguyện nhằm công bố các Khung An toàn AI Frontier cho các mô hình và hệ thống có năng lực cao nhất của họ, và áp dụng các thực hành quản lý rủi ro trên toàn bộ các giai đoạn phát triển và triển khai mô hình (‡1052).

    Ghi chú † -- Các bên ký kết tính đến tháng 12/2025 bao gồm: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing, và WRITER.

>white|orangered|left|14|15.5|bb Các Khung An toàn AI Frontier đã trở thành một cách tiếp cận có tổ chức nổi bật để quản lý rủi ro AI

Từ năm 2023, một số nhà phát triển AI tiên phong đã tự nguyện công bố các tài liệu mô tả cách họ dự định nhận diện và ứng phó với các rủi ro nghiêm trọng từ các hệ thống AI tiên tiến nhất của mình. Các Khung An toàn AI Tiên phong này mô tả cách một nhà phát triển AI dự định đánh giá, giám sát, và kiểm soát các mô hình và hệ thống AI tiên tiến nhất của họ trước và trong khi triển khai. Các khung này có nhiều điểm tương đồng, nhưng khác nhau ở một số khía cạnh quan trọng (‡1115, ‡1116). Hầu hết tập trung vào các rủi ro liên quan đến các mối đe dọa hóa học, sinh học, phóng xạ và hạt nhân (CBRN), các năng lực mạng máy tính nâng cao, và hành vi tự chủ nâng cao (‡1115, ‡1117). Một thiểu số các khung đề cập thêm các lĩnh vực rủi ro như phân biệt đối xử trái pháp luật ở quy mô lớn và khai thác tình dục trẻ em.

Một số nhà phát triển đã cập nhật framework của họ vào năm 2025, bổ sung các mục mới về thao tác gây hại, rủi ro không tương hợp (misalignment), và sao chép và thích nghi tự chủ (‡1078, ‡1118). Mặc dù nhiều framework mô tả các cách tiếp cận quản lý rủi ro tương tự – bao gồm mô hình hoá mối đe doạ (threat modelling), red-teaming, và đánh giá các năng lực nguy hiểm – nhưng chúng khác nhau về cách định nghĩa các bậc rủi ro và ngưỡng, tần suất các lần đánh giá, bộ đệm giữa các lần đánh giá và ngưỡng, cũng như mức độ toàn diện trong các cam kết giảm thiểu của chúng (ví dụ: liệu chúng có bao gồm việc xoá trọng số mô hình (model weights) hay chỉ tạm dừng phát triển) (‡1115, ‡1119). Xem Bàn 3.5 để biết thêm thông tin.

>white|orangered|left|14|15.5|bb Nhiều hành động trong các Khung An toàn AI Frontier dựa trên các cam kết dạng nếu-thì

Một phần quan trọng của Frameworks (Khung an toàn) Frontier AI Safety là các cam kết “nếu-thì”. Đây là các giao thức mang tính điều kiện, kích hoạt các phản hồi cụ thể khi các mô hình và hệ thống AI đạt các ngưỡng năng lực được xác định trước (‡1120). Ví dụ, một cam kết nếu-thì có thể nêu rằng nếu phát hiện một mô hình có khả năng hỗ trợ một cách có ý nghĩa cho người mới trong việc tạo ra và triển khai vũ khí CBRN, thì nhà phát triển sẽ thực hiện các biện pháp bảo mật nâng cao, các cơ chế kiểm soát triển khai và giám sát thời gian thực (‡991*).

Vào 2025, một số nhà phát triển AI đã công bố rằng các mô hình mới đã kích hoạt cảnh báo cảnh giới sớm hoặc rằng họ không thể loại trừ khả năng việc đánh giá tiếp theo sẽ cho thấy các mô hình đã vượt ngưỡng năng lực. Điều này khiến họ áp dụng các biện pháp bảo vệ tăng cường như một biện pháp phòng ngừa (‡7, ‡33, ‡1121*). Các Khung An toàn AI của Frontier thường yêu cầu đánh giá năng lực ban đầu trước khi thực hiện giảm thiểu rủi ro, cũng như phân tích rủi ro còn dư hoặc một hồ sơ an toàn, thường được thông tin từ hoạt động red-teaming, sau khi đã giảm thiểu. Xem Bàn 3.5 để biết thông tin chi tiết.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Khung sẵn sàng 2 (‡1078*)
  Các rủi ro được bao phủ:
1. Năng lực sinh học và hóa học
2. Năng lực an ninh mạng
3. Năng lực tự cải thiện của AI
  Các mức rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
- Mức cao: Có thể khuếch đại các lối đi hiện có dẫn đến gây hại nghiêm trọng (Yêu cầu các biện pháp kiểm soát bảo mật và các biện pháp bảo vệ)
- Quan trọng: Có thể mở ra các lối đi hoàn toàn mới dẫn đến mức độ gây hại nghiêm trọng chưa từng có (Tạm dừng phát triển tiếp cho đến khi các tiêu chuẩn về cơ chế bảo vệ và các biện pháp kiểm soát bảo mật được chỉ định đạt mức Chuẩn Quan trọng)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Chính sách mở rộng có trách nhiệm 2.2 (‡991*)
  Các rủi ro được bao phủ:
1. Vũ khí CBRN
2. Nghiên cứu và phát triển AI tự chủ (AI R&D)
3. Các hoạt động mạng (đang được đánh giá)
  Các mức rủi ro hoặc tương đương và các biện pháp bảo đảm liên quan:
  Mức độ An toàn AI (ASL)
- ASL-1: Không có rủi ro thảm khốc đáng kể
- ASL-2: Dấu hiệu sớm về các năng lực nguy hiểm (Các mô hình phải đáp ứng các Tiêu chuẩn Triển khai và Bảo mật ASL-2)
- ASL-3: Rủi ro lạm dụng thảm khốc tăng đáng kể (Các mô hình phải đáp ứng các Tiêu chuẩn Triển khai và/hoặc Bảo mật của ASL-3)
- ASL-4+: Phân loại trong tương lai (chưa được định nghĩa)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Frontier Safety Framework 3.0 (‡1040*)
  Các rủi ro được bao phủ:
1. Lạm dụng
    a. CBRN
    b. Mạng an ninh mạng
    c. Thao túng có hại
2. Nghiên cứu và Phát triển (R&D) Machine learning
3. Hiện tượng lệch hướng/ suy luận công cụ
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Các Cấp Độ Năng Lực Trọng Yếu
    Các mức năng lực mà, trong trường hợp không có biện pháp giảm thiểu (hồ sơ an toàn cho việc triển khai và các biện pháp giảm thiểu an ninh phù hợp với các mức an ninh của RAND 2, 3 hoặc 4 (‡1122)), các mô hình hoặc hệ thống AI có thể gây ra rủi ro gia tăng đối với khả năng gây hại nghiêm trọng. Các mức năng lực bao gồm các “đánh giá cảnh báo sớm”, với các “ngưỡng cảnh báo” cụ thể.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Khung công cụ AI Frontier 1.1 (‡990*)
  Các rủi ro được bao phủ:
1. An ninh mạng
2. Rủi ro hóa học và sinh học
  Các nhóm rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Ngưỡng Mức Rủi Ro
- Trung bình (phát hành kèm các biện pháp bảo mật và biện pháp giảm thiểu phù hợp)
- igh (không phát hành)
- Phê tính (dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Khung An toàn cho Mô hình Cấp biên (‡1123*)
  Các rủi ro được bao phủ:
1. sự phổ biến vũ khí CBRN
2. Các hoạt động tấn công mạng
3. Nghiên cứu và phát triển AI tự động
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo đảm liên quan:
  Ngưỡng năng lực quan trọng
    Các khả năng của mô hình có tiềm năng gây hại nghiêm trọng cho công chúng nếu bị sử dụng sai mục đích. (Nếu các ngưỡng được đáp ứng hoặc vượt quá, mô hình sẽ không được triển khai công khai nếu chưa có các biện pháp giảm thiểu rủi ro phù hợp)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Khung quản trị Frontier (‡1124*)
  Các rủi ro được bao phủ:
1. Vũ khí CBRN
2. Các hoạt động tấn công mạng
3. Tự chủ nâng cao (bao gồm nghiên cứu và phát triển AI)
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Mức độ rủi ro
- Thấp hoặc Trung bình (Cho phép triển khai theo yêu cầu của Chương trình Trí tuệ Nhân tạo Có trách nhiệm)
- Cao hoặc Nghiêm trọng (Cần xem xét thêm và các biện pháp khắc phục)
(bắt buộc)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Đánh giá rủi ro AI Frontier (‡1029*)
  Các rủi ro được bao phủ:
1. Tội phạm mạng
2. CBRN
3. Thuyết phục và thao túng
4. Phân biệt đối xử trái pháp luật ở quy mô lớn
  Các hạng rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Ngưỡng rủi ro – điểm rủi ro của mô hình (MR)
- MR1 hoặc MR2 (Kết quả đánh giá được ghi nhận bởi các nhóm kỹ thuật)
- MR3 (Các biện pháp giảm thiểu rủi ro và kết quả đánh giá được ghi nhận bởi các nhóm kỹ thuật và được xem xét định kỳ)
- MR4 (Cần hoàn thành đánh giá rủi ro chi tiết và cần có phê duyệt của trưởng đơn vị kinh doanh)
- MR5 (Cần hoàn thành và được phê duyệt bởi một ủy ban độc lập, ví dụ: ủy ban đạo đức AI của NVIDIA, một đánh giá rủi ro chi tiết.)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Khung mô hình AI bảo mật cho biên giới (‡1125*)
  Các rủi ro được bao phủ:
1. Sử dụng với mục đích gây hại (ví dụ: phần mềm độc hại, khai thác tình dục trẻ em)
2. Tác hại trong việc sử dụng thông thường, không mang tính độc hại, ví dụ như các kết quả gây ra kết quả phân biệt đối xử bất hợp pháp hoặc việc tạo mã không an toàn
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Khả năng xảy ra và mức độ gây hại trong ngữ cảnh
- Thấp
- Trung bình
- Cao
- Rất cao
    (Các biện pháp giảm thiểu rủi ro và các kiểm soát an ninh đã được áp dụng cho tất cả hệ thống và quy trình; cần phải điều chỉnh các biện pháp giảm thiểu bổ sung cho hệ thống AI và trường hợp sử dụng mà trong đó một mô hình được triển khai)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Chính sách sẵn sàng cho AGI (‡1127*)
  Các rủi ro được bao phủ:
1. Tội phạm mạng
2. Nghiên cứu và phát triển AI tự động
3. Tự sao chép và thích nghi tự động
4. Hỗ trợ vũ khí sinh học
  Cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Ngưỡng năng lực quan trọng
    Ngưỡng định lượng trên các tiêu chí đánh giá năng lực (Nếu vượt quá, tiến hành đánh giá năng lực nguy hiểm, các biện pháp an ninh thông tin và các biện pháp giảm thiểu triển khai, hoặc dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chính sách sẵn sàng Magic: AGI (‡1127*)
  Các rủi ro được bao phủ:
1. Tội phạm mạng
2. Nghiên cứu và phát triển AI tự động
3. Tự sao chép và thích nghi tự động
4. Hỗ trợ vũ khí sinh học
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Ngưỡng năng lực quan trọng
    Ngưỡng định lượng trên các chỉ số chuẩn năng lực (Nếu bị vượt, tiến hành đánh giá năng lực nguy hiểm, các biện pháp an ninh thông tin và các biện pháp giảm thiểu triển khai, hoặc dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Khung an toàn AI (‡1128*)
  Các rủi ro được bao phủ:
1. Mất kiểm soát
2. Lạm dụng (ví dụ: vũ khí sinh học hóa bằng công nghệ sinh hóa)
  Các mức rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Mức độ rủi ro
- Rủi ro thấp (Triển khai hệ thống AI, nhưng thực hiện giám sát sau đó để quản lý rủi ro)
- Rủi ro được xác định (Hoặc chỉ cấp quyền cho hệ thống AI mở được sử dụng bởi người dùng được ủy quyền để giảm thiểu rủi ro, hoặc trì hoãn việc triển khai cho đến khi thực hiện thêm các biện pháp an toàn, tùy thuộc vào trường hợp sử dụng)
- Rủi ro cao (Không triển khai hệ thống AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Khung an toàn AI Frontier (‡1129*)
  Các rủi ro được bao phủ:
1. Các mối đe dọa sinh học
2. An ninh mạng tấn công
3. Vận hành tự động và thao tác nâng cao
  Các bậc rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Mức độ rủi ro
- Mức 1 (Biện pháp bảo vệ cơ bản cho rủi ro tối thiểu và khả năng phát hành mã nguồn mở)
- Cấp 2 (giám sát theo thời gian thực, lọc prompt, phát hiện bất thường hành vi, kiểm soát truy cập, red-teaming và mô phỏng đối kháng)
- Cấp 3 (Các biện pháp bảo vệ nâng cao bao gồm red-teaming, triển khai theo giai đoạn, kiểm thử đối kháng, mã hóa, kiểm soát truy cập nhiều bên và kiến trúc zero-trust)
- Cấp 4 (Các giao thức an toàn tối đa cho các mô hình có tính rủi ro cao và các biện pháp bảo mật tối đa)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.5: Khung bảo đảm an toàn AI tiên phong
>white|black||9|11|br Bộ khung đầu tiên của Frontier AI Safety Frameworks được phát hành bởi một nhóm con các nhà phát triển AI đã ký Frontier AI Safety Commitments. Các khung này bao quát các rủi ro tương tự (với một số khác biệt nhỏ) và sử dụng các bậc rủi ro cũng như các cách tiếp cận quản lý rủi ro khác nhau.


>white|orangered|left|14|15.5|bb Hiệu quả của các Khung an toàn AI Frontier là không chắc chắn

Các Khung an toàn Frontier AI có thể đóng vai trò là công cụ quản lý rủi ro trong những điều kiện cụ thể và đối với một số nhóm rủi ro nhất định có con đường dẫn tới gây hại một cách thuyết phục (‡1117). Đồng thời, một số phân tích khác thảo luận các câu hỏi liên quan đến tính rõ ràng và phạm vi của chúng (‡111, ‡986) và về độ vững chắc của các ngưỡng năng lực AI và rủi ro (‡1031, ‡1130). Các khung hiện có thường tập trung vào một phần các lĩnh vực rủi ro. Vì vậy, một số rủi ro nổi bật, như giám sát trái pháp luật (‡1131, ‡1132) và hình ảnh thân mật không có sự đồng thuận (‡287), nhận được ít sự nhấn mạnh hơn. Khác với các cách tiếp cận quản lý rủi ro từ các lĩnh vực khác, như hàng không hoặc năng lượng hạt nhân (‡1133*), các Khung an toàn Frontier AI thường không sử dụng các ngưỡng rủi ro định lượng (‡1134) một cách rõ ràng.

Các đánh giá bên ngoài về mức độ tuân thủ của các nhà phát triển đối với các Frontier AI Safety Frameworks (Khung an toàn AI cho Frontier) của họ cho đến nay vẫn còn hạn chế, một phần vì hầu hết các khung đều mới, thông tin công khai có sẵn thưa thớt, và chưa có các cuộc kiểm toán bên ngoài được tiêu chuẩn hoá. Hiệu quả của chúng cũng sẽ được định hình bởi việc các cam kết được triển khai trong thực tiễn tốt đến mức nào – và ở mức độ nào. Tự thân các khung này có thể không đảm bảo quản lý rủi ro hiệu quả, vì tác động thực tế phụ thuộc vào việc chúng được triển khai tốt đến mức nào – và ở mức độ nào. Cho đến nay, chúng chưa hoàn toàn phù hợp với các tiêu chuẩn quản lý rủi ro quốc tế (‡1135). Một nghiên cứu về các cam kết tự nguyện trước đó cho thấy mức độ thực hiện không đồng đều giữa các hạng mục, gợi ý rằng việc tuân thủ các cam kết tự nguyện có khả năng sẽ khác nhau giữa các công ty và các lĩnh vực (‡1109).

Tổng thể, các Khung An toàn AI Frontier đại diện cho hình thức chi tiết nhất của quản lý rủi ro theo cơ chế tự nguyện của tổ chức hiện đang được sử dụng, nhưng khác nhau đáng kể về phạm vi, ngưỡng và mức độ có thể thực thi.

###@ Các sáng kiến về quy định và quản trị

>white|orangered|left|14|15.5|bb Một số khu vực pháp lý đã ban hành các đạo luật với các yêu cầu về minh bạch

Một số cách tiếp cận pháp quy ban đầu đặt ra các yêu cầu pháp lý nhằm tăng cường tiêu chuẩn hoá và tính minh bạch trong quản lý rủi ro. Đạo luật AI của EU, có hiệu lực từ năm 2024, thiết lập các yêu cầu liên quan đến tính minh bạch, bản quyền và an toàn đối với các mô hình AI đa dụng. Năm 2025, Bộ Quy tắc Thực hành AI đa dụng chung của EU được công bố để hỗ trợ việc tuân thủ các nghĩa vụ này bằng cách cung cấp hướng dẫn về tài liệu hoá mô hình và bản quyền, cũng như – đối với các mô hình tiên tiến nhất – các thực hành quản lý rủi ro như đánh giá, đánh giá rủi ro và giảm thiểu, an ninh thông tin và báo cáo các sự cố nghiêm trọng (‡965).

Các ví dụ khác về các yêu cầu quy định mới bao gồm Đạo luật Khung của Hàn Quốc về Phát triển Trí tuệ Nhân tạo và Xây dựng Niềm tin, trong đó đưa ra các yêu cầu đối với các hệ thống AI “tác động cao” trong các lĩnh vực trọng yếu (‡1136), và SB 53 của California, quy định các yêu cầu minh bạch đối với các khung an toàn và báo cáo sự cố (‡1104). Do các yêu cầu này mới được thiết lập gần đây, vẫn còn quá sớm để đánh giá chi tiết chúng sẽ ảnh hưởng như thế nào đến các thực hành quản lý rủi ro hoặc các kết quả rủi ro thực tế.

>white|orangered|left|14|15.5|bb Các sáng kiến quản trị rộng hơn cung cấp hướng dẫn tự nguyện

Một số khuôn khổ quản trị khu vực và liên khu vực hiện nay đã đưa ra các kỳ vọng chung cho việc quản lý rủi ro từ AI đa năng bằng cách cung cấp hướng dẫn không ràng buộc cho các nhà hoạch định chính sách và các tổ chức. “Khung quản trị an toàn AI” của Trung Quốc 2.0, được công bố vào 2025, cung cấp hướng dẫn có cấu trúc về phân loại rủi ro và các biện pháp đối phó trong toàn bộ quy trình phát triển và triển khai AI (‡1137). Các Quốc gia Thành viên ASEAN đã công bố “Hướng dẫn Mở rộng của ASEAN về Quản trị và Đạo đức AI (AI tạo sinh)”, đưa ra hướng dẫn về quản trị và đạo đức đối với AI đa năng, đồng thời nhằm hỗ trợ mức độ liên kết chính sách cao hơn giữa các Quốc gia Thành viên ASEAN (‡1138). Ngoài ra, các sáng kiến do các chuyên gia dẫn dắt như “Singapore Consensus”, được phát triển bởi các nhà khoa học AI từ nhiều quốc gia, đề ra các ưu tiên nghiên cứu về an toàn cho AI đa năng trên các khía cạnh đánh giá, phát triển và kiểm soát rủi ro (‡690).

###@ Cập nhật

Kể từ khi phát hành Báo cáo trước đó (tháng 1 năm 2025), bối cảnh quản lý rủi ro đối với AI đa mục đích đã thay đổi, cùng với việc công bố các tài liệu mới như Bộ Quy tắc Thực hành về AI đa mục đích của EU, Khung Báo cáo HAIP của G7, Khung Quản trị An toàn AI quốc gia của Trung Quốc 2.0 và nhiều Khung An toàn AI cho Đường biên của các nhà phát triển AI khác nhau. Các sáng kiến này mô tả các cách tiếp cận và thực hành mà các nhà phát triển AI sử dụng để quản lý rủi ro gắn với các hệ thống AI đa mục đích (‡1115). Có sự khác biệt đáng kể giữa các Khung An toàn AI cho Đường biên và giữa các báo cáo minh bạch HAIP (‡1103), phản ánh sự khác nhau trong thực tiễn tổ chức, việc ưu tiên rủi ro và giai đoạn ban đầu của hệ sinh thái quản lý rủi ro AI đa mục đích. Một hệ sinh thái đáng tin cậy, nơi các bên liên quan khác nhau trong hệ sinh thái AI đóng góp các thực hành quản lý rủi ro bổ sung trên toàn bộ vòng đời, có thể góp phần vào việc quản lý rủi ro hiệu quả (‡690).

###@ Khoảng trống bằng chứng

Hiện còn thiếu bằng chứng về: cách đo lường mức độ nghiêm trọng, mức độ phổ biến và khung thời gian của các rủi ro mới nổi; mức độ mà các rủi ro này có thể được giảm thiểu trong các bối cảnh thực tế; và cách khuyến khích hoặc thực thi việc áp dụng giảm thiểu một cách hiệu quả giữa các bên liên quan đa dạng. Cần có thêm nghiên cứu để hiểu các rủi ro khác nhau phổ biến đến mức nào và mức độ chúng khác nhau ra sao giữa các khu vực khác nhau trên thế giới, đặc biệt đối với các khu vực như Châu Á, Châu Phi và Mỹ Latinh đang nhanh chóng số hoá. Khi các mô hình AI ngày càng được trao mức độ tự chủ và quyền hạn lớn hơn, và khi tình trạng của khoa học đối với các rủi ro của AI đa mục đích tiếp tục tiến bộ, các cách tiếp cận quản lý rủi ro cũng sẽ cần phải thay đổi theo (‡639, ‡1139).

Một số biện pháp giảm thiểu rủi ro đang ngày càng trở nên phổ biến (‡690, ‡956), nhưng cần thêm nghiên cứu để hiểu trong thực tế các biện pháp giảm thiểu rủi ro và biện pháp bảo vệ có mức độ vững chắc ra sao đối với các cộng đồng và tác nhân AI khác nhau (bao gồm cả các doanh nghiệp vừa và nhỏ). Việc tiếp cận nhiều hơn với dữ liệu về việc triển khai và sử dụng mô hình trong đời thực có liên quan đến các đánh giá như vậy. Hơn nữa, nỗ lực quản lý rủi ro hiện nay khác nhau rất nhiều giữa các công ty AI hàng đầu. Người ta đã cho rằng động lực của các nhà phát triển chưa được điều chỉnh phù hợp tốt với việc đánh giá và quản lý rủi ro một cách toàn diện (‡934). Vẫn còn thiếu bằng chứng về mức độ mà các cam kết tự nguyện khác nhau đang được thực hiện, các công ty gặp phải những trở ngại nào khi tuân thủ đầy đủ các cam kết, và cách họ đang tích hợp Các Khung An toàn AI cho AI Tiên phong vào các thực hành quản lý rủi ro AI rộng hơn.

###@ Thách thức đối với các nhà hoạch định chính sách

Các thách thức trọng yếu bao gồm việc xác định cách ưu tiên các rủi ro đa dạng do AI mục đích chung gây ra, làm rõ tác nhân nào có vị trí phù hợp nhất để giảm thiểu các rủi ro này, và hiểu các động lực cũng như ràng buộc định hình hành động của họ. Bằng chứng cho thấy các nhà hoạch định chính sách hiện có quyền tiếp cận hạn chế đối với thông tin về việc các nhà phát triển và triển khai AI đang thử nghiệm, đánh giá và giám sát các rủi ro mới nổi như thế nào, cũng như về hiệu quả của các biện pháp giảm thiểu khác nhau (‡1140). Các nhà nghiên cứu và nhà hoạch định chính sách đã thảo luận về các nỗ lực minh bạch và cơ chế báo cáo sự cố mang tính hệ thống hơn như những cách có thể giúp cung cấp thông tin cho việc ưu tiên rủi ro, thúc đẩy niềm tin và tạo động lực cho phát triển có trách nhiệm (‡957). Trên thực tế, quản lý rủi ro liên quan đến nhiều tác nhân trên toàn chuỗi giá trị AI – như các nhà cung cấp dữ liệu và dịch vụ đám mây, các nhà phát triển mô hình, và các nền tảng lưu trữ mô hình – mỗi bên có những cơ hội khác nhau để đánh giá và quản lý các rủi ro khác nhau (‡1141). Việc chia sẻ thông tin hạn chế giữa các tác nhân này khiến cho việc xác định rủi ro nào có khả năng xảy ra hoặc có tác động lớn nhất trở nên khó khăn, đặc biệt khi xem xét các hệ quả xã hội ở cấp độ hạ nguồn.

