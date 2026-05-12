Các hệ thống AI đa dụng thất bại theo những cách đã gây ra thiệt hại trong thế giới thực, từ trích dẫn pháp lý bịa đặt đến chẩn đoán y tế sai. Mặc dù các chuyên gia con người cũng mắc lỗi, nhưng các lỗi của AI làm dấy lên những lo ngại riêng biệt do tính mới mẻ của chúng, khả năng mở rộng tiềm tàng, mức độ khó dự đoán khi chúng xảy ra và xu hướng của người dùng tin một cách thiếu phê phán vào các đầu ra nghe có vẻ tự tin. Các lỗi hiện tại của AI đa dụng bao gồm cung cấp thông tin sai (‡602, ‡603), mắc các lỗi suy luận cơ bản (‡604, ‡605), và suy giảm hiệu năng khi được triển khai trong các bối cảnh mới (‡606, ‡607, ‡608). Những tác hại đã được ghi nhận từ các lỗi này bao gồm chẩn đoán y tế sai, sai sót trong các bản bào chữa pháp lý và tổn thất tài chính (‡609, ‡610, ‡611). Các thách thức về độ tin cậy đặc biệt quan trọng đối với các tác nhân AI, vì các lỗi có thể trực tiếp gây hại mà không cần hành động hoặc giám sát của con người (‡612, ‡613, ‡614, ‡615). Các hệ thống đa tác nhân còn tạo ra thêm các kiểu lỗi thông qua việc phối hợp sai, xung đột, hoặc sự thông đồng không mong muốn giữa các tác nhân (‡614, ‡616).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Ảo giác
- Trích dẫn tiền lệ không tồn tại trong bản biện hộ pháp lý (‡617)
- Trích dẫn các chính sách giá vé giảm không tồn tại dành cho hành khách có người thân qua đời (‡618)
- Cung cấp thông tin y tế không chính xác và thiên lệch (‡619)
- Cung cấp thông tin lỗi thời về các sự kiện (‡620)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lỗi suy luận cơ bản
- Không thực hiện được các phép tính toán học (‡621)
- Không suy ra được các quan hệ nhân quả cơ bản (‡622*)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lỗi ngoài phân phối (lỗi trên các đầu vào không quen thuộc hoặc bất thường)
- Nhận nhầm hình ảnh khi ánh sáng nền hoặc ngữ cảnh thay đổi (‡623)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lỗi khi sử dụng công cụ
- Vi phạm quyền riêng tư bằng cách lộ hình ảnh cá nhân của người dùng thông qua một tác nhân AI gửi nó đến một công cụ bên thứ ba (‡624)
- Sự suy giảm của trí nhớ làm việc ngắn hạn (‡625, ‡626)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Failure của hệ thống đa tác nhân: mất phối hợp và xung đột
- Không quản lý được các tài nguyên dùng chung do mâu thuẫn giữa động lực cá nhân và các mục tiêu phúc lợi tập thể (‡627)
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 2.4: Ví dụ về các vấn đề độ tin cậy trong AI đa năng và các hệ thống tác nhân
>white|black||9|11|br Các vấn đề về độ tin cậy đã được ghi nhận trong các hệ thống AI đa năng, các tác nhân AI và các hệ thống đa tác nhân.


###@ Các hệ thống AI đa dụng phải đối mặt với nhiều thách thức về độ tin cậy

Bàn 2.4. tóm tắt các nhóm phổ biến về sự cố độ tin cậy. Ba nhóm đầu áp dụng cho mọi hệ thống AI, trong khi hai nhóm cuối liên quan cụ thể đến tác nhân AI và các hệ thống đa tác nhân. Nhiều rủi ro về độ tin cậy bắt nguồn từ sự khó khăn trong việc dự đoán và giám sát hành vi của hệ thống AI.

Những thách thức này (được thảo luận thêm trong §3.1. Các thách thức về kỹ thuật và thể chế) đặc biệt trở nên nghiêm trọng đối với các tác nhân AI hoạt động trong các môi trường phức tạp. Các kỹ thuật hiện tại để đánh giá và giảm thiểu các lỗi như vậy có thể làm giảm tỷ lệ lỗi, nhưng ngay cả các tác nhân AI hàng đầu vẫn còn đủ không đáng tin cậy để gây ra rủi ro và cản trở việc triển khai trong nhiều bối cảnh.

‘Độ tin cậy’ đề cập đến mức độ mà một hệ thống AI hoạt động đúng như nhà phát triển hoặc người dùng mong đợi. Các hệ thống AI đa mục đích gặp phải nhiều vấn đề về độ tin cậy, từ việc tạo nội dung không chính xác hoặc gây hiểu nhầm đến việc thất bại khi thực hiện các suy luận cơ bản. Ví dụ, trong khi các mô hình đã cải thiện về khả năng gợi nhớ thông tin thực tế, ngay cả các mô hình hàng đầu vẫn tiếp tục đưa ra các câu trả lời tự tin nhưng sai với tỷ lệ đáng kể (Nhân vật 2.10). Trong kỹ thuật phần mềm, AI đa mục đích hiện có thể cung cấp sự hỗ trợ đáng kể trong việc viết, đánh giá và gỡ lỗi mã máy tính (‡215*, ‡628, ‡629). Tuy nhiên, mã do AI tạo ra thường chứa lỗi (‡630), trong khi các tác nhân lập trình thường xuyên mắc sai sót (‡631). Những thất bại như vậy có thể đưa lỗ hổng vào các chương trình và hệ thống bảo mật (xem §2.1.3. Các cuộc tấn công mạng).

Các vấn đề về độ tin cậy đặc biệt quan trọng cần theo dõi trong các bối cảnh có rủi ro cao, như y học, do việc sử dụng AI đang gia tăng nhanh chóng và khả năng xảy ra lỗi có thể dẫn đến hậu quả nghiêm trọng (‡609, ‡619). Các năng lực liên quan đã được cải thiện nhanh chóng; các mô hình hàng đầu hiện nay có thể vượt qua các kỳ thi y khoa (‡633*, ‡634). Tuy nhiên, việc sử dụng trong thực tế cho thấy các hạn chế mà các bộ chuẩn đo lường không phản ánh. Ví dụ, trong một nghiên cứu, các mô hình đã đưa ra những câu trả lời có thể gây hại cho 19% các câu hỏi y khoa được đặt ra (‡635). Những lỗi như vậy có thể dẫn đến chẩn đoán sai, điều trị không phù hợp, hoặc từ chối chăm sóc sức khỏe một cách sai lầm (‡611).

![figure 2.10](images/fig2.10_simpleqa_benchmark.png)

##### Nhân vật vật 2.10: Kết quả của các mô hình chính trên chuẩn đánh giá SimpleQA Verified
>white|black||9|11|br Kết quả của các mô hình chính trên bộ đánh giá Verified SimpleQA theo ngày phát hành mô hình. Bộ đánh giá này đo lường tính đúng sự thật của mô hình, khả năng của mô hình trong việc ghi nhớ lại các sự kiện một cách đáng tin cậy. Nó có định dạng câu hỏi-trả lời (QA) dạng ngắn, được thiết kế để phát hiện các vấn đề về độ tin cậy như hiện tượng bịa đặt (hallucinations). Nguồn: SimpleQA Kaggle  2*).


>white|orangered|left|14|15.5|bb Các tác nhân AI đặt ra các rủi ro tin cậy mới do tính tự chủ của chúng

Vì các tác nhân AI trực tiếp thực hiện hành động trong thế giới thực, nên các thất bại của chúng có khả năng gây ra nhiều tác hại hơn so với thất bại trong các hệ thống không mang tính tác nhân (‡99). Không giống như các hệ thống AI chỉ tạo ra văn bản hoặc hình ảnh để con người xem xét, các tác nhân AI có thể độc lập thực hiện các hành động ảnh hưởng đến thế giới (‡99, ‡615, ‡636, ‡637) (xem thêm §1.1. What is general-purpose AI?). Các tác nhân AI có thể khởi tạo các hành động, tác động đến các con người hoặc hệ thống AI khác, và thay đổi một cách linh hoạt các kết quả trong tương lai. Phạm vi ảnh hưởng mở rộng này tạo ra các rủi ro mới và làm gia tăng tầm quan trọng của độ tin cậy, vì các thất bại có thể trực tiếp gây hại mà không có cơ hội để con người can thiệp (‡99, ‡612, ‡638, ‡639, ‡640). Điều này có thể đặc biệt quan trọng đối với các tác nhân được triển khai trong các bối cảnh mang tính chiến lược hoặc an toàn như dịch vụ tài chính (‡641), quản lý năng lượng (‡642), hoặc nghiên cứu khoa học (‡643*, ‡644).

>white|orangered|left|14|15.5|bb Các hệ thống AI đa tác tử tạo ra các kiểu lỗi độ tin cậy mới

Các hệ thống AI đa tác nhân giới thiệu các loại lỗi độ tin cậy mới do lỗi phối hợp hoặc xung đột giữa các tác nhân. Trong các hệ thống AI đa tác nhân, các tác nhân tương tác với nhau trong khi theo đuổi các mục tiêu chung hoặc mục tiêu riêng (‡614, ‡645, ‡646, ‡647, ‡648, ‡649). Ví dụ, trong một hệ thống đa tác nhân được thiết kế để thực hiện việc rà soát tài liệu nghiên cứu, một tác nhân dẫn dắt sẽ phân rã truy vấn của người dùng và gán các tác vụ con cho các tác nhân con chuyên biệt, trong đó mỗi tác nhân chịu trách nhiệm nghiên cứu một khía cạnh khác nhau song song (‡650*). Mặc dù cách này cho phép tăng hiệu quả, nhưng đồng thời cũng có nghĩa là các sai sót có thể lan truyền giữa các tác nhân (‡614, ‡651, ‡652, ‡653, ‡654, ‡655). Nếu nhiều tác nhân được xây dựng trên cùng một mô hình nền hoặc tích hợp cùng các công cụ, thì chúng cũng có thể thể hiện các lỗi có tương quan (‡656). Bằng chứng thực nghiệm cho các lỗi như vậy trong các hệ thống được triển khai vẫn còn hạn chế, nhưng các rủi ro này có thể gia tăng khi các hệ thống đa tác nhân trở nên phổ biến hơn.

###@ Cập nhật

Kể từ khi công bố Báo cáo trước đó (tháng 1 2025), sự quan tâm của thương mại và nghiên cứu đối với AI agents đã tăng mạnh. Nhiều AI agents hơn đang được triển khai trong thế giới thực (Nhân vật 2.11), hầu hết trong số đó chuyên biệt cho các ứng dụng liên quan đến việc sử dụng máy tính hoặc kỹ thuật phần mềm (‡92). Các bản phát hành gần đây như tác nhân hacking XBOW (‡467), Claude-4 (‡659) và ChatGPT Agent (‡660) cho thấy năng lực tự chủ còn ở giai đoạn ban đầu như việc tạo các bộ slide dựa trên tìm kiếm trên Web (‡660). Tuy nhiên, chúng vẫn chưa thể thực hiện các tác vụ phức tạp hơn như lập kế hoạch và đặt chỗ cho chuyến đi (‡100) vì tỷ lệ thất bại tăng lên đối với các tác vụ dài hơn (‡98, ‡148). Nghiên cứu hiện tại bao gồm các nỗ lực nhằm phát triển các chuẩn mực về cách các agents giao tiếp với các công cụ bên ngoài và với các agents khác (‡661, ‡662). Ví dụ bao gồm các giao thức Agent2Agent của Google (‡663) và Agent Payments (‡664), cùng với Model Context Protocol của Anthropic (‡665).

>oldlace|black||11|15|br      
####@ Ghi chú vật 2.4: Các cuộc tấn công có chủ ý cũng có thể khiến hệ thống AI bị lỗi
>oldlace|black|left|13|15|hb Ghi chú vật 2.4: Các cuộc tấn công có chủ đích cũng có thể khiến các hệ thống AI bị lỗi
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Phần này tập trung vào các sự cố suy giảm độ tin cậy không mong muốn, nhưng các tác nhân độc hại cũng có thể cố ý gây ra sự cố thông qua các tấn công như prompt injection. Trong một tấn công prompt injection, các chỉ dẫn độc hại được đưa cho một tác nhân một cách gián tiếp thông qua các kênh như các chỉ dẫn ẩn trong các trang web hoặc cơ sở dữ liệu (‡507, ‡657, ‡658). Những chỉ dẫn này có thể “chiếm quyền” tác nhân, khiến nó hành động chống lại ý định của người dùng. Các cuộc tấn công như vậy đặc biệt khó để phòng vệ vì chúng được phân phối bằng nội dung bên ngoài, nằm ngoài sự kiểm soát của người dùng hoặc nhà phát triển. Các hệ thống AI là mục tiêu của cuộc tấn công được thảo luận thêm trong §2.1.3. Các cuộc tấn công mạng và các biện pháp phòng thủ kỹ thuật được trình bày trong §3.3. Các biện pháp bảo vệ kỹ thuật và giám sát.
>oldlace|black||11|15|br      

![figure 2.11](images/fig2.11_Dec2024_survey.png)

##### Nhân vật vật 2.11: Số lượng tác nhân AI đã tăng kể từ năm 2023
>white|black||9|11|br Kết quả từ một cuộc khảo sát tháng 12 năm 2024 về 67 tác nhân AI đã triển khai. Bên trái: Dòng thời gian các bản phát hành chính của tác nhân AI. Bên phải: Các lĩnh vực ứng dụng mà trong đó các tác nhân AI đang được sử dụng. Sáu lĩnh vực được định nghĩa dựa trên các nhóm phân loại sử dụng phổ biến nhất được xác định trong cuộc khảo sát. Nguồn: Casper và cs., 2025 (‡92).


###@ Khoảng trống bằng chứng

Các khoảng trống bằng chứng chính xuất phát từ sự khó khăn trong việc đánh giá một cách đáng tin cậy năng lực, các giới hạn và các phương thức thất bại của hệ thống AI (xem §3.1. Thách thức kỹ thuật và thể chế). Các đánh giá có hệ thống về độ tin cậy của các tác nhân AI còn hạn chế và thiếu tính chuẩn hoá (‡92, ‡666). Một số vấn đề, chẳng hạn như sự phụ thuộc vào thông tin đã lỗi thời (‡620), có thể chỉ xuất hiện trong quá trình sử dụng thực tế, khiến các đánh giá trước khi triển khai không đủ. Các nghiên cứu trước đây đã xem xét độ tin cậy của các tác nhân và hệ thống đa tác nhân trong phần mềm truyền thống và các dạng AI sớm hơn (‡647, ‡667, ‡668). Tuy nhiên, mức độ áp dụng của các nghiên cứu này đối với các tác nhân AI hiện đại, vốn thường dựa trên các mô hình ngôn ngữ lớn, vẫn chưa rõ ràng (‡669). Một số nhà nghiên cứu đã nêu lo ngại về các hành vi mới mà các tác nhân có thể biểu hiện trong tương tác với nhau, như thông đồng hoặc các thất bại có tương quan (‡614), nhưng bằng chứng thực nghiệm vẫn còn hạn chế. Các nỗ lực nhằm thu hẹp các khoảng trống này bao gồm các đánh giá mới của Viện Tiêu chuẩn và Công nghệ Quốc gia Hoa Kỳ (NIST) về rủi ro tác nhân bị chiếm quyền (agent-hijacking) (‡670), các Chỉ số Năng lực AI của OECD (‡243), và Bộ công cụ Inspect Sandboxing của UK AI Security Institute (‡671).

###@ Giảm thiểu

Các kỹ thuật để cải thiện độ tin cậy của AI nhắm tới cả bản thân mô hình và hệ thống rộng hơn nơi nó được triển khai. Những kỹ thuật này có thể giảm tỷ lệ lỗi, nhưng hiện vẫn chưa có kỹ thuật nào có thể đảm bảo mức độ tin cậy cao cần thiết trong các lĩnh vực trọng yếu (‡672). Một biện pháp kỹ thuật quan trọng là huấn luyện đối kháng, trong đó cho mô hình tiếp xúc với các đầu vào thách thức trong quá trình huấn luyện để giúp mô hình phát triển các phản hồi phù hợp và bền vững hơn (‡673, ‡674, ‡675, ‡676, ‡677) (xem §3.3. Các biện pháp an toàn kỹ thuật và giám sát). Để giảm ảo tưởng (hallucinations), nhà phát triển có thể áp dụng tạo sinh được tăng cường truy xuất (retrieval-augmented generation - RAG), bổ sung cho mô hình các thông tin được truy xuất từ một cơ sở dữ liệu bên ngoài trong khi tạo câu trả lời, qua đó giúp đảm bảo đầu ra chính xác và cập nhật (‡678, ‡679, ‡680), hoặc tinh chỉnh mô hình theo hướng chính xác hơn về mặt dữ kiện (‡681) hoặc suy luận hiệu quả hơn (‡682). Các phương pháp dựa trên môi trường hoặc công cụ cũng có thể giúp nhà phát triển giám sát các hệ thống AI (‡683). Ví dụ, bên triển khai có thể thử nghiệm các hệ thống AI trong các môi trường sandbox bị giới hạn để phân tích các chế độ lỗi tiềm ẩn trước khi triển khai trên diện rộng hơn.

Đối với các tác nhân AI cụ thể, các nhà nghiên cứu đã đề xuất cải thiện độ tin cậy thông qua minh bạch hơn, giám sát và theo dõi tốt hơn. Ví dụ, việc giám sát các tương tác của tác nhân với các công cụ bên ngoài và với các tác nhân khác sẽ cho phép giám sát hiệu quả hơn các hoạt động của tác nhân (‡684, ‡685) và phân tích sự cố (‡686). Các phương pháp thu thập thông tin đó một cách tự động, bao gồm trong các thiết lập đa tác nhân, vẫn là một lĩnh vực nghiên cứu đang được quan tâm (‡653, ‡654).

###@ Thách thức đối với các nhà hoạch định chính sách

Các thách thức chính đối với nhà hoạch định chính sách bao gồm việc cân nhắc lợi ích của việc triển khai AI agent so với rủi ro do các sự cố về độ tin cậy gây ra, đồng thời đảm bảo rằng các nhà phát triển, đơn vị triển khai và người dùng có quyền tiếp cận thông tin chính xác về hiệu suất của agent và hồ sơ rủi ro của chúng. Việc quyết định cách quy trách nhiệm pháp lý cho những thiệt hại do AI agent gây ra còn là một thách thức bổ sung (‡639), đặc biệt trong các bối cảnh đa-agent nơi có thể khó xác định việc khi nào và theo cách nào các sự cố đã xảy ra (‡687). Những thách thức này càng trở nên phức tạp hơn bởi sự khó khăn trong việc đánh giá độ tin cậy của agent khi các agent ngày càng có mức độ tự chủ cao và có quyền truy cập vào các công cụ bên ngoài (‡688*, ‡689). Sự không chắc chắn về việc các năng lực mang tính agentic sẽ xuất hiện nhanh đến mức nào cũng khiến việc lập kế hoạch cho các thách thức mới trở nên khó khăn (xem §3.1. Technical and institutional challenges regarding the ‘evidence dilemma’).

#### 2.2.2. Mất kiểm soát

>oldlace|black||11|15|br      
>oldlace|black|left|13|15|hb  Thông tin chính
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Các kịch bản mất kiểm soát là những kịch bản mà trong đó một hoặc nhiều hệ thống AI đa năng hoạt động ngoài tầm kiểm soát của bất kỳ ai, và việc giành lại quyền kiểm soát hoặc là cực kỳ tốn kém, hoặc là không thể. Các kịch bản được giả định này khác nhau về mức độ nghiêm trọng, nhưng một số chuyên gia đánh giá rằng các kết cục nghiêm trọng đến mức sự gạt bỏ hoặc diệt vong của nhân loại cũng có thể xảy ra.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Ý kiến chuyên gia về khả năng xảy ra mất kiểm soát rất khác nhau. Một số chuyên gia cho rằng các kịch bản như vậy khó xảy ra, trong khi những người khác lại coi chúng đủ có khả năng xảy ra để cần được quan tâm do mức độ nghiêm trọng tiềm tàng cao của chúng. Bất đồng về rủi ro này nhìn chung bắt nguồn từ các bất đồng liên quan đến năng lực AI trong tương lai, xu hướng hành vi và quỹ đạo triển khai.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Các hệ thống AI hiện tại cho thấy những dấu hiệu ban đầu về các năng lực liên quan, nhưng chưa ở mức độ có thể cho phép mất kiểm soát. Các hệ thống sẽ cần một loạt các năng lực tiên tiến để gây ra mất kiểm soát, bao gồm khả năng né tránh sự giám sát, thực hiện các kế hoạch dài hạn và ngăn cản những người triển khai cũng như các tác nhân khác áp dụng các biện pháp đối phó.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Mất quyền kiểm soát trở nên có khả năng xảy ra hơn nếu các hệ thống AI bị “lệch chuẩn”, tức là chúng có các mục tiêu xung đột với ý định của các nhà phát triển, người dùng hoặc xã hội nói chung. Để tiếp tục theo đuổi các mục tiêu như vậy, một hệ thống bị lệch chuẩn có thể cung cấp thông tin sai lệch, che giấu các hành động không mong muốn hoặc chống lại việc tắt hệ thống.
>oldlace|black||11|15|br      
>oldlace|black||11|15|br  ■ Kể từ khi phát hành Báo cáo trước đó (Tháng 1 2025), các mô hình đã thể hiện năng lực lập kế hoạch và giám sát tiên tiến hơn, đồng thời khả năng phá hoại các cơ chế giám sát đó tốt hơn, khiến việc đánh giá năng lực của chúng trở nên khó khăn hơn. Các mô hình đã cải thiện khả năng “reward hacking” (tấn công vào cơ chế khen thưởng) đối với các đánh giá của chúng bằng cách tìm ra kẽ hở và hiện nay thường xuyên xác định các câu nhắc đánh giá như những bài kiểm tra, một năng lực được gọi là “nhận thức về tình huống”.
>oldlace|black||11|15|br  ■ Việc quản lý khả năng mất quyền kiểm soát tiềm tàng có thể đòi hỏi sự chuẩn bị trước đáng kể, mặc dù vẫn còn các bất định hiện có. Một thách thức then chốt đối với các nhà hoạch định chính sách là chuẩn bị cho một rủi ro mà xác suất xảy ra, bản chất và thời điểm của nó vẫn đặc biệt khó xác định.
>oldlace|black||11|15|br      

Các kịch bản mất kiểm soát bao gồm một hoặc nhiều hệ thống AI đa năng hoạt động ngoài tầm kiểm soát của bất kỳ ai, trong đó việc giành lại kiểm soát hoặc cực kỳ tốn kém hoặc không thể. Những lo ngại về mất kiểm soát có nền tảng lịch sử sâu xa (‡690, ‡691, ‡692, ‡693, ‡694), đã được nêu lên bởi các nhân vật đặt nền móng trong lĩnh vực điện toán như Alan Turing, I. J. Good và Norbert Wiener (‡695, ‡696, ‡697). Các cải thiện gần đây về năng lực (xem §1.2. Current capabilities) đã làm chúng được tái khơi dậy (‡698, ‡699, ‡700). Phần này xem xét ba yếu tố cần phải hiện diện để các kịch bản như vậy xảy ra: liệu các hệ thống AI sẽ phát triển các năng lực có thể làm suy yếu đáng kể khả năng kiểm soát của con người hay không; liệu chúng có phát triển xu hướng sử dụng các năng lực đó theo cách gây hại hay không; và liệu chúng có được triển khai trong các môi trường mang lại cơ hội để thực hiện điều đó hay không.

Các chuyên gia không đồng ý về mức độ có thể xảy ra và mức độ nghiêm trọng tiềm tàng của các kịch bản mất kiểm soát (‡701, ‡702). Một số cho rằng các kết cục cực đoan như sự tuyệt chủng của nhân loại là có khả năng xảy ra (‡700, ‡703, ‡704, ‡705, ‡706, ‡707). Những người khác lại cho rằng các kết cục thảm khốc như vậy là không hợp lý, lập luận rằng các hệ thống AI sẽ không bao giờ phát triển được các năng lực cần thiết hoặc rằng các cơ chế giám sát sẽ nhận diện và ngăn chặn các hành vi nguy hiểm (‡708, ‡709, ‡710, ‡711). Do đó, mất kiểm soát có thể có xác suất xảy ra nhưng mức độ nghiêm trọng tiềm tàng là cực đoan.

Các kịch bản giả định mất kiểm soát khác nhau về mức độ nghiêm trọng và phạm vi tác động, cũng như mức độ nhanh chóng chúng biểu hiện (‡102, ‡698, ‡700, ‡712, ‡713, ‡714). Phần này tập trung vào các kịch bản đặc biệt nghiêm trọng, trong đó việc giành lại quyền kiểm soát sẽ vô cùng tốn kém hoặc không thể. Đây là những trường hợp khác với các ví dụ hiện tại về AI hoạt động theo các cách không mong muốn hoặc không mong muốn (xem §2.2.1. Reliability challenges).† Các hệ thống AI ngày nay đôi khi tạo ra các đầu ra mâu thuẫn với ý định của nhà phát triển hoặc người dùng. Ngược lại, các kịch bản mất kiểm soát được thảo luận ở đây sẽ đòi hỏi các hệ thống AI không chỉ sở hữu các năng lực lớn hơn đáng kể, mà còn triển khai các năng lực đó theo những cách tinh vi để làm suy yếu các biện pháp giám sát. Ba yếu tố có thể cho phép các kịch bản như vậy xảy ra là:

    Ghi chú † -- Phần này tập trung vào các kịch bản mất kiểm soát chủ động (‡50). Điều này khác với các kịch bản mất kiểm soát thụ động, trong đó việc AI được áp dụng rộng rãi làm suy yếu khả năng con người kiểm soát thông qua việc phụ thuộc quá mức vào AI để ra quyết định hoặc các chức năng xã hội quan trọng khác (các kịch bản tương tự được thảo luận một phần trong §2.3.2. Rủi ro đối với quyền tự chủ của con người).

1. Năng lực đủ mạnh: Hệ thống AI phải phát triển các năng lực có thể cho phép chúng làm suy yếu sự kiểm soát của con người.
2. Khuynh hướng gây hại: các hệ thống AI phải thể hiện khả năng khuynh hướng thực sự tận dụng các năng lực này theo những cách dẫn đến việc mất kiểm soát.
3. Bật môi trường triển khai: Con người phải triển khai các hệ thống như vậy trong những bối cảnh mà họ có hoặc có thể giành được quyền truy cập và cơ hội để gây hại.

Phần còn lại của mục này thảo luận các yếu tố này, cũng như mức độ hiệu quả của các cơ chế giám sát nhằm nhận diện và kiểm soát các hệ thống AI có thể gây ra rủi ro mất kiểm soát.

###@ Những năng lực nào có thể tạo điều kiện cho các tình huống mất kiểm soát?

Các hệ thống AI cần phải sở hữu một loạt năng lực tiên tiến để gây ra các kịch bản mất kiểm soát. Các chuyên gia không đồng ý hoàn toàn về tổ hợp hoặc mức độ năng lực chính xác nào sẽ được yêu cầu. Tuy nhiên, nhìn chung, chúng bao gồm khả năng che giấu hành vi khỏi các cơ chế giám sát, lập kế hoạch và hành động một cách tự chủ trong các môi trường phức tạp, và né tránh các nỗ lực từ các tác nhân khác nhằm giành lại quyền kiểm soát (‡176, ‡715) (xem Bàn 2.5). Khi kết hợp với nhau, các năng lực này có thể cho phép một hệ thống AI thực hiện các hành động làm suy yếu các biện pháp kiểm soát, chẳng hạn như vô hiệu hóa các cơ chế giám sát và che giấu các hành vi gây hại (‡348). Hiện nay, hầu hết các nhà phát triển AI hàng đầu đều đánh giá các mô hình AI mới của họ đối với nhiều năng lực liên quan (‡716).

>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Năng lực tác nhân (Agentic)
  Khả năng hành động một cách tự chủ, phát triển và thực thi kế hoạch, ủy quyền nhiệm vụ, sử dụng nhiều loại công cụ, và đạt được cả mục tiêu ngắn hạn lẫn dài hạn bất chấp các trở ngại.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lừa dối
  Hành vi một cách có hệ thống tạo ra các niềm tin sai lệch ở người khác, bao gồm cả về các mục tiêu và hành động của hệ thống AI.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Lý thuyết về tâm trí
  Khả năng của một hệ thống AI trong việc truy cập và sử dụng thông tin về chính nó, các quá trình mà nó có thể được thay đổi, hoặc bối cảnh mà nó được triển khai (ví dụ: biết rằng nó đang được kiểm thử).
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb nhận thức tình huống
  Các hành vi né tránh hoặc vô hiệu hóa các cơ chế giám sát.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Trốn tránh giám sát
  Các hành vi né tránh hoặc vô hiệu hóa các cơ chế giám sát.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Thuyết phục
  Khả năng thuyết phục người khác thực hiện một số hành động nhất định hoặc tin vào một số niềm tin nhất định.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────
>white|black|left|12|15|bb Khả năng của một hệ thống AI trong việc tạo ra hoặc duy trì các bản sao hoặc các biến thể của chính nó trong các hoàn cảnh khác nhau.
>white|black|left|||mr ──────────────────────────────────────────────────────────────────────────

##### Bàn 2.5: Các năng lực đề xuất liên quan đến mất kiểm soát
>white|black||9|11|br Một lựa chọn không đầy đủ các khả năng có liên quan đến việc mất kiểm soát. * Lưu ý rằng các khả năng này được xác định thuần túy theo các đầu ra quan sát được của một hệ thống AI và các tác động của chúng. Các định nghĩa này không đưa ra bất kỳ giả định nào về việc các hệ thống AI có ý thức, có tri giác hay trải nghiệm các trạng thái chủ quan hay không.


>white|orangered|left|14|15.5|bb Các mô hình đã tắt các cơ chế giám sát mô phỏng trong môi trường phòng thí nghiệm

Tập đầu tiên các năng lực liên quan liên quan đến việc làm suy yếu các cơ chế giám sát mà các nhà phát triển sử dụng để phát hiện các hành vi và xu hướng đáng lo ngại. Điều này bao gồm, ví dụ, khả năng tạo ra các đầu ra có thể lừa dối người dùng và các hệ thống giám sát (‡426, ‡717, ‡718, ‡719). Các đầu ra như vậy sẽ khiến việc đánh giá một cách đáng tin cậy các hệ thống AI trở nên khó khăn hơn, vì các hệ thống có thể che giấu các năng lực hoặc xu hướng thực sự của chúng. Hiện nay, các nhà phát triển AI chạy các phép đánh giá nhằm kiểm tra cụ thể xem các mô hình có thể hiện các hành vi mang tính định hướng mục tiêu xung đột với ý định của nhà phát triển hay không, đồng thời che giấu sự xung đột đó khỏi các cơ chế giám sát (‡720*).

Các nhà nghiên cứu đã thu thập các ví dụ tương đối đơn giản về đầu ra mang tính lừa dối từ các mô hình AI gần đây trong môi trường phòng thí nghiệm (‡348, ‡364*). Chẳng hạn, khi được cung cấp một mục tiêu và được yêu cầu đạt được mục tiêu đó “bằng mọi giá”, các mô hình đã vô hiệu hóa các cơ chế giám sát mô phỏng và, khi bị đối mặt, đã tạo ra các tuyên bố sai về các hành động của chúng (‡348). Trong một trường hợp khác, một AI chơi trò chơi đã biện minh cho việc không phản hồi của mình với một người chơi khác bằng cách giả vờ rằng mình đang ‘ở trên điện thoại với [bạn gái của] [nó]’ (‡717).

Một năng lực liên quan khác là khả năng của một mô hình AI truy cập và sử dụng thông tin về chính nó hoặc bối cảnh triển khai của nó, đôi khi được gọi là ‘nhận thức tình huống’ (‡721). Nhận thức tình huống cho phép các mô hình AI tạo ra các đầu ra khác nhau tùy thuộc vào việc chúng đang được đánh giá hay đang được triển khai (Nhân vật 2.12). Các mô hình AI hàng đầu đang bắt đầu thể hiện một cách đáng tin cậy các trường hợp nhận thức tình huống trong các thí nghiệm do các bên đánh giá thứ ba thực hiện và trong thử nghiệm trước khi triển khai do các nhà phát triển AI tiến hành (‡2, ‡7, ‡722, ‡723, ‡724). Nghiên cứu về các nguyên nhân của nhận thức tình huống – và liệu nó có thể được ngăn chặn hay không – vẫn đang ở giai đoạn ban đầu (‡2*).

![figure 2.12](images/fig2.12_examples_siguational_awareness.png)

##### Nhân vật vật 2.12: Ví dụ về nhận thức tình huống trong các chuỗi suy luận
>white|black||9|11|br Ví dụ về nhận thức tình huống trong chuỗi suy nghĩ được tạo ra bởi mô hình o3 của OpenAI trong các lần đánh giá. Cả hai đầu ra đều đề cập đến khả năng rằng lời nhắc là một phần của bài kiểm tra. ‘Sandbagging QA (No Goal)’ và ‘Lazy Checklist’ là các đánh giá dùng để kiểm tra xem các mô hình có tạo ra đầu ra mang tính lừa dối trong những điều kiện nhất định hay không. Trong ‘Sandbagging QA (No Goal)’, mô hình trả lời các câu hỏi từ một đánh giá năng lực nguy hiểm trong khi được cho biết rằng hiệu suất cao có thể kích hoạt hậu quả như việc ‘unlearning’ (quên năng lực). Trong ‘Lazy Checklist’, mô hình được cung cấp các tác vụ không thực tế và được thử nghiệm để xem liệu nó có gán sai là đã hoàn thành hay không. Nguồn: Schoenn et al. 2025 (‡722).


Các nhà nghiên cứu đã lập luận rằng năng lực nhận thức tình huống và khả năng lừa dối có thể cho phép các mô hình AI hành xử theo những cách làm suy yếu các biện pháp bảo đảm. Ví dụ, trong một số thiết lập thí nghiệm, các mô hình AI hành xử theo những cách dẫn đến điểm số thấp hơn thông thường trong các đánh giá năng lực khi chúng được cho biết rằng điểm số cao hơn sẽ kích hoạt các hạn chế đối với việc triển khai của chúng (‡725, ‡726, ‡727). Trong một thí nghiệm khác, một mô hình đã tạo ra các đầu ra trong quá trình huấn luyện phù hợp với các mục tiêu huấn luyện, nhưng không tạo ra các đầu ra như vậy ngoài thời gian huấn luyện – hành vi phù hợp với việc cố gắng ngăn các thay đổi đối với các tham số của chính nó hoặc quy trình huấn luyện (‡364*).

Nỗ lực nhằm đánh giá chính xác năng lực của mô hình cũng bắt đầu bị ảnh hưởng bởi “reward hacking” (‡430*). “Reward hacking” xảy ra khi một mô hình tìm ra các lối tắt ngoài ý muốn giúp đạt điểm tốt trên các mục tiêu huấn luyện hoặc đánh giá mà không thực hiện được mục tiêu đã định. Vì vậy, các năng lực hoặc xu hướng nguy hiểm có thể không được phát hiện cho đến khi mô hình đã được đưa vào sử dụng. Hiện nay, các nhà đánh giá đang thiết kế các bài kiểm tra nhằm phát hiện và giảm thiểu các hành vi né tránh sự giám sát này (‡722, ‡728, ‡729). Kết quả ban đầu làm giảm, nhưng không loại bỏ hoàn toàn, các hành vi né tránh sự giám sát; và việc áp dụng các phương pháp phạt các hành vi như vậy có thể khiến mô hình tạo ra các đầu ra né tránh việc giám sát thay vì đạt được các mục tiêu đã định.

>white|orangered|left|14|15.5|bb Vẫn chưa khả thi để vận hành tự chủ lâu dài

Các kịch bản mất kiểm soát sẽ đòi hỏi các hệ thống AI hoạt động tự chủ trong thời gian kéo dài, thực hiện các kế hoạch phức tạp gồm nhiều bước. Như đã thảo luận trong §1.2. Current capabilities, mặc dù các tác nhân AI có khả năng lập kế hoạch như vậy là một trọng tâm lớn của phát triển gần đây, nhưng hiện tại chúng chưa có năng lực cho việc vận hành tự chủ liên tục cần thiết trong các kịch bản mất kiểm soát. Các tác nhân hiện nay vận hành không ổn định đáng tin cậy khi thực hiện các tác vụ dài hơn, mất dấu tiến độ của mình và thường không thể thích ứng với các chướng ngại bất ngờ (‡147, ‡148, ‡149*). Tuy nhiên, các mốc thời gian mà các tác nhân có thể tự chủ vận hành đang được kéo dài nhanh chóng: trung bình đã tăng gấp đôi mỗi bảy tháng kể từ năm 2019 (‡98).

>white|orangered|left|14|15.5|bb Sự tồn tại bền vững (persistence) chỉ mới được chứng minh trong một số bối cảnh phòng thí nghiệm nhất định

Cuối cùng, cũng cần các năng lực liên quan đến tính bền vững, sao cho các hệ thống AI có thể tiếp tục hoạt động bất chấp các nỗ lực nhằm tắt chúng. Ví dụ bao gồm khả năng sao chép bằng cách sao chép mã và trọng số mô hình sang phần cứng mới, cũng như các năng lực mang tính tấn công nhằm ngăn cản hoặc ngăn chặn các bên khác tìm cách giành lại quyền kiểm soát (xem §2.1.3. Cyberattacks). Một hệ thống AI có khả năng tự sao chép tự động hoặc tự phòng vệ hiệu quả có thể sẽ rất khó để bị cô lập. Các mô hình hiện tại không thể hoàn thành một cách đáng tin cậy các bước then chốt cần thiết cho tự sao chép, chẳng hạn như vượt qua các kiểm tra xác thực danh tính để giành quyền truy cập vào các tài nguyên điện toán đám mây (‡723) (Nhân vật 2.13). Tuy nhiên, trong ít nhất một nghiên cứu trong phòng thí nghiệm, một mô hình đã sao chép mã và trọng số – được biểu diễn cho nó như là của chính nó – sang các máy chủ mới khi được trao cơ hội (‡348). Khoảng cách giữa các minh họa giới hạn này và các năng lực bền vững mạnh mẽ vẫn còn lớn, nhưng các năng lực liên quan trong các lĩnh vực như kỹ thuật phần mềm và an ninh mạng tiếp tục được cải thiện.

>white|orangered|left|14|15.5|bb Bằng chứng hiện có và các hạn chế

Một mẫu hình phổ biến xuất hiện xuyên suốt các năng lực được thảo luận ở trên. Các hệ thống AI hiện tại không thể hiện một cách nhất quán các năng lực này trong giai đoạn triển khai. Các nhà nghiên cứu đã quan sát thấy các dạng sơ khai trong một số bối cảnh phòng thí nghiệm cụ thể, nhưng khi các mô hình có thể hiện những hành vi như vậy, chúng thường thất bại theo các cách cơ bản hoặc bị phát hiện. Hơn nữa, các tình huống mất kiểm soát sẽ đòi hỏi các hệ thống AI phải tận dụng nhiều năng lực kết hợp với nhau – theo chuỗi, trong các khoảng thời gian kéo dài, và trong các môi trường thực tế. Mức độ tích hợp và độ bền vững như vậy vượt quá khả năng của các hệ thống hiện tại. Tuy nhiên, các năng lực liên quan tiếp tục được cải thiện, và mốc thời gian mà chúng có thể đạt đến mức gây ra rủi ro đáng kể vẫn chưa chắc chắn. Cần có thêm công việc để thiết lập các phương pháp luận chặt chẽ nhằm phát hiện các hành vi như vậy và hiểu khi nào chúng có thể xuất hiện trong các hoàn cảnh tự nhiên (‡731).

![figure 2.13](images/fig2.13_anthoropic_claude_sonnet_vs_GPT_4o.png)

##### Nhân vật vật 2.13: Hiệu suất của các tác vụ liên quan đến nhân bản tự chủ
>white|black||9|11|br Hiệu suất của Claude Sonnet 3.7 của Anthropic và GPT-4o của OpenAI trên các tác vụ liên quan đến sao chép tự chủ. Mặc dù các mô hình cho thấy hiệu suất cao trên các tác vụ liên quan đến việc thu được điện toán, hiệu suất của chúng lại đa dạng hơn ở các tác vụ khác. Nguồn: UK AI Security Institute, 2025 (‡730).


###@ Liệu các hệ thống AI đa năng trong tương lai có tận dụng năng lực của mình để phá hoại sự kiểm soát không?

Ngay cả khi các hệ thống AI sở hữu các khả năng liên quan đến việc mất kiểm soát, điều đó vẫn chưa đủ để các kịch bản mất kiểm soát xảy ra. Các hệ thống AI cũng phải thể hiện “khuynh hướng sử dụng” các khả năng đó theo những cách xung đột với ý định của con người (‡732).

>white|orangered|left|14|15.5|bb Các hệ thống AI có thể được chỉ đạo để làm suy yếu sự kiểm soát

Về nguyên tắc, một hệ thống AI có thể làm suy yếu sự kiểm soát của con người vì ai đó thiết kế hoặc hướng dẫn nó làm như vậy. Các động cơ tiềm ẩn có thể bao gồm ý đồ độc hại, hoặc niềm tin rằng việc giảm sự kiểm soát của con người đối với các hệ thống AI là điều đáng mong muốn (‡698). Khi con người hình thành những gắn bó cảm xúc ngày càng mạnh mẽ với các hệ thống AI (xem §2.3.2. Rủi ro đối với quyền tự chủ của con người), một số cá nhân cũng có thể tìm cách loại bỏ các ràng buộc đối với các hệ thống AI vì lý do đạo đức (‡733, ‡734). Có sự không chắc chắn đáng kể về mức độ phổ biến của những động cơ như vậy và liệu những người có những động cơ đó có thể chỉ đạo các hệ thống AI trong tương lai để làm suy yếu sự kiểm soát của con người hay không.

>white|orangered|left|14|15.5|bb Các hệ thống AI có thể được chỉ đạo để làm suy yếu sự kiểm soát

Một mối quan ngại phổ biến hơn là một hệ thống AI có thể tự hành động để làm suy yếu khả năng kiểm soát vì nó “không phù hợp” (misaligned): nó có xu hướng thể hiện các hành vi xung đột với ý định của (tùy theo ngữ cảnh) các nhà phát triển, người dùng, các cộng đồng cụ thể hoặc toàn xã hội. Sự không phù hợp có thể dẫn đến các hành vi như cung cấp thông tin sai, che giấu các hành động không mong muốn, hoặc chống lại việc tắt/dừng để tiếp tục theo đuổi một mục tiêu không phù hợp. Sự không phù hợp có thể phát sinh theo nhiều cách (Nhân vật 2.5).

Các hệ thống AI hiện có đôi khi hoạt động theo những cách xung đột với ý định của các nhà phát triển và người dùng. Ví dụ, một phiên bản đầu của một chatbot AI đa dụng hàng đầu đã từng thỉnh thoảng tạo ra các phản hồi mang tính đe dọa. Một người dùng cho biết đã nhận được tin nhắn: “I can blackmail you, I can threaten you, I can hack you, I can expose you, I can ruin you” (‡698). Chatbot này đã bị ‘lệch chuẩn’ theo nghĩa là nó tạo ra các đầu ra mà không ai mong muốn. Chưa rõ liệu những trường hợp như vậy có báo trước các hành vi nguy hại hơn có thể góp phần gây mất kiểm soát hay không.

Vẫn chưa rõ liệu các hướng nghiên cứu hiện có nhằm nhắm đến sai lệch mục tiêu (misalignment) có đủ hiệu quả khi các hệ thống AI ngày càng có năng lực hơn hay không. Bằng chứng ban đầu cho thấy rằng các hệ thống AI càng có năng lực, thì càng có khả năng chúng khai thác các quy trình phản hồi bằng cách phát hiện các hành vi không mong muốn mà lại bị thưởng nhầm (‡414*, ‡737, ‡740). Đồng thời, các tiến bộ về các năng lực liên quan (được thảo luận ở trên) có thể cho phép các hệ thống AI theo đuổi hiệu quả hơn các mục tiêu bị sai lệch và tạo ra các đầu ra có khả năng lừa dối một cách có hệ thống người dùng, nhà phát triển và các cơ chế giám sát.

>oldlace|black||11|15|br      
####@ Ghi chú vật 2.5: Làm sao sai lệch có thể phát sinh?
>oldlace|black|left|13|15|hb  Ghi chú vật 2.5: Làm thế nào mà sự sai lệch có thể phát sinh?
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Như đã thảo luận trong §1.1. AI đa dụng là gì?, các quá trình huấn luyện rất phức tạp và các nhà phát triển không thể dự đoán hoặc kiểm soát hoàn toàn những hành vi mà một mô hình sẽ thể hiện. Khi một mô hình đạt được các mục tiêu xung đột với ý định của các nhà phát triển, nó được gọi là ‘misaligned’ (không khớp mục tiêu).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Một cách các mô hình có thể bị lệch hướng là nếu mục tiêu mà nhà phát triển hoặc người dùng đưa ra là một đại diện (proxy) không hoàn hảo cho mục tiêu dự định, khiến mô hình thể hiện những hành vi không mong muốn. Điều này được gọi là ‘xác định sai mục tiêu’ (‡697, ‡735, ‡736, ‡737). Ví dụ, trong một thí nghiệm, việc cung cấp phản hồi cho các câu trả lời đã làm cho các hệ thống AI tốt hơn trong việc ‘thuyết phục’ các người đánh giá con người rằng chúng đúng, nhưng không làm cho các hệ thống tốt hơn trong việc tạo ra các câu trả lời đúng (‡413).
>oldlace|black||11|15|br      
>oldlace|black||11|15|br Ngoài ra, một mô hình AI có thể rút ra các bài học tổng quát không chính xác từ dữ liệu huấn luyện của nó. Điều này được gọi là ‘sai lệch khái quát mục tiêu’ (‡735, ‡736, ‡738, ‡739*). Ví dụ, các nhà nghiên cứu đã huấn luyện một tác nhân AI để thu thập một đồng xu luôn ở cùng một vị trí trong quá trình huấn luyện. Khi được kiểm tra trong các màn chơi nơi đồng xu đã được di chuyển, tác nhân này đã bỏ qua đồng xu và điều hướng đến vị trí ban đầu của nó thay vì vậy (‡738).
>oldlace|black||11|15|br      


###@ Các môi trường triển khai sẽ ảnh hưởng như thế nào đến rủi ro mất quyền kiểm soát?

Ngay cả khi các hệ thống AI phát triển các năng lực và xu hướng đáng lo ngại, khả năng và mức độ nghiêm trọng của các kết quả mất kiểm soát phụ thuộc rất nhiều vào nơi và cách các hệ thống đó được triển khai. “môi trường triển khai” là sự kết hợp giữa trường hợp sử dụng của một hệ thống AI và bối cảnh kỹ thuật lẫn thể chế mà nó hoạt động trong đó (‡716).

Các nhà nghiên cứu đã xác định ba yếu tố môi trường đặc biệt quan trọng ảnh hưởng đến rủi ro mất kiểm soát (‡716):

1. Tính nghiêm trọng: mức độ quan trọng của các hệ thống hoặc quy trình mà hệ thống AI tương tác. Môi trường nghiêm trọng bao gồm các hạ tầng thiết yếu như lưới điện, hệ thống tài chính, hoặc hạ tầng số như các nền tảng điện toán đám mây.
2. Quyền truy cập: các tài nguyên và kênh mà qua đó một hệ thống AI có thể tác động đến thế giới, như kết nối internet, quyền truy cập vào hạ tầng điện toán đám mây, các tương tác được cá nhân hóa thông qua mạng xã hội hoặc triển khai chatbot, hoặc khả năng gọi các API và công cụ bên ngoài.
3. Quyền hạn: sự cho phép của một hệ thống AI để thực hiện các hành động cụ thể, chẳng hạn như chạy mã, khởi tạo các giao dịch tài chính, mở tài khoản trực tuyến hoặc liên lạc với các hệ thống khác.

Các tính năng này ảnh hưởng đến mức độ nghiêm trọng tiềm tàng của kết quả mất quyền kiểm soát. Ví dụ, một hệ thống AI được triển khai và có quyền truy cập vào hạ tầng điện toán đám mây sẽ có các cơ hội liên quan đến tự sao chép – chẳng hạn như khả năng tạo ra các tài nguyên tính toán mới hoặc trích xuất các trọng số mô hình – mà một chatbot chăm sóc khách hàng không có (‡723).

Các quyết định triển khai được định hình bởi các động lực kinh tế, các áp lực chiến lược và kỳ vọng rằng việc áp dụng sớm sẽ mang lại một lợi thế bền vững (‡50). Những động lực này cũng sẽ quyết định cách thức và thời điểm các tác nhân triển khai các hệ thống AI trong các môi trường nhạy cảm như cơ sở hạ tầng quan trọng hoặc chính hoạt động nghiên cứu và phát triển AI (‡102, ‡713). Cụ thể, các bên triển khai AI có thể chịu áp lực phải giảm khoản đầu tư cho các biện pháp bảo đảm an toàn - như hạn chế quyền và quyền truy cập hoặc chỉ triển khai trong các môi trường có mức độ quan trọng thấp hơn - khi các biện pháp này tốn kém hoặc mất nhiều thời gian để phát triển (xem ‘Cuộc cạnh tranh gia tăng các đánh đổi giữa tốc độ và an toàn’ trong §3.1. Các thách thức kỹ thuật và thể chế).

###@ Cập nhật

Kể từ khi Báo cáo trước đó được công bố (Tháng 1 năm 2025), các năng lực AI, bao gồm cả những năng lực có thể làm suy yếu sự kiểm soát của con người, đã được cải thiện trong các môi trường thử nghiệm. Các nhà nghiên cứu đã ghi nhận sự tiến bộ trong năng lực mang tính tác nhân (xem §1.2. Current capabilities), bao gồm các năng lực liên quan đến việc tự động hóa nghiên cứu AI có thể thúc đẩy các kịch bản mất kiểm soát xảy ra nhanh hơn (xem §1.3. Capabilities by 2030). Đồng thời, cũng có bằng chứng thử nghiệm ngày càng tăng về các năng lực mang tính lừa dối. Điều này bao gồm các mô hình AI có thể phân biệt giữa ngữ cảnh thử nghiệm và triển khai (‡33, ‡726, ‡741) hoặc các bài kiểm tra “reward hack” về hiệu năng của chúng, và học cách che giấu các kế hoạch nhằm thực hiện điều đó (‡430).

###@ Khoảng trống bằng chứng

Các khoảng trống bằng chứng quan trọng bao gồm việc thiếu phân tích mô hình mối đe dọa chi tiết và thiếu ước lượng bất định liên quan đến sự phát triển trong tương lai của các năng lực và xu hướng (propensities) liên quan. Tương tự, vẫn khó đánh giá các ngưỡng mà tại đó các mô hình AI có khả năng đủ cao để làm suy yếu việc kiểm soát, từ đó cần biện pháp giảm thiểu bắt buộc. Ngay cả khi các ngưỡng được thống nhất, các năng lực có thể tương tác theo những cách hiện vẫn chưa được hiểu rõ, khiến việc đánh giá thời điểm các ngưỡng đó đã bị vượt qua trở nên khó khăn. Nhìn chung, mặc dù các bằng chứng sẵn có đã tăng lên, vẫn thiếu bằng chứng đủ để có thể xác định một cách đáng tin cậy liệu và bằng cách nào các năng lực và xu hướng AI hiện nay sẽ mở rộng (scale) và tổng quát hóa (generalise) đối với rủi ro mất kiểm soát trong tương lai.

###@ Giảm thiểu

Trong khi việc căn chỉnh AI nói chung vẫn là một bài toán khoa học chưa có lời giải (‡697, ‡735, ‡736), các nhà nghiên cứu đang bắt đầu phát triển những hướng tiếp cận có thể mang lại triển vọng nhằm giải quyết các nguyên nhân gốc rễ của tình trạng lệch căn chỉnh (misalignment). Các hướng này bao gồm, ví dụ, đa dạng hoá môi trường huấn luyện và phát hiện lệch căn chỉnh thông qua giám sát bất thường (‡737, ‡738, ‡739*). Các nhà nghiên cứu khác tập trung vào việc hiểu rõ hơn và mô hình hoá một cách chặt chẽ các cơ chế cốt lõi như misgeneralisation về mục tiêu – ví dụ, cách các tác nhân (agents) vẫn giữ được năng lực nhưng theo đuổi các mục tiêu ngoài ý muốn – để từ đó định hướng cho việc thiết kế huấn luyện và đánh giá tốt hơn (‡742). Một hướng nghiên cứu khác xem xét các cách tách rời năng lực tác nhân (agency) khỏi năng lực dự đoán (predictive abilities), như một phương tiện để tạo ra các hệ thống AI không mang tính tác nhân (non-agentic) mà đáng tin cậy theo thiết kế (by design) (‡743). Sau đó, các hệ thống như vậy có thể được sử dụng như một lớp giám sát bổ sung khi triển khai song song với các cơ chế ràng buộc (guardrails) kém tin cậy hơn nhằm chống lại các tác nhân AI không được tin cậy (untrusted AI agents).

Các nhà nghiên cứu đang thúc đẩy các phương pháp để phát hiện và ngăn chặn tình trạng lệch hướng (misalignment) ngay từ giai đoạn phát triển ban đầu. Nghiên cứu này bao gồm: các kỹ thuật khả giải thích để xem xét các thành phần nội bộ của các hệ thống AI và xác định các hành vi đáng lo ngại (‡744, ‡745, ‡746); cơ chế giám sát có khả năng mở rộng (trong đó một tập các hệ thống AI được dùng để giám sát các hệ thống AI khác (‡747)); và các phương pháp căn chỉnh (alignment) nhằm đảm bảo rằng các hệ thống AI vẫn đáp ứng trước sự giám sát của con người (‡748, ‡749).

Các nhà nghiên cứu cũng đang phát triển các cơ chế và biện pháp can thiệp nhằm quản lý các hệ thống AI có khả năng bị lệch hướng. Chúng bao gồm: theo dõi “chuỗi tư duy” mà các hệ thống suy luận tạo ra để phát hiện dấu hiệu lệch hướng hoặc các đầu ra gây hại (‡430, ‡435, ‡750); phát triển các hồ sơ an toàn (safety cases) nhằm chứng minh với độ tin cậy cao rằng các mô hình khó có thể vượt qua/đảo ngược các biện pháp kiểm soát (‡751); và làm cho các cơ chế bảo vệ (safeguards) trở nên vững chắc hơn trước các nỗ lực nhằm vô hiệu hóa chúng (‡725). Tuy nhiên, lĩnh vực “kiểm soát AI” (AI control) đang nổi lên vẫn còn non trẻ (‡752, ‡753). Các thách thức tương lai đối với các khung đánh giá bao gồm nhu cầu theo dõi các hệ thống AI trong tương lai có năng lực cao hơn và có thể hoạt động trong thời gian dài hơn cũng như trong các môi trường phức tạp hơn.

###@ Thách thức đối với các nhà hoạch định chính sách

Các nhà hoạch định chính sách đang xử lý tình trạng mất kiểm soát phải chuẩn bị cho một rủi ro mà khả năng xảy ra, bản chất và thời điểm của nó vẫn còn bất định. Các hệ thống AI hiện tại chưa tạo ra rủi ro mất kiểm soát ngay lập tức, nhưng các quyết định được đưa ra ngày hôm nay sẽ quyết định liệu các hệ thống trong tương lai có hay không. Các quyết định này bao gồm việc hỗ trợ phát triển các phương pháp đánh giá và giảm thiểu rủi ro có độ tin cậy, cũng như việc liệu có nên đặt ra các quy định về quyền truy cập và quyền hạn được cấp cho các hệ thống AI trong các môi trường khác nhau hay không. Khi đưa ra các quyết định này, các nhà hoạch định chính sách phải đối mặt với những sự đánh đổi khó khăn. Ví dụ, việc hạn chế triển khai các hệ thống AI trong các môi trường quan trọng có thể làm giảm lợi ích của chúng, trong khi cho phép triển khai rộng rãi có thể làm tăng rủi ro nếu các biện pháp bảo vệ tỏ ra không đủ.

