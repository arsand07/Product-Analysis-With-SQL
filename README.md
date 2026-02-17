# 📊 E-Commerce Revenue Analysis (2017–2018)

## 📌 Project Overview

Project ini bertujuan untuk menganalisis pertumbuhan revenue pada dataset e-commerce selama periode 2017–2018.

Analisis difokuskan untuk menjawab pertanyaan berikut:
- Apakah revenue benar-benar bertumbuh?
- Apa yang mendorong pertumbuhan tersebut?
- Seberapa stabil pertumbuhannya?
- Apakah revenue terkonsentrasi pada transaksi besar?

---

## 🎯 Objectives

1. Mengukur tren revenue bulanan
2. Menghitung pertumbuhan (MoM & YoY)
3. Mengukur stabilitas pertumbuhan
4. Menganalisis distribusi revenue berdasarkan segmentasi transaksi
5. Menarik kesimpulan fase bisnis

---

## 🧹 Data Preparation

Dataset yang digunakan:
- Orders
- Order Items
- Payments
- Customers

Langkah data preparation:
- Menggunakan hanya order dengan status **"delivered"**
- Menggabungkan tabel untuk menghitung total revenue
- Mengelompokkan revenue per bulan

Alasan:
Revenue dianggap valid hanya jika order sudah delivered untuk menghindari bias dari order yang dibatalkan atau gagal.

---

## 📈 Step 1 — Revenue Trend Analysis

Menghitung total revenue per bulan.

**Temuan utama:**
- Revenue meningkat signifikan sepanjang 2017
- Puncak terjadi di akhir 2017 (~1.15M)
- Tahun 2018 revenue stabil di kisaran 1M–1.1M

**Insight:**
Bisnis mengalami fase pertumbuhan cepat (rapid expansion).

---

## 📊 Step 2 — Growth & Stability Analysis

Metode yang digunakan:
- Mean Monthly Growth (MoM)
- Year-over-Year Growth (YoY)
- Standard Deviation
- Coefficient of Variation (CV)

### Hasil

| Metric | 2017 | 2018 |
|--------|------|------|
| Avg MoM Growth | +31.55% | -0.95% |
| YoY Growth | - | +143% |
| CV | ~21% | ~21% |

**Insight:**
- 2017 → Pertumbuhan sangat agresif
- 2018 → Pertumbuhan mulai melambat
- Fluktuasi masih dalam kategori moderat

---

## 📦 Step 3 — Volume vs Value Analysis

Tujuan: Mengetahui apakah revenue naik karena:
- Jumlah order meningkat?
- Nilai transaksi per order meningkat?

Hasil:
- Average Order Value (AOV) relatif stabil (136–165)
- Kenaikan revenue didorong oleh peningkatan jumlah order

**Insight:**
Growth bersifat volume-driven, bukan price-driven.

---

## 🧩 Step 4 — Revenue Distribution Analysis

Segmentasi transaksi:

| Segment | Orders | Revenue |
|---------|--------|----------|
| 0–100 | 50,345 | 2.85M |
| 100–300 | 40,604 | 6.69M |
| >300 | 9,807 | 5.87M |

Kontribusi revenue:
- 100–300 → 43%
- >300 → 38%
- Top 10% transaksi menyumbang ~38.6% revenue

**Insight:**
Revenue cukup tersebar dan tidak terlalu terkonsentrasi pada segmen kecil.

---

## 🔄 Step 5 — Momentum Analysis

YoY Growth 2018: +143%  
Average MoM 2018: -0.95%

Interpretasi:
Secara tahunan bisnis masih tumbuh besar, tetapi momentum pertumbuhan mulai stagnan.

---

## 🏢 Business Phase Interpretation

- **2017 → Rapid Expansion**
- **2018 → Scale Consolidation**

Bisnis mulai memasuki fase stabilisasi setelah pertumbuhan agresif.

---

## 🧠 Key Takeaways

1. Revenue naik pesat karena peningkatan volume order.
2. Struktur revenue stabil dan tidak bergeser drastis antar segmen.
3. High-value transaction menyumbang ~38% revenue.
4. Momentum pertumbuhan mulai melambat di 2018.
5. Strategi retensi dan optimasi diperlukan untuk sustain growth.

---

## 🛠 Tools Used

- SQL Server 2022
- Microsoft Excel (Visualisasi)

---

## 📎 Author

Ari Sandi Kurniawan  
