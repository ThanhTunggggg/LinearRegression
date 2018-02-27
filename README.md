# LinearRegression
1. Giá trị λ* tối ưu tìm được: 1.98

2. Các giá trị dự đoán: 
 		 		2.69174308
 				2.49789414
 				2.30399461
 				2.16338798
 				1.79210342
3. Cách tìm:
-  Chia tập training thành 2 tập dự liệu là traing dataset và validation dataset tỷ lệ 8:2(160:40).
-  Thực hiện quá trình lặp:
     +Train Ridge Regression model tham số regularization λ trên tập training và tính sai số trung bình dự đoán (MSE) của model trên tập validation.
     +Thay đổi  λ.
- Giá trị  λ cho MSE nhỏ nhất là  λ* cần tìm.
- Ban đầu  λ được thử trong 1 tập cấp số cộng với công sai lớn. Quan sát sai số, sau đó thu nhỏ lại khoảng tìm kiếm và bước nhảy.
- Thực hiện lại xây dựng model với  λ* và dự đoán.
