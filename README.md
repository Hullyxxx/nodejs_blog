# Learning Node JS

## SSR & CSR

- SSR (Server Side Rendering): render giao diện luôn từ server.
    + Điểm mạnh: tốt cho sales, nhanh hơn trong lượt truy cập đầu tiên, thời gian phát triển applications nhanh, dùng cho những project nhỏ.
    + Điểm yếu: phải reload và gửi request khi có một request khác.
- CSR (Client Side Rendering): khá giống SSR nhưng trong html có một thẻ div#main trống và render apend html vào trong đó khi loaded page.
    + Điểm mạnh: không phải gửi request mới khi có một request khác. 
    + Điểm yếu: không phục vụ tốt cho việc sales do không có content nên bot không đọc được content, chậm hơn SSR trong lần truy cập đầu tiền.

## Install Framework Using in Nodejs

- `npm instal {tên thư viện}`

## Init Source 

- `npm init`: init source one project nodejs.

***IP Localhost***
- `127.0.0.1`

## Template Engine (handlebars)
- Layouts dùng để viết html giao diện chung
- Khi render html, mặc định vào project và tìm thư mục `views` => Phải config lại để control thư mục render
- Thư viện yêu cầu phải có `layours header and footer` và render html vào giữa.
- Config lại để đặt tên thục mục cho ngắn => Đọc docs (bỏ `config option vào function khi gọi function chạy thư viện`)
- Trong thực tế header và footer có rất nhiều layouts khác => tách cái layouts ra từng file riêng bằng cách tạo partials folder chứa các file layouts đó
 + Sau đó sử dụng syntax: `{{> foo/bar }}` để import thư mục đó vào