# MyPaint
โปรเจคนี้มีชื่อว่า "MyPaint" ทำขึ้นเพื่อสร้างโปรแกรมวาดรูปด้วยภาษา Python โดยใช้ tkinter ในการสร้าง GUI และใช้ pyinstaller ในการทำเป็น .exe

วิธีใช้งานโปรแกรม คือ ใช้เมาส์ในการวาดสิ่งต้องการลงในโปรแกรม สามารถ save, open, undo, redo, clear, เลือกสี และเลือกความหนาของเส้นได้

![alt text](https://github.com/tsunafield1/MyPaint/blob/main/Example.PNG)

สามารถเปิดไฟล์ที่บันทึกไว้ได้ที่เมนู File -> Open

![alt text](https://github.com/tsunafield1/MyPaint/blob/main/Example2.PNG)

สามารถบันทึกไฟล์ลงไดเรกทอรี่ที่เลือกไว้ได้ที่เมนู File -> Save

![alt text](https://github.com/tsunafield1/MyPaint/blob/main/Example3.PNG)

สามารถเปลี่ยนไดเรกทอรี่สำหรับบันทึกไฟล์ได้ที่เมนู File -> Change save directory

![alt text](https://github.com/tsunafield1/MyPaint/blob/main/Example4.PNG)

สามารถ undo, redo และ clear ไดที่เมนู Edit

สามารถเปลี่ยนสีของเส้นได้ที่เมนู Color 
- สามารถเลือกจาก 3 สีล่าสุดที่ใช้งานได้ที่เมนู Color -> Recent
- สามารถเลือกจากสีพื้นฐานของโปรแกรมได้ที่เมนู Color -> General
- สามารถเลือกสีอื่นๆ ได้ที่เมนู Color -> Custom

![alt text](https://github.com/tsunafield1/MyPaint/blob/main/Example5.PNG)

สามารถเปลี่ยนความหนาของเส้นได้ที่เมนู Size

สามารถทดลองใช้งานได้ด้วยการเปิดไฟล์ MyPaint.exe โดยจะมีการสร้างไฟล์เริ่มต้นของโปรแกรมขึ้นมาที่ D:\MyPaint

-----------------------

ใน Source มี 1 ไฟล์
- MyPaint.py คือ ไฟล์โค้ดของโปรแกรม

ใน Source/MyPaint.py มี 4 class
- Stack คือ โครงสร้างข้อมูลแบบ Stack สร้างด้วย list
- Queue คือ โครงสร้างข้อมูลแบบ Queue สร้างด้วย deque
- FileData คือ class ที่ใช้สำหรับอ่าน และเปรียบเทียบเวลาของไฟล์
- Sketchpad(Canvas) คือ class ควบคุมการทำงานทั้งหมดของโปรแกรม

มี 2 function
- QuickSort(li, left, right) คือ ฟังก์ชั่นสำหรับทำการเรียงข้อมูลแบบ Quick sort ใช้ในการเรียงไฟล์จากชื่อไฟล์
- InsertSort(li) คือ ฟังก์ชั่นสำหรับทำการเรียงข้อมูลแบบ Insertion sort ใช้ในการเรียงไฟล์จากเวลาที่ทำการบันทึกไฟล์

โปรเจคนี้เป็นส่วนหนึ่งของวิชา Data Structures and Algorithm ภาควิชาวิศวกรรมคอมพิวเตอร์ คณะวิศวกรรมศาสตร์ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง
