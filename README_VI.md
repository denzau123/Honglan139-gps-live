# Hồng Lân 139 GPS LIVE — App iPhone

Đây là bản PWA cài như app trên iPhone:
1. Đưa thư mục này lên Firebase Hosting.
2. Mở website bằng Safari.
3. Chọn Chia sẻ → Thêm vào Màn hình chính.
4. App sẽ có icon riêng và mở dạng ứng dụng.

Chế độ PHÁT GPS LIVE cần đăng nhập Firebase bằng tài khoản đã được cấp quyền.
Người xem không cần đăng nhập.

Lưu ý iPhone/iOS: Safari/PWA có thể hạn chế định vị khi app bị đưa xuống nền hoặc máy khóa màn hình. Muốn GPS nền ổn định hơn cần bản native iOS.

## Tính năng Điểm tiếp theo
- Thành viên đăng nhập có thể nhập tên điểm, địa chỉ, giờ show và tọa độ điểm tiếp theo.
- Tọa độ được lưu tại `live/hong_lan_139/nextStop` trong Firebase Realtime Database.
- Người xem thấy điểm tiếp theo, khoảng cách ước tính, ETA và nút xem điểm trên bản đồ.
- Khoảng cách tính đường chim bay bằng Haversine; ETA là ước tính theo tốc độ GPS hiện tại, hoặc 30 km/h khi xe đang chậm/không có tốc độ.
