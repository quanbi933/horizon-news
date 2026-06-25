---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> Đã chọn 8 tin quan trọng từ 10 nội dung.

---

1. [OpenAI ra mắt chip AI suy luận Jalapeno do Broadcom thiết kế](#item-1) ⭐️ 9.0/10
2. [Gefen là tối ưu thay thế trực tiếp cho AdamW, giảm 8× bộ nhớ](#item-2) ⭐️ 8.0/10
3. [Toà án Thụy Sĩ đánh giá Heretic để giảm can thiệp LLM quá mức](#item-3) ⭐️ 7.0/10
4. [Unlimited-OCR đã có trên ModelScope! Mô hình OCR đa ngôn ngữ 3,3B tham số để phân tích một lần trên hình ảnh đơn, tài liệu nhiều trang và PDF. Giấy phép: MIT](#item-4) ⭐️ 7.0/10
5. [RubyLLM: Một framework Ruby cho các nhà cung cấp AI chính](#item-5) ⭐️ 6.0/10
6. [Simon Willison phát hành cơ sở dữ liệu SQLite truy vấn được về tính tương thích trình duyệt](#item-6) ⭐️ 6.0/10
7. [Tom MacWright cảnh báo rằng CV được tạo bởi LLM làm mất tính cá nhân](#item-7) ⭐️ 6.0/10
8. [Gemma4-26B-A4B & 31B-QAT Không Lọc Cân Bằng đã ra mắt ra (tăng tốc  mắt với MTP (tăng tốc 35% & 53%)!](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI ra mắt chip AI suy luận Jalapeno do Broadcom thiết kế](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI đã công bố chip AI suy luận đầu tiên tên Jalapeno, được thiết kế cùng Broadcom và sản xuất bởi TSMC, nhằm nâng cao hiệu suất suy luận LLM. Điều này cho thấy OpenAI đang chuyển sang kiểm soát phần cứng AI của mình, giảm sự phụ thuộc vào GPU Nvidia và có thể giảm chi phí suy luận quy mô lớn. Jalapeno là một ASIC có kích thước reticle, được phát triển trong chín tháng, sử dụng quy trình 3 纳米 của TSMC, tích hợp kiến trúc mảng systolic và băng thông bộ nhớ cao để cân bằng tài nguyên tính toán và bộ nhớ.

hackernews · jamdesk · 24/6 17:47 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48663324)

**Bối cảnh**: Các chip AI tùy chỉnh là các mạch tích hợp đặc thù ứng dụng (ASIC) được thiết kế để tăng tốc các workload cụ thể như suy luận mô hình ngôn ngữ lớn, cung cấp hiệu suất và hiệu năng năng lượng tốt hơn so với GPU dùng chung. TSMC là nhà sản xuất pół dẫn hàng đầu, chịu trách nhiệm sản xuất các thiết kế tùy chỉnh cho các công ty như Google, Amazon và Microsoft bằng cách sử dụng các quy trình tiến bộ như 3 纳米. Broadcom cung cấp chuyên môn về việc chuyển đổi kiến trúc chip thành silicon có thể sản xuất, bao gồm các giao diện tốc độ cao và thực hiện ASIC, thường đóng vai trò là nhà phát triển chung trong các dự án bán tùy chỉnh.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip | OpenAI</a></li>
<li><a href="https://www.klover.ai/tsmc-ai-fabricating-dominance-chip-manufacturing-leadership-ai-era/">TSMC AI Fabricating Dominance: Chip Manufacturing Leadership in AI Era - Klover.ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/Broadcom">Broadcom - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận bày tỏ sự entusiasmo về tiềm năng tăng hiệu suất từ chip suy luận tùy chỉnh, đồng thời cũng có sự hoài nghi rằng chu kỳ phát triển chín tháng có thể bị overstated như một chiến lược marketing. Một số người dùng quan tâm đến kiến trúc nhúng trực tiếp trọng số mô hình vào ROM hoặc bộ nhớ trên chip, và đề cập đến các dự án như Taalas mà họ cho là mang lại cải thiện lớn về độ trễ và chi phí.

**Thẻ**: `#OpenAI`, `#custom AI chip`, `#Broadcom`, `#TSMC`, `#AI hardware`

---

<a id="item-2"></a>
## [Gefen là tối ưu thay thế trực tiếp cho AdamW, giảm 8× bộ nhớ](https://www.reddit.com/r/LocalLLaMA/comments/1uep96s/gefen_is_a_dropin_replacement_for_the_adamw/) ⭐️ 8.0/10

Gefen, được giới thiệu trong bài báo arXiv ngày 11 / 6 / 2026 và công khai trên GitHub, là thay thế trực tiếp cho AdamW giảm tối đa 8× bộ nhớ trạng thái tối ưu mà vẫn duy trì hiệu suất tương đương AdamW. Bộ nhớ tối ưu là một trong những chặn nghẽn lớn khi huấn luyện mô hình lớn; việc giảm 8× cho phép đặt mô hình lớn hơn hoặc batch lớn hơn trên cùng phần cứng, từ đó giảm chi phí và tiêu thụ năng lượng. Gefen tạo ra một mã hóa codebook dựa trên histogram và lập trình động chính xác, sau đó tái sử dụng các khối này để mở rộng moment đầu tiên, tiết kiệm khoảng 6,5 GiB mỗi tỷ tham số so với AdamW.

reddit · r/LocalLLaMA · /u/indicava · 24/6 20:39

**Bối cảnh**: AdamW lưu trữ hai vector phụ trợ (moment đầu và moment hai) cho mỗi tham số mô hình, điều này có thể tiêu thụ hàng gigabyte bộ nhớ trong các mô hình lớn. Việc giảm bộ nhớ trạng thái tối ưu là yếu tố then chốt để cho phép huấn luyện các mô hình lớn hơn trên phần cứng có giới hạn. Gefen giải quyết vấn đề này bằng cách lượng tử hóa các vector moment bằng một mã hóa codebook được học, duy trì hành vi mở rộng tương ứng trong khi giảm đáng kể bộ nhớ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.13894">[2606.13894] Gefen: Optimized Stochastic Optimizer - arXiv.org</a></li>
<li><a href="https://github.com/ndvbd/Gefen">GitHub - ndvbd/Gefen: Gefen: Optimized Stochastic Optimizer</a></li>

</ul>
</details>

**Thẻ**: `#optimizer`, `#AdamW`, `#memory efficiency`, `#deep learning`, `#training`

---

<a id="item-3"></a>
## [Toà án Thụy Sĩ đánh giá Heretic để giảm can thiệp LLM quá mức](https://www.reddit.com/r/LocalLLaMA/comments/1ueeund/the_swiss_federal_supreme_court_is_evaluating/) ⭐️ 7.0/10

Toà án Liên bang Thụy Sĩ đang đánh giá phương pháp Heretic để giảm thiểu hiện tượng can thiệp quá mức (over‑alignment) của mô hình ngôn ngữ lớn trong các tác vụ pháp luật hình sự đa ngôn ngữ, dựa trên bài nghiên cứu gần đây. Việc đánh giá này cho thấy một cơ quan pháp lý thực tế đang áp dụng giải pháp kỹ thuật để khắc phục vấn đề từ chối của LLM, thể hiện sự tương tác ngày càng tăng giữa nghiên cứu an toàn AI và thực tiễn tư pháp. Điều này có thể ảnh hưởng đến cách các tòa án sử dụng AI cho công việc pháp lý đa ngôn ngữ và thúc đẩy việc phát triển các hướng dẫn quản trị. Phương pháp Heretic tự động loại bỏ sự can thiệp an toàn (censorship) khỏi các mô hình ngôn ngữ transformer mà không cần huấn luyện lại đắt costo, và phần 5.2 của bài báo cho thấy kết quả tốt trên benchmark TF‑RefusalBench bao gồm các lời nhắc bằng Pháp, Đức, Ý và Anh.

reddit · r/LocalLLaMA · /u/-p-e-w- · 24/6 14:19

**Bối cảnh**: Hiện tượng can thiệp quá mức xảy ra khi các LLM từ chối các yêu cầu hợp pháp do huấn luyện an toàn quá nghiêm ngặt, gây hạn chế trong việc áp dụng chúng vào các lĩnh vực chuyên môn như pháp luật hình sự. Các nhà nghiên cứu đã xây dựng các benchmark đa ngôn ngữ như TF‑RefusalBench để đo lường vấn đề này và kiểm tra các kỹ thuật giảm thiểu như abliteration và Heretic. Toà án Liên bang Thụy Sĩ, đang gặp phải vấn đề từ chối tương tự, hiện đang thử Heretic để xem liệu nó có thể cải thiện sự tuân thủ của mô hình đồng thời vẫn giữ an toàn khi cần.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.23375v1">Measuring & Mitigating Over-Alignment for LLMs in Multilingual Criminal ...</a></li>
<li><a href="https://github.com/p-e-w/heretic">Heretic: Fully automatic censorship removal for language models</a></li>

</ul>
</details>

**Thẻ**: `#LLM alignment`, `#AI law`, `#Heretic`, `#over-alignment`, `#Swiss Federal Supreme Court`

---

<a id="item-4"></a>
## [Unlimited-OCR đã có trên ModelScope! Mô hình OCR đa ngôn ngữ 3,3B tham số để phân tích một lần trên hình ảnh đơn, tài liệu nhiều trang và PDF. Giấy phép: MIT](https://www.reddit.com/r/LocalLLaMA/comments/1ue51uk/unlimitedocr_is_now_on_modelscope_a_33b/) ⭐️ 7.0/10

Unlimited-OCR là mô hình OCR đa ngôn ngữ có 3,3 tỷ tham số, được phát hành dưới giấy phép MIT, cho phép phân tích toàn bộ tài liệu với đầu ra chuỗi dài và các tùy chọn triển khai linh hoạt.

reddit · r/LocalLLaMA · /u/Sporeboss · 24/6 05:53

**Thẻ**: `#OCR`, `#multilingual`, `#document‑parsing`, `#MIT‑license`, `#Transformers`

---

<a id="item-5"></a>
## [RubyLLM: Một framework Ruby cho các nhà cung cấp AI chính](https://rubyllm.com/) ⭐️ 6.0/10

RubyLLM được ra mắt như một gem Ruby cung cấp lớp trừu tượng thống nhất để tương tác với nhiều nhà cung cấp AI như OpenAI, Claude và Ollama, cho phép nhà phát triển xây dựng các ứng dụng chat, hình ảnh, nhúng và công cụ bằng mã nguồn tối thiểu. Nhờ cung cấp một API nhất quán giữa các dịch vụ LLM khác nhau, RubyLLM giảm thiểu rào cản cho nhà phát triển Ruby khi áp dụng tính năng AI, từ đó thúc đẩy việc tạo mẫu nhanh và dễ dàng chuyển đổi giữa các nhà cung cấp. RubyLLM chỉ cần ba phụ thuộc—Faraday, Zeitwerk và Marcel—and cung cấp các tính năng như streaming, đầu ra JSON có cấu trúc, trừu tượng agent và tích hợp Rails qua acts_as_chat. Tuy nhiên, một số người dùng báo cáo vấn đề về cache (ví dụ với xAI) và khó kh đo lường lại các lần thử lại để quan sát truy vết.

hackernews · doener · 24/6 14:41 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48660711)

**Bối cảnh**: Các mô hình ngôn ngữ lớn (LLM) là mô hình học sâu được đào tạo trên bộ dữ liệu văn bản khổng lồ để tạo ra và hiểu ngôn ngữ con người, stanowi nền tảng cho các dịch vụ như GPT‑4, Claude và các phiên bản Ollama cục bộ. Trong hệ sinh thái Ruby, các nhà phát triển thường phải sử dụng các gem riêng biệt (ví dụ gem cho OpenAI hoặc Gemini) để gọi các API này, dẫn đến mã lặp lại khi thay đổi nhà cung cấp. RubyLLM gom các tương tác này vào một giao diện độc lập với nhà cung cấp, giảm thiểu mã boilerplate và đơn giản hoá việc xây dựng ứng dụng Ruby có tích hợp AI.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers. Chat, images, embeddings, tools.</a></li>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ruby_llm: One delightful Ruby framework for every major AI provider. Build AI agents, chatbots, RAG apps, and multimodal workflows in beautiful, expressive code. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những bình luận thường khen RubyLLM vì sự dễ sử dụng và API sạch, so sánh với framework AI của Vercel, đồng thời chỉ ra những hạn chế như cache không ổn định (đặc biệt với xAI), khả năng quan sát truy vết hạn chế do cơ chế retry xóa mô hình, và đôi khi phản hồi từ người bảo trì chậm. Nhiều người dùng chia sẻ về việc sử dụng thành công trong hơn sáu tháng, các phần mở rộng cộng đồng như Raix, và mong chờ phiên bản 2.0, đồng thời xác nhận rằng API responses hiện đã được hỗ trợ bản địa.

**Thẻ**: `#Ruby`, `#AI`, `#LLM`, `#framework`, `#gem`

---

<a id="item-6"></a>
## [Simon Willison phát hành cơ sở dữ liệu SQLite truy vấn được về tính tương thích trình duyệt](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 6.0/10

Simon Willison đã chuyển đổi kho lưu trữ browser‑compat‑data của MDN thành một cơ sở dữ liệu SQLite khoảng 66 MB và công bố nó trên GitHub với tiêu đề CORS mở. Kho lưu trữ bao gồm một script tạo dựng được xây dựng bằng sqlite‑utils và một quy trình GitHub Actions cập nhật cơ sở dữ liệu và đẩy nó lên một nhánh orphan. Các nhà phát triển có thể truy vấn dữ liệu tương thích trình duyệt tại địa phương hoặc qua Datasette Lite, cho phép phân tích ngoại tuyến và tích hợp vào công cụ tùy chỉnh mà không cần dựa vào API web của MDN. Điều này nâng cao hiệu quả quy trình làm việc cho các nhà phát triển web xây dựng các trang web tương thích đa nền tảng. Cơ sở dữ liệu có dung lượng khoảng 66 MB, được xây dựng bằng thư viện Python sqlite‑utils qua script tên build_db.py, và được làm mới bởi một quy trình GitHub Actions که force‑push file đã cập nhật lên nhánh orphan db. Nó được cung cấp trực tiếp từ GitHub với CORS được bật và có thể được khám phá ngay lập tức bằng Datasette Lite.

rss · Simon Willison · 24/6 23:59

**Bối cảnh**: Bộ dữ liệu browser‑compat‑data của MDN là một tập dữ liệu JSON được cộng đồng duy trì, ghi lại các tính năng của nền tảng web được hỗ trợ trong từng phiên bản trình duyệt chính. SQLite là một engine cơ sở dữ liệu dựa trên file, không cần máy chủ, cho phép lưu trữ nhẹ và truy vấn SQL nhanh mà không cần tiến trình máy chủ riêng. Datasette Lite là một công cụ phía client có thể mở bất kỳ tệp SQLite nào được lưu trữ trực tuyến và cung cấp giao diện SQL tương tác trong trình duyệt, trong khi GitHub Actions tự động hoá quy trình xây dựng và xuất bản, và các tiêu đề CORS mở cho phép tệp được lấy từ bất kỳ nguồn gốc nào.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>
<li><a href="https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/">Introducing the MDN MCP server - MDN Web Docs</a></li>

</ul>
</details>

**Thẻ**: `#browser-compatibility`, `#SQLite`, `#web-development`, `#data-tools`, `#SimonWillison`

---

<a id="item-7"></a>
## [Tom MacWright cảnh báo rằng CV được tạo bởi LLM làm mất tính cá nhân](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 6.0/10

Trong tháng 6 năm 2026, Tom MacWright đã quan sát thấy các đơn xin việc được viết chung với LLM rõ ràng, liên kết tới trang portfolio và kho GitHub được tạo bởi LLM, cùng với thông điệp commit cũng được LLM sinh ra, khiến ông không thể biết gì về ứng viên ngoài việc họ dùng công cụ nào. Xu hướng này cho thấy việc sử dụng tài liệu xin việc do AI tạo ra có thể làm mất đi tính cá nhân, khiến nhà tuyển dụng khó đánh giá được kỹ năng và sự phù hợp thực sự của ứng viên, đồng thời gây ra lo ngại về sự phụ thuộc quá mức vào LLM trong quá trình tìm việc. MacWright ghi nhận rằng CV, trang portfolio, lịch sử GitHub và thông điệp commit đều được tạo bởi LLM, và mô tả CV được hoàn thiện và được nhắc nhở là chung chung và thiếu tính cá nhân, chỉ cho thấy ứng viên dùng какие công cụ cụ thể.

rss · Simon Willison · 24/6 18:13

**Bối cảnh**: Các mô hình ngôn ngữ lớn (LLM) là mạng neural được huấn luyện trên bộ dữ liệu văn bản khổng lồ để tạo ra ngôn ngữ giống con người, cho phép thực hiện các nhiệm vụ như viết bài, tóm tắt bài viết và tạo mã. Các công cụ và nghiên cứu gần đây cho thấy LLM có thể tự động tạo ra thông điệp commit Git theo định dạng chuẩn từ một diff trong vài giây, làm cho việc lưu trữ các đóng góp do AI tạo ra trở nên dễ dàng. Trong thị trường lao động, người xin việc ngày càng sử dụng LLM để viết CV, xây dựng trang portfolio và điền lịch sử GitHub, dẫn đến các tài liệu xin việc chỉ phản ánh đầu ra của mô hình thay vì kinh nghiệm thực tế của cá nhân.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/large-language-model-llm/">Large Language Model (LLM) - GeeksforGeeks</a></li>
<li><a href="https://arxiv.org/abs/2507.10906">[2507.10906] Evaluating Generated Commit Messages with Large ... GitHub - Pengyu03/LLM-Commit-Message-Generation: This ... Using Large Language Models for Commit Message Generation: A ... How to Generate Git Commit Messages with a Local LLM Auto-generate Commit Messages with LLMs in Your Terminal Step-by-Step Guide - Guidance Docs</a></li>

</ul>
</details>

**Thẻ**: `#careers`, `#ai`, `#hiring`, `#llm`, `#job-market`

---

<a id="item-8"></a>
## [Gemma4-26B-A4B & 31B-QAT Không Lọc Cân Bằng đã ra mắt ra (tăng tốc  mắt với MTP (tăng tốc 35% & 53%)!](https://www.reddit.com/r/LocalLLaMA/comments/1ueuki7/gemma426ba4b_31bqat_uncensored_balanced_are_out/) ⭐️ 6.0/10

Phát hành các mô hình Gemma 4-26B-A4B-QAT và Gemma 4-31B-QAT không lọc, cân bằng, đi kèm MTP mang lại tăng tốc 35% và 53%.

reddit · r/LocalLLaMA · /u/hauhau901 · 25/6 00:13

**Thẻ**: `#Gemma`, `#QAT`, `#uncensored`, `#LLM`, `#MTP`

---