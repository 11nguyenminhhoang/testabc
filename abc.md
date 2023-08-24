# Tổng Quan về Kỳ Thi AZ-104: Quản Lý Máy Ảo và Dịch Vụ Container Trên Azure

Kỳ thi AZ-104 tập trung vào việc đánh giá kỹ năng và kiến thức về quản lý máy ảo, dịch vụ container, và các dịch vụ liên quan trên Microsoft Azure. Dưới đây là các phần chính của kỳ thi.

## 1. **Quản Lý Máy Ảo (Virtual Machines)**

### a. Xây dựng và Kết Nối đến Máy Ảo
   - Tạo máy ảo Windows và Linux.
   - Kết nối đến máy ảo thông qua RDP và SSH.

### b. Vấn đề Kết Nối và Gỡ Lỗi
   - Xử lý các vấn đề kết nối.
   - Cài đặt dịch vụ như Internet Information Services.

### c. Chi Phí và Loại Máy Ảo
   - Hiểu về chi phí liên quan.
   - Các loại máy ảo và sử dụng thích hợp.

### d. Quản Lý Đĩa và Mã Hóa
   - Thêm đĩa dữ liệu, dừng máy.
   - Mã hóa đĩa phía máy chủ và sử dụng Azure Key Vault.

### e. Tùy Chọn Mã Hóa và Xem Xét Nhanh
   - Mã hóa tập dữ liệu, ảnh chụp.
   - Sử dụng Azure Disk Encryption và tùy chọn mã hóa khác.

### f. Các Tùy Chọn Khởi Động và Chạy Lệnh
   - Boot Diagnostics, chạy lệnh.
   - Các khái niệm như Confidential Computing và Azure Dedicated Host.

### g. Tính Sẵn Có và Quy Mô
   - Availability Sets, Zones.
   - Quy mô máy ảo và điều kiện quy mô.

### h. Hiểu và Sử Dụng Hình Ảnh Máy Ảo
   - Tạo và sử dụng hình ảnh chuyên biệt và tổng quát.

## 2. **Dịch Vụ Web và Container Azure**

### a. Azure Web Apps
   - Tạo và cấu hình Azure Web Apps.
   - Logging, Deployment Slots, và Tự Động Quy Mô.

### b. Azure Container Services
   - Cần thiết cho container và Docker.
   - Azure Container Registry và Instances.
   - Azure Container Apps và Azure Kubernetes.

### c. Lưu Trữ Persistent Trong Azure Kubernetes
   - Sử dụng đĩa và chia sẻ tệp.

## **Kết Luận**

Kỳ thi AZ-104 cung cấp một cái nhìn toàn diện về việc quản lý máy ảo và dịch vụ container trên Azure. Các chủ đề bao gồm cả việc xây dựng và quản lý máy ảo, cài đặt và cấu hình dịch vụ web và container, và các khía cạnh liên quan khác. Việc vượt qua kỳ thi này sẽ chứng minh kỹ năng và hiểu biết về các công nghệ và dịch vụ Azure quan trọng này.

***
#### 1a. Xây dựng và Kết Nối đến Máy Ảo

**Xây dựng Máy Ảo**:
- **Tạo Máy Ảo Windows và Linux**: Trong Azure, việc tạo máy ảo (VM) Windows hoặc Linux là một quá trình đơn giản thông qua Azure Portal hoặc Azure CLI.
- **Chọn Kích Thước và Hình Ảnh**: Cần lựa chọn kích thước VM phù hợp với yêu cầu hiệu suất và ngân sách. Hình ảnh OS cũng cần được xác định.

**Kết Nối đến Máy Ảo**:
- **RDP cho Windows**: Remote Desktop Protocol (RDP) được sử dụng để kết nối đến VM Windows. Cần mở cổng 3389 trong NSG.
- **SSH cho Linux**: Secure Shell (SSH) là phương pháp kết nối đến VM Linux. Cần mở cổng 22.

**Ứng Dụng Thực Tế**:
- Xây dựng môi trường phát triển hoặc kiểm thử nhanh chóng.
- Triển khai ứng dụng trên môi trường ảo hóa.
- Quản lý và điều chỉnh tài nguyên dễ dàng theo yêu cầu.

**Điểm Cần Lưu Ý**:
- An ninh: Cần thiết lập NSG và bảo mật cổng kết nối một cách hợp lý.
- Chi phí: Lựa chọn kích thước VM đúng cách để kiểm soát chi phí.
- Backup và Khôi Phục: Cần cân nhắc giải pháp sao lưu và khôi phục dữ liệu.

