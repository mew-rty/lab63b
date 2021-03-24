## การทดลองที่ 4 เรื่อง การเขียนโปรแกรมอินพุทสัญญาณดิจิทัล
## วัตถุประสงค์
 1.เพื่อศึกษาวิธีการเขียนโปรแกรมและcodeของการเขียนการทดลอง 
 
 2.เรียนรู้การใช้คำสั่งต่างๆของการเขียนโปรแกรม
 
 3.เพื่อศึกษาการใช้ platfrom IO
## อุปกรณ์ที่ใช้
   1.ไมโครคอนโทรเลอร์ esp-01
  
  2.USB to serial
  
  3.อุปกรณ์ที่ใช้สำหรับเขียนโปรแกรม (คอมพิวเตอร์ โน๊ตบุ๊ค) 

  4.อะเเดปเตอร์ที่ต่อกับ LED ส่องสว่าง

## ศึกษาข้อมูลเบื้องต้น
https://youtu.be/nFqoZT26U5k
## วิธีการทำการทดลอง
1. เสียบอะเเดปเตอร์ที่ต่อกับ LED ส่องสว่างกับUSB to serial

![image](https://user-images.githubusercontent.com/80879829/112281863-1c813400-8cb9-11eb-9e45-bf1b1847b0eb.png)

2.ต่อไมโครคอนโทรเลอร์ esp-01 เข้าไป

![image](https://user-images.githubusercontent.com/80879829/112282137-65d18380-8cb9-11eb-8419-656c98993818.png)

3.ดูหน้าตัวอย่างโปรแกรม platfromio.ini src ----> vi src/main.cpp 0twf
 อัพโหลดโปรเเกรมเข้าไปยังไมโครคอนโทรเลอร์โดยใช้คำสั่ง pio run -t upload 
 ![image](https://user-images.githubusercontent.com/80879829/112285914-6409bf00-8cbd-11eb-8aa3-92c3bb35debe.png)

พอรันเสร็จจะออกมาเเบบนี้

![image](https://user-images.githubusercontent.com/80879829/112286253-b5b24980-8cbd-11eb-99e0-56950091fd86.png)

เเล้วใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์

![image](https://user-images.githubusercontent.com/80879829/112286438-e72b1500-8cbd-11eb-9be7-aa8aa488fe23.png)

เเล้วลองเอาสายไฟสีขาวไปลองจิ้มไปที่เส้นสีดำ output จะ read เป็น 0 ไฟติด เเต่ถ้าปล่อยจะ read เป็น 1 ไฟดับ

![image](https://user-images.githubusercontent.com/80879829/112287263-c7e0b780-8cbe-11eb-868f-e16033034f82.png)

4.ต่อกับเซ็นเซอร์ ---> เเล้วก็เอา input ไปต่อกับเซนเซอร์

![image](https://user-images.githubusercontent.com/80879829/112287823-5a815680-8cbf-11eb-966d-c7c8d8a1fc9f.png)----->![image](https://user-images.githubusercontent.com/80879829/112288134-9f0cf200-8cbf-11eb-9c19-b85a6291fb1b.png)

5.ลองเอานิ้วปิด เปิด ตรงเซนเซอร์

![image](https://user-images.githubusercontent.com/80879829/112288441-ebf0c880-8cbf-11eb-8c22-94042bf013ab.png)
![image](https://user-images.githubusercontent.com/80879829/112289922-4fc7c100-8cc1-11eb-884b-f6a74578ff3e.png)

## การบันทึกผลการทดลอง
1.เมื่อเอานิ้วปิดเซนเซอร์ไฟจะดับ เเละread เป็น 1 ไฟดับ

![image](https://user-images.githubusercontent.com/80879829/112289091-91a43780-8cc0-11eb-906a-5f348b64c24b.png)

2.เมื่อเอานิ้วออกขากเซนเซอร์ไฟจะติดread เป็น 0 ไฟติด

![image](https://user-images.githubusercontent.com/80879829/112289177-a54f9e00-8cc0-11eb-997b-65938ac34318.png)


## อภิปรายการทดลอง
จากการทดลองจะเห็นได้ว่า ผลลัพธ์ที่ได้ออกมาเมื่อเอานิ้วมือปิดเซนเซอร์คือไฟ LED ไม่ติดแล้วค่าoutputที่ได้ออกมาก็เป็น read 1 

จากการทดลองจะเห็นได้ว่า ผลลัพธ์ที่ได้ออกมาเมื่อเอานิ้วออกจากเซนเซอร์คือไฟ LED ติดแล้วค่าoutputที่ได้ออกมาก็เป็น read 0
## คำถามหลังการทดลอง
Q..สามารถนำการทดลองไปปรับใช้กับอะไร
A..ไฟทางอัตโนมัติ
 
