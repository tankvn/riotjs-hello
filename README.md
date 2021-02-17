# riotjs-hello

### Một số tính năng

- Riot.Js cho phép người dùng áp dụng các thẻ HTML tùy chỉnh trên tất cả các trang và ứng dụng web. Bạn cũng có thể sử dụng lại các thẻ đó.
- Framework này tương tự như polymer và Reac.js. Tuy nhiên, so với hai framework kia, Riot.Js có tổ chức và nhỏ gọn hơn.
- Framekwork này tập trung cao độ vào các chức năng vi mô cho phép bạn làm việc cá nhân với các ứng dụng khác nhau cùng một lúc.


Riot lấy cảm hứng WebComponent từ React và Polymer, nhưng tinh gọn hơn rất nhiều. Thư viện này ra đời cuối năm 2013, sau React vài tháng. Hiện nay vẫn rất active. Hầu hết issues đều được giải quyết nhanh chóng.

Riot cung cấp cho bạn custom tags, observable và routing. Custom tags cho phép tạo ra các components, observable giúp các components này giao tiếp với nhau, còn routing là để map URL vào component tương ứng. Chừng đó xem như đủ cho bạn làm bất cứ điều gì với web apps.

Giống như React, Riot là UI framework, không có sẵn kiến trúc. Tất nhiên bạn có thể đem những pattern phổ biến như Redux, Flux bên React vào cho Riot.

Đặc biệt Riot hỗ trợ preprocessor, trong file components bạn có thể viết script bằng coffee, typescript, hoặc es6; hoặc thay HTML tag bằng Pug syntax. Nếu cần, bạn có thể tùy biến parser function để hỗ trợ thêm các processor khác.

Sample code:
```js
<todo>
	<h3>TODO</h3>

	<ul>
		<li each={ item, i in items }>{ item }</li>
	</ul>

	<form onsubmit={ handleSubmit }>
		<input ref="input">
		<button>Add #{ items.length + 1 }</button>
	</form>

	this.items = []

	handleSubmit(e) {
		e.preventDefault()
		var input = this.refs.input
		this.items.push(input.value)
		input.value = ''
	}
</todo>
```

### Every revolution begins with a Riot.js

Tôi bắt đầu sử dụng `Riot.js` vài năm trước và nó đã thay đổi phong cách phát triển ứng dụng web của tôi.

Tôi đã rất mệt mỏi khi phải học mỗi ngày những khái niệm mới và những cách phức tạp để tạo ra những thành phần tầm thường luôn giống nhau (đàn accordion, lớp phủ, trường nhập tùy chỉnh…).

Làm việc với `Riot.js` giúp tôi hiểu ra rằng ngay cả những tính năng phức tạp nhất cũng có thể đạt được với sự sang trọng và ít mã dựa vào sức mạnh của các thành phần web.

#### Riot.js 4

Riot.js 4 nhằm mục đích trở thành khung nhỏ nhất, đơn giản nhất và dễ dự đoán nhất cho các thành phần web. Nó được thiết kế để cung cấp cho bạn mọi thứ mà bạn mong muốn API các thành phần web gốc trông như thế nào. 


### Riot Modal

This a simple modal made with riot and [Animate.css](https://daneden.github.io/animate.css/).  
This demo also demonstrates the use of [slots](https://riot.js.org/documentation/#slots).

[Demo](https://riot.js.org/examples/plunker/?app=modal)


### Cheat Sheet
album
https://getbootstrap.com/docs/5.0/examples/album/

cheatsheet
https://getbootstrap.com/docs/5.0/examples/cheatsheet/

elements
https://folio.webestica.com/elements-accordion.html


### Releases
- v5.3.0  - Feb 13, 2021
- v4.14.0 - Sep 01, 2020
- v3.13.2 - Nov 25, 2018
- v2.6.9  - Feb 15, 2019
- v1.0.4  - Sep 17, 2014


### Những trình duyệt nào được hỗ trợ?

Riot.js 4 hỗ trợ tất cả các trình duyệt hiện đại chính. Các trình duyệt như IE11 không được hỗ trợ: nếu bạn cần hỗ trợ các trình duyệt cũ hơn, bạn có thể cân nhắc sử dụng phiên bản Riot cũ hơn

https://github.com/riot/riot  
https://github.com/riot/examples  