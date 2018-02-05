# +A: Tiếp theo là gì cho Người quản lý ứng dụng

## Quản lý toàn bộ Vòng đời Ứng dụng

Ứng dụng thuộc về những hệ thống phức tạp nhất con người thường xuyên tạo ra và duy trì. Quản lý CNTT cho một ứng dụng nên được thực hiện bởi các chuyên gia CNTT chịu trách nhiệm về toàn bộ vòng đời ứng dụng của CNTT. Chúng tôi đề nghị thiết lập vai trò của người quản lý ứng dụng làm đối tác kỹ thuật cho chủ sở hữu ứng dụng. Người quản lý ứng dụng chịu trách nhiệm về toàn bộ vòng đời ứng dụng từ khía cạnh CNTT, từ việc thu thập các yêu cầu cho tới khi quá trình nghỉ hưu, thường bị bỏ sót. 

## Yêu cầu và Quản lý Tài nguyên

* Thu thập và thương lượng các yêu cầu kinh doanh cho một ứng dụng với doanh nghiệp, bao gồm các yêu cầu bảo vệ đối với tính bí mật, tính xác thực, tính toàn vẹn và tính sẵn sàng của tất cả các tài sản dữ liệu và logic kinh doanh dự kiến.
* Biên soạn các yêu cầu kỹ thuật bao gồm các yêu cầu bảo mật chức năng và phi chức năng.
* Lập kế hoạch và đàm phán ngân sách bao gồm tất cả các khía cạnh của thiết kế, xây dựng, thử nghiệm và vận hành, bao gồm các hoạt động an ninh.

## Yêu cầu Đề xuất (RFP) và Hợp đồng

* Đàm phán các yêu cầu với các nhà phát triển nội bộ hoặc bên ngoài, bao gồm các nguyên tắc và yêu cầu bảo mật đối với chương trình bảo mật của bạn, ví dụ: SDLC, thực tiễn tốt nhất.
* Đánh giá việc hoàn thành tất cả các yêu cầu kỹ thuật, bao gồm quy hoạch và giai đoạn thiết kế.
* Đàm phán tất cả các yêu cầu kỹ thuật, bao gồm các thỏa thuận về thiết kế, bảo mật và mức dịch vụ (SLA).
* Thông qua mẫu và danh sách kiểm tra, chẳng hạn như [OWASP hợp đồng phần mềm an toàn](https://www.owasp.org/index.php/OWASP_Secure_Software_Contract_Annex). **Chú thích**: Phụ lục là luật hợp đồng của Hoa Kỳ, vì vậy xin vui lòng tham khảo ý kiến tư vấn pháp lý trước khi sử dụng phụ lục mẫu.

## Kế hoạch và Thiết kế

* Đàm phán kế hoạch và thiết kế với các nhà phát triển và cổ đông nội bộ, ví dụ: chuyên gia bảo mật.
* Xác định kiến trúc, kiểm soát và các biện pháp đối phó an toàn phù hợp với nhu cầu bảo vệ và mức độ đe dọa dự kiến. Điều này cần được hỗ trợ bởi các chuyên gia bảo mật.
* Đảm bảo rằng chủ sở hữu ứng dụng chấp nhận rủi ro còn lại hoặc cung cấp các tài nguyên bổ sung.
* Trong mỗi lần chạy nước rút, đảm bảo các câu chuyện bảo mật được tạo ra bao gồm các khó khăn được thêm vào cho các yêu cầu phi chức năng.

## Triển khai, Thử nghiệm và Triển khai

* Tự động triển khai an toàn ứng dụng, giao diện và tất cả các thành phần yêu cầu, bao gồm cả các ủy quyền cần thiết.
* Kiểm tra các chức năng kỹ thuật và tích hợp với kiến trúc CNTT và phối hợp các bài kiểm tra kinh doanh.
* Tạo ra "sử dụng" và "lạm dụng" các trường hợp thử nghiệm từ quan điểm kỹ thuật và kinh doanh.
* Quản lý kiểm tra an ninh theo quy trình nội bộ, nhu cầu bảo vệ, và mức độ đe dọa giả định bằng ứng dụng.
* Đặt ứng dụng đang hoạt động và di chuyển từ ứng dụng đã sử dụng trước đó nếu cần.
* Hoàn tất tất cả các tài liệu, bao gồm CMDB và kiến trúc an ninh.

## Hoạt động và Quản lý Thay đổi

* Các hoạt động phải bao gồm các nguyên tắc về quản lý bảo mật của ứng dụng (ví dụ: quản lý bản vá).
Nâng cao nhận thức bảo mật của người dùng và quản lý mâu thuẫn về khả năng sử dụng và bảo mật.
* Lập kế hoạch và quản lý các thay đổi, ví dụ: di chuyển sang các phiên bản mới của ứng dụng hoặc các thành phần khác như hệ điều hành, middleware và thư viện.
* Cập nhật tất cả các tài liệu, bao gồm trong cơ sở dữ liệu quản lý sự thay đổi (CMDB) và kiến trúc an ninh, kiểm soát, và biện pháp đối phó, bao gồm bất kỳ runbooks hoặc tài liệu dự án.

## Hệ thống nghỉ hưu

* Bất kỳ dữ liệu cần thiết nào cần được lưu trữ. Tất cả dữ liệu khác cần được xóa an toàn.
* An toàn nghỉ hưu cho ứng dụng, bao gồm xóa các tài khoản và vai trò không được sử dụng và các quyền.
* Thiết lập trạng thái ứng dụng của bạn để nghỉ hưu trong CMDB.
