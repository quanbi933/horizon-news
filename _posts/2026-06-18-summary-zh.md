---
layout: default
title: "Horizon Summary: 2026-06-18 (ZH)"
date: 2026-06-18
lang: zh
---

> Đã chọn 7 tin quan trọng từ 12 nội dung.

---

1. [GLM-5.2 là mô hình LLM chỉ văn bản mạnh nhất có trọng số mở](#item-1) ⭐️ 9.0/10
2. [Lore: Hệ thống VCS mã nguồn mở cho trò chơi](#item-2) ⭐️ 8.0/10
3. [Midjourney ra mắt khái niệm quét toàn thân y tế giá thấp AI](#item-3) ⭐️ 7.0/10
4. [Charity Majors: AI làm mã nguồn rẻ và ngay lập tức](#item-4) ⭐️ 7.0/10
5. [Gemma 4 E2B chạy trong trình duyệt qua WebGPU đạt 255 token/giây](#item-5) ⭐️ 7.0/10
6. [Inflect-Nano: Mô hình TTS siêu nhỏ 4,63 triệu tham số được phát hành](#item-6) ⭐️ 6.0/10
7. [Tài liệu rò rỉ tiết lộ OpenAI mất hàng tỷ đô la mỗi năm](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GLM-5.2 là mô hình LLM chỉ văn bản mạnh nhất có trọng số mở](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai đã phát hành GLM-5.2 cho người dùng gói lập trình vào ngày 13/6/2026, và sau đó công bố toàn bộ trọng số mở dưới giấy phép MIT vào ngày 16/6/2026. Mô hình này là LLM MoE có 753 tỷ tham số và cửa sổ ngữ cảnh 1 triệu token. GLM-5.2 đứng đầu chỉ số trí tuệ nhân tạo Artificial Analysis v4.1 với điểm 51, vượt qua các mô hình mở khác như MiniMax-M3 và DeepSeek V4 Pro. Hiệu suất tốt trên bảng xếp hạng Code Arena WebDev cho thấy một mô hình chỉ văn bản, trọng số mở có thể cạnh tranh với các hệ thống proprietari hàng đầu trong các tác vụ mã hóa thực tế. Mô hình có 753 tỷ tham số tổng nhưng chỉ 40 tham số hoạt động tại bất kỳ thời điểm nào (Mixture of Experts), dung lượng khoảng 1,51 TB, chỉ chấp nhận đầu vào văn bản và có cửa sổ ngữ cảnh 1 triệu token. Nó tiêu thụ khoảng 43k token đầu ra cho mỗi nhiệm vụ chỉ số trí tuệ, xếp hạng thứ hai trên bảng xếp hạng Code Arena WebDev, và được cung cấp qua OpenRouter với giá khoảng 1,40 USD/gettriệu token đầu vào và 4,40 USD/gettriệu token đầu ra.

rss · Simon Willison · 17/6 23:58

**Bối cảnh**: Kiến trúc Mixture‑of‑Experts cho phép mô hình chứa nhiều tham số nhưng chỉ kích hoạt một phần nhỏ (“expert”) cho mỗi token, từ đó giảm đáng kể lượng tính toán cần thiết cho huấn luyện và suy luận. Cửa sổ ngữ cảnh 1 triệu token cho phép mô hình xem xét các chuỗi rất dài—như một cuốn sách hoặc toàn bộ mã nguồn—lúc này, điều này là thiết yếu cho các nhiệm vụ đòi hỏi sự hiểu biết sâu xa về các mối quan hệ dài hạn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.ibm.com/think/topics/context-window">What is a context window ? | IBM</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#open-weights`, `#Mixture-of-Experts`, `#large-language-model`, `#AI-research`

---

<a id="item-2"></a>
## [Lore: Hệ thống VCS mã nguồn mở cho trò chơi](https://lore.org/) ⭐️ 8.0/10

Epic Games đã phát hành Lore, một hệ thống quản lý phiên bản mã nguồn mở được thiết kế để xử lý mở rộng các tài sản nhị phân lớn trong phát triển trò chơi, định vị nó như một lựa chọn thay thế cho Perforce. Lore giải quyết vấn đề hiệu suất kém của Git với các tệp nhị phân lớn, cung cấp cho cácstudio trò chơi một hệ thống VCS mã nguồn mở có thể mở rộng, giúp giảm sự phụ thuộc vào các hệ thống độc quyền đắt đỏ như Perforce. Lore bao gồm một subsystem lưu trữ dựa trên phân vùng và địa chỉ theo nội dung để loại bỏ trùng lặp tài sản và một subsystem quản lý phiên bản xây dựng các bản sửa đổi, nhánh, hợp nhất và staging từ các nguyên tắc lưu trữ; nó được thiết kế để đạt khả năng mở rộng chưa từng có cho cả dữ liệu và đội ngũ.

hackernews · regnerba · 17/6 14:30 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48571081)

**Bối cảnh**: Các hệ thống quản lý phiên bản như Git rất hiệu quả trong việc theo dõi thay đổi của mã nguồn dựa trên văn bản nhưng gặp khó khăn với các tệp nhị phân lớn như texture, mô hình 3D và âm thanh, które thường xuất hiện trong phát triển trò chơi. Perforce Helix Core đã trở thành tiêu chuẩn ngành cho các studio trò chơi nhờ khả năng hỗ trợ tài sản lớn, khóa tệp và quyền 限 chế mạnh mẽ, mặc dù đây là phần mềm độc quyền và có thể phức tạp để quản lý. Lore nhằm kết hợp tính mở nguồn của Git với khả năng mở rộng và xử lý tài sản của Perforce, nhắm vào nhu cầu cụ thể của các đội phát triển trò chơi hiện đại.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">GitHub - EpicGames/lore: Lore is a next-generation, open source revision control system · GitHub</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System - Phoronix</a></li>
<li><a href="https://www.perforce.com/blog/vcs/version-control-for-binary-files">Version Control for Binary Files: Manage Large Files Easily | Perforce Software</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận cho rằng mặc dù Git hoạt động tốt với mã nguồn, nhưng nó không hiệu quả đối với các tài sản nhị phân lớn như texture và mô hình, khiến các studio trò chơi vẫn phải dựa vào Perforce mặc dù nó phức tạp. Một số người dùng nhấn mạnh nhu cầu về khóa tệp độc quyền và khả năng mở rộng tốt hơn, biểu thị lạc quan rằng Lore có thể trở thành lựa chọn thay thế mã nguồn mở nhẹ hơn. Một số người đặc biệt nêu tiềm năng lợi ích cho quy trình làm việc của Unreal Engine, tuy nhiên cũng có người cảnh báo rằng việc przyję sẽ phụ thuộc vào sự成熟 của công cụ và tích hợp.

**Thẻ**: `#version-control`, `#game-development`, `#open-source`, `#scalability`, `#Perforce-alternative`

---

<a id="item-3"></a>
## [Midjourney ra mắt khái niệm quét toàn thân y tế giá thấp AI](https://www.midjourney.com/medical/blogpost) ⭐️ 7.0/10

Midjourney đã phát hành một video và bài đăng trên blog đề xuất một phương pháp y tế hình ảnh sinh tạo bởi AI, giá thấp và thấp bức xạ, gọi là Ultrasonic CT, để quét toàn thân nhanh chóng. Nếu thực hiện được, công nghệ này có thể làm cho việc quét toàn thân trở nên giá cả phải chăng và an toàn đủ để sử dụng thường xuyên, từ đó giúp phát hiện bệnh sớm và giảm lượng bức xạ gây hại cho bệnh nhân. Hệ thống Ultrasonic CT được đề xuất sử dụng một bể nước nhẹ màu vàng và xử lý AI để tạo hình ảnh trong khoảng 60 giây, tuy nhiên bản trình diễn hiện tại vẫn là giả thuyết và chưa được xác thực so sánh với MRI hoặc CT.

hackernews · ricochet11 · 18/6 01:59 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48579650)

**Bối cảnh**: Trí tuệ nhân tạo đang được ứng dụng ngày càng nhiều trong y tế hình ảnh để giảm nhiễu và cải thiện chất lượng hình ảnh từ các chụp liều lượng thấp, như siêu thấp liều PET hoặc CT. Các nghiên cứu cho thấy các thuật toán AI có thể tái tạo hình ảnh toàn thân chất lượng chuẩn đoán từ lượng bức xạ nhập vào rất ít, từ đó cho phép skrining an toàn và thường xuyên hơn. Các phương pháp quét toàn thân hiện tại bao gồm MRI, CT và PET, mỗi phương pháp có những trade‑off khác nhau về độ phân giải, chi phí và mức độ phơi nhiễm bức xạ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8266729/">Artificial Intelligence enables whole body Positron Emission ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11941271/">AI-Driven Advances in Low-Dose Imaging and Enhancement—A Review</a></li>
<li><a href="https://www.midjourney.com/medical">Midjourney Medical</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận chào đón ý tưởng về quét toàn thân giá rẻ và thường xuyên, cho rằng việc thu thập dữ liệu chi phí thấp có thể mở ra nhiều khả năng chẩn đoán. Nhiều người khác cảnh báo rằng đây là một ý tưởng còn speculative, thiếu dữ liệu cụ thể để hỗ trợ các 主張 về độ chính xác và an toàn, đồng thời nguy cơ過度 phát hiện và kết quả dương tính giả. Một số chuyên gia y tế bày tỏ sự quan tâm muốn biết thêm nhưng nghi ngờ phương pháp này có thể thay thế MRI trong thời gian gần được.

**Thẻ**: `#medical imaging`, `#AI`, `#healthcare`, `#Midjourney`, `#diagnostic technology`

---

<a id="item-4"></a>
## [Charity Majors: AI làm mã nguồn rẻ và ngay lập tức](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 7.0/10

Charity Majors nhận thấy rằng vào năm 2025, AI đã làm cho việc tạo mã nguồn trở nên miễn phí và tức thời, biến các dòng mã từ tài sản có giá trị, có thể tái sử dụng thành hàng hóa tiêu thụ và có thể tái tạo. Thay đổi này cho thấy AI đang định hình lại kinh tế phần mềm, buộc các kỹ sư phải suy nghĩ lại về quyền sở hữu mã, bảo trì và giá trị của việc viết mã tay trong thời đại mã nguồn được sinh ra bởi AI phong phú. Bình luận của Majors được lấy từ bài viết trên Substack có tiêu đề 'AI đòi hỏi nhiều kỷ律 kỹ thuật hơn. Không ít hơn', nhấn mạnh rằng mặc dù việc tạo mã nguồn trở nên rẻ, nhu cầu về kỷ律 kỹ thuật thực sự tăng lên.

rss · Simon Willison · 17/6 17:12

**Bối cảnh**: Lập trình hỗ trợ AI sử dụng các công cụ như GitHub Copilot và các mô hình ngôn ngữ lớn để tạo mã từ lời nhắc ngôn ngữ tự nhiên, làm tăng tốc độ phát triển. Các mô hình AI sinh tạo học hỏi các mẫu từ tập dữ liệu lớn để tạo ra các đoạn mã mới, giảm chi phí và thời gian cần thiết để viết phần mềm. Những công nghệ này đã chuyển đổi mã nguồn từ một tài sản được chăm sóc kỹ lưỡng thành một đầu ra có thể tái tạo ngay lập tức.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.coursera.org/learn/ai-assisted-programming">AI-Assisted Programming - Coursera</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_AI">Generative AI</a></li>

</ul>
</details>

**Thẻ**: `#charity-majors`, `#ai-assisted-programming`, `#generative-ai`, `#ai`, `#software-engineering`

---

<a id="item-5"></a>
## [Gemma 4 E2B chạy trong trình duyệt qua WebGPU đạt 255 token/giây](https://www.reddit.com/r/LocalLLaMA/comments/1u8g3d0/gemma_4_e2b_running_inbrowser_at_255_toks_using/) ⭐️ 7.0/10

Mô hình Gemma 4 E2B (2 tỷ tham số, QAT Mobile) đã được chứng minh chạy hoàn toàn trong trình duyệt web bằng các nhân WebGPU được tối ưu bởi Fable 5, đạt khoảng 255 token/giây trên chip M4 Max. Demo và mã nguồn nhân hiện đã được công khai trên Hugging Face Spaces. Điều này cho thấy các mô hình LLM đã được lượng tử hoá hiện đại có thể đạt tốc độ suy luận gần như nguyên bản trên phần cứng tiêu dùng chỉ bằng các tiêu chuẩn web, mở ra khả năng cho các ứng dụng AI bảo mật, không cần cài đặt. Đồng thời, nó nhấn mạnh vai trò ngày càng tăng của WebGPU như một bộ tăng tốc di động cho việc triển khai LLM ở biên. Các nhân được viết và tối ưu bởi Fable 5 trước khi ngừng hoạt động, sử dụng các shader tính toán WebGPU để triển khai các lớp transformer của Gemma 4 E2B. Mô hình sử dụng định dạng Quantization‑Aware Training (QAT) Mobile, giúp giảm bộ nhớ cần thiết mà vẫn giữ độ chính xác.

reddit · r/LocalLLaMA · /u/xenovatech · 17/6 17:06

**Bối cảnh**: Gemma 4 là gia đình mô hình ngôn ngữ mở trọng lượng mới nhất của Google, trong đó biến thể E2B có 2 tỷ tham số hiệu quả và phiên bản QAT dành cho thiết bị di động giúp giảm mức sử dụng bộ nhớ. WebGPU là tiêu chuẩn web hiện đại cho phép truy cập khả năng tính toán GPU từ trình duyệt, hỗ trợ các tác vụ đồ họa và tính toán hiệu quả mà không cần plugin. Các nghiên cứu gần đây như WebLLM cho thấy các nhân WebGPU được tối ưu có thể giữ lại tới 80 % hiệu suất gốc của GPU khi chạy suy luận LLM. Bản demo được phát hành dựa trên những tiến bộ này, cung cấp một triển khai hoàn toàn ở phía client của Gemma 4 E2B.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 4 model overview | Google AI for Developers</a></li>
<li><a href="https://arxiv.org/html/2412.15803v2">WebLLM: A High-Performance In-Browser LLM Inference Engine</a></li>
<li><a href="https://huggingface.co/spaces/webml-community/gemma-4-webgpu-kernels">Gemma 4 WebGPU Kernels - a Hugging Face Space by webml-community</a></li>

</ul>
</details>

**Thẻ**: `#Gemma`, `#WebGPU`, `#in-browser LLM`, `#model optimization`, `#AI inference`

---

<a id="item-6"></a>
## [Inflect-Nano: Mô hình TTS siêu nhỏ 4,63 triệu tham số được phát hành](https://www.reddit.com/r/LocalLLaMA/comments/1u8p9s1/i_released_inflectnano_an_ultraextreme_tiny_463m/) ⭐️ 6.0/10

Tác giả đã phát hành Inflect-Nano-v1, một mô hình TTS có 4,63 triệu tham số, bao gồm mô hình âm thanh 3,46 triệu và vocoder 1,17 triệu, có thể chạy trên phần cứng yếu. Mặc dù chất lượng còn hạn chế, Inflect‑Nano cho thấy việc tổng hợp lời nói có thể đạt được với dưới năm triệu tham số, mở ra khả năng cho các thiết bị biên, trợ lý ngoại tuyến và các tác nhân giọng dựa trên WASM. Mô hình xuất ra âm thanh 24 kHz, chỉ hỗ trợ tiếng Anh với một giọng nam đơn, và được phân phối trên Hugging Face kèm script suy luận PyTorch đơn giản.

reddit · r/LocalLLaMA · /u/b111ue · 17/6 22:50

**Bối cảnh**: Trong một hệ thống TTS thông thường, mô hình âm thanh trước tiên chuyển đổi văn bản thành các đặc trưng trung gian như mel‑spectrogram, sau đó vocoder biến đổi các đặc trưng này thành dạng sóng âm thanh có thể nghe được. Các kỹ thuật nén mô hình như cắt tỉa (pruning), lượng tử hóa (quantization) và phân giải thấp hạng (low‑rank decomposition) được sử dụng để giảm số lượng tham số mà vẫn giữ chức năng, cho phép triển khai trên thiết bị có tài nguyên hạn chế. Phát hành Inflect‑Nano cho thấy việc nén mạnh có thể tạo ra một mô hình TTS hoạt động được với chỉ vài triệu tham số.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://zilliz.com/ai-faq/what-is-the-function-of-a-vocoder-in-tts">What is the function of a vocoder in TTS ? - Zilliz Vector Database</a></li>
<li><a href="https://charansinghthakur9.medium.com/text-to-speech-tts-simplified-for-beginners-43218e5032d5">Text -to- Speech ( TTS ) simplified for beginners | by Charan... | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_compression">Model compression - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#TTS`, `#model compression`, `#edge AI`, `#speech synthesis`, `#open source`

---

<a id="item-7"></a>
## [Tài liệu rò rỉ tiết lộ OpenAI mất hàng tỷ đô la mỗi năm](https://www.reddit.com/r/LocalLLaMA/comments/1u8tcob/leaked_financial_docs_show_openai_is_losing/) ⭐️ 6.0/10

Các tài liệu tài chính bị rò rỉ cho thấy OpenAI đang mất hàng tỷ đô la mỗi năm, theo một bài đăng trên Reddit's r/LocalLLaMA. Việc rò rỉ này nhấn mạnh những lo ngại về tính bền vững của các mô hình AI lớn tốn kém và kích thích cuộc tranh luận về kinh tế học của AI so với các lựa chọn mã nguồn mở rẻ hơn. Các tài liệu prétendedly chi tiết các khoản thua lỗ hàng năm tính bằng tỷ, nhưng con số cụ thể và khung thời gian chưa được tiết lộ trong bản rò rỉ.

reddit · r/LocalLLaMA · /u/johnnyApplePRNG · 18/6 01:55

**Bối cảnh**: Các mô hình ngôn ngữ lớn (LLM) đòi hỏi tài nguyên tính toán enormes, với chi phí huấn luyện lên tới hàng trăm triệu đô la vì chúng có hàng tỷ tham số. Các phân tích gần đây cho thấy thị trường chia thành hai cấp: các API premium tính 费 $25–$30 cho mỗi triệu token đầu ra, trong khi các mô hình trọng lượng mở (open‑weight) có thể rẻ hơn 35 lần. Mặc dù có khả năng cao, nhiều công ty AI vẫn gặp khó khăn trong kiếm tiền từ các mô hình của họ, dẫn đến sự thua lỗ rộng rãi khi các mô hình giá không đủ chi phí huấn luyện và suy luận.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://maseconomics.com/economics-of-large-language-models-the-two-tier-ai-world/">Economics of Large Language Models: The Two‑Tier AI World - maseconomics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://capitalnexus.substack.com/p/ais-reality-check-why-95-of-companies">AI's Reality Check: Why 95% of Companies Are Losing Money on ...</a></li>

</ul>
</details>

**Thẻ**: `#AI`, `#OpenAI`, `#finance`, `#LLM`, `#industry analysis`

---