# 🔤 Training PaddleOCR with VinText 🇻🇳

> Notebook thực nghiệm huấn luyện và đánh giá **PaddleOCR** trên dữ liệu chữ tiếng Việt từ VinText, phục vụ bài toán OCR tài liệu/ảnh tiếng Việt.

---

## 📌 Giới thiệu

Training_PaddleOCR_with_Vintext tập trung vào quy trình chuẩn bị môi trường, dữ liệu, model và huấn luyện OCR bằng hệ sinh thái PaddlePaddle/PaddleOCR.

Toàn bộ quá trình được tổ chức trong một notebook lớn để có thể chạy trực tiếp trên Kaggle hoặc môi trường GPU tương tự.

---

## 🚀 Nội dung chính

- 📦 Cài đặt PaddlePaddle và PaddleOCR.
- 🇻🇳 Chuẩn bị dữ liệu OCR tiếng Việt từ VinText.
- 🧾 Chuyển đổi dữ liệu sang format phù hợp cho PaddleOCR.
- 🔠 Huấn luyện/đánh giá recognition model.
- 🔍 Thử nghiệm detection + recognition.
- 🧱 Thử nghiệm PPStructureV3 cho document parsing.
- 🖼️ Chạy inference trên dữ liệu test/PDF.
- 💾 Lưu checkpoint và kết quả để sử dụng lại.

---

## 🧠 Model / Pipeline được thử nghiệm

Trong notebook có cấu hình và thử nghiệm với các thành phần như:

- **PP-OCRv5 Mobile Recognition**
- **PP-OCRv5 Server Detection**
- **PPStructureV3**
- PaddlePaddle GPU
- PaddleOCR pipeline

Mục tiêu là đánh giá khả năng nhận dạng văn bản tiếng Việt và chuẩn bị model phù hợp cho các hệ thống OCR thực tế.

---

## 📂 Cấu trúc repository

~~~text
Training_PaddleOCR_with_Vintext/
├── train-paddleocr-vintext.ipynb   # Notebook huấn luyện / test chính
└── link.txt                        # Link dataset và tài liệu tham khảo
~~~

---

## 📂 Dataset

Nguồn dữ liệu được tham khảo từ VinText:

- VinText / dict-guided OCR:
  https://github.com/VinAIResearch/dict-guided

File link.txt trong repository lưu lại các nguồn dữ liệu và tài liệu PaddleOCR được dùng trong quá trình thử nghiệm.

---

## 🛠️ Công nghệ sử dụng

- 🐍 Python
- 📓 Jupyter Notebook / Kaggle
- 🔤 PaddleOCR
- ⚙️ PaddlePaddle
- 🧱 PPStructureV3
- 🎮 CUDA / GPU
- 🖼️ Computer Vision / OCR

Notebook có ghi nhận môi trường thử nghiệm PaddlePaddle 3.2.0 với GPU/CUDA tương ứng tại thời điểm thực hiện.

---

## ▶️ Cách chạy

### 1. Clone repository

~~~bash
git clone https://github.com/tttiuem2k3/Training_PaddleOCR_with_Vintext.git
cd Training_PaddleOCR_with_Vintext
~~~

### 2. Mở notebook

Mở file:

~~~text
train-paddleocr-vintext.ipynb
~~~

Khuyến nghị chạy trên:

- Kaggle Notebook có GPU.
- Google Colab có GPU.
- Máy local đã cài đúng PaddlePaddle GPU.

### 3. Chuẩn bị dataset

Tải VinText theo link trong link.txt và cập nhật đường dẫn dataset trong notebook theo môi trường đang sử dụng.

### 4. Chạy tuần tự các cell

Notebook bao gồm các bước cài thư viện, kiểm tra GPU, chuẩn bị dữ liệu, tải model, train và inference. Nên chạy theo đúng thứ tự để tránh sai version hoặc đường dẫn.

---

## 📚 Tham khảo

- [PaddleOCR Documentation](https://www.paddleocr.ai/)
- [PPStructureV3](https://www.paddleocr.ai/latest/en/version3.x/pipeline_usage/PP-StructureV3.html)
- [VinAIResearch/dict-guided](https://github.com/VinAIResearch/dict-guided)

---

## 🎯 Mục đích sử dụng

Kết quả từ notebook này có thể được dùng để:

- So sánh model OCR tiếng Việt.
- Fine-tune recognition model cho dữ liệu riêng.
- Tạo checkpoint cho OCR backend.
- Đánh giá detection/recognition trước khi đưa vào API production.

---

## 📞 Liên hệ

- 📧 Email: tttiuem2k3@gmail.com
- 👥 LinkedIn: [Thịnh Trần](https://www.linkedin.com/in/thinh-tran-04122k3/)
- 💬 Zalo / Phone: +84 329966939 | +84 336639775

---
