# Segmentation and Policy ( VLAN + ACL )

## Deskripsi
Praktik konfigurasi VLAN dan ACL pada jaringan dengan topologi
1 router, 2 switch, 4 PC, dan 1 server sebagai ISP.

## Topologi
- PC1, PC2 → SW1 → R1
- PC3, PC4 → SW2 → R1
- R1 → Server (ISP)

## Tujuan
- Memblokir PC4 supaya tidak bisa terkoneksi ke seluruh PC
- Seluruh PC bisa saling terkoneksi
- Seluruh PC termasuk PC4 bisa terkoneksi dengan Server

## Konfigurasi Utama
- VLAN pada SW1 dan SW2
- Subinterface dan Trunk mode pada SW1 dan SW2
- ACL pada R1
- DHCP pada R1

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping antar PC terkecuali PC4 | ✅ Berhasil |
| Ping seluruh PC menuju Server | ✅ Berhasil |
| Ping PC1 menuju PC4 | ❌ Request time out (RTO) |
| Ping PC4 menuju PC1 | 🚫 Destination Host Unreachable |
| Ping gateway PC1 menuju PC4 | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** DHCP Failed 
- **Solusi:** Trunk mode hanya untuk interface yang menuju R1

## Referensi
- Packet Tracer Lab