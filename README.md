# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session15_Ex06
### 1. Bản đặc tả không gian cộng tác (README.md)

markdown
# Green-Tech Smart Farm Workspace

## A. Cấu trúc Thư mục
- /sensors-code/: Code cảm biến (Python/Node.js). Chạy Hybrid (Local Git + Cloud Sync).
- /sensors-code/.env: Chứa pass/API key. Khai báo trong .gitignore, cấm push lên Git/Cloud.
- /reports-investor/: Báo cáo tiến độ và tài chính cho nhà đầu tư.
- /device-specs/: Tài liệu thông số phần cứng từ đối tác.

## B. Phân quyền
- Nhà đầu tư: Chỉ xem (View Only) thư mục /reports-investor/.
- Đối tác thiết bị: Bình luận (Comment/Suggest) trong /device-specs/.
- Đội Dev: Quyền Chỉnh sửa (Editor) toàn bộ workspace.

## C. Kênh giao tiếp (Channels)
- #general: Thông báo chung.
- #sensor-alerts: Nhận log lỗi cảm biến tự động.
- #dev-sync: Thảo luận kĩ thuật. Lỗi cảm biến bàn ở đây sẽ tạo thành Task có gắn Deadline cụ thể trên Workspace.

---

### 2. Xử lý sự cố & Bàn giao

* **Khôi phục folder `sensors` bị xóa nhầm:**
1. Mở Terminal gõ `git checkout HEAD -- sensors-code/` để kéo lại từ Git local.
2. Nếu mất hẳn, vào **Recycle Bin / Trash** trên giao diện Web của Cloud (hoặc History commit trên GitHub) bấm **Restore**.


* **Bảo mật file `.env`:** Thêm dòng `.env` vào tệp `.gitignore` ngay khi tạo project. Thành viên mới tự tạo file `.env` local theo file mẫu `.env.example`.
* **Chuyển quyền (Transfer Ownership):** Hết môn, Trưởng nhóm vào **Settings > Workspace Permissions**, chọn tài khoản Thầy/Cô hoặc Trưởng nhóm mới rồi đổi quyền thành **Owner** là xong.
