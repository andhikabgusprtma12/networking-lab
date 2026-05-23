# Basic Networking

## Deskripsi
Praktik basic networking dengan topologi sederhana sebagai berikut:
- Scenario satu network
 2 pc, 1 switch
- Scenario beda network
 2 pc, 1 switch
- Scenario beda network tapi saling konek
 2 pc, 1 switch, dan 1 router

## Topologi
- PC1, PC2 → SW1
- PC1, PC2 → SW1 → R1

## Tujuan
- Memahami cara kerja suatu jaringan
- Mengkoneksikan dua network yang berbeda

## Konfigurasi Utama
- Inter-network routing pada R1

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping antar PC satu network |  ✅ Berhasil |
| Ping PC beda network | ❌ Request time out (RTO) |
| Ping PC setelah konfigurasi | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** Network ID berbeda
- **Solusi:** Gunakan router untuk saling mengkoneksika network yang berbeda

## Referensi
- Packet Tracer Lab