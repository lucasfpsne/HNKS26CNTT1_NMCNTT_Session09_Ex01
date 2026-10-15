# Phần I. Phân tích cái sai của Nam
## 1. Cho rằng Microsoft Word phù hợp hơn Markdown
Nam chưa hiểu rõ sự khác biệt giữa Rich Text và Plain Text. Microsoft Word là định dạng tài liệu có cấu trúc phức tạp, chứa nội dung và thông tin định dạng như font chữ, màu sắc, hình ảnh. Trong khi đó, Markdown là văn bản thuần túy, sử dụng các ký hiệu đơn giản như `#`, `**`, `-` để định dạng. GitHub có thể hiển thị trực tiếp Markdown trên trình duyệt, đồng thời Git dễ dàng theo dõi những dòng được thêm, sửa hoặc xóa thông qua Git Diff. Ngược lại, Git không thể so sánh trực tiếp từng dòng nội dung bên trong file `.docx` như với file văn bản, khiến việc theo dõi thay đổi và giải quyết xung đột khó khăn hơn.
## 2. Cho rằng Markdown không thể tạo tài liệu chuyên nghiệp
Markdown an toàn và nhẹ hơn vì : 
-  Dung lượng nhỏ: Markdown chủ yếu lưu văn bản và ký hiệu định dạng nên thường nhẹ hơn Word.
    
-   Dễ khôi phục: Nếu mất một byte dữ liệu, file Markdown thường vẫn có thể mở và đọc được phần lớn nội dung. Trong khi đó, file `.docx` có cấu trúc ZIP/XML nên lỗi dữ liệu có thể khiến tài liệu không mở được hoặc mất một phần nội dung. Tuy nhiên, mất một byte không đồng nghĩa file Word chắc chắn hỏng hoàn toàn.
    
-   Hỗ trợ Git Diff: Git có thể xác định chính xác dòng nào thay đổi, giúp quản lý phiên bản và xử lý xung đột thuận tiện hơn.
# Phần II. Hoàn Thiện 
Bước 1: Truy cập [StackEdit](https://stackedit.io/app) để mở trình soạn thảo Markdown.

Bước 2: Sao chép đoạn giới thiệu dự án từ Microsoft Word và dán vào StackEdit, sau đó chỉnh lại cú pháp Markdown.

Bước 3: Nhập nội dung Markdown mẫu sau:

Nội dung file README.md
```
	1.Giới thiệu
Smart Farm là dự án quản lý nông trại thông minh của nhóm sinh viên PTIT.
	2. Mục tiêu
- Theo dõi nhiệt độ và độ ẩm.
- Quản lý dữ liệu cảm biến.
- Tự động hóa quá trình giám sát.
	3. Công nghệ sử dụng
- Python
- PowerShell
- GitHub
	4. Hướng dẫn chạy
```bash
python main.py
```
**Ghi chú:** Đây là nội dung minh họa cho tài liệu dự án.

Bước 4: Kiểm tra phần xem trước (Preview) trong StackEdit để đảm bảo tiêu đề, danh sách và khối mã hiển thị chính xác.

Bước 5: Chọn chức năng xuất Markdown trong StackEdit, tải tệp về và lưu với tên `README.md`. Sau đó đưa file lên GitHub để các thành viên có thể đọc và theo dõi thay đổi.
