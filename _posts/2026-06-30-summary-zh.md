---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> Đã chọn 5 tin quan trọng từ 13 nội dung.

---

1. [vLLM v0.24.0 bổ sung hỗ trợ MiniMax-M3, tối ưu DeepSeek-V4 và nâng cấp FP8 trên AMD ROCm.](#item-1) ⭐️ 8.0/10
2. [Qwen 3.6 27B là điểm cân bằng lý tưởng cho LLM cục bộ](#item-2) ⭐️ 8.0/10
3. [Rocket Lab mua lại Iridium, tạo doanh nghiệp không gian tích hợp](#item-3) ⭐️ 8.0/10
4. [Ornith-1.0: Gia đình LLM cấp phép MIT cho mã hoá tác động tới 397B](#item-4) ⭐️ 8.0/10
5. [Đề xuất tên miền .self miễn phí cho tự lưu trữ](#item-5) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 bổ sung hỗ trợ MiniMax-M3, tối ưu DeepSeek-V4 và nâng cấp FP8 trên AMD ROCm.](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 8.0/10

vLLM đã phát hành phiên bản 0.24.0 với 571 commits từ 256 nhà đóng góp, giới thiệu hỗ trợ mô hình MiniMax-M3, các tối ưu hóa sâu rộng cho DeepSeek-V4 và các cải tiến FP8 trên AMD ROCm bao gồm MXFP4 và FP8 sparse GQA. Phiên bản này mở rộng phạm vi hỗ trợ mô hình và cải thiện hiệu suất suy luận, cho phép người dùng chạy các mô hình mới có bối cảnh lớn trên GPU AMD với mức tiêu thụ bộ nhớ thấp hơn nhờ định dạng FP8. Các điểm nổi bật bao gồm hỗ trợ MiniMax-M3 với MiniMax Sparse Attention (MSA), bộ chỉ mục BF16/FP8, MXFP4, FP8 sparse GQA, cùng các tối ưu hóa DeepSeek-V4 như FlashInfer sparse index cache và cấp phát KV liên tục theo khối; MRv2 hiện mặc định hỗ trợ mô hình đã được lượng tử hóa và API chọn thiết bị đã thay đổi từ CUDA_VISIBLE_DEVICES sang tham số device_ids.

github · khluu · 29/6 19:41

**Bối cảnh**: vLLM là một thư viện suy luận mô hình ngôn ngữ lớn có throughput cao, hỗ trợ cả GPU NVIDIA và AMD qua các backend CUDA và ROCm. MiniMax-M3 là một mô hình ngôn ngữ trọng lượng mở có thể xử lý tới 1 triệu token nhờ cơ chế MiniMax Sparse Attention (MSA). DeepSeek-V4 là một loạt mô hình mới nhất có các tối ưu kiến trúc cho tác vụ tác động, trong khi FP8 là định dạng số thấp độ chính xác giúp giảm băng thông bộ nhớ và tăng hiệu suất tính toán trên phần mềm tương thích như GPU AMD MI300X.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.minimax.io/models/text/m3">MiniMax M3 - Coding & Agentic Frontier, 1M Context, Multimodal | MiniMax</a></li>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek AI: R1 Reasoning, API & Local Deployment 2026</a></li>
<li><a href="https://app.semanticdiff.com/gh/vllm-project/vllm/pull/45744/overview">PR #45744 [M3] Enable FP8 sparse GQA - SemanticDiff</a></li>

</ul>
</details>

**Thẻ**: `#vLLM`, `#LLM inference`, `#MiniMax-M3`, `#DeepSeek-V4`, `#AMD ROCm`

---

<a id="item-2"></a>
## [Qwen 3.6 27B là điểm cân bằng lý tưởng cho LLM cục bộ](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 8.0/10

Bài viết trên quesma.com tvrdí rằng Qwen 3.6 27B cung cấp cân bằng tốt nhất giữa hiệu suất và khả năng phần cứng để chạy LLM tại địa phương, dựa trên việc chạy mô hình trên MacBook Pro 128 GB. Điều này đã gây ra một cuộc thảo luận chi tiết trên Hacker News về yêu cầu phần cứng, hiệu quả chi phí và tính hữu ích thực tế. Điều này nhấn mạnh một mô hình trọng lượng mở có thể chạy tại địa phương, giúp giảm sự phụ thuộc vào các API đám mây đắt giá và làm rõ sự trade‑off giữa đầu tư phần cứng ban đầu và chi phí suy luận liên tục. Cuộc thảo luận cũng phản ánh sự quan tâm rộng rãi của cộng đồng đến phát triển AI tiết kiệm chi phí và bảo mật riêng tư. Qwen 3.6 27B là mô hình đa phương thức đậm 27 tỷ tham số, được ra mắt ngày 22/04/2026, đạt 77,2% trên SWE‑bench Verified và có thể chạy trên GPU có VRAM 16‑24 GB. Luồng thảo luận trên Hacker News ghi nhận rằng MacBook Pro M5 128 GB có giá khoảng 6.699 USD, trong khi ngân sách tương đương có thể mua nhiều crédito suy luận đám mây hơn trên các dịch vụ như OpenRouter.

hackernews · stared · 29/6 17:05 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48721903)

**Bối cảnh**: Qwen 3.6 27B là phần tiếp theo của 系列 Qwen 3.5 và vượt qua flagship trước đó Qwen 3.5‑397B MoE trên các benchmark code trong khi cần phần cứng ít hơn nhiều. Việc triển khai LLM tại địa phương vào năm 2026 chủ yếu phụ thuộc vào VRAM của GPU, với các hướng dẫn đề xuất các cấp độ từ cơ bản đến cao cấp cho mô hình ở quy mô này. Các dịch vụ suy luận tiết kiệm chi phí như Wafer Scale Engine của Cerebras cung cấp giá thấp tới 0,10 USD mỗi triệu token, tạo ra một lựa chọn đám mây thay cho việc chạy tại địa phương.

**Thảo luận cộng đồng**: Các bình luận viên khen ngợi hiệu suất của mô hình nhưng cảnh báo rằng việc chạy trên MacBook Pro gây quá nhiệt và tiếng quạt lớn, khiến nó không thực tế cho mã hóa hoạt động. Nhiều người cho rằng chi phí phần cứng cao vượt quá lợi ích, lưu ý rằng 10 USD dùng để mua crédito đám mây có thể truy cập các mô hình lớn hơn, trong khi một số người nhấn mạnh sự vui vẻ của việc 試 nghiệm tại địa phương dù kinh tế có thể không hiệu quả.

**Thẻ**: `#LLM`, `#Qwen`, `#local development`, `#AI hardware`, `#Hacker News discussion`

---

<a id="item-3"></a>
## [Rocket Lab mua lại Iridium, tạo doanh nghiệp không gian tích hợp](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

Rocket Lab công bố đã mua lại nhà điều hành vệ tinh thông tin Iridium, kết hợp dịch vụ phóng tên lửa của mình với vệ tinh LEO toàn cầu của Iridium để hình thành một doanh nghiệp không gian tích hợp từ khai phóng đến dịch vụ. Thỏa thuận này tạo ra một công ty không gian tích hợp dọc, kiểm soát cả quá trình phóng và cung cấp dịch vụ vệ tinh, có thể giảm chi phí và tăng độ tin cậy cho khách hàng, đồng thời đặt Rocket Lab ở vị trí cạnh tranh trực tiếp hơn với các đối thủ lớn như SpaceX. Iridium vận hành một cụm vệ tinh bao gồm 66 vệ tinh LEO hoạt động cung cấp dịch vụ thoại và dữ liệu dải L‑band trên toàn cầu. Tên lửa Electron của Rocket Lab đã thực hiện hơn 75 nhiệm vụ, và công ty đang phát triển tên lửa Neutron lớn hơn, dự kiến ra mắt năm 2024, có thể được sử dụng để bổ sung đội ngũ vệ tinh Iridium.

hackernews · everfrustrated · 29/6 14:09 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48719485)

**Bối cảnh**: Hệ thống vệ tinh Iridium là một mạng lưới vệ tinh quỹ đạo thấp Trái Đất (LEO) cung cấp phủ sóng toàn cầu về thoại và dữ liệu dải L‑band cho điện thoại vệ tinh và thiết bị thu phát. Rocket Lab là nhà cung cấp dịch vụ phóng tên lửa, nổi tiếng với tên lửa Electron chuyên phóng các vệ tinh nhỏ, và đang phát triển tên lửa Neutron lớn hơn. Một doanh nghiệp không gian tích hợp từ khai phóng đến dịch vụ kết hợp hoạt động phóng tên lửa, sản xuất vệ tinh, hạ tầng mặt đất và dịch vụ khách hàng cuối cùng dưới một công ty duy nhất.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab">Rocket Lab - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/smallsat-institute/sst-soa/integration-launch-and-deployment/">10.0 Integration, Launch, and Deployment - NASA</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận 者 nhấn mạnh những lợi thế chiến lược của vụ mua lại, như lượng phóng được bảo đảm và tích hợp dọc, đồng thời lo ngại về lượng rác không gian tăng lên, chi phí sử dụng Iridium trước đây cao và cảm nhận rằng Rocket Lab đã rời khỏi nguồn gốc New Zealand. Một số người so sánh giao dịch này với các tình huống trong khoa học viễn tưởng.

**Thẻ**: `#space`, `#satellite communications`, `#acquisition`, `#Rocket Lab`, `#Iridium`

---

<a id="item-4"></a>
## [Ornith-1.0: Gia đình LLM cấp phép MIT cho mã hoá tác động tới 397B](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

Ornith-1.0 là gia đình mô hình LLM trọng lượng mở cấp phép MIT được phát hành bởi DeepReinforce, dựa trên Gemma 4 và Qwen 3.5, cung cấp các biến thể dense và mixture-of-experts từ 9B đến 397B tham số. Nó đạt hiệu suất state-of-the-art trên các benchmark mã nguồn mở có quy mô tương đương. Bản phát hành cung cấp các mô hình mạnh mẽ, cấp phép mở cho phép nhà phát triển chạy các trợ lý mã hoá tác động nâng cao ở local, giảm sự phụ thuộc vào API độc quyền. Điều này thúc đẩy hệ sinh thái AI mã nguồn mở và mở rộng quyền truy cập vào các công cụ tạo mã chất lượng cao. Các biến thể bao gồm 9B Dense, 31B Dense, 35B MoE và 397B MoE; mô hình cơ sở Gemma 4 và Qwen 3.5 đều được cấp phép Apache 2.0, khiến giấy phép MIT tương thích. Tác giả đã kiểm tra phiên bản GGUF 35B (khoảng 20 GB) trên LM Studio, thấy thực thi harness tác động suôn sẻ và tốc độ vẽ khoảng 103 token/giây.

rss · Simon Willison · 29/6 16:17

**Bối cảnh**: Self-scaffolding là một phương pháp huấn luyện trong đó mô hình học cách tạo cả các bản thử nghiệm giải pháp và các dây cụt đặc 定 cho nhiệm vụ để hướng dẫn những bản thử nghiệm đó, đồng thời tối ưu hóa cả dây cụt và giải pháp để có trajectoires tìm kiếm tốt hơn. Kiến trúc Mixture‑of‑experts (MoE) chia các lớp feed‑forward thành nhiều subnetwork chuyên gia, định tuyến token tới một phần nhỏ các chuyên gia để tăng khả năng mà vẫn giữ mức tính toán thấp. Agentic coding sử dụng LLM trong một vòng lặp gồm lập kế hoạch, sử dụng công cụ, quan sát và sửa đổi để tự động viết và sửa đổi mã. Gemma 4 và Qwen 3.5 là các mô hình ngôn ngữ được đào tạo trước gần đây, được phát hành dưới giấy phép Apache 2.0, cung cấp nền tảng cho phép cho các công trình derivative.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://medium.com/data-science-in-your-pocket/ornith-1-0-self-learning-llm-for-coding-318c9a830bfc">Ornith 1.0 : Self Learning LLM for Coding | by Mehul Gupta | Data Science in Your Pocket | Jun, 2026 | Medium</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://scrimba.com/articles/what-is-agentic-coding/">What Is Agentic Coding ? A Developer's Guide [2026]</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#coding`, `#open-source`, `#agentic AI`, `#model release`

---

<a id="item-5"></a>
## [Đề xuất tên miền .self miễn phí cho tự lưu trữ](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 6.0/10

Một đề xuất giới thiệu một tên miền cấp cao mới .self sẽ cung cấp miễn phí các tên miền tập trung con người để cá nhân tự lưu trữ dịch vụ trực tuyến của họ. Ý tưởng này gây ra cuộc tranh luận về danh tính số, quản trị và phòng ngừa lạm dụng, nhấn mạnh sự đối lập giữa truy cập mở và lạm dụng trong hệ sinh thái tên miền. Kế hoạch dự định mỗi người sẽ nhận một tên miền .self miễn phí, cấm đỗ hoặc bán lại, và dựa vào quyên góp hoặc nguồn tài chính khác để chi trả chi phí hoạt động của TLD.

hackernews · HumanCCF · 29/6 19:49 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48724230)

**Bối cảnh**: Tên miền cấp cao (TLD) là đoạn cuối cùng của một tên miền, được quản lý bởi IANA và giám sát bởi ICANN cho các bổ sung mới. Self-hosting là việc chạy và duy trì website hoặc dịch vụ trên máy chủ cá nhân thay vì sử dụng nhà cung cấp bên thứ ba. Lịch sử, các TLD miễn phí như .tk đã được người dùng cá nhân sử dụng rộng rãi nhưng sau đó gặp phải lạm dụng, dẫn đến việc bị chặn bởi các nền tảng lớn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains">List of Internet top-level domains - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Top-level_domain">Top-level domain - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận cảnh báo rằng các tên miền miễn phí có thể thu hút kẻ lừa đảo như trường hợp .tk, đặt ra câu hỏi về cách tài trợ cho TLD mà không cần phí đăng ký, và tranh luận về mô hình xác thực cũng như cơ chế thu hồi tên miền không hoạt động để ngăn chặn chiếm đoán.

**Thẻ**: `#domain`, `#TLD`, `#self-hosting`, `#internet governance`, `#identity`

---