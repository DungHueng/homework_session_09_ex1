# BÀI 1: KIỂM TRA CÀI ĐẶT DOCKER ENGINE VÀ CHẠY CONTAINER HELLO-WORLD

## 1. Mục tiêu

- Kiểm tra phiên bản Docker CLI bằng lệnh `docker version`.
- Kiểm tra trạng thái Docker Engine và Docker Daemon bằng lệnh `docker info`.
- Khởi chạy container đầu tiên bằng image `hello-world`.
- Kiểm tra khả năng kết nối tới Docker Daemon mà không cần sử dụng tiền tố `sudo`.

## 2. Môi trường thực hành

- **Hệ điều hành:** Windows 11.
- **Terminal:** Windows CMD.
- **Docker:** Docker Desktop.
- **Docker CLI version:** 29.8.0.
- **Docker context:** `desktop-linux`.
- **Thư mục bài tập:** `D:\PTIT-IT_209\Session_09\Bai_01`.

## 3. Nội dung thực hiện

### 3.1. Kiểm tra phiên bản Docker

**Lệnh thực hiện:**

```cmd
docker version
```

**Kết quả:**

- Docker Client Version: `29.8.0`.
- API Version: `1.56`.
- Hệ điều hành Client: `windows/amd64`.
- Docker Context: `desktop-linux`.

Lệnh `docker version` hiển thị thông tin phiên bản Docker CLI và Docker Engine. Sau khi Docker Desktop được khởi động, Client có thể kết nối thành công tới Server.

### 3.2. Kiểm tra thông tin Docker Engine

**Lệnh thực hiện:**

```cmd
docker info
```

**Kết quả:**

- Server Version: `29.8.0`.
- Containers: `2`.
- Containers Running: `0`.
- Containers Stopped: `2`.
- Images: `2`.
- Operating System: `Docker Desktop`.
- Architecture: `x86_64`.
- CPUs: `12`.
- Total Memory: `7.557 GiB`.
- Kernel: `6.18.33.2-microsoft-standard-WSL2`.

**Nhận xét:**

Lệnh `docker info` trả về đầy đủ thông tin Client và Server. Docker Daemon đã hoạt động và sẵn sàng tiếp nhận các lệnh quản lý container.

### 3.3. Chạy container Hello-World

**Lệnh thực hiện:**

```cmd
docker run hello-world
```

**Kết quả:**

```text
Hello from Docker!
This message shows that your installation appears to be working correctly.
```

Docker đã tải image `hello-world` từ Docker Hub, tạo container và chạy chương trình kiểm tra. Container trả về thông báo thành công trên Terminal.