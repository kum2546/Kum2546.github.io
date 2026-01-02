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
