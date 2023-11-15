# DAP304x_asm1_khoanfx20883-funix.edu.vn
Test Grade Calculator là một chương trình để tính toán điểm thi cho nhiều lớp với sĩ số hàng nghìn học sinh. Mục đích của chương trình giúp giảm thời gian chấm điểm,áp dụng các functions khác nhau trong Python để viết chương trình với các tác vụ sau: 

1. readByFileName() cho phép người dùng nhập tên của một tệp và truy cập đọc: Mở các tập tin văn bản bên ngoài được yêu cầu với exception-handling. Nếu tệp tồn tại, bạn có thể in ra một thông báo xác nhận. Nếu tệp không tồn tại, bạn nên cho người dùng biết rằng không thể tìm thấy tệp.

2. matchAnswersFormat(answer) quét từng dòng của câu trả lời bài thi để tìm dữ liệu hợp lệ và cung cấp phân tích dữ liệu có trong tệp bạn vừa mở để đảm bảo rằng nó ở đúng định dạng. 
Mỗi tệp dữ liệu chứa một loạt câu trả lời của học sinh ở định dạng sau:
- Một dòng hợp lệ chứa danh sách 26 giá trị được phân tách bằng dấu phẩy
- N# cho một học sinh là mục đầu tiên trên dòng. Nó phải chứa ký tự “N” theo sau là 8 ký tự số.
-Nếu không có chữ cái nào sau dấu phẩy, điều này có nghĩa là học sinh đã bỏ qua việc trả lời câu hỏi.
- Báo cáo tổng số dòng dữ liệu hợp lệ trong tệp.
- Báo cáo tổng số dòng dữ liệu không hợp lệ trong tệp.

3. gradingAnswers(answersFile) lấy tệp dữ liệu hợp lệ từ readByFileName() để chấm điểm từng bài thi dựa trên tiêu chí đánh giá (rubric) được cung cấp và báo cáo chấm điểm các bài thi gồm 25 câu hỏi, trắc nghiệm dựa trên một chuỗi đại diện cho các câu trả lời là answer_key như sau:
+4 điểm cho mỗi câu trả lời đúng
0 điểm cho mỗi câu trả lời bị bỏ qua
-1 điểm cho mỗi câu trả lời sai

Tính toán các thống kê sau cho từng lớp:
- Đếm số lượng học sinh đạt điểm cao (>80).
- Điểm trung bình.
- Điểm cao nhất.
- Điểm thấp nhất.
- Miền giá trị của điểm (cao nhất trừ thấp nhất).
- Giá trị trung vị (Sắp xếp các điểm theo thứ tự tăng dần.).
- Trả về các câu hỏi bị học sinh bỏ qua nhiều nhất theo thứ tự: số thứ tự câu hỏi - số lượng học sinh bỏ qua -  tỉ lệ bị bỏ qua
- Trả về các câu hỏi bị học sinh sai qua nhiều nhất theo thứ tự: số thứ tự câu hỏi - số lượng học sinh trả lời sai - tỉ lệ bị sai

 4. saveGrade (className,scoreList) tạo một tệp “kết quả” chứa các kết quả chi tiết cho từng học sinh trong lớp của bạn. Mỗi dòng của tệp này phải chứa số ID của học sinh, dấu phẩy và sau đó là điểm của họ. Bạn nên đặt tên tệp này dựa trên tên tệp gốc được cung cấp

Học viên thiết lập phiên bản 3.9 cho Python 
“lastname_firstname_grade_the_exams.py.”
