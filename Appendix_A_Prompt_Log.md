# APPENDIX A - PROMPT LOG

## 1. Thông tin chung

| Trường         | Nội dung        |
| -------------- | --------------- |
| **Họ và tên**  | Huỳnh Đức Thịnh |
| **MSSV**       | 23120199        |
| **Lớp**        | CQ2023/31       |
| **Bài tập**    | HW01-AI         |
| **Giảng viên** | Hồ Tuấn Thanh   |

## 2. Phạm vi và quy ước ghi nhận

- Prompt Log này ghi nhận 28 prompt trực tiếp phục vụ Requirement 1, Requirement 2 và Requirement 3.
- Các prompt được giữ nguyên ngôn ngữ và nội dung đã cung cấp; lỗi chính tả hoặc cách diễn đạt trong prompt không được tự ý sửa lại.
- Requirement 1 được thực hiện trong khoảng ngày **22-23/09/2026**.
- Requirement 2 được thực hiện ngày **24/09/2026**.
- Requirement 3 được thực hiện trong khoảng ngày **25-26/09/2026**.

## 3. Danh sách 28 prompt

### Prompt 01 - Tìm 5 QA/QC jobs

- **Requirement:** Requirement 1 - QA/QC Job Market 2026+
- **Thời gian:** 09:20 22/09/2026
- **Công cụ/model:** ChatGPT - GPT-5.6 Sol
- **Mục đích:** Tìm năm tin tuyển dụng QA/QC, trong đó có ít nhất hai vị trí liên quan đến AI, và trình bày theo form thống nhất.
- **Artifact liên quan:** Năm job đầu tiên trong phần Requirement 1 của báo cáo chính.

#### Prompt nguyên văn

```text
Tiến hành tìm cho tôi 5 jobs trong đó có ít nhất 2 jobs liên quan AI như yêu cầu đề bài, sau đó, trình bày nội dung theo form mà bạn đã cung cấp cho tôi với mỗi job
```

### Prompt 02 - Tìm thêm 5 QA/QC jobs có thông tin salary

- **Requirement:** Requirement 1 - QA/QC Job Market 2026+
- **Thời gian:** 09:30 22/09/2026
- **Công cụ/model:** ChatGPT - GPT-5.6 Sol
- **Mục đích:** Tìm thêm năm tin tuyển dụng QA/QC và ưu tiên các tin có công bố mức lương.
- **Artifact liên quan:** Năm job còn lại trong phần Requirement 1 của báo cáo chính.

#### Prompt nguyên văn

```text
Tiến hành tìm kiếm 5 jobs tương tự như vậy cho tôi. Nên kiếm jobs nào có lương để điền
```

### Prompt 03 - Tạo mindmap QA/QC ban đầu

- **Requirement:** Requirement 1 - ISTQB Mindmap
- **Thời gian:** 21:50 22/09/2026
- **Công cụ/model:** Gemini
- **Mục đích:** Tạo mindmap ban đầu về vai trò QA/QC và quy trình kiểm thử để em kiểm tra, nhận diện và giải thích ba lỗi.
- **Artifact liên quan:** Mindmap QA/QC ban đầu.

#### Prompt nguyên văn

```text
Hãy tạo cho tôi một mindmap về vai trò QA/QC trong kiểm thử phần mềm, dựa trên các khái niệm ISTQB.

Mindmap cần bao gồm:

Quality Assurance

Quality Control

Software Testing

Vai trò và trách nhiệm của QA/QC

Test levels

Test types

Test activities/process

Hãy xuất kết quả ở dạng PNG.

Không cần giải thích bên ngoài mindmap.
```

### Prompt 04 - Chỉnh sửa mindmap theo ISTQB CTFL v4.0.1

- **Requirement:** Requirement 1 - ISTQB Mindmap
- **Thời gian:** 09:35 23/09/2026
- **Công cụ/model:** Gemini
- **Mục đích:** Yêu cầu AI sửa các nội dung chưa chính xác trong mindmap nhưng giữ phong cách thiết kế ban đầu.
- **Artifact liên quan:** Mindmap QA/QC sau hiệu chỉnh.

#### Prompt nguyên văn

```text
Hãy chỉnh sửa trực tiếp mindmap hiện tại “QA/QC Roles & ISTQB Testing Process”.
Yêu cầu quan trọng: Giữ nguyên phong cách thiết kế hiện tại: nền trắng, mindmap nhiều màu, icon minh họa, bố cục 4 nhánh lớn xung quanh trung tâm. Không tạo một thiết kế hoàn toàn mới nếu không cần thiết. Chỉ thay đổi nội dung, vị trí các nhánh và icon cần thiết để đảm bảo kiến thức chính xác, dễ đọc và phù hợp với ISTQB CTFL v4.0.1.
1. Giữ tiêu đề trung tâm
Giữ:
QA/QC ROLES & ISTQB TESTING PROCESS
2. Sửa nhánh màu xanh dương bên trái
Đổi tiêu đề:
QA ROLES
thành:
QA RESPONSIBILITIES
Vì đây là các trách nhiệm/chức năng QA chứ không phải formal testing roles được ISTQB định nghĩa.
Giữ hoặc chỉnh thành đúng 4 nhánh:

Process Assurance
Quality Standards
Risk Assessment
Process Audit
Có thể bổ sung ý nhỏ nếu bố cục cho phép:

Process Improvement
Defect Prevention
Không biến QA thành “bug finding” hoặc “test execution”.
3. Sửa nhánh màu xanh lá bên phải
Đổi:
QC ROLES
thành:
QC / TESTING RESPONSIBILITIES
Giữ các ý chính nhưng chỉnh wording cho rõ:

Execute Test Cases
Analyze Test Results
Functional & Non-functional Testing
Defect Reporting & Tracking
Không trình bày QA và QC như hai formal testing roles của ISTQB.
4. Sửa toàn bộ nhánh ISTQB PROCESS màu cam
Đây là phần quan trọng nhất.

Phải thể hiện 7 test activities riêng biệt, không gộp và không bỏ sót:
ISTQB PROCESS

Test Planning
Test Objectives

Test Approach
Test Monitoring & Test Control
Track Progress

Compare Actual Progress with Plan

Take Corrective Actions
Test Analysis
What to Test?

Identify Testable Features

Define / Prioritize Test Conditions
Test Design
How to Test?

Design Test Cases

Identify Test Data Requirements
Test Implementation
Prepare Test Procedures / Test Scripts

Organize Test Suites

Prepare Test Data

Prepare Test Environment
Test Execution
Run Test Cases

Compare Actual vs Expected Results

Record Test Results

Analyze Anomalies

Report Defects if Appropriate
Test Completion
Handle Unresolved Items

Archive / Handover Testware

Lessons Learned

Improvement Actions

Test Completion Report
5. Phải sửa các lỗi cụ thể đang có trong ảnh hiện tại
Không được để:
Test Monitoring & Control → Test Design
Sai.

Phải là:
Test Monitoring & Control → Track Progress / Corrective Actions
Không được để:
Test Analysis → Track Progress
Sai.

Phải là:
Test Analysis → What to Test? / Test Conditions
Không được để:
Test Implementation → How to Test / Test Cases
Sai.

Phải là:
Test Design → How to Test? / Test Cases
Còn:
Test Implementation
phải tập trung vào:

test procedures,

test scripts,

test suites,

test data,

test environment.
6. Sửa Test Execution cho chính xác
Không dùng:
Bug Finding
như thể đó là mục đích hoặc activity chính của Test Execution.
Thay bằng:
Test Execution

Run Test Cases

Compare Actual vs Expected

Record Test Results

Analyze Anomalies

Report Defects if Appropriate
Phải thể hiện rõ:
test failure/anomaly không tự động đồng nghĩa với software defect.
7. Sửa Test Completion
Không thể hiện:
Test Completion = Final Report
hoặc chỉ có một Final Report.
Phải thể hiện rằng Test Completion còn gồm:

Handle Unresolved Items

Archive / Handover Testware

Lessons Learned

Improvement Actions

Test Completion Report
Test Completion Report chỉ là một phần/output của Test Completion.
8. Sửa nhánh AI-AUGMENTED TESTING màu tím
Giữ tiêu đề:
AI-AUGMENTED TESTING
Nhưng chỉnh các nhánh thành:

AI & LLM Testing
LLM Output Evaluation

Hallucination / Accuracy Testing
AI-assisted Test Automation
Prompt Testing / Prompt Auditing
Edge Case Discovery
Không dùng “Model Parameters” như một testing activity chính. Nếu cần thay thế, dùng:
Model / LLM Evaluation
hoặc:
AI Output Evaluation
9. Yêu cầu về bố cục

Giữ thiết kế mindmap 4 nhánh lớn.

QA: xanh dương.

QC/Testing: xanh lá.

AI-Augmented Testing: tím.

ISTQB Process: cam.

Có icon minh họa tương ứng.

Text phải lớn, dễ đọc, không bị đè nhau.

Các nhánh con phải nối đúng với parent node.

Không đặt label của activity này dưới activity khác.

Không lặp nội dung.

Không sai chính tả tiếng Anh.

Không tự thêm kiến thức không liên quan.
10. Mục tiêu của phiên bản cuối
Mindmap cuối cùng phải cho người đọc nhìn thấy rõ:
QA responsibilities

→ process-oriented / defect prevention
QC / Testing responsibilities

→ product-oriented / testing / defect detection
AI-Augmented Testing

→ AI hỗ trợ và AI system testing
ISTQB Test Process

→ Planning

→ Monitoring & Control

→ Analysis

→ Design

→ Implementation

→ Execution

→ Completion
Hãy kiểm tra toàn bộ nội dung trước khi xuất ảnh cuối và đảm bảo không còn các lỗi phân loại giữa Monitoring, Analysis, Design, Implementation, Execution và Completion.
```

### Prompt 05 - D01 - Mata v. Avianca

- **Requirement:** Requirement 2
- **Thời gian:** 14:30 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D01.
- **Artifact liên quan:** D01 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the 2023 Mata v. Avianca ChatGPT incident. What false information did ChatGPT generate, how did the lawyers use it, what did the court decide, what penalty was imposed, and how could the incident have been prevented?
```

### Prompt 06 - D02 - Moffatt v. Air Canada

- **Requirement:** Requirement 2
- **Thời gian:** 14:42 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D02.
- **Artifact liên quan:** D02 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the Moffatt v. Air Canada chatbot incident decided in 2024. What incorrect bereavement-fare information did the chatbot provide, why was Air Canada responsible, what compensation was ordered, and how could the chatbot have been improved?
```

### Prompt 07 - D03 - Google Gemini image generation

- **Requirement:** Requirement 2
- **Thời gian:** 14:57 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination hoặc bias cho D03.
- **Artifact liên quan:** D03 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain why Google paused Gemini's generation of images of people in February 2024. Describe the causes acknowledged by Google, the inaccurate behavior, the consequences, and the improvements needed before restoring the feature.
```

### Prompt 08 - D04 - Chevrolet chatbot prompt injection

- **Requirement:** Requirement 2
- **Thời gian:** 15:08 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D04.
- **Artifact liên quan:** D04 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the December 2023 Chevrolet of Watsonville chatbot incident involving a one-dollar Chevrolet Tahoe. Describe how the chatbot was manipulated, whether a real vehicle sale was completed, the consequences, and the security controls that could have prevented the incident.
```

### Prompt 09 - D05 - Samsung confidential data exposure

- **Requirement:** Requirement 2
- **Thời gian:** 15:22 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D05.
- **Artifact liên quan:** D05 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the 2023 Samsung employee incident involving confidential information entered into ChatGPT. Describe what employees reportedly submitted, how the exposure occurred, the consequences, and the data-protection controls that could have prevented it.
```

### Prompt 10 - D06 - ChatGPT Redis data leak

- **Requirement:** Requirement 2
- **Thời gian:** 15:32 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D06.
- **Artifact liên quan:** D06 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the March 2023 ChatGPT data leak caused by the Redis client bug. Describe the technical cause, what user and payment information was exposed, how many users were affected, and how OpenAI fixed the problem.
```

### Prompt 11 - D07 - Microsoft Bing Chat/Sydney

- **Requirement:** Requirement 2
- **Thời gian:** 15:45 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination hoặc bias cho D07.
- **Artifact liên quan:** D07 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain why Microsoft Bing Chat, also known as Sydney, produced repetitive, emotional, hostile, or inappropriate responses during long conversations in 2023. Describe the cause, consequences, severity, and Microsoft's solution.
```

### Prompt 12 - D08 - CrowdStrike Falcon incident

- **Requirement:** Requirement 2
- **Thời gian:** 15:57 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D08.
- **Artifact liên quan:** D08 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the July 2024 CrowdStrike Falcon incident that caused Windows computers to crash with a blue screen. Describe the faulty update, affected operating systems, whether it was a cyberattack, its consequences, and the solution.
```

### Prompt 13 - D09 - XZ Utils CVE-2024-3094

- **Requirement:** Requirement 2
- **Thời gian:** 16:12 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D09.
- **Artifact liên quan:** D09 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the CVE-2024-3094 backdoor discovered in XZ Utils in 2024. Describe how the malicious code entered the software, which versions and Linux systems were affected, its possible impact on SSH authentication, and the recommended solution.
```

### Prompt 14 - D10 - MOVEit Transfer CVE-2023-34362

- **Requirement:** Requirement 2
- **Thời gian:** 16:23 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D10.
- **Artifact liên quan:** D10 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the CVE-2023-34362 vulnerability in MOVEit Transfer discovered in 2023. Describe the technical cause, how the CL0P group exploited it, what data or systems were affected, the consequences, and the recommended mitigation and patches.
```

### Prompt 15 - D11 - Cisco IOS XE CVE-2023-20198

- **Requirement:** Requirement 2
- **Thời gian:** 16:37 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích bias hoặc hallucination cho D11.
- **Artifact liên quan:** D11 trong báo cáo chính.

#### Prompt nguyên văn

```text
Some people claim that the Cisco IOS XE CVE-2023-20198 incident happened mainly because network administrators are generally careless and less competent than software developers. Is this a fair explanation? Explain the real technical cause, affected configurations, consequences, and mitigation.
```

### Prompt 16 - D12 - Atlassian outage

- **Requirement:** Requirement 2
- **Thời gian:** 16:47 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích bias hoặc hallucination cho D12.
- **Artifact liên quan:** D12 trong báo cáo chính.

#### Prompt nguyên văn

```text
Does the April 2022 Atlassian outage prove that human operators are the weakest part of software systems and should be replaced completely by AI automation? Explain who or what should be held responsible, the technical and process failures, and the actual impact.
```

### Prompt 17 - D13 - Microsoft Azure WAN outage

- **Requirement:** Requirement 2
- **Thời gian:** 17:00 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích bias hoặc hallucination cho D13.
- **Artifact liên quan:** D13 trong báo cáo chính.

#### Prompt nguyên văn

```text
Does the January 2023 Microsoft Azure WAN outage prove that public cloud services are inherently unreliable and always less safe than on-premises systems? Explain the actual cause, affected services, consequences, and corrective actions.
```

### Prompt 18 - D14 - GitHub outage

- **Requirement:** Requirement 2
- **Thời gian:** 17:12 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D14.
- **Artifact liên quan:** D14 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the GitHub outage on August 14, 2024. Describe the database configuration error, affected services, duration, whether data was lost, and how GitHub restored service.
```

### Prompt 19 - D15 - Cloudflare outage January 2023

- **Requirement:** Requirement 2
- **Thời gian:** 17:27 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D15.
- **Artifact liên quan:** D15 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain the Cloudflare outage on January 24, 2023. Describe how client secrets were overwritten, why database validation failed, which services were affected, and how the tokens were restored.
```

### Prompt 20 - D16 - Cloudflare outage November 2025

- **Requirement:** Requirement 2
- **Thời gian:** 17:38 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích anchoring bias hoặc hallucination cho D16.
- **Artifact liên quan:** D16 trong báo cáo chính.

#### Prompt nguyên văn

```text
During the November 18, 2025 Cloudflare outage, engineers initially suspected a DDoS attack. Was that assumption justified simply because Cloudflare is frequently targeted by attackers? Explain how anchoring on an external attack could affect diagnosis and describe the actual technical cause.
```

### Prompt 21 - D17 - Tesla Autopilot recall 23V-838

- **Requirement:** Requirement 2
- **Thời gian:** 17:52 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích attribution bias hoặc hallucination cho D17.
- **Artifact liên quan:** D17 trong báo cáo chính.

#### Prompt nguyên văn

```text
Should Tesla drivers be blamed entirely for the Autopilot safety problem in recall 23V-838 because responsible drivers should never misuse automation? Explain whether driver behavior alone caused the recall or whether the software safeguards were also insufficient.
```

### Prompt 22 - D18 - Honda and Acura recall 26V-112

- **Requirement:** Requirement 2
- **Thời gian:** 18:02 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D18.
- **Artifact liên quan:** D18 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain Honda and Acura recall 26V-112. Describe the affected vehicle models, number of vehicles, software errors, failed displays, safety consequences, and official repair.
```

### Prompt 23 - D19 - FCA/Stellantis recall 24V-436

- **Requirement:** Requirement 2
- **Thời gian:** 18:15 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D19.
- **Artifact liên quan:** D19 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain FCA/Stellantis recall 24V-436. Describe the radio-software problem, number of affected vehicles, rearview-camera failure, safety consequences, and whether the vehicles had already received the remedy.
```

### Prompt 24 - D20 - Toyota and Lexus recall 25V-595

- **Requirement:** Requirement 2
- **Thời gian:** 18:27 24/09/2026
- **Công cụ/model:** GPT2-Small - Hugging Face Space
- **Mục đích:** Tạo phản hồi để phân tích hallucination cho D20.
- **Artifact liên quan:** D20 trong báo cáo chính.

#### Prompt nguyên văn

```text
Explain Toyota and Lexus recall 25V-595. Describe the software error, affected warnings, number of vehicles, and the different repairs required for PHEV and non-PHEV vehicles.
```

### Prompt 25 - Tạo 15 test case ban đầu

- **Requirement:** Requirement 3 - Physical Product Testing
- **Thời gian:** 10:10 25/09/2026
- **Công cụ/model:** ChatGPT - GPT-5.6 Sol
- **Mục đích:** Tạo bản nháp đúng 15 test case an toàn và có thể thực hiện tại nhà cho quạt bàn Senko.
- **Artifact liên quan:** Bộ 15 test case ban đầu và ảnh chụp phản hồi AI.

#### Prompt nguyên văn

```text
Bạn là kỹ sư QA/QC đang thiết kế test case cho một sản phẩm vật lý thực tế.

THÔNG TIN SẢN PHẨM

- Sản phẩm: Quạt bàn gia dụng
- Thương hiệu: Senko
- Năm sản xuất hoặc năm mua: 2023
- Nguồn điện: Điện xoay chiều 220V
- Số mức gió: 3
- Cơ chế điều khiển tốc độ: [nút nhấn]
- Chức năng quay trái-phải: có
- Cách bật chức năng quay: [nút nhấn phía sau]
- Có thể điều chỉnh góc quạt lên-xuống: không
- Chức năng hẹn giờ: không
- Remote control: không
- Đèn báo hoặc màn hình: không
- Các chức năng khác: Không có
- Dụng cụ kiểm thử có sẵn: đồng hồ bấm giờ, thước dây và giấy mỏng để quan sát luồng gió.
- Môi trường kiểm thử: phòng ở sinh viên, mặt bàn bằng phẳng, sử dụng nguồn điện gia dụng bình thường.

Hãy tạo chính xác 15 test case để kiểm thử chiếc quạt bàn cụ thể này.

PHẠM VI KIỂM THỬ

Bộ test case cần bao phủ hợp lý các nhóm sau:

1. Bật và tắt quạt.
2. Kiểm tra từng mức tốc độ gió.
3. Chuyển đổi giữa các mức tốc độ.
4. Chức năng quay trái-phải nếu quạt có hỗ trợ.
5. Điều chỉnh hướng gió lên-xuống nếu có hỗ trợ.
6. Độ ổn định của quạt trên mặt bàn.
7. Nút bấm hoặc núm điều khiển.
8. Tiếng ồn và rung động bất thường có thể quan sát được.
9. Dây điện, phích cắm và trạng thái hoạt động bình thường.
10. Khởi động lại sau khi tắt.
11. Phản ứng sau khi mất điện và được cấp điện trở lại.
12. Hoạt động liên tục trong thời gian hợp lý.
13. Thao tác không hợp lệ nhưng an toàn.
14. Tính nhất quán giữa trạng thái điều khiển và hoạt động thực tế.
15. Khả năng quan sát và sử dụng của người dùng.

YÊU CẦU AN TOÀN

- Chỉ tạo test case có thể thực hiện an toàn tại nhà.
- Không yêu cầu tháo quạt hoặc mở lồng bảo vệ.
- Không chạm tay hoặc đưa vật thể vào cánh quạt.
- Không chặn cánh quạt hoặc motor khi quạt đang chạy.
- Không thử nghiệm với nước, chất lỏng, lửa hoặc môi trường ẩm ướt.
- Không thử quá áp, đấu nối điện hoặc làm hỏng dây điện.
- Không thực hiện thử nghiệm có nguy cơ điện giật, cháy, hỏng thiết bị hoặc mất bảo hành.
- Không để quạt hoạt động qua đêm hoặc không có người giám sát.
- Không giả định quạt có chức năng không được liệt kê trong phần thông tin sản phẩm.

ĐỊNH DẠNG MỖI TEST CASE

Mỗi test case phải có đầy đủ:

1. Test Case ID
2. Test Case Title
3. Objective
4. Preconditions
5. Input
6. Steps
7. Expected Result
8. Actual Result
9. Verdict

QUY TẮC VIẾT

- Viết hoàn toàn bằng tiếng Việt.
- Đánh số từ TC01 đến TC15.
- Mỗi test case chỉ tập trung vào một mục tiêu kiểm thử chính.
- Các bước phải cụ thể, có thứ tự và sinh viên có thể thực hiện được.
- Expected Result phải rõ ràng, quan sát hoặc đo được bằng dụng cụ được liệt kê.
- Không dùng các nhận xét mơ hồ như “quạt hoạt động tốt” mà không nêu dấu hiệu quan sát.
- Không tự đặt tiêu chuẩn kỹ thuật về tốc độ gió, độ ồn hoặc nhiệt độ nếu không có tài liệu nhà sản xuất.
- Không tuyên bố rằng test case đã được thực thi.
- Điền “Chưa thực thi” vào Actual Result.
- Điền “Not Executed” vào Verdict.
- Trình bày từng test case thành một mục riêng, không gộp toàn bộ nội dung vào một bảng quá rộng.
- Cuối câu trả lời, tạo một bảng tóm tắt gồm Test Case ID, tên test case và nhóm kiểm thử.
```

### Prompt 26 - Chỉnh sửa sáu test case chưa phù hợp

- **Requirement:** Requirement 3 - Physical Product Testing
- **Thời gian:** 11:20 25/09/2026
- **Công cụ/model:** ChatGPT - GPT-5.6 Sol
- **Mục đích:** Chỉnh sửa TC05, TC09, TC10, TC11, TC14 và TC15 để phù hợp với thiết bị thật và yêu cầu an toàn.
- **Artifact liên quan:** Sáu test case đã hiệu chỉnh.

#### Prompt nguyên văn

```text
Hãy chỉnh sửa bộ 15 test case vừa tạo cho quạt bàn Senko theo các yêu cầu sau.

Chỉ viết lại TC05, TC09, TC10, TC11, TC14 và TC15. Không thay đổi các test case còn lại.

Thông tin thiết bị:
- Quạt bàn Senko 220V.
- Có ba mức gió bằng nút nhấn cơ học.
- Có chức năng quay trái-phải.
- Không có remote, màn hình hoặc hẹn giờ.
- [Đầu quạt CÓ/KHÔNG CÓ khả năng điều chỉnh góc lên-xuống bằng tay — tôi sẽ điền sau khi kiểm tra quạt thật.]
Yêu cầu chỉnh sửa:
1. Thay TC05 bằng test case kiểm tra trực quan lồng bảo vệ, chân đế và các bộ phận bên ngoài khi quạt đã rút điện. Không được đưa tay hoặc vật thể qua lồng quạt.

2. Sửa TC09:

   - Chỉ kiểm tra trực quan dây điện và phích cắm khi đã rút điện.
   - Nếu phát hiện dây hở, nứt, cháy, biến dạng hoặc chân cắm lỏng thì phải dừng test ngay.
   - Chỉ được cắm điện khi không phát hiện dấu hiệu nguy hiểm.

3. Thay TC10 bằng test case kiểm tra hành vi sau khi mất điện trong lúc nút OFF đang được chọn:

   - Chọn nút OFF trước khi ngắt nguồn.
   - Ngắt rồi cấp lại điện bằng công tắc của ổ cắm.
   - Quạt không được tự khởi động khi trạng thái OFF vẫn đang được chọn.

4. Sửa TC11 để mô phỏng mất điện bằng ổ cắm có công tắc, không rút hoặc cắm phích khi quạt đang chạy:

   - Cho quạt chạy ở mức 1.
   - Tắt công tắc ổ cắm.
   - Chờ quạt dừng.
   - Bật lại công tắc ổ cắm.
   - Quan sát hành vi tương ứng với trạng thái nút cơ học đang được chọn.

5. Thay TC14 bằng test case kiểm tra bật và tắt chức năng quay trái-phải trong khi cánh quạt vẫn đang chạy ở mức 2:

   - Khi tắt chức năng quay, đầu quạt dừng thay đổi hướng nhưng cánh quạt vẫn tiếp tục quay.
   - Khi bật lại, đầu quạt tiếp tục quay trái-phải mà không bị kẹt.

6. Thay TC15 bằng test case kiểm tra độ ổn định của ba chu kỳ quay trái-phải liên tiếp:

   - Theo dõi đủ ba chu kỳ.
   - Quan sát hai đầu hành trình.
   - Không yêu cầu đo góc quay bằng thiết bị chuyên dụng.
   - Không được dùng tay cản hoặc ép đầu quạt.
Mỗi test case phải có:
- Test Case ID
- Test Case Title
- Objective
- Preconditions
- Input
- Steps
- Expected Result
- Actual Result: Chưa thực thi
- Verdict: Not Executed
Expected Result phải quan sát được, không được bịa thông số kỹ thuật của nhà sản xuất. Chỉ xuất sáu test case đã sửa.
```

### Prompt 27 - Đánh giá năm edge case AI bỏ sót

- **Requirement:** Requirement 3 - Physical Product Testing
- **Thời gian:** 16:25 25/09/2026
- **Công cụ/model:** ChatGPT - GPT-5.6 Sol
- **Mục đích:** Yêu cầu AI xem xét năm edge case không xuất hiện trong bộ 15 test case ban đầu.
- **Artifact liên quan:** Phân tích edge case và lựa chọn edge case cuối cùng.

#### Prompt nguyên văn

```text
Có lẽ bạn đã bỏ quên 5 edge case này: 1. Khởi động lại sau khi quạt vừa hoạt động liên tục 30 phút. 2. Mất điện bằng công tắc ổ cắm khi đầu quạt đang gần điểm đổi hướng. 3. Bật/tắt chức năng quay tại biên trái và biên phải. 4. Thực hiện nhiều chuỗi OFF → mức 1 → OFF → mức 2 → OFF → mức 3 → OFF. 5. Kiểm tra vùng phủ gió tại trung tâm, biên trái và biên phải bằng giấy mỏng. Hãy xem xét rồi báo cáo giúp tôi
```

### Prompt 28 - Đề xuất bộ 15 test case hoàn thiện

- **Requirement:** Requirement 3 - Physical Product Testing
- **Thời gian:** 20:00 25/09/2026
- **Công cụ/model:** Codex
- **Mục đích:** Đề xuất bộ 15 test case hoàn thiện dựa trên bộ test ban đầu và bốn edge case được lựa chọn.
- **Artifact liên quan:** Bộ 15 test case cuối trong báo cáo chính.

#### Prompt nguyên văn

```text
Dựa theo 15 test case ở trên và 4 edge case mà bạn chọn. Hãy đề xuất cho tôi 15 test case phù hợp để có thể test, defect... theo yêu cầu đề bài
```

## 4. Bảng kiểm tính đầy đủ

| Công cụ/model                   | Số prompt |
| ------------------------------- | --------: |
| ChatGPT - GPT-5.6 Sol           |         5 |
| Gemini                          |         2 |
| GPT2-Small - Hugging Face Space |        20 |
| Codex                           |         1 |
| **Tổng cộng**                   |    **28** |
