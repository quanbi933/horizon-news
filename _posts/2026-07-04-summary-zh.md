---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> Đã chọn 5 tin quan trọng từ 11 nội dung.

---

1. [Mistral phát hành Leanstral‑1.5, mô hình 6B tham số mở nguồn](#item-1) ⭐️ 9.0/10
2. [Jamesob công bố hướng dẫn chạy LLM tiên tiến tại local](#item-2) ⭐️ 8.0/10
3. [Bản đồ Khoảng trống AI mã nguồn mở được ra mắt bởi Current AI](#item-3) ⭐️ 7.0/10
4. [Meituan công bố LongCat 2.0 INT8/FP8 trên Hugging Face](#item-4) ⭐️ 6.0/10
5. [Qwen3.6-27b-mtp-q8 tự động mã hóa A* pathfinding trong trò chơi Java test](#item-5) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Mistral phát hành Leanstral‑1.5, mô hình 6B tham số mở nguồn](https://www.reddit.com/r/LocalLLaMA/comments/1umgdhx/mistral_released_leanstral15119ba6b/) ⭐️ 9.0/10

Mistral đã phát hành Leanstral‑1.5, một mô hình có giấy phép Apache‑2.0 với 6B tham số hoạt động, đạt kết quả tốt nhất trên miniF2F, PutnamBench, FATE‑H/X và phát hiện năm lỗi chưa biết trước trong mã nguồn thực tế. Phát hành này tiến bộ trong việc chứng minh định lý bằng AI khi cung cấp một mô hình mở nguồn, hiệu suất cao, có thể xác thực tính chính xác của phần mềm và phát hiện lỗi, giúp giảm chi phí xác thực cho nhà phát triển và nhà nghiên cứu. Leanstral‑1.5 được huấn luyện qua trung‑training, fine‑tuning có giám sát và học tăng cường bằng thuật toán CISPO; nó giải được 587/672 bài PutnamBench, đạt 87% trên FATE‑H và 34% trên FATE‑X, và đạt điểm tối đa trên miniF2F.

reddit · r/LocalLLaMA · /u/Tall-Ad-7742 · 3/7 14:44

**Bối cảnh**: Xác thực hình thức sử dụng bằng chứng toán học để đảm bảo rằng các thông số phần mềm hoặc phần cứng là chính xác, thường được hỗ trợ bởi các trình chứng minh định lý tương tác như Lean. miniF2F là một benchmark xuyên hệ thống chứa các bài toán toán học cấp Olimpiade được formal hóa trong các hệ thống như Lean, trong khi PutnamBench mở rộng điều này đến các bài toán cấp đại học từ cuộc thi Putnam. Thuật toán học tăng cường CISPO cắt bớt trọng số lấy mẫu quan trọng để ổn định việc huấn luyện các mô hình ngôn ngữ lớn, cho phép Leanstral‑1.5 học được các chiến lược chứng minh định lý hiệu quả.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/openai/miniF2F">GitHub - openai/miniF2F: Formal to Formal Mathematics Benchmark · GitHub</a></li>
<li><a href="https://trishullab.github.io/PutnamBench/">PutnamBench : A Multilingual Mathematics Benchmark for Formal...</a></li>
<li><a href="https://swift.readthedocs.io/en/v3.12/Instruction/GRPO/AdvancedResearch/CISPO.html">Clipped Importance Sampling Policy Optimization ( CISPO ) — swift...</a></li>

</ul>
</details>

**Thẻ**: `#formal verification`, `#AI for theorem proving`, `#Mistral`, `#Leanstral`, `#open-source model`

---

<a id="item-2"></a>
## [Jamesob công bố hướng dẫn chạy LLM tiên tiến tại local](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob đã phát hành một hướng dẫn chi tiết trên kho GitHub của mình về cách chạy các mô hình ngôn ngữ lớn tiên tiến tại local, được chia sẻ qua một bài đăng trên Hacker News và đã kích hoạt cuộc thảo luận rộng rãi. Hướng dẫn cung cấp các bước thực tế và có ý thức về chi phí để người yêu thích và nhà nghiên cứu có thể thử nghiệm các mô hình tiên tiến mà không cần API đám mây, nhấn mạnh các trade‑offs về phần cứng và kỹ thuật lượng tử hóa. Hướng dẫn tham chiếu đến cấu hình cụ thể như hệ thống 40.000 USD với bốn GPU giá 12.000 USD mỗi cái, thảo luận về việc chạy các mô hình như Qwen3.6‑27B, GLM‑5.2 và DeepSeek V4‑Flash, và bao gồm các phương pháp lượng tử hóa như INT8‑mix NVFP4 và lượng tử 6‑bit cho Qwen.

hackernews · livestyle · 3/7 15:03 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48775921)

**Bối cảnh**: Các mô hình ngôn ngữ lớn tiên tiến (LLM) như Qwen 3.6, GLM‑5.2 và DeepSeek V4 có hàng trăm tỷ tham số và thường cần lượng bộ nhớ GPU lớn để chạy ở độ chính xác đầy đủ. Việc chạy chúng ở local đòi hỏi phải sử dụng GPU tiêu thụ cao cấp có VRAM lớn hoặc áp dụng kỹ thuật lượng tử hóa để giảm kích thước mô hình đồng thời duy trì hiệu suất. Các cuộc thảo luận trong cộng đồng thường tập trung vào chi phí phần cứng, cácoffs giữa chất lượng mô hình và giá cả, cũng như khả thi của các cấu hình từ hai card RTX 3090 cho tới các hệ thống GPU đa card đắt tiền.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/jamesob/local-llm">GitHub - jamesob/local-llm: Everything I know about running LLMs locally · GitHub</a></li>
<li><a href="https://news.ycombinator.com/item?id=48775921">Jamesob's guide to running SOTA LLMs locally | Hacker News</a></li>
<li><a href="https://aiweekly.co/node/5306">James O'Beirne publishes local-LLM build guide for July 2026 | AI Weekly</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận cảnh báo rằng cấu hình 40.000 USD thực tế sẽ tốn khoảng 50‑55.000 USD và khuyên người đọc nên giảm mong đợi, lưu ý rằng các cấu hình local thường phụ thuộc vào lượng tử hóa và có thể vẫn kém hơn các mô hình đám mây. Một số người gợi ý các lựa chọn rẻ hơn như hai card RTX 3090 để chạy Qwen3.6‑27B, trong khi những người khác nhấn mạnh rằng với 128 GB VRAM qua kiến trúc bộ nhớ thống nhất (ví dụ Apple M5) cũng có thể chạy DeepSeek V4 Flash ở tốc độ hợp lý. Tổng thể, cuộc thảo luận thể hiện sự hứng thú về việc chạy LLM tại local nhưng cũng được cân bằng bằng nhận thức thực tế về chi phí, độ phức tạp và khoảng cách chất lượng.

**Thẻ**: `#LLM`, `#local deployment`, `#hardware`, `#AI`, `#guide`

---

<a id="item-3"></a>
## [Bản đồ Khoảng trống AI mã nguồn mở được ra mắt bởi Current AI](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

Simon Willison đã ra mắt Bản đồ Khoảng trống AI mã nguồn mở phiên bản v0.1 vào ngày 1 tháng 7 năm 2026, một danh mục gồm 421 sản phẩm AI mã nguồn mở covering phần mềm, mô hình, bộ dữ liệu và phần cứng. Bản đồ Khoảng trống cung cấp cho nhà nghiên cứu và nhà phát triển một tài liệu tham khảo có thể tra cứu để xác định các thành phần còn thiếu trong stack AI mã nguồn mở, từ đó giúp ưu tiên đầu tư và phát triển. Nó liệt kê 266 công cụ phần mềm, 85 mô hình, 50 bộ dữ liệu và 20 dự án phần cứng từ 228 tổ chức, được phân loại vào 14 danh mục trên ba lớp stack, với dữ liệu nền tảng được phát hành dưới giấy phép MIT trên GitHub (1.184 file YAML) và theo dõi 16.185 kho lưu trữ qua Datasette Lite.

rss · Simon Willison · 3/7 22:04

**Bối cảnh**: Current AI là một đối tác toàn cầu được ra mắt như một phi lợi nhuận tại Hội nghị Hành động AI ở Paris vào tháng 2 năm 2025, được hỗ trợ bởi 400 triệu USD vốn cam kết. Bản đồ Khoảng trống AI mã nguồn mở nhằm mô tả trạng thái hiện tại của AI mã nguồn mở để phát hiện các khoảng trống trong hệ sinh thái. Hội nghị Hành động AI nhấn mạnh việc truy cập AI độc lập, công nghệ thân thiện với môi trường và quản trị toàn cầu hiệu quả.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Action_Summit">AI Action Summit 2025 - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#open-source`, `#AI`, `#gap-map`, `#resources`, `#Current AI`

---

<a id="item-4"></a>
## [Meituan công bố LongCat 2.0 INT8/FP8 trên Hugging Face](https://www.reddit.com/r/LocalLLaMA/comments/1umo8zu/longcat_2_model_weights_have_been_published/) ⭐️ 6.0/10

Meituan đã công bố trọng số mô hình ngôn ngữ LongCat 2.0 trên Hugging Face, cung cấp cả phiên bản INT8 được lượng tử hoá và định dạng FP8. Phát hành này cung cấp cho cộng đồng mã nguồn mở một mô hình LLM Mixture‑of‑Experts dài bối cảnh mới, có thể chạy hiệu quả hơn trên phần cứng có hạn, mở rộng lựa chọn cho các tác vụ mã hóa và tác nhân tự trị. LongCat 2.0 là mô hình MoE có 1,6 tỷ tham số và cửa sổ bối cảnh 1 triệu token; phiên bản INT8 giảm kích thước mô hình xuống khoảng một phần tư so với FP16 ban đầu, trong khi định dạng FP8 cho phép suy luận trên GPU lớp Hopper với băng thông bộ nhớ giảm.

reddit · r/LocalLLaMA · /u/RhubarbSimilar1683 · 3/7 19:49

**Bối cảnh**: LongCat 2.0 là mô hình ngôn ngữ Mixture‑of‑Experts trọng số mở của Meituan, được thiết kế cho mã hóa, reasoning và quy trình tác nhân tự trị ở quy mô_frontier. Lượng tử hoá INT8 chuyển đổi các tham số 32‑bit floating‑point thành số nguyên 8‑bit, giảm bộ nhớ và yêu cầu tính toán. FP8 là định dạng số thực thấp độ chính xác được hỗ trợ bởi GPU mới như NVIDIA Hopper, cho phép suy luận nhanh hơn với ít bộ nhớ hơn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://longcat.chat/blog/longcat-2.0/">Introducing LongCat - 2 . 0</a></li>
<li><a href="https://www.emergentmind.com/topics/dynamic-int8-quantization-4e0999a9-2091-414e-a165-1e5221c6f060">Dynamic INT 8 Quantization</a></li>
<li><a href="https://en.wikipedia.org/wiki/Minifloat">Minifloat - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#long-context`, `#model-release`, `#HuggingFace`, `#Meituan`

---

<a id="item-5"></a>
## [Qwen3.6-27b-mtp-q8 tự động mã hóa A* pathfinding trong trò chơi Java test](https://www.reddit.com/r/LocalLLaMA/comments/1umvwb9/qwen3627bmtpq8_successfully_created_an_a/) ⭐️ 6.0/10

Người dùng đã chạy Claude Code tại local với mô hình Qwen3.6-27b-mtp-q8 để tạo ra thuật toán A* pathfinding cho một trò chơi test Java, kèm theo bộ kiểm tra tự tạo mà tự động theo dõi nhật ký, tái cấu trúc mã và khởi động lại trò chơi trong khoảng 12 giờ. Điều này chứng minh rằng một LLM chạy local có thể thực hiện các tác vụ mã hóa phức tạp từ đầu đến cuối—bao gồm tạo kiểm tra và gỡ lỗi lặp lại—nhấn tiềm năng thực tế của quy trình vibecoding cho phát triển AI trò chơi. Mô hình đã xây dựng một bộ kiểm tra tự động lái người chơi, theo dõi sự cố lỗi chỉ số, tái cấu trúc mã di chuyển NPC theo thời gian thực và khởi động lại trò chơi sau mỗi thay đổi; sau khoảng mười hai giờ kiểm tra tự động, NPC có thể di chuyển qua hầu hết các chướng ngại vật, mặc dù đôi khi vẫn gặp lỗi.

reddit · r/LocalLLaMA · /u/swagonflyyyy · 4/7 01:28

**Bối cảnh**: Qwen3.6-27b-mtp-q8 là mô hình đa phương thức hybrid‑thinking có 27 tỷ tham số của Alibaba, sử dụng dự đoán đa token (MTP) để đạt tốc độ sinh nhanh hơn 1,4‑2,2 lần mà không giảm độ chính xác. Claude Code là trợ lý mã hóa AI có tính chất tác động, có thể tự viết, kiểm tra và tái cấu trúc mã dựa trên lời mô tả bằng ngôn ngữ tự nhiên. Vibecoding là thực hành sử dụng mô hình ngôn ngữ lớn để tạo mã từ mô tả bằng ngôn ngữ tự nhiên, một thuật ngữ được Andrei Karpathy làm phổ biến vào đầu năm 2025.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://huggingface.co/originalGeek/Qwen3.6-27B-unsloth-MTP-Q8_0-HEAD-ONLY">originalGeek/ Qwen 3 . 6 - 27 B -unsloth- MTP - Q 8 _0-HEAD-ONLY...</a></li>
<li><a href="https://unsloth.ai/docs/models/qwen3.6">Run the new Qwen 3 . 6 - 27 B and 35B-A3B models locally!</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#code generation`, `#A* pathfinding`, `#vibecoding`, `#Java`

---