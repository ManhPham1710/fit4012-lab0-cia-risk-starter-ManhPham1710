Lab 01 Answers
CIA & Risk: Hệ thống lưu điểm
Họ và tên: Phạm Đức Mạnh

MSV: 1871020380

1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

Asset 1: Cơ sở dữ liệu điểm số của sinh viên (Student Grades Database) – Tài sản thông tin.

Asset 2: Mã nguồn của ứng dụng quản lý/nhập điểm (Grading Application Source Code) – Tài sản phần mềm.

Asset 3 (nếu có): Tài khoản và quyền truy cập của giảng viên/quản trị viên (Teacher/Admin Credentials) – Tài sản định danh.

2. Mapping CIA
Ghép từng sự cố với CIA.

Sự cố A (Điểm bị sửa đổi trái phép) -> Integrity (Tính toàn vẹn - Dữ liệu điểm bị thay đổi làm mất tính chính xác).

Sự cố B (Hệ thống bị sập vào lúc kiểm tra) -> Availability (Tính khả dụng - Hệ thống bị gián đoạn, không thể truy cập).

Sự cố C (Sinh viên xem được điểm của sinh viên khác) -> Confidentiality (Tính bảo mật - Thông tin riêng tư bị rò rỉ cho người không có thẩm quyền).

3. Phân tích sự cố B
Threat: Kẻ tấn công thực hiện chiến dịch DDoS (Distributed Denial of Service) hoặc số lượng lớn sinh viên truy cập đồng thời tạo ra một cuộc "tự DDoS" ngoài ý muốn.

Vulnerability: Hệ thống server có băng thông hạn chế, cấu hình phần cứng yếu, hoặc thiếu cơ chế cân bằng tải (Load Balancing) và chống DDoS.

Mitigation: Triển khai giải pháp cân bằng tải (Load Balancer), cấu hình Auto-scaling (tự động mở rộng tài nguyên), tích hợp dịch vụ giảm thiểu DDoS (WAF/CDN) và tối ưu hóa truy vấn cơ sở dữ liệu để chịu tải tốt hơn.

4. Reflection
(Viết 5-7 dòng cảm ý của riêng bạn về bài lab này, ví dụ:)

Qua bài Lab 01 này, em đã hiểu rõ hơn về cách áp dụng mô hình CIA vào một hệ thống thực tế như hệ thống lưu điểm. Việc xác định đúng tài sản (Assets) giúp chúng em biết rõ mình cần tập trung bảo vệ cái gì quan trọng nhất. Phân tích các mối đe dọa và lỗ hổng từ sự cố thực tế giúp em nhận ra rằng bảo mật không chỉ là chống lại hacker, mà còn là đảm bảo tính sẵn sàng trước các sự cố quá tải. Bài học này giúp em có tư duy quản trị rủi ro tốt hơn trong việc thiết kế và vận hành hệ thống sau này.

5. Bonus Flag
FIT4012{A-?-B-?-C-?}

Flag của em: FIT4012{A-INTEGRITY-B-AVAILABILITY-C-CONFIDENTIALITY}
