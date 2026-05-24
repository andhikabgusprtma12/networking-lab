# Small Office Network

## Deskripsi
Konfigurasi projek jaringan sederhana dengan topologi
1 router, 4 switch, 28 PC, 1 server sebagai ISP, dan 1 server sebagai service

## Topologi
- PC1 - PC8 → SW1 → R1
- PC9 - PC16 → SW2 → R1
- PC17 - PC24 → SW3 → R1
- PC25 - PC28 → SW4 → R1
- R1 → Server (ISP)
- R1 → Server (Service)

## Tujuan
- Konfigurasi vlan, dhcp, nat, dan acl
- Membuat dns server
- Membuat web server
- Membuat ssh server
- Semua PC bisa terkoneksi dengan service
- ACL berjalan sesuai tujuan

## Konfigurasi Utama
- VLAN pada SW
- DCHP pada R1
- NAT pada R1
- ACL pada R1
- DNS Server pada Server (ISP)
- Web Server pada Server (Service)
- SSH Server pada R1

## Hasil Pengujian
| Pengujian | Hasil |
|-----------|-------|
| Ping Server service | ✅ Berhasil |
| Ping Server ISP | ✅ Berhasil |
| Test dns | ✅ Berhasil |
| Test web browser | ✅ Berhasil |
| Test ssh | ✅ Berhasil |
| Ping staff ke marketing | ✅ Berhasil |
| Ping staff ke finance | 🚫 Destination Host Unreachable |
| Ping staff ke it | 🚫 Destination Host Unreachable |
| Ping marketing ke staff | ✅ Berhasil |
| Ping marketing ke finance | 🚫 Destination Host Unreachable |
| Ping marketing ke it | 🚫 Destination Host Unreachable |
| Ping finance ke staff | 🚫 Destination Host Unreachable |
| Ping finance ke marketing | 🚫 Destination Host Unreachable |
| Ping finance ke it | 🚫 Destination Host Unreachable |
| Ping it ke staff | ✅ Berhasil |
| Ping it ke marketing | ✅ Berhasil |
| Ping it ke finance | ✅ Berhasil |

## Kendala & Solusi
- **Kendala:** IT tidak bisa terhubung ke semua divisi
- **Solusi:** Utamakan permit icmp any any echo-reply sebelum deny
## Referensi
- Packet Tracer Lab