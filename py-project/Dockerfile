# ใช้ base image ที่มี Python ติดตั้งอยู่
FROM python:3.10-slim

# กำหนด directory ที่จะใช้ใน container
WORKDIR /app

# คัดลอกไฟล์ requirements.txt เข้ามาใน container
COPY requirements.txt .

# ติดตั้ง dependencies ที่ระบุใน requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# คัดลอก source code ของคุณเข้ามาใน container
COPY . .

# กำหนดคำสั่งที่ต้องการให้รันเมื่อ container เริ่มทำงาน
# CMD ["python", "your_script.py"]
