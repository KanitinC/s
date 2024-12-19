import matplotlib.pyplot as plt

# ข้อมูลยอดขาย 14 เดือน
sales = [
    341222, 563816, 721532, 793172, 772231, 694292, 
    844719, 944558, 730759, 836519, 811056, 381206, 
    98175, 41574
]
months = [
    "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
    "Jul", "Aug", "Sep", "Oct", "Nov", "Dec", 
    "Jan (Yr2)", "Feb (Yr2)"
]

# สร้างกราฟ
plt.figure(figsize=(10, 6))
plt.plot(months, sales, marker='o', color='blue', label="Sales")
plt.title("Monthly Sales Over 14 Months", fontsize=16)
plt.xlabel("Months", fontsize=12)
plt.ylabel("Sales (in THB)", fontsize=12)
plt.grid(True, linestyle='--', alpha=0.7)
plt.xticks(rotation=45)
plt.legend()
plt.tight_layout()

# แสดงกราฟ
plt.show()
