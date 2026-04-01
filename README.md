# FCL_Mediation

## Mô tả dự án

Dự án này thực hiện phân tích dữ liệu nghiên cứu về **Cơ chế thực thi đằng sau sự hài lòng của khách hàng trong dịch vụ trạm hàng container (Container Freight Station) dựa trên bằng chứng từ hoạt động logistics cảng biển**.

## Mục tiêu nghiên cứu

- Đánh giá độ tin cậy của các thang đo khảo sát thông qua Cronbach's Alpha
- Xác định cấu trúc yếu tố ẩn trong dữ liệu bằng phương pháp Phân tích yếu tố khám phá (Exploratory Factor Analysis - EFA)
- Phân tích mối quan hệ giữa các yếu tố ảnh hưởng đến sự hài lòng khách hàng trong dịch vụ logistics cảng biển

## Phương pháp nghiên cứu

### 1. Xử lý dữ liệu ban đầu
- Đọc và làm sạch dữ liệu từ file Excel (`Minh Tu_data.xlsx`)
- Chuyển đổi các biến quan sát thành dạng số
- Lọc các mẫu hợp lệ

### 2. Đánh giá độ tin cậy (Reliability Analysis)
- Tính Cronbach's Alpha cho từng thang đo
- Phân tích tương quan mục-tổng (Corrected Item-Total Correlation)
- Đánh giá Cronbach's Alpha nếu loại bỏ từng mục

### 3. Phân tích yếu tố khám phá (EFA)
- Kiểm định KMO (Kaiser-Meyer-Olkin)
- Kiểm định Bartlett's Test of Sphericity
- Trích xuất yếu tố bằng phương pháp Principal Component Analysis (PCA)
- Xoay yếu tố bằng phương pháp Varimax
- Đánh giá chất lượng tải trọng yếu tố

## Cấu trúc thang đo

Dự án sử dụng 5 thang đo chính:
- **RE**: Reliability (Độ tin cậy)
- **EMP**: Empathy (Sự đồng cảm)
- **DOC**: Documentation (Tài liệu)
- **CG**: Customer Guarantee (Bảo đảm khách hàng)
- **SAT**: Satisfaction (Sự hài lòng)

## File chính

- `Execution Mechanisms Behind Customer Satisfaction in Container Freight Station Services Evidence from Port Logistics Operations.ipynb`: Notebook chính chứa toàn bộ code phân tích
- `Minh Tu_data.xlsx`: Dữ liệu khảo sát thô (không bao gồm trong repo)

## Kết quả xuất ra

- `MinhTu_Cronbach_Summary.xlsx`: Tóm tắt Cronbach's Alpha cho tất cả thang đo
- `MinhTu_Cronbach_Detail.xlsx`: Chi tiết Cronbach's Alpha cho từng thang đo
- `MinhTu_EFA_Summary.xlsx`: Kết quả phân tích EFA bao gồm KMO, eigenvalues, factor loadings, communalities

## Yêu cầu kỹ thuật

- Python 3.x
- Các thư viện: pandas, numpy, scipy, scikit-learn, openpyxl

## Cách chạy

1. Đảm bảo file `Minh Tu_data.xlsx` nằm trong cùng thư mục với notebook
2. Mở notebook trong Jupyter Lab hoặc VS Code
3. Chạy từng cell theo thứ tự từ trên xuống dưới
4. Kết quả sẽ được xuất ra các file Excel trong thư mục làm việc

## Tác giả

- Minh Tú (Người thực hiện phân tích)
- Dự án nghiên cứu về logistics cảng biển

## Lưu ý

- Dữ liệu khảo sát gốc không được bao gồm trong repo vì lý do bảo mật
- Các kết quả phân tích phụ thuộc vào chất lượng dữ liệu đầu vào
- Tham khảo tài liệu thống kê chuyên ngành để hiểu rõ các chỉ số đánh giá