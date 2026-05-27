# Linux Networkin & SSH

## Deskripsi
Praktik konfigurasi web server menggunakan Apache2 pada Debian server
dengan Ubuntu sebagai client uang mengakses web server via browser

## Topologi
- Ubuntu (client) : 192.168.0.105
- Debian (server) : 192.168.0.110
- Network Mode : Bridge Adapter
- Koneksi : Ubuntu Browser → Apache2 Debian

## Tujuan
- Install dan konfigurasi Apache2 di Debian server
- Akses web server dari Ubuntu client via browser
- Memahami lifecycle sebuah service (enable, start, stop)

## Konfigurasi Utama
- Apache2 Web Server di Debian Server
- Bridge Adapter di VirtualBox
- Default page Apache2 sebagai landing page

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Akses Web Server dari Ubuntu client | ✅ Berhasil |
| Service Start | ✅ Berhasil |
| Servuce Stop | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** Problem landing page
- **Solusi:** Enable, Start, atau Restart apache2

## Referensi
- Apache2 Documentation
- Debian System Administration Manual