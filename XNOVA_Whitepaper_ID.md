# XNOVA
### Ekosistem Mining Deflasi DePIN di BNB Chain, Base & Polygon

**Whitepaper v1.0 — Juli 2026**

---

## Sangkalan

Dokumen ini hanya untuk tujuan informasi dan bukan merupakan nasihat keuangan, investasi, atau hukum. XNOVA adalah token utilitas yang digerakkan oleh komunitas. Aset kripto bersifat volatil dan mengandung risiko. Selalu lakukan riset sendiri (DYOR) sebelum berpartisipasi dalam pembelian token, aktivasi Boost, atau mint NFT apa pun.

---

## Daftar Isi

1. Ringkasan
2. Pendahuluan
3. Masalah
4. Solusi XNOVA
5. Cara Kerja Mining
6. Tokenomics
7. Mekanisme Burn
8. Ekosistem
9. Arsitektur Teknis
10. Keamanan & Kepercayaan
11. Roadmap
12. Alamat Kontrak & Verifikasi
13. Pengungkapan Risiko
14. Kesimpulan

---

## 1. Ringkasan

XNOVA adalah ekosistem mining deflasi yang terinspirasi dari konsep DePIN (Decentralized Physical Infrastructure Network), dibangun di atas BNB Chain, dengan perluasan yang sedang berlangsung ke Base dan Polygon. Berbeda dari model yield farming atau staking tradisional yang mengandalkan penerbitan token baru untuk membayar reward, mekanisme mining XNOVA didanai sepenuhnya oleh pembelian "Boost" dan NFT oleh pengguna. Setiap unit BNB yang dibelanjakan untuk mengaktifkan Boost atau mencetak (mint) NFT langsung dikonversi menjadi likuiditas permanen dan tidak dapat ditarik kembali di PancakeSwap, dengan token LP yang dihasilkan langsung dibakar (burn). Ini menciptakan lantai likuiditas yang terus bertumbuh dan tidak akan pernah bisa ditarik — baik oleh tim maupun siapa pun — dikombinasikan dengan pasokan token tetap yang tidak bisa dicetak ulang, di mana 50% di antaranya telah dibakar saat peluncuran.

XNOVA bukan sekadar token; ia adalah fondasi dari ekosistem yang lebih luas, mencakup agregator DEX multi-chain (xNovaSwap), platform peluncuran fair-launch untuk meme token (NOVAFUN), marketplace NFT (Kovyn), dompet dalam bentuk ekstensi browser (XNEO Wallet), platform chat komunitas Web3 (XNova Chat), konsol AI berbasis kepemilikan token (XNOVA AI), serta blockchain EVM buatan sendiri lengkap dengan explorer dan faucet miliknya sendiri (XNova Chain).

## 2. Pendahuluan

Ruang mining dan "GameFi" di Web3 telah dipenuhi oleh proyek-proyek yang menjanjikan imbal hasil tinggi yang didanai oleh penerbitan token yang tidak berkelanjutan, di mana peserta awal memperoleh keuntungan dengan mengorbankan peserta yang datang belakangan. Sebagian besar proyek ini memiliki tiga titik kegagalan yang sama:

- **Penerbitan reward yang inflasioner**, yang mengencerkan nilai pemegang token seiring waktu
- **Likuiditas yang tidak terkunci atau hanya terkunci sementara**, yang pada akhirnya bisa ditarik oleh tim
- **Tokenomics yang tidak transparan**, yang tidak dapat diverifikasi secara on-chain

XNOVA dirancang secara khusus untuk menghilangkan ketiga titik kegagalan ini sejak hari pertama.

## 3. Masalah

Sebagian besar platform "mining" atau "Boost" di Web3 saat ini beroperasi dengan salah satu dari dua model yang cacat:

1. **Model penerbitan gaya Ponzi** — setoran pengguna baru digunakan untuk membayar imbal hasil pengguna sebelumnya, tanpa penciptaan nilai nyata, sampai model tersebut runtuh.
2. **Likuiditas terkunci (bukan dibakar)** — tim mengunci token LP untuk jangka waktu tertentu (misalnya 100 hari, 1 tahun, bahkan 100 tahun), tetapi penguncian bukanlah sesuatu yang permanen. Penguncian dapat berakhir, diperpanjang secara curang, atau dilewati jika kontrak penguncian itu sendiri diretas atau merupakan proxy yang dikendalikan oleh tim.

Kedua model ini bergantung pada kepercayaan terhadap tim atau penyedia penguncian pihak ketiga. XNOVA menghilangkan ketergantungan ini sepenuhnya.

## 4. Solusi XNOVA

XNOVA menggantikan likuiditas yang "terkunci" dengan likuiditas yang "dibakar" — sebuah jaminan yang secara mendasar jauh lebih kuat.

| Model | Apakah likuiditas bisa ditarik? |
|---|---|
| Likuiditas tidak terkunci | Ya, kapan saja |
| Likuiditas terkunci dengan jangka waktu (misal 100 tahun) | Ya, begitu masa kunci berakhir, atau jika kontrak pengunci diretas |
| **Token LP yang dibakar (model XNOVA)** | **Tidak — tidak pernah, dalam keadaan apa pun** |

Ketika token LP dikirim ke alamat burn (dompet tanpa private key yang diketahui, misalnya `0x000...dEaD` atau alamat null yang setara), token tersebut menjadi permanen dan secara matematis tidak dapat dipulihkan. Ini bukan kebijakan atau janji — ini adalah jaminan kriptografis yang ditegakkan oleh blockchain yang sama yang mengamankan token itu sendiri.

Setiap kali pengguna membeli Boost mining atau mencetak NFT Supporter NFT, 100% BNB yang diterima dikonversi menjadi likuiditas XNOVA/BNB di PancakeSwap V2, dan token LP yang dihasilkan dibakar. Ini berarti:

- Kedalaman liquidity pool hanya akan terus bertambah — tidak akan pernah menyusut.
- Tidak ada skenario apa pun, baik jahat maupun tidak, yang memungkinkan likuiditas tersebut ditarik.
- Setiap pembelian di platform secara langsung dan permanen memperkuat lantai harga token.

## 5. Cara Kerja Mining

```
1. Beli Boost dengan BNB
   Pengguna mengaktifkan mining dengan membeli paket Boost
   menggunakan BNB.

2. Mining Token XNOVA
   Boost menghasilkan reward XNOVA seiring waktu berdasarkan
   besarnya investasi Anda.

3. BNB → Likuiditas
   100% BNB dari setiap pembelian Boost dikonversi menjadi
   likuiditas XNOVA/BNB di PancakeSwap V2.

4. Token LP Dibakar
   Token LP yang dihasilkan dari likuiditas tersebut langsung
   dibakar secara permanen — tidak dikunci, tidak divesting.
   Hilang selamanya.

5. Pasokan Deflasi
   Dikombinasikan dengan pembakaran 50% pasokan saat peluncuran,
   pasokan beredar dan likuiditas XNOVA hanya bergerak ke satu
   arah: menurun dan semakin terjamin secara permanen.
```

Reward mining didistribusikan dari alokasi khusus Mining Rewards (20% dari total pasokan) melalui smart contract mining resmi, seiring waktu, berdasarkan besar dan durasi Boost aktif milik pengguna.

## 6. Tokenomics

**Total Pasokan:** Tetap — tidak ada fungsi minting dalam kontrak. Pasokan hanya bisa menurun.

| Alokasi | % dari Total Pasokan | Tujuan |
|---|---|---|
| 🔥 Dibakar Saat Peluncuran | 50% | Dihapus secara permanen dari pasokan pada saat TGE. Dapat diverifikasi di BscScan. |
| 💧 Likuiditas (berkelanjutan) | 25% | Ditanamkan sejak awal dan terus diperkuat oleh pembelian Boost/NFT. LP dibakar pada setiap penambahan. |
| ⛏️ Reward Mining | 20% | Didistribusikan seiring waktu kepada penambang aktif melalui kontrak mining resmi. |
| 👨‍🚀 Tim | 5% | Berasal secara eksklusif dari pajak jual 5% — bukan dari alokasi di muka. Divesting/dikunci untuk pengembangan berkelanjutan. |

**Alamat Kontrak (BNB Chain):**
`0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69`

**Kontrak Mining:**
`0x06fe516f7631983cbf15626263bbdd97671f7735`

## 7. Mekanisme Burn

Prinsip kepercayaan inti dari XNOVA adalah pembakaran likuiditas yang berulang dan dipicu oleh setiap pembelian:

1. Pengguna membeli Boost atau mencetak NFT Supporter NFT, dengan pembayaran dalam BNB.
2. 100% dari BNB tersebut dipasangkan dengan XNOVA dan ditambahkan sebagai likuiditas ke pool XNOVA/BNB di PancakeSwap V2.
3. Token LP yang dihasilkan dari setoran tersebut dikirim ke alamat burn.
4. Posisi LP ini tidak akan pernah bisa ditarik oleh tim, oleh developer, atau oleh pihak ketiga mana pun — secara matematis tidak dapat diakses.

Ini berbeda dari — dan lebih kuat dari — penguncian likuiditas berbasis waktu. Penguncian adalah janji dengan tanggal kedaluwarsa. Pembakaran tidak memiliki tanggal kedaluwarsa, tidak memiliki pemilik, dan tidak memiliki kunci.

*Catatan: kadensi pembakaran yang tepat (per transaksi atau secara batch) dan apakah pembakaran dieksekusi secara otomatis oleh logika smart contract atau melalui transaksi manual yang dapat diverifikasi secara publik, harus diungkapkan secara transparan, disertai tautan transaksi burn langsung di BscScan setiap kali terjadi, guna menjaga akuntabilitas penuh.*

## 8. Ekosistem

XNOVA adalah lapisan dasar dari ekosistem Web3 yang lengkap:

| Produk | Tautan | Deskripsi |
|---|---|---|
| **XNOVA Core** | core.xnova.network | Platform mining deflasi utama — tempat pengguna membeli Boost, melakukan mining XNOVA, dan memicu mekanisme pembakaran likuiditas yang dijelaskan dalam dokumen ini. |
| **xNovaSwap** | app.xnova.network | Agregator DEX multi-chain non-custodial yang menemukan tarif swap terbaik di BNB Chain, Base, dan Polygon (PancakeSwap, QuickSwap, Uniswap, SushiSwap, BiSwap, dan lainnya), hanya dengan satu klik. |
| **NOVAFUN** | fun.xnova.network | Platform peluncuran fair-launch untuk meme token di BNB Chain. Token diluncurkan melalui bonding curve tanpa presale; likuiditas otomatis "naik kelas" ke PancakeSwap begitu mencapai batas 1 BNB, menghilangkan risiko rug-pull sejak dari desainnya. |
| **Kovyn** | kovyn.store | Marketplace NFT multi-chain di BNB Chain dan Base. Cetak dan daftarkan koleksi ERC-721 apa pun, bertransaksi dengan BNB, ETH, NOVA, TOSHI, BUSD atau USDC, dan sematkan NFT di mana saja melalui widget gratis. |
| **XNEO Wallet** | xneo.xnova.network | Dompet multi-chain dalam bentuk ekstensi browser, dengan fitur swap terintegrasi dan agregasi harga. |
| **XNova Chat** | chat.xnova.network | Platform chat real-time berbasis Web3 untuk trader kripto, kolektor NFT, dan komunitas blockchain, dengan akses yang dibatasi melalui koneksi dompet. |
| **XNOVA AI** | ai.xnova.network | Konsol AI berbasis kepemilikan token, yang hanya dapat diakses secara eksklusif oleh pemegang token XNOVA/NOVA di BNB Smart Chain. |
| **XNova Chain** | xrpc.xnova.network (explorer) · faucet.xnova.network (faucet) | Blockchain EVM buatan sendiri berbasis PoA (Chain ID 778 untuk mainnet, 1156 untuk testnet, simbol native NOVA), lengkap dengan block explorer sendiri, faucet testnet, dan bridge ke BSC. |

Pendekatan ekosistem ini berarti XNOVA bukanlah aset spekulatif tunggal, melainkan token utilitas dan reward yang menghubungkan sederet produk yang saling terintegrasi — sehingga meningkatkan kasus penggunaan nyata di luar sekadar spekulasi.

## 9. Arsitektur Teknis

- **Standar Token:** BEP-20 (BNB Chain), dengan perluasan cross-chain melalui infrastruktur bridge ke XNova Chain dan jaringan EVM lainnya.
- **Kontrak Mining:** Mendistribusikan reward XNOVA secara proporsional kepada pemegang Boost aktif berdasarkan besar dan durasi Boost.
- **Alur Kontrak Likuiditas:** Pembayaran Boost/NFT → pasangan LP otomatis di PancakeSwap V2 → pembakaran token LP.
- **Bridge XNova Chain:** Arsitektur bridge lock-and-mint antara BNB Chain dan XNova Chain, dilengkapi layanan relayer dan perlindungan anti-replay.
- **Lapisan NFT (NFT Supporter NFT):** Pembuatan SVG sepenuhnya on-chain dengan palet warna berbasis seed, memastikan metadata NFT tidak dapat hilang atau diubah di luar rantai (off-chain).

## 10. Keamanan & Kepercayaan

- **Tidak ada fungsi minting** — total pasokan bersifat tetap dan hanya bisa berkurang.
- **Tidak ada jalur penarikan likuiditas** — token LP dibakar, tidak dipegang oleh dompet atau kontrak pengunci mana pun.
- **Dapat diverifikasi on-chain** — semua pembakaran, penambahan likuiditas, dan distribusi mining dapat diverifikasi melalui BscScan.
- **Alokasi tim hanya berasal dari pajak jual** — tim tidak menerima alokasi token di muka sama sekali, menyelaraskan insentif dengan pertumbuhan ekosistem jangka panjang, bukan ekstraksi nilai sejak dini.

*Penambahan yang disarankan: laporan audit smart contract yang independen sebaiknya ditugaskan dan tautannya dicantumkan di sini sebelum melakukan dorongan besar menuju listing di exchange, untuk semakin memperkuat bagian ini.*

## 11. Roadmap

**Fase 1 — Selesai**
- Peluncuran token di BNB Chain
- Pembakaran 50% dari total pasokan saat peluncuran
- Penambahan likuiditas awal

**Fase 2 — Selesai**
- Kontrak mining diterapkan dan aktif
- Peluncuran koleksi NFT Supporter NFT
- Dimulainya ekspansi multi-chain (Polygon)

**Fase 3 — Sedang Berlangsung**
- Listing di CoinGecko & CoinMarketCap
- Program airdrop NFT
- Inisiatif pertumbuhan komunitas

**Fase 4 — Segera Hadir**
- Listing di exchange terpusat (CEX)
- Sistem governance untuk proposal komunitas
- Acara pembakaran token terjadwal lebih lanjut

## 12. Alamat Kontrak & Verifikasi

| Item | Alamat / Tautan |
|---|---|
| Token XNOVA (BNB Chain) | `0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69` |
| Kontrak Mining | `0x06fe516f7631983cbf15626263bbdd97671f7735` |
| Bukti Pembakaran Peluncuran | TX BscScan: `0x52eefca1b21c0c2af0816597070aa885b5c64f397f0bbe09d4b1cf7079b0b42e` |
| Kontrak xNovaSwap (BNB Chain) | `0xba10C405172cDA339B6dc898c151CB54Ac3a9fBD` |
| Kontrak NFT Kovyn (BNB Chain) | `0x81c03f5c8747fbF775934ed327Af640674FA01bC` |
| Kontrak NOVAFUN (BNB Chain) | `0x223733a3F2994FC554Ed90E8f62b653F9EB4E79A` |

Semua angka dan kontrak yang disebutkan dalam dokumen ini harus dapat diverifikasi secara independen oleh siapa pun pemegang token melalui BscScan kapan saja.

## 13. Pengungkapan Risiko

- Aset kripto dan DeFi sangat volatil. Nilai token dapat menurun secara signifikan.
- Smart contract, meskipun dirancang dengan hati-hati, mungkin mengandung kerentanan yang tidak terduga; pengguna sebaiknya hanya menempatkan dana yang mampu mereka relakan jika hilang.
- Perlakuan regulasi terhadap token, reward mining, dan NFT bervariasi menurut yurisdiksi dan dapat berubah.
- Pertumbuhan ekosistem di masa lalu atau peristiwa pembakaran sebelumnya bukan jaminan kinerja di masa depan.

## 14. Kesimpulan

Inovasi inti XNOVA sederhana namun kuat: menggantikan penguncian likuiditas yang berbasis kepercayaan dengan pembakaran likuiditas yang secara matematis bersifat permanen, didanai sepenuhnya oleh penggunaan platform secara organik, bukan oleh penerbitan token yang bersifat inflasioner. Dikombinasikan dengan pasokan tetap yang deflasi dan ekosistem produk yang terus bertumbuh — XNOVA Core, xNovaSwap, NOVAFUN, Kovyn, XNEO Wallet, XNova Chat, XNOVA AI, dan XNova Chain — XNOVA dibangun untuk menyelaraskan insentif pemegang jangka panjang dengan nilai yang nyata dan dapat diverifikasi secara on-chain.

---

*Dokumen ini akan diperbarui seiring perkembangan ekosistem XNOVA. Untuk versi terbaru, kunjungi xnova.network.*
