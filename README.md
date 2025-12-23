**Tổng Quan**

- Mục đích: Hướng dẫn cài đặt môi trường và sử dụng mô hình Transformer trong project.

**Yêu Cầu**

- Python >= 3.11
- Windows (hướng dẫn dưới đây dùng PowerShell/CMD)

**Cài Đặt Môi Trường**

- Tạo và kích hoạt virtual environment:

uv venv

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1   # PowerShell

.\.venv\Scripts\activate.bat    # CMD
```
```
uv sync

```

**Cấu trúc mô hình**

- Thư mục chứa mô hình: `models/`
- Ví dụ file mô hình có sẵn trong repository: `models/model_statedict-23-12-2025_15h06m.pth`

**Sử dụng với `transformer.ipynb`**

- Chạy các cell định nghĩa mô hình
- Load state_dict và dự đoán
- Lưu ý không cần chạy những cell về train hay test.

**Sử dụng với notebook VLSP `nlp-transformer-VLSP-v1-v2010c3d9978.ipynb`**

- (VI-EN) Lấy file .pt từ https://drive.google.com/file/d/1IHiffdr0yucKOTzOitb8b2emKD81XjWc/view về và copy vào folder models.
- (EN-VI) Lấy file .pt từ https://drive.google.com/file/d/1V8S3ZW3AKXDFwCEGxzC6qpbPiA263kFO/view về và copy vào folder models.
- Chạy tương tự như với 'transformer.ipynb'
**Nếu muốn train lại từ đầu**

- Chạy các file preprocess tương ứng cho 2 bài toán rồi chạy các cell 'transformer.ipynb', 'nlp-transformer-VLSP-v1-v2010c3d9978.ipynb' lần lượt.
- Chú ý: data raw đã được tải sẵn, có thể tự tải lại nhưng phải cung cấp key kaggle
```
