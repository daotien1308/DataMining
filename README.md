# DataMining
1. Nguyễn Anh Đắc 19133020
2. Nguyễn Thanh Tân Kỷ 19133031
3. Lại Hữu Trác 19133059
4. Đào Thị Cẩm Tiên 19133055
## Giới Thiệu
- Tiếp cận nước uống an toàn là điều cần thiết đối với sức khỏe, một quyền cơ bản của con người và là một thành phần của chính sách hiệu quả để bảo vệ sức khỏe. 
- Đây là vấn đề quan trọng như một vấn đề sức khỏe và phát triển ở cấp quốc gia, khu vực và địa phương. 
Ở một số vùng, người ta đã chỉ ra rằng các khoản đầu tư vào cấp nước và vệ sinh có thể mang lại lợi ích kinh tế ròng, vì việc giảm các tác động xấu đến sức khỏe và chi phí chăm sóc sức khoẻ lớn hơn chi phí thực hiện các can thiệp.

## Data
- Dữ liệu chứa các chỉ số chất lượng nước, gồm 10 cột và 3276 dòng
- Các cột trong tập dữ liệu:
  + pH value: Độ pH của nước. WHO đã khuyến cáo giới hạn pH tối đa cho phép từ 6,5 đến 8,5
  + Hardness(mg/l): Độ cứng của nước. Độ cứng của nước được định nghĩa đơn giản nhất là loại nước có tổng lượng muối Ca và Mg được hòa tan trong nước vượt qua mức cho phép
  + Solids (Total dissolved solids - TDS): Tổng chất rắn hoà tan trong nước. giới hạn mong muốn cho TDS là 500 mg / l và giới hạn tối đa là 1000 mg / l được quy định cho mục đích uống	
  + Chloramines: Mức clo lên đến 4 miligam mỗi lít (mg / L hoặc 4 phần triệu (ppm)) được coi là an toàn trong nước uống
  + Sulfate: lượng sulfate trong nước
  + Conductivity: tính dẫn điện. 
  + Organic_carbon: lượng cacbon hữu cơ trong nước
  + Trihalomethanes: lượng THM trong nước. Đây là sản phẩm phụ của quá trình khử trùng nước bằng Chlorine.
  + Turbidity: Độ đục của nước
  + Potability: Cho biết liệu nước có an toàn cho con người hay không, trong đó 1 nghĩa là Uống được và 0 nghĩa là Không uống được
  
  
  
## Kế Hoạch Phân Tích

- Nhóm đặt ra câu hỏi nghiên cứu chung là tìm ra các yếu tố ảnh hưởng tới chất lượng nước: Dự đoán chất lượng nước (1: an toàn, 0: không an toàn)
- Dự đoán:
  + Input: pH, Hardness, Solids, Chloramines, Sulfate, Conductivity, Organic_carbon, Trihalomethanes, Turbidity.
  + Output: Potability.

- Chia tập train, tập test tỷ lệ 75% train và 25% test
- Trên tập train sẽ thử các thuật toán:
  + KNN
  + Random Forest
  + Logistic Regression
- Phương pháp sử dụng: K-fold Cross Validate
- Lựa chọn mô hình cho kết quả tốt nhất.
- Đánh giá mô hình trên tập test.
