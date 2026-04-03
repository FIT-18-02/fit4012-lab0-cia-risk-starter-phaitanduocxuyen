# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Phạm Anh TÚ

**MSSV:** 1871020615

**Lớp/Nhóm:** CNTT-18_02

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Cơ sở dữ liệu điểm số (Database): Đây là tài sản quan trọng nhất, chứa dữ liệu thô về điểm của tất cả sinh viên.
- Asset 2: Tài khoản người dùng (Credentials): Bao gồm Username và Password của Giảng viên và Sinh viên để truy cập hệ thống.
- Asset 3 (nếu có):Sự riêng tư của sinh viên (Student Privacy): Quyền được giữ bí mật thông tin cá nhân và kết quả học tập.

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A ->(Không đăng nhập được) -> Availability (Tính sẵn sàng): Người dùng có quyền nhưng không thể truy cập dịch vụ vào thời điểm cần thiết.
- Sự cố B ->(Điểm bị đổi từ 8.0 thành 5.0) -> Integrity (Tính toàn vẹn): Dữ liệu đã bị thay đổi trái phép, không còn chính xác so với ban đầu.
- Sự cố C ->(Danh sách điểm bị lộ ra ngoài) -> Confidentiality (Tính bảo mật): Thông tin nhạy cảm bị tiết lộ cho những người không có thẩm quyền (nhóm chat ngoài lớp).

---

## 3. Phân tích sự cố B
- Threat: Hacker xâm nhập hệ thống hoặc một sinh viên có kiến thức IT thực hiện tấn công (Insider threat/External hacker) nhằm chỉnh sửa kết quả học tập.
- Vulnerability: Hệ thống thiếu kiểm soát truy cập (Access Control) chặt chẽ hoặc có lỗ hổng lập trình như SQL Injection.
- Mitigation: Kiểm soát dữ liệu đầu vào (Input Validation), phân quyền người dùng nghiêm ngặt và lưu nhật ký hệ thống (Audit Logs).

---

## 4. Reflection
Viết 5-7 dòng.
Qua bài lab này, em đã hiểu rõ hơn về tầm quan trọng của mô hình CIA trong việc bảo vệ hệ thống thông tin thực tế. Việc thiếu sót bất kỳ yếu tố nào trong ba trụ cột này đều có thể dẫn đến những hậu quả nghiêm trọng như làm mất uy tín của nhà trường hoặc gây thiệt hại cho sinh viên. Em nhận thấy rằng bảo mật không chỉ là dùng các kỹ thuật phức tạp mà còn bắt đầu từ việc thiết kế hệ thống có tính kiểm soát truy cập tốt. Là một sinh viên CNTT, em cần phải rèn luyện tư duy bảo mật ngay từ khi viết những dòng code đầu tiên để đảm bảo tính toàn vẹn và bảo mật cho dữ liệu của người dùng.


---

## 5. Bonus Flag
`FIT4012{A-?-B-?-C-?}`

Flag của em:FIT4012{A-Adore-B-Bypass-C-Crush}

