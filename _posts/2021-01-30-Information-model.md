---
layout: post
title: "Information Model (Mô hình Thông tin) cụ thể là gì?"
published: true
---


[Hỗ trợ các khái niệm trong nội dung của tiêu chuẩn BIM ISO 19650…]


Chúng ta nghe khái niệm Information model rất nhiều trong quy trình làm việc của BIM, cụ thể là quá trình các khối lượng thông tin được lưu hành và chuyển giao theo quy trình giữa các bên như thế nào. Nhưng cụ thể thì nó là gì và gồm nhưng thành phần cơ bản nào?


Một Mô hình Thông tin chuẩn, theo tiêu chuẩn PAS1192–2, bao gồm 3 phần tử chính là **Dữ liệu họa tính (Graphical Data)**, **Dữ liệu phi họa tính (Non-Graphical Data)**, và **Dữ liệu dưới dạng tài liệu (Documentation)**. Các dạng dữ liệu này đều được trữ và quản lý trong Môi trường dữ liệu chung (Common Data Environment). **Dữ liệu họa tính (Graphical data)** thường chỉ các loại thông tin ở dạng 2D hay 3D, như là các bản vẽ, model, bản báo cáo, cơ bản là loại thông tin thành phẩm có khả năng hiển thị hóa (visualize) dự án.


Một model của dự án thường chứa đến hàng ngàn các loại item khác nhau và ứng với mỗi item là vô số các loại thông tin kèm theo. Chính vì mất rất nhiều thời gian để tìm và chọn lọc thông tin phù hợp nên BIM cho phép việc phân tách một khối lượng thông tin nhất định và chuyển thể chúng dưới dạng một thuộc tính kỹ thuật số (digital attribute). Như vậy việc xử lí khối lượng lớn các thông tin đơn lẻ giờ đây được đơn giản hóa khi người dùng chỉ việc lọc và tương tác trực tiếp với các digital attribute trong database của dự án. Các dữ kiện ở dạng digital attribute đựơc gọi là **Dữ liệu phi họa tính (Non-graphical data)**.


Thành phẩm của tất cả các việc xử lí thông tin cuối cùng phải ở dưới dạng tĩnh (static), nghĩa là ở các dạng bảng in, PDF, scan, nói chung là dạng giấy tờ không thể thay đổi được nữa. Đây đã là một công đoạn truyền thống từ trước đến nay. Tuy nhiên càng ngày thì người ta sẽ hạn chế chuyển giao thông tin dưới dạng “tĩnh” mà sẽ là dưới dạng dữ liệu “sống” trữ trên hệ thống và do vậy dễ truy tìm và dễ quản lý hơn. Dữ liệu thông tin dưới dạng “tĩnh” để chuyển giao cho các bên sử dụng và tham khảo gọi là **Dữ liệu dưới dạng tài liệu (Documentation)**.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/Information-model.jpg)
{: refdef}


Tổng hợp bởi Jimmy Huy Nguyen


Đọc thêm tại https://www.thenbs.com/knowledge/building-information-modelling-what-information-is-in-the-model?fbclid=IwAR0qVzxM-1K8MUP7ojJhmXS59AojaPX7a5aXynIEy26VoQnE55jr1D9-rJA