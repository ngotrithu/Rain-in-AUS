# Rain-in-AUS
## Mô tả:
- Bộ dữ liệu này chứa các quan sát trong vòng 10 năm từ nhiều địa điểm khác nhau của nước Úc. `RainTomorrow` là biến mục tiêu, `yes` có nghĩa là ngày mai trời có mưa và lượng mưa lớn hơn 1mm, ngược lại là giá trị `no` thể hiện ngày mai trời không có mưa.
## Mục đích:
- Dự báo xem liệu ngày mai có mưa hay không bằng cách huấn luyện các mô hình phân loại dựa trên biến mục tiêu là `RainTomorrow`.
## Techniques:
- Handle Datetime variables
- Handle missing values
- Detecting and handle Outliers (IQR Range)
- One-Hot Encoder
- Feature Scaling
- Handle Imbalanced Dataset - SMOTE()
- Build Models
- Model Selection
- RandomizedSearchCV
## Modeling
- Logistic Regression
- Decision Tree
- Random Forest
- LightGBM
- Catboost
- XGBoost

=> Mô hình LightGBM cho độ chính xác tốt nhất 86.15% và tổng thời gian huấn luyện thấp nhất. Sau khi tiến hành `RandomizedSearchCV` độ chính xác của mô hình đã được cả thiện từ 86.15% lên 88.93 lên 2.78% (một sự cải thiện tương đối tốt). Nên chúng ta sẽ chọn mô hình LightGBM với các tham số đã tìm được để giải quyết cho bài toán này!
