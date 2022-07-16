# Caro_Game

1.Evenloop, Callback
-Evenloop
	+ Event loop là cơ chế giúp Javascript có thể thực hiện nhiều thao tác cùng một lúc (concurrency)
	+ Về bản chất, vòng lặp sự kiện(event loop) sẽ kiểm tra xem ngăn xếp(call stack) cuộc gọi có trống không và nếu có, sẽ xem xét hàng đợi sự kiện (event queue).
	Nếu có một cái gì đó trong đó, nó thêm nó vào ngăn xếp(call stack) cuộc gọi và thực hiện nó. 
	Vòng lặp sự kiện(event loop) liên tục chạy cho đến khi hết ca (nội dung trình duyệt được tải / trình duyệt bị đóng). Event table theo dõi tất cả các sự kiện đã được kích hoạt và gửi chúng đến hàng đợi sự kiện(event queue) sẽ được thực thi. 

-Callback
	+ Gọi lại là một function sẽ được thực thi sau khi một function khác đã được thực thi xong 
	+ Trong Javascript, functions là objects,do đó nó có thể nhận tham số là function, và cũng có thể trả về một function. Vì vậy bất cứ function nào được truyền vào như một tham số và được gọi sau đó sẽ có tên là callback function.

2.This trong JS
	+ This trong javascript nó cũng giống như các ngôn ngữ khác, đều là đại diện cho đối tượng hiện tại mà nó đang được sử dụng.
	+ Tất cả các hàm của JavaScript đều có thuộc tính, giống như mọi đối tượng khác. Và khi một hàm được thực thi, nó sẽ có thuộc tính this - một biến với giá trị là đối tượng đã gọi hàm sử dụng this.
	+ This luôn luôn tham chiếu (và có giá trị của) đối tượng - một đối tượng duy nhất - và nó thường được sử dụng bên trong hàm hay phương thức, mặc dù nó có thể dùng được một cách toàn cục bên ngoài hàm.

3.Object trong JS
	+ Object trong JavaScript (đối tượng trong JavaScript) là tập hợp của các cặp key-value. Và property là tên gọi của mỗi cặp key-value, tương tự như bản đồ, từ điển, hay hash-table trong ngôn ngữ lập trình khác.

		*Đối tượng là một tập hợp các thuộc tính
		*Thuộc tính là một cặp khóa - giá trị chứa tên và giá trị
		*Tên thuộc tính là một giá trị duy nhất có thể bị ép buộc vào một chuỗi và trỏ đến một giá trị
		*Giá trị thuộc tính có thể là bất kỳ giá trị nào, bao gồm các đối tượng khác hoặc các hàm, được liên 		kết với tên/khóa

4.Prototype
	+ Prototype là cơ chế mà các object trong javascript kế thừa các tính năng từ một object khác. Tất cả các object trong javascript đều có một prototype, và các object này kế thừa các thuộc tính (properties) cũng như phương thức (methods) từ prototype của mình.


5.Bài tập 
Mô tả ngắn:
	Xây dựng trò chơi cờ caro với JS
		+Chọn số hàng và số cột mong muốn theo số nguyên để tạo ra bàn cờ
		+Nhập tên người chơi
		+Mỗi người chơi 1 lượt đến khi giành chiến thắng
		+Hiển thị ra thông báo tên người chơi chiến thắng
