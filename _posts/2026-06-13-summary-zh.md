---
layout: default
title: "Horizon Summary: 2026-06-13 (ZH)"
date: 2026-06-13
lang: zh
---

> Đã chọn 10 tin quan trọng từ 14 nội dung.

---

1. [Phát hành vLLM v0.23.0 với cải tiến DeepSeek-V4 và Model Runner V2](#item-1) ⭐️ 8.0/10
2. [CRISPR-Cas12a2 chọn lọc phá vỡ chromatin để giết tế bào ung thư](#item-2) ⭐️ 8.0/10
3. [Thông báoDirective Mỹ ngừng truy cập Fable 5 và Mythos 5](#item-3) ⭐️ 7.0/10
4. [AI mã nguồn mở phải thắng: Tranh luận Hacker News](#item-4) ⭐️ 7.0/10
5. [Renault phát triển động cơ điện không sử dụng đất hiếm cho xe điện](#item-5) ⭐️ 7.0/10
6. [SEC đề xuất bãi bỏ quy định 20 năm chặn Wall Street giao dịch blockchain](#item-6) ⭐️ 7.0/10
7. [Apple công bố công cụ container mã nguồn mở Swift cho macOS](#item-7) ⭐️ 7.0/10
8. [Ollama phát hành phiên bản v0.30.8 với cải tiến MLX và cache prompt](#item-8) ⭐️ 6.0/10
9. [Cách cài đặt một trợ lý mã hoá địa phương trên macOS](#item-9) ⭐️ 6.0/10
10. [Chúng ta có biết rằng Quốc hội đang tranh luận về luật Crypto Wash Sale ngay bây giờ? (H.R. 9172)](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Phát hành vLLM v0.23.0 với cải tiến DeepSeek-V4 và Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

Phiên bản vLLM v0.23.0 bao gồm 408 commit từ 200 người đóng góp (63 người mới), với việc cứng nhắc DeepSeek-V4 trên nhiều backend, mở rộng Model Runner V2 cho các model dense Llama và Mistral, cập nhật frontend Rust, hỗ trợ Gemma 4, tương thích Transformers v5, offloading KV cache đa cấp, trình phân tích thống nhất và thêm nhiều model mới. Vì vLLM là thư viện phục vụ LLM được sử dụng rộng rãi, các cập nhật này nâng cao hiệu suất, mở rộng hỗ trợ model và đơn giản hoá triển khai sản xuất, ảnh hưởng đến các đội cơ sở hạ tầng AI và nhà phát triển dựa vào suy luận hiệu quả và mở rộng. DeepSeek-V4 có kernel attention TRTLLM-gen, metadata MLA sparse được tách rời và đường dẫn decode attention XPU; Model Runner V2 trở thành mặc định cho các model dense Llama/Mistral với bộ lấy mẫu FlashInfer và CUDA graphs có thể ngắt; frontend Rust thêm endpoint generate streaming và dynamic LoRA; offloading KV cache hỗ trợ cấp độ thứ hai là object-store; phân tích lý do và gọi công cụ được thống nhất dưới một giao diện Parser.parse().

github · khluu · 12/6 23:29

**Bối cảnh**: vLLM là thư viện cung cấp dịch vụ mô hình ngôn ngữ lớn với throughput cao, cho phép suy luận hiệu quả thông qua các kỹ thuật như paged attention và continuous batching. DeepSeek-V4 là mô hình AI có 1 nghìn tỷ tham số do DeepSeek ra mắt, nổi bật với kiến trúc bộ nhớ Engram và quy mô enormes. Model Runner V2 là động cơ thực thi được cập nhật trong vLLM, tối ưu việc chọn kernel, bắt đồ thị và song song cho các model dense và hỗn hợp MoE.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 (2026) — 1T Params, Benchmarks & Pricing</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.c-sharpcorner.com/article/docker-model-runner-adds-vllm-for-fast-ai-inference/">Docker Model Runner Adds vLLM for Fast AI Inference</a></li>

</ul>
</details>

**Thẻ**: `#vLLM`, `#LLM serving`, `#DeepSeek-V4`, `#Model Runner V2`, `#release`

---

<a id="item-2"></a>
## [CRISPR-Cas12a2 chọn lọc phá vỡ chromatin để giết tế bào ung thư](https://innovativegenomics.org/news/crispr-technique-selectively-shreds-cancer-cells/) ⭐️ 8.0/10

Nhà nghiên cứu đã thiết kế CRISPR-Cas12a2 để phát hiện chuyển RNA đặc biệt của khối u; khi nhận diện, enzym này kích hoạt quá trình phá vỡ rộng khắp DNA và chromatin, giết chọn lọc tế bào ung thư, bao gồm những đột biến trước đây không thể dùng thuốc, như được báo cáo trong bài báo Nature tháng 5/2026. Cách tiếp cận này mở rộng phạm vi mục tiêu ung thư có thể được tấn công bằng y học chính xác, cung cấp tiềm năng điều trị cho các loại ung thư thiếu thuốc hiệu quả, và thể hiện cơ chế giết tế bào mới của CRISPR ngoài việc chỉ cắt DNA. Cas12a2 có hoạt động nuclease không đặc biệt về chuỗi, được hướng dẫn bởi RNA, phá vỡ ssRNA, ssDNA và dsDNA, dẫn tới mảnh vỡ chromatin khi kết hợp với mục tiêu RNA bổ sung; phương pháp này vẫn còn ở giai đoạn tiền lâm sàng và có thể phát triển kháng thuốc.

hackernews · gmays · 12/6 15:15 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48505231)

**Bối cảnh**: CRISPR-Cas12a2 là một nuclease liên quan đến CRISPR, khác với Cas9 vì nó được kích hoạt khi kết nối với một mục tiêu RNA cụ thể và sau đó phá hủy vô chọn các axit nucleic gần đó, gây ra thương hại DNA và chromatin rộng rãi. Chromatin là kompleks của DNA và protein giúp đóng gói genoma; việc làm mảnh vỡ chromatin sẽ làm loạn quá trình chuyển 录 và sao chép DNA, dẫn tới tử tế bào. Nhiều loại ung thư có đột biến trong các gen được coi là 'không thể dùng thuốc' vì chúng không có túi kết nối thích hợp cho chất inhibitor nhỏ. Việc nhắm mục tiêu vào các đột biến này bằng CRISPR-Cas12a2 cho phép giết tế bào ung thư dựa trên đặc trưng biểu hiện RNA thay vì dựa vào vị trí kết nối thuốc.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41586-026-10466-y">RNA-triggered cell killing with CRISPR–Cas12a2 | Nature</a></li>
<li><a href="https://innovativegenomics.org/news/crispr-technique-selectively-shreds-cancer-cells/">New CRISPR Technique Selectively Shreds Cancer Cells, Including...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cas12a">Cas12a - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các thành viên chia sẻ link tới bản preprint và bài báo Nature, lưu ý rằng hoạt động phá vỡ chromatin của Cas12a2 gây phá hủy mạnh hơn so với việc cắt DNA đơn giản của Cas9, và cảnh báo rằng khả năng phát triển kháng thuốc ở u là khả dĩ. Một số người mong đợi CRISPR có thể chữa bệnh di truyền cá nhân, trong khi những người khác cho rằng CRISPR bị exaggerated, chỉ ra rằng số lượng liệu pháp CRISPR được phê duyệt bởi FDA vẫn hạn chế so với các phương pháp dựa trên vector virut.

**Thẻ**: `#CRISPR`, `#cancer therapy`, `#genomics`, `#precision medicine`, `#biotechnology`

---

<a id="item-3"></a>
## [Thông báoDirective Mỹ ngừng truy cập Fable 5 và Mythos 5](https://www.anthropic.com/news/fable-mythos-access) ⭐️ 7.0/10

Một bài đăng trên Hacker News gần đây tvr rằng Chính phủ Mỹ đã ban hành chỉ thị ngừng truy cập công khai vào các mô hình AI Fable 5 và Mythos 5 của Anthropic, gây ra cuộc tranh luận rộng rãi. Bài viết cho rằng lệnh này chủ yếu hướng tới người dùng ngoài Mỹ nhưng thực tế có thể ảnh hưởng đến quyền truy cập tổng thể. Nếu thông tin đúng, đây sẽ là một trong những lần đầu tiên chính phủ can thiệp trực tiếp để giới hạn truy cập công khai vào các mô hình LLM tiên tiến, ảnh hưởng đến đổi mới AI, cạnh tranh và an ninh quốc gia. Điều này cũng đặt ra câu hỏi về cách các quy định AI trong tương lai có thể cân bằng giữa lo ngại về an toàn và quyền truy cập mở vào các mô hình mạnh. Fable 5 được mô tả là mô hình mạnh mẽ nhất được Anthropic phát hành rộng rãi, được thiết kế cho các tác vụ suy luận phức tạp và tác động dài hạn, trong khi Mythos 5 là bản nâng cấp tăng dần so với Opus, tập trung vào bảo mật mạng và sinh học. Theo cáo buộc, chỉ thị này miễn trừ người dùng của chính phủ Mỹ nhưng sẽ chặn người dân không phải quốc gia Mỹ, có thể dẫn đến việc người dùng chuyển sang các mô hình được lưu trữ tại Trung Quốc.

hackernews · Dylan1312 · 13/6 00:51 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48511072)

**Bối cảnh**: Anthropic đã công bố Claude Fable 5 và Claude Mythos 5 vào đầu tháng 6 năm 2026 như là thế hệ mới nhất của các mô hình ngôn ngữ lớn. Fable 5 được định vị là mô hình mạnh mẽ nhất được phát hành rộng rãi của công ty, vượt trội trong các tác vụ suy luận và tác động dài hạn của tác nhân, trong khi Mythos 5 là một mô hình lớp Mythos được tối ưu hoá cho các tiêu chuẩn bảo mật mạng, sinh học và y tế. Cả hai mô hình đều được ra mắt cùng với một giai đoạn triển khai giới hạn cho khách hàng doanh nghiệp và người dùng trả phí, sau đó Fable 5 được mở rộng để truy cập công khai.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.cnbc.com/2026/06/09/anthropic-mythos-claude-fable-5.html">Anthropic releases Mythos-like AI model to the public, Claude Fable 5</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận chia rẽ, một số người coi đây là một trò chơi marketing hoặc là sự báo đáp xứng đáng, trong khi một số khác nhìn đây là dấu hiệu trước của việc chính phủ hạn chế truy cập vào các mô hình LLM mạnh mẽ. Nhiều người dùng cảnh báo rằng bước đi này có thể dẫn đến nhu cầu tăng về các mô hình được lưu trữ tại Trung Quốc và gây ra lo ngại về an ninh quốc gia cho các quốc gia khác. Cuộc thảo luận cũng cho thấy sự hoài nghi về tính xác thực của chỉ thị, vì chưa có bất kỳ xác nhận chính thức nào.

**Thẻ**: `#AI regulation`, `#LLM access`, `#US government policy`, `#Anthropic`, `#AI safety`

---

<a id="item-4"></a>
## [AI mã nguồn mở phải thắng: Tranh luận Hacker News](https://opensourceaimustwin.com/?share=v2) ⭐️ 7.0/10

Bài viết trên Hacker News có tiêu đề 'Open source AI must win'主張 rằng AI mã nguồn mở nên thắng, và đã kích hoạt một cuộc thảo luận chi tiết về khả thi, tài trợ và tác động xã hội của phát triển AI mở so với AI đóng. Cuộc tranh luận nhấn mạnh một mâu thuẫn chiến lược có thể quyết định quién kiểm soát khả năng AI, ảnh hưởng đến đổi mới, truy cập và nguy cơ độc quyền của các công ty lớn đối với các mô hình nền tảng. Các bình luận 者 đã nhấn mạnh những lo ngại về sự thống trị của doanh nghiệp, chi phí cấm đo để huấn luyện mô hình lớn, và những khó khăn kỹ thuật trong huấn luyện phi tập trung như độ trễ và nhiễm dữ liệu, đồng thời chỉ ra rằng các kỹ thuật như federated learning, LoRA và nền tảng Golem có thể giúp giảm thiểu một số thách thức.

hackernews · vednig · 13/6 02:14 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48511908)

**Bối cảnh**: AI mã nguồn mở là những mô hình mà mã code và trọng số được công khai, cho phép bất kỳ ai cũng có thể kiểm tra, sửa đổi và tái phân phối, trái ngược với các mô hình độc quyền được các công ty giữ kín. Huấn luyện các mô hình tiên tiến đòi hỏi tài nguyên tính toán enormes, dẫn đến sự quan tâm đến các mạng tính toán phi tập trung như Golem, cho phép người dùng chia sẻ sức mạnh GPU qua một thị trường peer-to-peer. Các kỹ thuật như federated learning cho phép huấn luyện trên các thiết bị phân tán mà không cần chia sẻ dữ liệu thô, trong khi các phương pháp hiệu quả về tham số như LoRA giảm số lượng trọng số cần huấn luyện khi tinh chỉnh các mô hình ngôn ngữ lớn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Federated_learning">Federated learning - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2106.09685">[2106.09685] LoRA: Low-Rank Adaptation of Large Language Models</a></li>
<li><a href="https://golem.network/">Golem Network</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận lo ngại nếu các phòng lab AI đóng chiếm ưu thế, chúng có thể trở thành người guarda của thông tin, phần mềm và công việc, thực chất chỉ đạo xã hội có thể nghĩ hoặc làm gì. Các người khác chỉ ra mức tài trợ khổng lồ cần thiết để huấn luyện và đặt câu hỏi liệu việc tính toán phi tập trung dựa trên tình nguyện viên có thể vượt qua được rủi ro về độ trễ và nhiễm dữ liệu không. Một số người cho rằng AI mã nguồn mở thực sự không thể thắng vì các lab chius có thể luôn hấp thụ những tiến bộ từ cộng đồng mở, mặc dù một số người khác bày tỏ sự ủng hộ và hỏi cách họ có thể giúp.

**Thẻ**: `#open-source AI`, `#AI ethics`, `#model training`, `#decentralization`, `#corporate control`

---

<a id="item-5"></a>
## [Renault phát triển động cơ điện không sử dụng đất hiếm cho xe điện](https://www.renaultgroup.com/en/magazine/energy-and-powertrains/all-about-electric-motors-with-no-rare-earths/) ⭐️ 7.0/10

Renault công bố đang phát triển động cơ điện không sử dụng đất hiếm cho các xe điện tương lai, nhấn mạnh thiết kế rotor cuộn loại bỏ từ vĩnh viễn. Giảm sự phụ thuộc vào tài nguyên đất hiếm có thể giảm chi phí, giảm thiểu rủi ro chuỗi cung ứng và nâng cao tính bền vững của sản xuất xe điện. Đồng thời, điều này tăng cường cạnh tranh với đối thủ như BMW, đã có động cơ không đất hiếm trên thị trường. Động cơ của Renault sử dụng kiến trúc rotor cuộn (động cơ đồng bộ kích điện) với chổi để cung cấp trường cho rotor, tránh việc dùng từ vĩnh viễn. Renault mục tiêu khoảng 160 kW công suất và có thể áp dụng công nghệ cuộn hairpin để tăng mật độ công suất, tương tự như động cơ cao áp không đất hiếm của Valeo.

hackernews · bestouff · 12/6 22:08 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48510010)

**Bối cảnh**: Hầu hết các động cơ traction của xe điện hiện nay đều sử dụng động cơ đồng bộ từ vĩnh viễn (PMSM) với từ석 neodymium thuộc nhóm đất hiếm để đạt mô men xoắn cao và hiệu suất. Các thiết kế thay thế như động cơ đồng bộ trường cuộn, động cơ từ không đồng bộ (switched reluctance) và động cơ cảm ứng có thể hoạt động mà không cần từ vĩnh viễn, nhưng thường phải hy sinh về mật độ công suất, độ phức tạp của điều khiển hoặc dao động mô men. Nghiên cứu gần đây cho thấy từ석 ferrite hoặc kỹ thuật cuộn nâng cao (ví dụ: hairpin) có thể nâng cao hiệu suất của các động cơ không đất hiếm, làm cho chúng trở nên khả thi cho xe điện.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.mdpi.com/2075-1702/13/8/702">Electric Vehicle Motors Free of Rare-Earth Elements—An Overview</a></li>
<li><a href="https://www.valeo.com/en/catalogue/pts/high-voltage-rare-earth-free-electric-motor/">High Voltage Rare Earth Magnet Free Electric Motor | Valeo</a></li>
<li><a href="https://www.tdk.com/en/tech-mag/ferrite02/012">Ferrite Magnets : Properties, Types, and Applications - TDK｜ Ferrite ...</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận cho thấy động cơ không từ vĩnh viễn không phải là điều mới, được nhắc đến là có hơn một세기 sử dụng và nhược điểm của thiết kế có chổi; họ nhấn mạnh động cơ không đất hiếm của BMW tiên tiến hơn (lên tới 300 kW trên kiến trúc 800 V) và thảo luận về lo ngại mòn của chổi, đồng thời suy đoán về việc kết hợp với pin natri của CATL có thể dẫn tới cuộc chiến giá và tầm xa.

**Thẻ**: `#electric vehicles`, `#rare earths`, `#motor technology`, `#sustainability`, `#automotive engineering`

---

<a id="item-6"></a>
## [SEC đề xuất bãi bỏ quy định 20 năm chặn Wall Street giao dịch blockchain](https://www.reddit.com/r/CryptoCurrency/comments/1u46j27/sec_targets_20yearold_rule_standing_between_wall/) ⭐️ 7.0/10

SEC đang tìm cách bãi bỏ một quy định 20 năm—có thể là Rule 15c6-1—ngăn cản các công ty Wall Street tham gia giao dịch chứng khoán dựa trên blockchain. Việc gỡ bỏ rào cản này có thể cho phép các tổ chức tài chính truyền thống quyết toán trên chuỗi các tài sản được mã hóa, tăng tính thanh khoản, giảm rủi ro đối phương và thúc đẩy việc áp dụng blockchain trong ngành tài chính. Quy định hiện tại yêu cầu hầu hết các giao dịch chứng khoán phải thanh toán trong vòng T+2, một khung thời gian không phù hợp với khả năng thanh toán gần như tức thì của mạng lưới blockchain. Việc sửa đổi quy định này sẽ đòi hỏi phải thay đổi các quy trình của cơ quan clearing và có thể gây ra tranh cãi về bảo vệ nhà đầu tư và rủi ro hệ thống.

reddit · r/CryptoCurrency · /u/kirtash93 · 12/6 20:22

**Bối cảnh**: Quy định SEC 15c6-1, được ban hành vào đầu những năm 1990, đặt chu kỳ thanh toán chuẩn cho các giao dịch của broker‑dealer là T+2 (trước đây là T+3) nhằm giảm rủi ro và đảm bảo thị trường có序. Các nền tảng giao dịch dựa trên blockchain có thể thanh toán giao dịch trong giây hoặc phút, tạo ra một sự không khớp với yêu cầu thời gian của quy định. SEC đã bắt đầu tìm cách thích ứng với tài chính trên chuỗi, như minh chứng bằng việc phê duyệt Paxos làm cơ quan clearing đầu tiên dựa trên blockchain và các phát biểu của Chủ tịch Paul Atkins về việc xem lại các quy định cho các nền tảng giao dịch trên chuỗi.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://cooleypubco.com/2022/02/10/proposes-shortening-settlement-cycle/">SEC proposes shortening the settlement cycle to T+ 1 —and asks: what...</a></li>
<li><a href="https://blockmanity.com/news/sec-breakthrough-paxos-earns-landmark-status-as-first-blockchain-clearing-agency/">SEC Breakthrough: Paxos Earns Landmark Status as First Blockchain ...</a></li>
<li><a href="https://ambcrypto.com/sec-chair-paul-atkins-signals-possible-rule-changes-for-onchain-trading-platforms/">SEC Chair Paul Atkins signals possible rule changes for... - AMBCrypto</a></li>

</ul>
</details>

**Thẻ**: `#SEC`, `#blockchain`, `#regulation`, `#Wall Street`, `#cryptocurrency`

---

<a id="item-7"></a>
## [Apple công bố công cụ container mã nguồn mở Swift cho macOS](https://github.com/apple/container) ⭐️ 7.0/10

Apple đã mã nguồn mở một công cụ mới dựa trên Swift tên 'container' cho phép chạy các container Linux dưới dạng máy ảo nhẹ trên macOS, được tối ưu cho Apple silicon. Kho lưu trữ đã nhận được hơn 100 sao trong vòng 24 giờ, cho thấy sự quan tâm mạnh mẽ của cộng đồng phát triển. Công cụ này cung cấp một lựa chọn bản địa, hiệu suất cao thay thế cho Docker và các runtime container khác trên Mac, đơn giản hóa quy trình phát triển cho người dùng Apple silicon. Nó cũng thể hiện cam kết ngày càng tăng của Apple đối với mã nguồn mở trong hệ sinh thái container. Công cụ được viết hoàn toàn bằng Swift, sử dụng Framework ảo hóa của Apple để tạo ra các máy ảo nhẹ, và hỗ trợ hình ảnh container tuân thủ chuẩn OCI, cho phép pull và push từ bất kỳ registry nào. Nó yêu cầu macOS 26 (or later) và phần cứng Apple silicon.

ossinsight · apple · 13/6 04:09

**Bối cảnh**: Đóng gói container bao gồm ứng dụng và các phụ thuộc vào các đơn vị cô lập có thể chạy nhất quán trong các môi trường khác nhau. Truyền thống, các nhà phát triển trên macOS thường dựa vào công cụ như Docker Desktop, который sử dụng một máy ảo Linux để chạy các container. Framework ảo hóa của Apple, được giới thiệu trong macOS, cho phép tạo ra các máy ảo nhẹ có hiệu suất gần bản địa, đặc biệt trên các chip Apple silicon. Khi xây dựng một runtime container dựa trên Swift sử dụng framework này, Apple cung cấp một giải pháp tích hợp và hiệu suất cao hơn để chạy các container Linux trên Mac.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/apple/container">GitHub - apple / container : A tool for creating and running Linux...</a></li>
<li><a href="https://opensource.apple.com/projects/container">Container - Apple Open Source</a></li>
<li><a href="https://www.techprovidence.com/apple-linux-containers-macos-tool-wwdc2025/">Apple Brings Native Linux Containers to macOS - Tech Providence</a></li>

</ul>
</details>

**Thẻ**: `#containerization`, `#macOS`, `#Swift`, `#Apple silicon`, `#DevOps`

---

<a id="item-8"></a>
## [Ollama phát hành phiên bản v0.30.8 với cải tiến MLX và cache prompt](https://github.com/ollama/ollama/releases/tag/v0.30.8) ⭐️ 6.0/10

Ollama v0.30.8 sửa lỗi chọn nhà cung cấp trong lệnh ollama launch, cải thiện cache prompt bằng cách tách rời khỏi sự thay đổi ngữ cảnh, và ổn định suy luận MLX với lớp tuyến tính và lớp nhúng được cứng hơn. Ngoài ra, nó thêm hỗ trợ tạo snapshot trong quá trình xử lý prompt và giải mã suy đoán, cũng như cải thiện xử lý mô hình lặp lại bằng trạng thái mỗi ranh giới từ nhân hạt gated‑delta. Các cập nhật này làm cho Ollama trở nên đáng tin cậy và nhanh hơn trên Apple Silicon, giảm độ trễ cho các prompt lặp lại nhờ tái sử dụng cache tốt hơn và cho phép thực hiện suôn sẻ các kiến trúc lặp lại. Vì vậy, nhà phát triển có thể triển khai nhiều loại LLM hơn với hiệu suất và ổn định được cải thiện. Các thay đổi chính bao gồm sửa lỗi chọn nhà cung cấp không đúng trong lệnh ollama launch và tách cache prompt khỏi sự thay đổi ngữ cảnh để tái sử dụng KV‑cache tốt hơn. Ngoài đó, MLX runner được cứng lớp tuyến tính và lớp nhúng, hỗ trợ tạo snapshot trong quá trình xử lý prompt và giải mã suy đoán, cũng như xử lý trạng thái mỗi ranh giới cho mô hình lặp lại qua nhân hạt gated‑delta.

github · github-actions[bot] · 12/6 17:04

**Bối cảnh**: Ollama là một runtime nhẹ cho phép người dùng chạy các mô hình ngôn ngữ lớn ở local, có hỗ trợ sẵn cho framework MLX của Apple trên Mac có chip M‑series. MLX sử dụng bộ nhớ thống 一 và GPU Neural Accelerator để tăng tốc suy luận, và việc tích hợp của Ollama giúp mô hình chạy nhanh hơn sau lần tải đầu tiên nhờ vào cache. Cache prompt lưu trữ context đã xử lý để các yêu cầu lặp lại có thể tái sử dụng KV cache, trong khi các mô hình lặp lại như quelli dựa trên nhân hạt gated‑delta cần xử lý trạng thái mỗi ranh giới để duy trì tính chính xác qua các khối.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=SnfDFwHeyA4">Ollama vs MLX Inference Speed on Mac Mini M4 Pro 64GB - YouTube</a></li>
<li><a href="https://quasa.io/media/ollama-just-got-blazing-fast-on-macs-full-mlx-support-brings-2-speedups-and-nvidia-quality-4-bit-inference">Ollama Just Got Blazing Fast on Macs: Full MLX Support Brings...</a></li>
<li><a href="https://github.com/ollama/ollama/issues/16635">cache_prompt is hardwired to the shift option — reproducible output and ...</a></li>

</ul>
</details>

**Thẻ**: `#ollama`, `#LLM`, `#MLX`, `#prompt caching`, `#software release`

---

<a id="item-9"></a>
## [Cách cài đặt một trợ lý mã hoá địa phương trên macOS](https://ikyle.me/blog/2026/how-to-setup-a-local-coding-agent-on-macos) ⭐️ 6.0/10

Hướng dẫn cài đặt và cấu hình một trợ lý mã hoá dựa trên LLM địa phương trên macOS bằng các công cụ như llama.cpp, kèm phản hồi từ cộng đồng về các tiêu chuẩn và các phương pháp thay thế.

hackernews · kkm · 12/6 17:34 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48507020)

**Thẻ**: `#macOS`, `#local LLM`, `#coding agent`, `#llama.cpp`, `#tutorial`

---

<a id="item-10"></a>
## [Chúng ta có biết rằng Quốc hội đang tranh luận về luật Crypto Wash Sale ngay bây giờ? (H.R. 9172)](https://www.reddit.com/r/CryptoCurrency/comments/1u47i2v/are_we_even_aware_that_congress_is_debating_a/) ⭐️ 6.0/10

Một người dùng Reddit cảnh báo rằng Quốc hội đang thảo luận về một dự luật mở rộng quy định wash sale truyền thống sang tài sản số, điều này có thể ảnh hưởng đến việc thu hoạch lỗ thuế cho các nhà giao dịch crypto trên chuỗi.

reddit · r/CryptoCurrency · /u/semaj_1028 · 12/6 21:00

**Thẻ**: `#cryptocurrency`, `#taxation`, `#regulation`, `#wash sale`, `#H.R.9172`

---