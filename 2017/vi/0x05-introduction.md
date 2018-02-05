# Giới thiệu

## Chào mừng bạn đến với OWASP Top 10 - 2017

Bản cập nhật chính này bổ sung thêm một số vấn đề mới, bao gồm hai vấn đề được lựa chọn bởi cộng đồng - A8: 2017-Không an toàn Deserialization và A10: 2017-Không đầy đủ Đăng nhập và Giám sát. Hai điểm khác biệt chính của OWASP 10 bản phát hành trước đó là phản hồi cộng đồng đáng kể và dữ liệu rộng lớn được tập hợp từ hàng chục tổ chức, có thể là số lượng dữ liệu lớn nhất đã từng được lắp ráp trong việc chuẩn bị một tiêu chuẩn an ninh ứng dụng. Điều này cho phép chúng tôi tự tin rằng OWASP mới nhất 10 giải quyết các nguy cơ bảo mật ứng dụng hiệu quả nhất hiện đang đối mặt với các tổ chức.

OWASP Top 10 cho năm 2017 chủ yếu dựa trên 40 + dữ liệu đệ trình từ các công ty chuyên về ứng dụng an ninh và một cuộc khảo sát ngành công nghiệp đã được hoàn thành bởi hơn 500 cá nhân. Dữ liệu này mở rộng các lỗ hổng được tập hợp từ hàng trăm tổ chức và hơn 100.000 ứng dụng và API thực trên thế giới. 10 mục hàng đầu được lựa chọn và được ưu tiên theo dữ liệu tỷ lệ này, kết hợp với các ước tính đồng nhất về khả năng khai thác, khả năng phát hiện và tác động.

Mục tiêu chính của OWASP Top 10 là đào tạo các nhà phát triển, nhà thiết kế, kiến ​​trúc sư, nhà quản lý và tổ chức về những hậu quả của những điểm yếu an ninh ứng dụng web phổ biến và quan trọng nhất. Top 10 cung cấp các kỹ thuật cơ bản để bảo vệ chống lại các khu vực có nguy cơ cao, và cung cấp hướng dẫn về nơi để đi từ đây.

## Lộ trình cho các hoạt động trong tương lai

**Đừng dừng lại ở mức 10**. Có hàng trăm vấn đề có thể ảnh hưởng đến an ninh chung của một ứng dụng web như được thảo luận trong Hướng dẫn của [Nhà phát triển OWASP](https://www.owasp.org/index.php/OWASP_Guide_Project) và [OWASP Cheat Sheet Series]( https://www.owasp.org/index.php/Category:Cheatsheets). Đây là những bài đọc thiết yếu cho bất cứ ai phát triển ứng dụng web và API. Hướng dẫn về cách hiệu quả để tìm các lỗ hổng trong các ứng dụng web và các API được cung cấp trong [Hướng dẫn Thử nghiệm OWASP](https://www.owasp.org/index.php/OWASP_Testing_Project).

**Thay đổi liên tục**. OWASP Top 10 sẽ tiếp tục thay đổi. Ngay cả khi không thay đổi một dòng mã ứng dụng của bạn, bạn có thể trở nên dễ bị tổn thương vì những lỗ hổng mới được phát hiện và phương pháp tấn công được tinh chế. Vui lòng xem lại lời khuyên khi kết thúc Top 10 trong Tiếp theo của Nhà phát triển, Người kiểm tra, Tổ chức và Người quản lý ứng dụng để biết thêm thông tin.

**Suy nghĩ tích cực**. Khi bạn đã sẵn sàng để ngừng theo đuổi các lỗ hổng và tập trung vào việc thiết lập các kiểm soát an ninh ứng dụng mạnh mẽ, dự án [OWASP Proactive Controls](https://www.owasp.org/index.php/OWASP_Proactive_Controls) cung cấp điểm khởi đầu để giúp các nhà phát triển xây dựng bảo mật vào các ứng dụng của họ và [Tiêu chuẩn Xác minh An ninh Ứng dụng OWASP (ASVS)](https://www.owasp.org/index.php/ASVS) là hướng dẫn cho các tổ chức và người đánh giá ứng dụng về những gì để xác minh.

**Sử dụng công cụ một cách khôn ngoan**. Các lỗ hổng bảo mật có thể khá phức tạp và bị chôn sâu trong mã nguồn. Trong nhiều trường hợp, cách tiếp cận hiệu quả nhất để tìm và loại bỏ những điểm yếu này là các chuyên gia của con người được trang bị các công cụ tiên tiến. Dựa vào các công cụ đơn lẻ cung cấp một cảm giác sai về bảo mật và không được khuyến cáo.

**Nhấn trái, phải và ở mọi nơi**. Tập trung vào việc đảm bảo an ninh là một phần không thể thiếu trong văn hoá của bạn trong suốt tổ chức phát triển. Tìm hiểu thêm trong [Mô hình trưởng thành đảm bảo phần mềm OWASP (SAMM)](https://www.owasp.org/index.php/OWASP_SAMM_Project).

## Cấp cho

Chúng tôi muốn cảm ơn các tổ chức đã đóng góp dữ liệu dễ bị tổn thương của họ để hỗ trợ cập nhật năm 2017. Chúng tôi đã nhận được hơn 40 phản hồi đối với cuộc gọi dữ liệu. Lần đầu tiên, tất cả các dữ liệu đóng góp cho một phát hành Top 10, và danh sách đầy đủ của người đóng góp, được công bố công khai. Chúng tôi tin rằng đây là một trong những bộ sưu tập dữ liệu dễ bị tổn thương lớn hơn và đa dạng hơn từng được thu thập công khai.

Vì có nhiều đóng góp hơn là không gian ở đây nên chúng tôi đã tạo ra một trang dành riêng để công nhận đóng góp được thực hiện. Chúng tôi muốn gửi lời cảm ơn chân thành tới các tổ chức này vì sẵn sàng đi tiên phong bằng cách chia sẻ công khai những dữ liệu dễ bị tổn thương từ những nỗ lực của họ. Chúng tôi hy vọng điều này sẽ tiếp tục phát triển và khuyến khích các tổ chức khác làm như vậy và có thể được coi là một trong những mốc quan trọng của chứng cứ an ninh dựa trên bằng chứng. OWASP Top 10 sẽ không thể có nếu không có những đóng góp đáng kinh ngạc này.

Một cảm ơn lớn cho hơn 500 cá nhân đã dành thời gian để hoàn thành ngành công nghiệp khảo sát xếp hạng. Tiếng nói của bạn đã giúp xác định hai bổ sung mới cho Top 10. Các nhận xét bổ sung, ghi chú khuyến khích và phê bình đều được đánh giá cao. Chúng tôi biết thời gian của bạn rất quý giá và chúng tôi muốn nói cảm ơn.

Chúng tôi muốn cảm ơn những cá nhân đã đóng góp ý kiến ​​xây dựng quan trọng và thời gian xem lại cập nhật này lên Top 10. Chúng tôi đã liệt kê chúng trên trang "Lời Cảm ơn" càng nhiều càng tốt.

Và cuối cùng, chúng tôi muốn cảm ơn tất cả các dịch giả trước đây, những người sẽ dịch bản phát hành Top 10 này sang nhiều ngôn ngữ khác nhau, giúp làm cho OWASP Top 10 dễ tiếp cận hơn với toàn bộ hành tinh này.
