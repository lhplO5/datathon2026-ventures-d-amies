# 🧩 DATATHON 2026 — THE GRIDBREAKER

Team name: Ventures D'amies
Members:
- Lê Hoàng Phương Linh – lhpl172005@gmail.com
- Trần Duy Hưng – tranduyhung0802@gmail.com
- Lê Ngọc Mai – macehelix@proton.mail
- Trương Hoàng Bách - 23bach.th@vinuni.edu.vn

Hosted by VinTelligence — VinUni DS&AI Club
Vòng 1: Data Science Competition – Time Series Forecasting & Business Analytics


📌 Problem statement

Dự báo doanh thu thuần (Revenue) và giá vốn (COGS) cho một công ty thương mại điện tử thời trang tại Việt Nam trong giai đoạn 01/01/2023 – 01/07/2024 dựa trên dữ liệu lịch sử từ 04/07/2012 – 31/12/2022.

Bài toán yêu cầu:
- Xây dựng mô hình dự báo chuỗi thời gian
- Phân tích EDA & trực quan hóa dữ liệu (60% điểm)
- Trả lời 10 câu hỏi trắc nghiệm (20% điểm)


📊 Dataset overview

Bộ dữ liệu gồm 15 file CSV, chia thành 4 lớp:

Lớp Master: products, customers, promotions, geography - Dữ liệu tham chiếu
Lớp Transaction: orders, order_items, payments, shipments, returns, reviews - Giao dịch
Lớp Analytical: sales, sample_submission - Doanh thu (train) & nộp bài
Lớp Operational: inventory, web_traffic - Tồn kho, traffic

Time range:
- Train: sales.csv – 04/07/2012 → 31/12/2022
- Test: sales_test.csv – 01/01/2023 → 01/07/2024


📁 Repository structure

datathon-2026-the-gridbreakers/
├── README.md
├── report/
│   └── Venture_d_amies___NeurIPS_2026_template.pdf
├── mcq/
│   └── mcq_final.ipynb
├── eda/
│   ├── notebook_eda/
│       └── ventures-d-amies-eda-datathon-2026-ver2.ipynb
│   ├── notebook_visualization/
│   └── powerbi_dashboard/
├── model/
    ├── notebook/
    └── submission/



🧪 How to reproduce results

1. Environment setup
Install required Python packages (pandas, numpy, matplotlib, seaborn, scikit-learn, lightgbm, xgboost, shap, plotly)

2. Data preparation
Run the following notebooks in order:
- eda/notebook/ventures-d-amies-eda-datathon-2026-ver2.ipynb
- eda/notebook_visualization/
- model/powerbi_dashboard/

3. Reproduce submission
Upload the notebook to Kaggle, import the competition dataset, and run the notebook. The submission.csv file will be generated automatically.


📈 Evaluation metrics

Bài nộp được đánh giá trên test set bằng:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² (Coefficient of Determination)

MAE & RMSE càng thấp, R² càng cao (gần 1) càng tốt.


📎 Important links

Kaggle Competition: https://www.kaggle.com/competitions/datathon-2026-round-1
NeurIPS 2025 Template: https://neurips.cc/Conferences/2025/CallForPapers
VinTelligence Fanpage: https://www.facebook.com/VinTelligence


✅ Checklist nộp bài - Vòng 1

[x] Đáp án 10 câu trắc nghiệm (mcq/answers.md)
[x] Phân tích EDA + biểu đồ (eda/)
[x] Mô hình dự báo + file submission.csv
[x] Báo cáo PDF (tối đa 4 trang, theo template NeurIPS)
[x] GitHub repository public
[x] Form nộp bài chính thức của BTC
[x] Ảnh thẻ sinh viên tất cả thành viên
[x] Cam kết tham gia Chung kết trực tiếp (23/05/2026 tại VinUni)