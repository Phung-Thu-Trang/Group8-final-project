# Group8-final-project
# 📊 Group-8 Project: IBM Stock Analysis Report
## 👥 Team Contribution

| Thành viên              | % Đóng góp | Mã sinh viên |
|-------------------------|------------|--------------|
| Phùng Thu Trang         | 17.5%      |    11226507  |
| Lê Thị Thanh Thủy       | 17.5%      |    11226230  |
| Nguyễn Thị Minh Khuê    | 17.5%      |    11223132  |
| Chu Thùy Linh           | 11.5%      |    11223349  |
| Phùng Thế Hiển          | 12%        |    11222278  |
| Lê Mạnh Đức             | 10%        |    11221362  |
| Đặng Thị Linh Chi       | 14%        |    11220948  |


## 💡 Mô tả dự án

Dự án này được xây dựng bằng Python với mục tiêu phân tích dữ liệu liên quan đến công ty và cổ phiếu của IBM, từ đó trực quan hóa , giúp xây dựng model dự đoán ngắn hạn phục vụ cho các nhà đầu tư đưa ra quyết định phù hợp với nhu cầu của mình.

Dự án bao gồm các bước chính:
- ✅ Đặt vấn đề & xác định mục tiêu
- ✅ Làm sạch và xử lý dữ liệu gốc
- ✅ Phân tích & trực quan hóa kết quả

> 🔧 **Công nghệ sử dụng**: Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook,Google Colab, PySpark, Numpy,...

---

## 🏗️ Cấu trúc thư mục
```
Group-8---project/
├── 📁 data/                        # Thư mục chứa dữ liệu
│   ├── 📁 raw/                     # Dữ liệu gốc ban đầu
│   │   ├── IBM.csv
│   └── 📁 processed/               # Dữ liệu đã được làm sạch
│       └── IBM_clean.csv
│
├── 📁 notebooks/                  # Các file Jupyter Notebook xử lý & phân tích
│   ├── data_processing.ipynb      # Xử lý, làm sạch dữ liệu
│   ├── model.ipynb                # Model dự đoán
│   └── visualize.ipynb            # Phân tích & trực quan hóa dữ liệu
│
├── README.md                     # Tài liệu mô tả dự án
└── requirements.txt              # Danh sách thư viện cần cài
```
---

## 🚀 Cách chạy dự án trên Google Colab

### Bước 1: Mở notebook từ GitHub trên Colab
Truy cập: https://colab.research.google.com

Chọn tab GitHub

Nhập đường dẫn repo:

```
https://github.com/Phung-Thu-Trang/Group8-final-project

```

### Bước 2: Chạy từng notebook theo thứ tự

data_processing.ipynb – tiền xử lý dữ liệu

visualize.ipynb – phân tích và trực quan hóa

model.ipynb – huấn luyện mô hình dự đoán

## 📈 Kết quả 

- ✅ Biểu đồ giá đóng cửa của IBM theo thời gian
- ✅ Biểu đồ phân phối lợi suất hàng ngày
- ✅ Ma trận tương quan giữa các biến
- ✅ Biểu đồ giá đóng cửa trung bình mỗi năm
- ✅ Biểu đồ khối lượng giao dịch trung bình theo tháng
- ✅ Biểu đồ Volume và Close Price của IBM theo thời gian
- ✅ Biểu đồ Khối lượng Giao dịch của IBM
- ✅ Biểu đồ Return vs Volatility (IBM) – Phân vùng rủi ro/lợi nhuận
- ✅ Đường trung bình động MA5 và MA10,MA20
- ✅ Chỉ báo RSI
- ✅ Chỉ báo MACD
- ✅ Biểu đồ Bollinger Bands
- ✅ Biểu đồ Stochastic Oscillator
- ✅ Biểu đồ Parabolic SAR
- ✅ Biểu đồ Actual and predict close price
- ✅ Biểu đồ Distribution of prediction errors on the test set
- ✅ Biểu đồ Residual Plot: Sai số theo giá thực tế
- ✅ Biểu đồ Bollinger Bands từ 2025 đến hết thời gian dự báo
- ✅ Biểu đồ MACD từ 2025 đến hết thời gian dự báo
