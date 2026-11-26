# BLOOM — Personal Productivity Studio
HTML/CSS/JavaScript ES modules + IndexedDB. Không cần Node/Python. Upload 5 file vào root nhánh main, Settings > Pages > main / root. Dùng HTTPS GitHub Pages (không mở file:// vì ES modules).

## Chức năng
CRUD, trạng thái, tìm kiếm/lọc/sắp xếp, Kanban (đổi trạng thái bằng select), Eisenhower, lịch tuần, cây ảo 5 giai đoạn, Pomodoro 25 phút, thống kê và heatmap 84 ngày, nhật ký theo ngày, dark mode, xuất JSON.

## Database
TaskFlowDB version 2: tasks (id), journal (date), settings (id). Nâng cấp từ version 1 giữ dữ liệu cũ trên cùng origin. Công việc cũ không có completedAt không được tính vào heatmap; không tự tạo lịch sử giả. Cây dựa trên số công việc hiện hoàn thành. Dữ liệu riêng theo trình duyệt/origin, không có server hay đồng bộ. JSON chỉ xuất, không nhập. Timer chạy khi trang còn mở, không lưu phiên đang chạy khi reload. Font Google có fallback offline.

## Kiểm thử thủ công
Tạo việc, sửa, đổi trạng thái, reload, xóa; kiểm tra Kanban, matrix, lịch tuần, heatmap sau khi hoàn thành; lưu nhật ký và reload; thử dark mode, export, timer. DevTools > Application > IndexedDB > TaskFlowDB để xem database.

### Rose Final
Sử dụng Arial/Helvetica cho toàn bộ nội dung tiếng Việt, chuẩn hóa Unicode NFC, không dùng font tải ngoài.
