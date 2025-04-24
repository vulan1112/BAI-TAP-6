# BAI-TAP-6
VU LAN_K225480106036_Hệ quản trị CSDL
## Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

DEADLINE: 23H59:59 NGÀY 25/4/2025

Ghi chú: Giải thích tại sao lại có SQL như vậy.
## CÁC BƯỚC IMPORT ĐƯỢC DỮ LIỆU TRONG sv_tnut.sql vào trong server.

Tạo cơ sở dữ liệu mới

![Screenshot (11)](https://github.com/user-attachments/assets/b97e1b4b-d8e8-4a2d-b083-3cd53410d671)

Đặt tên cho database

![image](https://github.com/user-attachments/assets/bf5c054a-a1c9-4795-a62f-72d09506a38e)

Đưa dữ liệu vào 

![Screenshot (12)](https://github.com/user-attachments/assets/87e3f6be-b32f-4827-ba24-cef3a8b5f004)

Cuối cùng ta được bảng dữ liệu thông tin sinh viên TNUT như sau:

![Screenshot (13)](https://github.com/user-attachments/assets/8e16ddaa-df59-4a2a-bf68-297455ece44c)

## 2.dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)

![image](https://github.com/user-attachments/assets/769d1180-fd89-4c09-b143-646f5c7d9774)

## 3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em.

![image](https://github.com/user-attachments/assets/69f328c9-9268-4588-ba4b-425dbd03e451)

## 4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em.

![image](https://github.com/user-attachments/assets/debc55a6-9b3d-4c3b-a70b-1aa3b3f39bd0)

## 5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em.

![image](https://github.com/user-attachments/assets/ffa166ed-adc9-42ca-8fcc-830adeeb8d41)

## 6. nhập sql để tìm xem có những sv nào trùng tên với em.

![image](https://github.com/user-attachments/assets/f0cd253d-3dda-4cef-9c5b-1a3facf6a3e0)

## 7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.

![image](https://github.com/user-attachments/assets/7116e718-ef64-4440-904f-576779f098dc)

## 8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.

![image](https://github.com/user-attachments/assets/fe532f20-cb93-4393-a714-866c61db4050)

## 9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.

![image](https://github.com/user-attachments/assets/09b5fd04-8040-4203-90c5-ff4fb3a72007)

**Select**: lấy dữ liệu ở các cột tại bảng SV

**FROM SV**: Chỉ định bảng dữ liệu cần truy vấn là bảng SV

**WHERE lop LIKE '%KMT%'**: điều kiện lọc dữ liệu, lop là cột chứa thông tin lớp học của sinh viên.

**LIKE '%KMT%'**: Tìm tất cả các bản ghi mà cột lop chứa chuỗi 'KMT' ở bất kỳ vị trí nào trong chuỗi giá trị của nó.

**%** là ký tự đại diện cho bất kỳ chuỗi ký tự nào hoặc chuỗi rỗng.

**ORDER BY ten, hodem**: Xắp xếp kết quả trả về theo-Cột tên trước (theo thứ tự từ A → Z)

Nếu các giá trị Tên giống nhau, tiếp tục sắp xếp theo hodem (cũng từ A → Z)

## 10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC).

Theo em các bạn nữ thì thường có họ tên đệm đa số là chữ **Thị** lên em tìm những bạn có tên đệm chữ thị là giả dụ bạn ấy là nữ và học ngành **KMT** .

![image](https://github.com/user-attachments/assets/350a91a0-5cf1-4ebb-ad46-bf2e07c5a5a2)

**WHERE [hodem] LIKE N'%Thị%'** 

 **WHERE** là điều kiện lọc, chỉ chọn những bản ghi thỏa mãn điều kiện này.

**hodem**: Cột này trong bảng **SV** lưu trữ thông tin về họ và đệm của sinh viên.

**LIKE**: Là toán tử dùng để tìm kiếm một mẫu chuỗi trong một cột. Cho phép tìm kiếm một phần của chuỗi, thay vì phải khớp chính xác toàn bộ chuỗi.

**N**: Là tiền tố trong SQL Server để biểu thị rằng chuỗi ký tự sau đó là kiểu nvarchar.

**'%Thị%'**: Đây là mẫu chuỗi mà em đang tìm kiếm trong cột **[hodem]**. Dấu phần trăm % là ký hiệu đại diện cho bất kỳ chuỗi ký tự nào (bao gồm chuỗi rỗng).

**AND [lop] LIKE N'%KMT%'**

**AND**: Đây là toán tử logic dùng để kết hợp các điều kiện trong câu truy vấn. Trong trường hợp này, bạn chỉ chọn những sinh viên có hodem chứa "Thị" và lop chứa "KMT".

**[lop]**: Cột này lưu trữ thông tin về mã lớp của sinh viên.

**LIKE**: được sử dụng để tìm kiếm một mẫu chuỗi trong cột [lop]

**N'%KMT%'**: Mẫu chuỗi này tìm kiếm tất cả các lớp mà chứa từ **KMT**.
