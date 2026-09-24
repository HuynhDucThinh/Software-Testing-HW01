# Phân tích sơ đồ tư duy QA/QC và 3 lỗi sai của AI theo chuẩn ISTQB CTFL v4.0.1

## 1. Tổng quan sơ đồ do AI tạo

Sơ đồ tư duy do công cụ AI sinh ra có chủ đề trung tâm: **"QA/QC ROLES & ISTQB TESTING PROCESS"** với 4 nhánh chính:

1. **QA ROLES (Xanh dương):** Process Assurance, Quality Standards, Risk Assessment, Process Audit.
2. **QC ROLES (Xanh lá):** Execute Test Cases, Bug Reporting & Tracking, Functional & Performance Testing, Result Analysis.
3. **AI-AUGMENTED TESTING (Tím):** AI & LLM Testing, Automation, Prompt Auditing, Edge Case Discovery.
4. **ISTQB PROCESS (Cam - Góc dưới bên phải):** Planning, Analysis & Design, Execution, Test Completion.

![QA/QC Roles & ISTQB Testing Process](QA_QC_Role_Mindmap.png)

<p align="center"><strong>Hình 1: Sơ đồ tư duy QA/QC Roles & ISTQB Testing Process do AI tạo ra.</strong></p>

---

## 2. Bảng tổng hợp 3 lỗi sai của AI trong sơ đồ

|  STT   | Tên lỗi                                                           | Vị trí trên sơ đồ           | Loại lỗi                             | Chuẩn đối chiếu (ISTQB CTFL v4.0.1)                                                                                        |
| :----: | :---------------------------------------------------------------- | :-------------------------- | :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| **01** | **ISTQB Test Process bị thiếu và gộp sai các nhóm hoạt động**     | Nhánh `ISTQB PROCESS`       | **INCOMPLETE / INCORRECT STRUCTURE** | Mục 1.4.1: Quy trình gồm 7 nhóm hoạt động riêng biệt, không gộp và không bỏ bước.                                          |
| **02** | **Test Execution bị giản lược/đồng nhất sai thành "Bug Finding"** | Nhánh con `Execution`       | **MISLEADING / OVERSIMPLIFIED**      | Mục 1.4.2 (Execution): Chạy test, so sánh actual vs expected, ghi nhận log và phân tích anomalies.                         |
| **03** | **Test Completion bị thu hẹp chỉ còn là "Final Report"**          | Nhánh con `Test Completion` | **INCOMPLETE**                       | Mục 1.4.2 (Completion): Bao gồm 6 hoạt động tổng kết, bàn giao, đóng môi trường, lessons learned; báo cáo chỉ là 1 output. |

---

## 3. Chi tiết phân tích từng lỗi sai

### Lỗi 1: ISTQB Test Process bị thiếu và gộp sai các nhóm hoạt động

#### 1. Mô tả lỗi

Ở góc phải phía dưới, tại nhánh **ISTQB PROCESS**, AI biểu diễn quy trình kiểm thử chỉ gồm 4 bước tuần tự đơn giản:
$$\text{Planning} \longrightarrow \text{Analysis \& Design} \longrightarrow \text{Execution} \longrightarrow \text{Test Completion}$$

#### 2. Nguyên nhân sai sót của AI

- **Gộp sai bản chất công việc:** AI gộp chung hai hoạt động `Test Analysis` và `Test Design` thành một nhãn `Analysis & Design`.
- **Bỏ sót Test Implementation:** AI nhảy thẳng từ thiết kế sang thực thi (`Execution`), bỏ qua toàn bộ giai đoạn chuẩn bị dữ liệu, môi trường và kịch bản thực thi.
- **Bỏ sót Test Monitoring & Test Control:** AI coi việc kiểm thử như một đường thẳng từ đầu đến cuối mà quên mất hoạt động giám sát, đo lường độ bao phủ và điều chỉnh liên tục.

#### 3. Định nghĩa đúng theo chuẩn ISTQB CTFL v4.0.1

Theo **ISTQB CTFL v4.0.1 (Section 1.4: The Test Process)**, quy trình kiểm thử chuẩn gồm **7 nhóm hoạt động chính**:

1. **Test Planning:** Xác định mục tiêu kiểm thử, phạm vi, rủi ro, nguồn lực và lịch trình.
2. **Test Monitoring and Test Control:** Giám sát tiến độ thực tế so với kế hoạch (monitoring) và thực hiện các hành động khắc phục kịp thời (control). Hoạt động này diễn ra liên tục xuyên suốt quy trình.
3. **Test Analysis ("What to test?"):** Phân tích test basis (yêu cầu, kiến trúc) để xác định các điều kiện kiểm thử (_test conditions_).
4. **Test Design ("How to test?"):** Thiết kế test cases chi tiết, test data specification, thiết kế môi trường và cơ sở hạ tầng phục vụ kiểm thử.
5. **Test Implementation:** Chuẩn bị đầy đủ mọi thứ để test có thể chạy được: tạo test data, viết test procedures/scripts (manual & automated), tổ chức test suites, cấu hình test environment và thiết lập lịch chạy.
6. **Test Execution:** Chạy test suites/scripts, so sánh kết quả thực tế với mong đợi, log kết quả và ghi nhận lỗi.
7. **Test Completion:** Thu thập dữ liệu từ các hoạt động test đã xong, tổng kết artifacts, bàn giao testware, rút ra bài học kinh nghiệm (_lessons learned_).

> **Ví dụ minh họa:**
> Với chức năng _Đăng nhập (Login)_:
>
> - **Test Analysis:** Xác định cần kiểm tra: Username hợp lệ/không hợp lệ, Password đúng/sai, Khóa tài khoản khi nhập sai 5 lần (_What to test_).
> - **Test Design:** Tạo test case cụ thể: Nhập user `abc@gmail.com`, pass `123456`, expected: đăng nhập thành công (_How to test_).
> - **Test Implementation:** Phải tạo trước user test trong cơ sở dữ liệu, dựng môi trường staging, viết automated script trên Selenium/Playwright trước khi bấm chạy. AI đã bỏ qua bước này.

#### 4. Gợi ý sửa lỗi trên sơ đồ

Thay thế cấu trúc 4 bước của nhánh `ISTQB PROCESS` thành 7 nhóm hoạt động chuẩn:

```text
ISTQB PROCESS
├── Test Planning
├── Test Monitoring & Control
├── Test Analysis (What to test)
├── Test Design (How to test)
├── Test Implementation (Prepare testware)
├── Test Execution (Run & Log)
└── Test Completion (Consolidate & Handover)
```

---

### Lỗi 2: Test Execution bị giản lược/đồng nhất sai thành "Bug Finding"

#### 1. Mô tả lỗi

Trong nhánh con `Execution`, AI chỉ vẽ hai nhánh lá:

```text
Execution
├── Test run status
└── Bug Finding
```

Cách đặt nhãn này khiến người đọc hiểu lầm rằng bản chất và mục đích duy nhất của việc thực thi test là "đi tìm bug" (_Bug Finding_).

#### 2. Nguyên nhân sai sót của AI

- AI nhầm lẫn giữa **mục tiêu thực thi kiểm thử** (đo lường chất lượng, xác minh hệ thống hoạt động đúng theo đặc tả) với **kết quả phụ phát sinh** khi test thất bại (phát hiện bug).
- Bỏ qua các bước phân tích nguyên nhân bất thường (_anomalies_) trước khi kết luận đó là defect.

#### 3. Định nghĩa đúng theo chuẩn ISTQB CTFL v4.0.1

Theo **ISTQB CTFL v4.0.1 (Section 1.4.2 - Test Execution)**:

- Test Execution là hoạt động **chạy các test suite/test scripts đã chuẩn bị, quan sát và so sánh kết quả thực tế (actual results) với kết quả mong đợi (expected results), và ghi nhận kết quả (Pass/Fail/Blocked)**.
- Khi actual result khác expected result, đó gọi là một bất thường. Tester phải điều tra nguyên nhân (do môi trường, do mạng, do dữ liệu sai, do hiểu sai đặc tả hay thực sự do code) trước khi lập báo cáo lỗi (_Defect Report_).
- Một kịch bản kiểm thử chạy thành công (Actual = Expected $\rightarrow$ Pass) không tìm ra bất kỳ bug nào nhưng vẫn là một hoạt động Test Execution hoàn hảo và có giá trị lớn (xác nhận độ tin cậy của phần mềm).

> **Ví dụ minh họa:**
> Khi test nút _Đăng nhập_, trang web quay vòng và báo Timeout:
>
> - Chưa thể lập tức kết luận là "Bug của phần mềm".
> - Tester phải kiểm tra: Server API có đang restart không? Mạng test có bị ngắt không? Database test có bị quá tải không?
> - Quy trình đúng: Run test $\rightarrow$ So sánh Actual vs Expected $\rightarrow$ Phát hiện Anomaly $\rightarrow$ Phân tích nguyên nhân $\rightarrow$ Nếu do code mới log Defect.

#### 4. Gợi ý sửa lỗi trên sơ đồ

Thay nhánh con của `Execution` bằng các hoạt động thành phần chính xác:

```text
Test Execution
├── Run Test Cases / Suites
├── Compare Actual vs Expected
├── Record Test Results (Pass/Fail/Block)
├── Analyze Anomalies
└── Report Defects (when confirmed)
```

---

### Lỗi 3: Test Completion bị thu hẹp chỉ còn là "Final Report"

#### 1. Mô tả lỗi

Tại nhánh `Test Completion`, AI chỉ đặt duy nhất một nhánh con:

```text
Test Completion
└── Final report
```

#### 2. Nguyên nhân sai sót của AI

- AI nhầm lẫn giữa **kết quả bàn giao dạng tài liệu** (_documentary output_) với **toàn bộ nhóm hoạt động đóng dự án kiểm thử** (_process closure activities_).
- Thiếu góc nhìn vòng đời dự án (SDLC).

#### 3. Định nghĩa đúng theo chuẩn ISTQB CTFL v4.0.1

Theo **ISTQB CTFL v4.0.1 (Section 1.4.2 - Test Completion)**, hoạt động kết thúc kiểm thử diễn ra tại các cột mốc dự án (release, kết thúc sprint, ngừng dự án) và bao gồm 6 nhiệm vụ cốt lõi:

1. **Kiểm tra và xử lý các hạng mục chưa giải quyết:** Rà soát lại tất cả các defect còn mở (open bugs), tạo change request hoặc chuyển vào product backlog cho sprint/release sau.
2. **Tạo Test Completion Report:** Lập báo cáo tóm tắt kiểm thử gửi cho các bên liên quan (Product Owner, Project Manager).
3. **Hoàn thiện và lưu trữ testware:** Lưu trữ test cases, automated test scripts, test data, test environment specifications vào kho lưu trữ chung để tái sử dụng cho các đợt Regression Test sau.
4. **Bàn giao testware:** Chuyển giao testware cho đội bảo trì (Maintenance team) hoặc khách hàng.
5. **Đóng và dọn dẹp môi trường kiểm thử:** Trả môi trường test, tắt hạ tầng cloud (AWS/Azure) để tiết kiệm chi phí, đưa test environment về trạng thái sạch đã thỏa thuận.
6. **Đúc kết bài học kinh nghiệm:** Họp Retrospective để phân tích những điểm làm tốt và chưa tốt, xác định cải tiến cho các chu kỳ kiểm thử kế tiếp.

> **Ví dụ minh họa:**
> Khi kết thúc đợt test một website E-Commerce trước đợt Big Sale:
>
> - Không thể chỉ viết báo cáo rồi bỏ đó.
> - Phải: (1) Đánh giá 3 lỗi mức Low còn tồn đọng xem có release được không; (2) Lưu lại 200 automation scripts vào Git repo để sprint sau chạy tiếp; (3) Reset cơ sở dữ liệu test về trạng thái trắng; (4) Ghi nhận rằng đợt này API test bị chậm do thiếu mock server để lần sau khắc phục.

#### 4. Gợi ý sửa lỗi trên sơ đồ

Mở rộng nhánh `Test Completion` thành các nhánh phản ánh đầy đủ hoạt động:

```text
Test Completion
├── Handle Unresolved Defects / Items
├── Test Completion Report (Final Report)
├── Archive & Handover Testware
├── Restore / Clean Test Environment
└── Lessons Learned & Process Improvement
```
