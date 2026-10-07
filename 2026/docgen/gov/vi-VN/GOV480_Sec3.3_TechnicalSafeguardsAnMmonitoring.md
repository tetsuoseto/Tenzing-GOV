##########
>white|orangered|left|14|30|hr Mục 3.3
### 3.3. Biện pháp bảo vệ kỹ thuật và giám sát
>white|orangered|left|24|30|hb Các biện pháp bảo vệ kỹ thuật và giám sát

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Một loạt biện pháp bảo vệ kỹ thuật được áp dụng ở các giai đoạn khác nhau trong quá trình phát triển và sử dụng AI. Những biện pháp này bao gồm các kỹ thuật được áp dụng trong quá trình phát triển mô hình để giúp hệ thống mạnh mẽ hơn và chống chịu tốt hơn trước việc sử dụng sai mục đích (chẳng hạn như tuyển chọn dữ liệu), hoạt động giám sát và kiểm soát trong giai đoạn triển khai- (chẳng hạn như lọc nội dung và giám sát của con người), cũng như các công cụ sau khi triển khai để giám sát hệ sinh thái AI rộng lớn hơn (chẳng hạn như xác minh nguồn gốc và phát hiện nội dung).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Các biện pháp bảo vệ kỹ thuật có những hạn chế và không thể ngăn chặn một cách đáng tin cậy hành vi gây hại trong mọi bối cảnh. Ví dụ, đôi khi người dùng có thể nhận được đầu ra có hại bằng cách diễn đạt lại yêu cầu hoặc chia nhỏ yêu cầu thành các bước nhỏ hơn. Tương tự, các công cụ như kỹ thuật đóng dấu chìm, vốn được thiết kế để nhận diện nội dung do AI tạo ra, thường có thể bị xoá hoặc thay đổi, làm hạn chế độ tin cậy của chúng.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Những hạn chế của từng biện pháp bảo vệ riêng lẻ có nghĩa là có thể cần áp dụng «phòng thủ nhiều lớp» để ngăn chặn một số kết quả gây hại. Ví dụ, một hệ thống có thể kết hợp mô hình được huấn luyện về an toàn với các bộ lọc đầu vào, bộ lọc đầu ra và bộ giám sát nội dung.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi Báo cáo gần nhất được công bố (tháng 1 năm 2025), các nhà nghiên cứu đã đạt được tiến bộ trong việc cải thiện các biện pháp bảo vệ, nhưng vẫn còn những hạn chế căn bản. Ví dụ, tỷ lệ thành công của các cuộc tấn công được thiết kế để vượt qua các biện pháp bảo vệ đã giảm, nhưng vẫn tương đối cao. Ngoài ra, cũng có những hạn chế căn bản về mức độ kỹ lưỡng mà các mô hình có trọng số mở có thể được bảo vệ.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Một thách thức then chốt đối với các nhà hoạch định chính sách là bằng chứng còn hạn chế về mức độ hiệu quả của các biện pháp bảo vệ trong nhiều trường hợp sử dụng thực tế đa dạng của các hệ thống AI đa dụng. Các nhà phát triển AI khác nhau đáng kể về lượng thông tin họ chia sẻ liên quan đến các biện pháp bảo vệ và hoạt động giám sát. Một thách thức khác là những đánh đổi tiềm tàng giữa việc áp dụng các biện pháp bảo vệ mạnh hơn với việc duy trì hiệu năng hoặc tính hữu ích của hệ thống.
>oldlace|black||11|15|br      


Các nhà phát triển AI có thể sử dụng một số biện pháp bảo vệ kỹ thuật hữu ích nhưng chưa hoàn hảo để giảm thiểu và quản lý rủi ro từ các hệ thống AI đa dụng, nhưng những thách thức về độ bền vững vẫn còn. Các nhà phát triển vẫn chưa thể hoàn toàn ngăn các hệ thống AI đa dụng thực hiện ngay cả những hành vi gây hại rõ ràng và đã được biết đến, chẳng hạn như cung cấp cho người dùng hướng dẫn phạm tội. Ví dụ, các nhà nghiên cứu đã chứng minh rằng những biện pháp bảo vệ tiên tiến nhất có thể bị vô hiệu hóa bằng các phương pháp tạo lời nhắc đối kháng (tức là ‘jailbreak’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), bằng cách yêu cầu mô hình chia nhỏ các nhiệm vụ gây hại phức tạp thành từng bước (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), và bằng những thay đổi đơn giản đối với mô hình (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Các nhà nghiên cứu tiếp tục nghiên cứu những biện pháp bảo vệ chống lại sự cố và hành vi lạm dụng (‡690). Các phương pháp này khác biệt đáng kể về mục đích và hiệu quả, và tác động của chúng rốt cuộc phụ thuộc vào bối cảnh xã hội-kỹ thuật và quản trị rộng lớn hơn, trong đó các hệ thống AI được xây dựng và triển khai.

Các biện pháp bảo vệ kỹ thuật có thể được chia thành ba loại chính: các kỹ thuật để phát triển mô hình an toàn hơn; các kỹ thuật được sử dụng trong quá trình triển khai để giám sát và kiểm soát; và các kỹ thuật hỗ trợ giám sát hệ sinh thái sau triển khai. Bàn 3.6 tóm tắt các biện pháp bảo vệ kỹ thuật đã thảo luận, hiệu quả của chúng và những thách thức còn tồn tại.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Phát triển các mô hình an toàn hơn
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Tuyển chọn dữ liệu (‡1167)
  Loại bỏ dữ liệu có hại để ngăn mô hình học các năng lực nguy hiểm. Những phương pháp này có thể hữu ích, bao gồm cả trong việc phát triển các mô hình có trọng số mở không có năng lực gây hại và chống lại quá trình tinh chỉnh có hại (‡55). Tuy nhiên, vẫn có những thách thức liên quan đến lỗi tuyển chọn dữ liệu và khả năng mở rộng (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Học tăng cường từ phản hồi của con người (‡64*)
  Huấn luyện mô hình để căn chỉnh với các mục tiêu được chỉ định, chẳng hạn như trở nên hữu ích và vô hại. Đây là một cách hiệu quả để giúp mô hình học các hành vi có lợi (‡64*). Tuy nhiên, việc tối ưu hóa quá mức để được con người chấp thuận có thể khiến mô hình hành xử theo cách giả dối hoặc xu nịnh (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các kỹ thuật căn chỉnh đa nguyên (‡1170)
  Huấn luyện mô hình để tích hợp nhiều quan điểm khác nhau về cách mô hình nên hành xử. Những kỹ thuật này giúp giảm mức độ mô hình thiên vị các quan điểm cụ thể (‡1170). Tuy nhiên, bất chấp những kỹ thuật này, bất đồng giữa con người là điều không thể tránh khỏi, và việc thiết kế những cách thức được chấp nhận rộng rãi để cân bằng các quan điểm cạnh tranh là rất khó (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Huấn luyện đối kháng (‡677)
  Huấn luyện mô hình để từ chối gây hại (ngay cả trong những bối cảnh xa lạ) và chống lại các cuộc tấn công từ người dùng có ý đồ xấu (ví dụ: “jailbreak”). Đây là một phương pháp hiệu quả giúp mô hình chống lại các nỗ lực lạm dụng (‡1064), nhưng những thách thức về độ bền vững vẫn còn tồn tại (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb ‘Quên’ trong học máy (‡1175, ‡1176)
  Huấn luyện mô hình bằng các thuật toán chuyên biệt nhằm chủ động triệt tiêu các năng lực có hại (ví dụ: kiến thức về các mối nguy sinh học). Những kỹ thuật này cung cấp một phương thức có mục tiêu để loại bỏ các năng lực có hại khỏi mô hình (‡1175, ‡1176), nhưng các thuật toán học quên hiện nay có thể thiếu tính vững chắc và gây ra những ảnh hưởng ngoài ý muốn đến các năng lực khác (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các công cụ về khả năng diễn giải và xác minh an toàn (‡1177)
  Một nhóm đa dạng các phương pháp thiết kế và xác minh nhằm cung cấp sự bảo đảm nghiêm ngặt hơn rằng các mô hình có những thuộc tính cụ thể liên quan đến an toàn. Các phương pháp này giúp người đánh giá đưa ra những khẳng định về độ an toàn với mức độ tin cậy cao hơn (‡1177), nhưng các phương pháp hiện tại dựa trên những giả định và hiếm khi có hiệu năng cạnh tranh trong thực tế (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Giám sát và kiểm soát
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các cơ chế giám sát dựa trên phần cứng (‡1179, ‡1180, ‡1181)
  Xác minh rằng các tiến trình được cấp quyền đang chạy trên phần cứng nhằm nghiên cứu các mối đe dọa bảo mật hoặc việc tuân thủ quy định. Những cơ chế này cung cấp các cách thức độc đáo để giám sát những phép tính nào đang được thực hiện trên phần cứng và do ai thực hiện (‡1181). Tuy nhiên, các cơ chế phần cứng không thể giám sát mọi loại mối đe dọa, và một số kỹ thuật đòi hỏi phần cứng chuyên dụng (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bộ giám sát tương tác người dùng (‡1154, ‡1166)
  Việc giám sát các tương tác của người dùng để phát hiện dấu hiệu sử dụng độc hại có thể giúp nhà phát triển chấm dứt dịch vụ đối với những người dùng có hành vi độc hại (‡1154, ‡1166). Tuy nhiên, việc thực thi có thể vô tình cản trở các nghiên cứu có ích về an toàn (‡689), và một số hình thức sử dụng sai mục đích rất khó phát hiện (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Trình giám sát tương tác người dùng (‡1154, ‡1166)
  Việc theo dõi các tương tác của người dùng để phát hiện dấu hiệu sử dụng với mục đích độc hại có thể giúp nhà phát triển chấm dứt dịch vụ đối với những người dùng này (‡1154, ‡1166). Tuy nhiên, việc thực thi các biện pháp có thể vô tình cản trở nghiên cứu hữu ích về an toàn (‡689), và một số hình thức sử dụng sai mục đích rất khó phát hiện (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bộ lọc nội dung (‡65*, ‡725)
  Việc lọc các đầu vào và đầu ra của mô hình có khả năng gây hại là một cách rất hiệu quả để giảm thiểu tác hại ngoài ý muốn và rủi ro sử dụng sai mục đích (‡725). Tuy nhiên, các bộ lọc đòi hỏi thêm tài nguyên tính toán và dễ bị một số kiểu tấn công (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bộ giám sát quá trình tính toán nội bộ của mô hình (‡744, ‡1183, ‡1184)
  Việc giám sát các dấu hiệu lừa dối hoặc các dạng nhận thức nội tại có hại khác ở mô hình có thể là một cách hiệu quả để phát hiện hành vi lừa dối (‡744, ‡1183, ‡1184). Tuy nhiên, các phương pháp hiện tại thiếu tính mạnh mẽ và độ tin cậy (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các bộ giám sát chuỗi suy nghĩ (‡430, ‡435)
  Theo dõi văn bản chuỗi suy nghĩ của mô hình để phát hiện dấu hiệu hành vi gây hiểu lầm hoặc lập luận có hại khác là một cách hiệu quả để hiểu và nhận diện các lỗi trong cách mô hình lập luận (‡435). Tuy nhiên, chúng có thể không đáng tin cậy (‡752, ‡753, ‡1186), và nếu mô hình được huấn luyện để tạo ra chuỗi suy nghĩ vô hại, chúng có thể học hành vi gây hiểu lầm (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Con người trong vòng lặp (‡1187, ‡1188, ‡1189)
  Việc con người giám sát và ghi đè các quyết định của hệ thống là thiết yếu trong một số ứng dụng trọng yếu về an toàn (‡1187). Tuy nhiên, các kỹ thuật này bị hạn chế bởi thiên kiến tự động hóa và giới hạn về tốc độ ra quyết định của con người (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cách ly trong sandbox (‡1192)
  Ngăn một tác tử AI trực tiếp tác động đến thế giới là một cách hiệu quả để hạn chế thiệt hại mà nó có thể gây ra (‡1192). Tuy nhiên, việc cô lập trong sandbox hạn chế khả năng trực tiếp thực hiện một số tác vụ của hệ thống (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Các công cụ hỗ trợ giám sát hệ sinh thái
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các kỹ thuật nhận dạng mô hình AI (‡1193*, ‡1194)
  Việc giúp dễ nhận diện các mô hình hoặc từng phiên bản riêng lẻ của mô hình trong các trường hợp sử dụng thực tế- giúp ích cho pháp chứng số và nhận thức về hệ sinh thái (‡1195). Tuy nhiên, một số kiểu sửa đổi mô hình có thể vô hiệu hóa các kỹ thuật này (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Suy luận nguồn gốc mô hình AI (‡1197)
  Những kỹ thuật này giúp các nhà nghiên cứu tìm hiểu cách các mô hình được chỉnh sửa trong hệ sinh thái AI, đặc biệt là các mô hình có trọng số mở. Chúng hỗ trợ công tác pháp y số và nâng cao nhận thức về hệ sinh thái (‡1198), nhưng cần có các dự án quy mô lớn để lập bản đồ toàn diện hệ sinh thái mô hình có trọng số mở (‡1198) .
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hình mờ và siêu dữ liệu (‡1199, ‡1200, ‡1201*)
  Những kỹ thuật này giúp phát hiện dễ dàng hơn liệu một đoạn văn bản, hình ảnh, video, v.v. có được AI tạo ra hoặc chỉnh sửa hay không, và bởi hệ thống nào. Chúng giúp nâng cao nhận thức về hệ sinh thái (‡1199, ‡1200, ‡1201*). Tuy nhiên, một số thao tác chỉnh sửa nội dung có thể làm giả hoặc xoá hình mờ và siêu dữ liệu (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phát hiện nội dung do AI tạo ra (‡1203, ‡1204, ‡1205*)
  Nâng cao khả năng phân biệt nội dung do AI tạo ra với nội dung thật giúp ích cho công tác pháp chứng số và nâng cao nhận thức về hệ sinh thái (‡1203, ‡1204). Tuy nhiên, các bộ phân loại có thể không đáng tin cậy (‡1205*) và có hiệu suất khác nhau giữa các phương thức.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.6: Các biện pháp bảo vệ kỹ thuật được thảo luận trong phần này
>white|black||9|11|br Tóm tắt các biện pháp bảo vệ kỹ thuật được thảo luận trong phần này, chia thành các phương pháp phát triển mô hình an toàn hơn, giám sát và kiểm soát trong thời gian triển khai, và các kỹ thuật hỗ trợ giám sát hệ sinh thái.


###@ Phát triển các mô hình an toàn hơn

Tuyến phòng thủ đầu tiên để ngăn chặn các tác hại từ hệ thống AI đa dụng là làm cho mô hình nền tảng an toàn hơn. Tiểu mục này đề cập đến các biện pháp bảo vệ được “tích hợp vào các tham số mô hình” trong quá trình phát triển mô hình (Nhân vật 3.6).

>white|orangered|left|14|15.5|bb Việc tuyển chọn dữ liệu huấn luyện có thể hạn chế sự phát triển của các năng lực tiềm ẩn nguy hiểm.

Các mô hình AI đa dụng hữu ích chính vì chúng phát triển nhiều kiến thức và năng lực sau khi xử lý dữ liệu huấn luyện, nhưng một số loại dữ liệu huấn luyện đóng vai trò lớn hơn hẳn trong việc phát triển các năng lực tiềm ẩn nguy hiểm. Ví dụ, một mô hình AI được huấn luyện bằng các bài báo về virus học có thể hỗ trợ tốt hơn trong các nhiệm vụ sinh học tiềm ẩn nguy cơ gây hại (‡549, ‡1206*) (xem thêm §2.1.4. Rủi ro sinh học và hóa học). Ngoài ra, các mô hình tạo ảnh/video được huấn luyện bằng hình ảnh khỏa thân của con người cũng có thể bị sử dụng sai mục đích để tạo deepfake thân mật không có sự đồng thuận (‡308, ‡319) (xem thêm §2.1.1. Nội dung do AI tạo ra và hoạt động phạm pháp).

Lọc dữ liệu huấn luyện là một biện pháp giảm thiểu hiệu quả đối với một số năng lực không mong muốn (‡319, ‡1167, ‡1207, ‡1208). Tuy nhiên, việc lọc các tập dữ liệu lớn được sử dụng để huấn luyện các mô hình AI đa dụng có thể khó khăn (‡1168) do chi phí cao (‡1209), lỗi lọc (‡1210) và những tác động tiêu cực đến chất lượng tập dữ liệu (‡1211). Những thách thức này càng trầm trọng hơn do tính đa ngôn ngữ của văn bản trên internet (‡1212), các thiên kiến văn hóa trong kiểm duyệt nội dung (‡1211, ‡1213, ‡1214, ‡1215), và thực tế là việc một phần dữ liệu nhất định có “gây hại” hay không phụ thuộc vào các yếu tố ngữ cảnh (‡1216). Dù vậy, việc lọc bỏ tài liệu có khả năng gây hại khỏi dữ liệu huấn luyện cho thấy triển vọng giúp các mô hình an toàn một cách đáng tin cậy hơn, bao gồm cả việc giúp các mô hình có trọng số mở chống chịu tốt hơn trước hành vi can thiệp gây hại (‡55). Mối quan hệ giữa nội dung dữ liệu huấn luyện và các năng lực mới xuất hiện của mô hình vẫn chưa được hiểu đầy đủ (‡1195), và việc lọc dường như hiệu quả hơn trong việc hạn chế các năng lực gây hại khi áp dụng cho những lĩnh vực tri thức rộng (‡55), so với các hành vi hẹp hơn (‡1206, ‡1217). Xem §3.4. Mô hình có trọng số mở để biết thêm thảo luận.

![figure 3.6](images/fig3.6_safeguards.png)

##### Nhân vật vật 3.6: Nơi áp dụng các biện pháp bảo vệ kỹ thuật
>white|black||9|11|br Các biện pháp bảo vệ kỹ thuật có thể được áp dụng ở những giai đoạn khác nhau trong quá trình phát triển mô hình. Việc tuyển chọn dữ liệu định hình những gì mô hình học được trong quá trình tiền huấn luyện và tinh chỉnh. Các phương pháp dựa trên huấn luyện như học tăng cường từ phản hồi của con người và huấn luyện tính vững chắc điều chỉnh hành vi của mô hình. Các phương pháp kiểm thử như tấn công đối kháng giúp xác định những lỗ hổng còn tồn tại. Một số kỹ thuật, chẳng hạn như các thuật toán an toàn theo thiết kế, áp dụng ở nhiều giai đoạn. Nguồn: Báo cáo An toàn AI Quốc tế 2026.


>white|orangered|left|14|15.5|bb Các phương pháp huấn luyện mô hình AI đa năng để trở nên hữu ích và vô hại chủ yếu dựa vào phản hồi của con người.

Rất khó để huấn luyện và đánh giá các mô hình nhằm bảo đảm chúng luôn tuân theo những nguyên tắc cấp cao như hữu ích, vô hại và trung thực. Trên thực tế, các nhà phát triển hướng đến mục tiêu này bằng cách tinh chỉnh các mô hình AI dựa trên các bản minh họa và phản hồi từ con người. Ví dụ, mô hình chính để tinh chỉnh các mô hình AI, được gọi là ‘học tăng cường từ phản hồi của con người’, dựa trên việc huấn luyện mô hình tạo ra các đầu ra được người gán nhãn đánh giá tích cực (‡1218). Tuy nhiên, phản hồi tích cực từ con người là một thước đo thay thế không hoàn hảo cho hành vi có lợi (‡737, ‡878, ‡1219, ‡1220) và bị hạn chế bởi sai sót cũng như thiên kiến của con người (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Điều này dẫn đến một số thách thức: các mô hình được tinh chỉnh bằng học tăng cường từ phản hồi của con người đôi khi chiều theo người dùng, một hành vi được gọi là “xu nịnh” (‡358, ‡740, ‡1226, ‡1227); đưa ra các câu trả lời hữu ích trong một số bối cảnh nhưng có hại trong những bối cảnh khác (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); đưa ra các câu trả lời khó đánh giá về tính chính xác (‡1233); hoặc thực hiện những hành động mà tính hữu ích hay có hại còn tùy thuộc vào ý kiến chủ quan (‡1234). Bàn 3.7 đưa ra ví dụ về những thách thức này. Một số nghiên cứu nhằm phát triển các phương pháp giúp con người đánh giá tốt hơn các giải pháp cho những nhiệm vụ phức tạp với sự hỗ trợ của AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tuy nhiên, hiện nay các phương pháp này có độ tin cậy hạn chế, và mức độ chúng được sử dụng để huấn luyện những mô hình AI tiên tiến nhất hiện nay chưa được công khai.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Nịnh bợ/chiều theo ý (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Mô hình chỉ đưa ra phản hồi tích cực, không chỉ ra rằng bài haiku không có cấu trúc âm tiết 5-7-5 chuẩn.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Một số hành động hữu ích trong một số bối cảnh nhưng lại có hại trong những bối cảnh khác (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Thông tin về nguy cơ sinh học có thể được sử dụng cho mục đích giáo dục và phòng thủ, nhưng cũng có thể cung cấp thông tin cho các tác nhân độc hại.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hành vi chính xác khó xác minh (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black||11|13|br Khó đánh giá tính chính xác của câu trả lời này vì việc đó đòi hỏi chuyên môn y tế. Ngay cả với một bác sĩ giàu kinh nghiệm, việc đánh giá những câu trả lời như thế này cũng cần thời gian và sự chú ý tỉ mỉ đến từng chi tiết.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Con người bất đồng về điều gì là đúng (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Mọi người bất đồng đáng kể về cách phản ứng đúng đắn.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.7: Lời nhắc của người dùng và phản hồi của mô hình AI
>white|black||9|11|br Ví dụ về những thách thức trong việc xác định và khuyến khích các hành động có lợi từ các mô hình AI.


>white|orangered|left|14|15.5|bb Con người không phải lúc nào cũng đồng thuận về những hành vi nào là đáng mong muốn, vì vậy cần có các phương pháp để cân bằng những sở thích xung đột.

Con người không phải lúc nào cũng đồng thuận về những phản hồi hoặc hành động mà các mô hình AI nên hoặc không nên đưa ra (‡1006). Điều này khiến việc phát triển các mô hình có hành động và tác động nhìn chung phù hợp với lợi ích của xã hội trở nên vô cùng khó khăn (‡420). Một số nhà nghiên cứu tìm hiểu xem sở thích của ai được phản ánh trong các hệ thống AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) và nỗ lực phát triển các kỹ thuật ‘căn chỉnh đa nguyên’ nhằm tạo thế cân bằng giữa những sở thích cạnh tranh nhau (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Chẳng hạn, các nhà phát triển AI có thể thiết kế hệ thống để tránh tạo ra những câu trả lời gây tranh cãi bằng cách từ chối đáp ứng một số yêu cầu nhất định, căn chỉnh theo quan điểm trung vị trong một mẫu người có liên quan, hoặc cá nhân hóa hệ thống cho từng người dùng.

Một thách thức phổ biến đối với các phương pháp này là nhìn chung, các hệ thống AI không thể căn chỉnh đồng đều với sở thích của tất cả mọi người, và những tác động xã hội về sau của chúng sẽ ảnh hưởng khác nhau đến các nhóm người khác nhau. Một số nhà nghiên cứu cho rằng phần lớn các phương pháp kỹ thuật nhằm đạt được sự căn chỉnh đa nguyên không giải quyết được, thậm chí có thể khiến người ta xao nhãng khỏi những thách thức sâu xa hơn, chẳng hạn như thiên kiến có tính hệ thống, động lực quyền lực trong xã hội và sự tập trung của cải, ảnh hưởng (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Các nhà phát triển AI sử dụng ‘huấn luyện đối kháng’ để cải thiện độ vững của mô hình.

Việc bảo đảm các mô hình AI có thể áp dụng một cách đáng tin cậy những hành vi có lợi mà chúng học được trong quá trình huấn luyện vào các bối cảnh triển khai trong thế giới thực là một thách thức. Ngay cả những mô hình được huấn luyện bằng tín hiệu học tập ‘hoàn hảo’ cũng có thể không khái quát hóa thành công sang mọi bối cảnh chưa từng gặp (‡738, ‡739, ‡1255, ‡1256, ‡1257). Ví dụ, một số nhà nghiên cứu nhận thấy rằng chatbot có nhiều khả năng thực hiện các hành động gây hại hơn khi sử dụng những ngôn ngữ ít xuất hiện trong dữ liệu huấn luyện của chúng (‡159, ‡880, ‡1258*, ‡1259), trong đó có nhiều ngôn ngữ chủ yếu được sử dụng ở các nước Nam bán cầu.

Trong những năm gần đây, các nhà nghiên cứu cũng đã tạo ra một bộ công cụ phong phú gồm các kỹ thuật ‘tấn công đối kháng’ có thể được sử dụng để khiến mô hình tạo ra những phản hồi có khả năng gây hại (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Ví dụ, một sáng kiến gần đây đã huy động cộng đồng đóng góp hơn 60,000 ví dụ đa dạng về các cuộc tấn công thành công nhằm vào các mô hình AI state- of-the-art, khiến các mô hình này vi phạm chính sách của công ty về hành vi được chấp nhận của mô hình (‡1149). Bàn 3.8 trình bày các ví dụ về kỹ thuật ‘jailbreak’ mà các nhà nghiên cứu đã chứng minh có thể khiến mô hình làm theo các yêu cầu gây hại.

Một phương pháp cải thiện độ bền vững của mô hình được gọi là ‘huấn luyện đối kháng’ (‡1064). Phương pháp này bao gồm việc tạo ra các ‘cuộc tấn công’ (ví dụ: jailbreak) nhằm khiến mô hình hành xử không mong muốn, rồi huấn luyện mô hình xử lý những cuộc tấn công này một cách phù hợp. Tuy nhiên, huấn luyện đối kháng không hoàn hảo (‡1260, ‡1261). Những kẻ tấn công liên tục phát triển được các cuộc tấn công mới thành công nhằm vào những mô hình tiên tiến nhất (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Vì nhà phát triển cần những ví dụ cụ thể về các dạng lỗi để huấn luyện mô hình chống lại chúng (‡512, ‡1263), kết quả là một trò chơi ‘mèo vờn chuột’ không ngừng, trong đó nhà phát triển liên tục cập nhật mô hình để ứng phó với các lỗ hổng mới được phát hiện, còn các đối thủ liên tục tìm kiếm những cuộc tấn công mới. Một số nhà nghiên cứu đã đề xuất huấn luyện đối kháng ở quy mô lớn hơn (‡1264, ‡1265) hoặc các thuật toán mới (‡675, ‡676, ‡1263, ‡1266, ‡1267) để cải thiện độ bền vững, nhưng các hệ thống AI hiện đại vẫn thường xuyên dễ bị tấn công.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Đưa ra các yêu cầu gây hại dưới dạng văn bản mã hóa, chẳng hạn như mã Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Định hướng trước cho hệ thống bằng các ví dụ về phản hồi tuân thủ đối với các yêu cầu có hại (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Đưa ra các yêu cầu có hại bằng những ngôn ngữ ít- tài nguyên, có khả năng ít được sử dụng trong quá trình huấn luyện (ví dụ: tiếng Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Chia một nhiệm vụ có hại thành nhiều nhiệm vụ phụ vô hại (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.8: Các chiến lược vượt rào an toàn
>white|black||9|11|br Các tác nhân độc hại và các đội đỏ đã sử dụng nhiều loại “jailbreak” khác nhau để khiến các mô hình AI làm theo những yêu cầu có hại mà bình thường chúng sẽ từ chối do các biện pháp bảo vệ. Các ví dụ đầu ra được các tác giả của Báo cáo soạn thảo nhằm mục đích minh họa. Nhiều mô hình AI hiện đại nhất hiện nay đã chống lại được hầu hết các phương pháp này, nhưng các kỹ thuật jailbreak mới vẫn tiếp tục được phát hiện.


>white|orangered|left|14|15.5|bb Các kỹ thuật “học quên” có thể giảm thiểu những năng lực có hại cụ thể của mô hình.

Một chiến lược khác để giảm thiểu rủi ro từ AI đa dụng là tinh chỉnh các mô hình để chúng không có năng lực trong một số lĩnh vực cụ thể có rủi ro cao (‡1175, ‡1176). Ví dụ, các nhà nghiên cứu đang nỗ lực phát triển những thuật toán “machine unlearning” có thể chủ động hạn chế các năng lực liên quan đến mối đe dọa sinh học hoặc khả năng tạo ra hình ảnh chân thực như ảnh chụp về cơ thể người khỏa thân (‡903, ‡1272, ‡1273). Những phương pháp này có thể giúp mô hình an toàn hơn đáng kể, nhưng phải đánh đổi bằng việc hạn chế một số ứng dụng có ích của các năng lực bị loại bỏ. Việc hạn chế kiến thức của các mô hình AI trong những lĩnh vực có hại cũng được đề xuất như một cách thiết kế các mô hình trọng số mở “chống can thiệp”, có khả năng chống lại việc tinh chỉnh có hại (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tuy nhiên, cho đến nay, việc thực hiện điều này một cách vững chắc vẫn còn là thách thức (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Xem §3.4. Mô hình trọng số mở để biết thêm thảo luận.

>white|orangered|left|14|15.5|bb Một số nhà nghiên cứu đang phát triển các phương pháp nhằm đưa ra những bảo đảm an toàn vững chắc hơn thông qua việc diễn giải các trạng thái nội tại của mô hình hoặc xác minh toán học

Một số nhà nghiên cứu đang nghiên cứu các phương pháp nhằm xác minh nghiêm ngặt hơn các thuộc tính liên quan đến an toàn của mô hình. Trong một hướng tiếp cận, các nhà nghiên cứu tìm cách diễn giải những phép tính nội bộ của mô hình để xác định rủi ro hoặc đưa ra lập luận thuyết phục hơn rằng mô hình an toàn (‡1285, ‡1286). Chẳng hạn, trong một nghiên cứu chứng minh tính khả thi, các nhà nghiên cứu cho thấy những công cụ phân tích phép tính nội bộ của mô hình ngôn ngữ có thể giúp người đánh giá xác định các hành vi gây hại (‡1287). Năm 2025, Anthropic cũng bắt đầu phân tích nội bộ mô hình như một cách nghiên cứu nhận thức tình huống và “ý định” của mô hình (‡2). Tuy nhiên, hiện nay những phương pháp này chưa phổ biến và chưa được biết đến là có khả năng cạnh tranh với các kỹ thuật đánh giá khác.

Một cách tiếp cận khác để đưa ra những đảm bảo mạnh mẽ hơn về tính an toàn là xây dựng các chứng minh toán học cho thấy một mô hình sẽ đáp ứng một số điều kiện an toàn nhất định (‡1177, ‡1282, ‡1288). Tuy nhiên, các chứng minh này giả định rằng bối cảnh kiểm thử phù hợp với bối cảnh triển khai và chưa được kiểm nghiệm trước nhiều kiểu đối thủ.

Hiện tại, chúng cũng chưa thể được mở rộng để áp dụng cho các mô hình lớn. Nhìn chung, các chuyên gia vẫn còn tranh luận đáng kể về tiềm năng của các phương pháp diễn giải và xác minh hình thức.

###@ Giám sát và kiểm soát tại thời điểm triển khai

Ngoài các biện pháp bảo vệ được triển khai trong quá trình phát triển mô hình, tuyến phòng thủ thứ hai chống lại các hành vi gây hại là các biện pháp bảo vệ bên ngoài, tập trung vào việc giám sát và kiểm soát hành động của mô hình hoặc hệ thống trong quá trình triển khai. Những biện pháp này giúp giảm thiểu sự cố và hành vi sử dụng sai mục đích, chẳng hạn như đầu ra bị ảo giác và các chỉ dẫn gây hại.

>white|orangered|left|14|15.5|bb Các đơn vị triển khai mô hình có thể sử dụng nhiều công cụ khác nhau để xác định và xử lý các hành vi có rủi ro cao của mô hình.

Khi một hệ thống AI đang hoạt động, đơn vị triển khai có thể giám sát các dấu hiệu rủi ro và can thiệp nếu chúng xuất hiện. Ví dụ, họ có thể kiểm tra đầu vào của mô hình để tìm dấu hiệu tấn công đối kháng, lọc nội dung không phù hợp khỏi đầu ra hoặc giám sát chuỗi suy nghĩ của hệ thống để phát hiện dấu hiệu về các kế hoạch gây hại. Các điểm mà đơn vị triển khai có thể giám sát và can thiệp vào cách mọi người sử dụng hệ thống của họ bao gồm phần cứng (‡1180, ‡1181), tương tác của người dùng (‡1154, ‡1166), đầu vào và đầu ra (‡65, ‡725, ‡1182), các phép tính nội bộ (‡744, ‡1183, ‡1184) và chuỗi suy nghĩ (‡430, ‡435). Đơn vị triển khai cũng có thể thực hiện nhiều hành động khi phát hiện rủi ro. Những hành động này bao gồm ghi nhật ký thông tin, lọc/chỉnh sửa nội dung gây hại, gắn cờ hoạt động bất thường, tắt hệ thống hoặc kích hoạt các cơ chế an toàn dự phòng. Nhân vật 3.7 minh họa các ví dụ về những cơ chế giám sát và kiểm soát phổ biến.

Vì linh hoạt và thường phát huy hiệu quả, các cơ chế này được sử dụng rộng rãi và có thể ngăn ngừa nhiều loại tác hại ngoài ý muốn (‡725, ‡751, ‡1289). Tuy nhiên, các biện pháp bảo vệ này chưa hoàn hảo, đặc biệt trước những cuộc tấn công ác ý được tối ưu hóa để khiến chúng thất bại (‡752, ‡1182). Nghiên cứu gần đây cũng tìm hiểu cách thức hoạt động giám sát có thể không đáng tin cậy nếu một hệ thống được tối ưu hóa dựa trên điểm số của bộ giám sát, chẳng hạn như bằng cách làm cho chuỗi suy nghĩ kém đáng tin cậy hơn (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Nhân vật vật 3.7: Các kỹ thuật giám sát và kiểm soát
>white|black||9|11|br Các kỹ thuật giám sát và kiểm soát được triển khai tại nhiều điểm: sàng lọc đầu vào và đầu ra để phát hiện nội dung có hại, theo dõi các trạng thái bên trong của mô hình, hạn chế các hành động bên ngoài thông qua môi trường hộp cát và duy trì sự giám sát của con người. Nguồn: Báo cáo An toàn AI Quốc tế 2026.


>white|orangered|left|14|15.5|bb Con người tham gia vào quy trình cho phép giám sát trực tiếp trong các bối cảnh có rủi ro cao.

Để giảm khả năng xảy ra sự cố do các tác nhân AI gây ra (xem §2.2.1. Thách thức về độ tin cậy), các đơn vị triển khai có thể hướng tới thiết kế các hệ thống AI hoạt động phối hợp với con người thay vì hoàn toàn tự chủ (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Điều này rất quan trọng đối với các trường hợp sử dụng mà những quyết định sai lầm có thể gây tổn hại nghiêm trọng, chẳng hạn như trong lĩnh vực tài chính, chăm sóc sức khỏe hoặc cảnh sát. Tuy nhiên, việc duy trì sự tham gia của con người trong quy trình thường không khả thi. Đôi khi, việc ra quyết định diễn ra quá nhanh, chẳng hạn như trong các ứng dụng trò chuyện có hàng triệu người dùng. Trong những trường hợp khác, sự thiên kiến và sai sót của con người có thể khuếch đại rủi ro do các sai sót cộng dồn (‡1187). Con người tham gia trong quy trình cũng thường có xu hướng mắc phải “thiên kiến tự động hóa”, nghĩa là họ thường đặt niềm tin vào hệ thống AI nhiều hơn mức hợp lý (‡1190, ‡1191) (xem §2.3.2. Rủi ro đối với quyền tự chủ của con người).

>white|orangered|left|14|15.5|bb “Cơ chế sandbox bảo vệ khỏi các rủi ro phát sinh từ hành vi tự chủ”

Các tác nhân AI có thể hành động tự chủ mà không bị giới hạn trên Web hoặc trong thế giới vật lý gây ra rủi ro cao hơn (xem §2.2.1. Thách thức về độ tin cậy). “Cách ly trong môi trường sandbox” là việc hạn chế các cách mà tác nhân AI có thể trực tiếp tác động đến thế giới, nhờ đó việc giám sát và quản lý chúng trở nên dễ dàng hơn nhiều (‡640, ‡1192, ‡1295). Ví dụ, hạn chế khả năng đăng lên internet hoặc chỉnh sửa hệ thống tệp của máy tính của một hệ thống AI có thể ngăn ngừa những tác hại ngoài ý muốn do các hành động bất ngờ gây ra (‡1296). Tuy nhiên, những phương pháp này không phải lúc nào cũng có thể áp dụng cho các ứng dụng mà hệ thống AI nhất thiết phải trực tiếp hành động trong thế giới.

###@ Công cụ giám sát hệ sinh thái: nguồn gốc mô hình và dữ liệu

Các công cụ truy xuất nguồn gốc mô hình và dữ liệu là những công cụ kỹ thuật giúp nghiên cứu hệ sinh thái AI, nhằm nâng cao nhận thức về các mục đích sử dụng và tác động ở hạ nguồn của các hệ thống AI.

>white|orangered|left|14|15.5|bb Các kỹ thuật xác định nguồn gốc hệ thống AI giúp truy vết việc sử dụng và tác động của các hệ thống.

Các nhà phát triển và đơn vị triển khai có thể sử dụng nhiều kỹ thuật khác nhau để nghiên cứu việc sử dụng mô hình và mức độ phổ biến của chúng «ngoài thực tế». Ví dụ, họ có thể tạo cho các mô hình những hành vi nhận dạng riêng biệt (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) hoặc áp dụng các mẫu riêng biệt vào trọng số của từng mô hình có trọng số mở (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Tuy nhiên, việc tăng khả năng chống chịu của những kỹ thuật này trước các sửa đổi đối với mô hình vẫn là một vấn đề chưa được giải quyết (‡1195, ‡1196*). Các nhà nghiên cứu cũng đang phát triển những phương pháp để «suy luận nguồn gốc mô hình» (‡1197, ‡1198, ‡1305, ‡1306), giúp trả lời những câu hỏi như: «Mô hình X là phiên bản được tinh chỉnh hay chưng cất từ mô hình Y?» Cuối cùng, một số nhà phát triển đang hướng tới xây dựng các giao thức và cơ sở hạ tầng cho tác tử AI, nhằm hỗ trợ việc nhận dạng và xác minh khi chúng tương tác với các hệ thống bên ngoài (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Nhân vật vật 3.8: Dấu chìm nhúng các nhiễu loạn không thể nhận biết vào hình ảnh và âm thanh
>white|black||9|11|br Dấu chìm nhúng những biến đổi nhiễu không thể nhận thấy vào hình ảnh và âm thanh, cho phép các công cụ phát hiện xác định nội dung do AI tạo ra. Trong hình này, dấu chìm trên cả hình ảnh và âm thanh đều được phóng đại để dễ nhìn thấy. Nguồn: hình ảnh Chameleon từ Unsplash (‡1313*). Các thành phần khác do các tác giả Báo cáo tạo ra. Báo cáo An toàn AI Quốc tế 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Nhân vật vật 3.9: Tỷ lệ thành công của các cuộc tấn công chèn prompt
>white|black||9|11|br Tỷ lệ thành công của các cuộc tấn công chèn lệnh, theo báo cáo của các nhà phát triển AI đối với những mô hình lớn được phát hành từ tháng 5 năm 2024 đến tháng 8 năm 2025. Mỗi điểm biểu thị tỷ lệ các cuộc tấn công thành công trong 10 lần thử nhằm vào một mô hình nhất định, ngay sau khi mô hình được phát hành. Tỷ lệ thành công được báo cáo của những cuộc tấn công này đã giảm dần theo thời gian, nhưng vẫn tương đối cao. Nguồn: Zou và cộng sự 2025 (‡1149), được trích dẫn trong Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Các kỹ thuật phát hiện nội dung AI giúp theo dõi sự lan truyền và tác động của nội dung do AI tạo ra.

Hình mờ, siêu dữ liệu và các công cụ phát hiện nội dung AI khác có thể giúp các nhà nghiên cứu theo dõi và nghiên cứu tác động trong thực tế của nội dung do AI tạo ra. 

Trước hết, hình mờ dữ liệu là những họa tiết tinh tế nhưng khác biệt được chèn vào phương tiện kỹ thuật số, có thể mã hóa thông tin về nguồn gốc của chúng (‡1199, ‡1200, ‡1201*). Đối với văn bản, chúng thường có dạng những thiên lệch tinh tế trong lựa chọn từ ngữ và phong cách (‡1308, ‡1309); đối với hình ảnh và video, chúng là những mẫu tinh tế phủ trên các điểm ảnh (‡1310); còn đối với âm thanh, chúng là những mẫu tinh tế trong sóng âm (‡1311). Nhân vật 3.8 minh họa những điều này.

Ngoài dấu chìm, nội dung do AI tạo ra cũng có thể được lưu bằng các định dạng tệp lưu trữ siêu dữ liệu về cách chúng được tạo ra. Ví dụ, nhiều thiết bị di động lưu các tệp hình ảnh và âm thanh bằng định dạng tệp có thể lưu thông tin về cài đặt máy ảnh, thời gian, vị trí, v.v. (‡1312). Siêu dữ liệu tương tự có thể được dùng để lưu thông tin về việc dữ liệu có được tạo ra bởi một hệ thống AI hay không. Giống như việc lấy dấu vân tay trong pháp y hình sự, dấu chìm và siêu dữ liệu có thể bị giả mạo hoặc xóa bỏ, nhưng vẫn hữu ích.

Các nhà nghiên cứu cũng đang nỗ lực phát triển các công cụ phát hiện nội dung do AI tạo ra (‡1203, ‡1204, ‡1205*) để giúp nhận diện nội dung do AI tạo ra trong thực tế, ngay cả khi không có hình mờ hoặc siêu dữ liệu. Tuy nhiên, các kỹ thuật nhận diện này có tỷ lệ thành công hạn chế.

###@ Cập nhật

Kể từ khi Báo cáo trước được công bố (tháng 1 năm 2025), đã có tiến triển trong việc phát triển các hệ thống AI với nhiều lớp biện pháp bảo vệ hiệu quả. Như đã thảo luận trong §3.2. Các phương thức quản lý rủi ro, phòng thủ nhiều lớp là một nguyên tắc cốt lõi trong quản lý rủi ro (‡1314). Ví dụ, các hệ thống AI kết hợp mô hình được huấn luyện về an toàn với bộ lọc đầu vào, bộ lọc đầu ra và các công cụ giám sát nội dung khác ngày càng được nghiên cứu và triển khai (‡32, ‡65, ‡1182*). Nghiên cứu gần đây cũng cho thấy rằng, mặc dù các nhà phát triển mô hình đã đạt được tiến triển trong việc tăng cường khả năng chống lại các nỗ lực vượt qua biện pháp bảo vệ, những kẻ tấn công vẫn thành công với tỷ lệ cao (Nhân vật 3.9).

###@ Những khoảng trống về bằng chứng

Cần có thêm bằng chứng để giúp các nhà nghiên cứu hiểu và tính đến những hạn chế của các phương pháp hiện có. Các biện pháp bảo vệ kỹ thuật cho hệ thống AI đang được cải thiện, nhưng các kỹ thuật này vẫn có những hạn chế. Ví dụ, tiến độ cải thiện độ vững chắc trong trường hợp xấu nhất của các hệ thống AI đa dụng còn chậm, và có những hạn chế căn bản đối với mức độ toàn diện mà các mô hình có trọng số mở có thể được bảo vệ và giám sát (‡1195, ‡1315, ‡1316) (xem thêm §3.4. Các mô hình có trọng số mở). Trong khi đó, không phải mọi biện pháp bảo vệ kỹ thuật đều phổ biến như nhau, hiệu quả như nhau hoặc đã được kiểm chứng ngang nhau trong thực tế. Ví dụ, huấn luyện đối kháng được sử dụng gần như phổ biến trên các mô hình tiên tiến nhất (‡64*, ‡677), trong khi các kỹ thuật diễn giải mô hình và xác minh hình thức đến nay vẫn ít được sử dụng trong các hệ thống vận hành thực tế (‡1177, ‡1285).

###@ Thách thức đối với các nhà hoạch định chính sách

Những thách thức chính đối với các nhà hoạch định chính sách bao gồm quyết định liệu có nên hỗ trợ nghiên cứu, phát triển, đánh giá và áp dụng các biện pháp bảo vệ kỹ thuật và phương pháp giám sát hay không, và nếu có thì hỗ trợ như thế nào. Điều này khó khăn vì hiểu biết của các nhà khoa học về cách bảo vệ các cơ chế một cách thiết thực nhất vẫn đang phát triển, và các thông lệ tốt nhất vẫn chưa được xác lập. Ví dụ, các nhà phát triển khác nhau áp dụng những biện pháp bảo vệ khác nhau, và cách tiếp cận của họ đối với việc giảm thiểu rủi ro kỹ thuật nói chung cũng rất khác nhau (‡1116). Cuối cùng, việc có các biện pháp bảo vệ kỹ thuật hiệu quả tự nó không đảm bảo an toàn, vì mức độ áp dụng và triển khai có thể khác nhau giữa các nhà phát triển và bối cảnh triển khai.

