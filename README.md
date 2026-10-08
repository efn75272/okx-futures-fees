# phí futures OKX: Cách tính maker, taker, funding và chọn mức phí phù hợp khi giao dịch hợp đồng

Khi tìm kiếm **phí futures OKX**, phần lớn người dùng muốn biết ba điều: mở và đóng một vị thế tốn bao nhiêu, phí có tính trên tiền ký quỹ hay toàn bộ giá trị lệnh, và làm thế nào để giảm chi phí giao dịch.

Câu trả lời ngắn gọn là: phí futures OKX được tính trên **giá trị danh nghĩa của vị thế**, không phải chỉ trên số tiền ký quỹ. Lệnh được khớp ngay thường chịu phí taker, còn lệnh nằm trên sổ lệnh trước khi khớp thường chịu phí maker. Với futures vĩnh cửu, bạn còn phải theo dõi phí funding vì khoản này được trao đổi giữa bên long và bên short trong từng chu kỳ thanh toán.

Bài viết này tổng hợp cách tính phí futures OKX, bảng phí Regular và VIP, các khoản chi phí có thể phát sinh, cùng cách sử dụng mã `CASH20` khi đăng ký qua liên kết được cung cấp.

> **Lưu ý về số liệu:** Nội dung được đối chiếu với trang phí và tài liệu hỗ trợ OKX đang hiển thị tại thời điểm kiểm tra ngày **6 tháng 10 năm 2026**. OKX cho biết mức phí thực tế của từng tài khoản có thể khác nhau theo khu vực, cặp giao dịch, cấp phí và trạng thái tài khoản. Hãy kiểm tra con số hiển thị trong bảng đặt lệnh trước khi giao dịch.

## Phí futures OKX gồm những khoản nào?

Một giao dịch futures thường có thể liên quan đến các khoản sau:

- Phí giao dịch khi mở vị thế.
- Phí giao dịch khi đóng vị thế.
- Phí funding đối với hợp đồng futures vĩnh cửu.
- Phí thanh lý bắt buộc nếu vị thế bị thanh lý.
- Phí thanh toán đối với một số hợp đồng futures kỳ hạn.
- Chênh lệch giá và trượt giá, dù đây không phải là phí giao dịch được ghi riêng.

Phí mở và phí đóng không có công thức riêng biệt. Cả hai đều dựa trên giá trị lệnh được khớp và mức maker hoặc taker áp dụng tại thời điểm đó. Nếu bạn mở vị thế bằng lệnh thị trường rồi đóng bằng lệnh thị trường, cả hai lần khớp thường đều chịu phí taker.

Điểm dễ nhầm nhất là **đòn bẩy không làm giảm giá trị dùng để tính phí**. Đòn bẩy chỉ giúp bạn dùng ít vốn ký quỹ hơn để kiểm soát vị thế lớn hơn. Phí vẫn được tính trên toàn bộ giá trị danh nghĩa của vị thế.

Ví dụ, bạn dùng 1.000 USDT làm ký quỹ với đòn bẩy 10x để mở vị thế trị giá 10.000 USDT. Với phí taker 0,05%, phí cho một lần khớp sẽ là:

text
10.000 USDT × 0,05% = 5 USDT


Nếu sau đó đóng vị thế với cùng giá trị và cũng chịu phí taker 0,05%, tổng phí giao dịch hai chiều là khoảng 10 USDT, chưa tính funding, trượt giá hoặc những khoản khác nếu có.

## Maker và taker khác nhau thế nào?

### Taker

Taker là lệnh lấy thanh khoản có sẵn trên sổ lệnh. Lệnh thị trường thường thuộc nhóm này vì được khớp ngay với các lệnh đang chờ.

Một lệnh giới hạn cũng có thể trở thành taker. Tên “lệnh giới hạn” không tự động đồng nghĩa với maker. Nếu lệnh giới hạn của bạn khớp ngay với lệnh đang có trên sổ lệnh, hệ thống có thể tính phí taker.

### Maker

Maker là lệnh được đưa lên sổ lệnh và chờ người khác khớp. Lệnh này bổ sung thanh khoản nên thường có mức phí thấp hơn taker.

Tuy nhiên, không nên cố biến mọi lệnh thành maker chỉ để tiết kiệm phí. Trong thị trường biến động mạnh, chờ lệnh khớp có thể khiến bạn bỏ lỡ điểm vào hoặc bị khớp một phần. Khoản phí thấp hơn không có nhiều ý nghĩa nếu giá vào lệnh lệch quá xa kế hoạch.

## Bảng phí futures OKX hiện tại

OKX sử dụng hệ thống gồm tài khoản Regular và các cấp VIP từ VIP 1 đến VIP 9. Cấp phí có thể được xác định bằng tài sản nắm giữ hoặc khối lượng giao dịch trong 30 ngày. Tài khoản được hưởng cấp cao nhất nếu đáp ứng nhiều điều kiện khác nhau.

Bảng dưới đây tổng hợp mức phí futures được OKX công bố. “Nhóm 1” thường chỉ nhóm các cặp có thanh khoản cao theo danh sách của OKX, còn “Nhóm 2” là các cặp khác trong phạm vi áp dụng. Danh sách cặp cụ thể có thể thay đổi theo thời điểm và khu vực.

| Cấp phí | Điều kiện tham khảo về tài sản hoặc khối lượng futures 30 ngày | Maker nhóm 1 | Taker nhóm 1 | Maker nhóm 2 | Taker nhóm 2 | Liên kết đăng ký |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| Regular | Tài sản dưới 100.000 USD hoặc futures dưới 5.000.000 USD | 0,0200% | 0,0500% | 0,0200% | 0,0500% | [ Đăng ký và kiểm tra ưu đãi CASH20](https://okx.com/join/CASH20) |
| VIP 1 | Tài sản từ 100.000 USD hoặc futures từ 5.000.000 USD | 0,0160% | 0,0450% | 0,0160% | 0,0450% | [ Mở tài khoản OKX qua mã CASH20](https://okx.com/join/CASH20) |
| VIP 2 | Tài sản từ 200.000 USD hoặc futures từ 10.000.000 USD | 0,0150% | 0,0360% | 0,0150% | 0,0360% | [ Kiểm tra điều kiện phí futures OKX](https://okx.com/join/CASH20) |
| VIP 3 | Tài sản từ 2.000.000 USD hoặc futures từ 50.000.000 USD | 0,0100% | 0,0280% | 0,0100% | 0,0280% | [ Đăng ký OKX để xem cấp phí](https://okx.com/join/CASH20) |
| VIP 4 | Tài sản từ 5.000.000 USD hoặc futures từ 200.000.000 USD | 0,0080% | 0,0270% | 0,0080% | 0,0270% | [ Xem bảng phí áp dụng cho tài khoản](https://okx.com/join/CASH20) |
| VIP 5 | Tài sản từ 20.000.000 USD hoặc futures từ 600.000.000 USD | 0,0050% | 0,0260% | 0,0050% | 0,0260% | [ Tham gia OKX qua liên kết ưu đãi](https://okx.com/join/CASH20) |
| VIP 6 | Tài sản từ 50.000.000 USD hoặc futures từ 1.000.000.000 USD | 0,0000% | 0,0250% | 0,0000% | 0,0250% | [ Kiểm tra mức phí VIP cao hơn](https://okx.com/join/CASH20) |
| VIP 7 | Tài sản từ 100.000.000 USD hoặc futures từ 1.500.000.000 USD | -0,0020% | 0,0200% | -0,0050% | 0,0250% | [ Xem quyền lợi VIP của OKX](https://okx.com/join/CASH20) |
| VIP 8 | Tài sản từ 250.000.000 USD hoặc futures từ 2.000.000.000 USD | -0,0050% | 0,0200% | -0,0100% | 0,0250% | [ Đăng ký và xem biểu phí hiện hành](https://okx.com/join/CASH20) |
| VIP 9 | Tài sản từ 500.000.000 USD hoặc futures từ 20.000.000.000 USD | -0,0050% | 0,0150% | -0,0100% | 0,0200% | [ Mở tài khoản OKX](https://okx.com/join/CASH20) |

Mức âm ở cột maker có nghĩa là người dùng có thể nhận rebate theo điều kiện của cấp phí, thay vì trả phí maker thông thường. Đây là mức dành cho cấp VIP cao, không phải ưu đãi mặc định cho tài khoản mới.

Người mới nên quan tâm trước hết đến dòng Regular. Với mức 0,0200% maker và 0,0500% taker, bạn có thể ước tính nhanh chi phí trước khi đặt lệnh. Cấp VIP chỉ trở nên thực tế nếu bạn có khối lượng giao dịch hoặc tài sản đủ lớn. Không nên tăng khối lượng giao dịch chỉ để săn mức phí thấp hơn, vì phí tiết kiệm được có thể nhỏ hơn chi phí do giao dịch quá mức.

## Cách tính phí futures OKX bằng USDT hoặc USDC

Đối với hợp đồng ký quỹ bằng USDT hoặc USDC, công thức cơ bản là:

text
Phí giao dịch =
Tỷ lệ phí × Số hợp đồng × Hệ số nhân × Khối lượng hợp đồng × Giá khớp


Trong nhiều hợp đồng phổ biến, có thể hiểu đơn giản hơn:

text
Phí giao dịch = Giá trị danh nghĩa vị thế × Tỷ lệ phí


Giả sử bạn mở vị thế BTCUSDT trị giá 20.000 USDT:

- Nếu là taker với phí 0,05%: `20.000 × 0,05% = 10 USDT`.
- Nếu là maker với phí 0,02%: `20.000 × 0,02% = 4 USDT`.

Nếu đóng vị thế với cùng giá trị:

- Mở taker, đóng taker: khoảng 20 USDT.
- Mở maker, đóng maker: khoảng 8 USDT.
- Mở maker, đóng taker: khoảng 14 USDT.
- Mở taker, đóng maker: khoảng 14 USDT.

Đây chỉ là ví dụ tính phí giao dịch. Giá trị cuối cùng có thể khác nếu vị thế được khớp thành nhiều phần, giá khớp thay đổi hoặc lệnh thuộc nhóm cặp có mức phí riêng.

Đối với futures ký quỹ bằng crypto, công thức sử dụng mệnh giá hợp đồng và giá khớp. Phí cũng được thanh toán bằng tài sản crypto liên quan thay vì nhất thiết bằng USDT. Vì vậy, nên xem dòng phí thực tế trong lịch sử lệnh sau khi giao dịch được khớp.

## Phí funding là gì?

Phí funding áp dụng cho futures vĩnh cửu, loại hợp đồng không có ngày đáo hạn cố định. Mục tiêu của cơ chế này là giúp giá hợp đồng bám sát giá chỉ số của tài sản cơ sở.

Funding không giống phí giao dịch. OKX mô tả đây là khoản được trao đổi trực tiếp giữa người đang giữ vị thế long và short. Khi funding dương, bên long thường trả cho bên short. Khi funding âm, bên short thường trả cho bên long. Khi funding bằng 0, không phát sinh khoản thanh toán funding giữa hai phía.

Công thức cơ bản:

text
Phí funding = Giá trị vị thế × Tỷ lệ funding


Ví dụ, bạn đang giữ vị thế trị giá 10.000 USDT và tỷ lệ funding tại thời điểm thanh toán là 0,01%:

text
10.000 × 0,01% = 1 USDT


Nếu tỷ lệ funding đổi chiều, bên nhận và bên trả cũng có thể thay đổi. Vì vậy, một vị thế có lợi nhuận trên biểu đồ vẫn có thể cho lợi nhuận ròng thấp hơn sau khi trừ funding và phí giao dịch.

Trước khi giữ lệnh qua thời điểm funding, hãy kiểm tra:

- Tỷ lệ funding hiện tại.
- Thời gian còn lại đến lần thanh toán kế tiếp.
- Vị thế của bạn là bên trả hay bên nhận.
- Giá trị danh nghĩa thực tế của vị thế.

## Phí thanh lý và phí thanh toán hợp đồng

Nếu vị thế bị thanh lý bắt buộc, OKX cho biết phí thanh lý được tính theo mức phí taker của cấp hiện tại của tài khoản. Đây là lý do không nên chỉ tính chi phí mở và đóng lệnh rồi bỏ qua rủi ro thanh lý.

Với một số hợp đồng futures kỳ hạn, OKX công bố phí thanh toán hợp đồng ở mức **0,01%** cho mọi cấp người dùng. Điều khoản cụ thể có thể phụ thuộc vào loại hợp đồng và khu vực cung cấp sản phẩm.

Futures kỳ hạn và futures vĩnh cửu cũng khác nhau ở điểm quan trọng:

- Futures vĩnh cửu không có ngày hết hạn cố định và có funding.
- Futures kỳ hạn có thời điểm thanh toán hoặc đáo hạn.
- Chi phí cuối cùng của hợp đồng kỳ hạn có thể bao gồm phí giao dịch và phí thanh toán.
- Sản phẩm nào được cung cấp còn phụ thuộc vào khu vực và điều kiện tài khoản.

## Cách kiểm tra phí futures OKX thực tế trên tài khoản

Mức phí hiển thị công khai chỉ mang tính tham khảo. OKX cho biết mức phí áp dụng cho tài khoản đã đăng nhập có thể khác với phần hiển thị cho khách truy cập chưa đăng nhập.

Bạn có thể kiểm tra theo các bước sau:

1. Đăng nhập vào tài khoản OKX.
2. Mở khu vực tài sản hoặc hồ sơ tài khoản.
3. Chọn phần phí giao dịch của tôi hoặc cấp phí giao dịch.
4. Mở một cặp futures cụ thể.
5. Kiểm tra phí maker và taker ngay trong bảng đặt lệnh.
6. Sau khi lệnh khớp, mở lịch sử lệnh để xem khoản phí thực tế.

Trên ứng dụng, tên menu có thể thay đổi theo phiên bản và khu vực. Nếu không thấy bảng phí, hãy vào khu vực giao dịch futures, mở phần thông tin thêm hoặc quy tắc phí.

Đừng chỉ nhìn tỷ lệ phần trăm. Hãy kiểm tra cả:

- Giá trị danh nghĩa của vị thế.
- Số hợp đồng.
- Loại ký quỹ.
- Giá khớp trung bình.
- Tỷ lệ funding.
- Phí ước tính khi mở và đóng.
- Khoảng cách thanh lý.

## Mã CASH20 có giúp giảm phí futures không?

Liên kết được cung cấp sử dụng mã **CASH20** và được giới thiệu với mức hoàn phí 20%. Bạn có thể bắt đầu từ đây:

[👉 Đăng ký OKX với mã CASH20](https://okx.com/join/CASH20)

Tuy nhiên, mức hoàn hoặc giảm phí từ liên kết giới thiệu không nên hiểu là phí futures cơ bản giảm trực tiếp từ 0,05% xuống một con số cố định trong mọi trường hợp. Cần phân biệt:

- Phí futures gốc theo cấp Regular hoặc VIP.
- Khoản giảm phí dành cho người được mời.
- Khoản hoàn phí nếu chương trình áp dụng cho tài khoản và sản phẩm của bạn.
- Điều kiện khu vực, thời gian, sản phẩm và trạng thái người dùng.
- Việc mã giới thiệu có được gắn thành công trong lúc đăng ký hay không.

Sau khi đăng ký, hãy kiểm tra phần giới thiệu hoặc phí giao dịch trong tài khoản. Nếu mức ưu đãi không hiển thị, không nên mặc định rằng mã đã được áp dụng.

Một điểm cũng cần lưu ý: mã giới thiệu thường cần được gắn khi tạo tài khoản hoặc trong quy trình đăng ký ban đầu. Nếu bạn đã có tài khoản, việc nhập mã sau đó có thể không thay đổi điều kiện phí, tùy theo quy tắc chương trình tại khu vực của bạn.

## Làm thế nào để giảm chi phí futures hợp lý?

### Ưu tiên kiểm soát giá trị vị thế

Vì phí tính trên giá trị danh nghĩa, tăng đòn bẩy có thể khiến chi phí tính trên vốn ký quỹ trông có vẻ nhỏ nhưng vẫn làm phí thực tế tăng theo quy mô vị thế. Đừng dùng đòn bẩy cao chỉ vì thấy số tiền phí trên phần ký quỹ không lớn.

### Hiểu cách lệnh được khớp

Lệnh giới hạn không đảm bảo chắc chắn phí maker. Nếu lệnh khớp ngay, nó có thể bị tính như taker. Khi chiến lược yêu cầu vào lệnh nhanh, phí taker có thể là chi phí hợp lý. Khi không cần khớp ngay, bạn có thể cân nhắc lệnh chờ.

### Tính cả hai chiều giao dịch

Một vị thế futures thường có ít nhất hai lần khớp: mở và đóng. Nếu chỉ tính phí mở, bạn sẽ đánh giá thấp chi phí. Với vị thế giữ lâu, funding có thể quan trọng hơn phí giao dịch ban đầu.

### Kiểm tra funding trước khi giữ lệnh

Funding thay đổi theo thị trường. Một vị thế giữ qua nhiều chu kỳ funding có thể chịu tổng chi phí đáng kể, đặc biệt khi giá trị danh nghĩa lớn.

### Không cố đạt VIP bằng giao dịch dư thừa

OKX cập nhật cấp phí dựa trên tài sản và khối lượng trong 30 ngày. Theo tài liệu hỗ trợ, dữ liệu được chụp vào một thời điểm nhất định và cấp phí được cập nhật theo chu kỳ hằng ngày, không phải thay đổi tức thời sau từng lệnh.

Nếu bạn phải thực hiện nhiều giao dịch không cần thiết để đạt một cấp VIP, rủi ro và phí phát sinh có thể vượt xa phần tiết kiệm.

## Phí futures OKX có rẻ không?

Với tài khoản Regular, mức tham khảo 0,0200% maker và 0,0500% taker là con số dễ dùng để lập dự toán ban đầu. Nhưng đánh giá “rẻ” hay “đắt” còn phụ thuộc vào:

- Bạn chủ yếu dùng maker hay taker.
- Tần suất giao dịch.
- Giá trị danh nghĩa mỗi vị thế.
- Thời gian nắm giữ.
- Tỷ lệ funding.
- Loại hợp đồng và cặp giao dịch.
- Mức trượt giá khi thị trường biến động.
- Cấp phí thực tế của tài khoản.

Nếu bạn chỉ giao dịch thỉnh thoảng, chênh lệch nhỏ giữa các cấp phí có thể không đáng để theo đuổi. Nếu bạn giao dịch với tần suất cao, việc kiểm tra chính xác maker, taker, funding và mức rebate sẽ quan trọng hơn việc nhìn vào một con số quảng cáo riêng lẻ.

Cách thực tế nhất là mở bảng đặt lệnh của đúng cặp futures bạn định giao dịch, kiểm tra tỷ lệ phí trên tài khoản đã đăng nhập, sau đó tính chi phí cho cả lúc mở và đóng vị thế. Mã `CASH20` có thể được sử dụng trong quy trình đăng ký qua liên kết dưới đây, nhưng mức ưu đãi cuối cùng vẫn cần được xác nhận trên tài khoản:

[👉 Kiểm tra ưu đãi đăng ký OKX và phí futures](https://okx.com/join/CASH20)
