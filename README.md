# Node-Mongo
MongoDB Atlas และการเชื่อมต่อกับ NodeJS ทำ CRUD API

โปรเจกต์ตัวอย่างการพัฒนา REST API ด้วย **Express** และ **Mongoose** เพื่อเชื่อมต่อไปยังฐานข้อมูลคลาวด์ **MongoDB Atlas** รองรับการทำงาน CRUD (Create, Read, Update, Delete) สำหรับข้อมูลสินค้า (Products)

---

## 🛠️ Tech Stack & Dependencies
- **Node.js** (JavaScript Runtime)
- **Express** (Web Framework)
- **Mongoose** (MongoDB ODM)
- **dotenv** (จัดการ Environment Variables)
- **nodemon** (Auto-reload Server ระหว่าง Development)

---

## 🚀 การติดตั้งและเริ่มต้นใช้งาน (Getting Started)

1. โคลนโปรเจกต์และติดตั้ง Dependencies
```bash
git clone [https://github.com/AndyCK10/Node-Mongo.git](https://github.com/AndyCK10/Node-Mongo.git)
cd Node-Mongo
npm install

หากเริ่มสร้างโปรเจกต์เองตั้งแต่ต้น ให้ใช้คำสั่ง
npm init -y
npm i express mongoose dotenv
npm i -D nodemon

2. ตั้งค่า Environment Variables
PORT=3000
MONGODB_URL="mongodb+srv://<username>:<password>@<cluster>.mongodb.net/<dbname>?retryWrites=true&w=majority"
หมายเหตุ: อย่าลืมใส่ IP Address ของคุณใน Network Access บน MongoDB Atlas เป็น 0.0.0.0/0 หรือ IP ปัจจุบัน

3. ตั้งค่า Scripts ใน package.json
เพิ่ม script สำหรับรัน nodemon ในไฟล์ package.json:
# "scripts": {
#   "start": "node app.js",
#   "dev": "nodemon app.js"
# }

4. รันโปรเจกต์
โหมด Development (Hot Reload):

Bash
npm run dev
โหมด Production:

Bash
npm start