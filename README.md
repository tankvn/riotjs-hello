# riotjs-hello

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




### Releases
- v5.3.0  - Feb 13, 2021
- v4.14.0 - Sep 01, 2020
- v3.13.2 - Nov 25, 2018
- v2.6.9  - Feb 15, 2019
- v1.0.4  - Sep 17, 2014