# PHÁT HIỆN CÂY LÚA BỆNH DỰA VÀO HÌNH ẢNH
# Phạm Công Danh - CH1802003
# Lê Hưng - CH2001006
# https://github.com/hungiscoding/CS2225.CH1501

# GIỚI THIỆU 
Việt Nam là một trong những nước có sản lượng xuất khẩu gạo hàng đầu thế giới. Tuy nhiên, hằng năm cây lúa khắp nơi đều gặp những bệnh khác nhau khiến năng xuất không đạt được hết mức. Nhóm chúng tôi muốn xây dựng một hệ thống có thể giúp người nông dân nhanh chóng bắt được đúng bệnh của cây lúa và thực hiện các biện pháp trị bệnh kịp thời. 
<br />
# THIẾT KẾ HỆ THỐNG 
Hệ thống của chúng tôi sẽ được train để phân loại các loại bệnh thường gặp của cây lúa, từ đó đưa ra gợi ý các điều trị, giúp người nông dân đạt năng suất cao nhất.<br />

# Đầu vào của hệ thống: 
Hình ảnh cây lúa bệnh.<br />

# Đầu ra của hệ thống: 
Loại bệnh của cây lúa.<br />

Dữ liệu để train và test hệ thống: tự thu thập.<br />
Rủi ro của hệ thống: Bộ dataset có thể không đủ lớn để nhận dạng các loại bệnh của cây lúa.<br /> 

# KỲ VỌNG VÀ HƯỚNG PHÁT TRIỂN
Tìm hiểu bài toán phân loại đa nhãn (multi-label classification) để nhận dạng cây lúa bị nhiều bệnh từ ảnh đầu vào<br /> 
Cải tiến thuật toán và thu thập thêm dữ liệu cây lúa khỏe mạnh, để có thể nhận dạng được cây lúa khỏe mạnh<br /> 


# NỘI DUNG
1. [Tóm tắt.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#tomtat)<br />
2. Mô tả bài toán.<br />
3. Loại bài toán ML.<br />
4. Quy trình.<br />
5. Dữ liệu.<br />
6. Công cụ.<br />
7. Đánh giá.<br />
8. Kết quả.<br />
9. Định hướng phát triển.<br />

<h3 id="tomtat">1. Tóm tắt</h3>
●Tên đề tài: Phát hiện cây lúa bệnh dựa vào hình ảnh<br />
●Tóm tắt về đồ án và kết quả đạt được<br />
- Lý do chọn đề tài: Việt Nam là một trong những nước có sản lượng xuất khẩu gạo hàng đầu thế giới. Nhóm chúng em muốn xây dựng một hệ thống phát hiện bệnh trên cây lúa, để có thể giúp nông dân có các biện pháp trị bệnh kịp và tăng năng xuất đạt được hết mức<br />
- Kết quả đạt được: Các thử nghiệm được thực hiện bằng cách phân chia bộ dữ liệu thành các tỷ lệ khác nhau giữa tập huấn luyện-thử nghiệm. Mô hình đề xuất sử dụng mô hình khá phổ biến là Inception v3, có khả năng phân loại bệnh hại lúa với độ chính xác là 90% đối với tập huấn luyện<br /><br />
● Ảnh thành viên trong nhóm<br />
-Họ và tên: Phạm Công Danh<br />
-MSHV: CH1802003<br />
![Danh](https://github.com/pcdanh/CS2225.CH1501/blob/master/Lab/danh.jpg?raw=true) <br />

-Họ và tên: Lê Hưng  <br />
-MSHV: CH2001006<br />
![Hung](https://github.com/pcdanh/CS2225.CH1501/blob/master/Lab/hung.jpg) <br />

