# Nhóm 15: PHÁT HIỆN CÂY LÚA BỆNH DỰA VÀO HÌNH ẢNH
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
[1. Tóm tắt.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#tomtat)<br />
[2. Mô tả bài toán.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#motabaitoan)<br />
[3. Loại bài toán ML.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#loaibaitoan)<br />
[4. Quy trình.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#quytrinh)<br />
[5. Dữ liệu.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#dulieu)<br />
[6. Công cụ.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#congcu)<br />
[7. Đánh giá.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#danhgia)<br />
[8. Kết quả.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#ketqua)<br />
[9. Định hướng phát triển.](https://github.com/pcdanh/CS2225.CH1501/blob/master/README.md#dinhhuongphattrien)<br />


<h3 id="tomtat">1. Tóm tắt</h3>
●Tên đề tài: Phát hiện cây lúa bệnh dựa vào hình ảnh<br />
●Tóm tắt về đồ án và kết quả đạt được<br />
- Lý do chọn đề tài: Việt Nam là một trong những nước có sản lượng xuất khẩu gạo hàng đầu thế giới. Nhóm chúng em muốn xây dựng một hệ thống phát hiện bệnh trên cây lúa, để có thể giúp nông dân có các biện pháp trị bệnh kịp và tăng năng xuất đạt được hết mức<br />
- Kết quả đạt được: Các thử nghiệm được thực hiện bằng cách phân chia bộ dữ liệu thành các tỷ lệ khác nhau giữa tập huấn luyện-thử nghiệm. Mô hình đề xuất sử dụng mô hình khá phổ biến là Inception v3, có khả năng phân loại bệnh hại lúa với độ chính xác là 90% đối với tập huấn luyện<br /><br />
● Ảnh thành viên trong nhóm<br />
-Họ và tên: Phạm Công Danh<br />
-MSHV: CH1802003

![Danh](https://github.com/pcdanh/image/blob/master/danh.jpg) <br>
-Họ và tên: Lê Hưng  <br />
-MSHV: CH2001006<br />

![Hung](https://github.com/pcdanh/image/blob/master/hung.jpg) <br>

<h3 id="motabaitoan">2. Mô tả bài toán</h3>
Task: Phát hiện cây lúa bệnh dựa vào hình ảnh<br>
Input:  Hình ảnh cây lúa bệnh<br>
Output: Loại bệnh của cây lúa<br>
Minh hoạ

![Minh hoa](https://github.com/pcdanh/image/blob/master/1.png) <br>

<h3 id="loaibaitoan">3. Loại bài toán ML</h3>
● Classification<br>
<h3 id="quytrinh">4. Quy trình</h3>

![Minh hoa](https://github.com/pcdanh/image/blob/master/2.png) <br>

<h3 id="dulieu">5. Dữ liệu</h3>
●Dataset: Có 241 tấm ảnh<br>
●Dữ liệu Train: 153 tấm ảnh<br>
●Dữ liệu Validation: 74 tấm ảnh<br>
●Dữ liệu Test: 17 tấm ảnh <br>
●Cách thu thập: Tự thu thập<br>
●Tham số: 22,853,411<br>
●Cách train: Train với số Epoch là 20<br>
●Cách test: dùng 6 tấm ảnh trong tập dữ liệu test để test<br>


<h3 id="congcu">6. Công cụ.</h3>
Data augmentation<br>
Inception v3<br>

<h3 id="danhgia">7. Đánh giá.</h3>

![Danh gia](https://github.com/pcdanh/image/blob/master/3.png) <br>

●Loss của bộ Train càng ngày càng giảm<br>
●Validation Accuracy càng ngày càng tăng lên<br>
●Độ chính xác trên 90%<br>

<h3 id="ketqua">8. Kết quả.</h3>
●Điểm mạnh<br>
-Có thể nhận dạng ảnh mà background có độ nhiễu cao.<br>
-Mô hình đề xuất có khả năng phân loại bệnh hại lúa với độ chính xác là 90% đối với tập huấn luyện<br>
●Điểm yếu<br>
-Chưa nhận dạng được cây lúa bị nhiều bệnh cùng lúc(bệnh bạc lá, bệnh đốm nâu) từ ảnh đầu vào.<br>
-Nhận dạng sai cây lúa khỏe mạnh <br>

<h3 id="dinhhuongphattrien">9. Định hướng phát triển.</h3>
●Tìm hiểu bài toán phân loại đa nhãn (multi-label classification) để nhận dạng cây lúa bị nhiều bệnh từ ảnh đầu vào<br>
●Cải tiến thuật toán và thu thập thêm dữ liệu cây lúa khỏe mạnh, để có thể nhận dạng được cây lúa khỏe mạnh<br>


