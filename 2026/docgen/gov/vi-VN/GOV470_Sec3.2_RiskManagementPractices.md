##########
>white|orangered|left|14|30|hr Mục 3.2
### 3.2. Các thực tiễn quản lý rủi ro
>white|orangered|left|24|30|hb Các thực hành quản lý rủi ro

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Quản lý rủi ro AI đa năng bao gồm một loạt các biện pháp được sử dụng để xác định, đánh giá và giảm thiểu rủi ro từ AI đa năng. Các biện pháp này bao gồm kiểm thử và đánh giá ở cấp mô hình (chẳng hạn như “red-teaming”), các quy trình tổ chức định hướng cho các quyết định về phát triển và phát hành, các biện pháp bảo vệ có điều kiện (chẳng hạn như các cam kết “nếu-thì”) và báo cáo sự cố.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Một số nhà phát triển AI đã xây dựng các Khung An toàn AI tiên phong. Các khung này bao gồm thông tin về đánh giá rủi ro và quy định các biện pháp có điều kiện, chẳng hạn như hạn chế quyền truy cập mà các công ty dự định áp dụng cho những mô hình có năng lực cao hơn. Chúng khác nhau về các rủi ro được đề cập, cách xác định các ngưỡng năng lực và những hành động được kích hoạt khi đạt đến các ngưỡng đó.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Bằng chứng về hiệu quả thực tế của các biện pháp quản lý rủi ro AI vẫn còn hạn chế. Việc thiếu báo cáo và giám sát sự cố khiến việc đánh giá mức độ các biện pháp hiện hành giảm thiểu rủi ro hiệu quả đến đâu, cũng như mức độ triển khai nhất quán của các biện pháp này, trở nên khó khăn.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi Báo cáo gần nhất được công bố (tháng 1 năm 2025), hoạt động quản lý rủi ro đã trở nên bài bản hơn nhờ các sáng kiến mới trong ngành và về quản trị. Các công cụ mới như Bộ quy tắc thực hành AI đa dụng của EU, Khuôn khổ quản trị an toàn AI 2.0 của Trung Quốc và Khuôn khổ báo cáo của Tiến trình AI Hiroshima của G7, cùng với các sáng kiến do doanh nghiệp dẫn dắt, cho thấy xu hướng hướng tới những cách tiếp cận được tiêu chuẩn hóa hơn về tính minh bạch, đánh giá và báo cáo sự cố.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Động lực thị trường và tốc độ phát triển AI đặt ra thêm nhiều thách thức. Do áp lực cạnh tranh, các công ty AI có thể phải đánh đổi giữa việc phát hành sản phẩm nhanh hơn và đầu tư vào các nỗ lực giảm thiểu rủi ro. Nhiều tác hại liên quan đến AI cũng bị chuyển gánh nặng sang bên ngoài, trong khi trách nhiệm pháp lý đối với những tác hại này vẫn chưa rõ ràng; các quy trình quản trị có thể chậm thích ứng với những thay đổi trong bối cảnh AI.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Những thách thức chính đối với các nhà hoạch định chính sách bao gồm việc xác định thứ tự ưu tiên giữa nhiều rủi ro đa dạng do AI đa dụng gây ra, và làm rõ những tác nhân nào trong toàn bộ chuỗi giá trị AI có vị thế tốt nhất để giảm thiểu các rủi ro đó. Những thách thức này càng trở nên phức tạp do khả năng quan sát hạn chế về cách thức các rủi ro được xác định, đánh giá và quản lý trên thực tế, cũng như việc chia sẻ thông tin rời rạc giữa các nhà phát triển, bên triển khai và nhà cung cấp cơ sở hạ tầng.
>oldlace|black||11|15|br      


Quản lý rủi ro AI bao gồm một loạt các biện pháp nhằm xác định, đánh giá và giảm khả năng xảy ra cũng như mức độ nghiêm trọng của các rủi ro liên quan đến hệ thống AI. Các biện pháp này có thể được triển khai bởi các nhà phát triển, đơn vị triển khai, đơn vị đánh giá và cơ quan quản lý AI. Ví dụ bao gồm mô hình hóa mối đe dọa, phân tầng rủi ro, thử nghiệm đối kháng (red-teaming), kiểm toán và báo cáo sự cố. Phần này trình bày các biện pháp quản lý rủi ro hiện nay, những diễn biến mới và các hạn chế còn tồn tại.

Kể từ đầu năm 2025, một số sáng kiến quốc tế mới về quản lý rủi ro AI đa dụng đã được hình thành, bao gồm các khuôn khổ về tính minh bạch của tổ chức và báo cáo rủi ro, cũng như các khuôn khổ pháp quy và quản trị.

![figure 3.4](images/fig3.4_categories_GAI_methods.png)

##### Nhân vật vật 3.4: Bốn thành phần của quản lý rủi ro
>white|black||9|11|br Bốn nhóm phương pháp quản lý rủi ro AI đa dụng: nhận diện rủi ro; phân tích và đánh giá rủi ro; giảm thiểu rủi ro; và quản trị rủi ro. Đây là một quy trình lặp đi lặp lại theo chu kỳ. Quản trị rủi ro, được thể hiện ở trung tâm, tạo điều kiện để các thành phần khác phát huy hiệu quả. Nguồn: Báo cáo An toàn AI Quốc tế 2026.


Những thách thức còn tồn tại bao gồm mức độ tiêu chuẩn hóa còn hạn chế, gây khó khăn cho việc tuân thủ và đánh giá, cũng như thiếu bằng chứng về hiệu quả trong thực tế. Hơn nữa, bối cảnh thể chế, văn hóa và chính trị khác nhau trên toàn cầu, điều này hàm ý rằng các cách tiếp cận nhằm xác định và quản lý rủi ro, bao gồm cả các ngưỡng rủi ro có thể chấp nhận, có thể khác nhau giữa các khu vực. Phần thảo luận về các cách tiếp cận quản lý rủi ro trong mục này mang tính mô tả: mục tiêu là cung cấp thông tin cho các chủ thể trong hệ sinh thái AI về những cách tiếp cận quản lý rủi ro hiện nay trên toàn cầu. Khi có sẵn, bằng chứng về hiệu quả và hạn chế của những cách tiếp cận này sẽ được thảo luận, nhưng các khuyến nghị chính sách nằm ngoài phạm vi của tài liệu này.

###@ Các thành phần của quản lý rủi ro

Quản lý rủi ro là một quy trình lặp đi lặp lại, bao gồm các thông lệ và phương pháp trải rộng trong toàn bộ chu trình phát triển và triển khai AI, đồng thời phối hợp với nhau một cách nhất quán (‡969). Quản lý rủi ro đối với AI đa dụng có thể bao gồm vai trò của nhiều bên, chẳng hạn như nhà khoa học dữ liệu, kỹ sư mô hình, kiểm toán viên, chuyên gia lĩnh vực, lãnh đạo cấp cao, người dùng cuối, cộng đồng chịu tác động, nhà cung cấp bên thứ ba, nhà hoạch định chính sách, chính phủ, tổ chức tiêu chuẩn và tổ chức xã hội dân sự (‡970, ‡971, ‡972). Các tiêu chuẩn quản lý rủi ro hàng đầu thường có khả năng tương tác với nhau, nhưng sử dụng thuật ngữ khác nhau để mô tả các thành phần của quản lý rủi ro (‡973, ‡974). Các tiêu chuẩn này thường có bốn thành phần liên kết với nhau (Nhân vật 3.4): xác định; phân tích và đánh giá; giảm thiểu; và quản trị rủi ro (‡970, ‡973, ‡975, ‡976). Các bảng dưới đây đưa ra những ví dụ minh họa về các phương pháp, kỹ thuật và công cụ phù hợp. Các thông lệ vẫn tiếp tục phát triển, vì vậy các bảng này không bao quát mọi trường hợp và mức độ phù hợp sẽ khác nhau tùy theo bối cảnh.

###@ Nhận diện rủi ro

Nhận diện rủi ro là quá trình tìm kiếm, nhận biết và mô tả các rủi ro. Việc nhận diện rủi ro toàn diện thường bao gồm các đánh giá dựa trên năng lực, nhằm kiểm tra xem các mô hình có sở hữu những năng lực nguy hiểm cụ thể hay không (‡977), cũng như mô hình hóa rủi ro (‡978) và dự báo (‡715*), được sử dụng để khảo sát các rủi ro hiện hữu và mới xuất hiện. Bàn 3.1 đưa ra nhiều ví dụ về các phương thức nhận diện rủi ro. Việc nhận diện rủi ro cũng dựa vào sự tham gia của các chuyên gia và cộng đồng liên quan để hiểu bối cảnh rộng hơn về cách các rủi ro xuất hiện (‡979, ‡980). Các cơ chế như chương trình săn lỗi có thể hỗ trợ quá trình này bằng cách tạo động lực để phát hiện các lỗ hổng chưa từng được biết đến (‡981) (Bàn 3.1). Một mục tiêu then chốt của việc nhận diện rủi ro là tính đến cả những rủi ro đã được biết đến và hiểu rõ lẫn những rủi ro tiềm ẩn trong tương lai vẫn còn chưa chắc chắn hoặc chưa được mô tả đầy đủ (‡982). Điều này đặc biệt quan trọng đối với AI đa dụng, khi nhiều rủi ro có thể chưa được hiểu đầy đủ hoặc chưa thể quan sát được (‡875).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các chương trình thưởng tìm lỗi bảo mật
  Các chương trình săn lỗi có thưởng hoặc công bố lỗ hổng khuyến khích mọi người tìm kiếm và báo cáo các lỗ hổng trong hệ thống AI. Một số nhà phát triển đã triển khai các chương trình săn lỗi có thưởng (‡983, ‡984).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tham vấn chuyên gia
  Các chuyên gia trong lĩnh vực, người dùng và cộng đồng chịu tác động cung cấp thông tin chuyên sâu về các rủi ro có thể xảy ra. Các hướng dẫn về AI có sự tham gia và bao trùm đang dần hình thành (‡985).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sơ đồ xương cá (Ishikawa)
  Sơ đồ xương cá là công cụ phân tích nguyên nhân gốc rễ đã được sử dụng rộng rãi, và các nhà nghiên cứu đã đề xuất sử dụng chúng để phân tích có cấu trúc các sự cố rủi ro AI (‡986).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dự báo
  Dự báo là quá trình dự đoán các sự kiện hoặc xu hướng trong tương lai dựa trên việc phân tích dữ liệu trong quá khứ và hiện tại. Phương pháp này đã được sử dụng để so sánh xác suất tương đối của, chẳng hạn, các kết quả kinh tế khác nhau do AI tiên tiến gây ra (‡715*, ‡987).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hệ thống phân loại rủi ro
  Các hệ phân loại rủi ro là cách phân loại và sắp xếp rủi ro theo nhiều chiều. Có một số hệ thống phác thảo các rủi ro từ AI đa dụng (‡906, ‡988).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hoạch định kịch bản
  Lập kế hoạch kịch bản bao gồm việc xây dựng các kịch bản tương lai khả dĩ và phân tích cách thức các rủi ro hiện thực hóa. Phương pháp này đã được sử dụng để tìm hiểu các rủi ro và tác động của các mô hình AI (‡989).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mô hình hóa mối đe dọa
  Mô hình hóa mối đe dọa là một quy trình nhằm xác định các mối đe dọa và lỗ hổng của một hệ thống. Nhiều nhà phát triển AI nhấn mạnh việc sử dụng mô hình hóa mối đe dọa để dự đoán các tình huống có thể xảy ra khi các hệ thống AI bị sử dụng sai mục đích (‡990, ‡991).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.1: Ví dụ về nhận diện rủi ro trong quản lý rủi ro AI đa dụng
>white|black||9|11|br Các phương pháp ví dụ để nhận diện rủi ro AI được liệt kê theo thứ tự bảng chữ cái. Các phương pháp được đưa vào񎟇
được thiết kế để hỗ trợ xác định nhiều loại rủi ro khác nhau, bao gồm rủi ro do việc sử dụng có mục đích xấu, rủi ro do trục trặc và rủi ro mang tính hệ thống. Do hoạt động quản lý rủi ro của AI đa dụng còn non trẻ, không phải phương pháp nào cũng phù hợp với mọi nhà phát triển hoặc đơn vị triển khai AI.


>white|orangered|left|14|15.5|bb Mô hình hóa mối đe dọa và phân loại rủi ro là những phương pháp nhận diện rủi ro nổi bật.

Hai phương pháp nổi bật để xác định các rủi ro từ AI đa dụng là mô hình hóa mối đe dọa International AI Safety Report 2026 (một quy trình có cấu trúc nhằm lập bản đồ cách các rủi ro liên quan đến AI có thể hiện thực hóa) và các hệ thống phân loại rủi ro. Chẳng hạn, Meta sử dụng các bài tập mô hình hóa mối đe dọa để dự đoán các kịch bản lạm dụng tiềm ẩn đối với các mô hình AI của mình (‡990), còn Anthropic đưa mô hình hóa mối đe dọa vào Tiêu chuẩn Triển khai ASL-3 của mình (‡991). Các hệ thống phân loại rủi ro và mối nguy của AI, trong đó liệt kê các nhóm rủi ro và ví dụ, cũng có thể làm điểm khởi đầu để khái niệm hóa, xác định và mô tả cụ thể những rủi ro đáng chú ý gắn với AI đa dụng trong các lĩnh vực ứng dụng cụ thể (‡906, ‡988, ‡992, ‡993).

###@ Phân tích và đánh giá rủi ro

Phân tích và đánh giá rủi ro là quá trình xác định mức độ rủi ro của một mô hình hoặc hệ thống AI và so sánh mức độ đó với các tiêu chí đã thiết lập để đánh giá tính chấp nhận được hoặc nhu cầu giảm thiểu rủi ro (‡994, ‡995, ‡996, ‡997). Quá trình này bao gồm các hoạt động như đo lường hiệu năng mô hình trên các bộ tiêu chuẩn (‡998) và các cuộc đánh giá (‡176, ‡715), tiến hành các bài tập kiểm thử đối kháng (‡999*), đánh giá tác động (‡1000) và kiểm toán (‡1001, ‡1002). Xem Bàn 3.2 để biết các ví dụ về phân tích và đánh giá rủi ro AI đa dụng. Các phương pháp này được thiết kế để hỗ trợ phân tích và đánh giá đồng thời nhiều loại rủi ro khác nhau.

Các mục tiêu chính của hoạt động phân tích và đánh giá rủi ro là tiến hành đánh giá năng lực và lỗ hổng của mô hình (‡1003), vận dụng mô hình hóa rủi ro vững chắc để hỗ trợ việc ra quyết định về các ngưỡng rủi ro (‡1004, ‡1005), và tìm hiểu cách các hệ thống AI được sử dụng trong thực tế nhằm đánh giá các tác động xã hội về sau (‡869, ‡904, ‡905, ‡1006). Các quy trình phân tích và đánh giá rủi ro thường được cho là có khả năng xác định rủi ro cao hơn khi có sự rà soát độc lập (‡1001, ‡1007), vận dụng chuyên môn liên ngành (‡1008), và bao gồm các quan điểm đa dạng từ nhiều lĩnh vực, ngành chuyên môn, cũng như từ các cộng đồng chịu ảnh hưởng (‡1009, ‡1010).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các cuộc kiểm toán
  Kiểm toán là các hoạt động đánh giá chính thức về hiệu suất và tác động của các mô hình AI và/ hoặc việc một tổ chức tuân thủ các tiêu chuẩn, chính sách và quy trình, được thực hiện nội bộ hoặc bởi một bên bên ngoài. Kiểm toán AI là một lĩnh vực đang phát triển, với nhiều công cụ và phương pháp hiện có để kiểm toán các mô hình AI và phương pháp thực hành của các nhà phát triển mô hình AI (‡1001, ‡1011, ‡1012, ‡1013, ‡1014, ‡1015, ‡1016, ‡1017, ‡1018).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các bộ chuẩn đánh giá
  Các bộ chuẩn đánh giá là những bài kiểm tra hoặc chỉ số được chuẩn hóa, thường mang tính định lượng, được sử dụng để đánh giá và so sánh hiệu suất của các hệ thống AI trên một tập hợp nhiệm vụ cố định được thiết kế để đại diện cho việc sử dụng trong thế giới thực (‡177, ‡1003).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phương pháp Bowtie
  Phương pháp nơ bướm là một phương pháp nổi tiếng để trực quan hóa những vị trí có thể bổ sung các biện pháp kiểm soát nhằm giảm thiểu các sự kiện rủi ro. Phương pháp này phân biệt rõ ràng giữa quản lý rủi ro chủ động và phản ứng (‡1019).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phương pháp Delphi
  Phương pháp Delphi là một kỹ thuật ra quyết định nhóm, sử dụng một loạt bảng câu hỏi để thu thập sự đồng thuận từ một nhóm chuyên gia (‡1020, ‡1021). Phương pháp này đã được sử dụng để hỗ trợ khám phá những tương lai có thể xảy ra với AI tiên tiến (‡1022).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Thử-nghiệm thực địa
  Thử nghiệm thực địa đánh giá hiệu suất và tác động của một hệ thống AI trong môi trường vận hành thực- tế. Một số nghiên cứu nhấn mạnh thử nghiệm thực địa là phương thức bổ trợ cho việc đánh giá mô hình nhằm đánh giá các kết quả và hệ quả trong thế giới thực (‡869, ‡1023*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá tác động
  Các đánh giá tác động đánh giá những tác động tiềm tàng của một công nghệ hoặc dự án. Việc này có thể bao gồm định lượng, tổng hợp và ưu tiên các tác động. Ví dụ, Đạo luật AI của EU yêu cầu các nhà phát triển hệ thống AI rủi ro cao tiến hành Đánh giá tác động đến các quyền cơ bản (‡1024).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá mô hình
  Các hoạt động đánh giá mô hình bao gồm các quy trình và bài kiểm tra nhằm đánh giá và đo lường hiệu suất của một mô hình AI trong một nhiệm vụ cụ thể. Có rất nhiều hoạt động đánh giá AI để đánh giá các năng lực và rủi ro khác nhau, bao gồm cả về an toàn, bảo mật và tác động xã hội (‡1025, ‡1026).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đánh giá rủi ro xác suất
  Đánh giá rủi ro xác suất là một phương pháp luận để đánh giá các rủi ro liên quan đến những hệ thống hoặc quy trình phức tạp, có tính đến yếu tố bất định. Phương pháp này đã được điều chỉnh để áp dụng cho các hệ thống AI tiên tiến (‡1027).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kiểm thử đội đỏ
  Red-teaming là một hoạt động trong đó một nhóm người hoặc các hệ thống tự động giả làm đối thủ và tấn công các hệ thống công nghệ của một tổ chức nhằm xác định các lỗ hổng. Nhiều công ty AI có các quy trình nội bộ để tiến hành red-teaming các hệ thống AI (‡458, ‡1028). Red-teaming cũng có thể được thực hiện bởi các bên bên ngoài công ty. Các nhóm này phải đối mặt với những thách thức như quyền truy cập hạn chế, nhưng cũng có thể phát hiện ra những hiểu biết độc đáo (‡689).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ma trận rủi ro
  Ma trận rủi ro là công cụ trực quan giúp ưu tiên các rủi ro dựa trên khả năng xảy ra và tác động tiềm tàng của chúng (‡1027). Một số nhà phát triển AI đưa các ma trận rủi ro cơ bản vào Khuôn khổ An toàn AI Tiên phong của họ (‡1029*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ngưỡng rủi ro/ cấp độ rủi ro
  Các ngưỡng hoặc cấp độ rủi ro là những giới hạn định lượng hoặc định tính nhằm phân biệt rủi ro có thể chấp nhận được với rủi ro không thể chấp nhận được, đồng thời kích hoạt các hành động quản lý rủi ro cụ thể khi bị vượt quá. Đối với AI đa dụng, các ngưỡng này được xác định dựa trên sự kết hợp của năng lực, tác động, năng lực tính toán, phạm vi tiếp cận và các yếu tố khác (‡946, ‡1005, ‡1030, ‡1031).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Mức độ chấp nhận rủi ro
  Mức độ chấp nhận rủi ro là mức rủi ro mà một tổ chức sẵn sàng chấp nhận. Trong AI, mức độ chấp nhận rủi ro thường được xác định một cách ngầm định thông qua các chính sách và thông lệ của công ty, trong khi một số chế độ quản lý quy định rõ những rủi ro không thể chấp nhận được và gắn với chúng các hệ quả pháp lý (‡1032). Một số công ty mô tả mức độ chấp nhận rủi ro của mình dựa trên rủi ro cận biên của một mô hình mới; tức là mức độ mà mô hình đó làm gia tăng rủi ro trong một tình huống phản thực tế, vượt quá mức rủi ro vốn đã do các mô hình hiện có hoặc các công nghệ khác gây ra (‡1033).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các hồ sơ an toàn
  Một hồ sơ lập luận an toàn là một lập luận có cấu trúc, được hỗ trợ bằng bằng chứng, cho thấy một hệ thống đủ an toàn để vận hành trong một bối cảnh cụ thể. Các tài liệu gần đây (‡1037, ‡1038, ‡1039) đã nghiên cứu hồ sơ lập luận an toàn cho các hệ thống AI tiên phong, và một số Khung An toàn AI tiên phong có đề cập đến chúng (‡1040*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phân tích an toàn hệ thống
  Phân tích an toàn hệ thống làm rõ các mối phụ thuộc giữa các thành phần và hệ thống mà chúng thuộc về, nhằm dự đoán cách các mối nguy ở cấp hệ thống có thể phát sinh từ lỗi thành phần hoặc quy trình, hoặc từ sự tương tác giữa các hệ thống con, yếu tố con người và điều kiện môi trường. Các phương pháp được áp dụng cho hệ thống AI trong tài liệu bao gồm phân tích quy trình lý thuyết hệ thống (STPA) (‡683, ‡1034*, ‡1035, ‡1036).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.2: Phân tích/đánh giá rủi ro trong quản lý rủi ro AI mục đích chung
>white|black||9|11|br Các phương pháp phân tích/đánh giá rủi ro AI, được liệt kê theo thứ tự bảng chữ cái. Do lĩnh vực quản lý rủi ro AI đa dụng còn non trẻ, không phải phương pháp nào cũng phù hợp với mọi nhà phát triển hoặc đơn vị triển khai AI.


>white|orangered|left|14|15.5|bb Các công cụ phân tích rủi ro phổ biến bao gồm các bộ tiêu chuẩn đánh giá và các đánh giá mô hình.

Các bộ benchmark và đánh giá mô hình là những bài kiểm tra được tiêu chuẩn hóa nhằm đánh giá hiệu suất của các hệ thống AI đa dụng trong những nhiệm vụ cụ thể. Các nhà nghiên cứu đã phát triển nhiều bộ benchmark và phương pháp đánh giá đa dạng, bao gồm các bộ câu hỏi trắc nghiệm khó, bài toán kỹ thuật phần mềm và các nhiệm vụ liên quan đến công việc trong môi trường văn phòng mô phỏng (‡188, ‡629, ‡998, ‡1041, ‡1042, ‡1043, ‡1044, ‡1045, ‡1046, ‡1047, ‡1048, ‡1049). Các đánh giá năng lực gây hại (‡715) được sử dụng để xác định liệu một mô hình hoặc hệ thống AI đa dụng có kiến thức hoặc kỹ năng đặc biệt nguy hiểm hay không, chẳng hạn như khả năng hỗ trợ các cuộc tấn công mạng (xem §2.1.3. Tấn công mạng).

Các quyết định có hệ quả lớn của doanh nghiệp và chính phủ về việc phát hành mô hình phần nào dựa vào các đánh giá này (‡1050, ‡1051, ‡1052). Tuy nhiên, các bộ chuẩn đánh giá khác biệt đáng kể về chất lượng và phạm vi (‡998, ‡1003), và có thể khó đánh giá tính hợp lệ của chúng do nhiều thiếu sót trong các phương pháp đánh giá chuẩn (‡902, ‡909, ‡1003, ‡1053*). Ví dụ, các bộ chuẩn đánh giá có thể trở nên ‘bão hòa’ – tức là điểm số của nhiều mô hình tiến sát điểm tối đa – khiến chúng không còn phân biệt rõ rệt giữa các mô hình. Mô hình cũng ngày càng có khả năng nhận diện một số tác vụ là hoạt động đánh giá và thể hiện hành vi khác với khi thực hiện các tác vụ tương tự trong bối cảnh triển khai, do ‘nhận thức tình huống’ (xem §2.2.2. Mất khả năng kiểm soát). Cuối cùng, các bộ chuẩn đánh giá và hoạt động đánh giá có những hạn chế đã được ghi nhận đầy đủ: đáng chú ý là chúng không nắm bắt được các rủi ro liên quan đến việc sử dụng AI đa năng trong các lĩnh vực mới và cho các tác vụ mới, vì điều kiện kiểm thử khác biệt ở nhiều mức độ so với cách sử dụng trong thế giới thực (‡913) (xem §1.2. Năng lực hiện tại và §3.1. Các thách thức về kỹ thuật và thể chế).

>white|orangered|left|14|15.5|bb Kiểm thử đội đỏ cho phép đánh giá rủi ro theo lĩnh vực- cụ thể hơn

Một phương pháp phổ biến khác để đánh giá rủi ro là kiểm thử đối kháng (red-teaming). “Đội đỏ” là một nhóm chuyên gia đánh giá được giao nhiệm vụ tìm kiếm các lỗ hổng, hạn chế hoặc nguy cơ bị sử dụng sai mục đích. Việc kiểm thử đối kháng có thể tập trung vào một lĩnh vực cụ thể và do các chuyên gia trong lĩnh vực đó thực hiện, hoặc có phạm vi mở để tìm hiểu các yếu tố rủi ro mới. Ví dụ: một đội đỏ có thể tìm hiểu các cuộc tấn công “bẻ khóa” nhằm vô hiệu hóa các giới hạn an toàn của mô hình (‡1054, ‡1055, ‡1056, ‡1057, ‡1058, ‡1059). So với các bộ tiêu chuẩn đánh giá, ưu điểm chính của việc kiểm thử đối kháng là các đội đỏ có thể điều chỉnh hoạt động đánh giá cho phù hợp với hệ thống cụ thể đang được kiểm thử. Ví dụ: các đội đỏ có thể thiết kế đầu vào tùy chỉnh để xác định các hành vi trong trường hợp xấu nhất, cơ hội sử dụng với mục đích xấu và các lỗi bất ngờ. Tuy nhiên, phương pháp này có thể đòi hỏi quyền truy cập đặc biệt vào các mô hình và có thể không phát hiện được những nhóm rủi ro quan trọng (‡999, ‡1028).

Điều quan trọng là việc không xác định được rủi ro không có nghĩa là những rủi ro đó ở mức thấp: các nghiên cứu trước đây cho thấy lỗi thường xuyên thoát khỏi quá trình phát hiện, đặc biệt khi các đội đỏ bị hạn chế quyền truy cập hoặc nguồn lực (‡1060). Nghiên cứu cũng đặt câu hỏi liệu hoạt động kiểm thử đội đỏ có thể tạo ra kết quả đáng tin cậy và có thể tái lập hay không (‡1061). Thành phần của đội đỏ và các chỉ dẫn dành cho những người thực hiện kiểm thử đội đỏ (‡1062), số vòng tấn công (‡1063) và quyền truy cập vào các công cụ của mô hình (‡1064, ‡1065) có thể ảnh hưởng đáng kể đến kết quả, bao gồm cả phạm vi rủi ro được bao quát. Các hướng dẫn toàn diện về kiểm thử đội đỏ nhằm giải quyết một số thách thức này (‡1066).

###@ Giảm thiểu rủi ro

Giảm thiểu rủi ro là quá trình ưu tiên, đánh giá và triển khai các biện pháp kiểm soát và đối phó nhằm giảm các rủi ro đã xác định. Ví dụ gồm kiểm soát truy cập (‡991), giám sát liên tục (‡986) và các cam kết nếu-thì (‡700). Việc giảm thiểu rủi ro đặt ra một câu hỏi then chốt: mức độ rủi ro nào là có thể chấp nhận được? Các khuôn khổ gần đây và chính sách của doanh nghiệp đã bắt đầu chính thức hóa các tiêu chí ‘chấp nhận rủi ro’ (‡965, ‡1040). Tuy nhiên, việc thiết lập các ngưỡng phù hợp vẫn còn nhiều thách thức, đặc biệt đối với những rủi ro có tác động sâu rộng đến xã hội (‡986, ‡1067). Hiện chưa có cơ chế được thiết lập nào để xác thực các quyết định chấp nhận rủi ro mà nhà phát triển đưa ra trước khi phát hành (‡1005).

Các phương pháp giảm thiểu rủi ro được mô tả trong Bàn 3.3 dưới đây có thể được điều chỉnh để giảm thiểu nhiều loại rủi ro, bao gồm cả một số rủi ro bất ngờ. Bàn này không bao gồm các phương pháp giảm thiểu kỹ thuật như huấn luyện đối kháng, bộ lọc nội dung và giám sát chuỗi suy nghĩ. Những phương pháp này được đề cập trong §3.3. Biện pháp bảo vệ và giám sát kỹ thuật, cũng như xuyên suốt Báo cáo, trong các đoạn ‘Biện pháp giảm thiểu’ cho từng rủi ro ở §2. Rủi ro.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chính sách sử dụng được chấp nhận
  Chính sách sử dụng được chấp nhận là tập hợp các quy tắc và hướng dẫn nhằm bảo đảm việc sử dụng mô hình AI có trách nhiệm, có đạo đức và hợp pháp. Các nhà phát triển AI thường công bố chính sách sử dụng được chấp nhận, cũng như chính sách sử dụng bị cấm, cùng với các bản phát hành mô hình mới (‡1068, ‡1069).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kiểm soát truy cập/sàng lọc người dùng
  Các biện pháp kiểm soát truy cập bao gồm việc sử dụng các chính sách và quy tắc để hạn chế quyền truy cập vào các mô hình AI, dữ liệu và hệ thống dựa trên vai trò, thuộc tính của người dùng và các điều kiện khác, nhằm ngăn chặn việc sử dụng trái phép, thao túng hoặc rò rỉ dữ liệu. Các công ty AI thường vô hiệu hóa những tài khoản bị phát hiện có hoạt động phạm tội (‡486) và thực hiện sàng lọc người dùng cũng như quy trình Nhận biết khách hàng (Know-Your-Customer) để đảm bảo các mô hình chỉ được sử dụng bởi những đối tượng đáng tin cậy (‡991, ‡1029*, ‡1070).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Đặc tả hành vi/mô hình
  Tài liệu đặc tả hành vi AI là tài liệu xác định cách một mô hình AI nên hành xử trong nhiều tình huống khác nhau. Tài liệu này đóng vai trò như bản thiết kế cho việc căn chỉnh và bảo đảm an toàn cho AI, định hướng quá trình phát triển, huấn luyện, đánh giá mô hình và các đầu ra của mô hình. Một số công ty AI sử dụng tài liệu đặc tả mô hình và công khai ít nhất một phần nội dung của các tài liệu này (‡1071, ‡1072).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát liên tục
  Giám sát liên tục là quy trình tự động diễn ra liên tục nhằm quan sát, phân tích và kiểm soát các hệ thống AI đang được sử dụng, theo dõi hiệu năng và hạn chế hành vi của chúng để đảm bảo độ tin cậy, hiệu quả và an toàn. Có rất nhiều công cụ hỗ trợ giám sát liên tục (‡1073*) cũng như các kỹ thuật hỗ trợ
Khả năng quan sát AI (‡1074).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phòng thủ theo chiều sâu
  Phòng thủ nhiều lớp là ý tưởng rằng có thể triển khai nhiều lớp phòng thủ độc lập và chồng lấp, sao cho nếu một lớp thất bại, các lớp khác vẫn có hiệu quả (‡1075, ‡1076). Nhiều Khung an toàn AI tiên phong đề cập đến ý tưởng này (ví dụ: (‡1077*)).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát hệ sinh thái
  Đây là quá trình giám sát hệ sinh thái AI rộng lớn hơn, bao gồm theo dõi năng lực tính toán và phần cứng, nguồn gốc mô hình, nguồn gốc dữ liệu và các mô hình sử dụng. Các tài liệu nghiên cứu bàn về hoạt động giám sát này trong mối liên hệ với những rủi ro từ AI đa dụng (‡690).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cam kết nếu-thì
  Các cam kết nếu-thì là tập hợp các quy trình và cam kết về mặt kỹ thuật và tổ chức nhằm quản lý rủi ro khi các mô hình AI ngày càng có năng lực hơn. Một số nhà phát triển AI sử dụng các loại cam kết này trong khuôn khổ An toàn AI tiên phong của họ (‡991, ‡1040, ‡1078*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các lằn ranh đỏ hoặc điều cấm
  Các lằn ranh đỏ là những giới hạn cụ thể được xác định theo năng lực, tác động hoặc loại hình sử dụng. Khái niệm này xuất hiện trong các tuyên bố và sáng kiến công khai, cũng như trong các lệnh cấm theo quy định (‡1079, ‡1080, ‡1081). Các tài liệu cũng nêu những hạn chế của cách tiếp cận dựa trên lằn ranh đỏ, bao gồm những thách thức liên quan đến sự đồng thuận và khả năng thực thi.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các chiến lược phát hành và triển khai
  Các chiến lược phát hành và triển khai AI đa dụng có thể bao gồm phát hành theo giai đoạn hoặc cung cấp quyền truy cập API để có thêm các phương án giảm thiểu trong trường hợp xảy ra hành vi lạm dụng hoặc tác hại ngoài dự kiến (‡1050, ‡1051, ‡1082).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.3: Giảm thiểu rủi ro trong quản lý rủi ro AI đa dụng
>white|black||9|11|br Các phương pháp ví dụ nhằm giảm thiểu rủi ro AI được liệt kê theo thứ tự bảng chữ cái. Những phương pháp này được thiết kế để hỗ trợ giảm thiểu đồng thời nhiều loại rủi ro khác nhau, bao gồm rủi ro do việc sử dụng ác ý, rủi ro do trục trặc và rủi ro mang tính hệ thống. Do hoạt động quản lý rủi ro AI đa dụng vẫn còn mới hình thành, không phải phương pháp nào cũng phù hợp với mọi nhà phát triển hoặc bên triển khai AI.


![figure 3.5](images/fig3.5_swiss_cheese_diagram.png)

##### Nhân vật vật 3.5: “Sơ đồ phô mai Thụy Sĩ” minh họa phương pháp phòng thủ nhiều lớp
>white|black||9|11|br Nhiều lớp phòng thủ có thể bù đắp những thiếu sót của từng lớp riêng lẻ. Các kỹ thuật quản lý rủi ro AI hiện nay còn có những thiếu sót, nhưng kết hợp nhiều lớp có thể giúp bảo vệ hiệu quả hơn nhiều trước các rủi ro. Nguồn: Báo cáo An toàn AI Quốc tế 2026.


>white|orangered|left|14|15.5|bb Phòng thủ nhiều lớp và các chiến lược phát hành là những công cụ giảm thiểu rủi ro quan trọng.

Mô hình ‘phòng-thủ-nhiều lớp’ có thể hỗ trợ quản lý rủi ro đối với AI đa- dụng. Trong ngữ cảnh này, ‘phòng-thủ-nhiều lớp’ là sự kết hợp các biện pháp kỹ thuật, tổ chức và xã hội được áp dụng ở các giai đoạn phát triển và triển khai khác nhau (Nhân vật 3.5). Điều này có nghĩa là tạo ra nhiều lớp biện pháp bảo vệ độc lập, để nếu một lớp thất bại, các lớp khác vẫn có thể ngăn ngừa tác hại. Một ví dụ thường được trích dẫn về mô hình phòng thủ nhiều lớp là hàng loạt biện pháp phòng ngừa được triển khai để ngăn chặn các bệnh truyền nhiễm. Vắc-xin, khẩu trang và rửa tay, cùng với các biện pháp khác, có thể kết hợp để giảm đáng kể nguy cơ lây nhiễm, mặc dù không biện pháp nào trong số này tự nó đạt hiệu quả 100% (‡1083*). Đối với AI đa dụng, phòng thủ- theo chiều sâu sẽ bao gồm các biện pháp kiểm soát không nằm trong chính mô hình AI mà thuộc hệ sinh thái rộng hơn. Chẳng hạn, điều này bao gồm các biện pháp kiểm soát đối với vật liệu cần thiết để thực hiện một cuộc tấn công sinh học, chẳng hạn như thuốc thử (‡1084, ‡1085). Tuy nhiên, các biện pháp phòng thủ- theo chiều sâu chủ yếu giải quyết những rủi ro liên quan đến tai nạn, trục trặc và hành vi sử dụng có ác ý, và có thể ít đóng vai trò hơn trong việc quản lý các rủi ro hệ thống (xem §3.5. Xây dựng khả năng chống chịu của xã hội).

Chiến lược phát hành và triển khai của một công ty là một thành phần quan trọng trong việc giảm thiểu rủi ro. Các quyết định về cách cung cấp mô hình cho người dùng có thể ảnh hưởng đáng kể đến mức độ phơi nhiễm rủi ro (‡1082). Các phương án phát hành và triển khai khác nhau bao gồm phát hành theo từng giai đoạn cho các nhóm người dùng hạn chế, cung cấp quyền truy cập thông qua các dịch vụ trực tuyến được kiểm soát (chẳng hạn như API), cũng như sử dụng các thỏa thuận cấp phép và chính sách sử dụng được chấp nhận nhằm cấm một số ứng dụng có hại theo quy định pháp luật (‡176, ‡1086, ‡1087). §3.4. Các mô hình có trọng số mở thảo luận chi tiết hơn về cách việc phát hành trọng số mô hình ảnh hưởng đến rủi ro.

###@ Quản trị rủi ro

Quản trị rủi ro là quá trình kết nối các đánh giá, quyết định và hành động trong quản lý rủi ro với chiến lược và mục tiêu của một tổ chức hoặc thực thể khác (‡1088, ‡1089). Bàn 3.4 tổng quan về các kỹ thuật quản trị rủi ro phổ biến. Như thể hiện trong Nhân vật 3.4, có thể hiểu quản trị rủi ro là cốt lõi của quản lý rủi ro, vì nó tạo điều kiện để các thành phần khác của quản lý rủi ro vận hành hiệu quả. Quản trị rủi ro cung cấp trách nhiệm giải trình, tính minh bạch và sự rõ ràng, qua đó hỗ trợ việc đưa ra các quyết định quản lý rủi ro dựa trên thông tin đầy đủ. Quản trị rủi ro có thể bao gồm các hoạt động như báo cáo sự cố (‡1090), phân bổ trách nhiệm về rủi ro (‡965) và bảo vệ người tố giác (‡1091). Theo nghĩa rộng hơn, quản trị rủi ro có thể bao gồm hướng dẫn, khuôn khổ, luật pháp, quy định, tiêu chuẩn quốc gia và quốc tế, cũng như các sáng kiến đào tạo và giáo dục. Một mục đích then chốt của quản trị rủi ro là thiết lập các chính sách và cơ chế của tổ chức nhằm làm rõ cách phân bổ trách nhiệm quản lý rủi ro trong toàn tổ chức hoặc thực thể khác, để hỗ trợ hoạt động giám sát phù hợp và trách nhiệm giải trình (‡965, ‡1092*, ‡1093).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tài liệu
  Các thực hành lập tài liệu giúp theo dõi thông tin quan trọng về các hệ thống AI, chẳng hạn như dữ liệu huấn luyện, các lựa chọn thiết kế, mục đích sử dụng dự kiến, hạn chế và rủi ro. “Thẻ mô hình” và “thẻ hệ thống”, cung cấp thông tin về cách một mô hình hoặc hệ thống AI được huấn luyện và đánh giá, là những ví dụ nổi bật về thực hành tốt nhất trong lập tài liệu AI (‡1094, ‡1095*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Báo cáo sự cố
  Báo cáo sự cố là quá trình ghi chép và chia sẻ một cách có hệ thống các trường hợp trong đó việc phát triển hoặc triển khai AI đã gây ra tác hại trực tiếp hoặc gián tiếp. Có một số nền tảng hỗ trợ báo cáo sự cố liên quan đến AI (‡1096, ‡1097), cũng như các khuôn khổ giúp việc báo cáo sự cố AI hiệu quả hơn (‡1090).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các khuôn khổ quản lý rủi ro
  Các khuôn khổ quản lý rủi ro là những kế hoạch của tổ chức nhằm giảm thiểu các khoảng trống trong phạm vi bao quát rủi ro, phối hợp các hoạt động quản lý rủi ro khác nhau và triển khai các cơ chế kiểm soát và cân bằng. Các khuôn khổ dành riêng cho AI đa dụng (‡986, ‡1098) thường đề cập đến những biện pháp khác được nêu trong phần này.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Danh mục rủi ro
  Sổ đăng ký rủi ro là nơi tập hợp các rủi ro khác nhau, thứ tự ưu tiên, người phụ trách và kế hoạch giảm thiểu. Loại tài liệu này khá phổ biến trong nhiều ngành, bao gồm cả an ninh mạng (‡1099), và đôi khi được sử dụng để đáp ứng các yêu cầu tuân thủ quy định.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phân bổ trách nhiệm về rủi ro
  Việc phân định vai trò và trách nhiệm trong quản lý rủi ro tại một tổ chức có thể định hình cơ chế giám sát nội bộ đối với quá trình ra quyết định (‡1002, ‡1093). Những cơ chế như vậy được phản ánh trong một số khuôn khổ quản trị, bao gồm Bộ Quy tắc thực hành về AI đa dụng của EU (‡965).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các báo cáo minh bạch
  Các báo cáo minh bạch mô tả các hoạt động quản lý rủi ro của một công ty AI bằng cách công khai một số thông tin nhất định hoặc chia sẻ tài liệu với các nhóm trong ngành hoặc cơ quan chính phủ. Ví dụ, nhiều công ty AI nộp báo cáo minh bạch theo Quy trình Hiroshima về AI (HAIP) (‡1100).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bảo vệ người tố giác
  Do phần lớn hoạt động phát triển AI diễn ra kín, một số khuôn khổ quản trị có các biện pháp bảo vệ người tố giác, nhằm cho phép họ báo cáo những rủi ro tiềm ẩn với cơ quan chức năng (‡1091).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.4: Quản trị rủi ro trong quản lý rủi ro AI đa dụng
>white|black||9|11|br Các phương pháp ví dụ về quản trị rủi ro AI được liệt kê theo thứ tự bảng chữ cái. Các phương pháp này được thiết kế để hỗ trợ quản trị đồng thời nhiều loại rủi ro khác nhau, bao gồm rủi ro từ việc sử dụng độc hại, rủi ro do trục trặc và rủi ro mang tính hệ thống. Do lĩnh vực quản lý rủi ro AI đa dụng còn non trẻ, không phải phương pháp nào cũng phù hợp với mọi nhà phát triển hoặc đơn vị triển khai AI.


>white|orangered|left|14|15.5|bb Việc lập tài liệu và tính minh bạch là những thành phần của quản trị rủi ro.

Các cơ chế lập tài liệu và minh bạch về thể chế, cùng với các hoạt động chia sẻ thông tin, tạo điều kiện cho việc giám sát từ bên ngoài và hỗ trợ các nỗ lực quản lý rủi ro liên quan đến AI đa dụng (‡1101, ‡1102). Việc công bố kết quả thử nghiệm trước khi triển khai trong một “thẻ mô hình” hoặc “thẻ hệ thống”, cùng với những thông tin cơ bản về mô hình hoặc hệ thống, bao gồm cách thức huấn luyện và những hạn chế tiềm tàng, đã trở thành thông lệ phổ biến (‡1094, ‡1095). Một số nhà phát triển cũng công bố các báo cáo minh bạch, trong đó nêu chi tiết hơn về các hoạt động quản lý rủi ro của họ (‡1103). Các yếu tố khác của việc lập tài liệu và minh bạch bao gồm giám sát và báo cáo sự cố (‡176, ‡1083*, ‡1103), cũng như chia sẻ thông tin — hoạt động có thể được các bên thứ ba như Frontier Model Forum hỗ trợ. Một số khuôn khổ pháp lý, chẳng hạn như Đạo luật AI của EU hoặc Đạo luật Minh bạch về Trí tuệ nhân tạo tiên phong của California - Dự luật Thượng viện số 53 (SB 53) (‡1081, ‡1104), trong một số trường hợp bắt buộc chia sẻ thông tin về các rủi ro của AI đa dụng.

>white|orangered|left|14|15.5|bb Cam kết của ban lãnh đạo và các cơ chế khuyến khích định hình thực tiễn quản lý rủi ro.

Văn hóa tổ chức, cơ cấu lãnh đạo và cơ chế khuyến khích ảnh hưởng đến các nỗ lực quản lý rủi ro theo nhiều cách khác nhau (‡1105). Cam kết của lãnh đạo và cơ cấu khuyến khích thường có liên quan đến cách các chính sách quản lý rủi ro được triển khai trên thực tế. Một số nhà phát triển có các hội đồng ra quyết định nội bộ thảo luận về cách thiết kế, phát triển và đánh giá các hệ thống AI mới một cách an toàn và có trách nhiệm. Các ủy ban giám sát và tư vấn, quỹ tín thác hoặc hội đồng đạo đức AI cũng có thể đóng vai trò là cơ chế đưa ra hướng dẫn quản lý rủi ro và giám sát tổ chức (‡1092*, ‡1106, ‡1107, ‡1108). Các nhà nghiên cứu cho rằng những thách thức trong việc tự quản trị trên tinh thần tự nguyện đồng nghĩa với việc kiểm toán, xác minh và tiêu chuẩn hóa bởi bên thứ ba có thể giúp củng cố công tác quản lý rủi ro đối với AI đa dụng (‡1001, ‡1011, ‡1109, ‡1110, ‡1111, ‡1112).

###@ Quản lý rủi ro của tổ chức, tính minh bạch và các khuôn khổ báo cáo rủi ro

Một số sáng kiến mới tập trung vào các quy trình quản lý rủi ro, tài liệu hóa và tính minh bạch. Ở hình thức hiện tại, Bộ Quy tắc Thực hành về AI đa dụng của EU đóng vai trò là khuôn khổ tự nguyện nhằm định hướng các thực hành về tính minh bạch, bản quyền, an toàn và bảo mật để hỗ trợ tuân thủ các quy định của Đạo luật AI EU đối với AI đa dụng (‡965). Tính đến tháng 12 năm 2025, hơn hai chục công ty† đã ký. Khuôn khổ Báo cáo của Quy trình Hiroshima về AI của G7 (HAIP) (‡1100) là khuôn khổ quốc tế đầu tiên về báo cáo công khai tự nguyện các thực hành quản lý rủi ro của tổ chức đối với các hệ thống AI tiên tiến. Ít nhất 20 nhà phát triển đã công bố các báo cáo minh bạch công khai, bao gồm việc xác định rủi ro, các chỉ số đánh giá, chiến lược giảm thiểu và quy trình bảo mật dữ liệu.

Các nhà phát triển AI đã tự nguyện đưa ra những cam kết về tính minh bạch. Tại Trung Quốc, các cam kết của 17 công ty AI Trung Quốc, do Liên minh Công nghiệp AI Trung Quốc điều phối, được công bố vào tháng 12 năm 2024 (‡1113) và cập nhật vào năm 2025 (‡1114). Tại Hội nghị Thượng đỉnh AI Seoul tháng 5 năm 2024 ở Hàn Quốc, 16 nhà phát triển AI từ nhiều quốc gia đã ký các cam kết tự nguyện về việc công bố Khung an toàn AI tiên phong cho những mô hình và hệ thống có năng lực cao nhất của họ, cũng như áp dụng các biện pháp quản lý rủi ro trong các giai đoạn phát triển và triển khai mô hình (‡1052).

    Ghi chú † -- Các bên ký kết tính đến tháng 12 năm 2025 bao gồm: Accexible, AI Alignment Solutions, Aleph Alpha, Almawave, Amazon, Anthropic, Bria AI, Cohere, Cyber Institute, Domyn, Dweve, EUC Inovação Portugal, Fastweb, Google, Humane Technology, IBM, Lawise, LINAGORA, Microsoft, Mistral AI, Open Hippo, OpenAI, Pleias, re-inventa, ServiceNow, Virtuo Turing và WRITER.

>white|orangered|left|14|15.5|bb Các Khuôn khổ An toàn AI Tiên phong đã trở thành một phương pháp tiếp cận nổi bật của các tổ chức trong quản lý rủi ro AI.

Kể từ năm 2023, một số nhà phát triển AI tiên phong đã tự nguyện công bố các tài liệu mô tả cách họ dự định xác định và ứng phó với những rủi ro nghiêm trọng từ các hệ thống tiên tiến nhất của mình. Các Khung An toàn AI tiên phong này mô tả cách một nhà phát triển AI dự định đánh giá, giám sát và kiểm soát các mô hình và hệ thống AI tiên tiến nhất của mình trước và trong quá trình triển khai. Các khung này có nhiều điểm tương đồng, nhưng khác nhau ở một số khía cạnh quan trọng (‡1115, ‡1116). Hầu hết tập trung vào các rủi ro liên quan đến các mối đe dọa hóa học, sinh học, phóng xạ và hạt nhân (CBRN), các năng lực mạng tiên tiến và hành vi tự chủ tiên tiến (‡1115, ‡1117). Một số ít khung đề cập đến các lĩnh vực rủi ro bổ sung, chẳng hạn như phân biệt đối xử trái pháp luật trên quy mô lớn và bóc lột tình dục trẻ em.

Một số nhà phát triển đã cập nhật các khung của họ vào năm 2025, bổ sung các mục mới về thao túng gây hại, rủi ro lệch hướng, và khả năng tự nhân bản và thích ứng (‡1078, ‡1118). Trong khi nhiều khung mô tả các phương pháp quản lý rủi ro tương tự – bao gồm mô hình hóa mối đe dọa, kiểm thử đội đỏ và đánh giá năng lực nguy hiểm – chúng khác nhau về định nghĩa các cấp độ và ngưỡng rủi ro, tần suất đánh giá, khoảng đệm giữa các lần đánh giá và ngưỡng, cũng như mức độ toàn diện của các cam kết giảm thiểu rủi ro (ví dụ: liệu các cam kết có bao gồm việc xóa trọng số mô hình hay chỉ tạm dừng phát triển) (‡1115, ‡1119). Xem Bàn 3.5 để biết thêm thông tin.

>white|orangered|left|14|15.5|bb Nhiều hành động trong các Khuôn khổ An toàn AI Tiên phong dựa trên các cam kết nếu-thì.

Một phần then chốt của các Khung An toàn AI Tiên phong là “cam kết nếu-thì”. Đây là những quy trình có điều kiện, kích hoạt các phản ứng cụ thể khi các mô hình và hệ thống AI đạt đến những ngưỡng năng lực được xác định trước (‡1120). Ví dụ, một cam kết nếu-thì có thể nêu rằng nếu phát hiện một mô hình có khả năng hỗ trợ đáng kể cho những người mới bắt đầu chế tạo và triển khai vũ khí CBRN, thì nhà phát triển sẽ áp dụng các biện pháp bảo mật tăng cường, biện pháp kiểm soát việc triển khai và hoạt động giám sát theo thời gian thực (‡991*).

Vào năm 2025, một số nhà phát triển AI thông báo rằng các mô hình mới đã kích hoạt cảnh báo sớm hoặc họ không thể loại trừ khả năng các đánh giá sâu hơn sẽ cho thấy các mô hình đã vượt qua các ngưỡng năng lực. Điều này khiến họ áp dụng các biện pháp bảo vệ tăng cường như một biện pháp phòng ngừa (‡7, ‡33, ‡1121*). Các Khung An toàn AI tiên phong thường yêu cầu đánh giá năng lực ban đầu trước khi giảm thiểu rủi ro, cũng như phân tích rủi ro còn lại hoặc hồ sơ an toàn, thường có sự hỗ trợ của hoạt động đội đỏ, sau khi giảm thiểu. Xem Bàn 3.5 để biết thông tin chi tiết.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb OpenAI: Khung Chuẩn bị Sẵn sàng 2 (‡1078*)
  Các rủi ro được đề cập:
1. Các năng lực sinh học và hóa học
2. Năng lực an ninh mạng
3. Khả năng tự cải thiện của AI
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ đi kèm:
- Cao: Có thể khuếch đại các con đường hiện có dẫn đến tác hại nghiêm trọng (Yêu cầu các biện pháp kiểm soát an ninh và biện pháp bảo vệ)
- Nghiêm trọng: Có thể tạo ra những con đường mới chưa từng có dẫn đến tổn hại nghiêm trọng (Tạm dừng phát triển thêm cho đến khi các tiêu chuẩn về biện pháp bảo vệ và kiểm soát bảo mật được quy định đạt mức Nghiêm trọng)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Anthropic: Chính sách mở rộng quy mô có trách nhiệm 2.2 (‡991*)
  Các rủi ro được đề cập:
1. vũ khí CBRN
2. Nghiên cứu và phát triển AI tự chủ (AI R&D)
3. Hoạt động không gian mạng (đang được đánh giá)
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các cấp độ an toàn AI (ASL)
- ASL-1: Không có rủi ro thảm khốc đáng kể
- ASL-2: Dấu hiệu ban đầu về các năng lực nguy hiểm (Các mô hình phải đáp ứng Tiêu chuẩn Triển khai và Bảo mật ASL-2)
- ASL-3: Rủi ro lạm dụng gây thảm họa tăng đáng kể (Các mô hình phải đáp ứng Tiêu chuẩn Triển khai và/ hoặc Tiêu chuẩn Bảo mật ASL-3)
- ASL-4+: Các phân loại trong tương lai (chưa được xác định)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Google: Khung An toàn AI Tiên phong 3.0 (‡1040*)
  Các rủi ro được đề cập:
1. Lạm dụng
    a. CBRN
    b. Mạng lướiуаҩ
    c. Thao túng có hại
2. Nghiên cứu và phát triển học máy
3. Lệch mục tiêu/ Suy luận công cụ
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các mức năng lực then chốt
    Các cấp độ năng lực mà tại đó, nếu không có các biện pháp giảm thiểu (hồ sơ an toàn cho việc triển khai và các biện pháp giảm thiểu an ninh phù hợp với cấp độ an ninh RAND 2, 3 hoặc 4 (‡1122)), các mô hình hoặc hệ thống AI có thể gây ra nguy cơ gia tăng về thiệt hại nghiêm trọng. Các cấp độ năng lực bao gồm “đánh giá cảnh báo sớm”, với các “ngưỡng cảnh báo” cụ thể.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Meta: Khung AI tiên phong 1.1 (‡990*)
  Các rủi ro được đề cập:
1. An ninh mạng
2. Rủi ro hóa học và sinh học

  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các mức ngưỡng rủi ro
- Trung bình (phát hành kèm theo các biện pháp bảo mật và biện pháp giảm thiểu phù hợp)
- igh (không phát hành)
- Nghiêm trọng (dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Amazon: Khung an toàn mô hình tiên phong (‡1123*)
  Các rủi ro được đề cập:
1. Sự phổ biến vũ khí CBRN
2. Các hoạt động mạng mang tính tấn công
3. Nghiên cứu và phát triển AI tự động
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Các ngưỡng năng lực then chốt
    Các năng lực của mô hình có khả năng gây tổn hại đáng kể cho công chúng nếu bị sử dụng sai mục đích. (Nếu các ngưỡng được đáp ứng hoặc vượt quá, mô hình sẽ không được triển khai công khai nếu không có các biện pháp giảm thiểu rủi ro phù hợp)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Microsoft: Khung quản trị AI tiên phong (‡1124*)
  Các rủi ro được đề cập:
1. vũ khí CBRN
2. Các hoạt động mạng mang tính tấn công
3. Khả năng tự chủ nâng cao (bao gồm R&D về AI)
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các mức độ rủi ro
- Thấp hoặc Trung bình (Được phép triển khai phù hợp với các yêu cầu của Chương trình AI có trách nhiệm)
- Cao hoặc Nghiêm trọng (Cần xem xét thêm và biện pháp giảm thiểu

bắt buộc)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb NVIDIA: Đánh giá rủi ro AI tiên phong (‡1029*)
  Các rủi ro được đề cập:
1. Tội phạm mạng
2. CBRN
3. Thuyết phục và thao túng
4. Phân biệt đối xử trái pháp luật trên quy mô lớn
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ đi kèm:
  Ngưỡng rủi ro – điểm rủi ro mô hình (MR)
- MR1 hoặc MR2 (Kết quả đánh giá được các nhóm kỹ thuật ghi lại)
- MR3 (Các biện pháp giảm thiểu rủi ro và kết quả đánh giá được các nhóm kỹ thuật ghi lại và rà soát định kỳ)
- MR4 (Cần hoàn thành đánh giá rủi ro chi tiết và phải được lãnh đạo đơn vị kinh doanh phê duyệt)
- MR5 (Một đánh giá rủi ro chi tiết cần được hoàn thành và phê duyệt bởi một hội đồng độc lập, ví dụ như hội đồng đạo đức AI của NVIDIA)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cohere: Khung mô hình AI tiên phong an toàn (‡1125*)
  Các rủi ro được đề cập:
1. Sử dụng với mục đích độc hại (ví dụ: phần mềm độc hại, bóc lột tình dục trẻ em)
2. Tác hại trong quá trình sử dụng thông thường, không có ác ý, ví dụ: đầu ra dẫn đến kết quả phân biệt đối xử bất hợp pháp hoặc tạo mã không an toàn

  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ liên quan:
  Khả năng xảy ra và mức độ nghiêm trọng của tác hại trong bối cảnh
- Thấp
- Trung bình
- Cao
- Rất cao
    (Các biện pháp giảm thiểu rủi ro và kiểm soát bảo mật được áp dụng cho tất cả các hệ thống và quy trình; cần điều chỉnh các biện pháp giảm thiểu bổ sung cho phù hợp với hệ thống AI và trường hợp sử dụng mà mô hình được triển khai)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb xAI: Chính sách về mức độ sẵn sàng cho AGI (‡1127*)
  Các rủi ro được đề cập:
1. Tội phạm mạng
2. Nghiên cứu và phát triển AI tự động
3. Tự sao chép và thích ứng tự chủ
4. Hỗ trợ vũ khí sinh học
  Các cấp độ rủi ro hoặc tương đương và các biện pháp bảo vệ tương ứng:
  Các ngưỡng năng lực then chốt
    Các ngưỡng định lượng đối với các bài đánh giá năng lực (Nếu vượt qua, tiến hành đánh giá năng lực nguy hiểm, áp dụng các biện pháp an ninh thông tin và biện pháp giảm thiểu rủi ro khi triển khai, hoặc dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Magic: Chính sách sẵn sàng AGI (‡1127*)
  Các rủi ro được đề cập:
1. Tội phạm mạng
2. Nghiên cứu và phát triển AI tự động
3. Tự nhân bản và thích ứng tự chủ
4. Hỗ trợ vũ khí sinh học
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các ngưỡng năng lực then chốt
    Các ngưỡng định lượng trên các bài đánh giá năng lực (Nếu vượt ngưỡng, tiến hành đánh giá năng lực nguy hiểm, áp dụng các biện pháp an ninh thông tin và biện pháp giảm thiểu rủi ro khi triển khai, hoặc dừng phát triển)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Naver: Khung an toàn AI (‡1128*)
  Các rủi ro được đề cập:
1. Mất quyền kiểm soát
2. Lạm dụng (ví dụ: vũ khí hóa sinh học

  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các mức độ rủi ro
- Rủi ro thấp (Triển khai các hệ thống AI, nhưng thực hiện giám sát sau đó để quản lý rủi ro)
- Rủi ro đã được xác định (Chỉ mở hệ thống AI cho người dùng được ủy quyền để giảm thiểu rủi ro hoặc hoãn triển khai cho đến khi áp dụng các biện pháp an toàn bổ sung, tùy thuộc vào trường hợp sử dụng)
- Rủi ro cao (Không triển khai các hệ thống AI)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb G42: Khuôn khổ An toàn AI Tiên phong (‡1129*)
  Các rủi ro được đề cập:
1. Các mối đe dọa sinh học
2. An ninh mạng tấn công
3. Vận hành tự chủ và thao tác nâng cao
  Các cấp độ rủi ro hoặc mức tương đương và các biện pháp bảo vệ liên quan:
  Các mức độ rủi ro
- Cấp độ 1 (Các biện pháp bảo vệ cơ bản đối với rủi ro tối thiểu và khả năng phát hành mã nguồn mở)
- Cấp độ 2 (giám sát thời gian thực, lọc prompt, phát hiện bất thường hành vi, kiểm soát truy cập, kiểm thử đối kháng và mô phỏng đối kháng)
- Cấp độ 3 (Các biện pháp bảo vệ nâng cao bao gồm kiểm thử red- teaming, triển khai theo từng giai đoạn, kiểm thử đối kháng, mã hóa, kiểm soát truy cập đa bên và kiến trúc zero-trust)
- Cấp độ 4 (Các quy trình an toàn tối đa cho các mô hình có hệ quả nghiêm trọng và các biện pháp bảo mật tối đa)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.5: Các khuôn khổ an toàn AI tiên phong
>white|black||9|11|br Bộ Khung An toàn AI Tiên phong đầu tiên được một số nhà phát triển AI đã ký Cam kết An toàn AI Tiên phong công bố. Các khung này đề cập đến những rủi ro tương tự nhau (với một vài khác biệt nhỏ) và áp dụng các cấp độ rủi ro cũng như phương pháp quản lý rủi ro khác nhau.


>white|orangered|left|14|15.5|bb Hiệu quả của các khuôn khổ an toàn AI tiên tiến nhất vẫn chưa chắc chắn.

Các Khuôn khổ An toàn AI Tiên phong có thể đóng vai trò là công cụ quản lý rủi ro trong những điều kiện cụ thể và đối với một số loại rủi ro nhất định có lộ trình dẫn đến tác hại đáng tin cậy (‡1117). Đồng thời, một số phân tích bàn về các vấn đề liên quan đến tính rõ ràng và phạm vi của chúng (‡111, ‡986), cũng như tính vững chắc của các ngưỡng về năng lực AI và rủi ro (‡1031, ‡1130). Các khuôn khổ hiện có thường tập trung vào một tập hợp con các lĩnh vực rủi ro. Vì vậy, một số rủi ro nổi bật, chẳng hạn như giám sát trái pháp luật (‡1131, ‡1132) và hình ảnh thân mật không có sự đồng thuận (‡287), ít được chú trọng hơn. Không giống các phương pháp tiếp cận quản lý rủi ro trong những lĩnh vực khác, chẳng hạn như hàng không hoặc điện hạt nhân (‡1133*), các Khuôn khổ An toàn AI Tiên phong thường không sử dụng các ngưỡng rủi ro định lượng rõ ràng (‡1134).

Các đánh giá bên ngoài về mức độ tuân thủ của các nhà phát triển đối với các Khuôn khổ An toàn AI Biên giới của họ cho đến nay vẫn còn hạn chế, một phần vì phần lớn các khuôn khổ này mới được ban hành gần đây, thông tin công khai còn khan hiếm và chưa có hoạt động kiểm toán bên ngoài nào được chuẩn hóa. Hiệu quả của chúng cũng sẽ phụ thuộc vào việc các cam kết được triển khai trong thực tiễn tốt đến đâu và ở mức độ nào. Tự thân, các khuôn khổ này có thể chưa bảo đảm quản lý rủi ro hiệu quả, vì tác động thực tiễn của chúng phụ thuộc vào việc chúng được triển khai tốt đến đâu và ở mức độ nào. Cho đến nay, chúng chưa hoàn toàn phù hợp với các tiêu chuẩn quản lý rủi ro quốc tế (‡1135). Một nghiên cứu về các cam kết tự nguyện trước đây cho thấy mức độ thực hiện các biện pháp không đồng đều, qua đó cho thấy mức độ tuân thủ các cam kết tự nguyện có thể khác nhau giữa các công ty và lĩnh vực (‡1109).

Xét tổng thể, các khuôn khổ an toàn AI tiên phong đại diện cho hình thức quản lý rủi ro tự nguyện ở cấp tổ chức chi tiết nhất hiện đang được áp dụng, nhưng khác biệt đáng kể về phạm vi, ngưỡng và khả năng thực thi.

###@ Các sáng kiến về quản lý và quản trị

>white|orangered|left|14|15.5|bb Một số khu vực pháp lý đã ban hành luật quy định các yêu cầu về tính minh bạch.

Một số cách tiếp cận quản lý ban đầu đưa ra các yêu cầu pháp lý nhằm tăng cường tính tiêu chuẩn hóa và minh bạch trong quản lý rủi ro. Đạo luật AI của EU, có hiệu lực vào năm 2024, đặt ra các yêu cầu liên quan đến tính minh bạch, bản quyền và an toàn đối với các mô hình AI đa năng. Năm 2025, Bộ Quy tắc Thực hành về AI đa năng của EU được công bố nhằm hỗ trợ việc tuân thủ các nghĩa vụ này thông qua hướng dẫn về tài liệu mô hình và bản quyền, cũng như – đối với những mô hình tiên tiến nhất – các biện pháp quản lý rủi ro như đánh giá, đánh giá và giảm thiểu rủi ro, an toàn thông tin và báo cáo sự cố nghiêm trọng (‡965).

Các ví dụ khác về yêu cầu pháp lý mới bao gồm Luật Khung của Hàn Quốc về Phát triển Trí tuệ nhân tạo và Thiết lập Niềm tin, đưa ra các yêu cầu đối với các hệ thống AI “có tác động cao” trong những lĩnh vực trọng yếu (‡1136), và SB 53 của California, đặt ra các yêu cầu về tính minh bạch đối với khuôn khổ an toàn và việc báo cáo sự cố (‡1104). Vì các yêu cầu này mới được thiết lập gần đây, hiện còn quá sớm để đánh giá chi tiết cách chúng sẽ ảnh hưởng đến các hoạt động quản lý rủi ro hoặc kết quả rủi ro thực tế.

>white|orangered|left|14|15.5|bb Các sáng kiến quản trị rộng hơn đưa ra hướng dẫn tự nguyện.

Hiện nay, một số khuôn khổ quản trị khu vực và liên khu vực đã nêu rõ những kỳ vọng chung về quản lý rủi ro từ AI mục đích chung thông qua việc cung cấp hướng dẫn không mang tính ràng buộc cho các nhà hoạch định chính sách và tổ chức. Khuôn khổ Quản trị An toàn AI của Trung Quốc 2.0, được công bố vào năm 2025, đưa ra hướng dẫn có cấu trúc về phân loại rủi ro và các biện pháp đối phó trong suốt quá trình phát triển và triển khai AI (‡1137). Các quốc gia thành viên ASEAN đã công bố ‘Hướng dẫn mở rộng của ASEAN về Quản trị và Đạo đức AI (AI tạo sinh)’, đưa ra hướng dẫn về quản trị và đạo đức AI mục đích chung, đồng thời hướng tới hỗ trợ sự thống nhất chính sách cao hơn giữa các quốc gia thành viên ASEAN (‡1138). Ngoài ra, các sáng kiến do chuyên gia dẫn dắt như Đồng thuận Singapore, do các nhà khoa học AI đến từ nhiều quốc gia xây dựng, đề ra các ưu tiên nghiên cứu về an toàn AI mục đích chung trong các lĩnh vực đánh giá rủi ro, phát triển và kiểm soát (‡690).

###@ Cập nhật

Kể từ khi Báo cáo gần nhất được công bố (tháng 1 năm 2025), bối cảnh quản lý rủi ro đối với AI đa dụng đã phát triển, với việc công bố các tài liệu mới như Bộ Quy tắc Thực hành về AI đa dụng của EU, Khuôn khổ Báo cáo HAIP của G7, Khuôn khổ Quản trị An toàn AI Quốc gia 2.0 của Trung Quốc và các Khung An toàn AI tiên phong của nhiều nhà phát triển AI. Các sáng kiến này mô tả những phương pháp tiếp cận và thực tiễn mà các nhà phát triển AI sử dụng để quản lý các rủi ro liên quan đến hệ thống AI đa dụng (‡1115). Có sự khác biệt đáng kể giữa các Khung An toàn AI tiên phong và giữa các báo cáo minh bạch HAIP (‡1103), phản ánh sự khác biệt trong thực tiễn của tổ chức, mức độ ưu tiên rủi ro và giai đoạn sơ khai của hệ sinh thái quản lý rủi ro AI đa dụng. Một hệ sinh thái đáng tin cậy, trong đó các chủ thể AI khác nhau đóng góp những thực tiễn quản lý rủi ro bổ trợ cho nhau trong suốt vòng đời, có thể góp phần quản lý rủi ro hiệu quả (‡690).

###@ Những khoảng trống về bằng chứng

Hiện còn thiếu bằng chứng về: cách đo lường mức độ nghiêm trọng, mức độ phổ biến và khung thời gian của các rủi ro mới nổi; mức độ có thể giảm thiểu những rủi ro này trong bối cảnh thực tế; và cách khuyến khích hoặc yêu cầu các bên liên quan đa dạng áp dụng biện pháp giảm thiểu một cách hiệu quả. Cần nghiên cứu thêm để hiểu mức độ phổ biến của các rủi ro khác nhau và mức độ khác biệt của chúng giữa các khu vực trên thế giới, đặc biệt là những khu vực như châu Á, châu Phi và Mỹ Latinh đang số hóa nhanh chóng. Khi các mô hình AI ngày càng được trao quyền tự chủ và thẩm quyền lớn hơn, đồng thời tri thức khoa học về các rủi ro của AI đa dụng ngày càng phát triển, các phương pháp quản lý rủi ro cũng cần tiếp tục đổi mới (‡639, ‡1139).

Một số biện pháp giảm thiểu rủi ro đang ngày càng phổ biến (‡690, ‡956), nhưng cần nghiên cứu thêm để hiểu rõ trên thực tế, các biện pháp giảm thiểu rủi ro và biện pháp bảo vệ vững chắc đến mức nào đối với các cộng đồng và tác nhân AI khác nhau (bao gồm cả các doanh nghiệp vừa và nhỏ). Việc tăng cường khả năng tiếp cận dữ liệu về quá trình triển khai và sử dụng mô hình trong đời thực là điều cần thiết cho những đánh giá như vậy. Hơn nữa, các nỗ lực quản lý rủi ro hiện có sự khác biệt rất lớn giữa các công ty AI hàng đầu. Có ý kiến cho rằng các động lực của nhà phát triển chưa phù hợp với việc đánh giá và quản lý rủi ro một cách toàn diện (‡934). Hiện vẫn còn thiếu bằng chứng về mức độ thực hiện các cam kết tự nguyện khác nhau, những trở ngại mà các công ty gặp phải khi thực hiện đầy đủ các cam kết, cũng như cách họ lồng ghép các Khung An toàn AI tiên phong vào các hoạt động quản lý rủi ro AI rộng hơn.

###@ Thách thức đối với các nhà hoạch định chính sách

Các thách thức chính bao gồm xác định cách ưu tiên những rủi ro đa dạng do AI đa- mục đích gây ra, làm rõ những chủ thể nào có vị thế tốt nhất để giảm thiểu các rủi ro đó, cũng như tìm hiểu các động lực và hạn chế định hình hành động của họ. Bằng chứng cho thấy hiện nay các nhà hoạch định chính sách khó tiếp cận thông tin về cách các nhà phát triển và triển khai AI kiểm thử, đánh giá và giám sát những rủi ro mới nổi, cũng như về hiệu quả của các biện pháp giảm thiểu khác nhau (‡1140). Các nhà nghiên cứu và nhà hoạch định chính sách đã thảo luận về các nỗ lực minh bạch và việc báo cáo sự cố có hệ thống hơn như những cách khả thi để cung cấp thông tin cho việc ưu tiên rủi ro, thúc đẩy niềm tin và khuyến khích phát triển có trách nhiệm (‡957). Trên thực tế, quản lý rủi ro liên quan đến nhiều chủ thể trong chuỗi giá trị AI – chẳng hạn như nhà cung cấp dữ liệu và dịch vụ đám mây, nhà phát triển mô hình và nền tảng lưu trữ mô hình – mỗi chủ thể có những cơ hội riêng để đánh giá và quản lý các rủi ro khác nhau (‡1141). Việc chia sẻ thông tin hạn chế giữa các chủ thể này khiến việc xác định những rủi ro nào có khả năng xảy ra cao nhất hoặc gây tác động lớn nhất trở nên khó khăn, đặc biệt khi xét đến các tác động xã hội ở những khâu sau.

