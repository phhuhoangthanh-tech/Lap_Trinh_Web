# Sổ tay các lệnh Git cơ bản (Git Cheat Sheet)

## 1. Khởi tạo & Trạng thái
- git init: Khởi tạo một Git repository (kho lưu trữ) mới tại thư mục hiện tại.
- git status: Kiểm tra trạng thái hiện tại (file nào mới tạo, file nào đã sửa, file nào đã sẵn sàng commit).

## 2. Lưu trữ thay đổi (Staging & Commit)
- git add <tên_file>: Đưa file cụ thể vào khu vực chuẩn bị lưu (Staging Area).
- git add .: Đưa tất cả các file có thay đổi vào Staging Area.
- git reset <tên_file: Bỏ file ra khỏi Staging Area nếu lỡ `add` nhầm (không làm mất nội dung code).
- git commit -m "nội dung ghi chú": Lưu lại một phiên bản code kèm theo lời mô tả thay đổi.

## 3. Xem lại lịch sử & So sánh
- git log: Xem toàn bộ lịch sử các lần commit (tác giả, ngày giờ, mã hash, thông điệp).
- git log --oneline: Xem lịch sử commit rút gọn (mỗi commit 1 dòng ngắn gọn).
- git diff: So sánh sự khác nhau giữa code hiện tại và lần commit gần nhất (khi chưa gõ `git add`).

## 4. Hoàn tác (Undo)
- git restore <tên_file>: Khôi phục lại trạng thái file giống hệt commit gần nhất (hủy toàn bộ chỉnh sửa chưa lưu).

## 5. Làm việc với GitHub (Remote)
- git remote add origin <URL_REPO>`: Kết nối thư mục máy tính với repo trên GitHub.
- git branch -M main`: Đổi tên nhánh mặc định thành `main`.
- git push -u origin main`: Đẩy toàn bộ commit từ máy tính lên GitHub.
- git pull`: Kéo code mới nhất từ GitHub về máy tính.


---
-git merge {branch name}
-git branch -d {brach name}