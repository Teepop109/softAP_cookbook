## ESP32-WiFi-AP - `softAP`
ใน ESP32, ฟังก์ชัน softAP ใช้สำหรับการสร้าง Wi-Fi Access Point (AP) หรือเรียกว่าโหมด "Soft Access Point" โดย ESP32 จะทำหน้าที่เป็นตัวกระจายสัญญาณ Wi-Fi ให้กับอุปกรณ์อื่น ๆ เชื่อมต่อเข้ามาได้ แทนที่จะทำหน้าที่เป็นลูกข่าย (Client) ไปเชื่อมต่อกับ Wi-Fi Network ที่มีอยู่
## ขั้นตอนการใช้งาน
1. เริ่มต้นโดยการเลือกตัวอย่าง `softAP`
# ![Screenshot 2024-10-30 195106](https://github.com/user-attachments/assets/a97759b7-c273-4dee-a48c-f96494e0559b)


# ![Screenshot 2024-10-30 195059](https://github.com/user-attachments/assets/382e7bcf-74db-4b5f-8935-db6314f0d0ff)


2. หลังจากเลือกตัวอย่างแล้ว ให้กดปุ่ม **Create**
# ![Screenshot 2024-10-30 195113](https://github.com/user-attachments/assets/7e0b5b01-a0a7-4057-b550-0ca30b05b552)


3. ตรวจสอบโค้ดในไฟล์ ` Kconfig.projbuild` สามารถแก้ไขเป็นชื่อของตัวเองที่ต้องการ เพราะจะได้เชื่อมต่อได้อย่างถูกต้องและเข้าใจ
# ![Screenshot 2024-10-30 195245](https://github.com/user-attachments/assets/9f955ec9-2bb5-4d1a-90ec-0c92f9c71a8e)

# ![Screenshot 2024-10-30 195300](https://github.com/user-attachments/assets/c7172a61-202a-4f73-87a2-c8fb5a6ea9a7)


## กด Buildเเละรันโปรแกรม

กด Build และรันโปรแกรม จากนั้นเลือก **UART**
# ![Screenshot 2024-10-30 195700](https://github.com/user-attachments/assets/31e2d617-1832-4342-a93c-8126ee65e4e7)

จะเจอ "SSID-..." ที่เรากำหนดไว้ เรากำหนดไว้ว่า " WiFiteepop109 "
ผลลัพธ์จะมีลักษณะดังนี้:
# ![Screenshot 2024-10-30 195700](https://github.com/user-attachments/assets/334f4787-88fb-4b3d-afd5-8c942ec450dc)
# พบว่ามี WiFi ชื่อ " WiFiteepop109 "
## เมื่อลองเชื่อมต่อ WiFi
# ![Screenshot 2024-10-30 201031](https://github.com/user-attachments/assets/eee38ac9-58b6-4abd-abe6-41879ffc26fc)
# ![Screenshot 2024-10-30 201004](https://github.com/user-attachments/assets/455d8c62-8f5b-420c-8bd1-025ff5a09803)
จะพบว่า IP ที่เชื่อมกับ ESP32 จะตรงกัน 
# ![Screenshot 2024-10-30 195814](https://github.com/user-attachments/assets/0dc74060-47ad-43cc-b2e9-c8f1c07c56d5)

### สรุปการทดลอง
สามารถใช้ ESP32 เพื่อให้เป็น WiFi-AP (Access Point) ทำหน้าที่เป็นจุดเชื่อมต่อให้กับอุปกรณ์อื่นๆ สามารถเชื่อมต่อเข้ามาได้ อุปกรณ์จะสร้างเครือข่าย Wi-Fi ที่ผู้ใช้สามารถเชื่อมต่อเพื่อเข้าถึงอินเทอร์เน็ตหรือเครือข่ายภายใน
