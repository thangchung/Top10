# RN Ghi chú Phát hành

## Điều gì đã thay đổi từ năm 2013 đến năm 2017?

Thay đổi đã tăng lên trong bốn năm qua, và OWASP Top 10 cần phải thay đổi. Chúng tôi đã tái cấu trúc lại OWASP Top 10, cải tiến phương pháp luận, sử dụng một quy trình gọi dữ liệu mới, làm việc với cộng đồng, sắp xếp lại các rủi ro của chúng tôi, viết lại từng rủi ro từ đầu và thêm các tham khảo đến các khuôn khổ và ngôn ngữ hiện đang được sử dụng rộng rãi.

Trong vài năm qua, công nghệ cơ bản và kiến trúc của ứng dụng đã thay đổi đáng kể:

* Microservices được viết bằng node.js và Spring Boot đang thay thế các ứng dụng khối đá truyền thống. Microservices đi kèm với những thách thức an ninh riêng của họ bao gồm việc thiết lập sự tin tưởng giữa microservices, container, quản lý bí mật, vv Mã số cũ không bao giờ mong đợi để có thể truy cập được từ Internet hiện đang ngồi phía sau một dịch vụ web API hay RESTful để được tiêu thụ bởi các ứng dụng duy nhất (SPA) và các ứng dụng di động. Các giả định về kiến trúc theo mã, chẳng hạn như những người gọi tin cậy, không còn giá trị nữa.
* Các ứng dụng một trang, được viết bằng các khuôn mẫu JavaScript như Angular và React, cho phép tạo các mặt trước rất phong phú về mặt mô đun. Chức năng phía máy khách có truyền thống được phân phát phía máy chủ mang những thách thức về an ninh riêng.
* JavaScript bây giờ là ngôn ngữ chính của web với node.js đang chạy phía máy chủ và khuôn khổ web hiện đại như Bootstrap, Electron, Angular và React đang chạy trên máy khách.

## Các sự cố mới, được hỗ trợ bởi dữ liệu

* **A4:2017-XML External Entities (XXE)** là một loại mới chủ yếu được hỗ trợ bởi các công cụ phân tích mã nguồn an ninh kiểm tra ([SAST](https://www.owasp.org/index.php/Source_Code_Analysis_Tools)) bộ dữ liệu.

## Các vấn đề mới, được hỗ trợ bởi cộng đồng

Chúng tôi yêu cầu cộng đồng cung cấp thông tin chi tiết về hai loại điểm yếu về phía trước. Sau hơn 500 bài đăng ngang hàng và xóa các vấn đề đã được dữ liệu hỗ trợ (chẳng hạn như Sensitive Data Exposure và XXE), hai vấn đề mới là: 

* **A8:2017-Insecure Deserialization**, cho phép thực hiện mã từ xa hoặc thao tác đối tượng nhạy cảm trên các nền tảng bị ảnh hưởng.
* **A10:2017-Insufficient Logging and Monitoring**, sự thiếu hụt này có thể ngăn cản hoặc làm chậm đáng kể hoạt động nguy hiểm và phát hiện vi phạm, phản hồi sự cố và các chứng cứ pháp y kỹ thuật số.

## Sáp nhập hoặc đã nghỉ hưu, nhưng không bị lãng quên

* **A4-Insecure Direct Object References** và **A7-Missing Function Level Access Control** sáp nhập vào **A5:2017-Broken Access Control**.
* **A8-Cross-Site Request Forgery (CSRF)**, như nhiều khuôn khổ bao gồm [CSRF defenses](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)), nó chỉ được tìm thấy trong 5% các ứng dụng.
* **A10-Unvalidated Redirects and Forwards**, trong khi được tìm thấy trong khoảng 8% các ứng dụng, nó đã được vạch ra bởi tổng thể bởi XXE.

![0x06-release-notes-1](images/0x06-release-notes-1.png)
