# Thành viên và phân việc — Day11 SVM 360 Fisheye · Nhóm ThangDz

## 1. Thông tin nhóm

- Khóa/lớp: AI thực chiến L2–L3 K4P1
- Tên nhóm: ThangDz
- Repo nhóm (Public): https://github.com/cuducquang/K4-DAY11-ThangDz
- Cách tổ chức: mỗi thành viên làm một slice riêng trong repo cá nhân, tự làm cả ba vai (gán nhãn, QA, chẩn đoán); QA chéo theo vòng trong `team.json`.
- Vòng QA (`team.json` → `qa_reviews`, người bên trái soát bài người bên phải): cuducquang → nguyenductung → nguyentrongthang → cuducquang.

## 2. Bảng thành viên

| Họ và tên | MSSV | Tên dùng trong mode | Slice được giao | QA bài của ai | Phần việc và bằng chứng | Link repo cá nhân | Commit nộp |
|---|---|---|---|---|---|---|---|
| Cù Đức Quang | 2A202602188 | cuducquang | B3-dense | Nguyễn Đức Tùng (B2-center) | P0–P6 đầy đủ. Khóa r1_craft `1093-F4B9`, rework `462F-999C`. `check` exit 0, `failed_gates` rỗng. | https://github.com/cuducquang/K4-L2-DAY11-CuDucQuang-2A202602188-SVM360-Fisheye | [`190e047`](https://github.com/cuducquang/K4-L2-DAY11-CuDucQuang-2A202602188-SVM360-Fisheye/commit/190e0476078ca9c4788f0b5a0730e7c3da6ff6b7) |
| Nguyễn Trọng Thắng | 2A202602169 | nguyentrongthang | B3-mid | Cù Đức Quang (B3-dense) | P0–P6 đầy đủ. Khóa r1_craft `F056-82C1`, rework `4E4E-6FF7`. `check` exit 0, `failed_gates` rỗng. | https://github.com/trogthang/K4-L2-DAY11-CuDucQuang-2A202602188-SVM360-Fisheye | [`29455d3`](https://github.com/trogthang/K4-L2-DAY11-CuDucQuang-2A202602188-SVM360-Fisheye/commit/29455d3efad00dec636b0e0dbc2259a090a7909d) |
| Nguyễn Đức Tùng | 2A202602227 | nguyenductung | B2-center | Nguyễn Trọng Thắng (B3-mid) | Đang làm: xong P0–P2, khóa r1_craft `B214-53BB`. Chưa có QA, chẩn đoán, rework, card. | https://github.com/NDTung23/K4-L2-DAY11-CuDucQuang-2A202602188-SVM360-Fisheye | [Điền khi xong] |

## 3. Bàn giao QA chéo

| Người soát → bài được soát | Mã khóa được soát | File review (trong repo người soát) | Trạng thái |
|---|---|---|---|
| cuducquang → nguyenductung (B2-center) | `B214-53BB` | [Điền] | Chưa làm. Lúc Quang tới P3, bài của Tùng chưa khóa nên Quang áp dụng phương án dự phòng và tự soát nguội slice của mình. |
| nguyenductung → nguyentrongthang (B3-mid) | `F056-82C1` | [Điền] | Chưa làm |
| nguyentrongthang → cuducquang (B3-dense) | `1093-F4B9` | [Điền] | Chưa đúng vòng: `r2_qa/qa_review.md` của Thắng hiện là bài soát slice B3-mid của chính Thắng. |

## 4. Bất đồng và phối hợp

- **Một ca đã phân xử:** `adasind_199770.jpg`, vật sát mép phải (B3-dense). Vùng `ego_body` hình chữ nhật của reference phủ lên một ThreeWheeler thật và một người đứng. Quang giữ nhãn đúng, không sửa để khớp số, và escalate lỗi của reference. Bằng chứng: `submission/30_escalation_ticket.md` (Ticket 1) và `40_decision_log.csv` dòng D1 trong repo của Quang.
- **Ca còn mở:** 199770 M9, L10/L11 (vật trong hiên tối), ghi `E5_unresolved` ở D8. Bước kiểm tiếp: xem frame video liền kề và nhận xét của người soát chéo.
- **Thay đổi phân công:** không đổi slice. Khác biệt duy nhất là phần QA ở mục 3.

## 5. Xác nhận trước khi nộp

- [x] cuducquang: `check` exit 0, `manifest.json` có `failed_gates` rỗng tại `190e047`.
- [x] nguyentrongthang: `check` exit 0, `manifest.json` có `failed_gates` rỗng tại `29455d3`.
- [ ] nguyenductung: `check` exit 0, `failed_gates` rỗng.
- [ ] Ba file `qa_review.md` đúng vòng QA đã có trong repo của người soát.
- [ ] Repo nhóm Public, mọi link mở được.

Chỉ đánh dấu việc đã kiểm thật. Không chạy `check` trong repo nhóm.
