# Visibility report

- Thư mục nhãn: `dataset\labels\train`
- 20 ảnh, 29 skeleton, trung bình 13.55 khớp có v > 0 mỗi người
- Tổng: v=2 333 | v=1 60 | v=0 100

| # | Khớp | v=2 | v=1 | v=0 | %v=1 |
| ---: | --- | ---: | ---: | ---: | ---: |
| 0 | nose | 22 | 0 | 7 | 0% |
| 1 | left_eye | 19 | 3 | 7 | 10% |
| 2 | right_eye | 21 | 1 | 7 | 3% |
| 3 | left_ear | 13 | 6 | 10 | 21% |
| 4 | right_ear | 17 | 6 | 6 | 21% |
| 5 | left_shoulder | 26 | 3 | 0 | 10% |
| 6 | right_shoulder | 27 | 2 | 0 | 7% |
| 7 | left_elbow | 23 | 2 | 4 | 7% |
| 8 | right_elbow | 26 | 2 | 1 | 7% |
| 9 | left_wrist | 19 | 4 | 6 | 14% |
| 10 | right_wrist | 21 | 3 | 5 | 10% |
| 11 | left_hip | 20 | 9 | 0 | 31% |
| 12 | right_hip | 21 | 7 | 1 | 24% |
| 13 | left_knee | 15 | 2 | 12 | 7% |
| 14 | right_knee | 16 | 4 | 9 | 14% |
| 15 | left_ankle | 14 | 2 | 13 | 7% |
| 16 | right_ankle | 13 | 4 | 12 | 14% |

## Đọc bảng này thế nào

1. Khớp nào có **%v=1 cao**: khớp hay bị che. Cổ tay và hông thường là hai vị trí cần xem lại guideline trước khi kết luận.
2. Khớp nào có **v=0 cao bất thường**: mọi người đang dùng Outside ở chỗ đáng lẽ là Occluded. Đó là lỗi số 3 của slide 46, và nó xoá thẳng khớp đó khỏi bảng điểm OKS.
3. Khi so hai người: **lệch lớn = bất đồng về guideline**, không phải về bức ảnh. Sửa guideline trước, sửa nhãn sau.
