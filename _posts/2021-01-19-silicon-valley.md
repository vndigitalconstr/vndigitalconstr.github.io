---
layout: post
title: "Áp dụng ISO 19650 vào dự án Metro cho Silicon Valley (Phần 1)"
published: true
---


Dự án BART to Silicon Valley là sự mở rộng của hệ thống metro San Francisco Bay Area Rapid Transit (BART) nối từ thành phố Fremont của hạt Alameda và băng qua các thành phố Milpitas, San Jose, và Santa Clara của hạt Santa Clara.
Phase 2 của dự án có độ dài 6 miles với đoạn đường hầm dài 5 miles băng qua khu trung tâm của San Jose. Sẽ có 3 trạm ngầm phân bổ dọc theo độ dài dự án và hiện đang trong giai đoạn thiết kế sơ bộ (preliminary design) và được ước chừng sẽ đi vào hoạt động trong năm 2030. Vì là phase 2 của dự án mở rộng tuyến metro Bay Area Rapid Transit (BART) để nối với thung lũng Silicon nên tên gọi chính thức của dự án là **BSVII (BART to Silicon Valley Phase II).**


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-1.png)
{: refdef}

{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-2.png)
{: refdef}


## ISO 19650 áp dụng vào các giai đoạn chuyển giao

Phần 2 của bộ tiêu chuẩn ISO 19650 được áp dụng chủ yếu vào dự án BSVII, nhất là ở các giai đoạn chuyển giao (Delivery Phase) của dự án và các công cụ BIM được sử dụng xuyên suốt và phối hợp toàn diện với nhau.


Như đã đề cập trong phần trước về ISO 19650, các khái niệm về chuyển giao trong phần 2 của tiêu chuẩn này giúp định hướng các bước đầu ra như điều phối nguồn lực (mobilization), phối hợp sản xuất thông tin (collaborative information development) và chuyển giao các model thông tin cho các bên (information model delivery).


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-3.png)
{: refdef}

Những nguyên tắc chính của ISO 19650 được vận dụng vào quy trình sử dụng và quản lý BIM trong dự án BSVII như sau:


- Xác định kế hoạch triển khai BIM
- Thiết lập môi trường chuyển giao số
- Thiết lập danh sách các mục tiêu cần đạt
- Điều phối nguồn lực
- Thiết lập các quy trình review, phê chuẩn, và chia sẻ thông tin


## 1) Appointment (Bố trí và điều phối các bộ phận)

Mott MacDonald trong dự án này là đơn vị được bổ nhiệm bởi client nên về công tác bố trí các đơn vị thực thi thì thuộc về trách nhiệm của client nhiều hơn. Về phía Mott MacDonald thì những nhiệm vụ quan trọng trong giai đoạn Appointment này là lập kế hoạch và quy trình BIM và quản lý dữ liệu cho các hoạt động sau này.


**Về quy trình triển khai BIM (BIM Execution Plan):**


Đây là bước quan trọng nhất trong giai đoạn thiết lập các cơ chế quản lý thông tin trước khi dự án bắt đầu. Team Mott MacDonald gặp rất nhiều những khó khăn ban đầu khi dự án gồm rất nhiều đơn vị từ nhiều lĩnh vực và quốc gia khác nhau và cần phải thiết lập một bộ tài liệu về quy trình BIM chuẩn hóa và thống nhất hóa cách làm việc của mọi bên. Bản báo cáo về quy trình triển khai BIM vì vậy đã đựơc sửa đi sửa lại và cập nhật liên tục trong suốt giai đoạn ban đầu. Nó được xem như là một dữ liệu ‘sống’ được review và đổi mới liên tục với sự tham gia đóng góp ý kiến của các đơn vị. Bộ hồ sơ này sau đó sẽ được hiệu chỉnh lần cuối, được duyệt bởi client sau đó là lưu hành cho các team.


**Về quy trình chuyển giao thông tin tổng thể (Master Information Delivery Plan , MIDP)**


Một tài liệu quan trọng thứ hai của việc thiết lập quy trình BIM tiền dự án là quy trình tổng thể về chuyển giao thông tin (MIDP). Thường thì MIDP sẽ được phân nhỏ thành các quy trình chuyển giao thông tin chức năng (Task Information Delivery Plan, TIDP) và được quản lý bởi các bộ phận chức năng đảm nhiệm một vai trò nhất định trong dự án. Các TIDP này tuy vận hành riêng rẽ trong nội bộ các bên nhưng thực chất là được tổng hợp với nhau trong môt nền tảng chung là MIDP.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-4.png)
{: refdef}


MIDP trong dự án này là các thông tin (bản vẽ, model, report) được lưu trữ trong Excel với các thông tin cụ thể như người phụ trách, thời gian, trạng thái. Để sinh động hóa các thông tin này thì công cụ Power BI được sử dụng bằng cách rút những thông tin từ Excel và hiển thị chúng dưới các dạng thông tin trực quan tóm tắt tiến độ dự án để ban quản lý dễ đánh giá và đưa ra quyết định.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-5.png)
{: refdef}


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-6.png)
{: refdef}


## 2) Mobilization (Điều phối tài nguyên và nguồn lực)


Giai đoạn này gồm có 2 pha chính là Tài nguyên (Resources) và Công nghệ (Technology).


**2.1) Tài nguyên (Resources)**
Một team chuyên về chuyển giao công nghệ số (Digital Delivery Team) cho dự án được lập ra sẽ chịu trách nhiệm toàn diện về môi trường số cho dự án, bao gồm thiết lập các nền tảng, công cụ, quy trình, và việc huấn luyện. Team này bao gồm các chuyên gia của Mott MacDonald từ khắp nơi trên thế giới như Úc, Mỹ, Anh.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-7.png)
{: refdef}


Nhân lực của team này sẽ được điều phối vào các bộ phận cũng như các đơn vị khác ở 46 địa điểm trên thế giới để đảm bảo sự đồng bộ trong việc áp dụng các ứng dụng số và quản lý thông tin giữa các bên. Một trong những vai trò đầu tiên là khảo sát về trình độ và kĩ năng của tất cả nhân lực trong việc sử dụng và làm quen với các công cụ và software (Revit, Bluebeam, BIM360, Civil 3D, SharePoint, vv) yêu cầu bởi dự án. Các báo cáo sẽ được hiển thị trong Power BI để phục vụ việc đánh giá mặt bằng năng lực chung của đội ngũ nhân lực.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-8.png)
{: refdef}


Ngay cả ở Mỹ thì các yêu cầu của tiêu chuẩn ISO 19650 và khái niệm CDE (Common Data Environment) vẫn còn khá mới mẻ và vì vậy đội ngũ Digital Delivery Team cũng hỗ trợ việc huấn luyện và đào tạo kĩ năng sử dụng các công cụ như Revit, Civil 3D, Navisworks.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-9.png)
{: refdef}


Một cơ sở dữ liệu chung trên nền tảng SharePoint là Project Wiki cũng được team Digital Delivery Team của Mott MacDonald lập nên như một thư viện mở hỗ trợ việc nâng cao kĩ năng số.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-10.png)
{: refdef}


Một cản trở lớn nhất trong giai đoạn đầu của dự án là sự tín nhiệm và niềm tin giữa các bên trong việc sử dụng thông tin của nhau. Quan trọng là phải đảm bảo đội ngũ dự án có niềm tin vào những nền tảng chung và những quy trình tiêu chuẩn thiết lập ban đầu bởi bên Mott MacDonald.


**2.2) Công nghệ (Technology)**


Các công cụ BIM nồng cốt sử dụng cho dự án đều là các sản phẩm của Autodesk. Lí do chính là các công cụ này đã khá phổ biến từ lâu và do vậy quen thuộc hơn với các đơn vị khắp nơi trên thế giới. Trường hợp đặc biệt là BIM360 mới được phổ biến gần đây và có những tính năng rất mới và do vậy cần có một sự làm quen lúc ban đầu với công cụ này.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-11.png)
{: refdef}


**2.2.a) Môi trường chuyển giao số (Digital Delivery Environment):**


Ngoài các công cụ chức năng cụ thể thì cần có các công cụ hỗ trợ về nền tảng để tích hợp và phối hợp các công cụ với nhau. Có 3 nền tảng đã được sử dụng cho dự án gồm SharePoint, ProjectWise, và BIM360. Ba nền tảng này được sử dụng cho các loại thông tin mang tính đặc thù khác nhau.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-12.png)
{: refdef}


Vì khó khăn để tìm được một nền tảng CDE duy nhất thỏa mãn tất cả những tiêu chí như tính tích hợp với mọi sản phẩm của Autodesk, tuân theo ISO 19650, khả năng đồng sở hữu và chịu trách nhiệm (co-authoring), vv. nên 3 nền tảng trên được sử dụng đồng thời và có sự liên kết nhất định với nhau.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-13.png)
{: refdef}


SharePoint


SharePoint có thể nói là công cụ khá phổ thông không giới hạn trong lĩnh vực xây dựng. SharePoint trong dự án này được chọn để quản lý các loại dữ liệu không chuyển giao (non-delivery information), ví dụ như các thông tin về quản lý dự án, sơ đồ nhân lực, các tài liệu về đào tạo, các links, templates, lịch nghỉ của nhân viên, nói chung là thông tin nội bộ hỗ trợ việc thực hiện dự án và không dùng để chuyển giao cho client hay các bên thứ ba.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-14.png)
{: refdef}


ProjectWise


ProjectWise là công cụ quản lý thông tin của dự án được sử dụng ngày càng nhiều bởi tính đa nhiệm cũng như cơ chế hoạt động rất tương hợp với tiêu chuẩn ISO 19650. ProjectWise trong dự án được dùng để quản lí tất cả các thông tin mang tính chuyển giao (deliverables), hay còn gọi là thành phẩm. Mott MacDonald đã hiệu chỉnh một số các thao tác để phù hợp hơn với yêu cầu của ISO 19650 như các đặt tên file, trạng thái của bản vẽ, mã phù hợp, quy trình review và chấp thuận bởi các bên,….


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-15.png)
{: refdef}


BIM360


BIM 360 đóng vai trò là nền tảng hỗ trợ các thông tin như Revit model và các mô hình liên đới (federated model) dưới định dạng Revit và Navisworks. Vì BIM360 bản chất không thật sự tương hợp với quy trình ISO 19650 nên team đã cần phải tạo một quy trình tương đương trong nền tảng BIM360 để quản lý các dữ liệu. Điểm mạnh lớn nhất của BIM360 là khả năng thể hiện và tăng sự trực quan cũng như tính tương tác trên các model tích hợp trên nền tảng.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-16.png)
{: refdef}


**2.2.b) Tiến trình chia sẻ thông tin (Information Sharing Workflows)**


Đối với BIM360, team đã phải tạo thủ công các folders cho các trạng thái Work in Progress và Shared (được chia sẻ), đồng thời là các quy trình chấp thuận trước khi thông tin được chuyển giao ra bên ngoài. Các thông tin được chấp thuận bởi tất cả các bên sẽ được copy một bản lưu trữ chứa trong folder Shared.


Đối với ProjectWise, các quy trình ngay từ đầu đã được thiết kế đúng theo tiêu chuẩn và vì vậy các quy trình sản xuất, review, và kiểm duyệt đựơc diễn ra một các tự động. Các thông tin tự động được gán mác về trạng thái (states) và sự phù hợp (suitability codes) để dễ dang cho các bên trong việc theo dõi và quản lý thông tin đầu ra.


**2.2.c) Công cụ Assemble**


Ở những giao đoạn đầu của dự án , các bản vẽ từ đội ngũ thiết kế có thể không đáp ứng được nhu cầu của bên phía bốc tách khối lượng do chất lượng các chi tiết có thể bị bể hay không được biểu hiện rõ trên một tỉ lệ cần thiết. Việc sản xuất các bản vẽ đáp ứng nhu cầu về chất lượng các chi tiết trên một tỉ lệ thích hợp được xem là quá khó khi phải thực hiện trong một thời gian ngắn và cuối cùng chỉ để dùng cho việc bốc tách khối lượng.


Chính vì lí do đó là công cụ Assemble đã được đề xuất sử dụng cho dự án. Công cụ mới này cho phép bên ước lượng quan sát được chi tiết model từ đó hiểu rõ hơn về hình thù của thiết kế. Không những vậy Assemble còn giúp hỗ trợ việc chiết xuất các chi tiết định lượng của thiết kế một cách dễ dàng và vì vậy tiết kiệm đáng kể về thời gian và tiền bạc.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-17.png)
{: refdef}


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-18.png)
{: refdef}


**2.2.c) Công cụ BIM Track**


Một công cụ mới nữa được giới thiệu vào dự án là BIM Track, sử dụng chủ yếu cho việc theo dõi và kiểm tra các xung đột giữa các phần tử trong model.


Lí do mà team quyết định không sử dụng Navisworks, vốn là một công cụ truyền thống để kiểm tra xung đột, là vì BIM Track còn cho phép việc kiểm tra các vấn đề không mang tính xung đột, ví dụ như cho phép người dùng yêu cầu thêm thông tin (RFI, Request For Information) của một chi tiết bất kì trong thiết kế. BIM Track còn có khả năng tích hợp với các ứng dụng BIM phổ biến như Revit, Navisworks, Civil 3D, Tekla Structures, Solibri. Ngoài ra BIM Track còn có tính năng phân tích dữ liệu, tạo report, và cho phép trình diện trên cả 2D và 3D.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-19.png)
{: refdef}


**2.2.d) Công cụ Power BI và Power Apps**


Hai ứng dụng Power BI và Power Apps của Office 365 cũng không còn xa lạ và có tính hiệu quả cao trong dự án. Power BI được sử dụng cho việc phân tích dữ liệu và tạo báo cáo với các dữ liệu thể hiện trực quan và thân thiện với người dùng.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-20.png)
{: refdef}


Ứng dụng Power Apps được sử dụng trong việc tự động hóa một vài tính năng chung như công cụ điều phối các đội ngũ, kiểm soát tài liệu (document control), danh mục của dự án, thông tin về BIM, vv.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-21.png)
{: refdef}


**2.2.e) Thực tế ảo (Virtual Reality)**
Kĩ thuật về thực tế ảo được giới thiệu vào dự án với việc đặt một station phục vụ cho các đội ngũ thiết kế trải nghiệm và vận dụng công nghệ này vào công việc. Các thực tế ảo mô phỏng dự án được vận hành trên các Revit models, ứng dụng Rehearsive App (phát triển bởi Mott MacDonald) và một headset cho người sử dụng.


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-22.png)
{: refdef}


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-23.png)
{: refdef}


{:refdef: style="text-align: center;"}
![1]({{ site.baseurl }}/images/metro-sv-24.png)
{: refdef}


**2.2.f) Về giao tiếp**


Việc giao tiếp giữa các đơn vị, các đội ngũ, các bộ phận chức năng được chú trọng khi nhân lực thực hiện dự án ở khắp nơi trên thế giới với các múi giờ khác nhau. Một số những nền tảng hỗ trợ việc giao tiếp bao gồm:


Microsoft Teams:


+ Trao đổi tức thời
+ Chia sẻ màn hình
+ Chia sẻ file
+ OneNote
+ Planner


Yammer:
+ Thảo luận mở giữa các thành viên
+ Giảm việc trao đổi qua email
+ Nâng cao sự phối hợp
+ Engage các thành viên dễ dàng


Newsletter:
+ Truyền đạc các chủ đề về quản lý thông tin


Các buổi meeting về BIM:
+ Cập nhật các tiêu chuẩn về sử dụng BIM
+ Chia sẻ các mẹo và kinh nghiệm hữu ích giữa các thành viên
+ Là nơi đề xuất ý tưởng và các phát kiến mới


…


Đón xem phần tiếp theo (Phần 2) của chuỗi bài Áp dụng ISO 19650 vào dự án Metro ở Silicon Valley về các giai đoạn tiếp theo của dự án khi các team phối hợp với nhau để đưa ra thành phẩm cuối cùng cũng như các cải tiến công nghệ và ứng dụng trong tương lai có thể đưa vào dự án.



Tổng hợp bởi Jimmy Huy Nguyen


Nguồn:


Bringing ISO 19650 to Silicon Valley — BIM Challenges on the BART Extension, Peter Starnes (Mott MacDonald), Brindusa Dumitrascu (Mott MacDonald), CES468335, Autodesk University


