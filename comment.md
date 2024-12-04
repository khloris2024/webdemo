# Nhận xét bài làm

## Tổng quan

**Lưu ý:**  trang web launch đầu tiên thường là `index.html` nên em nên đặt tên lại file `home.html` nha.

### Tổ chức folder
Cách tổ chức folder của em chưa được gọn gàng, khó quản lý và deploy. Có nhiều cách tổ chức folder. And gợi ý 1 cách tổ chức folder gọn hơn, phù hợp với bài này:
```css
.
└── btck/
    ├── home.html
    ├── shop.html
    ├── contact.html
    ├── cart.html
    ├── blog.html
    ├── css/
    │   ├── style.css /*CSS dùng chung giữa các trang*/
    │   ├── home.css
    │   ├── shop.css
    │   ├── contact.css
    │   ├── cart.css
    │   └── blog.css
    ├── js/
    │   ├── index.js /*JS dùng chung */
    │   ├── home.js
    │   ├── shop.js
    │   ├── contact.js
    │   ├── cart.js
    │   └── blog.js
    ├── asset/
    │   ├── universal/ /*các file (hình ảnh, logo,...) dùng chung */
    │   ├── home/
    │   │   └── image1.png /*file ví dụ*/
    │   ├── shop/
    │   ├── contact/
    │   ├── cart/
    │   └── blog/
    └── component/ /*những thành phần dùng chung*/
        ├── header.html /*header đầu trang*/
        ├── footer.html
        └── nav.html
```

## HTML

Thay vì đặt tên `div` là *je, he, shh, haha* thì em nên dành thời gian để nghĩ cho nó 1 cái tên dễ hình dung hơn :)))


Khúc này a không hiểu tại sao `div` lớn có `id` là `row` trong khi `div` nhỏ lại có `class` là `row` luôn :)))
```html
<div id="row">
        <div class="row">
            <img src="Mask Group.png" alt="Dining">
            <p>Dining</p>
        </div>
        <div class="row">
            <img src="Image-living room.png" alt="Living">
        <p>Living</p>
        </div>   
        <div class="row">
            <img src="Mask Group (1).png" alt="bedroom">
        <p>Bedroom</p>
        </div>
    </div>
```

Em thiếu nút `Show more` ở cuối `our product`

Trong `shop.html` thì em lại để phần `<img>` ở ngoài `<a>` nên cái nút cart nó không hoạt động

*Code sai*

```html
<div class="sup"><li><a href="cart.html"></a><img src="cart.png"></li></div>
```

*Code đúng*
```html
<div class="sup"><li><a href="cart.html"><img src="cart.png"></a></li></div>
```

Trong `blog.html` và `contact.html`, em không để header trong tag `head`

## CSS
Thiếu CSS cho phần `blog.html`

CSS của em dùng đơn vị là `px` khá nhiều. Theo a thì em nên hạn chế tối đa dùng đơn vị này vì em sẽ tràn hình ảnh ở những màn hình nhỏ hơn. 

1 số webpage của em còn thiếu CSS 

## JS
Em dùng JS để lấy product về và tạo HTML cho product chứ không phải tạo bằng tay.
