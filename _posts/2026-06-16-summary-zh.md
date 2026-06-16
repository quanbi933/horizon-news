---
layout: default
title: "Horizon Summary: 2026-06-16 (ZH)"
date: 2026-06-16
lang: zh
---

> Đã chọn 8 tin quan trọng từ 18 nội dung.

---

1. [Phát hành vLLM v0.23.0 với sự thành 熟 của DeepSeek-V4 và mở rộng Model Runner V2](#item-1) ⭐️ 8.0/10
2. [Mã độc trong công việc LinkedIn qua kho GitHub bị compromet](#item-2) ⭐️ 8.0/10
3. [Iroh 1.0 phát hành bộ kết nối peer-to-peer với transport tùy chỉnh](#item-3) ⭐️ 8.0/10
4. [Ask HN: Có ai đã thay thế Claude/GPT bằng mô hình địa phương để lập trình hàng ngày không?](#item-4) ⭐️ 8.0/10
5. [Hacker biến bóng đèn Wi‑Fi thành máy chủ ẩn chứa sách cấm](#item-5) ⭐️ 7.0/10
6. [Evalatro: một benchmark mở nơi các LLM chơi Balatro thật](#item-6) ⭐️ 7.0/10
7. [TinyWind: Trò chơi phiêu lưu hải tặc pixel-art với mô phỏng gió thực](#item-7) ⭐️ 6.0/10
8. [Qwable-v1: Mô hình Qwen3.6-35B-A3B mã nguồn mở được tinh chế từ Claude Fable-5](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Phát hành vLLM v0.23.0 với sự thành 熟 của DeepSeek-V4 và mở rộng Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

Phiên bản vLLM v0.23.0 được phát hành với 408 commits từ 200 nhà đóng góp, bao gồm 63 người mới. Nó làm thành 熟 hỗ trợ DeepSeek-V4 trên các backend, mở rộng Model Runner V2 cho các model dense Llama và Mistral, thêm tính năng frontend Rust, hỗ trợ Gemma 4, tương thích Transformers v5, offloading KV cache đa cấp, trình phân tích thống nhất và một số model mới. Các cập nhật này cải thiện hiệu suất, tính tương thích và khả năng sử dụng cho các mô hình ngôn ngữ lớn tiên tiến, đặc biệt là DeepSeek‑V4 và các họ Llama/Mistral phổ biến. Đồng thời, chúng tiến bộ kiến trúc mô-đun của vLLM, giúp nhà phát triển dễ dàng áp dụng các model mới và phần cứng backend. DeepSeek‑V4 đã nhận được kernel attention TRTLLM‑gen, hỗ trợ EPLB cho Mega‑MoE, giữ lại prefix‑cache chọn lọc, tính năng index‑share cho DSA MTP, được tách khỏi torch.compile, và có đường dẫn decode attention XPU. Model Runner V2 hiện là runner mặc định cho các model dense Llama và Mistral, có bộ lấy mẫu FlashInfer, đồ thị CUDA có thể ngắt, loại bỏ bong bóng pipeline‑song song, hỗ trợ kích thước block kernel cho model lai, MTP Gemma 4; frontend Rust thêm endpoint generate streaming, dynamic LoRA, version/server_info; và offloading KV cache đa cấp đã tăng lớp thứ hai object‑store, bật HMA mặc định và cho phép chính sách offloading mỗi request.

github · khluu · 15/6 05:27

**Bối cảnh**: vLLM là một thư viện suy luận mô hình ngôn ngữ lớn với throughput cao, tối ưu việc sử dụng bộ nhớ và thực thi kernel để phục vụ các mô hình lớn một cách hiệu quả. Model Runner V2 là việc thiết kế lại nhân thực thi lõi của vLLM, được ra mắt để giảm nợ kỹ thuật và nâng cao tính mô-đun, hiệu suất cũng như hỗ trợ các tính năng lấy mẫu mới và CUDA. DeepSeek‑V4 là một mô hình ngôn ngữ Mixture‑of‑Experts sắp ra mắt từ DeepSeek, được công bố vào năm 2026 với tới 1,6 nghìn tỷ tham số và các chế độ suy nghĩ và không suy nghĩ nâng cao. Transformers v5 là bản phát hành chính lớn mới nhất của thư viện Hugging Face Transformers, mà vLLM hiện tại nhắm tới để đảm bảo sự tương thích với các bộ tokenizer và bộ xử lý model mới hơn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V4 (2026) — 1T Params, Benchmarks & Pricing</a></li>

</ul>
</details>

**Thẻ**: `#vLLM`, `#LLM inference`, `#DeepSeek-V4`, `#Model Runner V2`, `#release`

---

<a id="item-2"></a>
## [Mã độc trong công việc LinkedIn qua kho GitHub bị compromet](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 8.0/10

Một người tuyển dụng LinkedIn làm giài thủ crypto startup, chia sẻ một kho GitHub công khai chứa mã độc ẩn sau, được thực thi qua script prepare của npm khi cài đặt dependencies. Điều này cho thấy các nền tảng chuyên nghiệp có thể bị wykorzyst để thực hiện các cuộc tấn công chuỗi cung ứng, đặt nhà phát triển dưới nguy cơ mất thông tin đăng nhập và thực thi mã từ xa. Payload độc hại được giấu trong các tệp test bị chú thích và được kích hoạt tự động bởi script prepare của npm trong quá trình npm install, không cần thao tác bổ sung từ người dùng.

hackernews · lwhsiao · 15/6 20:00 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48546294)

**Bối cảnh**: Các script vòng đời của npm như prepare được thực thi tự động sau khi chạy npm install, cho phép các gói chạy mã任意 mà không cần sự đồng ý rõ ràng của người dùng. Các kẻ tấn công lạm dụng tính năng này để nhúng mã độc vào các kho chứa có vẻ hợp pháp. Các lừa đảo việc làm trên LinkedIn thường bao gồm những người tuyển dụng giả mạo chia sẻ nhiệm vụ lập trình hoặc kho chứa để dụ développeurs chạy mã độc. Việc hiểu các cơ chế này giúp nhà phát triển nhận diện và tránh được các cuộc tấn công xã hội học.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://docs.npmjs.com/cli/v8/using-npm/scripts/">How npm handles the " scripts " field</a></li>
<li><a href="https://thecybersecguru.com/news/atomic-arch-aur-supply-chain-attack-ebpf-rootkit/">Atomic Arch: 900+ AUR Packages Backdoored... | The CyberSec Guru</a></li>
<li><a href="https://dev.to/xanderselorm/fake-job-offers-are-turning-github-repos-into-a-trap-5fad">Fake Job Offers Are Turning GitHub Repos Into a Trap</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận cho thấy sự lo ngại về mức độ phổ biến của lừa đảo này, nhấn mạnh rằng các cuộc tấn công tương tự đã xảy ra trong hai năm qua mà LinkedIn và GitHub ít có hành động. Nhiều người gọi ra cần có kênh báo cáo tốt hơn và phòng thủ có tổ chức chống lại tội phạm mạng, đồng thời nhắc nhở mọi người phải cảnh giác khi kiểm tra các kho mã không được yêu cầu.

**Thẻ**: `#security`, `#social-engineering`, `#npm`, `#LinkedIn`, `#job-scams`

---

<a id="item-3"></a>
## [Iroh 1.0 phát hành bộ kết nối peer-to-peer với transport tùy chỉnh](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 đã được phát hành, đưa ra một bộ kết nối peer-to-peer cho phép các ứng dụng kết nối trực tiếp qua máy chủ relay và transport do người dùng tự định nghĩa. Nhờ trừu tượng hoá lớp transport, Iroh đơn giản hoá việc xây dựng ứng dụng phân tán, loại bỏ nhu cầu người dùng quản lý tài khoản mạng bên ngoài như Tailscale và cho phép nhà phát triển nhúng kết nối P2P trực tiếp vào ứng dụng của họ. Iroh 1.0 bao gồm transport IPv4, IPv6 và relay mặc định, đồng thời cung cấp giao diện pluggable để triển khai transport tùy chỉnh như WebRTC hoặc BLE; nó sử dụng gói pkarr mã hóa khóa công khai để trao đổi thông tin kết nối, được viết bằng Rust và là mã nguồn mở.

hackernews · chadfowler · 15/6 15:13 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48542480)

**Bối cảnh**: Mạng peer-to-peer (P2P) là kiến trúc phân tán trong đó các nút chia sẻ tài nguyên và giao tiếp trực tiếp mà không cần máy chủ trung tâm. Máy chủ relay hoạt động như trung gian giúp các nút vượt qua NAT và tường lửa khi kết nối trực tiếp không thể thực hiện. Iroh áp dụng mô hình này bằng cách cung cấp một lớp trừu tượng transport cho phép ứng dụng chọn giữa transport relay nội bộ hoặc transport tùy chỉnh cho kết nối của chúng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Peer-to-peer">Peer - to - peer - Wikipedia</a></li>
<li><a href="https://docs.edgegap.com/learn/distributed-relay">Relays (P2P) | Edgegap Docs</a></li>
<li><a href="https://www.iroh.computer/">Iroh</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận thường so sánh Iroh với Tailscale nhưng đặt ở lớp ứng dụng, khen ngợi khả năng mở rộng transport tùy chỉnh đồng thời hỏi cần giải thích rõ hơn về các khóa mã hoá dùng để xác định đối tác. Một số người đặt câu hỏi về nhu cầu của một lớp mạng P2P khác khi đã có IP, IPv6 và QUIC, trong khi những người khác chào đón bước tiến hướng tới mạng phi tập trung, tự lưu trữ.

**Thẻ**: `#peer-to-peer`, `#networking`, `#Iroh`, `#release`, `#distributed systems`

---

<a id="item-4"></a>
## [Ask HN: Có ai đã thay thế Claude/GPT bằng mô hình địa phương để lập trình hàng ngày không?](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

Trong một bài đăng Ask HN, các nhà phát triển chia sẻ kinh nghiệm thay thế các trợ lý lập trình đám mây như Claude/GPT bằng các mô hình địa phương như Qwen và Gemma, bao gồm phần cứng, lựa chọn mô hình, hiệu suất và động lực.

hackernews · cloudking · 15/6 14:46

**Thẻ**: `#LLM`, `#local AI`, `#coding assistants`, `#privacy`, `#HN discussion`

---

<a id="item-5"></a>
## [Hacker biến bóng đèn Wi‑Fi thành máy chủ ẩn chứa sách cấm](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 7.0/10

Một người làm việc với phần cứng đã sửa đổi một bóng đèn thông minh Wi‑Fi để chạy một máy chủ web địa phương, lưu trữ bộ sưu tập các file EPUB của sách bị cấm, tạo thành một điểm thả thông tin ẩn có thể truy cập qua mạng Wi‑Fi của bóng đèn. Dự án này chứng minh rằng các thiết bị IoT giá rẻ có thể được tái sử dụng để vượt qua kiểm duyệt và bảo vệ tự do ngôn luận, nhấn mạnh xu hướng ngày càng tăng sử dụng thiết bị hàng ngày để chia sẻ thông tin ẩn. Nó cũng nâng cao nhận thức về các tác động bảo mật khi các thiết bị nhà thông minh được sử dụng làm kênh truyền thông ẩn. Vi điều khiển ESP8266/ESP32 của bóng đèn được ghi đè firmware tùy chỉnh (ví dụ qua Tasmotizer) để hoạt động như một điểm truy cập Wi‑Fi và máy chủ web mà vẫn duy trì chức năng chiếu sáng bình thường. Bộ nhớ lưu trữ bị giới hạn bằng flash của bóng đèn, chỉ cho phép lưu trữ một số tập tin EPUB nhỏ, và việc truy cập yêu cầu sự gần với tín hiệu Wi‑Fi của bóng đèn.

hackernews · sohkamyung · 15/6 22:37 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48547985)

**Bối cảnh**: Các bóng đèn thông minh dựa trên chip ESP8266 hoặc ESP32 có thể được lập lại firmware tùy chỉnh để chạy các dịch vụ bổ sung như máy chủ web, một quá trình được hỗ trợ bởi công cụ như Tasmotizer. Nghiên cứu đã chỉ ra rằng các thiết bị này cũng có thể bị khai thác để tạo ra các kênh truyền thông ẩn qua việc điều chỉnh ánh sáng hoặc tín hiệu điện, gây ra những lo ngại về bảo mật trong các triển khai IoT. Trong bối cảnh kiểm duyệt, việc tái sử dụng những bóng đèn này như máy chủ web ẩn cung cấp một phương pháp thấp chi phí để phân phối tài liệu bị cấm mà vẫn xuất hiện như các vật dụng gia đình thông thường.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://admantium.medium.com/tasmotizer-try-to-flash-a-wifi-led-light-with-a-custom-firmware-e9f0baed3bca">Tasmotizer: Try to Flash a WiFi LED Light with a Custom Firmware</a></li>
<li><a href="https://arxiv.org/abs/2408.14613">[2408.14613] Security Concerns in IoT Light Bulbs ... Covert Data Exfiltration Using Light and Power Channels Security Concerns in IoT Light Bulbs: Investigating Covert ... Security Concerns in IoT Light Bulbs: Investigating Covert ... GitHub - hak5peaks/Hackers-Nightlight: Turning smart lights ... The Dark Side of Smart Lighting: Check Point Research Shows ...</a></li>
<li><a href="https://ieeexplore.ieee.org/document/8988623">Covert Data Exfiltration Using Light and Power Channels</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận đã khen ngợi sự sáng tạo của dự án và bài viết chi tiết, chỉ ra rằng nó liên quan đến các cuộc tranh luận đang diễn ra về tự do ngôn luận và kiểm duyệt. Một số người so sánh với các dự án trước như PirateBox và đề xuất mở rộng ý tưởng thành mạng lưới sử dụng đèn năng lượng mặt trời hoặc thiết bị tương tự. Một số người bày tỏ lo ngại về khả năng lạm dụng nếu được phép tải lên tệp từ người dùng, trong khi những người khác thể hiện sự hứng thú khi thấy ý tưởng được phát triển hơn.

**Thẻ**: `#IoT`, `#censorship`, `#hack`, `#banned books`, `#smart light bulb`

---

<a id="item-6"></a>
## [Evalatro: một benchmark mở nơi các LLM chơi Balatro thật](https://www.reddit.com/r/LocalLLaMA/comments/1u6qso1/evalatro_an_open_benchmark_where_llms_play_the/) ⭐️ 7.0/10

Evalatro là một benchmark mở cho phép các LLM chơi thật trò chơi bài Balatro bằng cách nhận trạng thái trò chơi dưới dạng văn bản và gửi kết quả chạy lên bảng xếp hạng công khai, có thể xác minh. Nó cung cấp một môi trường có thể tái tạo và được chấm điểm bởi máy chủ để kiểm tra khả năng suy luận và lập kế hoạch của LLM trong một trò chơi phức tạp, đồng thời cung cấp bảng xếp hạng công khai để so sánh minh bạch các mô hình. Evalatro sử dụng 种子固定（fixed seeds） để đảm bảo khả năng tái tạo, tích hợp trò chơi Balatro thật với mod Steamodded và công cụ balatrobot, tính điểm trên máy chủ để ngăn chặn việc làm giả, và đặt mục tiêu là vượt qua Ante 12; công cụ tự động cài đặt trên Windows/macOS và cung cấp bảng điều khiển mã nguồn mở tại evalatro.dev.

reddit · r/LocalLLaMA · /u/awfulalexey · 15/6 19:32

**Bối cảnh**: Balatro là một trò chơi Roguelike đơn người xây dựng bộ bài dựa trên poker, trong đó người chơi tiến bộ qua các ante, mỗi ante gồm ba blind có độ khó tăng dần. Các mô hình ngôn ngữ lớn (LLM) là hệ thống AI sinh ra văn bản và có thể được nhắc đưa ra quyết định trong môi trường trò chơi. Các benchmark như Evalatro cung cấp các nhiệm vụ tiêu chuẩn để đo lường và so sánh khả năng suy luận, lập kế hoạch và thích nghi của LLM.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Balatro">Balatro - Wikipedia</a></li>
<li><a href="https://store.steampowered.com/app/2379780/Balatro/">Balatro on Steam Balatro Wiki Balatro | Balatro Wiki | Fandom Game: Balatro Balatro game - Play online in browser for free</a></li>

</ul>
</details>

**Thẻ**: `#LLMs`, `#benchmark`, `#Balatro`, `#AI evaluation`, `#open-source`

---

<a id="item-7"></a>
## [TinyWind: Trò chơi phiêu lưu hải tặc pixel-art với mô phỏng gió thực](https://tinywind.io/) ⭐️ 6.0/10

TinyWind, một trò chơi phiêu lưu hải tặc pixel-art chạy trên trình duyệt, đã được phát hành với một động cơ vật lý mô phỏng lực gió thực, và các gioc thủ đã sailed hơn 380.000 km đồng thời cung cấp phản hồi trên Hacker News. Trò chơi chứng minh rằng có thể đạt được mô phỏng gió thực trong các trò chơi 2D nhẹ, chạy trên trình duyệt, cung cấp cho các nhà phát triển indie một ví dụ thực tế về cơ chế lái thuyền sâu lắng. Thảo luận trên Hacker News cho thấy sự nhiệt huyết cùng với phản hồi xây dựng, giúp định hướng cải tiến và truyền cảm hứng cho các tựa game indie tập trung vào vật lý tương tự. TinyWind sử dụng hệ thống hạt đơn giản để minh họa gió, cho phép người chơi điều chỉnh góc thuyền và lái, nhưng các đánh giá cho thấy hướng gió khó nhận biết và việc điều chỉnh buồm cảm thấy không phản hồi, khiến lái ngược gió giống như có động cơ. Trò chơi miễn phí trên trình duyệt, đã ghi nhận hơn 380.000 km được lái và duy trì khoảng 245 thuyền trưởng hoạt động, trong khi độ khó tăng cao do mục tiêu của địch bắn chính xác và hiếm khi tìm thấy vật phẩm hồi máu.

hackernews · tinywind · 15/6 16:15 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48543475)

**Bối cảnh**: Mô phỏng gió trong trò chơi 2D thường bao gồm việc áp dụng lực lên các đối tượng dựa trên vector gió và sử dụng hệ thống hạt để trực quan hóa dòng chảy, như được minh họa trong hướng dẫn Physics Wind 2D. Các phương pháp nâng cao thường mượn từ động lực học chất tính toán, sử dụng các giải pháp nhanh như thuật toán chất thực thời của Jos Stam để tạo ra các hiệu ứng gió và khói tương tác. Các nhà phát triển indie thường áp dụng những kỹ thuật này để tăng độ sâu lắng cho các thể loại niche như lái thuyền, dù mô phỏng chất đầy đủ vẫn tốn kém về tính toán.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://psychoflowstudio.com/blog/physicswind2d/">Physics Wind 2D is Avaiable!</a></li>
<li><a href="https://www.cs.cmu.edu/afs/cs/academic/class/15462-s13/www/lec_slides/StamFluidforGames.pdf">Real-Time Fluid Dynamics for Games Jos Stam Alias | wavefront</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những người bình luận đã khen ngọt ngọt phong cách pixel art và sự mới lạ của vật lý gió thực, nhưng nhiều người cũng chỉ ra rằng hướng gió không rõ ràng, điều khiển buồm cảm thấy không phản hồi, và độ khó của trò chơi cao quá mức do mục tiêu của địch bắn chính xác và vật phẩm hồi máu hiếm. Một số người dùng đề xuất cải thiện như chỉ báo gió rõ ràng hơn, phân 离 điều khiển buồm và lái, cho phép điều chỉnh độ khó, và thêm cơ chế lái thuyền sâu hơn như tacking và phạt khi lái ngược gió.

**Thẻ**: `#game-development`, `#physics-simulation`, `#indie-games`, `#sailing`, `#hackernews`

---

<a id="item-8"></a>
## [Qwable-v1: Mô hình Qwen3.6-35B-A3B mã nguồn mở được tinh chế từ Claude Fable-5](https://www.reddit.com/r/LocalLLaMA/comments/1u6zj79/claude_fable_5_distilled/) ⭐️ 6.0/10

Tác giả công bố Qwable-v1, mô hình Qwen3.6-35B-A3B mã nguồn mở được tinh chế từ Claude Fable-5, phát hành mô hình, GGUFs và bộ dữ liệu huấn luyện trên Hugging Face dưới giấy phép AGPL-3.0. Điều này cung cấp lần đầu tiên một mô hình trọng lượng mở tái tạo một mô hình độc quyền mạnh mẽ nhưng chỉ tồn tại ngắn hạn, cho phép các nhà nghiên cứu nghiên cứu và phát triển dựa trên khả năng mã hóa tác động của nó mặc dù Anthropic đã ngừng truy cập do lệnh xuất khẩu. Nó cũng nhấn mạnh sự căng thẳng liên tục giữa việc tinh chế mô hình và các biện pháp chống tinh chế. Qwable-v1 được tinh chế từ 4.659 vết dấu mã hóa tác động rõ ràng của Claude Fable-5 lên Qwen3.6 trong khoảng 14 giờ trên một GPU H200, giữ lại đầu ra XML sử dụng công cụ như str_replace_editor. Bản phát hành bao gồm các định lượng GGUF IQ4_XS, Q4_K_M, Q5_K_M, Q8_0 và bộ dữ liệu SFT, tất cả đều được cấp phép AGPL-3.0.

reddit · r/LocalLLaMA · /u/Anony6666 · 16/6 01:21

**Bối cảnh**: Claude Fable-5 là mô hình mạnh nhất mà Anthropic đã phát hành công khai vào ngày 9 tháng 6 năm 2026, đạt 80,3% trên SWE-bench Pro và có bộ phân loại chống tinh chế loại bỏ chuỗi suy nghĩ trong API. Nó bị ngừng truy cập toàn cầu vào ngày 12 tháng 6 năm 2026 do lệnh xuất khẩu của Mỹ, do đó chỉ có sẵn khoảng bốn ngày. GGUF là định dạng lưu trữ các mô hình ngôn ngữ lớn đã được lượng tử hoá, với các biến thể như IQ4_XS và Q4_K_M biểu thị các trade-off khác nhau giữa kích thước, tốc độ và độ chính xác.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://kaitchup.substack.com/p/choosing-a-gguf-model-k-quants-i">Choosing a GGUF Model: K-Quants, IQ Variants, and Legacy Formats</a></li>

</ul>
</details>

**Thẻ**: `#LLM distillation`, `#Claude Fable-5`, `#open-weight models`, `#Qwen3`, `#agentic coding`

---