---
title: Hướng dẫn Reload css trình duyệt khi thay đổi Style.css
categories: tips
description: KKhi thay đổi Style.css mà ta không reload css (tải lại css) có thể không thấy sự thay đổi làm ta nhầm là bị lỗi, lý do và khắc phục như sau
thumbnail: /images/posts/huong-dan-reload-css-trinh-duyet-khi-thay-doi-file-style-css.jpeg
---

Khi chúng ta thiết kế website thường sử dụng các dòng lệnh CSS để thay đổi va tùy biến giao diện.

Nhưng khi thay đổi xong Css trong file style.css rồi ra ngoài tải lại trang web lại không thấy có thay đổi gì? Tại sao? chúng ta hãy xem nguyên nhân và giải pháp
## Cache ( Bộ nhớ đệm) của trình duyệt là nguyên nhân?
Kì thực các bạn có biết tại sao website bạn đã truy cập 1 lần rồi, lần sau truy cập vào cảm thấy nhanh hơn rất nhiều?

Chính là bởi vì cái trình duyệt ( ví dụ : Chrome, Cốc cốc, firefox…) của các bạn nó đã tự động tải trước một số các file ( trong đố có File CSS, nó lưu lại trong 1 bộ nhớ đệm( Cache).

Như tôi đã bàn tới, nó lưu lại với mục đích chủ yếu là giúp tắc tốc website của bạn, tránh tải đi tải lại các tài nguyên cố đinh.

Như vậy CSS là 1 tài nguyên được tải trước trong bộ nhớ đệm CACHE vì vậy nên trong các lần tải tiếp theo, trình duyệt sẽ nhớ và lấy CSS của lần đã tải trước đó.

## Vậy muốn thay đổi CSS website thì làm cách nào?
Chúng ta vừa đặt ra vấn đề nếu thay đổi CSS website thì chẳng phải sẽ bất tiện lắm sao? tại sao. Vì Css sẽ không được load lại.

Chúng ta yên tâm, Cache của trình duyệt sẽ được làm mới lại sau một thời gian nhất định.

Tuy nhiên Nếu bạn là 1 người Thiết kế website , liên tục thay đổi CSS thì sao nhỉ ? Thực ra chúng ta cũng các cách chủ động thông báo cho trình duyệt rằng có sự thay đổi, cần cập nhật lại CSS của một website nào đó.

Chúng ta có thể chủ động Tải lại CSS mới của website bằng 2 cách:

Nhanh nhất là Sử dụng tổ hợp phím Ctrl + F5:

Cách sử dụng: 1 lần, 2 lần, và nhiều lần hơn một chút. Nếu nó không thay đổi sau vài lần thực hiện tổ hợp phím.

Hãy xem cách sau dưới đây .

## Sử dụng Tiện ích mở rộng Auto Reload CSS
### #1: Bạn hãy cài đặt tiện ích mở rộng trên Google Chrome
Tên của tiện ích là Css Reloader . Chúng ta bắt đầu các bước cài đặt theo video sau đây :

#đang cập nhật …. còn tiếp