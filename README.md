<p align="center">
  <img src="labExpressNodeJS/uploads/img/logo.png" alt="AssetFlow Logo" width="240" />
</p>

<h1 align="center">📦 AssetFlow - ระบบยืม-คืนอุปกรณ์ (Equipment Borrow & Return System)</h1>

<p align="center">
  <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-v18+-68a063?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" /></a>
  <a href="https://expressjs.com/"><img src="https://img.shields.io/badge/Express.js-4.16+-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js" /></a>
  <a href="https://www.mongodb.com/"><img src="https://img.shields.io/badge/MongoDB-Atlas%20%2F%20Mongoose-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" /></a>
  <a href="https://getbootstrap.com/"><img src="https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" /></a>
  <a href="https://ejs.co/"><img src="https://img.shields.io/badge/Template-EJS-B4CA65?style=for-the-badge&logo=ejs&logoColor=black" alt="EJS" /></a>
</p>

> **AssetFlow** เป็นเว็บแอปพลิเคชันสำหรับบริหารจัดการการยืม-คืนอุปกรณ์ ครุภัณฑ์ และระบบแจ้งซ่อมบำรุงแบบครบวงจร พัฒนาขึ้นเพื่อช่วยให้องค์กรหรือสถานศึกษาควบคุม ตรวจสอบสถานะ และติดตามอุปกรณ์ได้อย่างมีประสิทธิภาพ พร้อมระบบแจ้งเตือนผ่านอีเมลแบบอัตโนมัติ

---

## 🖼️ ภาพตัวอย่างต้นแบบและระบบ (System Prototype & Preview)

### ✨ ภาพรวมระบบ (Landing Page & Overview)
<div align="center">
  <img src="labExpressNodeJS/uploads/img/index.png" alt="AssetFlow Landing Page & Prototype" width="85%" style="border-radius: 12px; box-shadow: 0 4px 14px rgba(0,0,0,0.15);" />
  <p><i>หน้า Landing Page สำหรับแนะนำระบบ สถิติการยืม-คืน และภาพรวมการทำงาน</i></p>
</div>

<br />

### 📱 1. หน้าจอฝั่งผู้ใช้งานทั่วไป (User Interfaces)

| ฟังก์ชันและหน้าจอ | ภาพตัวอย่างต้นแบบ (UI Prototype) |
| :--- | :--- |
| **หน้าแดชบอร์ด (User Dashboard)**<br>แสดงสถานะการยืม ประวัติ และทางลัดเมนู | <img src="AssetFlow/User - แดชบอร์ด.png" width="460" alt="User Dashboard" /> |
| **ค้นหาและเลือกอุปกรณ์ (Browse & Search)**<br>ค้นหาตามชื่อ และกรองตามหมวดหมู่ | <img src="AssetFlow/User - ค้นหาอุปกรณ์.png" width="460" alt="Browse Equipments" /> |
| **ยื่นคำขอยืมอุปกรณ์ (Borrow Request)**<br>ระบุวันที่ต้องการคืน และเหตุผลการยืม | <img src="AssetFlow/User - ส่งคำขอยืมอุปกรณ์.png" width="460" alt="Submit Borrow Request" /> |
| **รายละเอียดคำขอยืม (Request Details)**<br>ตรวจสอบข้อมูลคำขอ และสถานะการอนุมัติ | <img src="AssetFlow/User - รายละเอียดคำขอยืมอุปกรณ์.png" width="460" alt="Borrow Request Details" /> |
| **ประวัติการยืม-คืน (Borrow History)**<br>ติดตามสถานะรายการยืมทั้งหมดของผู้ใช้ | <img src="AssetFlow/User - รายการยืมและคืนอุปกรณ์.png" width="460" alt="Borrow History" /> |
| **การส่งคืนอุปกรณ์ (Return Equipment)**<br>ขั้นตอนการแจ้งส่งคืนอุปกรณ์เมื่อครบกำหนด | <img src="AssetFlow/User - คืนอุปกรณ์.png" width="460" alt="Return Equipment" /> |
| **แจ้งซ่อมอุปกรณ์ชำรุด (Repair Request)**<br>ระบุอาการเสียและส่งเรื่องให้ช่างประเมิน | <img src="AssetFlow/User - แจ้งซ่อม.png" width="460" alt="Report Broken Equipment" /> |
| **ติดตามรายการแจ้งซ่อม (Repair History)**<br>เช็คสถานะการซ่อมและความเห็นจากแอดมิน | <img src="AssetFlow/User - รายการแจ้งซ่อม.png" width="460" alt="Repair Request List" /> |
| **การแจ้งเตือน (Notifications)**<br>กล่องข้อความแจ้งเตือนสถานะต่างๆ | <img src="AssetFlow/User - การแจ้งเตือน.png" width="460" alt="User Notifications" /> |
| **การตั้งค่าโปรไฟล์ (Profile Settings)**<br>แก้ไขข้อมูลส่วนตัว เปลี่ยนรหัสผ่าน และรูปโปรไฟล์ | <img src="AssetFlow/User - การตั้งค่า.png" width="460" alt="User Settings" /> |

<br />

### 🛡️ 2. หน้าจอฝั่งผู้ดูแลระบบ (Admin Interfaces)

| ฟังก์ชันและหน้าจอ | ภาพตัวอย่างต้นแบบ (UI Prototype) |
| :--- | :--- |
| **จัดการคำขอยืม (Borrow Approval)**<br>อนุมัติ หรือ ปฏิเสธคำขอ พร้อมแจ้งเตือนผ่าน Email | <img src="AssetFlow/รายการคำขอยืมอุปกรณ์.png" width="460" alt="Admin Borrow Management" /> |
| **รายละเอียดคำขอยืมและสถานะ**<br>ดูข้อมูลผู้ขอยืม วันที่คืน และบันทึกข้อความ | <img src="AssetFlow/รายการคำขอยืมอุปกรณ์-2.png" width="460" alt="Admin Borrow Details" /> |
| **จัดการรายการอุปกรณ์ (Equipment List)**<br>คลังข้อมูลอุปกรณ์ทั้งหมดในระบบ | <img src="AssetFlow/รายการอุปกรณ์.png" width="460" alt="Admin Equipment List" /> |
| **รายละเอียดอุปกรณ์ (Equipment Details)**<br>ดูสเปก ตำแหน่งที่ตั้ง และประวัติของอุปกรณ์ | <img src="AssetFlow/รายละเอียดอุปกรณ์.png" width="460" alt="Admin Equipment Details" /> |
| **เพิ่มอุปกรณ์ใหม่ (Add Equipment)**<br>ฟอร์มลงทะเบียนอุปกรณ์ใหม่พร้อมอัปโหลดรูป | <img src="AssetFlow/เพิ่มอุปกรณ์.png" width="460" alt="Add Equipment Form" /> |
| **แก้ไขข้อมูลอุปกรณ์ (Edit Equipment)**<br>ปรับปรุงรายละเอียดและอัปเดตสถานะอุปกรณ์ | <img src="AssetFlow/แก้ไขอุปกรณ์.png" width="460" alt="Edit Equipment" /> |
| **ลบอุปกรณ์ / ถังขยะ (Soft Delete)**<br>ระบบลบอย่างปลอดภัย สามารถกู้คืนได้ | <img src="AssetFlow/ลบอุปกรณ์.png" width="460" alt="Delete Equipment" /> |
| **จัดการงานแจ้งซ่อม (Repair Management)**<br>อัปเดตสถานะงานซ่อม และระบุ Admin Comment | <img src="AssetFlow/รายการแจ้งซ่อม.png" width="460" alt="Admin Repair Management" /> |

---

## 📑 สารบัญ (Table of Contents)

1. [ภาพตัวอย่างต้นแบบและระบบ (System Prototype & Preview)](#️-ภาพตัวอย่างต้นแบบและระบบ-system-prototype--preview)
2. [ฟังก์ชันเด่นของระบบ (Features)](#-ฟังก์ชันเด่นของระบบ-features)
3. [ผังการทำงานของระบบ (System Workflow)](#-ผังการทำงานของระบบ-system-workflow)
4. [เทคโนโลยีที่ใช้พัฒนา (Tech Stack)](#-เทคโนโลยีที่ใช้พัฒนา-tech-stack)
5. [โครงสร้างฐานข้อมูล (Database Schema)](#-โครงสร้างฐานข้อมูล-database-schema)
6. [โครงสร้างโฟลเดอร์โปรเจกต์ (Project Structure)](#-โครงสร้างโฟลเดอร์โปรเจกต์-project-structure)
7. [ขั้นตอนการติดตั้งและเริ่มใช้งาน (Getting Started)](#-ขั้นตอนการติดตั้งและเริ่มใช้งาน-getting-started)
8. [การตั้งค่า Environment Variables](#-การตั้งค่า-environment-variables)
9. [บัญชีผู้ใช้งานเริ่มต้นและการทดสอบ](#-บัญชีผู้ใช้งานเริ่มต้นและการทดสอบ)
10. [ผู้จัดทำและข้อมูลวิชา](#-ข้อมูลรายวิชาและผู้จัดทำ)

---

## 🌟 ฟังก์ชันเด่นของระบบ (Features)

### 👤 1. ส่วนของผู้ใช้งานทั่วไป (User)
* **Authentication & Session:** สมัครสมาชิก, เข้าสู่ระบบ, จดจำ Session ผู้ใช้ และเปลี่ยนรหัสผ่านได้อย่างปลอดภัย (เข้ารหัสด้วย `bcryptjs`)
* **Equipment Browsing & Search:** ดูรายการอุปกรณ์ทั้งหมดในระบบ ค้นหาตามชื่อ และกรองตามหมวดหมู่ พร้อมแสดงสถานะความพร้อมใช้งาน (Available / Unavailable / Broken)
* **Borrow Request:** ยื่นคำขอยืมอุปกรณ์ โดยสามารถระบุวันที่ต้องการคืนและเหตุผลหรือหมายเหตุประกอบการยืมได้
* **Borrow History & Tracking:** ติดตามสถานะคำขอยืมของตนเองแบบเรียลไทม์:
  * `waiting` (รอการอนุมัติ)
  * `borrowed` (กำลังยืม / อนุมัติแล้ว)
  * `waitingForReturn` (ส่งคืนแล้ว / รอแอดมินยืนยัน)
  * `returned` (คืนสำเร็จเรียบร้อย)
  * `rejected` (คำขอถูกปฏิเสธ)
  * `late` (เกินกำหนดคืน)
  * `lost` (สูญหาย)
* **Repair Request (แจ้งซ่อม):** แจ้งอุปกรณ์ชำรุดเสียหาย พร้อมระบุรายละเอียดปัญหา และติดตามความคืบหน้าการซ่อมได้
* **Profile Management:** แก้ไขข้อมูลส่วนบุคคล และอัปโหลดรูปโปรไฟล์ (รองรับไฟล์รูปภาพผ่าน Multer)

---

### 🛡️ 2. ส่วนของผู้ดูแลระบบ (Admin)
* **Dashboard:** หน้าสรุปภาพรวมและสถิติต่างๆ เช่น จำนวนผู้ใช้งานทั้งหมด จำนวนอุปกรณ์ และจำนวนรายการยืม-คืนในระบบ
* **Borrow Approval System:** ตรวจสอบคำขอยืม อนุมัติ (Approve) หรือปฏิเสธ (Reject) พร้อมบันทึกเหตุผล
* **Automated Email Notification:** ส่งอีเมลแจ้งผลการอนุมัติ/ปฏิเสธคำขอยืมไปยังอีเมลของผู้ใช้โดยตรงอัตโนมัติผ่าน EmailJS API
* **Return Management:** บันทึกการรับคืนอุปกรณ์ ตรวจสอบสภาพ และปรับสถานะอุปกรณ์คืนสู่คลัง
* **Equipment Management (CRUD):** 
  * เพิ่มรายการอุปกรณ์ใหม่ พร้อมอัปโหลดรูปภาพ
  * แก้ไขข้อมูลและสถานะของอุปกรณ์
  * ระบบ **Soft Delete** (ลบแบบปลอดภัย มีประวัติถังขยะ สามารถกู้คืนหรือลบถาวรได้)
* **Category Management:** เพิ่ม/ลบ/แก้ไข หมวดหมู่อุปกรณ์
* **Repair Request Management:** จัดการคำขอแจ้งซ่อม ปรับสถานะ (`pending`, `in_progress`, `completed`, `rejected`) พร้อมระบุความเห็นของแอดมิน (Admin Comment)
* **User Management:** เพิ่ม ลบ แก้ไขข้อมูลผู้ใช้ และกำหนดสิทธิ์การเข้าถึง (`admin` / `user`) รวมถึงแผนก/สังกัด

---

## 🔄 ผังการทำงานของระบบ (System Workflow)

### 1. กระบวนการยืม - คืนอุปกรณ์ (Borrow & Return Lifecycle)

```mermaid
graph TD
    A[ผู้ใช้ยื่นคำขอยืมอุปกรณ์] --> B{แอดมินตรวจสอบคำขอ}
    B -- อนุมัติ (Approve) --> C[ส่งอีเมลแจ้งอนุมัติไปยังผู้ใช้]
    C --> D[สถานะ: borrowed / ผู้ใช้รับอุปกรณ์]
    B -- ปฏิเสธ (Reject) --> E[ส่งอีเมลแจ้งเหตุผลไปยังผู้ใช้]
    E --> F[สถานะ: rejected]
    D --> G[ผู้ใช้นำอุปกรณ์มาส่งคืน]
    G --> H[แอดมินตรวจสอบสภาพอุปกรณ์]
    H -- ครบถ้วนสมบูรณ์ --> I[สถานะ: returned / อุปกรณ์กลับสู่คลัง]
    H -- ชำรุด/เกินกำหนด/สูญหาย --> J[บันทึกสถานะ: late / lost / แจ้งซ่อม]
```

### 2. กระบวนการแจ้งซ่อมอุปกรณ์ (Repair Request Lifecycle)

```mermaid
graph TD
    A[ผู้ใช้แจ้งอุปกรณ์ชำรุด] --> B[สถานะ: pending รอการตรวจสอบ]
    B --> C{แอดมินประเมินงานซ่อม}
    C -- ดำเนินการซ่อม --> D[สถานะ: in_progress กำลังซ่อมบำรุง]
    C -- ปฏิเสธ --> E[สถานะ: rejected พร้อมแจ้งเหตุผล]
    D --> F[ซ่อมบำรุงเสร็จสิ้น]
    F --> G[สถานะ: completed / อุปกรณ์พร้อมใช้งาน]
```

---

## 🛠️ เทคโนโลยีที่ใช้พัฒนา (Tech Stack)

| ส่วนประกอบ | รายละเอียดเทคโนโลยี |
| :--- | :--- |
| **Runtime & Framework** | [Node.js](https://nodejs.org/) (v18+) & [Express.js](https://expressjs.com/) (v4.x) |
| **Database & ODM** | [MongoDB](https://www.mongodb.com/) (Atlas Cloud Database) & [Mongoose](https://mongoosejs.com/) (v8.x) |
| **View Engine & UI** | [EJS](https://ejs.co/) (Embedded JavaScript), [express-ejs-layouts](https://www.npmjs.com/package/express-ejs-layouts), [Bootstrap 5](https://getbootstrap.com/), [SweetAlert2](https://sweetalert2.github.io/), Google Font (Kanit) |
| **Authentication & Security** | [Express-Session](https://www.npmjs.com/package/express-session), [Bcryptjs](https://www.npmjs.com/package/bcryptjs), [Cookie-Parser](https://www.npmjs.com/package/cookie-parser) |
| **File Uploads** | [Multer](https://www.npmjs.com/package/multer) (จัดการการอัปโหลดไฟล์รูปภาพอุปกรณ์และรูปโปรไฟล์) |
| **Notification Services** | [EmailJS](https://www.emailjs.com/) / [Resend](https://resend.com/) API สำหรับส่งอีเมลแจ้งเตือน |
| **HTTP Client & Logger** | [Axios](https://axios-http.com/), [Morgan](https://www.npmjs.com/package/morgan) |

---

## 🗄️ โครงสร้างฐานข้อมูล (Database Schema)

ระบบใช้งานร่วมกับ MongoDB โดยมีคอลเลกชันหลักดังนี้:

1. **`users`**: จัดเก็บข้อมูลผู้ใช้งาน
   * `fname`, `lname`, `email`, `password` (hashed), `userProfile`, `userRole` (`admin` / `user`), `department`
2. **`equipments`**: จัดเก็บรายการอุปกรณ์
   * `name`, `category_id`, `description`, `status` (`available` / `unavailable` / `broken`), `image`, `location`, `deleted_at`
3. **`categories`**: จัดเก็บหมวดหมู่ของอุปกรณ์
   * `name`, `deleted_at`
4. **`departments`**: จัดเก็บแผนกหรือฝ่ายสังกัด
   * `name`, `deleted_at`
5. **`borrows`**: จัดเก็บประวัติและรายการยืม-คืน
   * `user_id`, `equipment_id`, `return_date`, `actual_return_date`, `note`, `status` (`waiting`, `borrowed`, `waitingForReturn`, `returned`, `rejected`, `late`, `lost`)
6. **`repair_requests`**: จัดเก็บข้อมูลคำขอแจ้งซ่อม
   * `user_id`, `equipment_id`, `issue_description`, `admin_comment`, `completion_date`, `status` (`pending`, `in_progress`, `completed`, `rejected`)

---

## 📁 โครงสร้างโฟลเดอร์โปรเจกต์ (Project Structure)

```text
project_CP363205_EquipmentBorrow-ReturnSystem/
├── README.md                          # เอกสารคู่มือโปรเจกต์
├── AssetFlow/                         # โฟลเดอร์จัดเก็บภาพต้นแบบ UI Prototype & Screenshots
│   ├── User - *.png                   # ภาพตัวอย่างหน้าจอฝั่ง User
│   └── *.png                          # ภาพตัวอย่างหน้าจอฝั่ง Admin
└── labExpressNodeJS/                  # ซอร์สโค้ดหลักของระบบ
    ├── app.js                         # จุดเริ่มต้นของ Express Application และการตั้งค่า Middleware
    ├── package.json                   # การประกาศ Dependencies และสคริปต์สั่งรัน
    ├── .env.example                   # ไฟล์ตัวอย่างสำหรับการตั้งค่า Environment Variables
    ├── bin/
    │   └── www                        # ไฟล์สำหรับเริ่ม HTTP Server
    ├── middleware/
    │   └── auth.js                    # Middleware ตรวจสอบสิทธิ์ (isAuthenticated, isAdmin, isUser)
    ├── models/                        # Mongoose Schemas & Data Models
    │   ├── Borrow.js                  # Model รายการยืม-คืน
    │   ├── Category.js                # Model หมวดหมู่อุปกรณ์
    │   ├── Department.js              # Model แผนก
    │   ├── listEquipment.js           # Model อุปกรณ์
    │   ├── Reqair_requests.js         # Model คำขอแจ้งซ่อม
    │   └── User.js                    # Model ผู้ใช้งาน
    ├── public/                        # Static Assets (Images, Icons, Custom Styles, Client Scripts)
    ├── routes/                        # API & Page Routing
    │   ├── admin.js                   # Route สำหรับการจัดการของผู้ดูแลระบบ (Admin)
    │   ├── index.js                   # Route หน้าแรก, เข้าสู่ระบบ, สมัครสมาชิก
    │   └── users.js                   # Route สำหรับผู้ใช้งานทั่วไป (User)
    ├── uploads/                       # โฟลเดอร์เก็บไฟล์ภาพที่อัปโหลด (Avatar, Equipment images)
    │   └── img/                       # รูปภาพต้นแบบ, โลโก้ และภาพประกอบหน้าเว็บ
    └── views/                         # EJS Templates สำหรับแสดงผลหน้าเว็บ
        ├── layouts/                   # Master Layouts (index, auth, navadmin, navuser)
        ├── login.ejs                  # หน้าเข้าสู่ระบบ
        ├── register.ejs               # หน้าสมัครสมาชิก
        ├── equipmentAdmin.ejs         # หน้าจัดการอุปกรณ์ (Admin)
        ├── Borrowequipment.ejs        # หน้าอนุมัติการยืม (Admin)
        ├── returnEquipmentAdmin.ejs   # หน้าบันทึกรับคืน (Admin)
        ├── reqair_requestsAdmin.ejs   # หน้าจัดการแจ้งซ่อม (Admin)
        ├── manage_user.ejs            # หน้าจัดการสมาชิก (Admin)
        ├── indexUser.ejs              # หน้าหลักของผู้ใช้
        └── userBorrowHistory.ejs      # หน้าประวัติการยืม-คืนของผู้ใช้
```

---

## 🚀 ขั้นตอนการติดตั้งและเริ่มใช้งาน (Getting Started)

### 1. ความต้องการของระบบ (Prerequisites)
* [Node.js](https://nodejs.org/) เวอร์ชั่น 18.0.0 ขึ้นไป
* [npm](https://www.npmjs.com/) หรือ [yarn](https://yarnpkg.com/)
* บัญชีหรือ Connection URI ของ [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) (หรือ Local MongoDB)

### 2. ดาวน์โหลดโปรเจกต์ (Clone Repository)
```bash
git clone https://github.com/chaiyawat19/project_CP363205_EquipmentBorrow-ReturnSystem.git
cd project_CP363205_EquipmentBorrow-ReturnSystem/labExpressNodeJS
```

### 3. ติดตั้ง Dependencies
```bash
npm install
```

### 4. ตั้งค่า Environment Variables
คัดลอกไฟล์ `.env.example` ไปเป็น `.env` และกรอกข้อมูลการเชื่อมต่อจริง:
```bash
cp .env.example .env
```
*(สำหรับ Windows PowerShell: `copy .env.example .env`)*

### 5. เริ่มต้นรันเซิร์ฟเวอร์ (Run Server)
```bash
npm start
```
หรือรันผ่าน Node โดยตรง:
```bash
node app.js
```

### 6. เข้าใช้งานผ่าน Web Browser
เปิดเบราว์เซอร์แล้วไปที่:
```text
http://localhost:3001
```

---

## ⚙️ การตั้งค่า Environment Variables

สร้างไฟล์ `.env` ไว้ที่โฟลเดอร์ `labExpressNodeJS/` โดยกำหนดค่าตัวแปรดังต่อไปนี้:

```env
# MongoDB Connection URI
MONGODB_URI=mongodb+srv://<username>:<password>@cluster0.xxxxx.mongodb.net/<dbname>

# Port สำหรับ Server (Default: 3001)
PORT=3001

# Resend API Key (ถ้าต้องการใช้งานส่งอีเมลผ่าน Resend)
RESEND_API_KEY=re_xxxxxxxxxxxxxxxxxxxx

# EmailJS Service Credentials (สำหรับการส่งอีเมลแจ้งเตือนผลการอนุมัติ)
EMAILJS_SERVICE_ID=service_xxxxxxx
EMAILJS_PUBLIC_KEY=xxxxxxxxx
EMAILJS_PRIVATE_KEY=xxxxxxxxx
EMAILJS_TEMPLATE_ID_APPROVE=template_xxxxxxx
EMAILJS_TEMPLATE_ID_REJECT=template_xxxxxxx
```

---

## 🔑 บัญชีผู้ใช้งานเริ่มต้นและการทดสอบ

ระบบมีการแบ่งสิทธิ์ชัดเจนผ่าน Middleware:
* **Admin (ผู้ดูแลระบบ):** เข้าถึง URL `/admin/*` จัดการระบบทั้งหมด
* **User (ผู้ใช้งานทั่วไป):** เข้าถึง URL `/users/*` เพื่อค้นหาอุปกรณ์ ยื่นขอยืม และแจ้งซ่อม

> 💡 **คำแนะนำ:** เมื่อเริ่มต้นใช้งานครั้งแรก สามารถลงทะเบียนผ่านหน้า `/register` แล้วเข้าไปปรับเปลี่ยนค่า `userRole` เป็น `'admin'` โดยตรงผ่านฐานข้อมูล MongoDB Atlas หรือผ่านแอดมินที่มีอยู่แล้วในระบบ

---

## 🎓 ข้อมูลรายวิชาและผู้จัดทำ

* **รหัสวิชา:** CP363205 / SC363205
* **ชื่อโปรเจกต์:** AssetFlow - Equipment Borrow & Return System
* **GitHub Repository:** [chaiyawat19/project_CP363205_EquipmentBorrow-ReturnSystem](https://github.com/chaiyawat19/project_CP363205_EquipmentBorrow-ReturnSystem)
