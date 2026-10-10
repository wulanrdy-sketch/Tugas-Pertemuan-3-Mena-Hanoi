# Tugas Menara Hanoi (Tower of Hanoi) - 4 Disk

## Deskripsi Tugas
Program ini dibuat untuk menyelesaikan tantangan Menara Hanoi dengan skenario:
- **Start:** 4 disk tersusun di tiang A.
- **Finish:** 4 disk tersusun di tiang C.
- **Aturan:** Hanya bisa memindahkan satu disk sekaligus, dan disk yang lebih besar tidak boleh diletakkan di atas disk yang lebih kecil.

## Bahasa Program & Tools
- **Bahasa:** Python
- **Platform:** Google Colab

## Penjelasan Algoritma (Notes)
Masalah Menara Hanoi diselesaikan menggunakan metode **Rekursi (Recursion)**. Berikut adalah logika berpikirnya untuk memindahkan `n` disk dari tiang `A` ke `C` dengan bantuan tiang `B`:

1. **Kasus Dasar (Base Case):** Jika hanya ada 1 disk (`n == 1`), langsung pindahkan disk tersebut dari tiang asal ke tiang tujuan.
2. **Langkah Rekursif (Jika n > 1):**
   - Langkah 1: Pindahkan `n-1` disk dari tiang **Asal (A)** ke tiang **Bantu (B)**, dengan tiang **Tujuan (C)** sebagai penopang sementara.
   - Langkah 2: Pindahkan disk ke-`n` (disk terbesar) dari tiang **Asal (A)** ke tiang **Tujuan (C)**.
   - Langkah 3: Pindahkan `n-1` disk yang tadi berada di tiang **Bantu (B)** ke tiang **Tujuan (C)**, dengan tiang **Asal (A)** sebagai penopang sementara.

## Kompleksitas Waktu
Jumlah langkah minimum untuk menyelesaikan Menara Hanoi dengan `n` disk adalah **2^n - 1**.
- Untuk 4 disk (sesuai soal): 2^4 - 1 = **15 langkah**.# Tugas-Pertemuan-3-Mena-Hanoi
