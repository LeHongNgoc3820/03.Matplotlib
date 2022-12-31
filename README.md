# Trực quan hoá dữ liệu với Matplotlib
[**Chi tiết bài viết**](https://github.com/LeHongNgoc3820/03.Matplotlib/blob/main/Data_Visualization_with_Matplotlib.ipynb)

**Dưới đây là tóm tắt lí thuyết**
## Nội dung:
1. Vai trò của trực quan hoá dữ liệu
2. Matplotlib
3. Quy trình tạo biểu đồ

## 1. Vai trò của trực quan hoá dữ liệu
**Định nghĩa:**  
"The use of compute-supported, visual representations of abstract data to amplify cognition." [(Card et al., 1999)](https://books.google.com.vn/books?hl=vi&lr=&id=wdh2gqWfQmgC&oi=fnd&pg=PR13&dq=Card+et+al.,+1999&ots=ooFE8vnNJv&sig=OSs6IKYX3nzWRAn_hVsS_rwPpPc&redir_esc=y#v=onepage&q=Card%20et%20al.%2C%201999&f=false)

**Tạm dịch:** là việc sử dụng các biểu diễn trực quan của dữ liệu trừu tượng thông qua sự hỗ trợ của máy tính để mở rộng nhận thức.

hay theo [Kirk (2016)](https://books.google.com.vn/books?hl=vi&lr=&id=wNpsDAAAQBAJ&oi=fnd&pg=PP1&dq=Kirk+(2016)&ots=AGw31mDjg5&sig=FmYDQTTO7RiapRygr5uns2B2hnY&redir_esc=y#v=onepage&q=Kirk%20(2016)&f=false), thì trực quan hoá dữ liệu có thể là sự diễn tả và trình bày dữ liệu để tạo điều kiện cho việc hiểu biết về dữ liệu.

**Vậy, tại sao cần trực quan hoá dữ liệu?**
+ Giúp người xem và hiểu dữ liệu một cách trực quan và dễ hiểu
+ Giúp giải quyết vấn đề nhanh
+ Kể câu chuyện về dữ liệu trong thời gian rất ngắn

### Nguyên tắc thiết kế:
**Good data visualization is:**
+ **Trustworthy (Tính trung thực)**: 
    + Sự tin tưởng khó kiếm, dễ mất
    + Tính trung thực và toàn vẹn cần phải có ở mọi nơi trong quá trình thực hiện project
    
+ **Accessible (Có khả năng tiếp cận):**
    + Cần phải biết ai là người sẽ xem các biểu đồ
    + Hiểu mục đích của việc trực quan hoá
    
+ **Elegant (Thanh lịch):**
    + Tập trung vào các yếu tố liên quan
    + Có phong cách thiết kế trước khi thể hiện

## 2. Matplotlib
### 2.1 Giới thiệu Matplotlib
+ Matplotlib là một thư viện vẽ biểu đồ 2D của Python, tạo ra các dạng hình vẽ khác nhau có chất lượng tốt.
+ Matplotlib có thể được sử dụng trong script Python (Python/IPython), Jupyter Notebook, ứng dụng web và 4 bộ tool GUI.
+ Người dùng có thể kiểm soát line style, font, các thuộc tính trên axes, ...thông qua giao diện hướng đối tượng hoặc thông qua các function.

### 2.2 Tại sao lại chọn Matplotlib?
+ Bởi vì, Matplotlib sẽ cố gắng làm cho mọi thứ dễ dàng trở nên dễ dàng hơn và những thứ khó khăn trở nên khả thi. Bạn có thể tạo các biểu đồ dạng plot, histogram, power spectra, barchart, error chart, scatter plot, ...với vài dòng code.

### 2.3 Quan sát biểu đồ
**Các thành phần chung trong biểu đồ gồm:**
+ Loại biểu đồ (bar, line, scatter, histogram, pie, ...)
+ Dữ liệu trên các trục (axes data ranges)
+ Nhãn trên trục (axes labels)
+ Ghi chú (legend)
+ Các chú thích (Annotations)

**Install Matplotlib:**  

`pip install matplotlib`

**Import vào để sử dụng:**

`import matplotlib.pyplot as plt`

**Một số lưu ý khác:**
+ Hiển thị biểu đồ: `plt.show()`
+ Tạo figure, axis:
    + `fig = plt.figure()`
    + `ax = plt.axes() `
+ Lưu figure: `plt.savefig(<tên_tập_tin>)`

## 3. Quy trình tạo biểu đồ
**Gồm các bước như sau:**  

**Bước 1: Chuẩn bị dữ liệu**
+ `list()`
+ `array()`
+ `Series()`
+ `DataFrame()`

**Bước 2: Tạo plot**
+ `plt.subplots()`
+ `plt.figure()`
+ `gridspec.GridSpec()`
+ `fig.add_subplot()`

**Bước 3: Vẽ biểu đồ**
+ `bar()`, `hist()`
+ `scatter()`/`Area() plot`
+ `pie()`/`Tree map`
+ `waffle chart wordCloud`

**Bước 4: Lưu plot**
+ `plt.savefig(<ten_bieu_do.png>)`

**Bước 5: Hiển thị plot**
+ `plt.show()`

