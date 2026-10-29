# HCM_KS26_CNTT2_IT108_Session14_Ex07
##  Phần 1. Phân tích vấn đề

### 1. Bảng đánh giá rủi ro

| Hạng mục | Rủi ro | Nguyên nhân | Xếp loại |
|---|---|---|---|
| Business Plan | Cao | Chỉ lưu trên máy trưởng nhóm, không sao lưu | Công nghệ + tổ chức |
| Mã nguồn HTML/CSS | Cao | Lưu trên USB dễ hỏng hoặc thất lạc | Công nghệ |
| Database test user | Cao | Không đồng bộ, dữ liệu bị cũ | Công nghệ + tổ chức |
| Slide Pitch | Trung bình | Gửi nhiều bản qua Zalo, dễ nhầm | Tổ chức |
| Tài liệu SRS | Trung bình | Gửi qua email nhiều lần, khó xác định bản mới | Tổ chức |

### 2. Hiện tượng 23 phiên bản file

Hiện tượng này gọi là **Version Conflict** (xung đột phiên bản).

Nguyên nhân là mỗi người sửa một bản riêng rồi gửi qua Zalo, không có nơi lưu chung.

Hậu quả là nhóm không biết bản nào mới nhất, dễ ghi đè bài của nhau, mất thời gian ghép file và có thể nộp nhầm bản cũ.

---

##  Phần 2. Sửa lỗi và nghiệm thu

### 3. Quy trình Hybrid Workflow

**Các bước thực hiện:**

1. **Bước 1:** Tạo thư mục `CampusPay` trên máy để lưu bài làm.
2. **Bước 2:** Cài Google Drive for Desktop và bật Auto Sync cho thư mục này.
3. **Bước 3:** Khi có mạng, file sẽ tự đồng bộ lên Google Drive để các thành viên có thể truy cập.

**Thư mục cần đồng bộ:** Plan, SRS, Slides, TestCases.

**Không cần đồng bộ:** Game, phim, file rác, `node_modules` vì không liên quan đến dự án và tốn dung lượng.

### 4. Xử lý khi gập laptop quá sớm

- **Biểu tượng:** Hiện dấu đang đồng bộ, chưa có dấu tích hoàn thành.
- **Hậu quả:** File mới vẫn còn trên máy, bản trên Drive có thể là bản cũ.
- **Cách xử lý:** Sau khi lưu bài, kiểm tra Google Drive đã hiện trạng thái Synced rồi mới tắt hoặc gập máy.
