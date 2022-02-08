# สวัสดีครับ ผม นาย ประกาศิต ลีพุด เลขทะเบียน 6310680399
โดยจะมาสรุปเนื้อหาต่างๆ ในงานที่มอบหมายดังนี้ครับ
# MARKDOWN
# สรุปเนื้อหาเกี่ยวกับ Microcontroller ESP-01
1. digital คือ การนำสัญญาณไฟฟ้ามาแทนด้วยตัวเลข ซึ่งเป็นเลขฐาน 2 มีแค่ 0กับ1 และยังสามารถนำค่าไปแสดงตัวเลขและตัวอักษรได้
2. voltage คือ ความต่างศักย์ของไฟฟ้าจากจุดสองจุด มี 2 ประเภทคือ แรงดัน AC และ แรงดัน DC ยกตัวอย่างเช่น แบตเตอรี่
3. computer คือ อุปกรณ์ที่ทำงานด้วยระบบอิเล็กทรอนิกส์ ซึ่งสามารถทำงานได้อัตโนมัติด้วยความเร็วที่สูง
4. internet คือ สัญญาณที่เชื่อมต่อกับอุปกรณ์ต่างๆ โดยจะใช้ในการสื่อสาร หรืออื่นๆ
5. program lag คือ ภาษาที่นำมาใช้สำหรับคอมพิวเตอร์โดยมีการพัฒนาตลอดเรื่อยๆ
6. platformio คือ การพัฒนาโปรแกรมแบบเปิด โดยใช้โปรแกรมการเขียนแบบเดียวซึ่งสามารถเขียนลง Microcontroller ได้หลายแบบ
7. iotset1 คือ ตัวรันคำสั่งบราวเซอร์ที่เราต้องการ
# สรุปการทดลอง ESP-01 การทดลอง
1.run example1 โดยจะเริ่มเขียนตัวโปรแกรมเข้าไปใน microcontroller โดยจะมี setup และ loop โดยในส่วน loop จะเพิ่มตัวแปล cnt โดย loop หน่วงเวลา 1 วินาที ซึ่งการแสดงผลจะเพิ่มค่า cnt ไปทีละ1 โดยเมื่อโปรแกรมแสดงเลขคู่จะเท่ากับ off(ไฟดับ) แสดงเลขคี่เท่ากับ on(ไฟสว่าง) โดยตัวของโปรแกรมจะมีค่า delay 0.5 วินาที
2.run example2 เป็นการเขียนโปรแกรมเข้าไปในตัว microconttoller เพื่อค้าหา wifi โดยใช้คำสั่ง pio device monitor โดยการแสดงผลจะแสดง wifi ที่หาเจอ
3.run example3 เป็นโปรเขียนโปรแกรมเข้าไปใน microcontroller โดยให้ต่อ port 0 เป็น input port 1 เป็น output ซึ่งจากโปรแกรมจะแสดงการนับ ซึ่งถ้าค่าของ cnt เป็นเลขคู่จะเท่ากับoff(หลอดไม่สว่าง) ถ้าเป็นเลขคี่จะเท่ากับ(on) และจะมีการ delay ทุกๆ 0.5 วินาที
4.run relay นำตัว microcontroller ที่เขียนโปรแกรมเรียบร้อยแล้ว มาต่อเชื่อกับตัวของ relay โดยจะให้เป็นตัวเปิดปิดสวิตซ์ของตัว relay 
5.run example3 setup ตัวโปรแกรม โดยให้ port0 เป็น input port2 เป็น output โดยตัวโปรแกรมจะอ่านค่าจาก port0 ซึ่งถ้าแสดงค้าเป็น 1 จะหมายถึง(off) แต่เมื่อกดปุุ่มสีดำ จะทำให้ port0 มีค่าเป็น 1 จะทำให้หลอดไฟสว่าง และเมื่อนำมาต่อกับ sensor ไปต่อถ้ามีแสง การอ่านค่าออกมาจะเป็น 0 ทำให้หลอดไฟสว่าง แต่ถ้าไม่มีแสง การอ่านค่าออกมาจะเป็น 1 ซึ่งทำให้หลอดไฟไม่สว่าง
6.run wifi เป็นการเขียนโปรแกรมลงไปในตัว microcontroller ในการเชื่อตัวของ wifi โดยทดสอบด้วยการเข้า web
7.run wiri AP เป็นการสร้าง wifi ของตัวเอง ให้คนอื่นมาเชื่อมต่อ โดยจะมีการกำหนด IPAdress โดยจะทดสอบโดยหา หาอุปกรณ์คอมพิวเตอร์หรือโทรศัพท์มาค้นหา wifi
