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
