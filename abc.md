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
***
#### 1b. Vấn đề Kết Nối và Gỡ Lỗi

**Vấn đề Kết Nối**:
- **Xác Định Vấn đề**: Cần phát hiện nhanh chóng liệu vấn đề kết nối đến VM có do bảo mật, cấu hình mạng, hay dịch vụ OS.
- **Sử dụng Network Watcher**: Azure Network Watcher giúp theo dõi, gỡ lỗi, và điagnostic vấn đề mạng.

**Gỡ Lỗi và Cài Đặt Dịch Vụ**:
- **Cài đặt Internet Information Services (IIS)**: Trong môi trường Windows, IIS là dịch vụ web server phổ biến, cần biết cách cài đặt và cấu hình.
- **Gỡ Lỗi Ứng Dụng và Hệ Thống**: Sử dụng công cụ như Azure Monitor và Log Analytics để gỡ lỗi ứng dụng và hệ thống.

**Ứng Dụng Thực Tế**:
- Đảm bảo tính sẵn sàng và hiệu suất của ứng dụng và dịch vụ.
- Tìm hiểu và giải quyết nhanh chóng các vấn đề kết nối và lỗi hệ thống.

**Điểm Cần Lưu Ý**:
- **Bảo Mật**: Đảm bảo rằng mọi cấu hình mạng và bảo mật đều đúng để tránh rủi ro.
- **Hiệu Suất**: Gỡ lỗi hiệu suất có thể đòi hỏi hiểu biết sâu về OS và ứng dụng.
- **Tài Liệu**: Lưu trữ tài liệu về cấu hình và các biện pháp gỡ lỗi để giúp trong tương lai.
***
#### 1c. Chi Phí và Loại Máy Ảo

**Chi Phí Liên Quan đến Máy Ảo**:
- **Hiểu về Chi Phí**: Việc tạo và duy trì máy ảo trên Azure sẽ đòi hỏi chi phí. Các yếu tố bao gồm kích thước VM, thời gian hoạt động, và lưu trữ.
- **Azure Cost Management**: Công cụ này giúp theo dõi chi phí và hiểu rõ hơn về cách phân bổ ngân sách.

**Loại Máy Ảo**:
- **Các Loại VM**: Azure cung cấp nhiều loại VM, từ loại tối ưu CPU, RAM, đến loại có hiệu suất đồ họa cao.
- **Lựa Chọn Phù Hợp**: Việc lựa chọn loại VM phù hợp sẽ ảnh hưởng đến hiệu suất và chi phí.

**Ứng Dụng Thực Tế**:
- **Phù Hợp Cho Nhu Cầu Kinh Doanh**: Lựa chọn loại VM phù hợp giúp đảm bảo hiệu suất và tính khả dụng trong khi kiểm soát chi phí.
- **Dự Toán và Theo Dõi Chi Phí**: Quản lý chi phí VM là một phần quan trọng của việc quản lý dịch vụ đám mây.

**Điểm Cần Lưu Ý**:
- **Tối Ưu Hóa Chi Phí**: Để tối ưu hóa chi phí, cần hiểu rõ về cấu trúc giá của Azure VM và lựa chọn đúng loại VM.
- **Hiệu Suất và Độ Tin Cậy**: Cần cân nhắc giữa chi phí và yêu cầu hiệu suất, đồng thời xác định các yếu tố khác như độ tin cậy và tính linh hoạt.
- **Quản Lý Chi Phí**: Sử dụng các công cụ như Azure Cost Management để theo dõi và quản lý chi phí liên quan đến VM.
***
#### 1d. Quản Lý Đĩa và Mã Hóa

**Quản Lý Đĩa**:
- **Thêm Đĩa Dữ Liệu**: Có thể thêm các đĩa dữ liệu vào VM để mở rộng lưu trữ.
- **Dừng Máy**: Hiểu về hành vi của VM khi dừng, như chi phí và tình trạng đĩa.

**Mã Hóa Đĩa**:
- **Server-Side Encryption**: Sử dụng Azure Disk Encryption để mã hóa đĩa.
- **Azure Key Vault**: Sử dụng để quản lý khóa mã hóa.

**Ứng Dụng Thực Tế**:
- **Bảo Mật Dữ Liệu**: Mã hóa đĩa giúp bảo vệ dữ liệu.
- **Quản Lý Lưu Trữ**: Thêm đĩa dữ liệu cho phép quản lý lưu trữ linh hoạt.

**Điểm Cần Lưu Ý**:
- **Quản Lý Khóa**: Quản lý khóa mã hóa là một yếu tố quan trọng trong bảo mật.
- **Hiệu Suất**: Cân nhắc giữa hiệu suất và bảo mật khi mã hóa đĩa.
***
#### 1e. Tùy Chọn Mã Hóa và Xem Xét Nhanh

**Tùy Chọn Mã Hóa**:
- **Mã Hóa Tập Dữ Liệu, Ảnh Chụp**: Sử dụng mã hóa để bảo vệ tập dữ liệu và ảnh chụp.
- **Azure Disk Encryption và Tùy Chọn Khác**: Hiểu về các tùy chọn mã hóa khác nhau.

**Xem Xét Nhanh về Tùy Chọn Mã Hóa**:
- **Tổng Quan Các Tùy Chọn**: Hiểu rõ các tùy chọn và lựa chọn tốt nhất cho nhu cầu cụ thể.

**Ứng Dụng Thực Tế**:
- **Bảo Mật**: Sử dụng mã hóa để bảo vệ dữ liệu quan trọng.
- **Tuân Thủ**: Đảm bảo tuân thủ các tiêu chuẩn bảo mật và quy định.

**Điểm Cần Lưu Ý**:
- **Lựa Chọn Đúng Tùy Chọn Mã Hóa**: Tùy chọn mã hóa phù hợp sẽ phụ thuộc vào yêu cầu bảo mật và tuân thủ.
***
#### 1g. Tính Sẵn Có và Quy Mô

**Tính Sẵn Có**:
- **Availability Sets**: Sử dụng để cải thiện tính sẵn còn và độ tin cậy.
- **Availability Zones**: Cung cấp tính sẵn còn ở cấp độ khu vực.

**Quy Mô Máy Ảo**:
- **Virtual Machine Scale Sets**: Quy mô máy ảo theo nhu cầu.
- **Điều Kiện Quy Mô**: Thiết lập điều kiện để tự động quy mô.

**Ứng Dụng Thực Tế**:
- **Độ Tin Cậy**: Cải thiện tính sẵn còn và khả năng phục hồi sau lỗi.
- **Linh Hoạt**: Quy mô theo nhu cầu, giúp quản lý hiệu quả nguồn lực.

**Điểm Cần Lưu Ý**:
- **Cân Nhắc Chi Phí**: Tính sẵn còn cao có thể tăng chi phí.
- **Cấu Hình Đúng Cách**: Cần cấu hình đúng để đảm bảo tính sẵn còn và quy mô hiệu quả.
***

