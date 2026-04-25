# Tujuan Lab:
- Memahami bagaimana problem bisa mengacaukan sebuah jaringan dan cara troubleshooting yang terbaik untuk mengatasi problem tersebut.

# Hasil:
- Skenario Subnet Mask salah:
    - Output yang dihasilkan adalah Request time out.
- Skenario Interface router shutdown:
    - Output yang dihasilkan adalah Request time out an Unreachable.
## Hasil lebih lengkap bisa di cek di folder images

# Analisis
- Skenario Subnet Mask salah:
    - letak problem ada di Subnet, PC-0 menggunakan subnet 255.0 sedangkan PC-1 menggunakan subnet 255.192
- Skenario Interface router shutdown:
    - Letak problem ada di Interface itu sendiri yang off / shutdown, sehingga access gateway terganggu.

# Solusi
- Solusi Subnet Mask salah:
    - Subnet mask harus di samakan, misal 255.0 dan 255.0 jangan 255.0 dan 255.192.
- Solusi Interface router shutdown:
    - Nyalakan tombol on pada router untuk mengaktifkan kembali interface yang mati.