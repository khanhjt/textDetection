Dùng YOLOv8 để huấn luyện mô hình nhận diện văn bản. Mô hình được áp dụng vào việc số hóa tài liệu sau này
# Run
## Cài các thư viện 
```
pip install -r requirements.txt

```
Làm theo các bước ở notebook main.ipynb

# Báo cáo
    - Tham số training
    - Kích thước 1024
    - Augument: Gộp các ảnh lại với nhau
    - Mectric: mAp95
    - Precision
    - Hiển thị từ 50 - 100 ảnh.
    - Xây dựng biểu đồ
## 1. Dataset
- Dùng dataset của VinAI - coco fomat
- Data có 2000 ảnh, 
- Xử lý và làm giàu đúng fomat input yolov8.
- Cấu trúc thư mục

```
|--datasets
    |--train
      |-- images
      |-- labels

    |--test
      |-- images
      |-- labels

    |--val
      |-- images
      |-- labels

```
## Đánh giá
### 1. epochs = 3, batch = 16, imgsz = 1024
### 2. epochs = 5, batch = 16, imgsz = 1024
### 3. epochs = 20, batch = 8, imgsz = 1024 
 - yolov8s.pt
 - (Tesla P40, 24446MiB)
 - 168 layers, 3005843 parameters, 0 gradients, 8.1 GFLOPs
 - Speed: 0.8ms preprocess, 51.1ms inference, 0.0ms loss, 2.8ms postprocess per image
 - 
