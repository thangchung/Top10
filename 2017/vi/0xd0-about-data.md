# +Dat Phương pháp luận và dữ liệu

Tại hội nghị thượng đỉnh dự án OWASP, những người tham gia tích cực và các thành viên trong cộng đồng đã quyết định xem xét tính dễ bị tổn thương, với tối đa hai (2) lớp dễ bị tổn thương về phía trước, với thứ tự được xác định bằng số liệu định lượng và một phần bằng các cuộc điều tra định tính.
 
## Khảo sát Xếp hạng Ngành

Đối với cuộc khảo sát, chúng tôi đã thu thập các loại tổn thương đã được xác định trước đó là "trên đỉnh" hoặc đã được đề cập trong phản hồi cho năm 2017 RC1 trong danh sách gửi thư Top 10. Chúng tôi đưa họ vào một cuộc khảo sát xếp hạng và yêu cầu người trả lời xếp hạng 4 lỗ hổng hàng đầu mà họ cảm thấy nên được đưa vào OWASP Top 10 - 2017. Cuộc khảo sát mở cửa từ ngày 2 tháng 8 đến ngày 18 tháng 9 năm 2017. Đã thu thập được 516 câu trả lời và các lỗ hổng đã được xếp hạng.

| Cấp | Điều tra dễ bị tổn thương Các loại | Số điểm |
| -- | -- | -- |
| 1 | Exposure of Private Information ('Privacy Violation') [CWE-359] | 748 |
| 2 | Cryptographic Failures [CWE-310/311/312/326/327]| 584 |
| 3 | Deserialization of Untrusted Data [CWE-502] | 514 |
| 4 | Authorization Bypass Through User-Controlled Key (IDOR & Path Traversal) [CWE-639] | 493 |
| 5 | Insufficient Logging and Monitoring [CWE-223 / CWE-778]| 440 |

Exposure of Private Information rõ ràng là dễ bị tổn thương cao nhất, nhưng rất dễ thích ứng như một sự nhấn mạnh vào **A3:2017-Sensitive Data Exposure**. Cryptographic Failures có thể phù hợp với Sensitive Data Exposure. Insecure deserialization được xếp hạng ở vị trí thứ ba, vì vậy nó được thêm vào Top 10 như **A8:2017-Insecure Deserialization** sau khi đánh giá rủi ro. Xếp hạng thứ tư User-Controlled Key được bao gồm trong **A5:2017-Broken Access Control**; nó là tốt để xem nó xếp hạng cao trong cuộc khảo sát, vì không có nhiều dữ liệu liên quan đến các lỗ hổng ủy quyền. Số 5 được xếp loại trong cuộc khảo sát là Insufficient Logging and Monitoring, mà chúng tôi tin là phù hợp với danh sách Top 10, đó là lý do tại sao nó đã trở thành **A10:2017-Insufficient Logging & Monitoring**. Chúng tôi đã chuyển đến một điểm mà các ứng dụng cần để có thể xác định những gì có thể là một cuộc tấn công và tạo ra đăng nhập, cảnh báo, leo thang và phản ứng thích hợp. 

## Gọi Dữ liệu công khai

Theo truyền thống, dữ liệu được thu thập và phân tích nhiều hơn theo dòng dữ liệu tần số: bao nhiêu lỗ hổng đã được tìm thấy trong các ứng dụng được kiểm tra. Như đã biết, các công cụ truyền thống báo cáo tất cả các trường hợp phát hiện ra một lỗ hổng và con người truyền thống báo cáo một phát hiện với một số ví dụ. Điều này làm cho rất khó để tổng hợp hai kiểu báo cáo theo cách tương đương.

Đối với năm 2017, tỷ lệ mắc đã được tính bằng số lượng ứng dụng trong một bộ dữ liệu nhất định có một hoặc nhiều loại lỗ hổng cụ thể. Dữ liệu từ nhiều cộng tác viên lớn đã được cung cấp trong hai lần xem. Phương thức thứ nhất là kiểu tần số truyền thống để đếm từng thể hiện của một lỗ hổng, trong khi thứ hai là số ứng dụng, trong đó mỗi lỗ hổng được tìm thấy (một lần hoặc nhiều lần). Mặc dù không hoàn hảo, điều này cho phép chúng tôi so sánh dữ liệu từ các công cụ hỗ trợ của con người và con người được hỗ trợ công cụ. Các dữ liệu thô và công việc phân tích là [có sẵn trong GitHub](https://github.com/OWASP/Top10/tree/master/2017/datacall). Chúng tôi dự định mở rộng thêm về cấu trúc này cho các phiên bản trong tương lai của Top 10.

Chúng tôi đã nhận được 40 bài đăng trong cuộc gọi dữ liệu và vì nhiều người từ cuộc gọi dữ liệu ban đầu đã tập trung vào tần suất, chúng tôi có thể sử dụng dữ liệu từ 23 cộng tác viên bao gồm ~ 114.000 ứng dụng. Chúng tôi đã sử dụng một khoảng thời gian một năm nếu có thể và được xác định bởi người đóng góp. Phần lớn các ứng dụng là duy nhất, mặc dù chúng tôi thừa nhận khả năng ứng dụng lặp lại giữa dữ liệu hàng năm từ Veracode. 23 bộ dữ liệu được sử dụng đã được xác định là công cụ hỗ trợ thử nghiệm của con người hoặc cụ thể cung cấp tỷ lệ mắc từ các công cụ hỗ trợ của con người. Sự dị thường trong dữ liệu đã chọn 100% + đã được điều chỉnh xuống đến 100% tối đa Để tính tỷ lệ mắc, chúng tôi tính phần trăm của tổng số các ứng dụng đã được tìm thấy có chứa từng loại dễ bị tổn thương. Xếp hạng tỷ lệ mắc đã được sử dụng cho tính toán tỷ lệ hiện nhiễm trong tổng thể nguy cơ xếp hạng Top 10.
