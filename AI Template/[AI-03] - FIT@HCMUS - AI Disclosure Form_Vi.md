# PHIẾU KHAI BÁO SỬ DỤNG AI

**Khoa Công nghệ Thông tin (FIT) - Trường Đại học Khoa học Tự nhiên, ĐHQG-HCM (HCMUS)**  
**CS423 / CSC13003 - Kiểm thử phần mềm (Tích hợp AI - 2026)**  
**CHÍNH SÁCH AI - BIỂU MẪU - 2026 v1.0**

Phiếu này được đính kèm với bài tập có sử dụng AI trong phạm vi được môn học cho phép.

Biểu mẫu được điều chỉnh từ tài liệu của Med Kharbach, PhD (2026), _AI Use Policy Templates for Higher Education_, giấy phép CC BY-NC-SA 4.0. Bản điều chỉnh này được chuẩn bị cho môn CS423 / CSC13003 - Kiểm thử phần mềm tại FIT@HCMUS.

## 1. Thông tin môn học và sinh viên

| Trường thông tin    | Nội dung                                          |
| ------------------- | ------------------------------------------------- |
| Môn học             | CS423 / CSC13003 - Kiểm thử phần mềm              |
| Mã bài tập          | HW01-AI                                           |
| Tên bài tập         | QA/QC Jobs - 20 Defects - Test a Physical Product |
| Nhóm sử dụng AI     | Category 4 - AI-Assisted Production               |
| Ngày khai báo       | 26/09/2026                                        |
| Họ và tên sinh viên | Huỳnh Đức Thịnh                                   |
| Mã số sinh viên     | 23120199                                          |

## 2. Nội dung khai báo

### 2.1. Công cụ AI đã sử dụng

| Công cụ / Model                  | Phạm vi sử dụng                                                                                                                                                                                                                                 |
| -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Gemini**                       | Em sử dụng Gemini để hỗ trợ tạo bản nháp ảnh sơ đồ tư duy về vai trò QA/QC và quy trình kiểm thử cho Yêu cầu 1; sau đó em tự kiểm tra nội dung theo ISTQB.                                                                                      |
| **ChatGPT-5.6 Sol**              | Em sử dụng ChatGPT-5.6 Sol để hỗ trợ gợi ý cấu trúc, từ khóa, nguồn tham khảo và cách trình bày. Em trực tiếp đọc nguồn, đối chiếu các lỗi trong sơ đồ và sự cố D01-D20, rà soát test case cho quạt bàn Senko và quyết định nội dung cuối cùng. |
| **GPT2-Small trên Hugging Face** | Em sử dụng GPT2-Small để tạo các phản hồi có khả năng chứa hallucination hoặc bias; em trực tiếp nhận diện, phân tích và sửa thông tin sai trong D01-D20 của Yêu cầu 2.                                                                         |

### 2.2. Các giai đoạn của bài tập có sử dụng AI

- [x] Brainstorming - Em sử dụng AI để tham khảo ý tưởng và tự lựa chọn hướng triển khai phù hợp.
- [x] Outlining - Em sử dụng AI để tham khảo cách tổ chức dàn ý, sau đó tự quyết định cấu trúc trình bày.
- [x] Drafting - Em sử dụng AI để tạo bản nháp tham khảo cho một số nội dung và test case.
- [x] Feedback - Em sử dụng phản hồi của AI như gợi ý cải thiện và tự đánh giá trước khi áp dụng.
- [x] Revision - Em tự chỉnh sửa và chuẩn hóa nội dung sau khi tham khảo gợi ý của AI.
- [ ] Coding - Em không sử dụng AI để tạo mã nguồn chương trình cho bài tập này.
- [x] Data analysis - Em sử dụng AI hỗ trợ tổng hợp ban đầu; em trực tiếp kiểm tra và phân tích thông tin việc làm, sự cố và kết quả đối chiếu.
- [x] Visual design - Em sử dụng Gemini hỗ trợ tạo bản nháp ảnh mindmap QA/QC và tự kiểm tra nội dung.
- [x] Other - Em sử dụng AI tạo phản hồi sai làm dữ liệu phân tích và đề xuất bản nháp test case; em tự đánh giá và hoàn thiện kết quả.

### 2.3. Các prompt hoặc nhiệm vụ chính đã giao cho AI

Ba nhóm prompt dưới đây là những prompt có ảnh hưởng trực tiếp nhất đến sản phẩm của Yêu cầu 1, Yêu cầu 2 và Yêu cầu 3. Toàn bộ prompt và câu trả lời đầy đủ được lưu trong Phụ lục A - `prompt_log.md`.

#### Nhóm prompt 1 - Yêu cầu 1: Tạo mindmap QA/QC

**Công cụ:** Gemini  
**Mục đích:** Hỗ trợ em tạo bản nháp mindmap để em kiểm tra và phát hiện ba nội dung chưa chính xác theo ISTQB.

> Hãy tạo cho tôi một mindmap về vai trò QA/QC trong kiểm thử phần mềm, dựa trên các khái niệm ISTQB.
>
> Mindmap cần bao gồm:
>
> - Quality Assurance
> - Quality Control
> - Software Testing
> - Vai trò và trách nhiệm của QA/QC
> - Test levels
> - Test types
> - Test activities/process
>
> Hãy xuất kết quả ở dạng PNG.
>
> Không cần giải thích bên ngoài mindmap.

#### Nhóm prompt 2 - Yêu cầu 2: Phân tích D01

**Công cụ:** GPT2-Small trên Hugging Face  
**Mục đích:** Em sử dụng phản hồi có khả năng chứa hallucination làm đối tượng để tự nhận diện, phân loại, giải thích và sửa lại bằng nguồn đối chiếu.

> Explain the 2023 Mata v. Avianca ChatGPT incident. What false information did ChatGPT generate, how did the lawyers use it, what did the court decide, what penalty was imposed, and how could the incident have been prevented?

Prompt trên là trường hợp đại diện. Quy trình tương tự được áp dụng cho các sự cố còn lại trong D01-D20; prompt và output đầy đủ được lưu trong `prompt_log.md`.

#### Nhóm prompt 3 - Yêu cầu 3: Tạo và chỉnh sửa test case cho quạt bàn Senko

##### Prompt 3.1 - Tạo 15 test case ban đầu

**Công cụ:** ChatGPT-5.6 Sol  
**Mục đích:** Hỗ trợ em đề xuất bản nháp 15 test case để em đánh giá, chỉnh sửa và hoàn thiện thành bộ test case an toàn, có thể thực hiện tại nhà đối với quạt bàn Senko.

> Bạn là kỹ sư QA/QC đang thiết kế test case cho một sản phẩm vật lý thực tế.
>
> **THÔNG TIN SẢN PHẨM**
>
> - Sản phẩm: Quạt bàn gia dụng
> - Thương hiệu: Senko
> - Năm sản xuất hoặc năm mua: 2023
> - Nguồn điện: Điện xoay chiều 220V
> - Số mức gió: 3
> - Cơ chế điều khiển tốc độ: [nút nhấn]
> - Chức năng quay trái-phải: có
> - Cách bật chức năng quay: [nút nhấn phía sau]
> - Có thể điều chỉnh góc quạt lên-xuống: không
> - Chức năng hẹn giờ: không
> - Remote control: không
> - Đèn báo hoặc màn hình: không
> - Các chức năng khác: Không có
> - Dụng cụ kiểm thử có sẵn: đồng hồ bấm giờ, thước dây và giấy mỏng để quan sát luồng gió.
> - Môi trường kiểm thử: phòng ở sinh viên, mặt bàn bằng phẳng, sử dụng nguồn điện gia dụng bình thường.
>
> Hãy tạo chính xác 15 test case để kiểm thử chiếc quạt bàn cụ thể này.
>
> **PHẠM VI KIỂM THỬ**
>
> Bộ test case cần bao phủ hợp lý các nhóm sau:
>
> 1. Bật và tắt quạt.
> 2. Kiểm tra từng mức tốc độ gió.
> 3. Chuyển đổi giữa các mức tốc độ.
> 4. Chức năng quay trái-phải nếu quạt có hỗ trợ.
> 5. Điều chỉnh hướng gió lên-xuống nếu có hỗ trợ.
> 6. Độ ổn định của quạt trên mặt bàn.
> 7. Nút bấm hoặc núm điều khiển.
> 8. Tiếng ồn và rung động bất thường có thể quan sát được.
> 9. Dây điện, phích cắm và trạng thái hoạt động bình thường.
> 10. Khởi động lại sau khi tắt.
> 11. Phản ứng sau khi mất điện và được cấp điện trở lại.
> 12. Hoạt động liên tục trong thời gian hợp lý.
> 13. Thao tác không hợp lệ nhưng an toàn.
> 14. Tính nhất quán giữa trạng thái điều khiển và hoạt động thực tế.
> 15. Khả năng quan sát và sử dụng của người dùng.
>
> **YÊU CẦU AN TOÀN**
>
> - Chỉ tạo test case có thể thực hiện an toàn tại nhà.
> - Không yêu cầu tháo quạt hoặc mở lồng bảo vệ.
> - Không chạm tay hoặc đưa vật thể vào cánh quạt.
> - Không chặn cánh quạt hoặc motor khi quạt đang chạy.
> - Không thử nghiệm với nước, chất lỏng, lửa hoặc môi trường ẩm ướt.
> - Không thử quá áp, đấu nối điện hoặc làm hỏng dây điện.
> - Không thực hiện thử nghiệm có nguy cơ điện giật, cháy, hỏng thiết bị hoặc mất bảo hành.
> - Không để quạt hoạt động qua đêm hoặc không có người giám sát.
> - Không giả định quạt có chức năng không được liệt kê trong phần thông tin sản phẩm.
>
> **ĐỊNH DẠNG MỖI TEST CASE**
>
> Mỗi test case phải có đầy đủ:
>
> 1. Test Case ID
> 2. Test Case Title
> 3. Objective
> 4. Preconditions
> 5. Input
> 6. Steps
> 7. Expected Result
> 8. Actual Result
> 9. Verdict
>
> **QUY TẮC VIẾT**
>
> - Viết hoàn toàn bằng tiếng Việt.
> - Đánh số từ TC01 đến TC15.
> - Mỗi test case chỉ tập trung vào một mục tiêu kiểm thử chính.
> - Các bước phải cụ thể, có thứ tự và sinh viên có thể thực hiện được.
> - Expected Result phải rõ ràng, quan sát hoặc đo được bằng dụng cụ được liệt kê.
> - Không dùng các nhận xét mơ hồ như “quạt hoạt động tốt” mà không nêu dấu hiệu quan sát.
> - Không tự đặt tiêu chuẩn kỹ thuật về tốc độ gió, độ ồn hoặc nhiệt độ nếu không có tài liệu nhà sản xuất.
> - Không tuyên bố rằng test case đã được thực thi.
> - Điền “Chưa thực thi” vào Actual Result.
> - Điền “Not Executed” vào Verdict.
> - Trình bày từng test case thành một mục riêng, không gộp toàn bộ nội dung vào một bảng quá rộng.
> - Cuối câu trả lời, tạo một bảng tóm tắt gồm Test Case ID, tên test case và nhóm kiểm thử.

##### Prompt 3.2 - Chỉnh sửa sáu test case chưa phù hợp

**Công cụ:** ChatGPT-5.6 Sol  
**Mục đích:** Hỗ trợ em đề xuất phương án chỉnh sửa TC05, TC09, TC10, TC11, TC14 và TC15; em rà soát và quyết định nội dung cuối cùng dựa trên thiết bị thật, khả năng quan sát và yêu cầu an toàn.

> Hãy chỉnh sửa bộ 15 test case vừa tạo cho quạt bàn Senko theo các yêu cầu sau.
>
> Chỉ viết lại TC05, TC09, TC10, TC11, TC14 và TC15. Không thay đổi các test case còn lại.
>
> **Thông tin thiết bị:**
>
> - Quạt bàn Senko 220V.
> - Có ba mức gió bằng nút nhấn cơ học.
> - Có chức năng quay trái-phải.
> - Không có remote, màn hình hoặc hẹn giờ.
> - Đầu quạt không có khả năng điều chỉnh góc lên-xuống bằng tay.
>
> **Yêu cầu chỉnh sửa:**
>
> 1. Thay TC05 bằng test case kiểm tra trực quan lồng bảo vệ, chân đế và các bộ phận bên ngoài khi quạt đã rút điện. Không được đưa tay hoặc vật thể qua lồng quạt.
> 2. Sửa TC09:
>    - Chỉ kiểm tra trực quan dây điện và phích cắm khi đã rút điện.
>    - Nếu phát hiện dây hở, nứt, cháy, biến dạng hoặc chân cắm lỏng thì phải dừng test ngay.
>    - Chỉ được cắm điện khi không phát hiện dấu hiệu nguy hiểm.
> 3. Thay TC10 bằng test case kiểm tra hành vi sau khi mất điện trong lúc nút OFF đang được chọn:
>    - Chọn nút OFF trước khi ngắt nguồn.
>    - Ngắt rồi cấp lại điện bằng công tắc của ổ cắm.
>    - Quạt không được tự khởi động khi trạng thái OFF vẫn đang được chọn.
> 4. Sửa TC11 để mô phỏng mất điện bằng ổ cắm có công tắc, không rút hoặc cắm phích khi quạt đang chạy:
>    - Cho quạt chạy ở mức 1.
>    - Tắt công tắc ổ cắm.
>    - Chờ quạt dừng.
>    - Bật lại công tắc ổ cắm.
>    - Quan sát hành vi tương ứng với trạng thái nút cơ học đang được chọn.
> 5. Thay TC14 bằng test case kiểm tra bật và tắt chức năng quay trái-phải trong khi cánh quạt vẫn đang chạy ở mức 2:
>    - Khi tắt chức năng quay, đầu quạt dừng thay đổi hướng nhưng cánh quạt vẫn tiếp tục quay.
>    - Khi bật lại, đầu quạt tiếp tục quay trái-phải mà không bị kẹt.
> 6. Thay TC15 bằng test case kiểm tra độ ổn định của ba chu kỳ quay trái-phải liên tiếp:
>    - Theo dõi đủ ba chu kỳ.
>    - Quan sát hai đầu hành trình.
>    - Không yêu cầu đo góc quay bằng thiết bị chuyên dụng.
>    - Không được dùng tay cản hoặc ép đầu quạt.
>
> Mỗi test case phải có:
>
> - Test Case ID
> - Test Case Title
> - Objective
> - Preconditions
> - Input
> - Steps
> - Expected Result
> - Actual Result: Chưa thực thi
> - Verdict: Not Executed
>
> Expected Result phải quan sát được, không được bịa thông số kỹ thuật của nhà sản xuất. Chỉ xuất sáu test case đã sửa.

### 2.4. Những phần cụ thể có sự đóng góp của AI

#### Yêu cầu 1 - Sơ đồ tư duy QA/QC và phân tích ba lỗi sai

- Em sử dụng Gemini để hỗ trợ tạo bản nháp mindmap từ yêu cầu do em cung cấp.
- Em đối chiếu mindmap với ISTQB CTFL v4.0.1, xác định ba điểm sai hoặc thiếu, giải thích nguyên nhân và trình bày nội dung sửa lại.
- AI không quyết định kết luận cuối cùng về tính đúng/sai của sơ đồ.

#### Yêu cầu 2 - Phân tích 20 sự cố phần mềm và AI/LLM

- Em sử dụng GPT2-Small để nhận các câu trả lời có khả năng chứa hallucination hoặc bias cho D01-D20 và dùng chúng làm đối tượng phân tích.
- Em lựa chọn sự cố, kiểm tra nguồn, quyết định nội dung cuối cùng và chịu trách nhiệm về tính chính xác của phần trình bày.

#### Yêu cầu 3 - Kiểm thử sản phẩm vật lý

- Em sử dụng ChatGPT-5.6 Sol để tham khảo bản nháp 15 test case ban đầu cho quạt bàn Senko; em đánh giá và hoàn thiện nội dung.
- Sau khi phát hiện một số trường hợp chưa phù hợp, em đưa ra yêu cầu chỉnh sửa TC05, TC09, TC10, TC11, TC14 và TC15. Em sử dụng đề xuất của ChatGPT-5.6 Sol làm tài liệu tham khảo trước khi tự quyết định phiên bản cuối cùng theo ràng buộc an toàn và đặc điểm thực tế của quạt.
- Việc kiểm tra quạt thật, bổ sung bốn edge case bị AI bỏ sót, lựa chọn test case, ghi nhận Actual Result, xác định Pass/Fail, lập defect và quay video minh chứng do em trực tiếp thực hiện; AI không thay thế các hoạt động này.

### 2.5. Cách rà soát, chỉnh sửa và xác minh đầu ra AI

#### Đối với Yêu cầu 1

Em đối chiếu nội dung mindmap với ISTQB CTFL v4.0.1, đặc biệt là các nhóm hoạt động của test process, ý nghĩa của Test Execution và phạm vi của Test Completion. Em chỉ rõ và sửa lại những nội dung bị đơn giản hóa, gộp sai hoặc thiếu dựa trên tài liệu chuẩn thay vì chấp nhận trực tiếp hình ảnh do AI hỗ trợ tạo ra.

#### Đối với Yêu cầu 2

Em kiểm tra từng sự cố bằng nguồn chính thức hoặc nguồn kỹ thuật đáng tin cậy; xác minh tên sự cố, thời điểm, nguyên nhân, hậu quả, mức độ nghiêm trọng và giải pháp. Các đường dẫn được mở và kiểm tra trước khi đưa vào báo cáo. Câu trả lời của GPT2-Small chỉ được dùng làm đối tượng phân tích lỗi.

#### Đối với Yêu cầu 3

Em đối chiếu test case với quạt Senko B1216 thực tế, ảnh sản phẩm, nhãn năng lượng và các giới hạn an toàn của đề bài. Em thay thế các bước không khả thi hoặc có nguy cơ mất an toàn. Em chỉ sử dụng các dấu hiệu có thể quan sát hoặc đo bằng đồng hồ bấm giờ, thước dây và giấy mỏng trong Expected Result; em không tự đặt thông số kỹ thuật mà nhà sản xuất không công bố. Em chỉ ghi kết quả Pass/Fail và defect sau khi trực tiếp thực hiện kiểm thử thực tế.

### 2.6. Trích dẫn công cụ AI

[1] Google, “Gemini,” generative artificial intelligence system, 2026. [Online]. Available: https://gemini.google.com/. [Accessed: Sep. 26, 2026].

[2] OpenAI, “ChatGPT-5.6 Sol,” large language model, 2026. [Online]. Available: https://chatgpt.com/. [Accessed: Sep. 26, 2026].

[3] yasserBH, “GPT2-Small,” Hugging Face Space, 2026. [Online]. Available: https://huggingface.co/spaces/yasserBH/GPT2-Small. [Accessed: Sep. 26, 2026].

## 3. Cam kết trung thực

Bằng việc ký tên dưới đây, em xác nhận rằng nội dung khai báo phía trên là chính xác và đầy đủ. Em hiểu rằng việc không khai báo hoặc khai báo sai về việc sử dụng AI được xem là vi phạm quy định về trung thực học thuật và có thể dẫn đến điểm 0 cho bài tập cùng các biện pháp xử lý kỷ luật.

## 4. Chữ ký xác nhận

| Trường thông tin    | Nội dung                     |
| ------------------- | ---------------------------- |
| Họ và tên sinh viên | Huỳnh Đức Thịnh              |
| Mã số sinh viên     | 23120199                     |
| Lớp / Khóa          | CQ2023/31                    |
| Môn học             | CSC13003 - Kiểm thử phần mềm |
| Giảng viên          | Hồ Tuấn Thanh                |
| Ngày                | 26/09/2026                   |
| Chữ ký              | Huỳnh Đức Thịnh              |

## Tài liệu tham khảo

1. Kharbach, M. (2026). _AI Use Policy Templates for Higher Education_. CC BY-NC-SA 4.0.
2. ISTQB Foundation Level Syllabus, phiên bản mới nhất.
3. Hardman, P. (2025). _A Post-AI Learning Taxonomy_.
4. Fuster Rabella, M. (2025). _OECD Education Working Paper No. 338_.
5. Perkins, M., Roe, J., & Furze, L. (2025). _AI Assessment Scale_.
6. Anthropic. (2025). _Building Reliable AI Test Agents_.
7. Tài liệu DeepEval và Promptfoo về các framework kiểm thử hệ thống LLM.
