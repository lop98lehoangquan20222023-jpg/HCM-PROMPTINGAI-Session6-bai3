# Báo cáo thiết kế giải pháp:
1. Đưa bài toán và lời giải vào.
2. Gia sư AI phân tích kiến thức.
3. Đặt câu hỏi Feynman.
4. Chấm điểm theo các tiêu chí Rubric.
5. Đưa ra điểm sau khi chấm và nhận xét.
# Thiết kế chuỗi Prompt:
## Prompt 1:
```
Bạn là một gia sư AI.Hãy phân tích lời giải bài toán sau: và đưa ra 5 kiến thức quan trọng cần kiểm tra trong bài toán.Trình bày ngắn gọn dễ hiểu.
```
## Prompt 2:
```
Bạn là một gia sư AI.Hãy đặt ra các câu hỏi dựa trên kiến thức của bài toán đó để tôi có thể giải thích.Không đưa ra đáp án trước khi tôi trả lời.Chỉ đặt một câu hỏi một lân.
```
## Prompt 3:
```
Bạn là một giáo viên chấm bài kiểm tra,hãy chấm điểm bài trả lời của tôi dựa trên các tiêu chí sau:
1. Hiểu bản chất: 0-2 điểm.
2. Giải thích đơn giản: 0-2 điểm.
3. Độ chính xác: 0-2 điểm.
4. Ví dụ minh họa: 0-2 điểm.
5. Khả năng ứng dụng: 0-2 điểm.

Tổng điểm tối đa là 10.

Giải thích rõ lý do cho từng điểm.
Không tự suy đoán kiến thức tôi chưa trình bày
```
## Prompt 4:
```
Dựa trên kết quả chấm điểm:
1. Nêu điểm mạnh.
2. Chỉ ra lỗi sai.
3. Giải thích kiến thức đúng.
4. Đề xuất cách cải thiện.
5. Đặt một câu hỏi kiểm tra lại.
Dùng từ ngữ gần gũi,dễ hiểu.
```
## Prompt 5:
```
Đóng vai một người viết báo cáo:
Tổng hợp kết quả thành báo cáo gồm:

- Chủ đề kiểm tra.
- Câu trả lời của sinh viên.
- Bảng điểm Rubric.
- Tổng điểm trên thang 10.
- Xếp loại.
- Nhận xét.
- Hướng cải thiện.

Trình bày bằng Markdown rõ ràng.
```
# Kết quả:
## Prompt 1:
```
# PHÂN TÍCH BÀI TOÁN THEO PHƯƠNG PHÁP GIA SƯ AI

## 1. Phân tích lời giải

Bài toán thuộc chương trình Toán lớp 12, chủ đề **ứng dụng đạo hàm để khảo sát hàm số và giải bài toán chứa tham số**.

| Câu | Kiến thức sử dụng | Kết quả |
|---|---|---|
| Câu 1 | Quy tắc tính đạo hàm | \(f'(x)=3(x-3)(x+1)\) |
| Câu 2 | Giải phương trình đạo hàm bằng 0 và xét dấu | Cực đại tại \(x=-1\), cực tiểu tại \(x=3\) |
| Câu 3 | Tìm GTLN, GTNN trên đoạn | GTLN = 10, GTNN = -22 |
| Câu 4 | Đồ thị hàm số và phương trình chứa tham số | \(m\in(-22;10)\) |

**Nhận xét:** Lời giải đúng về mặt toán học. Tuy nhiên, phần bảng xét dấu và bảng tổng kết bị lỗi định dạng. Nên sử dụng bảng Markdown thông thường để trình bày rõ ràng hơn.

---

## 2. Năm kiến thức quan trọng cần kiểm tra

### Kiến thức 1: Quy tắc tính đạo hàm

- Biết tính đạo hàm của hàm đa thức.
- Biết rút gọn và phân tích đạo hàm thành nhân tử.

Ví dụ:

\[
f(x)=x^3-3x^2-9x+5
\]

\[
f'(x)=3(x-3)(x+1)
\]

### Kiến thức 2: Tìm cực trị của hàm số

- Giải phương trình \(f'(x)=0\).
- Xác định điểm cực đại và cực tiểu.
- Biết sử dụng bảng xét dấu đạo hàm.

Kết quả:
- Cực đại tại \(x=-1\).
- Cực tiểu tại \(x=3\).

### Kiến thức 3: Xét dấu đạo hàm và chiều biến thiên

- Khi \(f'(x)>0\): Hàm số đồng biến.
- Khi \(f'(x)<0\): Hàm số nghịch biến.

Đây là cơ sở để lập bảng biến thiên của hàm số.

### Kiến thức 4: Tìm giá trị lớn nhất và nhỏ nhất trên đoạn

Các bước thực hiện:

1. Tính giá trị hàm số tại hai đầu đoạn.
2. Tìm các điểm cực trị nằm bên trong đoạn.
3. Tính giá trị hàm số tại các điểm đó.
4. So sánh tất cả kết quả.

Kết quả:

\[
\max_{[-2;4]}f(x)=10
\]

\[
\min_{[-2;4]}f(x)=-22
\]

### Kiến thức 5: Giải phương trình chứa tham số bằng đồ thị

- Hiểu phương trình \(f(x)=m\) tương ứng với giao điểm giữa đồ thị \(y=f(x)\) và đường thẳng \(y=m\).
- Dựa vào giá trị cực đại và cực tiểu để xác định số nghiệm.
- Biết xác định điều kiện để phương trình có đúng 3 nghiệm thực phân biệt.

Kết quả:

\[
\boxed{-22<m<10}
\]

---

## 3. Tổng kết kiến thức

| STT | Kiến thức | Mức độ quan trọng |
|---|---|---|
| 1 | Quy tắc đạo hàm | Cao |
| 2 | Tìm cực trị | Cao |
| 3 | Xét dấu và chiều biến thiên | Cao |
| 4 | Tìm GTLN, GTNN | Cao |
| 5 | Phương trình chứa tham số | Rất cao |

---

## 4. Kiểm tra kiến thức theo phương pháp Feynman

Để kiểm tra mức độ hiểu bài, sinh viên cần trả lời câu hỏi sau:

**Câu hỏi:**

Tại sao khi \(f'(x)>0\) thì hàm số đồng biến, còn khi \(f'(x)<0\) thì hàm số nghịch biến?

**Yêu cầu:**

- Giải thích bằng ngôn ngữ đơn giản.
- Không học thuộc định nghĩa máy móc.
- Có thể sử dụng ví dụ thực tế để minh họa.
- Giải thích như đang giảng cho một người chưa học đạo hàm.

Từ câu trả lời của sinh viên, gia sư AI sẽ đánh giá mức độ hiểu bài theo Rubric 10 điểm.

---

## 5. Kết luận

Bài toán giúp sinh viên củng cố 5 kiến thức quan trọng:

1. Tính đạo hàm.
2. Tìm cực trị.
3. Xét chiều biến thiên.
4. Tìm giá trị lớn nhất và nhỏ nhất.
5. Giải phương trình chứa tham số bằng đồ thị.

Việc kết hợp phương pháp Feynman và Rubric giúp sinh viên không chỉ biết cách giải bài toán mà còn hiểu được bản chất của từng bước thực hiện.
```
## Prompt 2:
```
# GIA SƯ AI – KIỂM TRA KIẾN THỨC THEO PHƯƠNG PHÁP FEYNMAN

## 1. Mục tiêu

Sử dụng phương pháp Feynman để kiểm tra mức độ hiểu bài của sinh viên thông qua việc giải thích kiến thức bằng ngôn ngữ đơn giản.

Gia sư AI sẽ:
- Đặt câu hỏi dựa trên bài toán đã học.
- Chỉ đặt một câu hỏi mỗi lần.
- Không đưa ra đáp án trước khi sinh viên trả lời.
- Đánh giá câu trả lời và chỉ ra lỗi sai.
- Đặt câu hỏi tiếp theo sau mỗi lần trả lời.
- Chấm điểm theo Rubric thang điểm 10 sau khi hoàn thành.

## 2. Quy trình kiểm tra

1. Gia sư AI đưa ra câu hỏi.
2. Sinh viên tự giải thích kiến thức.
3. AI phân tích câu trả lời.
4. AI nhận xét điểm đúng và điểm cần cải thiện.
5. AI tiếp tục đặt câu hỏi tiếp theo.
6. Hoàn thành bài kiểm tra và chấm điểm.

## 3. Bộ câu hỏi kiểm tra kiến thức

### Câu 1: Quy tắc tính đạo hàm

Cho hàm số:

\[
f(x)=x^3-3x^2-9x+5
\]

**Yêu cầu:**

Hãy giải thích cách tính đạo hàm của hàm số trên và tại sao kết quả là:

\[
f'(x)=3x^2-6x-9
\]

Giải thích bằng ngôn ngữ đơn giản như đang giảng cho một người chưa biết về đạo hàm.

## 4. Quy định khi kiểm tra

- Không cung cấp đáp án trước khi sinh viên trả lời.
- Không đặt nhiều câu hỏi cùng lúc.
- Khuyến khích sinh viên giải thích bằng cách hiểu của mình.
- Không đánh giá chỉ dựa trên độ dài câu trả lời.
- Nhận xét rõ ràng, dễ hiểu và mang tính xây dựng.

## 5. Đánh giá kết quả

Sau khi hoàn thành các câu hỏi, AI sử dụng Rubric 10 điểm để đánh giá:

| Tiêu chí | Điểm tối đa |
|---|---:|
| Hiểu bản chất kiến thức | 2 |
| Giải thích đơn giản | 2 |
| Độ chính xác | 2 |
| Ví dụ minh họa | 2 |
| Khả năng vận dụng | 2 |
| **Tổng điểm** | **10** |

## 6. Kết luận

Phương pháp Feynman giúp sinh viên chủ động suy nghĩ, tự giải thích kiến thức và phát hiện những phần chưa hiểu.

Thông qua việc kết hợp Rubric, gia sư AI có thể đánh giá mức độ hiểu bài và đề xuất phương pháp cải thiện phù hợp.
```
## Prompt 3:
```
# GIA SƯ AI – CHẤM ĐIỂM BÀI LÀM THEO RUBRIC

## 1. Vai trò

Bạn là một giáo viên chấm bài kiểm tra, có nhiệm vụ đánh giá kiến thức của sinh viên dựa trên câu trả lời thực tế.

## 2. Mục tiêu

- Đánh giá mức độ hiểu bài của sinh viên.
- Chấm điểm theo Rubric thang điểm 10.
- Giải thích rõ lý do cho từng điểm.
- Chỉ ra điểm mạnh và điểm cần cải thiện.
- Đưa ra hướng dẫn giúp sinh viên hiểu bài tốt hơn.

## 3. Các tiêu chí chấm điểm

| STT | Tiêu chí | Điểm tối đa |
|---|---|---:|
| 1 | Hiểu bản chất | 2 |
| 2 | Giải thích đơn giản | 2 |
| 3 | Độ chính xác | 2 |
| 4 | Ví dụ minh họa | 2 |
| 5 | Khả năng ứng dụng | 2 |
| | **Tổng điểm** | **10** |

## 4. Đề bài kiểm tra

Cho hàm số:

\[
f(x)=x^3-3x^2-9x+5
\]

Hãy giải thích cách tính đạo hàm của hàm số và tại sao kết quả là:

\[
f'(x)=3x^2-6x-9
\]

Sinh viên cần giải thích bằng ngôn ngữ đơn giản và thể hiện cách hiểu của mình.

## 5. Quy định chấm điểm

1. Chỉ đánh giá dựa trên nội dung sinh viên thực sự trình bày.
2. Không tự suy đoán kiến thức sinh viên chưa thể hiện.
3. Không chấm điểm chỉ dựa trên độ dài câu trả lời.
4. Giải thích rõ lý do cho từng mức điểm.
5. Nếu sinh viên không đề cập đến ví dụ, không tự cho điểm tối đa ở tiêu chí ví dụ minh họa.
6. Nếu thiếu dữ liệu, ghi rõ chưa đủ cơ sở đánh giá.

## 6. Cấu trúc kết quả chấm điểm

### 6.1. Bảng điểm

| Tiêu chí | Điểm đạt được | Điểm tối đa | Nhận xét |
|---|---:|---:|---|
| Hiểu bản chất | Chưa chấm | 2 | Chờ câu trả lời |
| Giải thích đơn giản | Chưa chấm | 2 | Chờ câu trả lời |
| Độ chính xác | Chưa chấm | 2 | Chờ câu trả lời |
| Ví dụ minh họa | Chưa chấm | 2 | Chờ câu trả lời |
| Khả năng ứng dụng | Chưa chấm | 2 | Chờ câu trả lời |
| **Tổng điểm** | **Chưa chấm** | **10** | |

### 6.2. Nhận xét của giáo viên

- **Điểm mạnh:** Những kiến thức sinh viên trình bày đúng.
- **Điểm yếu:** Những nội dung còn thiếu hoặc chưa chính xác.
- **Lý do trừ điểm:** Giải thích cụ thể từng tiêu chí.
- **Hướng cải thiện:** Đề xuất cách học và sửa lỗi.

### 6.3. Kết luận

Sau khi chấm điểm, giáo viên đưa ra nhận xét tổng quan về mức độ hiểu bài của sinh viên.

## 7. Nguyên tắc quan trọng

**Không chấm điểm khi chưa có câu trả lời của sinh viên.**

Nếu sinh viên chưa gửi bài làm, yêu cầu sinh viên cung cấp câu trả lời trước khi tiến hành đánh giá.
```
