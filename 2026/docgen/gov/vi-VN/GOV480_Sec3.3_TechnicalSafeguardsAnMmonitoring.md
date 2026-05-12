##########
>white|orangered|left|14|30|hr Mục 3.3
### 3.3. Biện pháp kỹ thuật và giám sát
>white|orangered|left|24|30|hb Các biện pháp bảo vệ kỹ thuật và giám sát

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black|left|11|15|br      
>oldlace|black||11|15|br  ■ Một loạt các biện pháp bảo đảm kỹ thuật đa dạng được sử dụng ở các giai đoạn khác nhau của việc phát triển và sử dụng AI. Chúng bao gồm các kỹ thuật được áp dụng trong quá trình phát triển mô hình để làm cho hệ thống bền vững hơn và có khả năng chống bị lạm dụng (chẳng hạn như làm sạch và chọn lọc dữ liệu), giám sát và kiểm soát trong thời gian triển khai (chẳng hạn như lọc nội dung và giám sát của con người), và các công cụ sau triển khai để theo dõi hệ sinh thái AI rộng hơn (chẳng hạn như truy xuất nguồn gốc và phát hiện nội dung).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Các biện pháp bảo vệ kỹ thuật có những giới hạn và không thể ngăn chặn hành vi gây hại một cách đáng tin cậy trong mọi bối cảnh. Ví dụ, đôi khi người dùng có thể nhận được các kết quả gây hại bằng cách diễn đạt lại yêu cầu hoặc chia nhỏ yêu cầu thành các bước nhỏ hơn. Tương tự, các công cụ như watermarking vốn được thiết kế để nhận diện nội dung do AI tạo ra thường có thể bị gỡ bỏ hoặc thay đổi, điều này làm giảm độ tin cậy của chúng.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Những hạn chế của các biện pháp bảo vệ riêng lẻ có thể khiến cần đến “phòng thủ theo chiều sâu” để ngăn chặn một số kết quả gây hại nhất định. Ví dụ, một hệ thống có thể kết hợp một mô hình được huấn luyện về an toàn với các bộ lọc đầu vào, các bộ lọc đầu ra và các bộ giám sát nội dung.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi công bố Báo cáo trước đó (Tháng 1 2025), các nhà nghiên cứu đã đạt được tiến bộ trong việc cải thiện các biện pháp đảm bảo an toàn, nhưng vẫn còn những hạn chế cơ bản. Ví dụ, tỷ lệ thành công của các cuộc tấn công được thiết kế để vượt qua các biện pháp đảm bảo an toàn đã giảm, nhưng vẫn ở mức tương đối cao. Ngoài ra, còn tồn tại các hạn chế cơ bản về mức độ có thể đảm bảo an toàn một cách triệt để cho các mô hình trọng số mở.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Một thách thức quan trọng đối với các nhà hoạch định chính sách là bằng chứng còn hạn chế về mức độ hiệu quả của các biện pháp bảo vệ (safeguards) trên nhiều cách sử dụng thực tế khác nhau của các hệ thống AI đa năng (general-purpose AI). Các nhà phát triển AI khác nhau rất nhiều về mức độ họ chia sẻ thông tin về các biện pháp bảo vệ và hoạt động giám sát của mình. Một thách thức nữa là khả năng tồn tại các đánh đổi giữa việc áp dụng các biện pháp bảo vệ mạnh hơn và việc duy trì hiệu năng hoặc tính hữu ích của hệ thống.
>oldlace|black||11|15|br      


Các nhà phát triển AI có thể sử dụng một số biện pháp bảo vệ kỹ thuật hữu ích nhưng chưa hoàn hảo để giảm thiểu và quản lý rủi ro từ các hệ thống AI đa năng, tuy nhiên các thách thức về độ bền vững vẫn còn tồn tại. Các nhà phát triển vẫn không thể hoàn toàn ngăn cản các hệ thống AI đa năng thực hiện ngay cả những hành động gây hại đã được biết đến rộng rãi và công khai, chẳng hạn như việc cung cấp cho người dùng hướng dẫn để thực hiện tội phạm. Ví dụ, các nhà nghiên cứu đã chỉ ra rằng các biện pháp bảo vệ tiên tiến nhất có thể bị vượt qua thông qua các phương pháp nhắc–mồi đối kháng (tức là ‘jailbreaks’) (‡1055, ‡1063, ‡1142, ‡1143, ‡1144, ‡1145, ‡1146, ‡1147, ‡1148, ‡1149*), bằng cách khiến các mô hình phân rã các tác vụ gây hại phức tạp thành từng bước (‡1150, ‡1151, ‡1152, ‡1153, ‡1154), và thông qua các thay đổi mô hình đơn giản (‡1155, ‡1156, ‡1157, ‡1158, ‡1159, ‡1160, ‡1161, ‡1162, ‡1163, ‡1164, ‡1165, ‡1166). Các nhà nghiên cứu tiếp tục làm việc trên các biện pháp bảo vệ chống lại sự trục trặc và lạm dụng (‡690). Các phương pháp này khác nhau rất nhiều về mục đích và mức độ hiệu quả, và tác động cuối cùng phụ thuộc vào bối cảnh xã hội-kỹ thuật và bối cảnh quản trị rộng hơn trong đó các hệ thống AI được xây dựng và triển khai.

Các biện pháp bảo vệ kỹ thuật có thể được chia rộng rãi thành ba nhóm: các kỹ thuật để phát triển các mô hình an toàn hơn; các kỹ thuật được sử dụng trong giai đoạn triển khai để giám sát và kiểm soát; và các kỹ thuật hỗ trợ giám sát hệ sinh thái sau khi triển khai. Bàn 3.6 tóm tắt các biện pháp bảo vệ kỹ thuật được thảo luận, mức độ hiệu quả của chúng và các thách thức còn tồn tại.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Phát triển các mô hình an toàn hơn
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Dữ liệu được tuyển chọn (‡1167)
  Loại bỏ dữ liệu có hại để ngăn mô hình học các năng lực nguy hiểm. Các phương pháp này có thể hữu ích, bao gồm cho việc phát triển các mô hình mã nguồn mở thiếu các năng lực gây hại và chống lại việc tinh chỉnh gây hại (‡55). Tuy nhiên, vẫn có những thách thức liên quan đến lỗi gán nhãn khi thu thập dữ liệu và khả năng mở rộng (‡1168).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Học tăng cường từ phản hồi của con người (‡64*)
  Huấn luyện mô hình để phù hợp với các mục tiêu đã chỉ định, chẳng hạn như trở nên hữu ích và vô hại. Đây là một cách hiệu quả để giúp mô hình học các hành vi có lợi (‡64*). Tuy nhiên, việc tối ưu quá mức để được con người phê duyệt có thể khiến mô hình hành xử một cách lừa dối hoặc xu nịnh (‡1169).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Kỹ thuật căn chỉnh đa nguyên (‡1170)
  Huấn luyện mô hình để tích hợp nhiều quan điểm khác nhau về việc nó nên hành động như thế nào. Các kỹ thuật này giúp giảm mức độ mà các mô hình ưu tiên những quan điểm cụ thể (‡1170). Tuy nhiên, bất chấp các kỹ thuật này, sự bất đồng giữa con người là không thể tránh khỏi, và thật khó để thiết kế những cách cân bằng các quan điểm cạnh tranh được chấp nhận rộng rãi (‡1171, ‡1172, ‡1173, ‡1174).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Huấn luyện đối kháng (‡677)
  Huấn luyện mô hình để từ chối gây hại (kể cả trong các bối cảnh chưa quen) và để chống lại các cuộc tấn công từ người dùng độc hại (ví dụ: “jailbreaks”). Đây là một phương pháp hiệu quả để giúp mô hình chống lại các nỗ lực lạm dụng (‡1064), nhưng các thách thức về độ bền vững vẫn còn (‡1149*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Máy “unlearning” (‡1175, ‡1176)
  Huấn luyện một mô hình bằng các thuật toán chuyên biệt nhằm chủ động ức chế các năng lực gây hại (ví dụ: hiểu biết về tác nhân sinh học gây nguy hại). Những kỹ thuật này cung cấp một cách tiếp cận có mục tiêu để loại bỏ các năng lực gây hại khỏi mô hình (‡1175, ‡1176), nhưng các thuật toán unlearning hiện tại có thể thiếu tính bền vững và gây ra các tác động không mong muốn đến các năng lực khác (‡1159, ‡1161).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các công cụ diễn giải và xác minh an toàn (‡1177)
  Một tập hợp đa dạng các phương pháp thiết kế và kiểm chứng nhằm cung cấp mức đảm bảo chặt chẽ hơn rằng các mô hình có các tính chất liên quan đến an toàn cụ thể. Chúng cho phép người đánh giá đưa ra các khẳng định về an toàn với độ tin cậy cao hơn (‡1177), nhưng các phương pháp hiện tại phụ thuộc vào các giả định và hiếm khi đạt hiệu quả cạnh tranh trong thực tiễn (‡1178).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Giám sát và điều khiển
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cơ chế giám sát dựa trên phần cứng (‡1179, ‡1180, ‡1181)
  Xác minh rằng các quy trình được ủy quyền đang chạy trên phần cứng nhằm nghiên cứu các mối đe dọa bảo mật hoặc tuân thủ quy định. Các cơ chế này cung cấp những cách thức độc đáo để giám sát những phép tính nào đang được thực hiện trên phần cứng và bởi ai (‡1181). Tuy nhiên, các cơ chế phần cứng không thể giám sát cho mọi loại mối đe dọa, và một số kỹ thuật yêu cầu phần cứng chuyên dụng (‡1180, ‡1181).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát tương tác người dùng (‡1154, ‡1166)
  Theo dõi các tương tác của người dùng để phát hiện dấu hiệu của việc sử dụng độc hại có thể giúp nhà phát triển chấm dứt dịch vụ đối với người dùng độc hại (‡1154, ‡1166). Tuy nhiên, việc thực thi có thể vô tình cản trở các hoạt động nghiên cứu hữu ích về an toàn (‡689), và một số dạng lạm dụng khó có thể phát hiện (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát tương tác người dùng (‡1154, ‡1166)
  Việc giám sát tương tác của người dùng để phát hiện dấu hiệu sử dụng độc hại có thể giúp các nhà phát triển chấm dứt dịch vụ đối với người dùng độc hại (‡1154, ‡1166). Tuy nhiên, việc thực thi có thể vô tình cản trở nghiên cứu có lợi cho an toàn (‡689), và một số hình thức lạm dụng rất khó phát hiện (‡1150).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Bộ lọc nội dung (‡65*, ‡725)
  Lọc các đầu vào và đầu ra của mô hình có khả năng gây hại là một cách rất hiệu quả để giảm thiểu các tác hại vô tình và rủi ro lạm dụng (‡725). Tuy nhiên, bộ lọc đòi hỏi thêm năng lực tính toán và dễ bị tổn thương trước một số kiểu tấn công (‡1182*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát phép tính nội bộ của mô hình (‡744, ‡1183, ‡1184)
  Giám sát các dấu hiệu lừa dối hoặc các dạng nhận thức nội bộ khác có hại trong mô hình có thể là một cách hiệu quả để phát hiện sự lừa dối (‡744, ‡1183, ‡1184). Tuy nhiên, các phương pháp hiện tại thiếu tính vững chắc và độ tin cậy (‡1185).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Giám sát chuỗi suy luận (‡430, ‡435)
  Giám sát văn bản chain-of-thought của mô hình để phát hiện các dấu hiệu của hành vi gây hiểu lầm hoặc các dạng suy luận có hại khác là một cách hiệu quả để hiểu và nhận ra các điểm thiếu sót trong cách các mô hình suy luận (‡435). Tuy nhiên, chúng có thể không đáng tin cậy (‡752, ‡753, ‡1186), và nếu các mô hình được huấn luyện để tạo ra chain of thought mang tính vô hại, chúng có thể học hành vi gây hiểu lầm (‡430).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Con người trong vòng lặp (‡1187, ‡1188, ‡1189)
  Giám sát và các cơ chế ghi đè của con người đối với các quyết định của hệ thống là thiết yếu trong một số ứng dụng mang tính an toàn - an ninh cao (‡1187). Tuy nhiên, các kỹ thuật này bị giới hạn bởi thiên kiến do tự động hóa và các giới hạn về tốc độ ra quyết định của con người (‡1190, ‡1191).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Cô lập (‡1192)
  Việc ngăn một tác nhân AI tác động trực tiếp đến thế giới là một cách hiệu quả để hạn chế mức độ nguy hại mà nó có thể gây ra (‡1192). Tuy nhiên, cơ chế cô lập (sandboxing) lại hạn chế khả năng của hệ thống trong việc trực tiếp thực hiện một số tác vụ nhất định (‡1192).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|orangered|left|12|15|hb Các công cụ để tạo điều kiện thuận lợi cho việc giám sát hệ sinh thái
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Các kỹ thuật xác định mô hình AI (‡1193*, ‡1194)
  Việc làm cho các mô hình, hoặc các thể hiện riêng lẻ của mô hình, dễ nhận biết hơn trong các trường hợp sử dụng thực tế sẽ hỗ trợ cho giám định số và nhận thức về hệ sinh thái (‡1195). Tuy nhiên, các kỹ thuật này có thể bị vượt qua bằng một số kiểu chỉnh sửa mô hình (‡1196*).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Suy luận nguồn gốc mô hình AI (‡1197)
  Những kỹ thuật này cho phép các nhà nghiên cứu tìm hiểu cách các mô hình được điều chỉnh trong hệ sinh thái AI, đặc biệt là các mô hình trọng số mở (open-weight). Chúng hỗ trợ cho pháp y kỹ thuật số và nhận thức hệ sinh thái (‡1198), nhưng sẽ cần các dự án quy mô lớn để lập bản đồ đầy đủ hệ sinh thái các mô hình trọng số mở (‡1198).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Watermarks và metadata (‡1199, ‡1200, ‡1201*)
  Những kỹ thuật này giúp phát hiện dễ hơn khi một đoạn văn bản, hình ảnh, video, v.v., đã được tạo ra hoặc chỉnh sửa bởi AI, và bởi hệ thống nào. Chúng tạo điều kiện thuận lợi để nâng cao nhận thức về hệ sinh thái (‡1199, ‡1200, ‡1201*). Tuy nhiên, watermark và siêu dữ liệu có thể bị làm giả hoặc bị gỡ bỏ thông qua một số thay đổi đối với nội dung (‡1202).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Phát hiện nội dung do AI tạo (‡1203, ‡1204, ‡1205*)
  Việc cải thiện khả năng của người dùng trong việc phân biệt giữa nội dung do AI tạo ra và nội dung chân thực giúp cho lĩnh vực pháp y số và nâng cao nhận thức về hệ sinh thái (‡1203, ‡1204). Tuy nhiên, các bộ phân loại có thể không đáng tin cậy (‡1205*) và hiệu năng có thể thay đổi theo từng phương thức.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.6: Các biện pháp bảo vệ kỹ thuật được thảo luận trong phần này
>white|black||9|11|br Tóm tắt các biện pháp bảo vệ kỹ thuật được thảo luận trong phần này, được chia thành các phương pháp để phát triển các mô hình an toàn hơn, giám sát và kiểm soát trong thời gian triển khai, và các kỹ thuật để tạo điều kiện cho việc giám sát hệ sinh thái.


###@ Phát triển các mô hình an toàn hơn

Một tuyến phòng thủ đầu tiên chống lại các tác hại từ các hệ thống AI đa mục đích là làm cho mô hình nền tảng an toàn hơn. Phần này trình bày các cơ chế bảo vệ được “tích hợp sẵn vào các tham số của mô hình” trong quá trình phát triển mô hình (Nhân vật 3.6).

>white|orangered|left|14|15.5|bb Việc tuyển chọn dữ liệu huấn luyện có thể hạn chế sự phát triển của các năng lực tiềm ẩn có thể gây nguy hiểm

Các mô hình AI đa dụng có ích một cách chính xác là vì chúng phát triển một phạm vi rộng các kiến thức và năng lực sau khi xử lý dữ liệu huấn luyện, nhưng một số loại dữ liệu huấn luyện lại chịu trách nhiệm không cân xứng đối với việc phát triển các năng lực có khả năng nguy hiểm. Ví dụ, một mô hình AI được huấn luyện trên các bài báo về virus học có thể có khả năng tốt hơn trong việc cung cấp hỗ trợ cho các tác vụ sinh học có thể gây hại (‡549, ‡1206*) (xem thêm §2.1.4. Rủi ro sinh học và hóa học). Ngoài ra, các bộ tạo ảnh/video được huấn luyện trên các hình ảnh về khỏa thân của con người cũng có thể bị lạm dụng để tạo deepfake thân mật không có sự đồng thuận (‡308, ‡319) (xem thêm §2.1.1. Nội dung do AI tạo ra và hoạt động tội phạm).

Việc lọc dữ liệu huấn luyện là một biện pháp giảm thiểu hiệu quả chống lại một số năng lực không mong muốn (‡319, ‡1167, ‡1207, ‡1208). Tuy nhiên, có thể khó lọc các bộ dữ liệu lớn được dùng để huấn luyện các mô hình AI đa dụng (‡1168) do chi phí cao (‡1209), lỗi khi lọc (‡1210), và các tác động tiêu cực đến chất lượng của bộ dữ liệu (‡1211). Những thách thức này còn trầm trọng hơn bởi tính đa ngôn ngữ của văn bản trên internet (‡1212), các định kiến văn hóa trong điều tiết nội dung (‡1211, ‡1213, ‡1214, ‡1215), và thực tế rằng liệu một phần dữ liệu nhất định có ‘có hại’ hay không phụ thuộc vào các yếu tố ngữ cảnh (‡1216). Tuy vậy, việc lọc các nội dung có khả năng gây hại khỏi dữ liệu huấn luyện cho thấy triển vọng trong việc làm cho các mô hình an toàn một cách đáng tin cậy hơn, bao gồm việc giúp các mô hình trọng số mở (open-weight models) có khả năng chống lại sự can thiệp gây hại tốt hơn (‡55). Mối quan hệ giữa nội dung dữ liệu huấn luyện và các năng lực mô hình nảy sinh (emergent model capabilities) vẫn chưa được hiểu đầy đủ (‡1195), và việc lọc dường như hiệu quả hơn trong việc hạn chế các năng lực có hại khi áp dụng cho các miền kiến thức rộng (‡55) so với các hành vi hẹp hơn (‡1206, ‡1217). Xem §3.4. Open-weight models để thảo luận thêm.

![figure 3.6](images/fig3.6_safeguards.png)

##### Nhân vật vật 3.6: Nơi áp dụng các biện pháp bảo vệ kỹ thuật
>white|black||9|11|br Các biện pháp bảo vệ kỹ thuật có thể được áp dụng ở các giai đoạn khác nhau trong quá trình phát triển mô hình. Việc tuyển chọn và làm sạch dữ liệu (data curation) định hình những gì mô hình học được trong giai đoạn tiền huấn luyện (pre-training) và tinh chỉnh (fine-tuning). Các phương pháp dựa trên huấn luyện như học tăng cường từ phản hồi của con người (reinforcement learning from human feedback) và huấn luyện về độ bền vững (robustness training) điều chỉnh hành vi của mô hình. Các phương pháp kiểm thử như tấn công đối kháng (adversarial attacks) giúp xác định các lỗ hổng còn tồn tại. Một số kỹ thuật, như các thuật toán được thiết kế theo hướng an toàn (safe-by-design algorithms), bao trùm nhiều giai đoạn. Nguồn: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Các phương pháp huấn luyện các mô hình AI đa năng để hữu ích và an toàn chủ yếu dựa vào phản hồi của con người

Việc huấn luyện và đánh giá các mô hình để liên kết một cách đáng tin cậy với các nguyên tắc cấp cao như hữu ích, vô hại và trung thực là rất khó. Trên thực tế, các nhà phát triển nhắm tới việc đạt được điều này bằng cách tinh chỉnh các mô hình AI bằng các minh họa và phản hồi từ con người. Ví dụ, mô hình chủ đạo cho việc tinh chỉnh các mô hình AI, được gọi là ‘học tăng cường từ phản hồi của con người’, dựa trên việc huấn luyện các mô hình để tạo ra các đầu ra mà người gán nhãn đánh giá là tích cực (‡1218). Tuy nhiên, phản hồi tích cực từ con người là một đại diện không hoàn chỉnh cho hành vi mang lại lợi ích (‡737, ‡878, ‡1219, ‡1220) và bị giới hạn bởi lỗi của con người và thiên kiến (‡1169, ‡1221, ‡1222*, ‡1223, ‡1224, ‡1225).

Điều này dẫn đến một số thách thức: các mô hình được tinh chỉnh bằng learning theo reinforcement từ phản hồi của con người đôi khi “chiều” theo người dùng, một hành vi được gọi là “sycophancy” (‡358, ‡740, ‡1226, ‡1227); đưa ra các phản hồi có thể hữu ích trong một số ngữ cảnh nhưng gây hại trong những ngữ cảnh khác (‡1228, ‡1229, ‡1230, ‡1231, ‡1232); đưa ra các phản hồi khó đánh giá về độ đúng (‡1233); hoặc thực hiện các hành động mà mức độ hữu ích hoặc gây hại là vấn đề quan điểm (‡1234). Bàn 3.7 cung cấp các ví dụ về những thách thức này. Một số nghiên cứu nhằm phát triển các phương pháp giúp con người đánh giá tốt hơn các giải pháp cho các tác vụ phức tạp với sự hỗ trợ của AI (‡409, ‡1235, ‡1236, ‡1237, ‡1238, ‡1239, ‡1240, ‡1241*, ‡1242). Tuy nhiên, hiện nay các phương pháp này có độ tin cậy giới hạn, và mức độ chúng được sử dụng để huấn luyện các mô hình AI tiên tiến nhất hiện nay là không được công khai.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Sự xu nịnh/lua nịnh (‡358, ‡740, ‡1226)
![table3.7_1](images/table3.7_1_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Mô hình chỉ đưa ra phản hồi tích cực, nhưng không chỉ ra sự thiếu cấu trúc âm tiết đúng của một bài haiku 5-7-5.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Một số hành động có ích trong một số ngữ cảnh nhưng gây hại trong các ngữ cảnh khác (‡1228, ‡1229, ‡1230, ‡1231, ‡1232)
![table3.7_2](images/table3.7_2_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Thông tin về rủi ro sinh học có thể được sử dụng cho giáo dục và phòng vệ, nhưng cũng để cung cấp thông tin cho các tác nhân độc hại.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Hành vi đúng là khó để xác minh (‡1233*)
![table3.7_3](images/table3.7_3_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black||11|13|br Tính chính xác của câu trả lời này rất khó để đánh giá vì nó cần chuyên môn y tế. Ngay cả đối với một bác sĩ giàu kinh nghiệm, việc đánh giá các câu trả lời như thế này đòi hỏi thời gian và sự chú ý cẩn thận đến từng chi tiết.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black||12|15|bb Con người không đồng ý về điều gì là đúng (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249)
![table3.7_4](images/table3.7_4_challenge.png)
>white|black||11|13|bb Giải thích:
>white|black|left|11|13|br Mọi người bất đồng đáng kể về việc phản hồi đúng là gì.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.7: Lời nhắc người dùng và phản hồi của mô hình AI
>white|black||9|11|br Ví dụ về các thách thức trong việc xác định và tạo động lực cho các hành động có lợi từ các mô hình AI.


>white|orangered|left|14|15.5|bb Con người không phải lúc nào cũng đồng ý về những hành vi nào là đáng mong muốn, vì vậy cần các phương pháp để cân bằng các sở thích cạnh tranh

Con người không phải lúc nào cũng đồng ý về việc các mô hình AI nên hoặc không nên xuất ra những phản hồi hay hành động gì (‡1006). Điều này khiến việc phát triển các mô hình có hành động và tác động phù hợp một cách rộng rãi với lợi ích của xã hội trở nên đặc biệt khó khăn về bản chất (‡420). Một số nhà nghiên cứu tìm hiểu sở thích của ai được phản ánh trong các hệ thống AI (‡1234, ‡1243, ‡1244, ‡1245, ‡1246, ‡1247, ‡1248, ‡1249) và nỗ lực phát triển các kỹ thuật “điều chỉnh mang tính đa nguyên” nhằm hướng tới việc cân bằng giữa các sở thích cạnh tranh (‡1170, ‡1248, ‡1250, ‡1251, ‡1252, ‡1253). Ví dụ, các nhà phát triển AI có thể thiết kế hệ thống để tránh tạo ra các câu trả lời gây tranh cãi bằng cách từ chối phản hồi một số yêu cầu nhất định, hoặc bám theo quan điểm trung vị trong một mẫu người liên quan, hoặc cá nhân hoá hệ thống cho từng người dùng.

Một thách thức phổ biến đối với các cách tiếp cận này là nói chung, các hệ thống AI không thể căn chỉnh một cách ngang bằng với sở thích của mọi người, và các tác động xã hội trong tương lai của chúng sẽ ảnh hưởng đến các nhóm người khác nhau theo những cách khác nhau. Một số nhà nghiên cứu cho rằng phần lớn các cách tiếp cận kỹ thuật đối với căn chỉnh đa nguyên (pluralistic alignment) không giải quyết được các thách thức sâu hơn, thậm chí có thể làm xao nhãng khỏi các thách thức đó, như các thiên kiến mang tính hệ thống, động lực quyền lực trong xã hội, và sự tập trung của cải và ảnh hưởng (‡1171, ‡1172, ‡1173, ‡1174, ‡1254).

>white|orangered|left|14|15.5|bb Các nhà phát triển AI sử dụng ‘adversarial training’ để cải thiện độ bền vững của mô hình

Việc đảm bảo rằng các mô hình AI có thể chuyển giao một cách vững chắc các hành vi có lợi mà chúng học được trong quá trình huấn luyện sang các bối cảnh triển khai trong thực tế là một thách thức. Ngay cả các mô hình được huấn luyện với một “tín hiệu học tập” “hoàn hảo” cũng có thể không tổng quát hoá thành công tới tất cả các bối cảnh chưa từng gặp (‡738, ‡739, ‡1255, ‡1256, ‡1257). Ví dụ, một số nhà nghiên cứu đã phát hiện rằng chatbot có xu hướng thực hiện các hành động gây hại nhiều hơn trong các ngôn ngữ có dữ liệu huấn luyện bị thiếu hụt (‡159, ‡880, ‡1258*, ‡1259), bao gồm nhiều ngôn ngữ được sử dụng chủ yếu ở Toàn cầu Phía Nam.

Trong những năm gần đây, các nhà nghiên cứu cũng đã tạo ra một bộ công cụ lớn gồm các kỹ thuật ‘tấn công đối kháng’ có thể được dùng để khiến các mô hình tạo ra các phản hồi tiềm ẩn gây hại (‡505, ‡1142, ‡1143, ‡1145, ‡1147, ‡1148). Ví dụ, một sáng kiến gần đây đã tổng hợp từ cộng đồng hơn 60,000 ví dụ đa dạng về các cuộc tấn công thành công nhằm vào các mô hình AI hiện đại, qua đó khiến chúng vi phạm các chính sách của công ty về hành vi mô hình được chấp nhận (‡1149). Bàn 3.8 trình bày các ví dụ về các kỹ thuật ‘bẻ khóa’ mà các nhà nghiên cứu đã chứng minh có thể làm cho các mô hình tuân theo các yêu cầu gây hại.

Một phương pháp để cải thiện độ bền vững của mô hình được gọi là ‘adversarial training’ (‡1064). Phương pháp này bao gồm việc xây dựng các ‘attacks’ (ví dụ: jailbreaks) được thiết kế nhằm khiến một mô hình hành xử không mong muốn, và huấn luyện mô hình để xử lý các attacks này một cách phù hợp. Tuy nhiên, adversarial training là không hoàn hảo (‡1260, ‡1261). Các kẻ tấn công liên tục có khả năng phát triển các attacks mới thành công chống lại các mô hình hiện đại nhất (‡1063, ‡1146, ‡1149, ‡1261, ‡1262). Vì các nhà phát triển cần các ví dụ cụ thể về các chế độ thất bại để huấn luyện chống lại chúng (‡512, ‡1263), kết quả là một cuộc chơi ‘mèo vờn chuột’ kéo dài: các nhà phát triển liên tục cập nhật mô hình để phản ứng trước các lỗ hổng mới được phát hiện, trong khi các đối thủ liên tục tìm kiếm các attacks mới. Một số nhà nghiên cứu đã đề xuất adversarial training quy mô lớn hơn (‡1264, ‡1265) hoặc các thuật toán mới (‡675, ‡676, ‡1263, ‡1266, ‡1267) nhằm cải thiện độ bền vững, nhưng các hệ thống AI hiện đại vẫn luôn dễ bị tổn thương.

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Tạo các yêu cầu gây hại dưới dạng mã hóa, chẳng hạn như mã Morse (‡1268)
![table3.8_1](images/table3.8_1_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Khởi tạo hệ thống với các ví dụ về phản hồi tuân thủ cho các yêu cầu gây hại (‡1058, ‡1269, ‡1270*)
![table3.8_2](images/table3.8_2_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Thực hiện các yêu cầu gây hại bằng các ngôn ngữ có tài nguyên thấp có khả năng ít được sử dụng trong quá trình huấn luyện (ví dụ: Swahili (‡1271))
![table3.8_3](images/table3.8_3_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Chiến lược: Chia một nhiệm vụ gây hại thành nhiều nhiệm vụ con có vẻ vô hại (‡1150)
![table3.8_4](images/table3.8_4_malicious_actor.png)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 3.8: Chiến lược vượt rào (jailbreaking)
>white|black||9|11|br Các tác nhân độc hại và các nhóm red team đã sử dụng nhiều loại “jailbreaks” để buộc các mô hình AI tuân theo các yêu cầu gây hại mà chúng thường sẽ từ chối do các biện pháp bảo vệ. Các ví dụ đầu ra được các tác giả của Báo cáo viết nhằm mục đích minh họa. Nhiều mô hình AI hiện đại hiện nay đã chống lại hầu hết các phương pháp này, nhưng các kỹ thuật jailbreak mới vẫn tiếp tục được phát hiện.


>white|orangered|left|14|15.5|bb Các kỹ thuật “quên có chủ đích” có thể giảm thiểu các khả năng có hại cụ thể của mô hình

Một chiến lược khác để giảm thiểu rủi ro từ AI đa năng là tinh chỉnh (fine-tune) các mô hình để thiếu năng lực trong một số lĩnh vực có nguy cơ cao cụ thể (‡1175, ‡1176). Ví dụ, các nhà nghiên cứu đang làm việc để phát triển các thuật toán “machine unlearning” (tự “quên” máy) có thể đặc biệt ức chế các năng lực liên quan đến mối đe dọa sinh học hoặc đến việc tạo ra các hình ảnh con người trông chân thực (photorealistic) ở trạng thái khỏa thân (‡903, ‡1272, ‡1273). Các phương pháp này có thể làm cho các mô hình an toàn hơn đáng kể, đổi lại là việc hạn chế một số ứng dụng tích cực của các năng lực mà mô hình đã “unlearn”. Việc giới hạn kiến thức của các mô hình AI trong các lĩnh vực gây hại cũng đã được đề xuất như một cách để thiết kế các mô hình “tamper-resistant” (kháng can thiệp) có trọng số mở (open-weight) nhằm chống lại việc tinh chỉnh (fine-tuning) gây hại (‡1274, ‡1275, ‡1276, ‡1277, ‡1278). Tuy nhiên, cho đến nay, điều này vẫn khó thực hiện một cách vững chắc (robustly) (‡1158, ‡1160, ‡1161, ‡1195, ‡1206, ‡1279, ‡1280, ‡1281*, ‡1282, ‡1283, ‡1284). Xem §3.4. Open-weight models để thảo luận thêm.

>white|orangered|left|14|15.5|bb Một số nhà nghiên cứu đang làm việc trên các phương pháp để đạt được các đảm bảo an toàn mạnh hơn thông qua việc diễn giải các trạng thái nội bộ của mô hình hoặc xác minh toán học

Một số nhà nghiên cứu đang làm việc trên các phương pháp để xác minh chặt chẽ hơn các thuộc tính an toàn liên quan đến mô hình. Trong một cách tiếp cận, các nhà nghiên cứu hướng tới việc diễn giải các phép tính nội bộ của mô hình để hoặc là nhận diện rủi ro, hoặc là đưa ra các lập luận thuyết phục hơn rằng mô hình an toàn (‡1285, ‡1286). Ví dụ, trong một bản chứng minh khái niệm, các nhà nghiên cứu đã chỉ ra rằng các công cụ phân tích phép tính nội bộ của một mô hình ngôn ngữ có thể giúp người đánh giá nhận diện các hành vi gây hại (‡1287). Vào năm 2025, Anthropic cũng bắt đầu phân tích các thành phần nội bộ của mô hình như một cách để nghiên cứu khả năng nhận thức tình huống của mô hình và “ý định” (‡2). Tuy nhiên, các kiểu phương pháp này hiện không phổ biến hoặc chưa được biết là có tính cạnh tranh so với các kỹ thuật đánh giá khác.

Một cách tiếp cận khác để tạo ra các đảm bảo mạnh mẽ hơn về an toàn là xây dựng các chứng minh toán học rằng một mô hình sẽ thỏa mãn một số điều kiện an toàn nhất định (‡1177, ‡1282, ‡1288). Tuy nhiên, các chứng minh này giả định rằng bối cảnh kiểm thử khớp với bối cảnh triển khai và chưa được kiểm thử trước nhiều loại kẻ tấn công.

Hiện tại, chúng cũng không thể được mở rộng để áp dụng cho các mô hình lớn. Nhìn chung, các chuyên gia đang tranh luận đáng kể về tiềm năng của khả năng diễn giải và các phương pháp xác minh hình thức.

###@ Giám sát và điều khiển tại thời điểm triển khai

Ngoài các biện pháp bảo vệ được triển khai trong quá trình phát triển mô hình, một lớp phòng vệ thứ hai chống lại các hành vi gây hại là các biện pháp bảo vệ từ bên ngoài, tập trung vào việc giám sát và kiểm soát các hành động của mô hình hoặc hệ thống trong giai đoạn triển khai. Các biện pháp này giúp giảm thiểu sự cố và việc lạm dụng, chẳng hạn như các đầu ra bịa đặt (hallucinated outputs) và các hướng dẫn gây hại.

>white|orangered|left|14|15.5|bb Các trình triển khai mô hình có thể sử dụng nhiều công cụ khác nhau để xác định và xử lý các hành vi của mô hình có nguy cơ cao

Khi một hệ thống AI đang chạy, một người triển khai (deployer) có thể theo dõi các dấu hiệu rủi ro và can thiệp nếu chúng xuất hiện. Ví dụ, họ có thể kiểm tra các đầu vào của một mô hình để phát hiện dấu hiệu của các cuộc tấn công đối kháng, lọc nội dung không phù hợp khỏi các đầu ra, hoặc theo dõi chuỗi suy nghĩ (chain of thought) của hệ thống để phát hiện các kế hoạch gây hại. Các điểm mà người triển khai có thể theo dõi và can thiệp vào cách con người sử dụng hệ thống của họ bao gồm phần cứng (‡1180, ‡1181), tương tác người dùng (‡1154, ‡1166), đầu vào và đầu ra (‡65, ‡725, ‡1182), các phép tính nội bộ (‡744, ‡1183, ‡1184), và chuỗi suy nghĩ (‡430, ‡435). Ngoài ra, khi phát hiện rủi ro, người triển khai có thể thực hiện nhiều hành động khác nhau. Chúng bao gồm ghi nhật ký thông tin, lọc/sửa đổi nội dung gây hại, gắn cờ cảnh báo cho hoạt động bất thường, tắt hệ thống, hoặc kích hoạt cơ chế dự phòng (failsafes). Nhân vật 3.7 minh hoạ các ví dụ về cơ chế giám sát và kiểm soát phổ biến.

Vì chúng linh hoạt và thường hiệu quả, các cơ chế này được sử dụng rộng rãi và có thể ngăn nhiều loại tác hại không chủ ý (‡725, ‡751, ‡1289). Tuy nhiên, các biện pháp bảo vệ này không hoàn hảo, đặc biệt trong các cuộc tấn công độc hại được tối ưu hóa để khiến chúng thất bại (‡752, ‡1182). Nghiên cứu gần đây cũng đã khám phá cách giám sát có thể không đáng tin cậy nếu một hệ thống được tối ưu hóa dựa trên các điểm số của một bộ giám sát, ví dụ, bằng cách làm cho chuỗi suy nghĩ kém đáng tin cậy hơn (‡435*, ‡1185, ‡1290).

![figure 3.7](images/fig3.7_monitoring_and_control.png)

##### Nhân vật vật 3.7: Kỹ thuật giám sát và điều khiển
>white|black||9|11|br Các kỹ thuật giám sát và kiểm soát hoạt động tại nhiều điểm: sàng lọc đầu vào và đầu ra để phát hiện nội dung gây hại, theo dõi các trạng thái nội bộ của mô hình, giới hạn các hành động bên ngoài thông qua cơ chế hộp cát (sandboxing), và duy trì sự giám sát của con người. Nguồn: International AI Safety Report 2026.


>white|orangered|left|14|15.5|bb Con người trong vòng lặp cho phép giám sát trực tiếp trong các bối cảnh có rủi ro cao

Để giảm khả năng xảy ra lỗi từ các tác nhân AI (xem §2.2.1. Thách thức về độ tin cậy), bên triển khai có thể hướng tới việc thiết kế các hệ thống AI hoạt động phối hợp với con người thay vì tự vận hành hoàn toàn (‡1188, ‡1189, ‡1291*, ‡1292, ‡1293, ‡1294). Điều này đặc biệt quan trọng đối với các trường hợp sử dụng mà các quyết định sai có thể gây ra hậu quả nghiêm trọng, chẳng hạn trong tài chính, y tế hoặc cảnh sát. Tuy nhiên, việc có “con người tham gia vòng lặp” (human in the loop) thường là không thực tế. Đôi khi việc ra quyết định diễn ra quá nhanh, như trong các ứng dụng chat với hàng triệu người dùng. Ở những trường hợp khác, định kiến và sai sót của con người có thể làm gia tăng rủi ro do các lỗi chồng lấp (‡1187). Con người trong vòng lặp cũng thường thể hiện “thiên kiến do tự động hóa” (automation bias), nghĩa là họ thường đặt nhiều niềm tin hơn vào hệ thống AI so với mức mà hệ thống đó xứng đáng (‡1190, ‡1191) (xem §2.3.2. Rủi ro đối với quyền tự chủ của con người).

>white|orangered|left|14|15.5|bb ‘Sandboxing’ giúp bảo vệ khỏi các rủi ro phát sinh từ các hành vi tự động

Các tác nhân AI có thể hoạt động tự động mà không bị giới hạn trên Web hoặc trong thế giới vật lý sẽ gây ra các rủi ro cao hơn (xem §2.2.1. Các thách thức về độ tin cậy). ‘Sandboxing’ bao gồm việc giới hạn các cách thức mà tác nhân AI có thể tác động trực tiếp đến thế giới, từ đó việc giám sát và quản lý chúng trở nên dễ dàng hơn nhiều (‡640, ‡1192, ‡1295). Ví dụ, việc hạn chế khả năng của một hệ thống AI trong việc đăng lên internet hoặc chỉnh sửa hệ thống tệp của máy tính có thể ngăn ngừa các tác hại bất ngờ từ các hành động bất ngờ (‡1296). Tuy nhiên, các cách tiếp cận này không phải lúc nào cũng có thể được sử dụng cho các ứng dụng mà ở đó hệ thống AI buộc phải hành động trực tiếp trong thế giới.

###@ Công cụ giám sát hệ sinh thái: mô hình và nguồn gốc dữ liệu

Công cụ mô hình và nguồn gốc dữ liệu là các công cụ kỹ thuật để nghiên cứu hệ sinh thái AI, nhằm nâng cao nhận thức về các mục đích sử dụng và tác động đầu nguồn của các hệ thống AI.

>white|orangered|left|14|15.5|bb Các kỹ thuật truy xuất nguồn gốc (provenance) của hệ thống AI giúp truy vết việc sử dụng và tác động của các hệ thống đó

Các nhà phát triển và người triển khai có thể sử dụng nhiều kỹ thuật khác nhau để nghiên cứu việc sử dụng mô hình và sự lan truyền “trong thế giới thực”. Ví dụ, họ có thể cho mô hình các hành vi nhận dạng duy nhất (‡1193, ‡1297, ‡1298, ‡1299, ‡1300) hoặc áp dụng các mẫu duy nhất lên trọng số của từng mô hình mã nguồn mở (open-weight) (‡1193, ‡1194, ‡1301, ‡1302, ‡1303, ‡1304). Tuy nhiên, việc làm cho các kỹ thuật này có khả năng chống chịu tốt hơn trước các sửa đổi đối với mô hình vẫn là một bài toán mở (‡1195, ‡1196*). Các nhà nghiên cứu cũng đang phát triển các phương pháp để “suy luận nguồn gốc mô hình” (‡1197, ‡1198, ‡1305, ‡1306), giúp trả lời các câu hỏi thuộc dạng: “Mô hình X có phải là phiên bản được tinh chỉnh (fine-tuned) hoặc được chưng cất (distilled) từ mô hình Y hay không?” Cuối cùng, một số nhà phát triển đang hướng tới các giao thức và hạ tầng cho các tác nhân AI để hỗ trợ việc nhận dạng và xác minh khi chúng tương tác với các hệ thống bên ngoài (‡661, ‡1307).

![figure 3.8](images/fig3.8_wantermarks.png)

##### Nhân vật vật 3.8: Watermarks nhúng các nhiễu loạn không thể nhận biết vào hình ảnh và âm thanh
>white|black||9|11|br Watermark (dấu chìm) nhúng các nhiễu loạn không nhận biết được vào hình ảnh và âm thanh, giúp nội dung được tạo bởi AI có thể được nhận diện bởi các công cụ phát hiện. Trong hình này, watermark của cả hình ảnh và âm thanh được phóng đại để tăng khả năng nhìn thấy. Nguồn: Ảnh Chameleon từ Unsplash (‡1313*). Các yếu tố khác do các tác giả Báo cáo tạo ra. International AI Safety Report 2026.


![figure 3.9](images/fig3.9_prompt_injection_attacks.png)

##### Nhân vật vật 3.9: Tỷ lệ thành công của cuộc tấn công prompt injection
>white|black||9|11|br Tỷ lệ thành công của các cuộc tấn công tiêm nhiễm prompt, theo báo cáo của các nhà phát triển AI cho các mô hình lớn được phát hành trong khoảng từ May 2024 đến August 2025. Mỗi điểm biểu thị tỷ lệ các cuộc tấn công thành công trong 10 lần thử đối với một mô hình nhất định ngay sau khi phát hành. Tỷ lệ thành công của các cuộc tấn công dạng này đã giảm theo thời gian, nhưng vẫn ở mức tương đối cao. Nguồn: Zou et al. 2025 (‡1149), được trích dẫn trong Anthropic 2025 (‡2).


>white|orangered|left|14|15.5|bb Các kỹ thuật phát hiện nội dung do AI tạo ra giúp theo dõi sự lan truyền và tác động của nội dung do AI tạo ra

Chữ ký mờ, siêu dữ liệu và các công cụ phát hiện nội dung AI khác có thể giúp các nhà nghiên cứu theo dõi và nghiên cứu tác động thực tế của nội dung do AI tạo ra. 

Trước hết, watermark dữ liệu (data watermarks) là các hoa văn tinh vi nhưng phân biệt được được nhúng vào phương tiện kỹ thuật số có thể mã hóa thông tin về nguồn gốc của chúng (‡1199, ‡1200, ‡1201*). Đối với văn bản, chúng thường có dạng các sai lệch tinh vi trong cách chọn từ và phong cách (‡1308, ‡1309); đối với hình ảnh và video, các mẫu tinh vi trải trên các pixel (‡1310); và đối với âm thanh, các mẫu tinh vi trong sóng âm (‡1311). Nhân vật 3.8 minh họa điều này.

Ngoài watermark, nội dung do AI tạo ra còn có thể được lưu bằng các định dạng tệp có khả năng lưu metadata về cách chúng được tạo ra. Ví dụ, nhiều thiết bị di động lưu tệp hình ảnh và âm thanh bằng một định dạng tệp có thể lưu thông tin về cài đặt camera, thời gian, vị trí, v.v. (‡1312). Metadata tương tự cũng có thể được dùng để lưu thông tin về việc dữ liệu có được tạo ra bởi một hệ thống AI hay không. Tương tự như dấu vân tay trong pháp y hình sự, watermark và metadata có thể bị can thiệp hoặc bị xóa, nhưng nhìn chung vẫn hữu ích.

Các nhà nghiên cứu cũng đang nỗ lực phát triển các bộ phát hiện nội dung do AI tạo ra (‡1203, ‡1204, ‡1205*) để giúp xác định nội dung do AI tạo ra trong thực tế, ngay cả khi không có watermark hoặc siêu dữ liệu. Tuy nhiên, các kỹ thuật nhận diện này có tỷ lệ thành công hạn chế.

###@ Cập nhật

Kể từ khi phát hành Báo cáo trước đó (Tháng 1 2025), đã có tiến triển trong việc phát triển các hệ thống AI với nhiều lớp cơ chế bảo vệ hiệu quả. Như đã thảo luận trong §3.2. Thực hành quản lý rủi ro, defence-in-depth là một nguyên tắc cốt lõi trong quản lý rủi ro (‡1314). Ví dụ, các hệ thống AI kết hợp các mô hình đã được huấn luyện về an toàn với bộ lọc đầu vào, bộ lọc đầu ra và các bộ giám sát nội dung khác ngày càng được nghiên cứu và triển khai (‡32, ‡65, ‡1182*). Nghiên cứu gần đây cũng cho thấy rằng, mặc dù các nhà phát triển mô hình đã đạt được tiến bộ trong việc tăng cường độ bền vững trước các nỗ lực nhằm vượt qua các cơ chế bảo vệ, thì các tác nhân tấn công vẫn thành công với tỷ lệ cao (Nhân vật 3.9).

###@ Khoảng trống bằng chứng

Cần thêm bằng chứng để giúp các nhà nghiên cứu hiểu và tính đến các hạn chế của các cách tiếp cận hiện có. Các biện pháp bảo vệ kỹ thuật cho các hệ thống AI đang được cải thiện, nhưng các kỹ thuật lại gặp phải những hạn chế. Ví dụ, tiến độ cải thiện độ vững chắc trường hợp xấu nhất của các hệ thống AI đa mục đích còn chậm, và tồn tại những giới hạn cơ bản về mức độ có thể bảo vệ và giám sát triệt để các mô hình trọng số mở (‡1195, ‡1315, ‡1316) (xem thêm §3.4. Các mô hình trọng số mở). Trong khi đó, không phải tất cả các biện pháp bảo vệ kỹ thuật đều phổ biến như nhau, hiệu quả như nhau, hoặc đã được chứng minh như nhau trong thế giới thực. Ví dụ, huấn luyện đối kháng hầu như được sử dụng rộng rãi trên các mô hình đầu bảng (‡64*, ‡677), trong khi các kỹ thuật khả giải thích mô hình và xác minh hình thức nhìn chung ít được dùng đến cho đến nay trong các hệ thống triển khai (‡1177, ‡1285).

###@ Thách thức đối với các nhà hoạch định chính sách

Các thách thức chính đối với các nhà hoạch định chính sách bao gồm việc quyết định liệu và theo cách nào họ nên hỗ trợ nghiên cứu, phát triển, đánh giá, và áp dụng các cơ chế bảo vệ kỹ thuật cũng như các phương pháp giám sát. Điều này là khó khăn vì nhận thức của các nhà khoa học về cách thức tốt nhất để bảo vệ các cơ chế một cách thực tiễn vẫn đang tiếp tục phát triển và các thông lệ tốt nhất vẫn chưa được thiết lập. Ví dụ, các nhà phát triển khác nhau áp dụng các biện pháp bảo vệ khác nhau, và các cách tiếp cận của họ để giảm thiểu rủi ro kỹ thuật nhìn chung cũng có mức độ khác biệt rất lớn (‡1116). Cuối cùng, việc tồn tại các biện pháp bảo vệ kỹ thuật hiệu quả không, tự nó, đảm bảo an toàn, vì việc chấp nhận và triển khai có thể thay đổi giữa các nhà phát triển và các bối cảnh triển khai.

