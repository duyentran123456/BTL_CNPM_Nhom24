# Phần mềm quản lý thu phí trong tổ dân phố
Phần mềm có chức năng hỗ trợ quản lý thu phí trong tổ dân phố, gồm các chức năng: xem danh sách hộ khẩu, quản lý thu phí các hộ, quản lý đóng góp các hộ, thêm loại đóng góp, xem chi tiết các khoản đóng của từng hộ, thống kê các khoản phí đã thu theo thể loại và theo thời gian.

## Requirements:
- **[JDK 8. trở lên](https://www.oracle.com/java/technologies/javase-downloads.html)**
- **IDE:** 
  * Netbeans IDE (download tại [đây](https://netbeans.org/downloads/8.2/rc/))
  * hoặc Eclipse IDE (download tại [đây](https://www.eclipse.org/downloads/))
 - **[XAMPP](https://www.apachefriends.org/download.html)** (có thể xem hướng dẫn cấu hình XAMPP tại [đây](https://thachpham.com/thu-thuat/cai-dat-localhost-xampp.html))
 
 ## Cài đặt chương trình:
 **Clone project từ github** 
   - Tải file nén trực tiếp từ trang github   
   
 **Tạo database** 
   - Mở trình duyệt, truy cập _http://localhost/phpmyadmin/_    
   - Tạo một database mới, đặt tên là _quanlydonggop_    
   - Copy câu lệnh SQL từ _quanlydonggop.sql_ trong thư mục _database_ của project, ấn thực thi    
   
 **Thêm thư viện cho project:** 
   - Mở Netbeans, chọn _File -> Open project_, tìm đến thư mục chứa project, chọn project và bấm Open project    
   - Ấn chuột phải vào project trong giao diện Netbeans, chọn _properties -> libraries -> add jar_, tìm đến thư mục libs của project và chọn các file .jar trong thư mục 
   
 **Chạy project:** 
   - Vào _src/com/dao/impl/AbstractDAO.java_, thay _"root"_ và _""_ trong phương thức _getConnection()_ bằng _username_ và _password_ trong MySQL của bạn.    
   - Vào _src/com/gui/main/Run.java_, ấn vào Run để chạy project    
   - Ứng dụng hiển thị màn hình đăng nhập, điền username _"admin"_ và mật khẩu _"1"_ để tiếp tục
