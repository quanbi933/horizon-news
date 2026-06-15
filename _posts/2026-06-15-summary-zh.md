---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> Đã chọn 9 tin quan trọng từ 13 nội dung.

---

1. [Tại sao AI chưa thay thế kỹ sư phần mềm, và sẽ không](#item-1) ⭐️ 8.0/10
2. [Hỗ trợ EAGLE đã được hợp nhất vào llama.cpp](#item-2) ⭐️ 8.0/10
3. [Kobo coi EPUB hợp lệ là lỗi do Adobe RMSDK.](#item-3) ⭐️ 7.0/10
4. [LLM Rio-3.5-Open-397B được 주장 là 'nhà sản xuất' nhưng thực ra là trộn trọng số](#item-4) ⭐️ 7.0/10
5. [Giới thiệu Heretic Grimoire: Hệ thống sao lưu ưu tiên local, chống chịu việc gỡ bỏ, giữ cho các mô hình không được kiểm duyệt luôn có sẵn vĩnh viễn](#item-5) ⭐️ 7.0/10
6. [Công cụ CLI Agent-Reach cho phép AI agent truy cập web miễn phí](#item-6) ⭐️ 7.0/10
7. [Thư viện Python Headroom nén đầu vào LLM để giảm token 60-95%](#item-7) ⭐️ 7.0/10
8. [Show HN: Kage – Đóng gói trang web thành file nhị phân xem offline](#item-8) ⭐️ 6.0/10
9. [Các file GGUF mới cho Command A Plus hỗ trợ suy luận local qua llama.cpp](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Tại sao AI chưa thay thế kỹ sư phần mềm, và sẽ không](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan và Sayash Kapoor đã công bố một bài luận 主張 rằng AI chưa gây ra việc sa thải hàng loạt trong ngành phần mềm, dựa trên dữ liệu WARN Act của New York cho thấy không có bất kỳ khai báo sa thải liên quan đến AI nào trong năm đầu tiên. Kết quả này thách thức những nỗi sợ szer rằng AI sẽ sớm thay thế công việc phần mềm và cho thấy các nghề nghiệp có ít nhiệm vụ thích hợp để tự động hóa hơn có thể còn bền bỉ hơn. New York đã thêm ô kiểm tra AI vào hồ sơ WARN Act vào tháng 3/2025; hơn 160 công ty đã nộp bản thông báo và không có ai đánh dấu ô đó. Bài luận xác định ba nút thắt chính — quyết định what to build, xác thực giao hàng, và sự hiểu biết sâu sắc về mã nguồn, kinh doanh và môi trường — làm hạn chế tác động của AI.

rss · Simon Willison · 14/6 23:54

**Bối cảnh**: Luật WARN Act là luật lao động Mỹ yêu cầu các nhà cung cấp công việc phải thông báo trước 60 ngày về các cuộc sa thải hàng loạt hoặc đóng cửa nhà máy. New York đã sửa đổi luật này vào tháng 3/2025 để thêm một ô kiểm tra cho phép nhà công việc الإفصاح về việc sa thải có liên quan đến AI, nhằm theo dõi mất việc do tự động hóa gây ra. Ngành phần mềm không chỉ bao gồm việc viết mã mà còn bao gồm các hoạt động như thu thập yêu cầu, gỡ lỗi và hiểu bối cảnh kinh doanh, które vẫn phụ thuộc fortemente vào con người.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Worker_Adjustment_and_Retraining_Notification_Act_of_1988">Worker Adjustment and Retraining Notification Act of 1988 - Wikipedia</a></li>
<li><a href="https://www.dol.gov/agencies/eta/layoffs/warn">WARN Act Compliance Assistance - U.S. Department of Labor</a></li>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>

</ul>
</details>

**Thẻ**: `#AI impact`, `#software engineering`, `#labor market`, `#AI policy`, `#WARN Act`

---

<a id="item-2"></a>
## [Hỗ trợ EAGLE đã được hợp nhất vào llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1u5z4j0/eagle_support_merged_into_llamacpp/) ⭐️ 8.0/10

Kỹ thuật suy diễn speculative decoding EAGLE đã được hợp nhất vào kho mã llama.cpp, cho phép người dùng đạt được tốc độ suy diễn LLM nhanh hơn 2-6 lần trên thiết bị địa phương. Sự hợp nhất này được công bố qua bài đăng trên Reddit bởi /u/Diablo-D3 kèm liên kết tới commit. Việc tích hợp EAGLE vào llama.cpp cải thiện hiệu suất và chất lượng đầu ra khi triển khai LLM tại địa phương, mang lại lợi ích cho các công cụ dựa trên llama.cpp như Ollama và LM Studio. Điều này phản ánh xu hướng rộng hơn của ngành về các kỹ thuật suy diễn hiệu quả như speculative decoding. EAGLE hoạt động ở mức tính năng, ngoại suy từ trạng thái ẩn trước đầu ra của mô hình, hỗ trợ kích thước batch lớn hơn một, suy diễn không tham lam, và được tích hợp với gpt‑fast để tăng tốc thêm. Các thí nghiệm trên RTX 3090 với mô hình LLaMA2‑chat 7B ở độ chính xác int4 cho thấy tăng tốc 2‑6 lần trên MT‑bench mà không cần huấn luyện bổ sung.

reddit · r/LocalLLaMA · /u/Diablo-D3 · 14/6 22:45

**Bối cảnh**: llama.cpp là một thư viện mã nguồn mở C/C++ cho phép suy diễn LLM trên nhiều loại phần cứng khác nhau bằng cách sử dụng thư viện tensor GGML, và là nhân của nhiều công cụ suy diễn tại địa phương như Ollama và LM Studio. Suy diễn speculative decoding tăng tốc độ tạo token bằng cách dự đoán các token trước thời gian thực; EAGLE (Extrapolation Algorithm for Greater Language‑Model Efficiency) là một họ các phương pháp như vậy, hoạt động ở mức tính năng, sử dụng fusión đa lớp và kỹ thuật kiểm tra tại thời gian huấn luyện để đạt được mức tăng tốc 2‑6 lần đồng thời vẫn giữ phân phối đầu ra của mô hình.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://arxiv.org/abs/2503.01840">[2503.01840] EAGLE-3: Scaling up Inference Acceleration of ... GitHub - SafeAILab/EAGLE: Official Implementation of EAGLE-1 ... An Introduction to Speculative Decoding for Reducing Latency ... EAGLE (speculative decoding) - AI Wiki EAGLE-3 Speculative Decoding: 2-6x Faster LLM Inference Guide Amazon SageMaker AI introduces EAGLE based adaptive ... LLM Inference Optimization: 2026 Update | Wei’s Learning Notes</a></li>
<li><a href="https://github.com/SafeAILab/EAGLE">GitHub - SafeAILab/EAGLE: Official Implementation of EAGLE-1 ... An Introduction to Speculative Decoding for Reducing Latency ... EAGLE (speculative decoding) - AI Wiki EAGLE-3 Speculative Decoding: 2-6x Faster LLM Inference Guide Amazon SageMaker AI introduces EAGLE based adaptive ... LLM Inference Optimization: 2026 Update | Wei’s Learning Notes</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++</a></li>

</ul>
</details>

**Thẻ**: `#llama.cpp`, `#EAGLE`, `#LLM inference`, `#open-source`, `#quantization`

---

<a id="item-3"></a>
## [Kobo coi EPUB hợp lệ là lỗi do Adobe RMSDK.](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/) ⭐️ 7.0/10

Bài viết giải thích rằng Kobo đánh dấu một số file EPUB là không hợp lệ mặc dù chúng vượt qua EPUBCheck, và cho rằng nguyên nhân là do Adobe RMSDK. Bài viết khuyên sử dụng công cụ kepubify để chuyển EPUB sang định dạng KEPUB thân thiện với Kobo. Điều này cho thấy sự mảnh vỡ trong hệ sinh thái ebook khi các moteurs rendering độc quyền khiến các file tuân thủ chuẩn bị bị từ chối, ảnh hưởng đến nhà xuất bản, nhà phát triển và người dùng Kobo dựa vào việc trao đổi file suôn sẻ. Việc hiểu cách giải quyết giúp tránh công việc lặp lại và nâng cao khả năng tương thích giữa các nền tảng. Vấn đề xuất phát từ Adobe RMSDK, mà Kobo sử dụng để xác thực và hiển thị EPUB, và có thể được vượt qua bằng cách đặt tên file có phần mở rộng .kepub.epub hoặc chuyển đổi bằng kepubify—công cụ nhanh, độc lập, xử lý HTML lỗi và bảo toàn bố cục đồng thời thêm các tính năng nâng cao dành cho Kobo.

hackernews · sohkamyung · 14/6 22:54 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48533848)

**Bối cảnh**: EPUB là tiêu chuẩn mở cho sách điện tử được xác thực bởi EPUBCheck để đảm bảo tuân thủ المواصفات. Bộ phát triển phần mềm Reader Mobile (RMSDK) của Adobe là một thư viện độc quyền được sử dụng bởi nhiều nền tảng đọc sách điện tử, bao gồm Kobo, để hiển thị EPUB và áp dụng DRM. Kobo mở rộng chuẩn bằng định dạng KEPUB riêng của mình, cung cấp các tính năng bổ sung như hiệu ứng lật trang tốt hơn và truy cập vào trình xem hình ảnh nội bộ khi file sử dụng hậu tố .kepub.epub. Các công cụ như kepubify tự động hoá quá trình chuyển đổi sang định dạng này, giúp khắc phục sự chênh lệch tương thích do xác thực nghiêm ngặt của RMSDK gây ra.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://pgaskin.net/kepubify/">Kepubify - pgaskin.net</a></li>
<li><a href="https://medium.com/@jiminypan/five-interesting-facts-about-adobe-legacy-ebook-rmsdk-b7be0123c874">Five interesting facts about Adobe legacy eBook RMSDK - Medium</a></li>
<li><a href="https://medium.com/@inesferreira789/kobo-kepub-format-why-and-how-9b5c1b39798">Kobo Kepub format : Why and How. Well, Kobo has been... | Medium</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những người bình luận chỉ ra phần mềm Adobe lịch sử không đáng tin cậy và khó tiếp cận RMSDK, khen ngợi kepubify vì tạo ra file thân thiện với Kobo, và thảo luận về cách tính chất living‑standard của các specs EPUB dựa trên web dẫn đến sự nhầm lẫn về phiên bản. Một số người cũng đề cập đến thiết bị thay thế như PineNote để tránh những vấn đề trong hệ sinh thái này.

**Thẻ**: `#epub`, `#ebook`, `#adobe`, `#kobo`, `#digital publishing`

---

<a id="item-4"></a>
## [LLM Rio-3.5-Open-397B được 주장 là 'nhà sản xuất' nhưng thực ra là trộn trọng số](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 7.0/10

Phân tích cho thấy Rio-3.5-Open-397B, được trình bày là mô hình tinh chỉnh tự phát của Qwen3.5-397B, thực chất là sự trộn trọng số khoảng 60% Nex-N2 Pro và 40% Qwen3.5-397B dựa trên độ tương đồng trọng số theo lớp. Kết luận này xuất phát từ một issue trên GitHub nơi thành viên cộng đồng kiểm tra các tensor trọng số trên 60 lớp. Điều này gây ra lo ngại về việc ghi công và trong suốt trong cộng đồng AI mã nguồn mở, khi việc tuyên bố một mô hình là 'nhà sản xuất' nhưng thực sự là sự trộn của các tác phẩm hiện có có thể gây hiểu lầm và vi phạm giấy phép. Đồng thời, điều này cũng cho thấy việc lấy trung bình trọng số đơn giản có thể nâng cao hiệu suất, kích thích thảo luận về các thực tiễn hợp nhất mô hình. Đặt ra dựa trên việc quan sát thấy mỗi tensor trọng số trong Rio-3.5-Open-397B khớp với một nội suy tuyến tính 0.6/0.4 của tensor tương ứng trong Nex-N2 Pro và Qwen3.5-397B trên tất cả 60 lớp, với độ lệch hàng nghìn độ lệch chuẩn. Không phát hiện bất kỳ tinh chỉnh bổ sung hoặc 蒸馏 nào trong các trọng số đã phát hành.

hackernews · unrvl22 · 14/6 15:37 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48528371)

**Bối cảnh**: Việc hợp nhất mô hình kết hợp các điểm kiểm tra đã được tinh chỉnh của các mô hình ngôn ngữ lớn bằng các kỹ thuật như lấy trung bình trọng số để tạo ra một mô hình mới kế thừa khả năng từ các mô hình cha. Nex-N2 Pro là một mô hình hỗn hợp chuyên gia 397B tham số do Nex AGI phát hành, được xây dựng trên Qwen3.5-397B-A17B. Qwen3.5-397B là mô hình ngôn ngữ lớn flagship của 系列 Qwen của Alibaba, thường được sử dụng làm cơ sở để tinh chỉnh thêm.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/large-language-model-merging">Large Language Model Merging</a></li>
<li><a href="https://huggingface.co/nex-agi/Nex-N2-Pro">nex-agi/Nex-N2-Pro - Hugging Face</a></li>
<li><a href="https://pi.dev/models/together/qwen-qwen3-5-397b-a17b">Qwen 3 . 5 397 B A17 B · Models · Pi</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các thành viên cộng đồng biểu hiện sự ngạc nhiên khi một sự kết hợp tuyến tính đơn giản của trọng số có thể nâng cao hiệu suất, đặt câu hỏi về việc có có bất kỳ quá trình 蒸馏 nào được tham gia, và tranh luận về đạo đức khi tuyên bố một mô hình hợp nhất là 'nhà sản xuất' mà không ghi công thích đáng. Một số người dùng cũng hỏi giải thích về cách hoạt động của việc hợp nhất mô hình, cho thấy nhu cầu về hướng dẫn kỹ thuật rõ ràng hơn.

**Thẻ**: `#LLM`, `#model merging`, `#AI transparency`, `#open-source models`, `#model evaluation`

---

<a id="item-5"></a>
## [Giới thiệu Heretic Grimoire: Hệ thống sao lưu ưu tiên local, chống chịu việc gỡ bỏ, giữ cho các mô hình không được kiểm duyệt luôn có sẵn vĩnh viễn](https://www.reddit.com/r/LocalLLaMA/comments/1u5lmge/introducing_the_heretic_grimoire_the/) ⭐️ 7.0/10

Heretic Grimoire là một hệ thống sao lưu ưu tiên local được thiết kế để giữ cho các mô hình ngôn ngữ không được kiểm duyệt luôn có sẵn vô thời hạn, dù có các nỗ lực gỡ bỏ.

reddit · r/LocalLLaMA · /u/-p-e-w- · 14/6 13:47

**Thẻ**: `#Heretic`, `#local LLM`, `#backup system`, `#uncensored models`, `#takedown-resilient`

---

<a id="item-6"></a>
## [Công cụ CLI Agent-Reach cho phép AI agent truy cập web miễn phí](https://github.com/Panniantong/Agent-Reach) ⭐️ 7.0/10

Kho lưu trữ GitHub Panniantong/Agent-Reach đã nhận được 102 sao trong 24 giờ, ra mắt một công cụ CLI Python cho phép AI agent duyệt và tìm kiếm trên Twitter, Reddit, YouTube, GitHub, Bilibili và XiaoHongShu mà không cần trả phí API. Việc loại bỏ chi phí API của Agent-Reach giảm thiểu rào cản cho nhà phát triển khi trang bị AI agent bằng dữ liệu web thời gian thực, từ đó tăng tốc quá trình thử nghiệm và triển khai các agent tự chủ trên nhiều nền tảng. Công cụ được viết bằng Python, hoạt động dưới dạng giao diện dòng lệnh, và có thể sử dụng Selenium kèm ChromeDriver không được phát hiện để thu thập dữ liệu từ các trang web mà tránh bị chặn.

ossinsight · Panniantong · 15/6 04:49

**Bối cảnh**: Các AI agent thường cần thông tin mới nhất từ các website để thực hiện nhiệm vụ, nhưng việc truy cập dữ liệu qua API chính thức có thể tốn kém hoặc bị giới hạn tốc độ. Việc thu thập dữ liệu web cho phép các chương trình trích xuất dữ liệu công khai trực tiếp từ trang web, sử dụng các kỹ thuật như phân tích HTML, xoay tiêu đề và sử dụng trình duyệt không giao diện. Để tránh bị chặn bởi các biện pháp chống bot, các nhà phát triển thường sử dụng công cụ như ChromeDriver không được phát hiện, điều chỉnh trình duyệt được điều khiển bởi Selenium để mô phỏng hành vi người dùng thực. Agent-Reach kết hợp các phương pháp này vào một công cụ CLI duy nhất, cho phép agent thu thập dữ liệu từ nhiều nền tảng mạng xã hội và nội dung mà không cần khóa API.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.zenrows.com/blog/undetected-chromedriver">Undetected ChromeDriver in Python Selenium: How to... - ZenRows</a></li>
<li><a href="https://www.capsolver.com/blog/web+scraping/web-scraping-anti-detection-techniques">Web Scraping Anti-Detection Techniques : Stable Data Extraction</a></li>
<li><a href="https://multilogin.com/blog/web-scraping-techniques/">Top Web Scraping Techniques for Effective Data Collection</a></li>

</ul>
</details>

**Thẻ**: `#AI agents`, `#web scraping`, `#CLI`, `#open-source`, `#automation`

---

<a id="item-7"></a>
## [Thư viện Python Headroom nén đầu vào LLM để giảm token 60-95%](https://github.com/chopratejas/headroom) ⭐️ 7.0/10

Kho lưu trữ GitHub chopratejas/headroom đã tăng 89 sao trong 24 giờ qua, ra mắt một thư viện và proxy Python nén đầu ra công cụ, nhật ký, tệp và các đoạn RAG trước khi đến LLM, giảm sử dụng token 60‑95% mà vẫn giữ chất lượng câu trả lời. Việc giảm số token gửi tới LLM giúp Headroom giảm chi phí API và độ trễ cho các tác nhân AI, đường ống RAG và công cụ phát triển, làm cho các ứng dụng mô hình lớn trở nên khả thi và mở rộng hơn. Headroom là một gói Python thuần túy có thể chạy như một proxy địa phương hoặc máy chủ MCP, không cần thay đổi mã; nó chặn các yêu cầu tương thích OpenAI và áp dụng nén cho nhật ký, đầu ra công cụ, các đoạn RAG và tệp, đạt được tới 80% tiết kiệm token trong các bài kiểm tra.

ossinsight · chopratejas · 15/6 04:49

**Bối cảnh**: Các mô hình ngôn ngữ lớn xử lý đầu vào dưới dạng token, và các bối cảnh dài nhanh chóng vượt quá giới hạn token, tăng chi phí và làm chậm phản hồi. Các hệ thống tăng cường truy xuất (RAG) thường cung cấp nhiều đoạn đã truy xuất cho mô hình, trong đó nhiều đoạn chứa thông tin không liên quan. Headroom giải quyết vấn đề này bằng cách nén các đoạn và các đầu ra công cụ khác trước khi chúng đến LLM, giữ lại chỉ thông tin cần thiết để trả lời chính xác.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/chopratejas/headroom">GitHub - chopratejas/headroom: Compress tool outputs, logs ...</a></li>
<li><a href="https://headroomlabs.ai/">Headroom - Context Optimization for LLM Tooling & Agents</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#LLM optimization`, `#token compression`, `#Python library`, `#AI infrastructure`, `#prompt engineering`

---

<a id="item-8"></a>
## [Show HN: Kage – Đóng gói trang web thành file nhị phân xem offline](https://github.com/tamnd/kage) ⭐️ 6.0/10

Kage thu thập một trang web, loại bỏ JavaScript và gói gói các tài nguyên tĩnh thành một file thực thi nhị phân duy nhất có thể cung cấp trang web địa phương để xem offline. Công cụ này cung cấp một cách đơn giản và di động để lưu trữ và chia sẻ trang web mà không cần máy chủ web, hữu ích cho tài liệu, đọc offline hoặc môi trường có kết nối hạn chế. Công cụ sử dụng Chrome headless để chụp ảnh mỗi trang, loại bỏ toàn bộ JavaScript, nhúng CSS và hình ảnh, sau đó gắn bộ lưu trữ vào một bản sao của nhị phân kage qua cờ --format binary để tạo ra một file thực thi tự cung cấp.

hackernews · tamnd · 14/6 17:25 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48529990)

**Bối cảnh**: Các công cụ lưu trữ website thường tải xuống HTML, CSS, hình ảnh và JavaScript để cho phép duyệt offline, nhưng nhiều công cụ cần một máy chủ địa phương để cung cấp các tệp. Kage khác bằng cách loại bỏ JavaScript và gói gói bộ ảnh tĩnh thành một file thực thi duy nhất có thể tự hoạt động như một máy chủ web. Nó dựa trên Chrome headless để render trang và chụp DOM như người dùng thấy, sau đó loại bỏ các script trước khi đóng gói.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing , with...</a></li>
<li><a href="https://www.httrack.com/">HTTrack Website Copier - Free Software Offline Browser (GNU GPL)</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Một số bình luận viên chỉ ra rằng GIF demo được tạo bằng công cụ ascii‑gif của tác giả và khen Kage cho phép truy cập offline các trang như wiki công ty. Một số người khác đặt câu hỏi về nhu cầu máy chủ địa phương khi đầu ra là tĩnh, so sánh Kage với SingleFile và HTTrack, và đề xuất cải tiến như điểm vào HTML tự chứa. Trong tổng thể, cuộc thảo luận thấy Kage là một công cụ tăng tiến hữu ích nhưng còn tranh luận về các lựa chọn thay thế và các cải thiện có thể.

**Thẻ**: `#offline viewing`, `#website archiving`, `#single binary`, `#web utility`, `#Show HN`

---

<a id="item-9"></a>
## [Các file GGUF mới cho Command A Plus hỗ trợ suy luận local qua llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1u64t9i/command_a_plus_ggufs_posted/) ⭐️ 6.0/10

Người dùng /u/coder543 đã chia sẻ các file GGUF mới được chuyển đổi và lượng tử hoá cho Command A Plus, làm cho model có thể chạy local qua llama.cpp. Điều này cung cấp các phiên bản GGUF lượng tử hoá mới nhất cho mô hình MoE mạnh mẽ 25B tham số hoạt động, cho phép cộng đồng LLM local chạy Command A Plus hiệu quả trên phần cứng tiêu dùng. Các file GGUF được tạo từ mô hình Command A Plus của Cohere, sử dụng công cụ chuyển đổi của llama.cpp và bao gồm các mức lượng tử hoá khác nhau (ví dụ Q4_K_M, Q5_K_S).

reddit · r/LocalLLaMA · /u/coder543 · 15/6 03:11

**Bối cảnh**: GGUF (GGML Universal File) là định dạng file nhị phân lưu trữ tensor và metadata của mô hình để tải và chạy LLM hiệu quả trên phần cứng tiêu dùng. Command A Plus là mô hình MoE nguồn mở của Cohere có 25B tham số hoạt động và 218B tổng tham số, hỗ trợ tác vụ đa phương thức, suy luận và đa ngôn ngữ với bối cảnh 190k token. Lượng tử hoá mô hình giảm độ chính xác của trọng số sang biểu diễn bit thấp hơn, giảm nhu cầu về bộ nhớ và tính toán mà vẫn giữ hiệu suất, cho phép chạy các mô hình lớn trên tài nguyên hạn chế.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>
<li><a href="https://docs.cohere.com/docs/command-a-plus">Cohere's Command A Plus Model | Cohere</a></li>
<li><a href="https://www.datacamp.com/tutorial/quantization-for-large-language-models">Quantization for Large Language Models (LLMs): Reduce AI Model Sizes Efficiently | DataCamp</a></li>

</ul>
</details>

**Thẻ**: `#llama.cpp`, `#GGUF`, `#Command A Plus`, `#local LLM`, `#model quantization`

---