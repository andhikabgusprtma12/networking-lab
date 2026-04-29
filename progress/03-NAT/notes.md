# NAT (Network Address Translation)

## Deskripsi
Praktik konfigurasi NAT pada jaringan dengan topologi
2 router, 3 switch, 6 PC, dan 1 server sebagai ISP.

## Topologi
- PC0, PC1, PC2 → SW1 → R1
- PC3, PC4, PC5 → SW2 → R1
- R1 → SW3 → R2 → Server (ISP)

## Tujuan
- PC antar network dapat saling berkomunikasi
- Seluruh PC dapat mengakses internet melalui NAT

## Konfigurasi Utama
- Inter-network routing pada R1
- NAT Overload (PAT) pada R1
- Default route R1 → R2

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping antar PC beda network | ✅ Berhasil |
| Ping ke gateway | ✅ Berhasil |
| Ping ke internet (Server) | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** Cloud tidak bisa di-ping sebagai simulasi ISP
- **Solusi:** Mengganti Cloud dengan Server dan dikonfigurasi
  sebagai endpoint ISP

## Referensi
- Packet Tracer Lab