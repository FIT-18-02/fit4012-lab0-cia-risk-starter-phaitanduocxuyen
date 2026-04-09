# FIT4012 - Report 1 Page
## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab
- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm
- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính
**Assets:**
- Dữ liệu điểm số (Grade Data): Đây là tài sản quan trọng nhất, phản ánh kết quả học tập của sinh viên.
- Cơ sở dữ liệu người dùng: Bao gồm thông tin đăng nhập, phân quyền của giảng viên và sinh viên.

**CIA mapping:**
- Sự cố A -> (Rò rỉ bảng điểm chưa công bố): -> Confidentiality (Tính bảo mật) - Thông tin bị truy cập bởi người không có thẩm quyền.   
- Sự cố B -> (Sinh viên tự ý chỉnh sửa điểm trên hệ thống): -> Integrity (Tính toàn vẹn) - Dữ liệu bị thay đổi trái phép, không còn chính xác.
- Sự cố C -> (Hệ thống sập trong giờ đăng ký xem điểm): -> Availability (Tính khả dụng) - Người dùng không thể truy cập dịch vụ khi cần thiết.

**Phân tích sự cố B:**
- Threat: Sinh viên có kỹ năng tin học (Insider threat) hoặc hacker bên ngoài cố tình xâm nhập để thay đổi kết quả học tập.
- Vulnerability: Hệ thống kiểm soát truy cập lỏng lẻo, thiếu cơ chế xác thực đa yếu tố (2FA) hoặc không kiểm tra kỹ quyền hạn (Broken Access Control) ở phía backend.
- Mitigation: Triển khai phân quyền nghiêm ngặt (Role-based Access Control), mã hóa dữ liệu, thiết lập nhật ký hệ thống (Audit logs) để theo dõi mọi thao tác thay đổi dữ liệu và sử dụng xác thực hai lớp cho tài khoản giảng viên.

### 4. Kết luận ngắn
Qua bài lab này, em đã nắm vững cách áp dụng mô hình CIA để phân loại các rủi ro an ninh mạng trong thực tế. Phần khó nhất là việc phân biệt rạch ròi giữa Threat và Vulnerability, vì chúng thường có mối quan hệ mật thiết với nhau. Điều cần lưu ý nhất khi phân tích một sự cố an toàn thông tin là phải nhìn nhận từ nhiều phía: không chỉ ở khía cạnh kỹ thuật mà còn ở quy trình vận hành và con người. Việc xác định đúng tài sản (Assets) chính là bước then chốt để xây dựng một chiến lược bảo mật hiệu quả và tiết kiệm tài nguyên.