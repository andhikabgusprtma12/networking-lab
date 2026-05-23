# Service and Monitoring Lab

## Deskripsi
Praktik konfigurasi Service pada jaringan dengan topologi
1 router, 2 switch, 4 PC, 1 server sebagai ISP, dan 1 server sebagai service

## Topologi
- PC1, PC2 → SW1 → R1
- PC3, PC4 → SW2 → R1
- R1 → Server (ISP)
- R1 → Server (Service)

## Tujuan
- Membuat web server
- Membuat ssh server
- Semua PC bisa terkoneksi dengan service yang di buat

## Konfigurasi Utama
- Web Server pada Server (Service)
- SSH Server pada R1

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping Server service | ✅ Berhasil |
| Test web browser | ✅ Berhasil |
| Test ssh | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** Server Reset Connection
- **Solusi:** Ubah seach web browser dari 12.12.12.1 menjadi 12.12.12.2
## Referensi
- Packet Tracer Lab