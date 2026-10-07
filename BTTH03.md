**Bài 3 : Kiến trúc sư hạ tầng Cloud Server** 

### ***Phần 1: Mã nguồn***

\- Danh sách đầy đủ các câu lệnh Windows PowerShell đã sử dụng để hoàn thành 3 yêu cầu nghiệp vụ (tạo cây thư mục, tạo file, sao chép đệ quy), ghi theo đúng thứ tự thực thi.  
mkdir .\\Farm-Manager\\code\\app

mkdir .\\Farm-Manager\\database\\db

mkdir .\\Farm-Manager\\logs\\guides

New-Item .\\Farm-Manager\\code\\app\\main.py, .\\Farm-Manager\\code\\app\\models.py, .\\Farm-Manager\\code\\app\\utils.py \-ItemType File

Copy-Item .\\Farm-Manager\\logs .\\Farm-Manager\\logs-backup \-Recurse

\- Ghi chú ngắn bên cạnh mỗi lệnh giải thích: lệnh này làm gì và tham số `-Recurse` / `-Force` có ý nghĩa gì

mkdir → tạo thư mục.

New-Item → tạo file.

Copy-Item → sao chép.

\-Recurse → sao chép cả thư mục con và file bên trong.

\-Force → ép thực hiện, kể cả khi có một số trường hợp bị cản trở bởi thuộc tính/tồn tại của mục

### ***Phần 2: Kiểm thử***

\- Sau khi chạy xong, gõ lệnh ls .\\Farm-Manager (hoặc dir .\\Farm-Manager) để liệt kê cây thư mục vừa tạo.

Sau khi làm xong, chạy:

ls .\\Farm-Manager

hoặc muốn **vẽ đẹp toàn bộ cây thư mục \+ file** thì:

tree .\\Farm-Manager /F

Dùng `.\` để sử dụng đường dẫn tương đối, giúp lệnh không phụ thuộc vào ổ đĩa hoặc đường dẫn tuyệt đối cụ thể như `C:\...` 

