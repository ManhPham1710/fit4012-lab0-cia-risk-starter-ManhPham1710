# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Phạm Đức Mạnh

**MSSV:** 1871020

**Lớp/Nhóm:** CNTT 18-01

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Bảng điểm sinh viên
- Asset 2: Tài khoản đăng nhập (giảng viên/sinh viên)
- Asset 3: Cơ sở dữ liệu điểm
- Asset 4: Log thay đổi điểm

---

## 2. Mapping CIA

- Sự cố A -> Availability (hệ thống không đăng nhập được = không sẵn sàng)
- Sự cố B -> Integrity (điểm bị sửa trái phép = mất toàn vẹn)
- Sự cố C -> Confidentiality (danh sách điểm bị lộ = mất bí mật)

---

## 3. Phân tích sự cố B
- Threat: Người dùng trái phép hoặc nội bộ sửa điểm không đúng thẩm quyền
- Vulnerability: Phân quyền chưa chặt, không có log theo dõi, thiếu xác thực 2 lớp (MFA)
- Mitigation: Bật MFA, phân quyền rõ theo vai trò, ghi log mọi thao tác sửa điểm, yêu cầu phê duyệt khi thay đổi điểm

---

## 4. Reflection
Nếu là quản trị viên, em sẽ ưu tiên xử lý sự cố B trước vì điểm bị sửa sai ảnh hưởng trực tiếp đến quyền lợi sinh viên và tính tin cậy của hệ thống. Sự cố A chỉ là gián đoạn tạm thời, có thể khắc phục nhanh. Sự cố C đã xảy ra rồi nên cần điều tra song song. Việc kiểm soát chặt quyền sửa điểm và có log đầy đủ là ưu tiên hàng đầu.


---

## 5. Bonus Flag
`FIT4012{A-A-B-I-C-C}`

Flag của em:`FIT4012{A-A-B-I-C-C}`

