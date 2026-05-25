# Linux Networkin & SSH

## Deskripsi
Praktik konfigurasi ssh remote akses menggunakan VirtualBox 
dengan Ubuntu sebagai host dan Debian sebagai client.

## Topologi
- Ubuntu (host) : 192.168.0.105
- Debian (client) : 192.168.0.110
- Network Mode : Bridge Adapter
- Koneksi : Ubuntu SSh → Debian

## Tujuan
- Setup SSH server di Debian client
- Remote akses dari Ubuntu host ke Debian client

## Konfigurasi Utama
- SSH Server di Debian client
- Bridge Adapter di VirtualBox
- SSH Client di Ubuntu host

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping Debian client ke Ubuntu host | ✅ Berhasil |
| SSH Ubuntu host ke Debian client | ✅ Berhasil |
| Remote command via SSH | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** SSH gagal koneksi saat network mode NAT
- **Solusi:** Ganti network NAT menjadi Bridge Adapter

## Referensi
- VirtualBox Documentation
- Debian OpenSSH Manual