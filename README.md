# textDetection use YOLOv8
## Training with Yolov8
    - Tham số training
    - Kích thước 1024
    - Agument: Gộp các ảnh lại với nhau

## Đánh giá
    - Mectric: mAp95

## So sánh version
    - Precision

## Test
    - Hiển thị từ 50 - 100 ảnh.
    - Xây dựng biểu đồ
## 1. Dataset

- Cấu trúc thư mục

```
|--dataset
    |--train
      |-- images
          |-- 000000.jpg
          |-- 000001.jpg
                .
                .
          |-- xxxxxx.jpg
      |-- labels
          |-- 000000.txt
          |-- 000001.txt
                .
                .
          |-- xxxxxx.txt
    |--valid
      |-- images
          |-- 100000.jpg
          |-- 100001.jpg
                .
                .
          |-- xxxxxx.jpg
      |-- labels
          |-- 100000.txt
          |-- 100001.txt
                .
                .
      |-- xxxxxx.txt
```
