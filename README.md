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
