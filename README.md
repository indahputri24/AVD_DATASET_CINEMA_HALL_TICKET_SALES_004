# Analisis Perilaku Penonton Bioskop: Python & Tableau

Mini project mata kuliah Analisis dan Visualisasi Data. Proyek ini menganalisis 1.440 transaksi tiket bioskop untuk memahami pola pembelian, preferensi genre, pemilihan tipe kursi, harga tiket, dan faktor yang memengaruhi pembelian ulang.

## Dataset
[Cinema Hall Ticket Sales and Customer Behavior](https://www.kaggle.com/datasets/himelsarder/cinema-hall-ticket-sales-and-customer-behavior) (Kaggle): 1.440 baris dan 7 kolom (usia, harga tiket, genre film, tipe kursi, jumlah penonton per transaksi, dan pembelian ulang).

## Tools
Python (Google Colab), Pandas, Matplotlib, Seaborn, Tableau Public.

## Struktur Repositori

| Folder | Isi |
|---|---|
| `Checkpoint 1` | Business understanding: tujuan bisnis, tujuan analisis data, dan rencana proyek |
| `Checkpoint 2` | Data understanding dan data preparation (menghasilkan `data_bersih_cinnema_ticket.xlsx`) |
| `Checkpoint 3` | Visualisasi dan insight di Python |

## Alur Kerja

1. **Business understanding:** menentukan tujuan dan rencana analisis.
2. **Data understanding:** memeriksa struktur data, statistik deskriptif, dan korelasi awal.
3. **Data preparation:**
   - Memeriksa missing value, duplikat, dan outlier (IQR): tidak ditemukan.
   - Mengubah nilai "Alone" menjadi 1 pada jumlah penonton.
   - Mengubah Yes/No menjadi 1/0 pada pembelian ulang.
   - Membuat kolom total harga tiket per transaksi.
   - Menghapus kolom ID tiket.
4. **Visualisasi di Python:** histogram, bar chart, boxplot, dan analisis korelasi, masing-masing dengan insight dan rekomendasi.
5. **Dashboard di Tableau:** data hasil pembersihan divisualisasikan dalam dashboard interaktif dengan filter genre, tipe kursi, jumlah penonton, rentang usia, dan harga tiket.

## Temuan Utama

- Hampir separuh transaksi (±48%) adalah pembelian 1 tiket.
- Action dan Horror paling banyak ditonton, Sci-Fi paling sedikit.
- VIP paling banyak dipilih (36,2%), diikuti Standard (32,0%) dan Premium (31,7%).
- Median harga tiket hampir sama di semua tipe kursi (±16–18).
- Median usia penonton sekitar 38–41 tahun di semua genre.
- Semua variabel berkorelasi sangat lemah dengan pembelian ulang (|r| < 0,05), sehingga tidak ada faktor tunggal yang menonjol.
