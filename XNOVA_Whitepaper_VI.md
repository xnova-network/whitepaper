# XNOVA
### Hệ Sinh Thái Đào Coin Giảm Phát DePIN trên BNB Chain, Base & Polygon

**Sách Trắng v1.0 — Tháng 7, 2026**

---

## Tuyên Bố Miễn Trừ Trách Nhiệm

Tài liệu này chỉ nhằm mục đích cung cấp thông tin và không phải là lời khuyên tài chính, đầu tư hay pháp lý. XNOVA là token tiện ích do cộng đồng dẫn dắt. Tài sản tiền mã hóa có tính biến động cao và tiềm ẩn rủi ro. Luôn tự nghiên cứu (DYOR) trước khi mua token, kích hoạt Boost, hoặc mint NFT.

---

## Mục Lục

1. Tóm Tắt
2. Giới Thiệu
3. Vấn Đề
4. Giải Pháp XNOVA
5. Cách Thức Đào Hoạt Động
6. Tokenomics
7. Cơ Chế Đốt Token
8. Hệ Sinh Thái
9. Kiến Trúc Kỹ Thuật
10. Bảo Mật & Niềm Tin
11. Lộ Trình Phát Triển
12. Địa Chỉ Hợp Đồng & Xác Minh
13. Công Bố Rủi Ro
14. Kết Luận

---

## 1. Tóm Tắt

XNOVA là hệ sinh thái đào coin giảm phát lấy cảm hứng từ mô hình DePIN (Mạng Lưới Cơ Sở Hạ Tầng Vật Lý Phi Tập Trung), được xây dựng trên BNB Chain, với kế hoạch mở rộng sang Base và Polygon. Khác với các mô hình yield farming hay staking truyền thống dựa vào việc phát hành token mới để trả thưởng, cơ chế đào của XNOVA được tài trợ hoàn toàn từ việc người dùng mua các gói "Boost" và NFT. Mỗi đơn vị BNB chi để kích hoạt Boost hoặc mint NFT sẽ được chuyển đổi trực tiếp thành thanh khoản vĩnh viễn, không thể thu hồi trên PancakeSwap, và các token LP tạo ra sẽ bị đốt ngay lập tức. Điều này tạo ra một nền tảng thanh khoản liên tục tăng trưởng, không bao giờ có thể rút được — dù bởi đội ngũ hay bất kỳ ai khác — kết hợp với nguồn cung token cố định, không thể mint thêm, trong đó 50% đã bị đốt ngay khi ra mắt.

XNOVA không chỉ là một token; đây là nền tảng của một hệ sinh thái rộng lớn hơn bao gồm bộ tổng hợp DEX đa chuỗi (xNovaSwap), nền tảng launchpad công bằng cho meme token (NOVAFUN), chợ NFT (Kovyn), ví dưới dạng tiện ích mở rộng trình duyệt (XNEO Wallet), nền tảng chat cộng đồng Web3 (XNova Chat), bảng điều khiển AI dành riêng cho người nắm giữ token (XNOVA AI), và một blockchain EVM tự xây dựng với trình khám phá và vòi nhận token thử nghiệm riêng (XNova Chain).

## 2. Giới Thiệu

Không gian đào coin và "GameFi" trong Web3 đã bão hòa với các dự án hứa hẹn lợi nhuận cao được tài trợ bởi việc phát hành token không bền vững, nơi người tham gia sớm hưởng lợi bằng chi phí của người tham gia sau. Hầu hết các dự án này đều mắc phải ba điểm yếu:

- **Phát hành phần thưởng lạm phát** làm loãng giá trị của người nắm giữ theo thời gian
- **Thanh khoản không khóa hoặc chỉ khóa tạm thời**, cuối cùng vẫn có thể bị đội ngũ rút ra
- **Tokenomics không minh bạch**, không thể xác minh on-chain

XNOVA được thiết kế đặc biệt để loại bỏ cả ba điểm yếu này ngay từ ngày đầu tiên.

## 3. Vấn Đề

Hầu hết các nền tảng "đào coin" hoặc "Boost" trong Web3 hiện nay hoạt động theo một trong hai mô hình có sai sót:

1. **Mô hình phát hành kiểu Ponzi** — tiền gửi của người dùng mới được dùng để trả lợi nhuận cho người dùng trước đó, không tạo ra giá trị thực, cho đến khi mô hình sụp đổ.
2. **Thanh khoản bị khóa (không bị đốt)** — đội ngũ khóa token LP trong một khoảng thời gian cố định (ví dụ 100 ngày, 1 năm, thậm chí 100 năm), nhưng việc khóa không phải là vĩnh viễn. Khóa có thể hết hạn, bị gia hạn gian lận, hoặc bị vượt qua nếu chính hợp đồng khóa bị xâm phạm hoặc là một proxy do đội ngũ kiểm soát.

Cả hai mô hình đều phụ thuộc vào niềm tin đối với đội ngũ hoặc bên khóa thứ ba. XNOVA loại bỏ hoàn toàn sự phụ thuộc này.

## 4. Giải Pháp XNOVA

XNOVA thay thế thanh khoản "bị khóa" bằng thanh khoản "bị đốt" — một sự đảm bảo mạnh mẽ hơn về bản chất.

| Mô hình | Thanh khoản có thể bị rút ra không? |
|---|---|
| Thanh khoản không khóa | Có, bất cứ lúc nào |
| Thanh khoản khóa theo thời gian (ví dụ 100 năm) | Có, một khi hết hạn khóa, hoặc nếu hợp đồng khóa bị xâm phạm |
| **Token LP bị đốt (mô hình XNOVA)** | **Không — không bao giờ, trong bất kỳ trường hợp nào** |

Khi token LP được gửi đến địa chỉ đốt (một ví không có khóa riêng tư nào được biết đến, ví dụ `0x000...dEaD` hoặc địa chỉ null tương đương), chúng trở nên vĩnh viễn và không thể khôi phục về mặt toán học. Đây không phải là một chính sách hay lời hứa — đó là một sự đảm bảo mật mã học được thực thi bởi chính blockchain đang bảo vệ token đó.

Mỗi khi người dùng mua một Boost đào coin hoặc mint một NFT Supporter NFT, 100% BNB nhận được sẽ được chuyển đổi thành thanh khoản XNOVA/BNB trên PancakeSwap V2, và các token LP tạo ra sẽ bị đốt. Điều này có nghĩa là:

- Độ sâu của pool thanh khoản chỉ có tăng lên — không bao giờ giảm.
- Không có kịch bản nào, dù ác ý hay không, có thể khiến thanh khoản đó bị rút ra.
- Mỗi giao dịch mua trên nền tảng đều trực tiếp và vĩnh viễn củng cố mức giá sàn của token.

## 5. Cách Thức Đào Hoạt Động

```
1. Mua Boost bằng BNB
   Người dùng kích hoạt việc đào bằng cách mua các gói Boost
   bằng BNB.

2. Đào Token XNOVA
   Các Boost tạo ra phần thưởng XNOVA theo thời gian dựa trên
   khoản đầu tư của bạn.

3. BNB → Thanh Khoản
   100% BNB từ mỗi lần mua Boost được chuyển đổi thành thanh
   khoản XNOVA/BNB trên PancakeSwap V2.

4. Token LP Bị Đốt
   Token LP được tạo ra từ thanh khoản đó bị đốt ngay lập tức
   và vĩnh viễn — không khóa, không vesting. Biến mất mãi mãi.

5. Nguồn Cung Giảm Phát
   Kết hợp với việc đốt 50% nguồn cung khi ra mắt, nguồn cung
   lưu hành và thanh khoản của XNOVA chỉ di chuyển theo một
   hướng duy nhất: giảm xuống và được bảo đảm vĩnh viễn hơn.
```

Phần thưởng đào được phân phối từ khoản phân bổ "Mining Rewards" chuyên biệt (20% tổng nguồn cung) thông qua hợp đồng thông minh đào chính thức, theo thời gian, dựa trên quy mô và thời hạn Boost đang hoạt động của người dùng.

## 6. Tokenomics

**Tổng Nguồn Cung:** Cố định — hợp đồng không có chức năng mint. Nguồn cung chỉ có thể giảm.

| Phân Bổ | % Tổng Nguồn Cung | Mục Đích |
|---|---|---|
| 🔥 Đốt Khi Ra Mắt | 50% | Loại bỏ vĩnh viễn khỏi nguồn cung tại thời điểm TGE. Có thể xác minh trên BscScan. |
| 💧 Thanh Khoản (liên tục) | 25% | Được khởi tạo ban đầu và liên tục được củng cố bởi các giao dịch mua Boost/NFT. LP bị đốt sau mỗi lần bổ sung. |
| ⛏️ Phần Thưởng Đào | 20% | Được phân phối theo thời gian cho các thợ đào đang hoạt động thông qua hợp đồng đào chính thức. |
| 👨‍🚀 Đội Ngũ | 5% | Chỉ đến từ thuế bán 5% — không phải từ phân bổ trước. Được vesting/khóa để phục vụ phát triển liên tục. |

**Địa Chỉ Hợp Đồng (BNB Chain):**
`0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69`

**Hợp Đồng Đào:**
`0x06fe516f7631983cbf15626263bbdd97671f7735`

## 7. Cơ Chế Đốt Token

Nguyên tắc niềm tin cốt lõi của XNOVA là việc đốt thanh khoản định kỳ, được kích hoạt bởi mỗi giao dịch mua:

1. Người dùng mua một Boost hoặc mint một NFT Supporter NFT, thanh toán bằng BNB.
2. 100% số BNB đó được ghép với XNOVA và thêm vào làm thanh khoản cho pool XNOVA/BNB trên PancakeSwap V2.
3. Các token LP được tạo ra từ khoản gửi đó sẽ được chuyển đến một địa chỉ đốt.
4. Vị thế LP này không bao giờ có thể bị rút bởi đội ngũ, nhà phát triển, hay bất kỳ bên thứ ba nào — nó không thể tiếp cận được về mặt toán học.

Điều này khác biệt — và mạnh mẽ hơn — so với việc khóa thanh khoản theo thời gian. Khóa là một lời hứa có ngày hết hạn. Đốt thì không có ngày hết hạn, không có chủ sở hữu, và không có chìa khóa.

*Lưu ý: tần suất đốt chính xác (theo từng giao dịch hay theo lô) và việc đốt được thực hiện tự động bởi logic hợp đồng thông minh hay thông qua giao dịch thủ công có thể xác minh công khai, cần được công bố minh bạch kèm liên kết đến các giao dịch đốt trực tiếp trên BscScan khi chúng xảy ra, để duy trì khả năng kiểm toán đầy đủ.*

## 8. Hệ Sinh Thái

XNOVA là lớp nền tảng của một hệ sinh thái Web3 toàn diện:

| Sản Phẩm | Liên Kết | Mô Tả |
|---|---|---|
| **XNOVA Core** | core.xnova.network | Nền tảng đào coin giảm phát chính — nơi người dùng mua Boost, đào XNOVA, và kích hoạt cơ chế đốt thanh khoản được mô tả trong tài liệu này. |
| **xNovaSwap** | app.xnova.network | Bộ tổng hợp DEX đa chuỗi, phi lưu ký, tìm ra tỷ giá swap tốt nhất trên BNB Chain, Base và Polygon (PancakeSwap, QuickSwap, Uniswap, SushiSwap, BiSwap, và nhiều nền tảng khác), chỉ với một cú nhấp chuột. |
| **NOVAFUN** | fun.xnova.network | Nền tảng launchpad công bằng cho meme token trên BNB Chain. Token được ra mắt thông qua đường cong bonding không có presale; thanh khoản tự động chuyển sang PancakeSwap khi đạt mức trần 1 BNB, loại bỏ rủi ro rug-pull ngay từ thiết kế. |
| **Kovyn** | kovyn.store | Chợ NFT đa chuỗi trên BNB Chain và Base. Mint và niêm yết bất kỳ bộ sưu tập ERC-721 nào, giao dịch bằng BNB, ETH, NOVA, TOSHI, BUSD hoặc USDC, và nhúng NFT ở bất cứ đâu thông qua widget miễn phí. |
| **XNEO Wallet** | xneo.xnova.network | Ví dưới dạng tiện ích mở rộng trình duyệt, hỗ trợ đa chuỗi, với chức năng swap tích hợp và tổng hợp giá. |
| **XNova Chat** | chat.xnova.network | Nền tảng chat thời gian thực dựa trên Web3 dành cho nhà giao dịch tiền mã hóa, nhà sưu tập NFT và cộng đồng blockchain, yêu cầu kết nối ví để truy cập. |
| **XNOVA AI** | ai.xnova.network | Bảng điều khiển AI dành riêng, chỉ mở khóa cho người nắm giữ token XNOVA/NOVA trên BNB Smart Chain. |
| **XNova Chain** | xrpc.xnova.network (trình khám phá) · faucet.xnova.network (vòi nhận token) | Blockchain EVM tự xây dựng, chạy theo cơ chế đồng thuận PoA (Chain ID 778 cho mainnet, 1156 cho testnet, ký hiệu gốc NOVA), có trình khám phá khối, vòi nhận token thử nghiệm, và cầu nối với BSC riêng. |

Cách tiếp cận theo hệ sinh thái này có nghĩa là XNOVA không phải là một tài sản đầu cơ đơn lẻ, mà là token tiện ích và phần thưởng kết nối một bộ các sản phẩm có thể tương tác với nhau — làm tăng các trường hợp sử dụng thực sự vượt ra ngoài việc đầu cơ.

## 9. Kiến Trúc Kỹ Thuật

- **Chuẩn Token:** BEP-20 (BNB Chain), với khả năng mở rộng đa chuỗi thông qua hạ tầng cầu nối tới XNova Chain và các mạng EVM khác.
- **Hợp Đồng Đào:** Phân phối phần thưởng XNOVA theo tỷ lệ cho những người nắm giữ Boost đang hoạt động, dựa trên quy mô và thời hạn của Boost.
- **Luồng Hợp Đồng Thanh Khoản:** Thanh toán Boost/NFT → tự động ghép cặp LP trên PancakeSwap V2 → đốt token LP.
- **Cầu Nối XNova Chain:** Kiến trúc cầu nối kiểu lock-and-mint giữa BNB Chain và XNova Chain, cùng với dịch vụ relayer và cơ chế bảo vệ chống replay.
- **Lớp NFT (NFT Supporter NFT):** Tạo SVG hoàn toàn on-chain với bảng màu dựa trên seed, đảm bảo dữ liệu metadata của NFT không thể bị mất hoặc thay đổi off-chain.

## 10. Bảo Mật & Niềm Tin

- **Không có chức năng mint** — tổng nguồn cung là bất biến và chỉ có thể giảm.
- **Không có đường dẫn rút thanh khoản** — token LP bị đốt, không được giữ bởi bất kỳ ví hay hợp đồng khóa nào.
- **Khả năng xác minh on-chain** — tất cả các lần đốt, bổ sung thanh khoản và phân phối đào đều có thể xác minh qua BscScan.
- **Phân bổ đội ngũ chỉ đến từ thuế bán** — đội ngũ không nhận bất kỳ phân bổ token trước nào, giúp đồng nhất động lực với sự phát triển dài hạn của hệ sinh thái thay vì khai thác sớm.

*Đề xuất bổ sung: nên thuê một đơn vị kiểm toán độc lập cho hợp đồng thông minh và liên kết báo cáo tại đây trước bất kỳ nỗ lực lớn nào nhằm niêm yết trên sàn giao dịch, để củng cố thêm phần này.*

## 11. Lộ Trình Phát Triển

**Giai Đoạn 1 — Hoàn Thành**
- Ra mắt token trên BNB Chain
- Đốt 50% tổng nguồn cung khi ra mắt
- Bổ sung thanh khoản ban đầu

**Giai Đoạn 2 — Hoàn Thành**
- Triển khai và kích hoạt hợp đồng đào
- Ra mắt bộ sưu tập NFT Supporter NFT
- Khởi động mở rộng đa chuỗi (Polygon)

**Giai Đoạn 3 — Đang Tiến Hành**
- Niêm yết trên CoinGecko & CoinMarketCap
- Chương trình airdrop NFT
- Các sáng kiến phát triển cộng đồng

**Giai Đoạn 4 — Sắp Tới**
- Niêm yết trên các sàn giao dịch tập trung (CEX)
- Hệ thống quản trị cho các đề xuất cộng đồng
- Thêm các sự kiện đốt token theo lịch trình

## 12. Địa Chỉ Hợp Đồng & Xác Minh

| Mục | Địa Chỉ / Liên Kết |
|---|---|
| Token XNOVA (BNB Chain) | `0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69` |
| Hợp Đồng Đào | `0x06fe516f7631983cbf15626263bbdd97671f7735` |
| Bằng Chứng Đốt Khi Ra Mắt | Giao dịch BscScan: `0x52eefca1b21c0c2af0816597070aa885b5c64f397f0bbe09d4b1cf7079b0b42e` |
| Hợp Đồng xNovaSwap (BNB Chain) | `0xba10C405172cDA339B6dc898c151CB54Ac3a9fBD` |
| Hợp Đồng NFT Kovyn (BNB Chain) | `0x81c03f5c8747fbF775934ed327Af640674FA01bC` |
| Hợp Đồng NOVAFUN (BNB Chain) | `0x223733a3F2994FC554Ed90E8f62b653F9EB4E79A` |

Tất cả các con số và hợp đồng được đề cập trong tài liệu này đều có thể được bất kỳ người nắm giữ nào xác minh độc lập qua BscScan bất cứ lúc nào.

## 13. Công Bố Rủi Ro

- Tài sản tiền mã hóa và DeFi có tính biến động rất cao. Giá trị token có thể giảm đáng kể.
- Hợp đồng thông minh, dù được thiết kế cẩn thận, vẫn có thể chứa các lỗ hổng chưa lường trước; người dùng chỉ nên đầu tư số tiền mà họ có thể chấp nhận mất.
- Việc xử lý pháp lý đối với token, phần thưởng đào và NFT khác nhau theo từng khu vực pháp lý và có thể thay đổi.
- Sự tăng trưởng trước đây của hệ sinh thái hay các sự kiện đốt trước đây không đảm bảo hiệu suất trong tương lai.

## 14. Kết Luận

Đổi mới cốt lõi của XNOVA đơn giản nhưng mạnh mẽ: thay thế các cơ chế khóa thanh khoản dựa trên niềm tin bằng việc đốt thanh khoản vĩnh viễn về mặt toán học, được tài trợ hoàn toàn bởi việc sử dụng nền tảng một cách tự nhiên thay vì bởi phát hành lạm phát. Kết hợp với nguồn cung cố định, giảm phát và một hệ sinh thái sản phẩm đang phát triển — XNOVA Core, xNovaSwap, NOVAFUN, Kovyn, XNEO Wallet, XNova Chat, XNOVA AI và XNova Chain — XNOVA được xây dựng để đồng nhất động lực của người nắm giữ dài hạn với giá trị thực, có thể xác minh trên chuỗi.

---

*Tài liệu này sẽ được cập nhật khi hệ sinh thái XNOVA phát triển. Để xem phiên bản mới nhất, truy cập xnova.network.*
