# Mạch thời gian thực MKE-M09 RTC DS1307 Module

## Giới thiệu

MKE-M09 RTC DS1307 Module là mạch đồng hồ thời gian thực (Real Time Clock - RTC) được sử dụng để cung cấp thông tin chính xác về giờ, phút, giây, thứ, ngày, tháng và năm trong các ứng dụng cần theo dõi và đồng bộ với thời gian thực tế. Module sử dụng IC DS1307 và giao tiếp I²C, cho phép kết nối dễ dàng với vi điều khiển chỉ thông qua hai chân tín hiệu SDA (Data) và SCL (Clock). Module tích hợp pin CR1220 giúp duy trì thời gian ngay cả khi mất nguồn chính, đảm bảo dữ liệu thời gian luôn được lưu giữ liên tục

Module được ứng dụng rộng rãi trong nhiều hệ thống như: đồng hồ điện tử, máy chấm công, hệ thống ghi dữ liệu (Data Logger), bộ điều khiển tưới cây theo lịch, hệ thống báo thức, nhà thông minh, bộ điều khiển đèn tự động, máy cho ăn tự động, trạm quan trắc môi trường và các thiết bị IoT cần lưu trữ thời gian chính xác.

Sản phẩm được thiết kế đặc biệt phù hợp cho các mô hình robot, dự án STEM, đồ án học tập và thực hành điện – điện tử, giúp người học dễ dàng tiếp cận nguyên lý hoạt động của đồng hồ thời gian thực, giao tiếp I2C và kỹ thuật đồng bộ dữ liệu theo thời gian. Đây là công cụ lý tưởng cho học sinh, sinh viên, giáo viên giảng dạy STEM và những người yêu thích nghiên cứu sáng tạo.

MKE-M09 RTC DS1307 Module hỗ trợ điện áp giao tiếp 3.3V và 5VDC, cho phép kết nối trực tiếp và an toàn với Arduino, Raspberry Pi, NVIDIA Jetson, Micro:bit và nhiều nền tảng điều khiển khác. Sản phẩm đi kèm cáp kết nối 4P XH2.54 – Dupont, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

## Thông số kỹ thuật
- Điện áp hoạt động: 5VDC
- Chuẩn giao tiếp: Digital I2C
- Các chân giao tiếp:
  - SDA (Serial Data)
  - SCL (Serial Clock)
- Điện áp giao tiếp: TTL 3.3/5VDC
- IC thời gian thực: DS1307
- Tích hợp pin CR1220 lưu giữ thời gian khi không cấp nguồn
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Hoạt động ổn định, chống nhiễu tốt
  - Giao tiếp đơn giản chỉ với 2 dây tín hiệu
  - Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 4P XH2.54 – Dupont


## Các chân tín hiệu
<table><thead>
  <tr>
    <th>MKE-M09</th>
    <th>Ghi chú</th>
  </tr></thead>
<tbody>
  <tr>
    <td>GND</td>
    <td>Chân cấp nguồn âm 0VDC</td>
  </tr>
  <tr>
    <td>5V</td>
    <td>Chân cấp nguồn dương 5VDC</td>
  </tr>
  <tr>
    <td>SDA</td>
    <td>Chân tín hiệu I2C Serial Data</td>
  </tr>
  <tr>
    <td>SCL</td>
    <td>Chân tín hiệu I2C Serial Clock</td>
  </tr>
</tbody>
</table>

## Hướng dẫn sử dụng
### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân GND và 5V.
- Kết nối chân SCL của Module với chân I2C Clock của mạch điều khiển.
- Kết nối chân SDA của Module với chân I2C Data của mạch điều khiển.

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu **"MKE_M09_RTC_DS1307_Serial_XXX"** tại **File / Examples / MAKEREDU / Module / MKE_M09_RTC_DS1307**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port** của mạch và nhấn **Upload** để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân SDA và SCL của Module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import** chương trình theo đường link sau: `https://github.com/makereduvn/mke_m09_rtc_ds1307_microbit/`
- Kết nối mạch Micro:bit và **Download** chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân SDA và SCL của Module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT** trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT** sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-09 RTC DS1307](/extras/MKE-M09_1.jpg)

## Hình ảnh sản phẩm
![MKE-09 RTC DS1307](/extras/MKE-M09_2.png)
![MKE-09 RTC DS1307](/extras/MKE-M09_3.png)
