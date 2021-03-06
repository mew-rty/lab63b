# การทดลองที่ 2 เรื่อง การเขียนโปรแกรมค้นหาไวไฟ

## วัตถุประสงค์
1.เพื่อศึกษาวิธีการเขียนโปรแกรมและcodeของการเขียนการทดลอง 
 
 2.เรียนรู้การใช้คำสั่งต่างๆของการเขียนโปรแกรม
 
 3.เพื่อศึกษาการใช้ platfrom IO
## อุปกรณ์ที่ใช้
   1.ไมโครคอนโทรเลอร์ esp-01 แบบมี wifi
  
  2.USB to serial
  
  3.อุปกรณ์ที่ใช้สำหรับเขียนโปรแกรม (คอมพิวเตอร์ โน๊ตบุ๊ค) 

## ศึกษาข้อมูลเบื้องต้น
https://youtu.be/yBjab0UNuB8
## วิธีการทำการทดลอง
  1.เสียบไมโครคอนโทเลอร์เข้ากับ USB to serial
  
  ![image](https://user-images.githubusercontent.com/80879829/112275297-0cb22180-8cb2-11eb-9a5b-5272312e3d28.png)
 
 2.เตรียมอัพโหลดโปรแกรม
   
  ดูหน้าตัวอย่างโปรแกรม platfromio.ini src ----> vi src/main.cpp  0twf
  
 3.อัพโหลดโปรเเกรมเข้าไปยังไมโครคอนโทรเลอร์โดยใช้คำสั่ง pio run -t upload แล้วกดปุ่มสีดำลงไป 

![image](https://user-images.githubusercontent.com/80879829/112279829-eb076900-8cb6-11eb-86cc-847e3a6f90ce.png)

เมื่อเสร็จจะเป็นเเบบนี้

![image](https://user-images.githubusercontent.com/80879829/112280129-433e6b00-8cb7-11eb-9a36-c9da5f56d1a1.png)

4.ใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์ว่าพบ wifi อะไรบ้าง

## การบันทึกผลการทดลอง
จะสังเกตเห็น WiFi ที่พบได้คือ 4-5 ตัว เเล้วเเต่ความเเรงของสัญญาณที่ได้รับ

![image](https://user-images.githubusercontent.com/80879829/112280477-a203e480-8cb7-11eb-8eed-c443e8965266.png)

## อภิปรายผลการทดลอง 
จากผลจะสังเกตเห็น WiFi ที่พบได้คือ 4-5 ตัว เเล้วเเต่ความเเรงของสัญญาณที่ได้รับ แต่ถ้ามีความเเรงของสัญญาณอื่นที่รับได้ก็จะเเดงออกมามากกว่านี้
## คำถามหลังการทดลอง
Q..สามารถค้นหาทwifiได้มากที่สุดเท่าไร

A..ไม่มีขีดจำกัดเเล้วเเต่ความเเรงที่ได้รับ
