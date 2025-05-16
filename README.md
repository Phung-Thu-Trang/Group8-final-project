# Group8-final-project
# 📊 Group-8 Project: IBM Stock Analysis Report
## 👥 Team Contribution

| Thành viên              | % Đóng góp | Mã sinh viên |
|-------------------------|------------|--------------|
| Phùng Thu Trang         | 14.2%      |    11226507  |
| Lê Thị Thanh Thủy       | 14.2%      |    11226230  |
| Nguyễn Thị Minh Khuê    | 14.2%      |    11223132  |
| Chu Thùy Linh           | 14.2%      |    11223349  |
| Phùng Thế Hiển          | 14.2%      |    11222278  |
| Lê Mạnh Đức             | 14.2%      |    11221362  |
| Đặng Thị Linh Chi       | 14.2%      |    11220948  |


## 💡 Mô tả dự án

Dự án này được xây dựng bằng Python với mục tiêu phân tích dữ liệu liên quan đến công ty và cổ phiếu của IBM, từ đó trực quan hóa , giúp xây dựng model dự đoán ngắn hạn phục vụ cho các nhà đầu tư đưa ra quyết định phù hợp với nhu cầu tài chính của mỗi cá nhân .

Dự án bao gồm các bước chính:

- ✅ Tìm hiểu về công ty & tiềm năng của cổ phiếu IBM

- ✅ Làm sạch và xử lý dữ liệu gốc

   📁 Mục tiêu
  
Notebook này thực hiện tiền xử lý dữ liệu chứng khoán IBM từ file CSV bằng cách sử dụng PySpark trong môi trường Google Colab, bao gồm:

  Kiểm tra và xử lý giá trị thiếu (null)

  Chuyển đổi định dạng ngày

  Loại bỏ dữ liệu lỗi

  Chuyển đổi dữ liệu sang pandas và lưu file kết quả sạch để tải về

- ✅ Model dự đoán ngắn hạn

  🧠 Huấn luyện mô hình Ridge Regression
  
Dữ liệu sau khi xử lý được chia theo tỷ lệ 80:20:

  80% dữ liệu đầu tiên được sử dụng để huấn luyện mô hình Ridge Regression, trong đó các chỉ báo kỹ thuật (như MA, RSI, MACD, v.v.) được sử dụng làm biến đầu vào 
  (features).

  20% dữ liệu còn lại được dùng để đánh giá hiệu suất mô hình, thông qua việc so sánh giá trị dự đoán với giá trị thực tế của giá đóng cửa.

  Nếu sai số dự đoán nằm trong ngưỡng chấp nhận được (ví dụ như RMSE thấp, R² cao), mô hình sẽ được sử dụng để dự báo giá đóng cửa cho 20 ngày tiếp theo chưa có 
  trong tập dữ liệu ban đầu.


- ✅ Phân tích & trực quan hóa kết quả

  📊 Trực quan hóa dữ liệu
  
Phần này thực hiện trực quan hóa toàn diện dữ liệu giá cổ phiếu IBM nhằm hỗ trợ phân tích kỹ thuật và đánh giá rủi ro:

  Biểu đồ giá đóng cửa theo thời gian và phân phối lợi suất hàng ngày

  Ma trận tương quan giữa các biến tài chính như giá mở cửa, đóng cửa, cao nhất, thấp nhất và khối lượng

  Biểu đồ trung bình năm/tháng cho giá và khối lượng giao dịch

  Biểu đồ kết hợp Volume và Close Price

  Phân tích Return vs. Volatility, xác định vùng rủi ro/lợi nhuận

  Trực quan các chỉ báo kỹ thuật gồm:

  Đường trung bình động (MA5, MA10, MA20)

  RSI (Relative Strength Index)

  MACD và đường tín hiệu

  Bollinger Bands

  Parabolic SAR

  Stochastic Oscillator (%K và %D)

Các biểu đồ giúp nhận diện xu hướng, tín hiệu mua bán và mức độ biến động của cổ phiếu trong từng giai đoạn cụ thể.


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
