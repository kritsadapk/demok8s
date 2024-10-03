# ใช้ Node.js image
FROM node:14

# ตั้ง working directory
WORKDIR /usr/src/app

# คัดลอก package.json และ package-lock.json
COPY package*.json ./

# ติดตั้ง dependencies
RUN npm install

# คัดลอกไฟล์ทั้งหมดไปยัง container
COPY . .

# กำหนด port ที่แอปจะรัน
EXPOSE 3001

# คำสั่งเริ่มต้นเมื่อ container เริ่มทำงาน
CMD ["node", "app.js"]
