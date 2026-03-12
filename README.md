# Hệ Thống Nhận Diện Vật Cản cho Xe Tự Hành (Obstacle Detection System)

Hệ thống tích hợp YOLO (Computer Vision) và LiDAR/Cảm Biến Siêu Âm (Distance Sensing) để nhận diện và mô tả vật cản cho xe tự hành.

## 📋 Mục Tiêu
- Nhận diện các vật cản sử dụng YOLO
- Đo khoảng cách bằng cảm biến siêu âm/LiDAR
- Xác định loại và đặc điểm vật cản
- Điều khiển xe tránh vật cản

## 🏗️ Cấu Trúc Dự Án
nhan-dien-vat-can/
├── README.md
├── requirements.txt
├── setup.md
├── config/
│   ├── config.yaml
│   └── sensor_config.yaml
├── src/
│   ├── __init__.py
│   ├── yolo_detector.py
│   ├── sensor_reader.py
│   ├── data_processor.py
│   └── main.py
├── models/
├── tests/
│   ├── test_yolo.py
│   └── test_sensor.py
├── logs/
├── output/
└── docs/
    ├── INSTALLATION.md
    ├── USAGE.md
    └── ARCHITECTURE.md

## 🚀 Bắt Đầu Nhanh
```bash
git clone https://github.com/nguyengiap2004/nhan-dien-vat-can.git
cd nhan-dien-vat-can
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 src/main.py
```

## 🔧 Công Nghệ
- YOLO v8
- OpenCV
- Python 3.8+
- Raspberry Pi GPIO (optional)

## 📚 Tài Liệu
- Installation Guide
- Usage Guide
- Architecture Documentation