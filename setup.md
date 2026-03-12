# Setup Guide - Hệ Thống Nhận Diện Vật Cản

## Yêu Cầu Hệ Thống

### Phần Cứng Tối Thiểu
- Bo mạch chính: Raspberry Pi 4 / Jetson Nano / máy tính
- Camera: USB Webcam hoặc Camera Module
- Cảm biến: HC-SR04 (Ultrasonic) hoặc LiDAR
- RAM: 4GB+
- Storage: 16GB+

### Phần Mềm
- Python 3.8+
- pip (Python package manager)
- Git

## Bước Cài Đặt

### 1. Cài Đặt Python và Pip
```bash
sudo apt-get update
sudo apt-get install python3 python3-pip python3-venv
```

### 2. Clone Repository
```bash
git clone https://github.com/nguyengiap2004/nhan-dien-vat-can.git
cd nhan-dien-vat-can
```

### 3. Tạo Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Cài Đặt Dependencies
```bash
pip install -r requirements.txt
```

### 5. Download YOLO Model
```bash
python3 -c \"from ultralytics import YOLO; YOLO('yolov8n.pt')\" 
```

### 6. Cấu Hình Cảm Biến
Chỉnh sửa config/sensor_config.yaml theo thiết bị của bạn