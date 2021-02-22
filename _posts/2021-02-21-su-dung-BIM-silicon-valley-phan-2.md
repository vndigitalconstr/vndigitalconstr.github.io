---
layout: post
title: "Áp dụng ISO 19650 vào dự án Metro cho Silicon Valley (Phần 2)"
published: true
---


Tiếp theo phần 1 (Áp dụng ISO 19650 vào dự án Metro cho Silicon Valley), phần 2 của bài viết sẽ đi vào 2 giai đoạn tiếp theo của quy trình BIM theo khuyến nghị của tiêu chuẩn ISO 19650.


## 3) Collaborative Production (Hợp tác sản xuất)


**3.1) Kết nối các dữ liệu**


Sau khi đã trang bị tất cả các nguồn lực, tài nguyên, và công cụ cần thiết cho lộ trình số hóa dự án, việc tiếp theo là đảm bảo các dữ liệu từ các nguồn có khả năng liên kết và được sử dụng qua lại trên nhiều nền tảng khác nhau.


Ví dụ như dữ liệu từ các nền tảng khác nhau sẽ có format khác nhau, do vậy khi trao đổi các dữ liệu này giữa các nền tảng khác nhau thì cần convert chúng dưới các định dạng exchange format như Navisworks, IFC, DXF hoặc chiết xuất chúng dưới dạng text hay table. Phần lớn các thao tác chuyển đổi format của dữ liệu được thực hiện bằng các thủ công, tuy nhiên một số đã được tự động hóa bởi các chuyên gia trong team.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-1.png)
{: refdef}


**3.2) Các biểu diễn dữ liệu (Renditions)**


Mặc dù đã thiết lập những môi trường dữ liệu chung (Common Data Environment) để chứa các model, team vẫn gặp các thử thách khi liên kết 2 nền tảng BIM360 và ProjectWise. Do vậy, team đã phải tạo các bản biểu diễn (renditions) bằng phương pháp thủ công với việc cập nhật liên tục các phiên bản khác nhau.


**3.3) Các mã thể hiện tính phù hợp (suitability codes)**


Thuật ngữ Suitability codes theo ISO 19650 là các dạng mã số thể hiện tính phù hợp của một item (report, bản vẽ, biểu diễn, model) trong việc nó đang ở trạng thái gì và có thể được sử dụng cho mục đích nào và chỉ có thể được nhìn thấy bởi ai. Các mã phù hợp thể hiện mức độ tự tin về một item trong việc là nó có sẵn sàng để được chia sẻ cho tất cả các bên, hay có thể chuyển giao cho khách hàng, hay tốt nhất là chỉ lưu hành nội bộ tùy vào giai đoạn và độ chỉnh chu của sản phẩm. Các mã phù hợp này là ứng dụng tích hợp có sẵn trong ProjectWise, nhưng phải được thiết lập thủ công trong nền tảng BIM 360.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-2.png)
{: refdef}


(Hình trên) Các mã phù hợp bao gồm S0 (Working in Progress, các item còn trong quá trình tạo, chưa chính thức, chỉ sử dụng nội bộ trong bộ phần chịu trách nhiệm), S1 (Suitable for Coordination, có thể được chia sẻ cho các bên liên quan để sử dụng), S2 (Suitable for Information, dữ liệu chia sẻ cho các bên chỉ đơn thuần mang tính chất tham khảo), S3 (Suitable for Review & Comment, dữ liệu có thể được chia sẻ cho các bên để đánh giá và đưa feedback), S4 (dữ liệu có thể được chuyển giao cho client).


**3.4) Các trạng thái (states)**


Trạng thái của một hồ sơ (Kết hợp với mã phù hợp) là biểu hiện của việc một hồ sơ đó đã được thông qua, kiểm duyệt, và chấp thuận bởi đối tượng nào. Quá trình một hồ sơ đi qua các vòng kiểm duyệt bởi các đối tượng khác nhau được gọi là workflow. Cơ bản là để một hồ sơ đạt chuẩn yêu cầu thì nó phải đi qua hết một workflow, hoàn tất tất cả các vòng kiểm duyệt.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-3.png)
{: refdef}


Ví dụ như khi một bản vẽ vừa hoàn thành thì nó sẽ ở trạng thái *Working in Progress (chỉ có ở trạng thái này thì bản vẽ mới cho phép thực hiện các thay đổi và chỉnh sửa)*. Sau đó để nó lên được trạng thái tiếp theo là *Content check (cho việc kiểm tra nội dung)* thì nó phải được chấp thuận bởi 1 đối tượng thường với vai trò là họa viên hoặc kĩ sư. Sau đó để lên được trạng thái tiếp theo nữa là *Technical Check (cho việc kiểm tra về kĩ thuật)* thì nó phải được chấp thuân bởi đối tượng là kĩ sư thiết kế *(người này chịu trách nhiệm trực tiếp cho các chi tết trong bản vẽ)*. Để lên trạng thái tiếp theo là *Shared (cho việc chia sẻ giữa các bên)* thì nó phải được chấp thuận bởi kĩ sư trưởng *(là người chịu trách nhiệm chính thức trong một bộ phận)*. Để lên tiếp các trạng thái như *Coordination Check*, *Approve*, *Authorization (cho việc phê chuẩn và các đánh giá cuối cùng)* thì nó thường phải được chấp thuận bởi package lead (trưởng gói dự án. Sau cùng là trạng thái *Published (chính thức được phể chuẩn để sử dụng)* thì nó phải được thông qua bởi người quản lý dự án Project Manager và sẽ được truy cập bởi client.


Trong bất kì trạng thái nào mà người phê chuẩn cảm thấy hồ sơ không đủ tiêu chuẩn hay cần phải được sửa đổi thì họ có thể *revise/reject* trạng thái của hồ sơ trở lại trạng thái ban đầu là *Working in Progress* cho việc chỉnh sửa.


**3.5) Công tác đảm bảo chất lượng các model trong CAD/Revit**


Do việc thiết kế và thiết lập các model được thực hiện bởi nhiều đơn vị từ nhiều quốc gia và tổ chức khác nhau nên vần có một bản nguyên tắc chung trong việc kiểm định chất lượng của các sản phẩm model. Công tác này sẽ đươc thực hiện bởi người tạo model cũng như BIM team.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-4.png)
{: refdef}


**3.6) Liên đới các model (Model Federation)**


Việc liên đới các model vởi nhau được thực hiện trong BIM 360 và Navisworks. Các model được tạo đơn thuần trong Revit/CAD được lưu trữ dưới dạng Navisworks NWC cho việc tích hợp với nhau tạo thành một mô hình liên đới tài sản tổng thể (asset federation model) và là một phần của model dự án. Như vậy khi muốn truy cập vào bất cứ phần nào của dự án thì chỉ việc export phần đó trong mô hình liên đới dưới dạng format NWD có thể xem được cả trong nền tảng BIM 360 và Navisworks. Theo đánh giá thì phần lớn các team member thích sử dụng BIM 360 hơn trong việc nhìn và hiển thị trực quan model.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-5.png)
{: refdef}


**3.7) Quá trình nhận diện và khắc phục các xung đột phần tử**


Các model trong Navisworks được sử dụng cho việc phát hiện các xung đột và va chạm phần tử (clash detection). Các xung đột phát hiện trong Navisworks sẽ được xuất vào nền tảng BIM Track và nền tảng này sẽ lần lượt thông báo các đối tượng liên quan như trưởng phòng thiết kế hay họa viên model về các item cần được giải quyết. Quy trình tổng thể có thể tìm thấy trong sơ đồ dưới:


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-6.png)
{: refdef}


**3.8) Quy trình theo dõi các vấn đề**


BIM Track như trong phần 1 có đề cập thì nền tảng này ngoài khả năng giải quyết các xung độ phần tử thì còn có thể theo dõi và báo cáo các vấn đề về vi phạm tiêu chuẩn, ảnh hưởng về tài chính, điều phối về thiết kế, yêu cầu làm sáng tỏ thông tin, vv. Các vấn đề này có thể được tạo trực tiếp trên giao diện của BIM Track hay bất cứ nền tảng nào tích hợp vởi BIM Track. Điểm mấu chốt là các thông tin về đối tượng hướng đến phải được điền chính xác và rõ ràng để BIM Track có thể gửi report đến đúng với các đối tượng này.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-7.png)
{: refdef}


**3.9) Các tiêu chuẩn của phòng (Room Criteria)**


Các phòng (room) trong Revit thường được đặt tên không đồng nhất và được đánh số khác biệt nhau giữa các bên. Không những vậy thì diện tích tiêu chuẩn của phòng cũng bị sai lệch khi thực hiện bởi các bên. Vì lí do đó, một công cụ bên thứ ba là BIMLink để xuất bản các dữ liệu phòng vào trong Excel từ một model liên đới trên Revit. Việc đối chiếu thông tin của dữ liệu phòng với dữ liệu tiêu chuẩn được thực hiện trong spreadsheet của Excel và các kết quả đánh giá và sửa đổi sẽ được xuất ngược lại vào model trong Revit và tự động update các dữ liệu trong model. BIMLink được xem là một trong những công cụ thẩm định chất lượng hiệu quả trong dự án.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-8.png)
{: refdef}


**3.10) Các buổi họp SHARC (Share, Appraisal Review & Coordinate)**


Dù có nhiều các công cụ hỗ trợ sự phối hợp giữa các bên như thế nào thì giao tiếp qua hội thoại trực tiếp vẫn đóng vai trò vô cùng quan trọng. Các buổi meeting giữa các bên sẽ xoay quanh việc thảo luận trực tiếp trên các model và từ đó đưa ra những kế hoạch hành động tương ứng.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/silicon-9.png)
{: refdef}


## 4) Information model delivery (Chuyển giao các model thông tin)


Vì dự án vẫn đang ở trong giai đoạn phát triển concept về thiết kế nên các quy trình về chuyển giao model thông tin của tài sản (asset information delivery) chưa được đi vào chi tiết. Tuy nhiên thì team vẫn đang làm việc với các bên để trao đổi về các yêu cầu về thông tin trong vòng đời của dự án (Project lifecycle) từ đó team có thể phát triển các quy tắc tương ứng. Các quy tắc này sẽ được phát triển thêm khi dự án đi vào giai đoạn thiết kế chi tiết (detailed design).


## 5) Kết quả


Dù đã có những công tác chuẩn bị kĩ lưỡng cho việc lên kế hoạch áp dụng các công cụ số nhưng team đã và vẫn đang đối mặt thường trực với các thách thức lớn. Nhất là việc hệ tiêu chuẩn ISO 19650 vẫn còn khá mới mẻ ở Bắc Mỹ, và dự án là trải nghiệm đầu tiên về quy trình ISO 19650 đối với phần lớn các nhân lực. Thứ hai là kiểu “thói cũ khó bỏ” khi đòi hỏi các nhân lực phải thay đổi cách làm việc từ trước đến nay và học lại từ đầu cách sử dụng các công cụ và nền tảng công nghệ.


Một thử thách khác là vấn đề đào tạo nhân lực khi đội ngũ luôn có sự thay đổi về cơ cấu nhân lực và luôn có thành viên mới tham gia vào dự án nên việc đào tạo đòi hỏi phải diễn ra nhanh, tinh gọn, và chuẩn bị kịp thời để nhân lực có thể tham gia ngay vào quy trình làm việc của dự án.


Cột mốc đầu tiên mà team đạt được là vào tháng 12 năm 2019 khi 10% khối lượng thiết kế đã được chuyển giao. Có tổng cộng 920 files đã được nộp, 199 model 3D được tạo và xử lí tổng cộng 1835 files được chuyển tới team. Ngoài ra theo khảo sát thì năng lực của đội ngũ đã tăng 50% nhờ vào hệ thống đào tạo được chuẩn bị lúc ban đầu.


Tổng hợp và dịch thuật bởi Jimmy Huy Nguyen


Nguồn:


*Bringing ISO 19650 to Silicon Valley — BIM Challenges on the BART Extension*, Peter Starnes (Mott MacDonald), Brindusa Dumitrascu (Mott MacDonald), CES468335, Autodesk University