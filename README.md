# 🚗 TrafficXY - Hệ thống giám sát giao thông thông minh (Backend)

> **TrafficXY** là hệ thống giám sát giao thông hiện đại, sử dụng AI để nhận diện phương tiện vi phạm, cung cấp thông tin chi tiết.

---

## 🌟 Tính năng Backend

✅ **Nhận diện phương tiện vi phạm** từ camera giám sát.  
✅ **Xử lý hình ảnh bằng AI** với GPU tăng tốc.  
✅ **Lưu trữ và truy vấn dữ liệu xe vi phạm**.  

---

## 🛠️ Hướng dẫn cài đặt Backend trên Windows

> **🔹 Yêu cầu hệ thống:** Windows 10/11, RAM tối thiểu **8GB**, VGA NVIDIA tối thiểu **8GB**, Python **3.9+**, Anaconda.

### 📌 1️⃣ Cài đặt **Visual Studio Code**

🖥️ Tải và cài đặt **VS Code** tại: [🔗 VS Code](https://code.visualstudio.com/)  
✨ **Extensions gợi ý:**
- 🟢 `Python` (hỗ trợ lập trình Python)
- 🟢 `Pylance` (cung cấp gợi ý mã nguồn thông minh)
- 🟢 `REST Client` (kiểm thử API nhanh chóng)

### 📌 2️⃣ Cài đặt **Anaconda**

🐍 **Tải và cài đặt Anaconda** tại: [🔗 Anaconda](https://www.anaconda.com/)  
📌 **Kiểm tra cài đặt thành công:**
```sh
conda --version
```

### 📌 3️⃣ Clone dự án và tạo môi trường ảo **trafficx**

📥 **Clone repository từ GitHub:**
```sh
git clone https://github.com/MinhPhambk/TrafficX_Backend.git
cd TrafficX_Backend
```

🐍 **Tạo và kích hoạt môi trường ảo:**
```sh
conda create -n trafficx python=3.9 -y
conda activate trafficx
```

### 📌 4️⃣ Cài đặt các thư viện cần thiết

📦 **Cài đặt dependencies từ file requirements.txt:**
```sh
pip install -r requirements.txt
```

---

## 🖥️ Hướng dẫn cài đặt trên máy có GPU NVIDIA

> **🔹 Yêu cầu GPU tối thiểu:** NVIDIA GTX **1650** trở lên, hỗ trợ **CUDA 11+**.

### 📌 5️⃣ Kiểm tra GPU và CUDA

🚀 **Kiểm tra xem hệ thống đã nhận diện GPU NVIDIA chưa:**
```sh
nvidia-smi
```

🔍 **Kiểm tra phiên bản CUDA đang sử dụng:**
```sh
nvcc --version
```

### 📌 6️⃣ Cài đặt thư viện hỗ trợ GPU

⚡ **Cài đặt PyTorch với CUDA:**
```sh
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

### 📌 7️⃣ Chạy hệ thống Backend

🚀 **Khởi động dự án:**
```sh
python StartProject.py
```

---

## ☁️ Hướng dẫn chạy trên Google Colab (nếu không có GPU cục bộ)

### 📌 5️⃣ Cấu hình môi trường trên Google Colab

🛠️ **Bước 1:** Mở [🔗 Google Colab](https://colab.research.google.com/)  
🖥️ Chọn "Runtime" → "Change runtime type" → **Chọn GPU**  

🌍 **Bước 2:** Clone repository và cài đặt thư viện
```sh
!git clone https://github.com/MinhPhambk/TrafficX_Backend.git
%cd TrafficX_Backend
!pip install -r requirements.txt
```

### 📌 6️⃣ Chạy hệ thống trên Google Colab

🚀 **Khởi động hệ thống trên Google Colab:**
```sh
!python StartProject.py
```

📌 **Lưu ý:** Khi chạy trên Colab, cần đảm bảo phiên bản PyTorch tương thích với GPU Colab. Nếu gặp lỗi, thử chạy:
```sh
!pip install torch torchvision torchaudio
```

---

## 🐳 Cài đặt và chạy hệ thống bằng Docker

### 📌 1️⃣ Cài đặt Docker
🖥️ Tải và cài đặt **Docker Desktop** tại: [🔗 Docker](https://www.docker.com/products/docker-desktop/)  
📌 **Kiểm tra cài đặt thành công:**
```sh
docker --version
```

### 📌 2️⃣ Clone dự án và build Docker image
📥 **Clone repository từ GitHub:**
```sh
git clone https://github.com/MinhPhambk/TrafficX_Backend.git
cd TrafficX_Backend
```

🐳 **Build Docker image:**
```sh
docker build -t trafficx-backend .
```

### 📌 3️⃣ Chạy hệ thống bằng Docker
🚀 **Khởi động container:**
```sh
docker run --gpus all -p 8000:8000 --name trafficx-container trafficx-backend
```

📌 **Dừng container:**
```sh
docker stop trafficx-container
```

📌 **Xóa container:**
```sh
docker rm trafficx-container
```

📌 **Xóa image:**
```sh
docker rmi trafficx-backend
```

---

## 🚀 Hỗ trợ & Liên hệ

📧 **Email:** [phamngocminh1230@gmail.com](mailto:phamngocminh1230@gmail.com)  
🐞 **Báo lỗi:** [🔗 Issues trên GitHub](https://github.com/MinhPhambk/TrafficX_Backend/issues)  

🎯 **TrafficX - Công nghệ giao thông thông minh, an toàn hơn mỗi ngày!** 🚦


