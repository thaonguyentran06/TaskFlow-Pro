# TaskFlow
Ứng dụng quản lý công việc minimalist, HTML/CSS/JavaScript ES modules và IndexedDB.

## Triển khai
Upload index.html, style.css, app.js, db.js và README.md vào root repository Public. Settings > Pages > Deploy from a branch > main > /(root). Không cần Node.js hay Python. Khi chạy local, dùng VS Code Live Server (không mở file trực tiếp vì ES modules).

## Database
TaskFlowDB / tasks, khóa chính id. Trường: title, description, deadline, category, priority, status, created. IndexedDB lưu theo origin và trình duyệt, không đồng bộ giữa thiết bị. F12 > Application > IndexedDB để xem dữ liệu. Xuất JSON để lưu bản sao (chưa hỗ trợ nhập lại).

## Kiến trúc
Browser UI (index.html + style.css) → app.js (logic CRUD, filter, statistics) → db.js (IndexedDB transactions) → TaskFlowDB/tasks.

## Kiểm thử đề xuất
Tạo công việc, tải lại trang, sửa tên, đổi trạng thái, kiểm tra thống kê, xóa, lọc và tìm kiếm, đổi theme, chạy/tạm dừng/reset Pomodoro, xuất JSON. Kiểm tra giao diện mobile.
