# zalo-auto-message-v2
Gửi message tự động lên zalo

## Các bước thực hiện
- Bước 1: Người dùng chọn số lượng tin nhắn gửi đi trong mỗi lần tool chạy
  - Ví dụ: 1 tin nhắn; 2 tin nhắn; 3 tin nhắn ...
  ![image](https://github.com/user-attachments/assets/54e2579c-820a-4edf-9650-bff38ba5cf49)

- Bước 2: Người dùng nhập nội dung tin nhắn sau khi có tin nhắn hiệu lệnh bắt đầu gửi
  - Nếu có nhiều kiểu tin nhắn hiệu lệnh bắt đầu gửi thì mỗi hiệu lệnh phân biệt bằng **dấu ;**
    - Hiệu lệnh cuối cùng không được viết thêm dấu ; ở cuối
    - Ví dụ tool sẽ bắt khi có 1 trong 2 hiệu lệnh tin nhắn mới là **Bắt đầu** hoặc **Bắt đầu khóa căn** để bắt đầu chạy tool, thì sẽ nhập vào ô input như sau: **bắt đầu; bắt đầu khóa căn** (chú ý: không cần viết chứ in hoa vì trong code đã check hết cả trường hợp tin nhắn viết bằng chữ hoa chứ thường hết rồi, chỉ cần nhập đúng nội dung tin nhắn hiệu lệnh là được)
    ![image](https://github.com/user-attachments/assets/85ba5c89-ad9c-4621-aae0-5774639dbd65)

  - Nếu chỉ có 1 kiểu tin nhắn bắt hiệu lệnh thôi thì **không cần viết thêm dấu ;**
    - Ví dụ: Bắt đầu khóa căn
    ![image](https://github.com/user-attachments/assets/8afb8b10-8a2c-49f2-9184-fb68ecb23eb0)

  - Nếu không nhập nội dung gì thì **tuyệt đối không nhập bất cứ kí tự nào** tức là gửi tin nhắn không cần hiệu lệnh để bắt đầu gửi
    - Ví dụ: nếu không cần hiệu lệnh để bắt đầu thì để như hình ảnh bên dưới
    ![image](https://github.com/user-attachments/assets/19f33a3c-2773-41d8-a00d-b81ffd55a9c2)

- Bước 3: Người dùng nhập nội dung tin nhắn các lô cần chốt
  - Các lô cần chốt phân biệt với nhau bằng **dấu ;** và **lô cuối cùng không viết dấu dấu ;**
    - Ví dụ: Lock KTL 01; Lock KTL 02
    ![image](https://github.com/user-attachments/assets/7e67e12a-6d8c-491f-9e09-ca783fc14096)

- Bước 4: Ấn **Gửi tin nhắn** thì sẽ xuất hiện một thông báo **Có x tin nhắn. Bắt đầu gửi** thì ấn **OK** để bắt đầu chạy tool (nếu ko bấm ok thì tool vẫn chưa chạy)
  - Ví dụ:
  ![image](https://github.com/user-attachments/assets/defc4aa9-7ae1-4dfc-8fa0-31b29f66f98e)

- Bước 5: Ngồi đợi tool chạy. trong lúc tool đang chạy thì **không được tắt màn hình, không được chuyển sang tab google mới, không mở thêm tab mới ở google ví dụ như youtube, facebook để tránh tốn nhiều ram và làm lag máy tính sẽ làm cho tool không chạy đúng được** cho đến khi tool chạy thành công.
  - Ví dụ: nhấn phím **Windows** (hoặc hình biểu tưởng window) sau đó nhập **Task Manager** để mở trình quản lý tác vụ lên để xem xem máy tính có đang có dấu hiệu bị lag ko. Nếu phần memory >=85% và cpu >= 70% thì máy tính đang phải làm việc rất nhiều, thì khi chạy tool có thể làm cho tool chạy không chính xác.
    ![image](https://github.com/user-attachments/assets/38af73b0-32df-483e-8a1f-e8c8ba838629)

- Bước 6: Lưu ý
  - Với trường hợp gửi tin nhắn không cần có hiệu lệnh tin nhắn để bắt đầu. Khi ấn Gửi tin nhắn, xong có thông báo xác nhận, nhấn OK mờ tin nhắn không được gửi luôn thì là do tool chưa cập nhật được tin nhắn mới nhất. Thực hiện thao tác cuộn con lăn chuột lên trên xuống dưới một tí để tool cập nhật được tin nhắn mới nhất.
    - Ví dụ: cuộn con lăn lên trên để xem các tin nhắn trước đó một chút ![image](https://github.com/user-attachments/assets/5a8b0c72-49d6-4d2b-87a4-9f335d94118a)
    Sau đó lại cuộn xuống dưới để tool cập nhật được tin nhắn mới nhất. (Nếu tool tự động gửi tin nhắn sau khi bấm xác nhận OK rồi thì ko cần thực hiện cuộn tin nhắn nữa, để cho tool chạy tự động)
  - Với trường hợp tool đang chạy tự động rồi, nhưng để đảm báo tool chắc chắn đang hoạt động thì sau khoảng thời gian tầm 5 phút thực hiện click chuột phải vào đoạn chát tin nhắn trên zalo, hoặc cuộn tin nhắn lên trên hoặc xuống dưới để web zalo biết người dùng vẫn đang hoạt động trên đoạn chat. Để tránh trường hợp trình duyệt phát hiện người dùng ko có bất cứ hành động nào trên zalo thì sẽ giải phóng hay tạm chạy script của tool.
    - Ví dụ: sau khoảng thời gian 3 đến 5 phút click chuột 1 lần vào đoạn chat zalo để trình duyệt biết người dùng vẫn còn đang trong đoạn chat (chú ý ấn click 1 lần vào đoạn chát thôi, ấn 2 lần sẽ rep lại tin nhắn của một người nào đó, hoặc đơn giản là cứ cuộn chuột lên trên rồi xuống dưới kiểu như giả lập rằng mình đang đọc tin nhắn từ đoạn chát)
    ![image](https://github.com/user-attachments/assets/796d846c-0ac8-4213-b0df-72144aabaed6)
  - Trong một số trường hợp nếu tool hoạt động không đúng. Thì vào lại trong extensions của google xong ấn vào nút khoanh màu đỏ để Làm mới lại tool gửi đi
    ![image](https://github.com/user-attachments/assets/25ce73a1-6e14-4805-9e44-9b1f9217e4d7)


- Bước 7: Khi có thông báo **Đã gửi thành công x tin nhắn**. Ấn **OK** để xác nhận với Tool
  ![image](https://github.com/user-attachments/assets/34abb255-9ad4-4eaf-8825-2d280ddfb129)

- Bước 8: Kết thúc Gửi tin nhắn
- Bước 9: Lưu ý: Trong quá trình test tool thì không nói. Nhưng trước khi chuẩn bị gửi tin nhắn lên lock căn lên nhóm zalo thật. thì trước khi thực hiện các bước từ 1 đến bước 8 như hướng dẫn ở trên thì cần Reload lại trang zalo web để làm mới và để tool chạy ổn định nhất có thể.
  - Ví dụ: ấn nút làm mới để làm mới lại trang zalo trước khi thao tác từ bước 1 đến bước 8
    ![image](https://github.com/user-attachments/assets/198462ff-8077-4266-9d2c-7a7aa2098d60)
- Bước 10: Cảnh báo: trong quá trình chạy tool cứ 30s tool lại check kết nối tới zalo một lần, nếu không kết nối được tới zalo thì sẽ có thông báo như ảnh bên dưới. Lúc đó người dùng cần thực hiện bấm OK để xác nhận cảnh báo và Reload lại trang zalo ngay. Tránh để lâu thì cứ 30s lại có thông báo cảnh báo như hình bên dưới 1 lần. Nếu cứ để cảnh báo như vậy lâu mờ ko Reload lại trang thì sẽ làm cho web zalo bị lag, đơ. 
![image](https://github.com/user-attachments/assets/172f9aa9-4ff6-452f-8569-b482186e8b3c)

