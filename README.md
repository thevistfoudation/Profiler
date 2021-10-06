# Profiler
## Document Profiler
### MỤC LỤC 
- [I.UI and UI Details Profiler là gì ?](#What)
- [II.UI and UI Details Profiler Dùng như thế nào ?](#How)
- [III.UI and UI Details Profiler Dùng trong trường hợp thế nào ?](#When)
<a name="What"></a>
## I. UI and UI Details Profiler là gì ?
`UI and UI Details Profiler` là window cung cấp thông tin về lượng thời gian và tài nguyên mà Unity dành để thiết lập và hiển thị giao diện người dùng trong ứng dụng của bạn. Bạn có thể sử dụng modules này để hiểu cách Unity xử lý việc phân lô giao diện người dùng cho ứng dụng của bạn, bao gồm lý do và cách nó phân lô các đối tượng. Bạn cũng có thể sử dụng modules này để tìm hiểu xem phần nào của giao diện người dùng chịu trách nhiệm cho hiệu suất chậm hoặc để xem trước giao diện người dùng trong khi bạn kiểm tra dòng thời gian.
![image](https://user-images.githubusercontent.com/47918431/135761714-fb5910ef-6cea-41ec-81ea-87b9def94bea.png)
<a name="How"></a>
## II. UI and UI Details Profiler Dùng như thế nào ?
I: để sử dụng Profiler 
 - 1: Mở Profiler `Window` -> `Analyis` -> `Profiler`
 - ![image](https://user-images.githubusercontent.com/47918431/135762542-fb77b537-d5f3-4438-bef1-bcbdad01bfa8.png)
 - 2: Cấu hình lại Profiler 
    - Ở góc trên cùng bên trái `Profiler Modules` , và mở nó xuống và chọn các mục `CPU , UI , UI Details`
    - ![image](https://user-images.githubusercontent.com/47918431/135762741-eae6054d-cd04-4df8-8d93-66bc2f075c79.png)
    - kết quả hiển thị :
    - ![image](https://user-images.githubusercontent.com/47918431/135763119-04e82995-1421-46b4-a52c-5f4f0864dd18.png)
    - Biểu đồ giao diện hiển thị thời gian dành cho việc tính toán bố cục và kết cấu . Phần chi tiết giao diện người dùng cung cấp thông tin quan trọng về quá trình chạy của sản phẩm
 - 3: Chọn panel `UIDetails` và ghi lại thành bảng phân tích canvas trong sence của bạn 
 - ![image](https://user-images.githubusercontent.com/47918431/135763092-7ba0abe6-db52-436c-a948-5470fed2a4cd.png)
 - 4 : Click vào 1 phần tử trên giao diện  sẽ thấy điểm được đánh dấu xuất hiện , và điểm được đánh dấu này sẽ hiện thị layout và quá trình render của cpu lúc event được triggered
 - ![image](https://user-images.githubusercontent.com/47918431/136245472-fd424c37-20d1-4c9e-9455-aea40c14a164.png)

https://docs.unity3d.com/2019.1/Documentation/Manual/ProfilerUI.html
https://learn.unity.com/tutorial/ui-profiler-2019-3


<a name="When"></a>
## III. Tổng kết UI and UI Details Profiler
- Markers can be overwhelming, depending on the usecase profiled. Hiding or showing them when needed helps the chart readability.
- To make visibility clearer, you can select the preview background according to the UI you are previewing. A white-ish UI on a white background won’t be readable, for example, so you can change it.
- Detaching the preview allows better screen estate management.
- Overdraw and composite overdraw are used to determine which parts of the UI are drawn for nothing

