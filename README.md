# mua proxy: phân loại IP, giá thật theo GB và theo IP, và cách chọn gói để không bị khóa tài khoản

Người gõ "mua proxy" vào Google thường đang ở một trong ba tình huống: cần thêm IP để nuôi tài khoản, cần IP sạch cho tool cào dữ liệu, hoặc vừa bị khóa một dàn nick và đang tìm chỗ mua khác. Cả ba đều dẫn tới cùng một câu hỏi thực tế: trả bao nhiêu tiền, cho loại IP nào, và làm sao biết nhà cung cấp không bán cho mình một dải IP đã bị đưa vào blacklist từ lâu.

Bài này đi theo đúng thứ tự đó. Phần đầu là cách phân loại proxy và giá thị trường, phần sau là một nhà cung cấp cụ thể — 9Proxy — với bảng giá đầy đủ các gói đang niêm yết, để bạn có mốc so sánh bằng số thật thay vì nghe quảng cáo.

## Trước khi trả tiền: bốn câu hỏi quyết định giá

Giá proxy không nằm ở "proxy đắt hay rẻ". Nó nằm ở bốn lựa chọn bạn phải chốt trước.

**Proxy datacenter hay proxy dân cư.** IP datacenter sinh ra từ máy chủ của các nhà cung cấp cloud, tốc độ cao, giá rẻ, nhưng dải IP công nghiệp này bị Facebook, TikTok hay Amazon nhận ra rất nhanh. Proxy dân cư là IP do nhà mạng hộ gia đình cấp (FPT, Viettel, VNPT ở Việt Nam; AT&T, Comcast ở Mỹ), nên nền tảng nhìn vào thấy một người dùng bình thường đang online. Cái giá phải trả là chi phí cao hơn nhiều lần.

**Proxy tĩnh hay proxy xoay.** IP tĩnh giữ nguyên trong suốt thời gian thuê, phù hợp cho tài khoản chính, shop bán hàng, tài khoản quảng cáo — những thứ cần một "địa chỉ nhà" cố định. Proxy xoay đổi IP theo mỗi request hoặc theo chu kỳ, phù hợp cho cào dữ liệu, đăng ký hàng loạt, chạy tool.

**Proxy riêng hay dùng chung.** IP dùng chung rẻ, nhưng nếu người khác dùng cùng IP đó đi spam thì bạn ăn đạn lây. Với công việc nghiêm túc, đây là khoản tiết kiệm không nên tiết kiệm.

**Giao thức.** HTTP/HTTPS đủ cho lướt web, tool marketing, SEO. SOCKS5 cần khi chạy phần mềm giả lập game, tool chuyên dụng, hoặc các tác vụ cần truyền cả UDP.

Chốt xong bốn điểm này thì giá mới có nghĩa để so sánh. Cùng một nhà cung cấp, gói proxy dân cư xoay theo GB thường rẻ hơn gói IP tĩnh rất nhiều — nhưng hai thứ đó không thay thế được cho nhau.

## Hai cách tính tiền proxy phổ biến trên thị trường

Hầu hết nhà cung cấp proxy dân cư tính tiền theo một trong hai kiểu:

- **Theo GB:** bạn mua một lượng băng thông, dùng hết thì nạp thêm. Rao IP bao nhiêu cũng được, miễn là trong hạn mức GB đã trả tiền.
- **Theo số lượng IP:** bạn mua một số IP cố định, mỗi IP thường đi kèm băng thông không giới hạn trong thời gian nó còn sống.

Kiểu thứ nhất hợp với công việc xoay IP liên tục nhưng mỗi request tốn ít dữ liệu: kiểm tra giá, kiểm tra quảng cáo, kiểm tra hiển thị theo vùng, gọi API. Kiểu thứ hai hợp với phiên làm việc dài, tải dữ liệu nặng, hoặc những việc khó đoán trước sẽ ngốn bao nhiêu băng thông.

Không có kiểu nào rẻ hơn tuyệt đối. Một job cào dữ liệu 200 GB bằng mô hình theo GB sẽ tốn tiền gấp nhiều lần so với việc mua vài chục IP có băng thông không giới hạn — và ngược lại, một job chỉ cần đổi IP liên tục mà mỗi lần tải vài trăm KB thì mua IP theo gói là lãng phí.

## 9Proxy tính tiền thế nào

9Proxy là nhà cung cấp proxy dân cư chạy cả hai mô hình trên cùng một tài khoản: gói theo IP (băng thông không giới hạn) và gói theo GB (tạo endpoint không giới hạn, chỉ trừ dung lượng). Một số thông số đáng ghi lại trước khi xem giá:

- Pool khoảng 20 triệu IP dân cư tại hơn 90 quốc gia
- Nhắm mục tiêu theo quốc gia, thành phố, mã ZIP và ISP
- Hỗ trợ HTTP/HTTPS và SOCKS5
- Cam kết uptime 99,95%, hỗ trợ 24/7
- Chế độ xoay IP và chế độ sticky (giữ IP theo phiên cấu hình)
- Thanh toán bằng thẻ tín dụng, thẻ ngân hàng, crypto (USDT, BTC, ETH, LTC, DOGE), Alipay, Apple Pay, Google Pay

Điểm khác nhau về mặt kỹ thuật giữa hai mô hình khá rõ. Gói theo IP yêu cầu app desktop để forward cổng cục bộ, mỗi IP sống từ vài giờ tới tối đa 24 giờ, băng thông không giới hạn trong thời gian đó, IP không tự xoay nhưng có thể bật xoay tự động trên các cổng chỉ định. Gói theo GB không cần app, thao tác trực tiếp trên dashboard, xác thực bằng username/password hoặc whitelist IP, traffic chạy qua IP dân cư xoay liên tục và bị trừ dần theo dung lượng.

👉 [Xem bảng giá và các gói proxy hiện có của 9Proxy](https://bit.ly/9-Proxy)

## Bảng giá đầy đủ các gói đang niêm yết

### Nhóm gói theo GB

| Gói | Giá mỗi GB | Tổng tiền | Hiệu lực | Link mua |
| --- | --- | --- | --- | --- |
| 5 GB | $3,00 | $15 | 180 ngày | [Mua gói 5 GB](https://bit.ly/9-Proxy) |
| 50 GB + 5 GB | $2,10 | $105 | 180 ngày | [Mua gói 50 GB + 5 GB](https://bit.ly/9-Proxy) |
| 100 GB | $1,50 | $150 | 180 ngày | [Mua gói 100 GB](https://bit.ly/9-Proxy) |
| 200 GB | $1,00 | $200 | 180 ngày | [Mua gói 200 GB](https://bit.ly/9-Proxy) |
| 1.000 GB | $0,80 | $800 | 180 ngày | [Mua gói 1.000 GB](https://bit.ly/9-Proxy) |
| 2.000 GB | $0,75 | $1.500 | 180 ngày | [Mua gói 2.000 GB](https://bit.ly/9-Proxy) |
| 3.000 GB (Enterprise) | $0,72 | $2.160 | Không giới hạn | [Xem gói Enterprise 3.000 GB](https://bit.ly/9-Proxy) |
| 6.000 GB (Enterprise) | $0,70 | $4.200 | Không giới hạn | [Xem gói Enterprise 6.000 GB](https://bit.ly/9-Proxy) |
| 10.000 GB (Enterprise) | $0,68 | $6.800 | Không giới hạn | [Xem gói Enterprise 10.000 GB](https://bit.ly/9-Proxy) |

Con số đáng chú ý nằm ở cột hiệu lực. Các gói từ 5 GB tới 2.000 GB có hạn 180 ngày kể từ lúc mua, nghĩa là dung lượng chưa dùng hết sẽ mất sau mốc đó. Nhóm Enterprise bỏ hẳn giới hạn thời gian, nên nếu bạn làm dự án theo đợt, mua nhiều rồi dùng rải rác trong nhiều tháng thì đây là điểm cần tính vào chi phí thực.

### Nhóm gói theo IP và gói bundle

| Gói | Cấu hình | Giá | Đặc điểm | Link mua |
| --- | --- | --- | --- | --- |
| 100 IP | 100 IP dân cư | $20 ($0,20/IP) | Băng thông không giới hạn, IP dùng đến khi hết | [Mua gói 100 IP](https://bit.ly/9-Proxy) |
| Gói IP số lượng lớn | Từ 500 IP trở lên, có mốc 1.000 IP kèm IP thưởng khi thanh toán bằng crypto | Giá mỗi IP giảm dần theo số lượng, mức sàn 9Proxy công bố là khoảng $0,015/IP | Băng thông không giới hạn | [Xem giá gói IP theo số lượng](https://bit.ly/9-Proxy) |
| Starter Bundle | 100 IP + 5 GB | $30 | Kết hợp IP cố định và traffic xoay | [Mua gói Starter Bundle](https://bit.ly/9-Proxy) |
| Popular Bundle | 1.500 IP + 50 GB | $180 | Cho job vừa cần phiên ổn định vừa cần xoay | [Mua gói Popular Bundle](https://bit.ly/9-Proxy) |
| Pro Bundle | 5.000 IP + 500 GB | $720 | Khối lượng lớn, chạy liên tục | [Mua gói Pro Bundle](https://bit.ly/9-Proxy) |

Hai lưu ý về bảng này. Thứ nhất, giá gói theo IP đã qua nhiều lần điều chỉnh và khác nhau tùy số lượng, nên mức $20 cho 100 IP là con số được ghi nhận ổn định ở gói vào, còn các mốc lớn hơn nên xem trực tiếp trên trang giá thay vì tin vào bảng tổng hợp của bên thứ ba. Thứ hai, vài nguồn cũ vẫn ghi gói Starter Bundle ở mức $25; mức $30 là con số xuất hiện trong các bài đánh giá cập nhật gần đây.

👉 [Tạo tài khoản 9Proxy để xem giá gói theo số lượng IP](https://bit.ly/9-Proxy)

## Chọn gói theo IP hay theo GB: cách quyết định trong một phút

Có một phép thử đơn giản. Nếu bạn không đoán được một job sẽ ngốn bao nhiêu GB, đừng mua gói GB.

Ví dụ cụ thể với bảng giá trên. Job nuôi 50 tài khoản, mỗi tài khoản cần một IP ổn định, dùng vài tiếng mỗi ngày, tải chủ yếu là ảnh và video ngắn — băng thông tiêu hao rất khó lường trước. Gói 100 IP giá $20 với băng thông không giới hạn xử lý việc này mà không cần đếm GB. Ngược lại, nếu bạn chạy script kiểm tra giá sản phẩm trên 5 sàn, mỗi request vài chục KB, số lượng request lớn nhưng tổng dữ liệu nhỏ, thì gói 5 GB giá $15 cho 180 ngày là điểm bắt đầu rẻ hơn hẳn.

Một chi tiết dễ bị bỏ qua: gói theo IP có thời gian sống mỗi IP từ vài giờ tới 24 giờ. Với tác vụ cần IP cố định suốt nhiều ngày cho một tài khoản, bạn nên kiểm tra kỹ cơ chế thay thế và chế độ sticky trước khi mua số lượng lớn. Theo bài đánh giá của iTWire, 9Proxy áp dụng chính sách thay thế IP lỗi với mốc thời gian được nêu ở mức 60 giây, đây là điểm cộng cho các phiên chạy dài.

Còn nếu bạn không chắc mình thuộc nhóm nào, cách rẻ nhất vẫn là mua gói nhỏ nhất, chạy thử 2–3 ngày trên đúng mục tiêu thật, rồi mới quyết định mở rộng.

## Dấu hiệu bạn đang mua phải dải IP bẩn

Đây là phần mà quảng cáo của mọi nhà cung cấp đều giống nhau, còn thực tế thì khác nhau. Vài dấu hiệu đáng để kiểm tra trước khi nạp một khoản tiền lớn.

**Giá thấp bất thường.** Proxy dân cư có chi phí nền thật: nhà cung cấp phải trả cho các ISP và cho người dùng chia sẻ băng thông. Một dải IP dân cư giá vài nghìn đồng một tháng gần như chắc chắn là IP tái sử dụng, đã bị dùng cho spam trước đó.

**Không rõ nguồn IP.** Hỏi thẳng nhà cung cấp lấy IP từ đâu. Câu trả lời hợp lý là từ ứng dụng có người dùng đồng ý chia sẻ băng thông. Nếu họ né câu hỏi, đó là tín hiệu xấu.

**Không cho kiểm tra trước.** Bất kỳ nhà cung cấp nào cũng nên cho bạn xem mẫu IP hoặc mua gói nhỏ để test. Ở 9Proxy, không có bản dùng thử tự động trên website, nhưng theo các kênh cộng đồng mà đội ngũ này duy trì, vẫn có đợt dùng thử số lượng nhỏ cho người dùng mới tùy tình hình IP sẵn có, và bạn cần liên hệ hỗ trợ để xin.

Sau khi có IP trong tay, ba bước kiểm tra nên làm ngay:

1. Dán IP vào công cụ kiểm tra uy tín như IPQualityScore hoặc Scamalytics để xem điểm rủi ro. IP dùng cho công việc nghiêm túc nên có mức rủi ro thấp.
2. Đo ping và tốc độ tải thực tế, đừng tin thông số quảng cáo.
3. Chạy kiểm tra kết nối trên chính nền tảng mục tiêu trước khi nạp vào phần mềm nuôi tài khoản, tránh cảnh tool đang chạy thì gãy IP làm hỏng cả dàn nick.

## Mua proxy của 9Proxy: quy trình và những điểm cần biết trước

Thứ tự thực tế khá ngắn. Bạn tạo tài khoản bằng email, nạp tiền bằng một trong các phương thức được hỗ trợ (thẻ, crypto, ví điện tử), chọn gói theo IP hoặc theo GB, rồi lấy thông tin kết nối từ dashboard.

Với gói theo IP, bước cài app desktop cần làm sớm vì đó là kênh forward cổng để proxy hoạt động. Nếu bạn chạy đa thiết bị hoặc đa máy ảo, đây là điểm cần tính trước: app desktop không thuận tiện bằng extension trình duyệt, và các bài đánh giá độc lập cũng nêu đúng hạn chế này. Với gói theo GB thì ngược lại, mọi thứ chạy từ dashboard, không cần cài gì.

Vài điểm khác nên biết để không kỳ vọng sai:

- **Streaming không phải sở trường.** iTWire ghi nhận 9Proxy vượt được kiểm tra trên các sàn thương mại điện tử nhưng có thể bị phát hiện trên Netflix. Nếu mục tiêu của bạn là xem nội dung theo vùng, đây không phải lựa chọn phù hợp.
- **Pool nhỏ hơn nhóm dẫn đầu.** 20 triệu IP là con số tốt trong phân khúc ngân sách, nhưng vẫn thấp hơn các nhà cung cấp cấp doanh nghiệp có pool hàng trăm triệu IP. Với mục tiêu quá đặc thù về thành phố hoặc ISP, số lượng lựa chọn sẽ mỏng hơn.
- **Không có trial tự động.** Khác với một số đối thủ, 9Proxy không mở sẵn bản dùng thử trên web. Bạn muốn test thì mua gói nhỏ nhất hoặc liên hệ hỗ trợ.
- **Đánh giá bên thứ ba ở mức khá.** Thư mục proxy ProxyLook xếp 9Proxy ở mức 3,9/5, và điểm mạnh được ghi nhận là giá và độ ổn định, không phải tính năng doanh nghiệp.

Về phía ngược lại, cấu trúc giá là điểm đáng chú ý nhất. Mức $0,20/IP ở gói 100 IP, mức sàn công bố $0,015/IP khi mua khối lượng lớn, và mức $0,68/GB ở gói Enterprise là những con số cạnh tranh so với phần lớn thị trường proxy dân cư. Chương trình affiliate của 9Proxy cũng khá rõ ràng: hoa hồng trọn đời tối đa 15%, thanh toán crypto, và người được mời nhận mức giảm 5%.

👉 [Đăng ký 9Proxy để xem gói phù hợp với ngân sách của bạn](https://bit.ly/9-Proxy)

## Câu hỏi thường gặp khi mua proxy

**Mua proxy ở đâu để không bị lừa?**

Chọn nhà cung cấp minh bạch về nguồn IP, có bảng giá công khai, có kênh hỗ trợ trả lời được, và cho bạn mua gói nhỏ để test. Ba tiêu chí này lọc được phần lớn nơi làm ăn chộp giật.

**Proxy dân cư có cần thay kèm trình duyệt antidetect không?**

Nếu bạn chạy nhiều tài khoản trên cùng một máy, có. Proxy đổi IP nhưng dấu vân tay trình duyệt vẫn giữ nguyên, và các nền tảng hiện tại đọc cả hai. Đổi IP mà không tách môi trường trình duyệt thì chỉ giải quyết được một nửa vấn đề.

**Proxy miễn phí dùng tạm được không?**

Không nên, kể cả để test. Proxy free thường bị hàng nghìn người dùng chung, tốc độ rất chậm, và có nguy cơ bị gắn mã độc để lấy thông tin đăng nhập. Số tiền tiết kiệm được không bù nổi rủi ro mất tài khoản.

**Nên mua IPv4 hay IPv6?**

IPv4 tương thích với gần như mọi nền tảng. IPv6 rẻ hơn nhưng nhiều trang lớn vẫn chưa hỗ trợ hoặc chặn khá gắt. Nếu bạn nuôi tài khoản, chọn IPv4.

**Mua ít trước có bị tính giá cao hơn nhiều không?**

Có chênh, nhưng không đáng để mạo hiểm. Chênh lệch giữa gói 100 IP và gói khối lượng lớn tính trên vài chục đô đầu tiên luôn nhỏ hơn thiệt hại của một dàn tài khoản bị khóa vì dùng dải IP kém chất lượng.

**9Proxy có cho dùng thử không?**

Theo thông tin trên các kênh cộng đồng của 9Proxy, đợt dùng thử số lượng nhỏ dành cho người dùng mới vẫn có nhưng tùy tình hình IP sẵn có, và bạn phải liên hệ hỗ trợ để hỏi. Trên website không có nút dùng thử tự động.

## Chốt lại

Câu hỏi "mua proxy" thực ra gồm ba quyết định tách biệt: chọn loại IP theo mục tiêu công việc, chọn cách tính tiền theo kiểu sử dụng, rồi mới chọn nhà cung cấp. Làm ngược lại — chọn nhà cung cấp trước rồi mới xem loại IP — là cách nhanh nhất để trả tiền cho thứ mình không cần.

Với 9Proxy, điểm mạnh nằm ở giá và ở việc có sẵn cả hai mô hình tính tiền trên cùng một tài khoản: gói theo IP với băng thông không giới hạn cho công việc cần IP ổn định, gói theo GB cho công việc cần xoay liên tục với dung lượng nhỏ. Điểm cần cân nhắc là không có bản dùng thử tự động, app desktop bắt buộc với gói theo IP, và pool 20 triệu IP tuy đủ rộng cho hầu hết nhu cầu nhưng không so được với các nhà cung cấp cấp doanh nghiệp về độ chi tiết nhắm mục tiêu.

Nếu vẫn đang phân vân giữa hai mô hình, hãy bắt đầu từ gói nhỏ nhất ở cả hai hướng, chạy thử trên đúng nền tảng bạn cần, rồi mở rộng ở hướng nào cho kết quả ổn định hơn.

👉 [Bắt đầu với gói proxy nhỏ nhất của 9Proxy](https://bit.ly/9-Proxy)
