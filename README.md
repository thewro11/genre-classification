# Classification of Music Genres from the Given Music

## 👨‍👧‍👧 สมาชิกภายในกลุ่ม
- 6310400941 จิรัชญา ผ่านพินิจ
- 6310401041 ธิติ ทวีสิน
- 6310403974 ณัฐดนัย ตันวาณิชกุล

## 📝 รายงานความคืบหน้า
### ความคืบหน้าครั้งที่ 1
- ค้นคว้าหาแหล่งข้อมูล โดยได้พบแหล่งข้อมูลเป็น Spotify Web API ซึ่งสามารถทำ HTTP Request เพื่อดึงข้อมูลตัวอย่างเพลง (`.wav` audio file) ได้ (อยู่ในไฟล์ `/v01_pull_data_from_spotify.ipynb` และ `v02_create_multi_file_wav.ipynb`)
- แปลงไฟล์ตัวอย่างเพลง (`.wav`) แต่ละไฟล์ให้เป็นไฟล์รูปภาพ chroma key และ wave form สำหรับการทดลองจำแนกประเภทของเพลงด้วยการใช้ image classification (อยู่ในไฟล์ `v03_genre-classification.ipynb`)

### ความคืบหน้าครั้งที่ 2 (อยู่ในไฟล์ `v04_model.ipynb`)
- เตรียมข้อมูล Train, Validation, และ Test สำหรับการฝึกโมเดล โดยการแปลงไฟล์ตัวอย่างเพลง (`.wav`) แต่ละไฟล์ให้อยู่ในรูป array ของข้อมูล MFCC ของไฟล์ตัวอย่างเพลง โดยในเบื้องต้นมีข้อมูล 5 คลาส คลาสละ 150 เพลง
- สร้างโมเดล CNN ที่เรียนรู้จากชุดข้อมูล MFCC ของไฟล์ตัวอย่างเพลง
- ฝึกโมเดลและแสดงค่า Accuracy และ Loss

## 📦 Resource ของโครงงาน
- [ลิงก์ไฟล์รูปภาพ chroma key และ wave form](https://drive.google.com/drive/folders/1jTkwsPyasSwUhkH10SsyLqFdTN3Dn2qh)
- [ลิงก์ไฟล์เพลง .wav](https://drive.google.com/file/d/16YOO-ECQ_M4j4nF5oCfxYbD7wWBL5h5E/view?usp=share_link)