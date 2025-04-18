# SafeSpace: Your Workspace Quality Monitor

## Overview

SafeSpace adalah sebuah aplikasi web yang dirancang untuk memantau kualitas lingkungan kerja dalam ruangan perkantoran. Aplikasi ini mengimplementasikan sistem IoT berbasis ESP32 untuk mengumpulkan data parameter lingkungan kerja secara real-time dan menyajikannya dalam antarmuka yang intuitif dan informatif.

## Fitur Utama

### Real-time Monitoring
- Pemantauan suhu (°C)
- Pemantauan kelembaban (%)
- Pemantauan kadar CO2 (ppm)
- Pemantauan kadar VOC (mg/m³)
- Pemantauan tingkat kebisingan (dB)
- Pemantauan kualitas pencahayaan (lux)

### Analytics Dashboard
- Visualisasi tren data selama 24 jam terakhir
- Grafik dinamis yang diperbarui secara real-time
- Indikator status parameter (Baik, Sedang, Buruk)

### AI-Powered Suggestions
- Analisis kondisi ruangan saat ini
- Prediksi perubahan parameter dalam beberapa jam ke depan
- Rekomendasi tindakan untuk meningkatkan kualitas ruangan
- Peringatan dini untuk parameter yang mendekati ambang batas tidak aman

### Employee Feedback System
- Rating kondisi ruangan dengan antarmuka intuitif
- Form untuk masukan dan saran dari karyawan
- Sistem notifikasi untuk konfirmasi pengiriman feedback

## Teknologi

SafeSpace dibangun menggunakan:
- **Frontend**: HTML5, CSS3, JavaScript
- **Sensor**: Modul ESP32 dengan sensor suhu, kelembaban, CO2, VOC, kebisingan, dan cahaya
- **AI Processing**: Algoritma Random Forest Classification dan Time Series Forecasting
- **Visualisasi**: Chart.js untuk visualisasi data dinamis

## Arsitektur Sistem

```
┌─────────────┐    ┌────────────┐    ┌─────────────┐
│  Sensor IoT  │───►│  Backend   │◄───┤  Frontend   │
│  (ESP32)     │    │  Server    │    │  (Web App)  │
└─────────────┘    └────────────┘    └─────────────┘
                         ▲
                         │
                  ┌──────┴───────┐
                  │  AI Engine   │
                  │ (Forecasting)│
                  └──────────────┘
```

## Manfaat

1. **Peningkatan Kesehatan dan Keselamatan Kerja (K3)**
   - Identifikasi cepat kondisi lingkungan kerja yang tidak sehat
   - Pencegahan masalah kesehatan yang terkait dengan kualitas udara dalam ruangan

2. **Efisiensi Energi**
   - Optimalisasi sistem HVAC berdasarkan data real-time
   - Penghematan energi melalui rekomendasi AI

3. **Peningkatan Produktivitas**
   - Lingkungan kerja yang lebih sehat mendorong produktivitas yang lebih tinggi
   - Pengurangan ketidakhadiran karyawan terkait masalah kesehatan

4. **Kepatuhan Regulasi**
   - Membantu organisasi memenuhi standar K3 yang ditetapkan
   - Dokumentasi kondisi lingkungan kerja untuk audit

## Cara Penggunaan

1. **Dashboard Utama**
   - Lihat status parameter lingkungan kerja saat ini
   - Perhatikan notifikasi untuk peringatan dan saran

2. **Analytics**
   - Analisa tren parameter selama 24 jam terakhir
   - Identifikasi pola dan anomali

3. **Feedback**
   - Berikan rating untuk kondisi lingkungan kerja
   - Sampaikan saran atau keluhan melalui form yang disediakan
