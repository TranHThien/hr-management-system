# Hệ thống Quản lý Nhân sự (HRM System)

Một hệ thống quản lý nhân sự toàn diện được xây dựng trên nền tảng **ASP.NET MVC**, được thiết kế để tối ưu hóa các quy trình tổ chức bao gồm quản lý nhân viên, lương thưởng và hợp đồng.

## Tổng quan

Hệ thống HRM cung cấp một nền tảng tập trung cho các chuyên gia nhân sự và quản trị viên để quản lý đội ngũ nhân sự một cách hiệu quả. Hệ thống sở hữu giao diện hiện đại được xây dựng bằng **Tailwind CSS** và backend mạnh mẽ tích hợp với **SQL Server**.

## Các tính năng chính

### Quản lý Nhân viên
- Quản lý toàn bộ vòng đời của nhân viên (Thêm, Xem, Cập nhật, Thôi việc).
- Hồ sơ chi tiết bao gồm thông tin cá nhân, thông tin liên lạc và trạng thái công việc.
- Phân chia phòng ban và sơ đồ tổ chức.

### Quản lý Hợp đồng
- Quản lý các loại hợp đồng khác nhau (Thử việc, Chính thức, Thời vụ).
- Cấu hình lương cơ bản và hệ số lương.
- Theo dõi hiệu lực và ngày hết hạn của hợp đồng.

### Lương & Chấm công
- **Chấm công:** Theo dõi sự hiện diện hàng ngày của tất cả nhân viên.
- **Bảng lương tháng:** Tự động tính toán lương dựa trên lương cơ bản, hệ số và công làm việc.
- **Trạng thái thanh toán:** Giám sát và cập nhật trạng thái chi trả cho các bảng lương hàng tháng.

### Quản lý Phòng ban
- Tạo và quản lý các phòng ban trong tổ chức (VD: Nhân sự, Kế toán, IT).
- Điều chuyển nhân viên vào các phòng ban cụ thể.

### Báo cáo & Thống kê
- Dashboard phân tích dành cho quản lý nhân sự.
- Dữ liệu thống kê về cơ cấu nhân sự và chi phí lương.

### Phân quyền truy cập (RBAC)
- **Admin:** Cấu hình hệ thống và quản lý cấp cao.
- **Nhân sự (HR):** Quản lý vận hành nhân viên, hợp đồng và lương thưởng.
- **Nhân viên:** Truy cập thông tin cá nhân và các dịch vụ tự phục vụ cho nhân viên.

## Công nghệ sử dụng

- **Backend:** ASP.NET MVC (.NET Framework 4.7.2), C#
- **Database:** Microsoft SQL Server
- **Frontend:** HTML5, CSS3, JavaScript
- **Styling:** Tailwind CSS, Font Awesome, Google Fonts (Inter)
- **Design:** StarUML (Mô hình hóa logic/class/ERD)

## Cấu trúc dự án

- `human_resource_management/`: Dự án web chính.
  - `Areas/Admin/`: Trang quản trị và cài đặt hệ thống.
  - `Areas/HumanResource/`: Các hoạt động nhân sự cốt lõi (Nhân viên, Lương, Thống kê).
  - `Areas/Employee/`: Cổng thông tin cho nhân viên.
  - `Controllers/`: Logic xử lý của ứng dụng.
  - `Views/`: Giao diện người dùng.
  - `Models/`: Các thực thể dữ liệu và business logic.
- `_db.sql`: Script khởi tạo cấu trúc cơ sở dữ liệu.
- `Nhom_2_Lan_1.mdj`: File thiết kế StarUML.

## Cài đặt & Thiết lập

1. **Thiết lập Cơ sở dữ liệu:**
   - Mở SQL Server Management Studio (SSMS).
   - Chạy script `_db.sql` để tạo database `QuanLyNhanSu` và các bảng liên quan.

2. **Thiết lập Dự án:**
   - Mở file giải pháp `human_resource_management.sln` bằng **Visual Studio**.
   - Cập nhật chuỗi kết nối (connection string) trong `Web.config` để khớp với SQL Server cục bộ của bạn.
   - Khôi phục các gói NuGet (Phải chuột vào Solution > Restore NuGet Packages).

3. **Chạy ứng dụng:**
   - Nhấn `F5` hoặc nút **Start** trong Visual Studio để chạy ứng dụng trên IIS Express.

## Bản quyền

Dự án này được phát triển cho mục đích học tập trong khuôn khổ chương trình học tại NTU Học kỳ 1 (2025-2026).
