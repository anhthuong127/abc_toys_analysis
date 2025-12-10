**🧸 ABC Toys – Sales Performance Analysis**

**📌 Project Overview | Tổng quan dự án**

(EN)
This dataset contains transactional and performance information for a network of retail stores.
It is designed for business analysis, performance benchmarking, and deep-dive investigations into what drives top-performing and under-performing stores.
The dataset enables users to evaluate profitability, sales volume, and product-level contributions across different stores.

(VN)
Bộ dữ liệu này chứa thông tin về giao dịch và hiệu suất kinh doanh của một mạng lưới cửa hàng bán lẻ. Dữ liệu được xây dựng nhằm phục vụ phân tích hoạt động kinh doanh, so sánh hiệu quả giữa các cửa hàng và phân tích chuyên sâu các yếu tố ảnh hưởng đến hiệu suất cao hoặc thấp của từng cửa hàng. Dataset cho phép đánh giá lợi nhuận, sản lượng bán và mức độ đóng góp của từng sản phẩm tại mỗi cửa hàng.

**📂 Dataset | Nguồn dữ liệu**

(EN)
The dataset simulates transactional and operational data of a toy retail chain, provided for academic purposes by the University of Science (VNU-HCM).

(VI)
Dữ liệu hoạt động kinh doanh của chuỗi cửa hàng đồ chơi ABC Toys, được cung cấp cho mục đích học thuật bởi Trường Đại học Khoa học Tự nhiên – ĐHQG TP.HCM.

**Main Tables | Các bảng chính**

- Sales: Sale_ID, Date, Store_ID, Product_ID, Units
- Products: Product_ID, Product_Name, Product_Category, Product_Cost, Product_Price
- Stores: Store_ID, Store_Name, Store_City, Store_Location, Store_Open_Date
- Inventory: Store_ID, Product_ID, Stock_On_Hand

**🎯 Project Objectives | Mục tiêu phân tích**

(EN)
- Evaluate overall revenue, profit, and margin trends
- Analyze business performance by store, city, and location type
- Identify top-performing and underperforming products
- Assess inventory levels and detect stock risks
- Provide actionable recommendations for business improvement

(VI)
- Đánh giá xu hướng doanh thu, lợi nhuận và biên lợi nhuận
- Phân tích hiệu quả kinh doanh theo cửa hàng, thành phố và vị trí
- Xác định sản phẩm bán chạy và bán kém
- Phân tích tình trạng tồn kho
- Đề xuất giải pháp cải thiện hiệu quả kinh doanh

**🔎 Methodology | Quy trình thực hiện**

**Step 1: Data Understanding & ERD**

Identify relationships between Sales – Products – Stores – Inventory
Build ERD to understand data structure

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/dd3cca84-7419-46b1-846c-db6c51f7532b" />

**Step 2: Data Cleaning & Preparation (Python)**

(EN)
- Convert price and cost columns from string to numeric
- Convert date columns to datetime format
- Merge all tables into a unified dataset
- Remove records with missing Stock_On_Hand
- Create new features:
+ Revenue
+ Profit
+ Month
+ Detect and remove outliers (Units > 10)
(VI)
- Chuyển kiểu dữ liệu giá và ngày tháng
- Gộp các bảng dữ liệu
- Loại bỏ dữ liệu thiếu ở cột tồn kho
- Tạo thêm các cột doanh thu, lợi nhuận, tháng
- Loại bỏ outlier ở cột số lượng bán

**Step 3: Exploratory Data Analysis & Visualization**

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/503e9f5b-a4b7-46f9-aaab-91712bf36518" />

**📊 Key Insights | Insight chính**

**1. Overall Business Performance | Tổng quan**

✅ All stores are profitable

📈 Revenue and profit increased in 2023 compared to 2022

📉 Profit margin slightly decreased due to decline in Colorbuds sales
<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/f9e6f80e-2d9a-4e43-9aef-91e946b56244" />

**2. Store & Location Performance | Hiệu quả theo cửa hàng**
(EN)
- Airport stores (ID 30, 31) generate the highest revenue
- Residential areas show average performance
- Underperforming stores (ID 5, 26, 40) suffer from low sales volume rather than pricing or margin issues

(VI)
- Các cửa hàng khu vực sân bay có doanh thu cao nhất
- Các cửa hàng bán kém chủ yếu do số lượng bán thấp, không phải do giá hay biên lợi nhuận

  <img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/e8d74512-ea5f-4aa0-b3a5-96d4bba9fa6d" />


**➡️ Recommended actions:**
- Improve store layout and visual merchandising
- Increase promotions and local marketing
- Train staff to improve customer experience

**3. Time & Seasonality | Thời gian & mùa vụ**

- Weekends (Friday–Saturday) have the highest revenue
- Peak months: April–May and September
- Games peak in January–February due to holidays and promotions

--> Inventory and staffing should align with seasonal demand.

<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/3282ca2c-0d33-412f-ba27-d201112a0608" />

**4. Product Performance | Hiệu quả sản phẩm**

- Toys & Electronics contribute the highest profit
- Colorbuds: high margin, strong profit driver but declining sales
- Magic Sand: strong sales growth but lower margin
- Low-performing products to consider reducing:
+ Classic Dominoes
+ Uno Card Game

<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/bd95936e-0d6c-41bd-9fb4-62fb5acd8bd2" />

**5. Inventory Analysis | Phân tích tồn kho**
- Overstock products: Deck of Cards, PlayDoh Can → need promotion or price adjustment
- Low stock, high-margin products: Jenga, Playfoam → increase stock

<img width="1399" height="701" alt="image" src="https://github.com/user-attachments/assets/7764f079-0913-41ee-8525-026954562080" />

**✅ Business Recommendations | Đề xuất**
(EN)

- Expand stores in high-performing locations (airports)
- Focus on medium-price, high-margin products
- Optimize inventory based on seasonality
- Reduce low-profit, slow-moving products
- Improve store experience for underperforming locations

(VI)
- Mở rộng cửa hàng tại khu vực doanh thu cao như Airport
- Ưu tiên sản phẩm giá trung bình, biên lợi nhuận cao như Color Buds
- Điều chỉnh tồn kho theo mùa vụ, tăng cường dự trữ Toys và tổ chức bán 
- Cắt giảm sản phẩm bán chậm, lợi nhuận thấp
- Nâng cao trải nghiệm tại các cửa hàng bán kém

**🛠️ Tools & Technologies | Công cụ sử dụng**

- Python (Pandas)
- Tableau

**🚀 Project Links | Liên kết dự án**

**Authour:** Thuong Tran 
LinkedIn Profile: https://www.linkedin.com/in/trananhthuong

**📊 Tableau Story:**
https://public.tableau.com/app/profile/tran.thuong6933/viz/ABC_toys_project1_17649249940680/StoryF

**💻 GitHub (Code):**
https://github.com/anhthuong127/abc_toys_analysis

**📂 Cleaned Data:**
https://drive.google.com/drive/folders/1I-GiRSyvC9FNxTpFroYZ189g_n3JNDEY


📌 View all my explaination HERE! https://drive.google.com/drive/folders/1I-GiRSyvC9FNxTpFroYZ189g_n3JNDEY
