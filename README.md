# Dự án Tiền xử lý và Phân tích Dữ liệu

Dự án này tập trung vào việc khám phá, tiền xử lý và chuẩn bị loại dữ liệu ảnh.



## Mô tả tập dữ liệu

### Dữ liệu ảnh X-quang Ngực (Viêm phổi)

* **Tên:** [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
* **Tổng quan:** Tập dữ liệu chứa **5,863 ảnh X-quang ngực** (JPEG) được thu thập từ bệnh nhi (1-5 tuổi) tại *Guangzhou Women and Children’s Medical Center, China*.
* **Phân loại:** Dữ liệu được chia thành hai lớp để phân loại nhị phân:
    * `PNEUMONIA` (Viêm phổi): 4,273 ảnh
    * `NORMAL` (Bình thường): 1,584 ảnh
* **Cấu trúc:** Dữ liệu được chia sẵn thành 3 tập: `train/`, `test/`, và `val/`.
* **Lý do lựa chọn:** Đây là dữ liệu y khoa trực quan nhưng chứa nhiều nhiễu (độ sáng không đồng đều, tương phản thấp). Dự án này khám phá các kỹ thuật tiền xử lý (chuẩn hoá, CLAHE, phát hiện biên) để cải thiện độ rõ nét và làm nổi bật các cấu trúc phổi.


## Hướng dẫn chạy Notebooks

### 1. Yêu cầu về môi trường

Dự án này yêu cầu Python 3.x và các thư viện được liệt kê trong file `requirements.txt`.

**Bước 1: (Tùy chọn) Tạo và kích hoạt môi trường ảo**
```bash
# Tạo môi trường ảo
python -m venv venv

# Kích hoạt môi trường (Windows)
.\venv\Scripts\activate

# Kích hoạt môi trường (macOS/Linux)
source venv/bin/activate
```
**Bước 2: Cài đặt các thư viện cần thiết**
```bash
pip install -r requirements.txt
```

### Hướng dẫn chạy chi tiết

1. Khởi động Jupyter Lab hoặc Jupyter Notebook từ thư mục gốc của dự án:
   ```bash
   jupyter lab
   ```

#### Xử lý ảnh (Image Processing)

1. Tải dataset theo nguồn ở dưới, giải nén và để vào thư mục `data/images`. Sẽ có dạng `data/images/chest_xray`
2. Mở thư mục `notebooks`.
2. Chọn kernel chạy cho đúng đường dẫn python của môi trường ảo (venv) đã tạo ở bước trên.
3. Chạy các file `.ipynb` theo thứ tự đã đánh số.

## Tài nguyên bên ngoài

**Dataset Ảnh:**
  * Kaggle: https://drive.google.com/drive/folders/1RpmFLvLxbpw5nr5aKZQiBjWLCr8DyAIh?usp=drive_link
  * Nguồn gốc: https://data.mendeley.com/datasets/rscbjbr9sj/2

