# Blog

Blog
image.png
Setup
Trong đó ý nghĩa các folder như sau:

public: chứa các file public bên ngoài như js, css và template của ứng dụng
site: chứa ba folder chính là controller, model và view. Folder này chứa source code của ứng dụng frontend
system: chứa hai folder
core: Các thư viện cấu hình cho hệ thống MVC
library: Chứa các thư viện được tạo trong quá trình xây dựng ứng dụng
admin: folder này giống như site nhưng nó chứa source dành cho ứng dụng backend
index.php đóng vai trò file bootstrap cho frontend, nó sẽ chạy code của folder site
admin.php đóng vai trò file bootstrap cho backend, nó chạy code của folder admin
Như vậy tóm lại:

Hệ thống MVC sẽ phân chia làm hai module chính là site (frontend) và admin (backend), mỗi module sẽ có một file bootstrap (index.php cho folder site và admin.php cho folder admin).
Hệ thống MVC có một folder system dùng để chứa những thư viện dùng chung cho cả frontend và backend
Hệ thống MVC có folder public chứa các file như js, css, jquery, ... Đặc biệt nó có một folder upload dùng để chứa hình ảnh upload cho tin tức

<h1>  Phần 2</h1>
Trong bài các bạn cần chú ý các vấn đề sau:

Có tạo mới file admin/config/init.php
Xóa đi phương thức load() trong FT_Controller.php
Chỉnh lại file bootstrap admin.php và nó có gọi qua hàm FT_Load() nằm trong file FT_Common.php
Thêm hàm FT_Load() vào file FT_Common.php

<h1>Phần 3</h1>
Mục lục
1. Tạo file config.php cho module trong MVC
2. Tạo thư viện load config trong MVC
3. Tạo đối tượng load config trong FT_Controller
4. Thao tác với thư viện config trong Controller
<h1>Phần 4</h1>
1. Library trong mô hình MVC
2. Thư mục library nằm ở đâu trong mô hình MVC
3. Viết thư viện load library
4. Bổ sung thư viện vào FT_Controller
4. Load libray tại Controller
<h1>Phần 5</h1>
<h1>Phần 6</h1>
1. View là gì?
2. Viết thư viện view loader
3. Thêm view loader vào FT_Controller
4. Tạo mới một view
5. Load view trong Controller
6 Truyền Data từ controller sang view
<h1>Phần 7</h1>
1. Vị trí đặt Base_Controller
2. Load Base_Controller trong hàm FT_Load()
3. Ví dụ sử dụng Base_Controller
