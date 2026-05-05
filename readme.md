##Tools yang dipakai untuk membuat video presentasi ini
<img src="https://img.shields.io/badge/Google%20Meet-00897B?style=for-the-badge&logo=googlemeet&logoColor=white"/>
<img src="https://img.shields.io/badge/CapCut-000000?style=for-the-badge&logo=capcut&logoColor=white"/>

Link YouTube
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)]([https://youtube.com/@USERNAME_KAMU](https://youtu.be/nQduUctuD1Q?si=oXB3K-YTabtNqqwx))

Identitas Laporan


| Keterangan     | Detail                                     |
| -------------- | ------------------------------------------ |
| Mata Kuliah    | Etika Profesi A                            |
| Dosen Pengampu | Adi Wahyu Pribadi, S.Si., M.Kom            |
| Kelompok       | Kelompok 13                                |
| Institusi      | Universitas Pancasila — Teknik Informatika |
| Semester       | Genap 2025/2026                            |


Anggota Kelompok


| NPM        | Nama                     |
| ---------- | ------------------------ |
| 4524210124 | Reno Budiman             |
| 4524210077 | Nayunda Krisna Abi Pasya |
| 4524210095 | Rofif Rizkullah Hisyam   |
| 4524210128 | Akmal Alief Ramadhan     |
| 4524210118 | Rangga Veda Aswangga     |






# Analisis Kasus: Ransomware Bank Syariah Indonesia (BSI) 2023

## Deskripsi Kasus

Pada Mei 2023, Bank Syariah Indonesia (BSI) mengalami serangan ransomware oleh kelompok LockBit 3.0 yang menyebabkan gangguan layanan perbankan selama beberapa hari. Layanan yang terdampak meliputi ATM, mobile banking, dan transaksi teller.

Selain itu, terdapat dugaan kebocoran sekitar 1,5 TB data yang mencakup data nasabah dan karyawan.

---

## Analisis Kritis

### **1. Kegagalan BCP/DRP (Business Continuity Plan / Disaster Recovery Plan)**

**Temuan Kritis:**
- Lumpuhnya layanan selama berhari-hari menunjukkan indikasi kegagalan sistemik dalam perencanaan kontinuitas bisnis.
- Dalam industri perbankan, standar global mensyaratkan high availability system, namun BSI gagal mempertahankan layanan dasar.

**Analisis:**
- Tidak adanya failover system yang efektif  
- Recovery Time Objective (RTO) tidak terpenuhi  
- Kemungkinan besar backup:
  - Tidak terisolasi (tidak air-gapped)
  - Ikut terenkripsi oleh ransomware  

**Kritik:**  
Kondisi ini menunjukkan bahwa BSI tidak berada pada level maturity keamanan siber yang memadai untuk institusi keuangan skala nasional.

---

### **2. Minimnya Transparansi (Potential Information Withholding)**

**Temuan Kritis:**
- Informasi kepada publik disampaikan secara terbatas, lambat, dan defensif  
- Tidak ada pengungkapan detail terkait:
  - Jenis data yang bocor  
  - Tingkat risiko bagi nasabah  

**Analisis:**
- Berpotensi melanggar prinsip right to be informed dalam perlindungan data pribadi  
- Menunjukkan pendekatan reputasi lebih diutamakan dibanding perlindungan konsumen  

**Kritik:**  
BSI terkesan lebih fokus pada pengendalian citra dibandingkan transparansi kepada nasabah.

---

### **3. Dampak Nyata terhadap Nasabah (Consumer Harm)**

**Dampak Langsung:**
- Tidak dapat melakukan transaksi finansial  
- Terganggunya aktivitas ekonomi, terutama bagi pelaku usaha  

**Dampak Tidak Langsung:**
- Risiko penyalahgunaan data seperti penipuan dan phishing  
- Penurunan kepercayaan terhadap sistem perbankan digital  

**Kritik:**
- Tidak terlihat adanya skema kompensasi yang jelas  
- Tidak ada mitigasi proaktif terhadap risiko kebocoran data  

---

## Analisis Hukum (Indonesia)

### **1. Undang-Undang No. 27 Tahun 2022 tentang Perlindungan Data Pribadi (UU PDP)**

**Pasal Relevan:**
- Pasal 39: Pengendali Data wajib menjaga keamanan data pribadi  
- Pasal 46: Wajib melakukan pemberitahuan jika terjadi kebocoran data  

**Analisis:**  
Jika kebocoran benar terjadi, BSI wajib memberikan notifikasi resmi kepada subjek data. Keterlambatan atau ketidakjelasan informasi dapat dikategorikan sebagai pelanggaran.

---

### **2. Peraturan OJK No. 38/POJK.03/2016 (Manajemen Risiko TI Perbankan)**

**Kewajiban Bank:**
- Menjamin keamanan, keandalan, dan ketersediaan sistem  
- Memiliki Disaster Recovery Center (DRC) yang berfungsi optimal  

**Analisis:**  
Gangguan berhari-hari menunjukkan bahwa DRC tidak berjalan efektif dan manajemen risiko TI tidak optimal.

---

### **3. Undang-Undang No. 8 Tahun 1999 tentang Perlindungan Konsumen**

**Hak Konsumen:**
- Hak atas kenyamanan, keamanan, dan keselamatan  
- Hak atas informasi yang benar, jelas, dan jujur  

**Analisis:**  
Nasabah dirugikan karena tidak dapat bertransaksi dan tidak mendapatkan informasi yang transparan.

---

### **4. PP No. 71 Tahun 2019 tentang Penyelenggaraan Sistem dan Transaksi Elektronik**

**Kewajiban:**
- Menjamin keandalan dan keamanan sistem elektronik  
- Melakukan mitigasi dan pemulihan saat terjadi gangguan  

**Analisis:**  
Kegagalan layanan menunjukkan ketidaksiapan dalam pemulihan sistem dan potensi pelanggaran kewajiban penyelenggara sistem elektronik.

---

## Evaluasi Keseluruhan

|        Aspek          |    Penilaian  |            Catatan                |
|-----------------------|---------------|-----------------------------------|
| Keamanan Siber        | Lemah         | Berhasil ditembus ransomware      |
| BCP/DRP               | Gagal         | Layanan lumpuh berhari-hari       |
| Transparansi          | Rendah        | Informasi tidak terbuka           | 
| Kepatuhan Hukum       | Dipertanyakan | Potensi pelanggaran UU PDP        |
| Perlindungan Konsumen | Kurang        | Dampak besar tanpa mitigasi jelas |

---

## Rekomendasi

### **Aspek Teknis**
- Implementasi Zero Trust Architecture  
- Backup berbasis immutable storage dan air-gapped system  
- Security Operations Center (SOC) 24/7  
- Penetration testing berkala  

### **Aspek Tata Kelola**
- Audit kepatuhan terhadap UU PDP dan regulasi OJK  
- Pembentukan tim Incident Response profesional  
- Simulasi serangan siber secara berkala  

### **Aspek Hukum dan Komunikasi**
- Pemberitahuan insiden secara cepat kepada publik  
- Notifikasi resmi kepada seluruh nasabah terdampak  
- Penyediaan kompensasi atau langkah remediasi  

---

## Kesimpulan Akhir

Kasus ransomware BSI bukan sekadar insiden teknis, melainkan indikasi kelemahan struktural dalam keamanan siber, tata kelola risiko, dan kepatuhan hukum.

**Tiga poin utama:**
1. Kegagalan sistemik pada BCP/DRP  
2. Kurangnya transparansi kepada publik  
3. Potensi pelanggaran regulasi perlindungan data dan konsumen  

Dalam konteks industri perbankan, kejadian ini menjadi peringatan bahwa transformasi digital tanpa kesiapan keamanan yang matang dapat menimbulkan risiko sistemik yang besar.
