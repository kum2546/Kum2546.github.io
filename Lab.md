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


