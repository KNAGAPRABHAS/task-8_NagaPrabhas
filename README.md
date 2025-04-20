

---

# 📊 Task 8: Simple Sales Dashboard Design – README

## 🎯 Objective:
Create a **basic interactive dashboard** using **Power BI** to display **sales performance** by **product, region, and month** using a dataset like `Superstore_Sales.csv`.

---

## 🛠 Tools Used:
- **Power BI Desktop**
- (Optional) Excel or Python for minor data cleaning

---

## 📁 Dataset:
- `Superstore_Sales.csv`  
  Columns include:
  - Order Date
  - Region
  - Category
  - Sales
  - Profit

---

## ✅ Steps Followed:

### 🔹 **Step 1: Import the CSV File**
- Open Power BI → Click **Home > Get Data > Text/CSV**
- Load the dataset `Superstore_Sales.csv` into Power BI

---

### 🔹 **Step 2: Create “Month-Year” from Order Date**
- In **Data view**, click **New Column** and enter:
  ```DAX
  MonthYear = FORMAT([Order Date], "MMM YYYY")
  ```
- (Optional for sorting) Add:
  ```DAX
  MonthSort = FORMAT([Order Date], "YYYYMM")
  ```
- Use `MonthSort` to sort `MonthYear` properly.

---

### 🔹 **Step 3: Add Visuals**
- 📈 **Line Chart**:  
  - Axis: `MonthYear`  
  - Values: `Sales`  
  - Shows sales trend over time

- 📊 **Bar Chart**:  
  - Axis: `Region`  
  - Values: `Sales`  
  - Shows total sales by region

- 🍩 **Donut Chart**:  
  - Legend: `Category`  
  - Values: `Sales`  
  - Shows sales distribution by product category

---

### 🔹 **Step 4: Add Slicer**
- Insert a **Slicer Visual** from the **Visualizations pane**
- Drag **`Region`** or **`Category`** into the slicer field
- Customize:
  - Enable **single or multi-select**
  - Optional: Set orientation to **horizontal** or use **dropdown**

---

---

### 🔹 **Step 6: Write 3 Short Insights**

#### 📌 Insights based on visuals:
1. **West region** had the highest total sales across all quarters.  
2. The **Technology** category generated the most revenue and profit.  
3. **December** recorded the peak in sales, indicating strong seasonal trends.

---

## 📦 Deliverables:

- ✅ Power BI Dashboard file (`.pbix`)
- ✅ Screenshot
- ✅ This `README.md` file
- ✅ Text/Slide file with **3 insights**

---

## 📸 Example Dashboard Elements:
- Line chart showing monthly sales trend  
- Bar chart comparing regional performance  
- Donut chart highlighting sales by category  
- Region filter/slicer for interactivity  
- Clear color-coded highlights for high performers  

![image](https://github.com/user-attachments/assets/67e7b942-b1dd-4f10-8749-2d8f0d405181)
![image](https://github.com/user-attachments/assets/fefa2f3d-a451-4a02-a23f-879d51c7320d)
![image](https://github.com/user-attachments/assets/401fc714-8f33-4dd0-8a61-8dd3a8452c4d)
![image](https://github.com/user-attachments/assets/decef67c-dac7-48b3-af71-f427aad2c549)
![image](https://github.com/user-attachments/assets/cc80c436-e806-4685-bcf0-eb2b5992cd2d)



---
