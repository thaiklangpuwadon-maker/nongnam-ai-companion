# Nong Nam AI Companion V2 Fix

แก้จากเวอร์ชันก่อน:
1. เพิ่มหน้า Permission ไมค์ก่อนเข้าใช้งานครั้งแรก
2. เก็บค่า micPermissionAsked / micPermissionGranted ใน localStorage
3. ไม่พาไปขออนุญาตไมค์ซ้ำทุกครั้ง
4. เพิ่มชุดผู้หญิง 12 เลเวล และผู้ชาย 12 เลเวล
5. เลเวล 1 ใช้งานได้ ชุดอื่นล็อกไว้
6. ถ้าเปิดใน Facebook/LINE/Messenger มีคำเตือนให้เปิด Safari/Chrome

หมายเหตุเรื่องไมค์:
- getUserMedia ใช้ขอสิทธิ์ไมค์
- SpeechRecognition ของ browser บางตัว โดยเฉพาะ in-app browser อาจยังฟังไม่ได้แม้อนุญาตไมค์แล้ว
- ถ้าจะขายจริง ควรใช้ STT API ผ่าน server เช่น Whisper/Google Speech แทน Web Speech API
