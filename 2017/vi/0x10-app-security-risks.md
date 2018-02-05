# Rủi ro - Áp dụng Rủi ro An ninh

## Rủi ro An ninh Ứng dụng là gì?

Những kẻ tấn công có thể sử dụng nhiều đường dẫn khác nhau thông qua ứng dụng của bạn để gây hại cho doanh nghiệp hoặc tổ chức của bạn. Mỗi một trong những đường dẫn này thể hiện một nguy cơ có thể, hoặc không thể, nghiêm trọng đủ để đảm bảo sự chú ý.

![App Security Risks](images/0x10-risk-1.png)

Đôi khi những con đường này là tầm thường để tìm và khai thác, và đôi khi chúng rất khó khăn. Tương tự, những thiệt hại gây ra có thể không có hậu quả, hoặc nó có thể đưa bạn ra khỏi kinh doanh. Để xác định rủi ro cho tổ chức của bạn, bạn có thể đánh giá khả năng liên quan đến mỗi tác nhân đe dọa, vector tấn công, và điểm yếu về an ninh và kết hợp nó với ước tính về tác động kỹ thuật và kinh doanh đối với tổ chức của bạn. Cùng nhau, những yếu tố này xác định nguy cơ tổng thể của bạn.

## Rủi ro của tôi là gì

[OWASP Top 10](https://www.owasp.org/index.php/Top10) tập trung vào việc xác định những rủi ro bảo mật ứng dụng web nghiêm trọng nhất đối với một loạt các tổ chức. Đối với mỗi rủi ro này, chúng tôi cung cấp thông tin chung về khả năng và ảnh hưởng kỹ thuật sử dụng sơ đồ xếp hạng đơn giản sau, dựa trên Phương pháp Đánh giá Rủi ro của OWASP.  

| Đại lý đe doạ | Khả năng khai thác | Điểm yếu Yếu | Tính dễ bị phát hiện | Tác động Kỹ thuật | Tác động kinh doanh |
| -- | -- | -- | -- | -- | -- |
| Appli-   | Easy 3 | Widespread 3 | Easy 3 | Severe 3 | Business     |
| cation   | Average 2 | Common 2 | Average 2 | Moderate 2 | Specific |
| Specific | Difficult 1 | Uncommon 1 | Difficult 1 | Minor 1 |       |

Trong ấn bản này, chúng tôi đã cập nhật hệ thống đánh giá rủi ro để hỗ trợ tính toán khả năng và tác động của bất kỳ rủi ro nào. Để biết thêm chi tiết, vui lòng xem [Lưu ý về Rủi ro](0xc0-note-about-risks.md). 

Mỗi tổ chức là duy nhất, và như vậy là các mối đe dọa diễn viên cho tổ chức đó, mục tiêu của họ và tác động của bất kỳ hành vi vi phạm nào. Nếu một tổ chức lợi ích công cộng sử dụng hệ thống quản lý nội dung (CMS) để cung cấp thông tin công cộng và hệ thống y tế sử dụng CMS giống hệt nhau cho các hồ sơ y tế nhạy cảm, các tác nhân gây nguy hiểm và các tác động kinh doanh có thể rất khác nhau đối với cùng một phần mềm. Điều rất quan trọng để hiểu được rủi ro đối với tổ chức của bạn dựa trên các tác nhân gây ra hiện tượng đe dọa và tác động kinh doanh.

Khi có thể, tên của những rủi ro trong Top 10 được sắp xếp với [Common Weakness Enumeration](https://cwe.mitre.org/) (CWE) điểm yếu để quảng bá các quy ước đặt tên chung được chấp nhận và để giảm sự nhầm lẫn.

## Tài liệu tham khảo

### OWASP

* [Phương pháp đánh giá rủi ro OWASP](https://www.owasp.org/index.php/OWASP_Risk_Rating_Methodology)
* [Bài báo về Mô hình Nguy cơ / Nguy cơ](https://www.owasp.org/index.php/Threat_Risk_Modeling)

### Bên ngoài

* [ISO 31000: Quản lý rủi ro tiêu chuẩn](https://www.iso.org/iso-31000-risk-management.html)
* [ISO 27001: ISMS](https://www.iso.org/isoiec-27001-information-security.html)
* [NIST Cyber Framework (Hoa Kỳ)](https://www.nist.gov/cyberframework)
* [Các Giải pháp Giảm nhẹ Chiến lược ASD (AU)](https://www.asd.gov.au/infosec/mitigationstrategies.htm)
* [NIST CVSS 3.0](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator)
* [Công cụ mô hình đe dọa của Microsoft](https://www.microsoft.com/en-us/download/details.aspx?id=49168)
