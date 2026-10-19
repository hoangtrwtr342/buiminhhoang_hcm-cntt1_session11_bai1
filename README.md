# Bài 1 : Chuẩn hóa Heading Styles cho tài liệu SRS

## Phần 1: Phân tích nguyên nhân sự cố
  
  1.1 Tại sao định dạng thủ công gây lỗi "No table of contents entries found

Định dạng thủ công (Direct/Manual Formatting): Khi Nam tăng cỡ chữ lên 18, 20 hay in đậm, thuộc tính cốt lõi của đoạn văn đó trong hệ thống của Word vẫn là Style Normal với Outline Level: Body Text (nội dung thân bài).

Cơ chế thu thập của Auto TOC: Mặc định, công cụ Auto TOC chỉ lọc các đoạn văn bản có Outline Level từ 1 đến 3 (tương ứng với các style Heading 1, Heading 2, Heading 3).

Hậu quả: Khi chạy lệnh tạo mục lục, Word quét toàn bộ văn bản nhưng không tìm thấy đoạn nào có Outline Level hợp lệ để trích xuất, dẫn đến thông báo: "No table of contents entries found". 
Việc định dạng thủ công còn làm mất khả năng quản lý đồng bộ—khi muốn đổi màu hay font, người dùng buộc phải sửa thủ công từng trang thay vì cập nhật tập trung tại Styles pane

 1.2. Lỗi sai khiến đoạn văn 5 trang bị đẩy vào mục lục
Có hai nguyên nhân trực tiếp dẫn đến hiện tượng một đoạn văn bản dài xuất hiện trong mục lục : 
Gán nhầm phạm vi Style: Nam đã bôi đen (hoặc vô tình áp dụng) style Heading 1 cho cả khối nội dung thân bài thay vì chỉ áp dụng cho dòng tiêu đề ngắn gọn.

Kế thừa Style và ngắt dòng sai cách : 
Nếu Nam gõ tiêu đề ở dạng Heading 1, sau đó nhấn Shift + Enter (ngắt dòng mềm - Line Break) thay vì Enter (ngắt đoạn - Paragraph Break), Word sẽ coi toàn bộ văn bản tiếp theo thuộc cùng một đoạn văn với tiêu đề và mang trọn vẹn style Heading 1.

Hoặc trong thiết lập của style Heading 1, thuộc tính Style for following paragraph chưa được đặt về Normal, khiến khi gõ xong tiêu đề và bấm Enter, các đoạn văn bản sau tự động kế thừa luôn style Heading 1.  


## Phần 2: Quy trình khắc phục và chuẩn hóa tài liệu SRS

1. Khắc phục lỗi đoạn văn 5 trang

Trước khi dựng lại mục lục, cần trả lại đúng thuộc tính cho phần nội dung thân bài:

Nhấn Ctrl + F để mở thanh Navigation, chọn tab Headings.

Tìm đến mục tiêu đề bị kèm khối văn bản 5 trang để định vị nhanh.

Bôi đen toàn bộ đoạn văn bản 5 trang đó (loại trừ dòng tiêu đề thực sự).

Nhấn tổ hợp phím Ctrl + Shift + N (hoặc chọn style Normal trên thanh công cụ Home > Styles) để đưa đoạn văn về định dạng chuẩn của thân bài.
