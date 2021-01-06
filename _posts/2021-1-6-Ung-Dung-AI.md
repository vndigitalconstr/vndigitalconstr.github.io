---
layout: post
title: 'Ứng dụng AI vào quy hoạch đô thị nhà ở'
published: true
---

Một số ứng dụng lớn nhất của AI trong xây dựng số hiện nay là **thiết kế phái sinh (generative design)**, một dạng tự động hóa có thể tạo ra hàng loạt các thiết kế khác nhau dựa trên một số thuật toán và quy chuẩn thiết lập ban đầu bởi người thiết kế. Cụ thể hơn, thiết kế phái sinh là một dạng thuật toán tiến hóa lấy phạm vi biến đầu vào (variable ranges), thực thi bộ đánh giá, khám phá không gian thiết kế cho các giải pháp tối ưu và đưa ra vô số giải pháp khả thi để đáp ứng các tiêu chí được cung cấp ban đầu.


Quy hoạch khu nhà ở hiện đại (town planning) trên các nước trên thế giới và cả Việt Nam đang đi theo xu hướng chuẩn hóa thiết kế (standardization) cho các mẫu nhà và thay vì vậy nhấn mạnh hơn vào cách sắp đặt cảnh quan và các đơn vị nhà sao cho hòa hợp với thiên nhiên và hướng tới tương lai bền vững (sustainability). Cùng đi qua mô hình AI của Bonava, một công ty phát triển dự án về nhà ở của Bắc Âu và một trong những đơn vị lớn nhất và lâu đời nhất của khối Scandinavia , trong việc tự động hóa các mẫu thiết kế trên một diện tích quy hoạch lớn và từ đó hỗ trợ việc đưa ra quyết định tối ưu nhất về kinh tế, môi trường, và tính bền vững cho khu vực.

## 1/ BIM và Thiết kế và xây dựng ảo (Virtual Design and Construction)

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-1.png)
{: refdef}

**Thiết kế và xây dựng ảo (Virtual Design and Construction-VDC)** là hành trang quan trọng để hướng việc thay đổi thị trường về phát triển dự án bất động sản. Mục đích qua trọng là số hóa quy trình từ thiết kế đến thi công, nâng cao khả năng phối hợp giữa các ban ngành, giảm chi phí vận hành và tăng năng suất với sự tập trung hướng đến khách hàng.

BIM giữ vai trò quan trọng là nền tảng của tất cả các thiết kế và dữ liệu. Trong đó thì Revit là nền tảng chính với các mẫu thiết kế có sẵn trong Revit family và vì vậy việc tích hợp Revit với các nền tảng BIM khác là vô cùng quan trọng.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-2.png)
{: refdef}

## 2/ Thiết kế tự động hóa dựa trên dữ liệu phái sinh

Theo quy trình truyền thống thì các thiết kế khác nhau sẽ cho ra các kết quả khác nhau và sẽ chọn ra phương án cuối cùng cho thiết kế với kết quả tốt nhất. Tuy nhiên với xu hướng của công nghệ AI bây giờ, do các thiết kế khác nhau có thể được tạo ra nhanh chóng nên vì vậy có thể chọn ra kết quả tối ưu nhất dựa trên những dữ liệu thiết kế tiềm năng và từ đó sexcho ra được thiết kế cuối cùng.

**Quy trình truyền thống:**

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-3.png)
{: refdef}

**Quy trình tự động hóa:**

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-4.png)
{: refdef}

## 3/ Quy trình thiết kế không gian quy hoạch của Bonava

### 3.1 Bước 1: Chuẩn bị và Thiết lập (Setup)

**Những đơn vị có sẵn (một đơn vị tòa nhà)** gồm các module được tạo và lưu trữ dưới dạng Revit family với những thông tin kỹ thuật được đính kèm

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-5.png)
{: refdef}

Những quyết định sẽ được đặt ra về thiết kế của đơn vị (nhà ) nào là phù hợp cho yêu cầu dự án và có thể kết hợp bao nhiêu kiểu thiết kế khác nhau và kết hợp như thế nào

**Yếu tố ngoại cảnh**: Dùng dữ liệu GIS để lấy quan trắc địa lý và các hệ thống hạ tầng và điều kiện tự nhiên của một địa điểm

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-6.png)
{: refdef}

Yếu tố của một khu đất dự án ảnh hưởng đến quyết định để đưa ra thiết kế phù hợp, vd: địa hình dốc, đường xá đã có sẵn,…

**Tiêu chuẩn và yêu cầu**: Mỗi khu vực có những tiêu chuẩn nhất định cho các công trình như tiêu chuẩn quốc gia, tiêu chuẩn về phòng cháy và thoát hiểm

Ví dụ: Yêu cầu về độ rộng của vỉa hè, chiều cao ngói tòa nhà, bề rộng không gian sau nhà

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-7.png)
{: refdef}

### 3.2 Bước 2: Khai triển các phương án (Generate)

Như nguyên lí của thuật toán phái sinh, thiết kế các đơn vị (nhà) sẽ cố định và thay đổi các biến số khác để tạo ra hàng loạt những phương án thiết kế khác nhau dựa trên các tiêu chuẩn và điều kiện ngoại cảnh của bước 1. Các biến số có thể là hệ thống đường, số lượng kiểu nhà, diện tích mảng xanh,… trong diện tích dự án. Chính vì vậy mà AI có thể khai triển được hàng ngàn các phương án khác nhau.

Hình bên dưới là một số mẫu thiết kế, trong đó các khối xanh nhạt và xanh đậm đại diện cho các đơn vị nhà bố trí theo những layout khác nhau.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-8.png)
{: refdef}

Các phương án được thực hiện và trữ trên nền tảng Rhinoceros 3D, , có thể được xem trên giao diện Design Explorer và được cho một ID nhất định.

**Procedural algorithm**: Thuật toán mở rộng của thuật toán phái sinh cho phép một phương án được khai triển bằng cách mở rộng trên phương án được khai triển trước đó. Ví dụ như AI có thể khai triển các kiểu phương án khác với cùng một hệ thống đường xá của một phương án mà được đánh giá là hiệu quả trước đó.

**Thuật toán cho kiểu nhà nhiều hộ gia đình**: Với thuật toán cho kiểu nhà đơn cho một gia đình thì mẫu thiết kế nhà có thể là hằng số, nhưng sẽ phức tạp hơn cho kiểu nhà nhiều hộ gia đình vì lúc này kiểu nhà sẽ là một biến vì có tới hàng trăm cách để phối hợp các Revit module.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-9.png)
{: refdef}

### 3.3 Bước 3: Đánh giá và Phân tích (Evaluation)

Các yếu tố đánh giá được thể hiện qua các thông số trong các cột và mỗi phương án sẽ có một biểu đồ nhất định ứng với giá trị mà nó đi qua trong mỗi cột.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-10.png)
{: refdef}

Ví dụ như phương án #48 bên dưới được đánh giá qua biểu đồ xanh đi ngang qua các cột đại diện cho các yếu tố ứng với số điểm mà nó đạt được cho mỗi cột (yếu tố)

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-11.png)
{: refdef}

Bằng cách chồng lên nhau các biểu đồ của tất cả hàng trăm hàng ngàn phương án sẽ cho một đánh giá khả quan về các yếu tố như chi phí, tính khả thi, và để các bên phối hợp ăn ý với nhau hơn trong việc đưa ra quyết định cuối cùng

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-12.png)
{: refdef}

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-13.png)
{: refdef}

Các team khác nhau sẽ có những tiêu chí đánh giá khác nhau và vì vậy sẽ có yêu cầu về điểm số khác nhau giữa các yếu tố đánh giá. Team tài chính sẽ quan tâm hơn về yếu tố số lượng nhà và dữ liệu đất để tính toán chi phí dự án, Team bán hàng và Marketing thì nhìn vào các yếu tố như mảng xanh hay diện tích đón ánh nắng để quảng bá dự án tốt hơn với khách hàng tiềm năng

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-14.png)
{: refdef}

### 3.4 Bước 4: Lựa chọn phương án và Đưa ra quyết định (Final design)

Để hỗ trợ cho việc review hàng ngàn phương án khác nhau trữ trong database của Revit, Window được chạy bởi script Dynamo trong Revit và kết nối với database trong Revit cho phép các phương án được thể hiện trực quan. Người dùng chỉ cần nhập mã ID ứng với mỗi dự án thì 3D model sẽ hiện lên tương ứng.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-15.png)
{: refdef}

Nếu người dùng muốn đi sâu vào chi tiết hoặc muốn điều chỉnh một phương án bất kì thì chỉ cần nhấn nút "import to Revit" trên window thì toàn bộ phương án với các thông tin liên quan sẽ được chạy và trình duyệt trực tiếp trên Revit

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-16.png)
{: refdef}

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-17.png)
{: refdef}

Vì các đơn vị nhà đã có sẵn trong Revit dưới dạng family, việc mô phỏng toàn bộ phương án trong Revit sẽ diễn ra nhanh hơn vì Revit không cần phải tải lại dữ liệu cho các mẫu nhà mà chỉ đơn giản lấy chúng ra từ kho family và sẵp xếp với nhau tương ứng với thiết kế của phương án.

### 4/ Các công cụ được sử dụng trong quy trình (Bước 1 đến Bước 4)

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-18.png)
{: refdef}

Các family đơn vị nhà (housing unit) được tạo và lưu trữ trong Revit nên vì vậy các phương án cũng được mô phỏng trên nền tảng Revit để dễ dàng lấy thông tin. Các phương án thiết kế được phái sinh (generate) trong nền tảng Rhinoceros 3D và các dữ liệu đánh giá thì được chuyển thành dạng format .json và được trữ trong dữ liệu của nền tảng Mongo. Giao diện của các dữ liệu đánh giá phương án cũng như các bảng báo cáo đánh giá được thực hiện trên trình duyệt mở là Design Explorer thân thiện với người dùng. Các phương án thiết kế được trình duyệt trên Design Explorer sẽ có những mã ID nhất định kể cả khi chúng được import lại vào Revit khi người dùng muốn truy cập sâu thêm vào dự án.

### 5/ Kết quả

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-19.png)
{: refdef}

### 6/ Chúng ta có thể kì vọng những gì trong tương lai?

Bonava đã đầu tư phát triển công nghệ thiết kế phái sinh dựa vào AI và thuật toán trong những năm gần đây. Dưới đây là những cột mốc về những tiến hóa trong tính năng mà công ty đã đạt được từ năm 2017 bắt đầu với model theo tham số (parametric modelling) trong Revit và có thể trong tương lai là Machine learning khi AI có thể tự học và tự cải thiện trên kinh nghiệm trước đó. Mục đích lớn nhất của AI là giúp chúng ta đưa ra quyết định dễ dàng và tối ưu hóa.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-20.png)
{: refdef}

Tổng hợp bởi Jimmy Huy Nguyen


Reference:


Connecting people and algorithms - Generative Design for informed decisions by Sofia Malmsten (Bonava), Anita Apele (Bonava), Erik Forsberg (Bonava), Autodesk University, AS467596

Infographic tổng hợp các ý chính của chủ đề được nhóm VNDCC biên soạn có thể được tìm thấy dưới đây.

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/ai-21.png)
{: refdef}