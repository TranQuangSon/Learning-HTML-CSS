- Cùng cấp _./_
- Truy xuất ra ngoài 1 cấp _../_
- Thuộc tính _attribute_
- Thẻ _tag_:
- price: giá
- image: hình ảnh

- CSS nó sẽ chạy từ trên xuống dưới, nếu có cùng 2 đoạn thực hiện cùng chức năng thì nó sẽ ưu tiên đoạn code ở dưới
- _div_ là thẻ block, có độ rộng 100% phần tử chứa nó, lưu ý: chưa nói tới vấn đề khi sử dụng vs CSS
- _img_ là thẻ inline, tự động, dùng để hiển thị hình ảnh vs 2 thuộc tính là `src` và `alt`
- _alt_ viết tắt của `alternate text` nó dùng trong việc SEO, khi hình ảnh bị lỗi hoặc sai đường dẫn thì _alt_ sẽ hiển thị để người dùng biết hình ảnh đó nói về cái gì
- _span_ là thẻ inline, nó thường được dùng cho những đoạn chữ ngắn
- _class_ là thuộc tính dùng để sử dụng các class cho thẻ, sau dùng để styles trong CSS
- Việc đặt tên class khá là nan giải, khó, ko nên đặt tên Tiếng Việt, nên đặt Tiếng Anh ngắn gọn dễ hiểu 
- Thẻ  tiêu đề: h1 -> h6
- _h1_: mỗi trang chỉ tối đa 1 thẻ h1 , dùng cho những tiêu đề lớn của trang
- _h2_: dùng được nhiều, dùng cho những block to
- _h3_: dùng được nhiều, dùng cho những block nhỏ
- Thẻ _a_: là thẻ inline, chắc chắn là dùng cho liên kết, nó có 3 thuộc tính hay dùng `href`,
`target`(nhấn vào liên kết sẽ chuyển sang tab mới), `rel`
- Khi dùng `target` có giá trị _blank_ thì thêm thuộc tính rel = "noopener noreferrer"
- Fonts chữ:
- 1. Có sẵn ở Google Fonts
- 2. Không có ở Google mà phải mua ở trên mạng
- _font-weight_: độ đậm nhạt của chữ, từ 100 -> 900, normal, bold, bolder, extra bold, light, thin, regular, medium, semibold
- _font-family_: thiết lập font chữ, truyền vào là font name(tên của font chữ)
- _san-serif_: chữ không chân
- _serif_: chữ có chân
- CSS Selectors: _tag_, _class_, _id_, _attribute_
- Tags: _h1_, _h2_, _h3_, _div_, _body_, _span_, _a_
- Class: .name, .tour, .tour-content
- Id: #header, #content
- Attribute: Later `*`
- Special selector: \*(bao quát hết selector)
- _user agent stylesheet_: CSS mặc định của trình duyệt, mỗi trình duyệt sẽ có CSS mặc định khác nhau
- CSS Reset: dùng để reset lại CSS mặc định của các trình duyệt, `bắt buộc` phải có đầu tiên
- **box-sizing**
- _shorthand_: viết rút gọn
- _box-sizing_: margin, padding, border, width, height, đơn vị px
-_content-box_: độ rộng lúc này của 1 khối sẽ bằng width + padding (left + right) + border(left + right)
- _border-box_: độ rộng của 1 khối sẽ bao gồm cả padding và border, nên áp dụng cho toàn bộ selector (\*)
- _width_: chiều rộng
- _height_: chiều cao
- _border_: viền
- _color_: màu chữ
- _backgroud-color_: màu nền
- _padding_: không thể dùng số âm
- _margin_: có thẻ dùng số âm, có giá trị `auto`
- _text-decoration_: gạch chân dưới thẻ a, `none`, `underline`, `overline`
- _border-radius_: độ bo góc của khối, càng lớn thì càng bo góc, hình vuông thì ra tròn, chữ nhật thì ra elip
- _line-height_: khoảng cách giữa các dòng chữ
- Khi những thẻ inline nằm cạnh nhau thì nó sẽ nằm trên 1 hàng, ngược lại những thẻ block thì nó sẽ tạo ra hàng mới 
- _display_: block, inline, inline-block, none, flex, grid
- `block`: biến thành thẻ block
- `inline`: biến thành thẻ inline, nó sẽ bị hạn chế vài thuộc tính CSS liên quan tới box-sizing như padding-top, padding-bottom, margin-top, margin-bottom
- `inline-block`: biến thành thẻ inline-block, là sự kết hợp giữa inline và block, khi các thẻ có thuộc tính inline-block nó sẽ kế thừa đặc tính của inline-block tức là nằm cạnh nhau thì sẽ nằm trên 1 hàng, có độ rộng bằng nội dung mà nó chứa, không bị hạn chế CSS
- `none`: ẩn, không thấy không nhấn được
- `flex`: dùng rất nhiều hiện nay
- _min-width_: độ rộng tối thiểu, vd 100px thì sẽ >= 100px
- _max-width_: độ rộng tối đa, vd 100px thì sẽ chỉ =< 100px
- _flex-box_: áp dụng thuộc tính `display: flex` vào phần tử mình muốn dàn layout
- _flex-direction_: `row` là các cột từ trái qua phải, `row-reverse` là các cột từ phải qua trái, `column` là các cột theo chiều dọc từ trên xuống dưới, `column-reverse` thì ngược
- _calc_: hàm dùng để tính toán, + - * /, lưu ý phải có khoảng cách giữa các phép tính
- _align-items_: `stretch` là thuộc tính làm cho các cột bằng nhau, `flex-start` là căn phần trên đầu, `flex-end` là căn phần ở dưới, `center` là căn giữa vs nhau, `baseline` là các dòng chữ đầu tiên bằng nhau
- _flex-wrap_: `nowrap` là không cho phép xuống hàng, `wrap` là cho phép xuống hàng
- _oject-fit_: `cover` thường được dùng cho thẻ ảnh, dùng để phủ hết khung khoảng trống, không làm cho ảnh bị méo
- Day 2:
- _justify-content_: `flex-start` là các phần tử nằm dồn về phía bên trái, `flex-end` thì các phần tử nằm dồn về phía bên phải, `center` là các phần tử nằm ở giữa, `space-between` là các phần tử nằm đầu và cuối, `space-around` là khoảng trống xung quanh, ở giữa gấp đôi, `space-evenly` là khoảng trống xung quanh bằng nhau
- _column-gap_: khoảng trống chiều dọc
- _row-gap_: khoảng chống chiều ngang
/* gap: 30px 30px; row-gap - column-gap */
- _overflow_: `hidden` là dạng không cho chữ bị tràn ra bên ngoài, 
- _word-break_: `break-all` khi hết đoạn thì một từ sẽ tự động ngắt ở bất kỳ chữ nào để xuống hàng, `break-word` xuống dòng theo từ tùy thuộc khoảng trống bao nhiêu
- _white-space_: `nowrap` không cho chữ xuống hàng, luôn luôn nằm trên 1 hàng
- _text-overflow_: `ellipsis` hiện dấu 3 (...) trên đoạn
- _text-truncate_: (evondev) có 2 dòng, hiện 3(...)
Day 3
- _component_: mục đích là tái sử dụng vào có thể tùy chỉnh 1 chỗ để sử dụng nhiều nơi
- _pug_: 
Day 4
- _mixins_: giống function trong JavaScript mục đích là tái sử dụng code

- _position_: có 5 giá trị chính: `static`, `relative`, `absolute`, `sticky`, `fixed`, khi sử dụng thuộc tính position này thì đi kèm sẽ có các thuộc tính khác như top, right, bottom, left z-index
- `relative`: khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là `absolute` hay không?
- `absolute`: khi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó gần nhất có sử dụng position là absolute hay relative không?

Day 5
- _reponsive_: sử dụng HTML và CSS để tự động thay đổi kích thước, ẩn, thu nhỏ hoặc phóng to trang web để làm cho trang web trông đẹp mắt trên tất cả các thiết bị (máy tính để bàn, máy tính bảng và điện thoại)
- _breakpoints_: 320px, 480px, 768px, 1024px, 1200px, 1366px, 1440px, 1600px, 1920px
- _min-width_: (media queries)
/* @media screen and (min-width: breakpoints) */
- _max-width_:  (media queries)
/* @media screen and (max-width: breakpoints - 0.2px) */
- _media queries_

Day 6:
- _transform_: translate(translateX(value), translateY(value)), skew(skewX, skewY), rotate(rotateX, Y, Z), scale(X, Y)
- `translateX`: Nếu giá trị là số dương thì nó sẽ di chuyển qua bên phải, ngược lại thì di chuyển qua bên trái
- `translateY`: Nếu giá trị là số dương thì nó sẽ đi xuống, ngược lại thì sẽ đi lên 
- `value`: 10px, 20px, -15px, -30px, 10%(lưu ý: khi sử dụng % thì % ở đây chính là độ rộng hoặc chiều cao của khối chúng ta đang áp dụng thuộc tính transform và hàm translate)

Day 7:
- _variables_: biến là gì? khai báo như thế nào? Cách sử dụng ra sao? Ưu và nhược điểm nó là gì?
- Biến là khai báo 1 giá trị để có thể sử dụng đi sử dụng lại ở nhiều chỗ, khi muốn cập nhật thì cập nhật ở 1 chỗ 
- Thường sẽ khai báo ở `root`:
Khai báo:
 --primary-color: orange;
 --secondary-color: blue;
 --text-color: red;
 --font-size-sm: 16px;
- Cách sử dụng: var(--font-size-sm)

Day 8:
- _display_: `grid` là một tổ hợp của những đường ngang và dọc cắt nhau – một nhóm xác định các cột và nhóm kia xác định các hàng
- _grid-template-columns_: sẽ tương ứng với số cột, các giá trị sẽ tương ứng với chiều rộng của các cột lần lượt từ trái sang phải
- _grid-template-rows_: sẽ tương ứng số hàng, các giá trị sẽ tương ứng với chiều cao của các hàng lần lượt từ trên xuống dưới
- 1fr = fraction unit
- _grid-auto-flow_ : `column` sẽ tương thích vs số cột nằm trên 1 hàng ko bị xuống dòng