# 📑 DAX Documentation  

This file contains the main DAX measures used in the **Retail Sales Dashboard**.  

### Total Sales  
```DAX
Total Sales = SUM(Sales[SalesAmount])
```  

### Total Sales YTD  
```DAX
Total Sales YTD = TOTALYTD(SUM(Sales[SalesAmount]), 'Date'[Date])
```  

### Gross Profit  
```DAX
Gross Profit = [Total Sales] - [Total Cost]
```  

### Variance from Target  
```DAX
Variance from Target = [Total Sales] - [Target Sales]
```  

### Profit Margin %  
```DAX
Profit Margin % = DIVIDE([Gross Profit], [Total Sales], 0)
```  

---
