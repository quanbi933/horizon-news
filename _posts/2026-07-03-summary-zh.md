---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> Đã chọn 13 tin quan trọng từ 15 nội dung.

---

1. [An American Privacy Emergency](#item-1) ⭐️ 9.0/10
2. [Virginia cấm bán dữ liệu vị trí chính xác trong bán dặm 1,750 feet](#item-2) ⭐️ 8.0/10
3. [Hồi quy Linux 6.9 để lại khóa mã hóa LUKS trong bộ nhớ sau khi tạm dừng](#item-3) ⭐️ 8.0/10
4. [Thảo luận trên Hacker News về tác động của Exapunks đến việc học assembly](#item-4) ⭐️ 8.0/10
5. [Podman v6.0.0 ra mắt với mạng nâng cao và tính năng Quadlet](#item-5) ⭐️ 8.0/10
6. [Patch CUDA cho phép DeepSeek V4 Flash chạy bối cảnh 1M token trên RTX 5090](#item-6) ⭐️ 8.0/10
7. [PeerTube: Nền tảng video miễn phí, phi tập trung và liên kết thay thế YouTube](#item-7) ⭐️ 7.0/10
8. [Nhà nghiên cứu AI cao cấp tại Nvidia nghi ngờ AGI, khuyên mô hình open-source tùy chỉnh](#item-8) ⭐️ 7.0/10
9. [Sử dụng DSPy để đánh giá và cải thiện các system prompt SQL của Datasette Agent](#item-9) ⭐️ 6.0/10
10. [Thử nghiệm trợ lý głos nguồn mở kết hợp Parakeet, Gemma 4 31B, Qwen3TTS.](#item-10) ⭐️ 6.0/10
11. [CEO Palantir chỉ trích mô hình AI đóng, anuncia mua chip Nvidia](#item-11) ⭐️ 6.0/10
12. [Mã nguồn Kimi K2.7 hiện có sẵn trong GitHub Copilot](#item-12) ⭐️ 6.0/10
13. [Kế hoạch xây dựng lại Gemma 4 31b với các lớp attention được sửa đổi](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [An American Privacy Emergency](https://scottaaronson.blog/?p=9902) ⭐️ 9.0/10

A U.S. Commerce Department directive prohibits differential privacy and noise infusion techniques in Census Bureau data releases, raising alarms about weakened privacy protections.

hackernews · flowercalled · 3/7 00:01 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48768992)

**Thẻ**: `#privacy`, `#differential-privacy`, `#census`, `#data-protection`, `#policy`

---

<a id="item-2"></a>
## [Virginia cấm bán dữ liệu vị trí chính xác trong bán dặm 1,750 feet](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Ngày 13/4/2026, Chủ tịch Virginia Abigail Spanberger đã ký SB 338 thành luật, sửa đổi Luật Bảo vệ Dữ liệu Người tiêu dùng Virginia để cấm bán dữ liệu vị trí chính xác của người tiêu dùng có thể xác định vị trí người trong bán kính 1.750 feet, có hiệu lực từ ngày 1/7/2026. Cấm này giải quyết những lo ngại về quyền riêng tư liên quan đến việc theo dõi vị trí chi tiết, khiến Virginia trở thành bang thứ ba hạn chế việc bán solche dữ liệu và có thể ảnh hưởng đến tiêu chuẩn bảo vệ dữ liệu quốc gia. Luật định nghĩa dữ liệu vị trí chính xác là dữ liệu từ GPS, trạm cơ sở, Wi‑Fi hoặc Bluetooth xác định vị trí trong bán kính 1.750 feet, đồng thời vẫn cho phép bán dữ liệu vị trí không chính xác hoặc được tổng hợp.

hackernews · toomuchtodo · 2/7 21:03 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48767347)

**Bối cảnh**: Luật Bảo vệ Dữ liệu Người tiêu dùng Virginia (VCDPA) trước đây đã xem dữ liệu vị trí là thông tin nhạy cảm, yêu cầu sự đồng ý chọn vào trước khi xử lý. Tháng 4/2026, Virginia đã sửa đổi VCDPA để cấm eindeutig bán dữ liệu vị trí chính xác, trở thành bang thứ ba sau California và Colorado áp dụng hạn chế như vậy. Quy định này phản xu hướng pháp luật bảo mật tại cấp bang nhằm kiểm soát việc theo dõi vị trí độ phân giải cao.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.regulatoryoversight.com/2026/04/virginia-becomes-third-state-to-ban-sale-of-consumers-precise-geolocation-data/">Virginia Becomes Third State to Ban Sale of Consumers' Precise ...</a></li>
<li><a href="https://newmedialaw.proskauer.com/2026/04/15/virginia-expands-vcdpa-with-ban-on-sale-of-precise-consumer-geolocation-data/">Virginia Expands VCDPA with Ban on Sale of Precise Consumer Geolocation ...</a></li>
<li><a href="https://stateofsurveillance.org/news/virginia-bans-geolocation-data-sales-sb338-privacy-2026/">Virginia Just Banned the Sale of Your Location Data</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận chào đón luật này là bước tiến nhưng cảnh báo rằng các công ty có thể tránh luật bằng cách chỉ bán dữ liệu vị trí không chính xác hoặc đã được tổng hợp. Họ cũng chỉ ra khó khăn trong việc thi hành, đặc biệt đối với các công ty ngoài bang, và dẫn chứng các trường hợp lạm dụng như việc theo dõi lượt đến các cơ sở Planning Parenthood để chạy quảng cáo chống phá thai có mục tiêu.

**Thẻ**: `#privacy`, `#legislation`, `#geolocation`, `#data protection`, `#Virginia law`

---

<a id="item-3"></a>
## [Hồi quy Linux 6.9 để lại khóa mã hóa LUKS trong bộ nhớ sau khi tạm dừng](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Từ phiên bản nhân Linux 6.9, thao tác tạm dừng LUKS không còn xóa khóa mã hóa đĩa khỏi RAM, để lại khóa trong bộ nhớ sau khi thức lại. Hồi quy này để lộ khóa mã hóa trước các cuộc tấn công cold‑boot hoặc DMA, làm giảm mức độ bảo mật của mã hóa đĩa đầy đủ trên laptop và các thiết bị sử dụng tạm dừng/resume. Lỗi này xuất phát từ sự thay đổi trong đường dọn dẹp crypto của nhân, bỏ qua lệnh gọi bước xóa khóa của cryptsetup luksSuspend, ảnh hưởng đến các bản phân phối kích hoạt tính năng tạm dừng LUKS (ví dụ Debian, NixOS).

hackernews · IngoBlechschmid · 2/7 15:25 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48763035)

**Bối cảnh**: LUKS (Linux Unified Key Setup) là định dạng mã hóa đĩa tiêu chuẩn cho Linux, lưu trữ khóa chính trong bộ nhớ nhân khi volume được kích hoạt. Khi hệ thống tạm dừng vào RAM, thao tác tạm dừng LUKS được thiết kế để xóa khóa chính khỏi bộ nhớ nhằm ngăn chặn các cuộc tấn công cold‑boot. Trước phiên bản Linux 6.9, đường dẫn tạm dừng của nhân đã chính xác gọi bước xóa khóa, nhưng một hồi quy đã loại bỏ việc gọi này.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://man.archlinux.org/man/cryptsetup-luksSuspend.8.en">cryptsetup-luksSuspend(8) — Arch manual pages</a></li>
<li><a href="https://discuss.privacyguides.net/t/since-linux-6-9-luks-suspend-stopped-wiping-disk-encryption-keys-from-memory/38949">Since Linux 6.9, LUKS suspend stopped wiping disk-encryption keys from memory - General - Privacy Guides Community</a></li>
<li><a href="https://en.wikipedia.org/wiki/Linux_Unified_Key_Setup">Linux Unified Key Setup - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận viênแสดง phản ứng đa dạng, một số đặt câu hỏi về mức độ nghiêm trọng và phạm vi của hồi quy trong khi một số khác nhấn mạnh rủi ro thực sự của việc lộ khóa trong quá trình tạm dừng. Nhiều người nhận ra rằng vấn đề主要 ảnh hưởng đến các bản phân phối kích hoạt tính năng tạm dừng LUKS, và họ đánh giá cao việc bổ sung các test để ngăn ngừa hồi quy. Một số người dùng còn speculation về ý định độc hại, mặc dù đa số cho rằng đây là một lỗi không intentional.

**Thẻ**: `#Linux`, `#LUKS`, `#disk encryption`, `#security`, `#kernel regression`

---

<a id="item-4"></a>
## [Thảo luận trên Hacker News về tác động của Exapunks đến việc học assembly](https://www.zachtronics.com/exapunks/) ⭐️ 8.0/10

Người dùng Hacker News gần đây đã thảo luận về trò chơi puzzle lập trình Exapunks, chia sẻ câu chuyện cá nhân về cách trò chơi đã nâng cao hiểu biết của họ về ngôn ngữ assembly và kỹ năng lập trình. Thảo luận này nhấn mạnh giá trị giáo dục của các trò chơi Zachtronics, cho thấy trải nghiệm dễ tiếp cận và vui chơi có thể làm sáng tỏ lập trình thấp cấp cho mọi người. Exapunks được phát hành phiên bản truy cập sớm vào ngày 9 tháng 8 năm 2018 và chính thức vào ngày 22 tháng 10 năm 2018 bởi Zachtronics, bao gồm máy cầm tay imaginary Redshift và một ngôn ngữ giống assembly để giải quyết các câu đố.

hackernews · yu3zhou4 · 2/7 18:41 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48765663)

**Bối cảnh**: Zachtronics là nhà phát triển game độc lập nổi tiếng với các trò chơi puzzle tập trung vào lập trình như TIS-100, SHENZHEN I/O và Opus Magnum. Ngôn ngữ assembly là ngôn ngữ lập trình cấp thấp gần với mã máy của máy tính, thường được coi là khó học. Exapunks sử dụng một ngôn ngữ assembly-like giả định để giảng dạy những khái niệm này qua các câu đố mở và một console cầm tay có thể chia sẻ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Exapunks">Exapunks - Wikipedia</a></li>
<li><a href="https://thinkygames.com/games/exapunks/">Exapunks · Thinky Games</a></li>
<li><a href="https://www.zachtronics.com/exapunks/">EXAPUNKS - Zachtronics</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận cho rằng Exapunks đã tăng cường sự tự tin của họ về assembly và lập trình thấp cấp, cho thấy trò chơi dạy họ giải quyết câu đố trước khi tối ưu hóa. Họ cũng nhấn mạnh khía cạnh xã hội, đề nghị chơi cùng bạn bè để chia sẻ mẹo tối ưu và trao đổi về các giải pháp. Một số người dùng nói rằng trò chơi đã ảnh hưởng đến con đường nghề nghiệp của họ, cho họ dũng cảm đối mặt với các bài toán Advent of Code và Project Euler.

**Thẻ**: `#programming`, `#game`, `#education`, `#assembly`, `#Zachtronics`

---

<a id="item-5"></a>
## [Podman v6.0.0 ra mắt với mạng nâng cao và tính năng Quadlet](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0, ra mắt vào tháng 7 năm 2026, giới thiệu các khả năng mạng mới dựa trên Netavark và Aardvark DNS, đồng thời cải tiến Quadlet để quản lý các container rootless. Các cập nhật này làm tăng cường vị thế của Podman như một lựa chọn thay thế Docker không cần daemon, đặc biệt phù hợp với môi trường rootless và CI/CD, đồng thời giải quyết những vấn đề mạng đã lâu tồn tại, cản trở việc sử dụng. Phát hành này dựa trên Netavark làm backend mạng mặc định, bao gồm Aardvark DNS để khám phá dịch vụ, và bổ sung mẫu Quadlet giúp đơn hoá việc triển khai container rootless mà không cần daemon.

hackernews · soheilpro · 2/7 14:23 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48762098)

**Bối cảnh**: Podman là một công cụ container mã nguồn mở quản lý container và pod mà không cần daemon trung tâm, hỗ trợ chạy rootless để tăng cường bảo mật. Stack mạng của Podman, Netavark (viết bằng Rust) kèm theo Aardvark DNS, đã thay thế backend CNI cũ kể từ phiên bản 4.0, mang lại hỗ trợ IPv6 tốt hơn và tích hợp DNS. Những nền tảng này cho phép các tính năng mới trong v6.0.0, như cấu hình mạng được nâng cao và Quadlet điều phối container.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-network.1.html">podman-network — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/podman-new-network-stack">Podman 4.0's new network stack: What you need to know</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-03-18-fix-rootless-podman-network-issues/view">How to Fix Rootless Podman Network Issues - oneuptime.com</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận đón nhận các tính năng mạng mới và Quadlet, cho rằng việc chuyển từ Docker sang Podman có thể đơn giản như cài đặt và trỏ tới các file docker‑compose hiện có. Một số người dùngแสดง sự phiền phù vì Podman vẫn thiếu gói bản cập nhật cho Ubuntu và các phân phối phổ biến, hạn chế việc sử dụng. Ngoài ra, có người hỏi về kinh nghiệm thực tế khi di chuyển các hệ thống tự động hóa dựa trên compose sang Podman.

**Thẻ**: `#Podman`, `#containerization`, `#Docker alternative`, `#release`, `#open source`

---

<a id="item-6"></a>
## [Patch CUDA cho phép DeepSeek V4 Flash chạy bối cảnh 1M token trên RTX 5090](https://www.reddit.com/r/LocalLLaMA/comments/1ulymml/llamacpp_patch_deepseek_v4_flash_running_with/) ⭐️ 8.0/10

Một nhà phát triển đã vá llamacpp bằng một nhân CUDA tùy chỉnh để chạy DeepSeek V4 Flash tại địa phương với bối cảnh 1M token trên RTX 5090, giảm lượng VRAM từ khoảng 256 GB xuống khoảng 3,75 GiB và tăng tốc độ prefill. Cách phát hiện này làm cho các mô hình LLM bối cảnh siêu dài trở nên khả thi trên GPU tiêu dùng, giảm đáng kể rào cản phần cứng cho nhà nghiên cứu và nhà phát triển, đồng thời chứng minh cách tích hợp nhân atenção thưa vào llamacpp để suy luận hiệu quả. Việc vá thêm một bộ chỉ mục sáng tạo được tăng tốc CUDA cho cơ chế atenção thưa của DeepSeek, đạt khoảng 159 t/s prefill tại 1M token với khoảng 31 GiB VRAM (hoặc khoảng 3,75 GiB khi ubatch 768) và duy trì tốc độ decode khoảng 13,7 t/s; tính chính xác đã được xác minh bằng thử nghiệm kim trong rơm cho độ sâu lên tới 1M token.

reddit · r/LocalLLaMA · /u/da_dragon321 · 2/7 23:54

**Bối cảnh**: llamacpp là một thư viện C/C++ để suy luận LLM hỗ trợ cả backend CPU và GPU, bao gồm CUDA. DeepSeek V4 Flash là một mô hình hỗn hợp chuyên gia có 284 tỷ tham số và cửa sổ bối cảnh 1 triệu token, sử dụng DeepSeek Sparse Attention (DSA), dựa vào bộ chỉ mục sáng tạo để chọn các token liên quan. RTX 5090 là GPU tiêu dùng mới nhất của NVIDIA, cung cấp VRAM lớn và nhiều nhân CUDA, phù hợp để chạy các mô hình lớn khi lượng bộ nhớ được giảm.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://deepinfra.com/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash - Demo - DeepInfra</a></li>
<li><a href="https://medium.com/@inamdaraditya98/deepseeks-breakthrough-how-sparse-attention-unlocks-next-gen-llm-efficiency-3bc233342aeb">DeepSeek Sparse Attention: How Lightning Indexing Revolutionizes LLM Efficiency | Medium</a></li>

</ul>
</details>

**Thẻ**: `#llamacpp`, `#DeepSeek-V4-Flash`, `#CUDA patch`, `#long-context LLM`, `#RTX 5090`

---

<a id="item-7"></a>
## [PeerTube: Nền tảng video miễn phí, phi tập trung và liên kết thay thế YouTube](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube là nền tảng video miễn phí, mã nguồn mở, phi tập trung sử dụng giao thức ActivityPub để liên kết giữa các phiên bản và áp dụng công nghệ peer‑to‑peer để giảm tải máy chủ, định vị mình như một lựa chọn thay thế cho các dịch vụ tập trung như YouTube. PeerTube giải quyết những lo ngại ngày càng tăng về tập trung dữ liệu và kiểm duyệt bằng cách cung cấp một mạng lưới video phi tập trung tôn trọng quyền riêng tư, kết nối với hệ sinh thái Fediverse rộng hơn, cho phép nhà sáng tạo giữ quyền kiểm soát nội dung của mình mà vẫn có thể tiếp cận khán giả trên các phiên bản độc lập. PeerTube sử dụng giao thức ActivityPub để liên kết và tùy chọn sử dụng streaming peer‑to‑peer dựa trên WebTorrent để phân tán tải phát video giữa các người xem. Mặc dù nó cung cấp lưu trữ và phát video mạnh mẽ, nhưng hiện tại PeerTube chưa có công cụ kiếm tiền tích hợp và phụ thuộc vào việc khám phá ở mức phiên bản, điều này có thể giới hạn khả năng tiếp cận khán giả.

hackernews · doener · 2/7 11:17 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48759634)

**Bối cảnh**: PeerTube được ra mắt năm 2017 bởi nhà phát triển Chocobozzz và hiện được duy trì bởi tổ chức phi lợi nhuận Pháp Framasoft, là một nền tảng video mã nguồn mở triển khai giao thức ActivityPub, cho phép các phiên bản khác nhau giao tiếp như một phần của hệ sinh thái Fediverse. Nhờ sử dụng công nghệ peer‑to‑peer tùy chọn, các video phổ biến có thể được phát trực tiếp từ trình duyệt của người xem, giảm bớt chi phí băng thông cho từng máy chủ. Là một phần của mạng xã hội phi tập trung, PeerTube cung cấp một lựa chọn thay thế cho các nền tảng video tập trung như YouTube, Vimeo và Dailymotion.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ActivityPub">ActivityPub</a></li>
<li><a href="https://github.com/Chocobozzz/PeerTube">GitHub - Chocobozzz/PeerTube: ActivityPub-federated video streaming platform using P2P directly in your web browser · GitHub</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận đánh giá cao khả năng lưu trữ video liên kết, tôn trọng quyền riêng tư của PeerTube cho các dự án mã nguồn mở, nhưng họ cũng chỉ ra rằng nền tảng hiện tại thiếu các tùy chọn kiếm tiền và có khán giả nhỏ, khiến việc tìm kiếm nội dung phổ biến trở nên khó khăn. Một số người thấy nó đủ để lưu trữ video hướng dẫn tự lưu trữ, trong khi những người khác phàn nàn về khả năng khám phá hạn chế và sự phụ thuộc vào việc cura­tion ở mức phiên bản.

**Thẻ**: `#decentralized`, `#video platform`, `#open source`, `#federated`, `#PeerTube`

---

<a id="item-8"></a>
## [Nhà nghiên cứu AI cao cấp tại Nvidia nghi ngờ AGI, khuyên mô hình open-source tùy chỉnh](https://www.reddit.com/r/LocalLLaMA/comments/1ult0f4/its_officially_over_one_of_the_fathers_of_ai_at/) ⭐️ 7.0/10

Một nhà nghiên cứu AI cao cấp tại Nvidia заяви rằng trí tuệ nhân tạo tổng quát (AGI) không 太可能, so sánh các mô hình đóng của OpenAI và Anthropic với các dịch vụ internet đóng AOL và Prodigy, và khuyên các doanh nghiệp nên sử dụng mô hình open-source được tùy chỉnh. Nhận xét của ông nhấn mạnh sự tăng trưởng của sự hoài nghi về AGI trong thời gian ngắn và nhấn mạnh sự chuyển đổi hướng tới các giải pháp AI mở, có thể tùy chỉnh, có thể làm cho việc áp dụng AI trở nên dân chủ hơn trong các ngành công nghiệp. Nhà nghiên cứu không đưa ra timetable cụ thể cho AGI nhưng đã đối lập tính hạn chế của các mô hình proprietary với sự linh hoạt của các LLM open-source mà doanh nghiệp có thể tinh chỉnh để phù hợp với các nhiệm vụ cụ thể.

reddit · r/LocalLLaMA · /u/9gxa05s8fa8sh · 2/7 20:06

**Bối cảnh**: Trí tuệ nhân tạo tổng quát (AGI) là một hệ thống AI giả định có thể khớp hoặc vượt qua khả năng nhận thức của con người trên hầu hết các nhiệm vụ. Các mô hình ngôn ngữ lớn (LLM) open-source là các mô hình được cung cấp miễn phí mà bất kỳ ai cũng có thể kiểm tra, sửa đổi và triển khai, cho phép doanh nghiệp tạo ra các giải pháp tùy chỉnh. AOL và Prodigy là các dịch vụ trực tuyến đầu những năm 1990 cung cấp các khu vực nội dung tường tường (walled‑gardens), cuối cùng đã mất đi sự liên quan khi Internet mở rộng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AOL">AOL - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prodigy_(online_service)">Prodigy (online service) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#AI`, `#AGI`, `#open source`, `#Nvidia`, `#LLMs`

---

<a id="item-9"></a>
## [Sử dụng DSPy để đánh giá và cải thiện các system prompt SQL của Datasette Agent](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 6.0/10

Simon Willison đã áp dụng framework DSPy để đánh giá và tinh chỉnh các system prompt SQL của Datasette Agent dùng để trả lời câu hỏi về dữ liệu qua truy vấn chỉ đọc, sử dụng mô hình GPT-4.1 mini và nano qua Claude Fable 5. Công việc này minh họa một cách tiếp cận thực tế và tự động hóa trong thiết kế prompt, giúp nâng cao độ tin cậy và chính xác của các agent dựa trên LLM, đồng thời cung cấp một mẫu có thể tái sử dụng để tối ưu các hệ thống AI tương tự. Các prompt ban đầu không liệt kê tên cột khiến mô hình đoán tên cột (như page_count, o.order_id, first_name) và gây ra vòng lặp lỗi‑thử lại; DSPy đề xuất либо đưa tên cột vào phần liệt kê schema, либо làm mềm lời khuyên "đừng gọi describe_table/.

rss · Simon Willison · 2/7 18:25

**Bối cảnh**: DSPy là một framework Python mã nguồn mở mà trong đó các tương tác với mô hình ngôn ngữ được xem như các mô-đun có thể lập trình, cho phép tối ưu hoá tự động các prompt và trọng lượng qua các signature và teleprompter. Datasette Agent là một trợ lý AI được xây dựng trên Datasette, cho phép người dùng đặt câu hỏi bằng ngôn ngữ tự nhiên về dữ liệu và thực hiện các truy vấn SQL chỉ đọc để lấy kết quả. Khi kết hợp hai công cụ này, ta có thể nghiên cứu cách cải thiện có hệ thống các prompt ảnh hưởng đến hành vi tạo SQL của agent.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help ...</a></li>

</ul>
</details>

**Thẻ**: `#DSPy`, `#Datasette`, `#prompt engineering`, `#SQL agents`, `#AI research`

---

<a id="item-10"></a>
## [Thử nghiệm trợ lý głos nguồn mở kết hợp Parakeet, Gemma 4 31B, Qwen3TTS.](https://www.reddit.com/r/LocalLLaMA/comments/1ulgwld/talking_with_gemma_4_31b/) ⭐️ 6.0/10

Thử nghiệm kết hợp mô hình nhận dạng giọng nói Nvidia Parakeet, mô hình ngôn ngữ Gemma 4 31B được phục vụ qua Cerebras và mô hình chuyển đổi văn bản thành lời nói Qwen3TTS để sao chép API realtime của OpenAI. Điều này cung cấp một giải pháp hoàn toàn mã nguồn mở, có thể triển khai cục bộ thay thế cho các trợ lý thoại độc quyền, nâng cao quyền riêng tư và cho phép tùy chỉnh. Hệ thống sử dụng mô hình Nvidia Parakeet‑tdt‑0.6b‑v2 (600 tr tham số ASR), Gemma 4 31B dense có cửa sổ ngữ cảnh 256K token và một triển khai Qwen3TTS streaming.

reddit · r/LocalLLaMA · /u/futterneid · 2/7 12:29

**Bối cảnh**: Nvidia Parakeet là một mô hình nhận dạng giọng nói mã nguồn mở được thiết kế để transcribe tiếng Anh với chất lượng cao.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://huggingface.co/nvidia/parakeet-tdt-0.6b-v2">nvidia / parakeet -tdt-0.6b-v2 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/google/gemma-4-31b-it">Gemma 4 31 B - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://github.com/andimarafioti/faster-qwen3-tts">GitHub - andimarafioti/faster-qwen3-tts: Real-time text-to ...</a></li>

</ul>
</details>

**Thẻ**: `#voice assistant`, `#Gemma 4`, `#open-source AI`, `#realtime API`, `#speech synthesis`

---

<a id="item-11"></a>
## [CEO Palantir chỉ trích mô hình AI đóng, anuncia mua chip Nvidia](https://www.reddit.com/r/LocalLLaMA/comments/1ulb4nx/palantir_ceo_rages_against_closed_models/) ⭐️ 6.0/10

CEO Palantir công khai chỉ trích các mô hình AI đóng của Anthropic và OpenAI, buộc tội chúng của việc tính phí quá cao và lạm dụng dữ liệu, đồng thời thông báo rằng Palantir đã đạt thỏa thuận mua chip Nvidia để chạy các mô hình ngôn ngữ địa phương cho khách hàng doanh nghiệp. Điểm nhấn này nhấn mạnh xu hướng tăng trưởng của doanh nghiệp trong việc ưu tiên các mô hình AI mở chạy địa phương, mang lại sự kiểm soát dữ liệu tốt hơn và chi phí dự đoán được, đồng thời cũng thể hiện sự căng thẳng cạnh tranh giữa các nhà cung cấp mô hình đóng và các công ty tìm kiếm độc lập phần cứng qua GPU Nvidia. Thỏa thuận bao gồm việc mua GPU Nvidia để triển khai các mô hình LLM mã nguồn mở trên premises cho khách hàng doanh nghiệp, cho phép suy luận địa phương mà không cần dựa vào API bên ngoài; CEO cụ thể tên Anthropic và OpenAI là ví dụ về mô hình chius mà được cho là tính phí quá cao và lạm dụng dữ liệu người dùng.

reddit · r/LocalLLaMA · /u/burner20170218 · 2/7 07:15

**Bối cảnh**: Các mô hình AI đóng là hệ thống sở hữu trọng số và dữ liệu huấn luyện không được công khai, thường được cung cấp qua API đám mây và được đánh giá cao về hiệu suất và hỗ trợ, trong khi các mô hình AI mở công bố kiến trúc và trọng số, cho phép kiểm tra, sửa đổi và triển khai địa phương. Việc chạy LLM trên premises giúp doanh nghiệp duy trì chủ quyền dữ liệu, giảm độ trễ và tránh chi phí API lặp lại, nhưng đòi hỏi phần cứng phù hợp như GPU Nvidia cung cấp sức mạnh tính toán cần thiết để thực hiện suy luận. Các GPU Nvidia mới nhất như H100 và RTX 6000 Ada thường được đề xuất cho workload LLM nhờ VRAM cao và hiệu suất nhân tensor, khiến chúng trở thành lựa chọn thực tế cho các doanh nghiệp mua chip để lưu trữ mô hình địa phương.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/ai-open-models-have-benefits-so-why-arent-they-more-widely-used">AI open models have benefits. So why aren’t they more widely used? | MIT Sloan</a></li>
<li><a href="https://www.techtarget.com/searchenterpriseai/feature/Attributes-of-open-vs-closed-AI-explained">Attributes of Open vs. Closed AI Explained</a></li>
<li><a href="https://developersvoice.com/blog/ai-development/running-ai-on-prem/">Running AI On-Prem: A Practical Guide to Using Local LLMs ...</a></li>

</ul>
</details>

**Thẻ**: `#AI`, `#Open Source`, `#Large Language Models`, `#Enterprise AI`, `#Palantir`

---

<a id="item-12"></a>
## [Mã nguồn Kimi K2.7 hiện có sẵn trong GitHub Copilot](https://www.reddit.com/r/LocalLLaMA/comments/1ulm1gt/kimi_k27_code_is_generally_available_in_github/) ⭐️ 6.0/10

Mô hình Kimi K2.7 Code, một mô hình agentic mã nguồn mở, hiện đã được cung cấp rộng rãi như một tùy chọn có thể chọn trong bộ chọn mô hình của GitHub Copilot. Đây là lần đầu tiên một mô hình mã nguồn mở được cung cấp trực tiếp trong Copilot. Nhà phát triển có thêm lựa chọn LLM bên trong Copilot, bao gồm một lựa chọn mã nguồn mở và chi phí thấp hơn so với các mô hình riêng tư. Điều này mở rộng hệ sinh thái các mô hình có sẵn để hỗ trợ mã hóa bằng AI và khơi gợi sự cạnh tranh và đổi mới. Kimi K2.7 Code cải thiện khả năng mã hóa dài hạn và khả năng agent, đồng thời sử dụng ít hơn 30% token suy nghĩ so với K2.6. Nó yêu cầu bật thinking và preserve_thinking là True, với nhiệt độ đề xuất là 1.0 cho chế độ suy nghĩ.

reddit · r/LocalLLaMA · /u/zxyzyxz · 2/7 15:51

**Bối cảnh**: GitHub Copilot là một công cụ hoàn thành mã dựa trên AI, gợi ý đoạn mã khi nhà phát triển gõ. Nó hỗ trợ nhiều mô hình ngôn ngữ mà người dùng có thể chọn từ bộ chọn mô hình. Một mô hình mã nguồn mở có nghĩa là các trọng số của nó được công khai, cho phép bất kỳ ai cũng có thể kiểm tra, tinh chỉnh hoặc chạy mô hình độc lập, trái với các mô hình riêng tư đóng nguồn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.kimi.com/resources/kimi-k2-7-code">Kimi K2.7 Code: Open-Source Agentic Coding Model</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K2.7-Code">moonshotai/Kimi-K2.7-Code · Hugging Face</a></li>
<li><a href="https://github.blog/changelog/2026-07-01-kimi-k2-7-is-now-available-in-github-copilot/">Kimi K2.7 Code is generally available in GitHub Copilot</a></li>

</ul>
</details>

**Thẻ**: `#AI code generation`, `#GitHub Copilot`, `#Kimi K2.7`, `#LLM`, `#developer tools`

---

<a id="item-13"></a>
## [Kế hoạch xây dựng lại Gemma 4 31b với các lớp attention được sửa đổi](https://www.reddit.com/r/LocalLLaMA/comments/1ulmez2/rebuilding_gemma_4_31b_better_as_26b/) ⭐️ 6.0/10

Tác giả thông báo về dự án xây dựng lại mô hình Gemma 4 31b bằng cách tái cấu trúc các lớp attention trượt cửa sổ (SWA) và thêm mạng lũy remaining dựa trên attention để nâng cao khả năng cohérence toàn cầu. Nếu thành công, việc sửa đổi kiến trúc này có thể chứng minh cách các thay đổi có mục tiêu giảm kích thước mô hình đồng thời duy trì hoặc nâng cao hiệu suất, cung cấp một bản thiết kế để tối ưu hóa LLM do cộng đồng 주도. Kế hoạch bao gồm việc loại bỏ lớp SWA block yếu nhất, điều chỉnh lại kích thước cửa sổ SWA còn lại thành 1024/2048/4096/8192 token, chèn mạng lũy remaining dựa trên attention (từ bài báo Moonshot khoảng đầu năm 2026), và huấn luyện lại bằng cách sử dụng top‑K logits từ mô hình 31b gốc để giảm tham số từ khoảng 30,81 tỷ xuống khoảng 26,02 tỷ.

reddit · r/LocalLLaMA · /u/NineThreeTilNow · 2/7 16:05

**Bối cảnh**: Gemma 4 31b là một mô hình ngôn ngữ decoder‑only sử dụng một số lớp attention trượt cửa sổ (SWA) để xử lý các chuỗi dài một cách hiệu quả đồng thời giữ một lớp attention toàn cầu để mô hình quan hệ giữa các token. Mạng lũy remaining dựa trên attention thêm các đường dẫn remaining phụ trợ bằng attention, giúp thông tin di chuyển tự do hơn giữa các lớp và có thể nâng cao khả năng cohérence. Phương pháp top‑K logits đóng băng các lớp ngoài của mô hình và huấn luyện lại các lớp bên trong để dự đoán các token có xác suất cao nhất, từ đó giữ nguyên từ vựng và tokenizer.

**Thẻ**: `#Gemma`, `#LLM architecture`, `#attention mechanisms`, `#model experimentation`, `#AI research`

---