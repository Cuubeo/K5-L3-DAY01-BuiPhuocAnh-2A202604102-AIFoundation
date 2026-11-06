# Báo cáo cá nhân — Day 01: Lọc tin nhắn rác bằng ML, DL, Embedding và LLM

- **MSSV: 2A202604102**
- **Họ và tên: Bùi Phước Anh**
- **SEED: 2A202604102** (in ở ô đầu notebook):

## 1. Bằng chứng

| Tệp | Có? |
| --- | --- |
| [`day01_lab.ipynb`](day01_lab.ipynb) — notebook đã chạy, còn output | ☐ |
| [`lab1_report.json`](lab1_report.json) — do ô "Báo cáo cuối" sinh ra | ☐ |
| [`hand_calc.jpg`](hand_calc.jpg) — ảnh tính tay có các bước | ☐ |

## 2. Kết quả chính
                                     f1  f1_SUB
1. BoW + LogReg (tự code)        0.888   0.919
2. BoW + MLP (deep learning)     0.975   0.974
3a. Encoder (MiniLM) + kNN       0.917   0.976
3b. Encoder (MiniLM) + LogReg    0.941   0.919
3c. Encoder (MiniLM) + MLP head  0.946   0.919
## 3. Dự đoán và thực tế

dự đoán [ml_f1] tôi dự đoán kết quả là ~0.8 nhưng kết quả thực tế thì cao hơn lên tới 0.905
dự đoán [ml_lr] tôi dự đoán ở lr=0.001 thì loss đi ngang, tuy nhiên nó đi theo đường dốc thoải xuống
dự đoán [dl_curve] tôi dự đoán val loss sẽ càng tiến gần về không nếu càng huấn luyện nhiều và sẽ dừng lại, tuy nhiên sau 11 epoch thì val loss lại tăng lên
