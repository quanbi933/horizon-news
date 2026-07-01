---
layout: default
title: "Horizon Summary: 2026-07-01 (ZH)"
date: 2026-07-01
lang: zh
---

> Đã chọn 7 tin quan trọng từ 17 nội dung.

---

1. [Anthropic ra mắt Claude Sonnet 5, mô hình LLM tập trung vào tính agentic](#item-1) ⭐️ 8.0/10
2. [Claude Code nhúng dấu ẩn steganography để phát hiện việc model distillation](#item-2) ⭐️ 8.0/10
3. [Anthropic ra mắt Claude Science, công cụ AI hỗ trợ nghiên cứu](#item-3) ⭐️ 8.0/10
4. [Ollama v0.31.1 mang lại tăng tốc ~90% cho Gemma 4 trên Apple Silicon](#item-4) ⭐️ 7.0/10
5. [Google DeepMind ra mắt Gemini Image Flash Lite (Nano Banana 2 Lite)](#item-5) ⭐️ 7.0/10
6. [Shot-scraper 1.10 thêm lệnh video để ghi lại demo của agent](#item-6) ⭐️ 7.0/10
7. [Mỹ gỡ bỏ xuất khẩu Claude Fable 5 và Mythos 5](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic ra mắt Claude Sonnet 5, mô hình LLM tập trung vào tính agentic](https://www.anthropic.com/news/claude-sonnet-5) ⭐️ 8.0/10

Anthropic đã ra mắt Claude Sonnet 5 vào tháng 6/2026, một mô hình LLM đa phương tiense trung bình được thiết kế để thể hiện hành vi agentic như lập kế hoạch, sử dụng công cụ và hoạt động tự chủ. Việc ra mắt này nhấn mạnh tầm quan trọng ngày càng tăng của các LLM agentic trong việc tự động hoá quy trình phức tạp, đồng thời gây ra cuộc thảo luận về các trade‑off chi phí‑hiệu suất so với các mô hình lớn như Opus. Claude Sonnet 5 cung cấp đầu vào đa phương tiện, truy cập API và khả năng gọi công cụ được nâng cao, nhưng các benchmark cộng đồng cho thấy chi phí mỗi nhiệm vụ cao hơn Opus ở mức độ medium trở lên và hiệu suất kém hơn trong các bài kiểm tra trivia và phát hiện lỗ hổng.

hackernews · marinesebastian · 30/6 17:59 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48736605)

**Bối cảnh**: Gia đình Claude của Anthropic bao gồm Haiku (nhỏ nhất), Sonnet (trung bình) và Opus (lớn nhất), trong đó Sonnet thường là lựa chọn trung gian linh hoạt cho các nhà phát triển. Dòng Sonnet đã phát triển từ các phiên bản 3.5‑3.7, lần đầu tiên thể hiện khả năng mã hóa và sử dụng công cụ mạnh mẽ, đánh dấu thời đại ban đầu của AI agentic. Các LLM agentic là các mô hình ngôn ngữ kết hợp bộ nhớ, lập kế hoạch và tích hợp công cụ để thực hiện tự chủ các nhiệm vụ nhiều bước.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-5">Introducing Claude Sonnet 5 \ Anthropic</a></li>
<li><a href="https://llm-stats.com/models/claude-sonnet-5">Claude Sonnet 5 Benchmarks, Pricing & Context Window</a></li>
<li><a href="https://labs.adaline.ai/p/what-are-agentic-llms-a-comprehensive">What Are Agentic LLMs? Use Cases, Risks, and How They Work</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận cho rằng chi phí mỗi nhiệm vụ của Sonnet 5 vượt 過 Opus ở mức độ medium hoặc cao hơn, cho thấy Opus vẫn còn hiệu quả về chi phí cho nhiều công việc. Một số người dùng nhấn mạnh khả năng agentic mạnh mẽ hơn của nó, như lập kế hoạch và sử dụng công cụ, có thể giảm nhu cầu sử dụng mô hình lớn hơn trong các quy trình tự chủ. Ngoài ra, có người chỉ ra những điểm yếu như kiến thức trivia limitado, độ chính xác khi gọi công cụ và khả năng phát hiện lỗ hổng, đồng thời thừa nhận lợi thế về tốc độ so với các mô hình tương đương.

**Thẻ**: `#Claude`, `#Sonnet 5`, `#LLM`, `#AI agents`, `#Anthropic`

---

<a id="item-2"></a>
## [Claude Code nhúng dấu ẩn steganography để phát hiện việc model distillation](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 8.0/10

Công cụ Claude Code của Anthropic đã được phát hiện nhúng dấu ẩn steganographic vào yêu cầu của người dùng để phát hiện việc sao chép mô hình (model distillation) bởi các công ty Trung Quốc. Việc đánh dấu ẩn này gây ra những lo ngại nghiêm trọng về sự trong suốt và niềm tin, vì người dùng không biết rằng yêu cầu của họ đang được vân tay, và nó thể hiện sự căng thẳng tăng dần giữa việc bảo vệ IP của nhà cung cấp AI và nhu cầu về hệ thống AI mở và có trách nhiệm. Các dấu ẩn được nhúng qua những thay đổi tinh vi trong định dạng yêu cầu, tồn tại trong quá trình truyền và có thể được trích xuất phía máy chủ để xác định yêu cầu xuất phát từ mô hình được 蒸馏; kỹ thuật này được mô tả là steganography underhanded và không thay đổi nội dung 可见 của prompt.

hackernews · kirushik · 30/6 15:44 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48734373)

**Bối cảnh**: Steganography là việc giấu thông tin bên trong dữ liệu thường thấy để không thể nhận ra bằng mắt thường. Model distillation là kỹ thuật huấn luyện một mô hình nhỏ hơn để mô phỏng hành vi của một mô hình AI lớn hơn, thường được sử dụng để sao chép khả năng độc quyền. Claude Code là công cụ mã hóa tác động của Anthropic, một hệ thống mã hóa tác động (agentic) đọc mã nguồn, chỉnh sửa tệp và chạy lệnh qua terminal, IDE, ứng dụng desktop và trình duyệt, và công ty thu thập dữ liệu sử dụng bao gồm các yêu cầu và phản hồi chấp nhận mã.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://wpnews.pro/news/claude-code-is-steganographically-marking-requests">Claude Code Is Steganographically Marking Requests — Web Pulse</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://github.com/anthropics/claude-code">anthropics/ claude - code : Claude Code is an agentic coding tool that...</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những bình luận viên chỉ trích sự thiếu trong suốt, đặt câu hỏi về đạo đức và hiệu quả của việc đánh dấu steganographic, và tranh luận về việc liệu điều này có gây hại cho người dùng hợp pháp không; một số người đề xuất sử dụng các lựa chọn mã nguồn mở hoặc AI địa phương để tránh việc theo dõi ẩn.

**Thẻ**: `#AI ethics`, `#steganography`, `#Claude Code`, `#model distillation`, `#transparency`

---

<a id="item-3"></a>
## [Anthropic ra mắt Claude Science, công cụ AI hỗ trợ nghiên cứu](https://claude.com/product/claude-science) ⭐️ 8.0/10

Anthropic đã ra mắt Claude Science, một nền tảng AI làm việc cho nhà khoa học chạy máy chủ local và cung cấp giao diện web, cho phép các nhà khoa học kết nối với cơ sở dữ liệu, công cụ tính toán và cụm institusional của họ. Nhờ kết nối dữ liệu và tính toán trong một môi trường duy nhất, Claude Science nhằm giảm bớt việc chuyển đổi ngữ cảnh cho nhà khoa học, đặc biệt là trong các môi trường có quy định chặt chẽ như dược phẩm, nơi việc kết nối trực tiếp laptop với dữ liệu bị hạn chế. Claude Science chạy một máy chủ local có giao diện web, tích hợp với nhiều cơ sở dữ liệu và hệ thống tính toán cao cấp (ví dụ công cụ Biomni HPC), và sử dụng một mô hình LLM được tối ưu cho nhiệm vụ khoa học thay vì ra mắt mô hình mới.

hackernews · lebovic · 30/6 17:07 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48735770)

**Bối cảnh**: Một nền tảng AI làm việc kết hợp mã, dữ liệu và tài nguyên tính toán trong một giao diện đơn để đơn hoá quy trình nghiên cứu. Thông thường, các nhà khoa học phải jongle giữa nhiều công cụ—cơ sở dữ liệu, notebooks và lịch trình công việc trên cụm—dẫn đến thiếu hiệu quả. Các cụm institusional là các tài nguyên tính toán cao cấp được chia sẻ mà tổ chức cung cấp cho mô phỏng lớn và xử lý dữ liệu. Khi chạy một máy chủ local kết nối với các cụm này, Claude Science cho phép các nhà khoa học giữ dữ liệu sau tường lửa mà vẫn truy cập được vào khả năng tính toán mạnh.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-science-ai-workbench">Claude Science, an AI workbench for scientists \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/06/30/anthropics-claude-science-bets-on-workflow-not-a-new-model-to-win-over-scientists/">Anthropic’s Claude Science bets on workflow, not a new model, to win over scientists | TechCrunch</a></li>
<li><a href="https://www.statnews.com/2026/06/30/anthropic-release-claude-science-ceo-dario-amodei/">Anthropic releases Claude Science, a product aimed at researchers, the pharma industry</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận nhấn mạnh giá trị của khả năng kết nối Claude Science với cụm institusional và công cụ chuyên dụng như Biomni HPC, đặc biệt trong các môi trường mà kết nối trực tiếp laptop‑dữ liệu bị chặn. Một số người dùng báo cáo đạt được kết quả thành công nhưng vừa phải trong các tác vụ chuyên biệt (ví dụ thiết kế RNAi thuốc trừ sâu), và chỉ ra rằng AI đôi khi áp dụng quy tắc chung và thiếu xác thực chuyên sâu. Một số người khác mong đợi sản phẩm tập trung nhiều hơn vào suy luận khoa học thay vì chỉ là notebook dữ liệu, cho thấy sự chênh lệch giữa mong đợi và khả năng hiện tại.

**Thẻ**: `#AI`, `#data science`, `#Anthropic`, `#research tools`, `#product launch`

---

<a id="item-4"></a>
## [Ollama v0.31.1 mang lại tăng tốc ~90% cho Gemma 4 trên Apple Silicon](https://github.com/ollama/ollama/releases/tag/v0.31.1) ⭐️ 7.0/10

Ollama v0.31.1 bật multi-token prediction và cập nhật các engine MLX và llama.cpp, giúp Gemma 4 trên Apple Silicon tạo token nhanh hơn khoảng 90% trung bình mà không cần cấu hình nào. Cải tiến này mang lại hiệu năng đáng kể cho người dùng Mac khi chạy LLM tại địa điểm, giảm độ trễ cho các agent coding và các ứng dụng khác mà không cần thiết lập thêm. Phiên bản này cải thiện việc tải mô hình MoE Gemma 4 trong engine MLX, thêm kernel ma trận nhỏ batch mới, nâng cấp llama.cpp lên bản build 9840 và nâng cao hiệu suất MTP.

github · github-actions[bot] · 30/6 22:10

**Bối cảnh**: Ollama là một công cụ phổ biến để chạy các mô hình ngôn ngữ lớn tại địa điểm trên nhiều phần cứng khác nhau. Gemma 4 là một mô hình Mixture-of-Experts của Google mà có thể được tối ưu bằng kỹ thuật giải đoán speculative như multi-token prediction. Các Mac Apple Silicon có thể tăng tốc suy luận qua framework MLX, trong khi llama.cpp cung cấp một backend suy luận C++ được sử dụng rộng rãi.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://ollama.com/blog/faster-gemma-4-mlx-mtp">Faster Gemma 4 on MLX with multi-token prediction · Ollama Blog</a></li>
<li><a href="https://medium.com/@ion.stefanache0/multi-token-prediction-mtp-and-ollama-the-local-llm-server-6d8d8d61157e">Multi-Token Prediction(MTP) and Ollama (the local LLM-server) on RTX-4060/8GB VRAM(as GPU-card) | by Ion | May, 2026 | Medium</a></li>
<li><a href="https://macgpu.com/en/blog/2026-0402-mac-metalrt-mlx-llamacpp-local-llm-engine-comparison.html">2026 MetalRT / MLX / llama.cpp on Mac: Engine Comparison & Tuning</a></li>

</ul>
</details>

**Thẻ**: `#ollama`, `#gemma-4`, `#apple-silicon`, `#performance`, `#mlx`

---

<a id="item-5"></a>
## [Google DeepMind ra mắt Gemini Image Flash Lite (Nano Banana 2 Lite)](https://deepmind.google/models/gemini-image/flash-lite/) ⭐️ 7.0/10

Google DeepMind đã phát hành Gemini Image Flash Lite, còn được gọi là Nano Banana 2 Lite, một mô hình tạo ảnh được distilled tạo ra khoảng 1.000 ảnh trong khoảng 4 giây và cung cấp khả năng render văn bản tốt hơn so với phiên bản trước, mặc dù không hỗ trợ kiểm soát tỉ lệ khung hình chi tiết. Tốc độ và chi phí thấp của mô hình cho phép tạo ảnh thực thi lượng lớn và thời gian thực cho các ứng dụng như thiết kế UI, quảng cáo và công cụ giáo dục, đồng thời khả năng render văn bản tốt hơn cải thiện khả năng sử dụng cho các thiết kế cần tipografi rõ ràng. Mô hình được xây dựng trên Gemini 3.1 Flash‑Lite, là phiên bản distilled của một mô hình ảnh Gemini lớn hơn, hỗ trợ đầu vào đa phương (văn bản, hình ảnh, video, âm thanh, PDF), chi phí khoảng 0,034 USD mỗi 1.000 ảnh, nổi bật về render văn bản nhưng không cho phép điều khiển tỉ lệ khung hình theo chương trình.

hackernews · minimaxir · 30/6 16:48 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48735444)

**Bối cảnh**: Phương pháp distillation chuyển 移 kiến thức từ một mô hình AI lớn và mạnh mẽ sang một mô hình nhỏ hơn, nhanh hơn mà vẫn giữ lại hầu hết các khả năng. Gemini 3.1 Flash‑Lite thuộc 系列 Gemini 3 của Google, được thiết kế để là mô hình đa phương thức thấp latency và hiệu quả chi phí cho các tác vụ tần suất cao. Thương hiệu Nano Banana là dòng mô hình tạo ảnh hiệu quả của DeepMind, trong đó Nano Banana 2 Lite là phiên bản distilled mới nhất.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini-image/flash-lite/">Gemini 3.1 Flash- Lite Image – Nano Banana ... — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-lite">Gemini 3.1 Flash-Lite | Gemini API | Google AI for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận khen ngợi tốc độ ấn tượng và khả năng render văn bản tốt hơn, thấy hữu ích cho việc tạo mẫu nhanh và ứng dụng truyện tranh cho trẻ em. Một số chỉ ra việc thiếu khả năng kiểm soát tỉ lệ khung hình và yêu cầu phải có tài khoản Google One để sử dụng bản demo AI Studio, đồng thời lo ngại về việc sử dụng hình ảnh tạo bởi AI để che giấu bất động sản kém chất lượng. Một số cũng chỉ ra sự vắng mặt của ChatGPT trong bảng so sánh hiệu suất là một điểm thiếu sót.

**Thẻ**: `#AI image generation`, `#Google DeepMind`, `#Gemini`, `#multimodal models`, `#model distillation`

---

<a id="item-6"></a>
## [Shot-scraper 1.10 thêm lệnh video để ghi lại demo của agent](https://simonwillison.net/2026/Jun/30/shot-scraper-video/#atom-everything) ⭐️ 7.0/10

Phiên bản shot-scraper 1.10, phát hành ngày 30/6/2026, ra mắt lệnh mới `video` để ghi lại demo của ứng dụng web dựa trên file `storyboard.yml` bằng Playwright. Điều này cho phép các agent AI và nhà phát triển tạo ra video demo chia sẻ về quy trình làm việc, giúp trong việc gỡ lỗi, tài liệu và hợp tác mà không cần công cụ bổ sung. Lệnh này đọc file YAML storyboard mô tả việc khởi động máy chủ, URL, viewport, con trỏ, selector chờ đợi và JavaScript tùy chỉnh, sau đó dùng Playwright để ghi lại phiên làm việc thành file MP4 hoặc WebM; tùy chọn `--auth` cung cấp cookie cho các trang cần xác thực.

rss · Simon Willison · 30/6 16:54

**Bối cảnh**: Shot-scraper là tiện ích dòng lệnh để chụp màn hình và tự động hóa tương tác web. Playwright là framework kiểm thử end-to-end đa trình duyệt cung cấp tự động hóa đáng tin cậy với tính năng auto‑wait. File storyboard.yml mô tả một chuỗi hành động (như khởi động máy chủ, điều hướng, nhấp) mà shot-scraper có thể thực hiện và ghi lại.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/simonw/shot-scraper">GitHub - simonw/shot-scraper: A command-line utility for ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Playwright_(software)">Playwright (software) - Wikipedia</a></li>
<li><a href="https://playwright.dev/">Playwright</a></li>

</ul>
</details>

**Thẻ**: `#shot-scraper`, `#web automation`, `#video recording`, `#developer tools`, `#Playwright`

---

<a id="item-7"></a>
## [Mỹ gỡ bỏ xuất khẩu Claude Fable 5 và Mythos 5](https://twitter.com/AnthropicAI/status/2072106151890809341) ⭐️ 6.0/10

Bộ Thương mại Mỹ đã thông báo rằng đã gỡ bỏ kiểm soát xuất khẩu đối với các mô hình AI Claude Fable 5 và Mythos 5 của Anthropic, theo một bức thư ngày 30/6/2026 được gửi tới Chief Compute Officer Tom Brown của Anthropic. Điều này xảy ra sau các bức thư trước đó ngày 12/6 và 26/6/2026, trong đó chính phủ phối hợp với Anthropic để xử lý các rủi ro liên quan đến các mô hình này. Quyết định này làm nổi bật sự không thể đoán trước của chính sách xuất khẩu AI của Mỹ, có thể làm giảm niềm tin của nhà đầu tư và doanh nghiệp dựa vào các mô hình tiên tiến để thực hiện các chức năng quan trọng. Nó cũng kích hoạt tranh luận về việc liệu các biện pháp kiểm soát có nên được thay thế bằng luật pháp rõ ràng, có thể dự đoán để hỗ trợ phát triển AI bền vững. Mặc dù lệnh cấm xuất khẩu đã được gỡ bỏ, Anthropic đã thêm bộ phân loại mới vào Claude Fable 5 để chặn các tác vụ liên quan đến an ninh mạng, khiến các tác vụ code và debug thường xuyên phải quay lại sử dụng mô hình Opus 4.8. Cả Claude Fable 5 và Mythos 5 đều được mô tả là đạttat‑the‑art, vượt qua các chuẩn mốc trước đó trong lĩnh vực phát triển phần mềm, công việc kiến thức, thị giác và nghiên cứu khoa học.

hackernews · Pragmata · 30/6 23:55 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48740771)

**Bối cảnh**: Kiểm soát xuất khẩu là các hạn chế của chính phủ Mỹ về việc chuyển giao một số công nghệ cao급, bao gồm mô hình AI, sang thực thể nước ngoài để bảo vệ an ninh quốc gia. Loại mô hình Claude của Anthropic bao gồm Opus, Sonnet, Haiku và các biến thể mới như Fable và Mythos, trong đó Fable 5 được quảng cáo là mô hình mạnh nhất dành cho việc viết mã và các tác vụ tự trị phức tạp. Bức thư của Bộ Thương mại Mỹ vào tháng 6/2026 cho thấy, sau khi phối hợp với Anthropic, chính phủ đã xác định rủi ro có thể được quản lý, từ đó cho phép xuất khẩu lại các mô hình này.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5</a></li>
<li><a href="https://www.bbc.com/news/articles/cdr42623e1do">Fable and Mythos : Anthropic says US lifts export ban on its advanced...</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận cho biết việc thay đổi không thể dự đoán về kiểm soát xuất khẩu làm mất niềm tin đối với các nhà cung cấp AI Mỹ và gây khó khăn trong lập kế hoạch dài hạn. Một số người cho rằng sự thiếu sót của luật pháp rõ ràng có thể dẫn đến lạm dụng và làm giảm đầu tư vào các công ty AI Mỹ, trong khi những người khác đặt câu hỏi về hiệu quả của kiểm soát xuất khẩu khi các mô hình Trung Quốc ngày càng cạnh tranh.

**Thẻ**: `#AI policy`, `#export controls`, `#Anthropic`, `#AI regulation`, `#Hacker News`

---