# 🛒 Brazilian E-Commerce Big Data Analytics (PySpark)

## 📌 Giới thiệu

Dự án này xây dựng một hệ thống phân tích dữ liệu thương mại điện tử quy mô lớn dựa trên **Apache Spark (PySpark)**, nhằm:

* Phân tích hành vi khách hàng
* Xây dựng hệ thống gợi ý sản phẩm
* Ứng dụng nhiều thuật toán Machine Learning trên dữ liệu lớn

Dataset sử dụng: **Olist Brazilian E-Commerce (Kaggle)**

---

## 👥 Thành viên

* Nguyễn Đỗ Ngọc Hân – 23126013 (Leader)
* Cao Khanh – 23126016
* Đinh Đoàn Quang Mẫn – 23126026
* Thái Công Thanh Tú – 23126052

---

## 📂 Dataset

Nguồn dữ liệu:
🔗 https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Dataset bao gồm nhiều bảng liên quan đến:

* Customers
* Orders
* Products
* Payments
* Reviews
* Sellers

---

## ⚙️ Công nghệ sử dụng

* **Apache Spark (PySpark)**
* **Spark MLlib**
* Python (Pandas, NumPy)
* Visualization: Matplotlib, Seaborn, Plotly
* Google Colab + Google Drive
* Kaggle API

---

## 🚀 Pipeline tổng thể

### 1. Data Preparation

* Load dữ liệu từ nhiều file CSV
* Data cleaning (missing values, duplicates)
* Join các bảng dữ liệu
* Feature Engineering:

  * RFM (Recency - Frequency - Monetary)
  * TF-IDF (text feature)
* Xây dựng Pipeline với Spark ML

---

### 2. Machine Learning Models

Dự án triển khai nhiều nhóm thuật toán:

#### 📌 Classification

* Dự đoán hành vi hoặc phân loại khách hàng

#### 📌 Regression

* Dự đoán giá trị liên tục (ví dụ: giá, doanh thu)

#### 📌 Clustering

* Phân nhóm khách hàng (Customer Segmentation)

#### 📌 Recommendation System

* ALS (Collaborative Filtering)
* Gợi ý sản phẩm cho người dùng

#### 📌 Association Rules

* FP-Growth
* Khai phá luật kết hợp (Market Basket Analysis)

---

### 3. Evaluation & Optimization

* Chi-Square Test (feature selection)
* Hyperparameter Tuning
* So sánh mô hình (Model Comparison)

---

## 🛠️ Cài đặt môi trường

### 1. Cài đặt dependencies

```bash
pip install pyspark==3.5.7 pandas matplotlib seaborn plotly kaggle
```

### 2. Yêu cầu Java

```bash
apt-get install openjdk-17-jdk-headless
```

---

## 📥 Tải dữ liệu từ Kaggle

1. Upload file `kaggle.json`
2. Cấu hình:

```bash
mkdir -p /root/.kaggle
cp kaggle.json /root/.kaggle/
chmod 600 /root/.kaggle/kaggle.json
```

3. Download dataset:

```bash
kaggle datasets download -d olistbr/brazilian-ecommerce
unzip brazilian-ecommerce.zip
```

---

## ▶️ Cách chạy project

* Mở notebook `.ipynb` bằng **Google Colab**
* Mount Google Drive
* Chạy từng cell theo thứ tự:

  1. Setup environment
  2. Load data
  3. Data preprocessing
  4. Training models
  5. Evaluation

---

## 📊 Kết quả đạt được

* Xây dựng pipeline xử lý dữ liệu lớn với Spark
* Triển khai nhiều mô hình ML trên cùng dataset
* Xây dựng hệ thống gợi ý sản phẩm
* Phân tích hành vi khách hàng hiệu quả

---

## 📌 Điểm nổi bật

* Sử dụng **Big Data framework (Spark)** thay vì Pandas truyền thống
* Áp dụng **nhiều thuật toán ML trong cùng project**
* Có **pipeline hoàn chỉnh từ data → model → evaluation**

---

## 📎 Ghi chú

* Project được thiết kế để chạy trên **Google Colab**
* Cần GPU/High RAM để xử lý nhanh hơn (khuyến nghị)

---

## ⭐ Future Work

* Triển khai real-time recommendation
* Xây dựng dashboard (Streamlit / Power BI)
* Tối ưu performance với Spark cluster

---

## 📬 Liên hệ

Nếu bạn có câu hỏi hoặc góp ý, vui lòng liên hệ nhóm phát triển.


