## การทดลองที่ 6 เรื่อง การเขียนโปรแกรมสร้างไวไฟแอคเซสพอยต์ (Wifi AP)
## วัตถุประสงค์
 1.เพื่อศึกษาวิธีการเขียนโปรแกรมและcodeของการเขียนการทดลอง 
 
 2.เรียนรู้การใช้คำสั่งต่างๆของการเขียนโปรแกรม
 
 3.เพื่อศึกษาการใช้ platfrom IO
 
 4.หลักการสร้างตัวปล่อยสัญญาณ
## อุปกรณ์ที่ใช้
   1.ไมโครคอนโทรเลอร์ esp-01
  
  2.USB to serial
  
  3.อุปกรณ์ที่ใช้สำหรับเขียนโปรแกรม (คอมพิวเตอร์ โน๊ตบุ๊ค) 
  4.มือถือ ( ใช้สำหรับ ค้นหา wifi )

## ศึกษาข้อมูลเบื้องต้น
https://youtu.be/T26DVHePlTs

## วิธีการทำการทดลอง
1.เสียบไมโครคอนโทเลอร์เข้ากับ USB to serial
  
  ![image](https://user-images.githubusercontent.com/80879829/112275297-0cb22180-8cb2-11eb-9a5b-5272312e3d28.png)
  
2.ดูหน้าตัวอย่างโปรแกรม platfromio.ini src ----> vi src/main.cpp 0twf
  ![image](https://user-images.githubusercontent.com/80879829/112293594-e3e75780-8cc4-11eb-80e8-8a15bf10b5ea.png)
![image](https://user-images.githubusercontent.com/80879829/112293658-f366a080-8cc4-11eb-9fd0-cbdcf60c7e6a.png)

3. ใช้คำสั่ง pio run -t upload เเล้วกดรีเซ็ต

![image](https://user-images.githubusercontent.com/80879829/112293846-2b6de380-8cc5-11eb-8361-1fd6f375fd3e.png)
4.ใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์ เเละใช้มือถือค้นหา wifi ที่เราสร้าง

![image](https://user-images.githubusercontent.com/80879829/112294047-5f490900-8cc5-11eb-8220-b83642433914.png)

## การบันทึกผลการทดลอง
![image](https://user-images.githubusercontent.com/80879829/112294144-6a039e00-8cc5-11eb-8f12-831a6096c010.png)

## อภิปรายผลการทดลอง
จากการทดลองจะเห็นว่าเมื่อเราทราบตัวปล่อย WiFI ของเราเองจากโปรแกรมที่เรารันขึ้นมา เอามือถือหรือว่า notebook มาค้นหาก็จะปรากฏชื่อ WiFi ที่เราสร้างเองเราก็สามารถใช้ได้โดยการกรอกpasswordที่เราระบุไว้
## คำถามหลังการทดลอง
Q..สามารถเชื่อม wifi ได้มากสุดเท่าไร

A..ขึ้นอยู่กับความสามารถของesp-01
