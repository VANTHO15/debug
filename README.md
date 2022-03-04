# Debug in dữ liệu từ chương trình lên console SWV

# Để sử dụng tính năng này, bạn cần:

# Bổ sung đoạn code sau vào trước hàm int main (void) {}
![image](https://user-images.githubusercontent.com/56969447/156747806-dce09dda-7108-44b9-b01d-f38b43330822.png)
# Thêm nội dung bạn muốn in lên console, có thể in dữ liệu ở nhiều kiểu khác nhau:
![image](https://user-images.githubusercontent.com/56969447/156747836-f02640a7-5887-44c6-8595-7ef5fa021439.png)
# Cấu hình Debug: Nhấn chuột phải vào project muốn debug [1], sau đó chọn Debug as [2] và chọn Debug Configuration[3]:
![image](https://user-images.githubusercontent.com/56969447/156747868-1073631d-bed3-4e06-b50d-34df703be202.png)
# Trên cửa sổ Debug Configurations, bạn chọn thẻ Debugger[1], sau đó tích chọn Enable Serial Wire Viewer (SWV) [2], nhấn chọn Apply[3] rồi Debug[4]:
![image](https://user-images.githubusercontent.com/56969447/156747887-291680d8-a8db-4901-8d7c-7ddd8ad0a68f.png)
# Mở giao diện hiển thị dữ liệu: Từ giao diện Debug, chọn Window -> Show View -> SWV -> SWV ITM Data Console:
![image](https://user-images.githubusercontent.com/56969447/156747910-dfd01174-87f1-459c-b949-089fecd97d4e.png)
# Trên diện SWV ITM Data Console, nhấn vào biểu tượng configure trace[1], tích chọn vào Port 0[2] và nhấn chọn Ok[3]. Sau đó chọn biểu tượng Start trace[4] và nhấn vào biểu tượng Resume [5] để bắt đầu chạy debug và quan sát kết quả ở thẻ Port 0 của SWV ITM Data Console [6]
![image](https://user-images.githubusercontent.com/56969447/156747935-26018d25-46cf-4f43-b734-63d1bc3c057c.png)
# Kết quả với ví dụ:
![image](https://user-images.githubusercontent.com/56969447/156747970-52b5109e-f59a-4b4e-b89a-21a16ca3c47e.png)



# Debug vẽ biểu đồ dữ liệu với SWV

# Biến được sử dụng để vẽ biểu đồ là biến toàn cục. Trong ví dụ của mình thì mình khai báo biến toàn cục test: uint8_t test = 0; và thực hiện tăng biến test lên 1 đơn vị sau mỗi 1 giây để thấy sự thay đổi trên biểu đồ:
![image](https://user-images.githubusercontent.com/56969447/156748010-a16e24e4-dc69-49f3-afcc-0804519c5e30.png)
# Nhấn chuột phải vào Project muốn debug [1], sau đó chọn Debug as [2], chọn Debug Configuration [3]:
![image](https://user-images.githubusercontent.com/56969447/156748032-38ba969d-88eb-467b-a277-f439b29a1c68.png)
# Trên cửa sổ Debug Configurations, bạn chọn thẻ Debugger[1], sau đó tích chọn Enable Serial Wire Viewer (SWV) [2], nhấn chọn Apply[3] rồi Debug[4]:
![image](https://user-images.githubusercontent.com/56969447/156748058-934364fe-da7e-400b-9690-6e97b3791413.png)
# Từ cửa sổ Debug, chọn Window -> Show View -> SWV -> SWV Data Trace Timeline Graph:
![image](https://user-images.githubusercontent.com/56969447/156748089-e1e094a3-328b-4044-8429-821acb0ac374.png)
# Tại thẻ SWV ITM Data Console, nhấn vào biểu tượng configure trace[1], tích chọn vào Port 0[2], tích chọn Enable Comparator và điền tên biến muốn vẽ biểu đồ giá trị [3] và sau đó nhấn chọn OK[4]. Chọn biểu tượng Start trace[4], sau đó chọn biểu tượng Resume [5] để bắt đầu chạy debug và quan sát kết quả ở SWV Data Trace Timeline Graph [6]
![image](https://user-images.githubusercontent.com/56969447/156748102-7e22ad4d-fd3a-4030-83d6-0d2c0c088d0e.png)
# Kết quả với ví dụ:
![image](https://user-images.githubusercontent.com/56969447/156748123-bd90047a-46c7-4148-983f-10739258044d.png)

