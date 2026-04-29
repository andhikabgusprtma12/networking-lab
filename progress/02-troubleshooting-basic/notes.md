# Trouble Shooting Basic

## Deskripsi
Praktik trouble shooting basic dengan topologi sederhana sebagai berikut:
- Scenario Subnet Mask salah
 2 pc, 1 switch
- Scenario Interface Shutdown
 2 pc, 1 switch, 1 router

## Topologi
- PC0, PC1 → SW1
- PC0, PC1 → SW1 → R1

## Tujuan
- Memahami cara kerja sebuah masalah pada suatu jaringan
- Membenarkan masalah yang terjadi pada suatu jaringan

## Konfigurasi Utama
- Inter-network routing pada R1
- Shutdown interface pada R1

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping antar PC beda subnet | ❌ Request time out (RTO) |
| Ping ke gateway aktif | ❌ Request time out (RTO) |
| Ping ke gateway nonakitif | 🚫 Destination Host Unreachable |

## Kendala & Solusi
- **Kendala:** Subnet Mask berbeda dan Interface shutdown
- **Solusi:** Samakan Subnet Mask agar bisa saling terkoneksi (255.0 sama 255.0) dan ketik command no shutdown di R1

## Referensi
- Packet Tracer Lab

