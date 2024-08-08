# Data Collection workshop

ใน Workshop นี้จะทำบน Google Colab โดยจะมี Step ดังนี้
1) ดึงข้อมูลจาก MySQL
2) ดึงข้อมูลจาก API
3) Merge / Join ข้อมูล
4) Output ผลลัพธ์

[เกี่ยวกับ Dataset] ข้อมูลที่ใช้ในการทำ Workshop นี้มาจาก E-commerce Business Transaction Dataset ใน Kaggle: https://www.kaggle.com/datasets/gabrielramos87/an-online-shop-business/data

โดยได้ทำการแปลงข้อมูลออกเป็น 3 table และนำเข้า database

ข้อมูลดั้งเดิมมีทั้งหมด 8 columns:

- TransactionNo (หมวดหมู่): รหัสการทำรายการ (อักษร “C” ในรหัสระบุการยกเลิก)
- Date (ตัวเลข): วันที่ทำรายการ
- ProductNo (หมวดหมู่): รหัสสินค้า
- Product (หมวดหมู่): ชื่อสินค้า
- Price (ตัวเลข): ราคาสินค้าต่อหน่วย หน่วยเป็นปอนด์ (£)
- Quantity (ตัวเลข): จำนวนสินค้า แต่ละรายการต่อธุรกรรม (ค่าติดลบหมายถึงรายการที่ยกเลิก)
- CustomerNo (หมวดหมู่): รหัสสมาชิกลุกค้าแต่ละราย
- Country (หมวดหมู่): ชื่อประเทศที่ลูกค้าอาศัยอยู่