![cf](LAB1.png)

1.อนุมัติ (Approve) คำขอใบรับรอง Smart Card

  -สำหรับผู้ใช้ tsutton และ mmallory

2.ปฏิเสธ (Deny) คำขอใบรับรอง Web Server

  -สำหรับเครื่อง CorpSrv12

3.เพิกถอนใบรับรอง (Revoke Certificate) ของผู้ใช้ bchan

  -เพราะทำ Smart Card หาย

  -เลือกเหตุผลการเพิกถอนเป็น Key Compromise

4.ยกเลิกการเพิกถอน (Unrevoke) ใบรับรองของ CorpDev3

![cf](LAB2.png)

1.เปิด Server Manager

2.ที่หน้า Dashboard จะมีงานเริ่มต้นให้ทำ ได้แก่

    -Configure this local server → ตั้งค่าเซิร์ฟเวอร์

    -Add roles and features → ติดตั้ง Roles / Services

    -Add other servers to manage → เพิ่มเครื่องอื่นให้จัดการ

    -Create a server group → จัดกลุ่มเซิร์ฟเวอร์

    -Connect this server to cloud services → เชื่อมต่อบริการคลาวด์

![cf](LAB3.png)

ขั้นตอนสั้น ๆ ที่เกี่ยวข้องกับหน้านี้คือ

1.คลิกเมนู Local Server บนแถบซ้าย

2.หน้านี้จะแสดงข้อมูลสำคัญของเซิร์ฟเวอร์ เช่น

    -ชื่อเครื่อง (CorpServer2)

    -โดเมนที่เข้าร่วม (CorpNet.local)

    -สถานะ Firewall / Remote Management

    -IPv4 / IPv6

    -ระบบปฏิบัติการและฮาร์ดแวร์

3.สามารถคลิกลิงก์แต่ละรายการเพื่อแก้ไขค่าการตั้งค่าได้

![cf](LAB4.png)

ขั้นตอนสั้น ๆ คือ

1.เปิดตัวช่วยติดตั้ง Roles / Features บน Windows Server

2.หน้านี้เป็นหน้าแนะนำก่อนเริ่มติดตั้ง แจ้งว่า

    -บัญชี Administrator ต้องตั้งรหัสผ่าน

    -การตั้งค่าเครือข่ายต้องถูกต้อง

    -ควรอัปเดต Windows ให้เป็นเวอร์ชันล่าสุด

3.เมื่อพร้อมแล้ว ให้กด Next เพื่อไปขั้นตอนถัดไป

![cf](LAB5.png)

คำอธิบายขั้นตอนแบบสั้น ๆ:

1.เลือกประเภทการติดตั้ง

ตัวเลือกที่เลือกอยู่คือ

    ✅ Role-based or feature-based installation
    (ใช้สำหรับติดตั้ง Roles หรือ Features บนเครื่องเซิร์ฟเวอร์นี้)

2.อีกตัวเลือกคือ

    ⭕ Remote Desktop Services installation
    (ใช้เมื่อต้องติดตั้งระบบ Remote Desktop VDI — ซึ่งไม่ใช้ในงานนี้)

3.หลังเลือกแล้วให้กด Next เพื่อไปขั้นตอนถัดไป

![cf](LAB6.png)

ขั้นตอนการติดตั้ง Role หรือ Feature ของ Windows Server สรุปขั้นตอนสั้นๆ ได้ดังนี้

1.เลือกรูปแบบการติดตั้ง: ติ๊กเลือก "Select a server from the server pool" 

เพื่อระบุว่าจะติดตั้งลงบนเครื่องเซิร์ฟเวอร์โดยตรง (ไม่ใช่ไฟล์ Hard Disk เสมือน)

2.เลือกเซิร์ฟเวอร์เป้าหมาย: คลิกเลือกชื่อเซิร์ฟเวอร์จากรายการในช่อง Server Pool 

(ในภาพคือเครื่อง CorpServer2.CorpNet.local)

3.ไปต่อ: เมื่อเลือกเครื่องเสร็จแล้ว ให้กดปุ่ม Next เพื่อไปเลือก Role หรือ Feature ที่ต้องการติดตั้งในหน้าถัดไป

![cf](LAB7.png)

สรุปสั้นๆ ดังนี้

1.เลือกบทบาท (Roles): ติ๊กถูกหน้าชื่อบริการที่ต้องการติดตั้งลงในเซิร์ฟเวอร์ 

(เช่น DNS Server, DHCP Server หรือ Web Server)

2.ตรวจสอบสถานะ: สังเกตในรายการจะเห็นบางรายการขึ้นว่า (Installed) หมายถึงติดตั้งไปแล้ว หรือบางรายการมีแถบสีดำ 

(เช่น File and Storage Services) หมายถึงมีการติดตั้งบางส่วนไว้แล้ว

3.ดูรายละเอียด: เมื่อคลิกที่ชื่อ Role ด้านขวาจะแสดงคำอธิบาย (Description) ว่าหน้าที่นั้นใช้ทำอะไร

4.ไปต่อ: เมื่อเลือก Role ที่ต้องการครบแล้ว ให้กดปุ่ม Next เพื่อไปตั้งค่า Feature ในหน้าถัดไป

![cf](LAB8.png)

ภาพทั้งสองแสดงขั้นตอนต่อเนื่องในการปรับแต่งความสามารถของ Windows Server ผ่าน Add Roles and Features Wizard 

สรุปสั้นๆ ได้ดังนี้

1.ภาพ Select server roles (LAB7.png)

ขั้นตอนนี้คือการเลือก "หน้าที่หลัก" (Roles) ให้กับเซิร์ฟเวอร์

    เลือกบทบาท: ติ๊กเลือกบริการหลักที่ต้องการ เช่น DNS Server หรือ DHCP Server

    สถานะการติดตั้ง: รายการที่มีเครื่องหมายถูกและระบุว่า (Installed) คือติดตั้งไปแล้ว เช่น Hyper-V และ 
    
    Print and Document Services

2.ภาพ Select features (LAB8.png)

ขั้นตอนนี้คือการเลือก "เครื่องมือเสริม" (Features) เพื่อสนับสนุนการทำงานของ Roles หรือตัวระบบปฏิบัติการเอง

    เลือกฟีเจอร์: ติ๊กเลือกโปรแกรมเสริมหรือความสามารถเฉพาะทาง เช่น .NET Framework หรือ BitLocker

    สถานะปัจจุบัน: ในภาพมีการติดตั้ง Group Policy Management ไว้เรียบร้อยแล้ว

![cf](LAB9.png)

ภาพเหล่านี้แสดงขั้นตอนการกำหนดค่าในหน้าต่าง Add Roles and Features Wizard ของ Windows Server สรุปสั้นๆ ดังนี้

1. เลือกบทบาท (Select server roles - LAB7.png)

       เป็นขั้นตอนการเลือก "หน้าที่หลัก" ให้กับเซิร์ฟเวอร์

       ในภาพมีการติดตั้งบทบาท Hyper-V และ Print and Document Services ไว้แล้ว

       บทบาท Remote Access และ File and Storage Services มีการติดตั้งไว้แล้วบางส่วน

2.เลือกคุณสมบัติเสริม (Select features - LAB8.png)

    เป็นการเลือก "ความสามารถเสริม" เพื่อสนับสนุนการทำงานของระบบ

    ในภาพมีการติดตั้ง Group Policy Management ไว้เรียบร้อยแล้ว

    มีการติดตั้งคุณสมบัติบางส่วนของ .NET Framework 4.5 ไว้แล้ว (2 จาก 7 รายการ)

3. ข้อมูล Remote Access (LAB9.png)

       เป็นหน้าแสดงรายละเอียดของบทบาท Remote Access ที่ถูกเลือกไว้

       อธิบายว่าบริการนี้รวม DirectAccess และ VPN เข้าด้วยกัน เพื่อให้เครื่องลูกข่ายเชื่อมต่อเข้าเครือข่ายองค์กรได้จากระยะไกล

       ให้กดปุ่ม Next เพื่อเข้าไปเลือก Role Services เฉพาะเจาะจงในหน้าถัดไป

![cf](LAB10.png)


