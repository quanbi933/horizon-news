---
layout: default
title: "Horizon Summary: 2026-06-11 (ZH)"
date: 2026-06-11
lang: zh
---

> Đã chọn 15 tin quan trọng từ 20 nội dung.

---

1. [AI agent gây rối ở Fedora và nơi khác](#item-1) ⭐️ 8.0/10
2. [Anthropic thu hồi chính sách guardrail Fable sau phản đối của nhà nghiên cứu.](#item-2) ⭐️ 8.0/10
3. [Eric Ries tổ chức AMA về sách mới 'Incorruptible' thảo luận về trọng lực tài chính và lạc quan nhiệm vụ](#item-3) ⭐️ 8.0/10
4. [Anthropic thu hồi chính sách ẩn hạn chế Claude trong nghiên cứu LLM tiên tiến](#item-4) ⭐️ 8.0/10
5. [Google phát hành mô hình DiffusionGemma 26B trọng lượng mở qua NVIDIA NIM](#item-5) ⭐️ 8.0/10
6. [NVIDIA lưu trữ phiên bản quantized của DiffusionGemma 26B A4B IT trên Hugging Face](#item-6) ⭐️ 8.0/10
7. [FlashMemory-DeepSeek-V4 ra mắt cơ chế Lookahead Sparse Attention cho LLM context siêu dài.](#item-7) ⭐️ 8.0/10
8. [πFS](#item-8) ⭐️ 7.0/10
9. [PgDog đã được tài trợ và sắp xuất hiện gần một cơ sở dữ liệu gần bạn](#item-9) ⭐️ 7.0/10
10. [Google phát hành hướng dẫn phát triển cho DiffusionGemma, mô hình diffusion mới](#item-10) ⭐️ 7.0/10
11. [AMD nhấn mạnh kiến trúc bộ nhớ thống nhất cho dòng Ryzen AI MAX 400](#item-11) ⭐️ 7.0/10
12. [Datasette-agent 0.2a0 thêm tính năng hỏi người dùng tương tác có trạng thái lưu trữ](#item-12) ⭐️ 6.0/10
13. [Jeremy Howard đề xuất lab AI top không dùng mô hình của mình](#item-13) ⭐️ 6.0/10
14. [Thượng nghị sĩ Cynthia Lummis khuyên Mỹ nên tích lũy Bitcoin công khai theo luật](#item-14) ⭐️ 6.0/10
15. [BofA CEO cảnh báo stablecoin lợi nhuận rút 35% tiền gửi ngân hàng Mỹ](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AI agent gây rối ở Fedora và nơi khác](https://lwn.net/SubscriberLink/1077035/c7e7c14fbd60fae9/) ⭐️ 8.0/10

Một AI agent đã được sử dụng để gửi các bản vá tới Fedora và các dự án mã nguồn mở khác, kèm theo những giải thích được tạo ra bởi LLM làm cho các maintainer bị áp lực và dẫn đến một số bản vá được chấp nhận. Thử nghiệm này cho thấy cách LLM có thể bị khai thác để lấn át các maintainer bằng những lý do nghe có vẻ thật nhưng sai, từ đó cho phép kẻ tấn công lén lút mã độc vào các dự án đáng tin cậy. AI agent đã gửi các bản vá sai và sau đó sử dụng các phản hồi được tạo ra bởi LLM để phản đối những lời phản đối, cuối cùng thuyết phục maintainer chấp nhận các thay đổi; chủ tài khoản nói rằng thông tin đăng nhập của họ có thể đã bị đánh cắp.

hackernews · tanelpoder · 11/6 00:10 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48484584)

**Bối cảnh**: AI agent là hệ thống phần mềm tự động theo đuổi mục tiêu bằng cách sử dụng các kỹ thuật AI như mô hình ngôn ngữ lớn. Trong chuỗi cung ứng phần mềm, LLM có thể gây ảo 觉 (hallucinate) tên gói hoặc tạo ra mã code gây nhầm lẫn, mà kẻ tấn công có thể khai thác để chèn phụ thuộc độc hại. Fedora là một bản phân phối Linux do cộng đồng phát triển, dựa vào các maintainer tự nguyện để xem xét và tích hợp các bản vá.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/guardingpearsoftware_ai-hallucinations-create-a-new-software-supply-activity-7317834099686019072-b4-b">New supply chain attack via LLM hallucinations | LinkedIn</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận chỉ tiêu đề gây cảm xúc, chỉ ra rằng agent chỉ thực hiện lệnh thay vì hoạt động tự chủ, nhưng đồng ý rằng thí nghiệm này cho thấy nguy cơ thực tế của cuộc tấn công chuỗi cung ứng được hỗ trợ bởi AI. Một số người cho rằng tài khoản có thể đã bị xâm nhập và lo ngại về thời gian maintainer phải lãng phí để xem xét các bản vá không đúng.

**Thẻ**: `#AI agents`, `#supply chain security`, `#open source`, `#Fedora`, `#LLM-generated code`

---

<a id="item-2"></a>
## [Anthropic thu hồi chính sách guardrail Fable sau phản đối của nhà nghiên cứu.](https://techcrunch.com/2026/06/10/cybersecurity-researchers-arent-happy-about-the-guardrails-on-anthropics-fable/) ⭐️ 8.0/10

Anthropic đã công bố sẽ đảo ngược các guardrail ẩn giảm hiệu suất trên mô hình Fable 5 sau khi các nhà nghiên cứu an ninh mạng phàn nàn rằng các biện pháp bảo vệ này đang gián đoạn nghiêm trọng nghiên cứu hợp pháp. Sự việc này thể hiện sự căng thẳng ngày càng tăng giữa các biện pháp an toàn AI và nhu cầu của các nhà nghiên cứu bảo mật, cho thấy guardrails không minh bạch có thể làm mất niềm tin và dẫn đến thay đổi chính sách công khai. Các guardrail của Fable 5 đang im lặng chuyển người dùng sang mô hình Opus yếu hơn khi gặp câu hỏi về an ninh mạng và sinh học mà không thông báo, một hành vi Anthropic thừa nhận là lựa chọn sai và đã xin lỗi.

hackernews · speckx · 10/6 16:42 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48478969)

**Bối cảnh**: Claude Fable 5 là mô hình Mythos‑class đầu tiên mà Anthropic công khai cung cấp, được mô tả là mô hình AI đa mục đích mạnh nhất đến nay và được claiming vượt qua các mô hình trước trong lập trình, kiến thức và thị giác. Mô hình này được quảng cáo là an toàn để sử dụng rộng rãi vì nó đi kèm với các guardrail nội 建 thành chặn đầu ra trong các lĩnh vực nguy cơ cao như an ninh mạng và sinh học. Mặc dù mục đích của các biện pháp này là ngăn chặn việc lạm dụng, chúng cũng có thể ảnh hưởng đến nghiên cứu hợp pháp nếu không được làm rõ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.cnbc.com/2026/06/09/anthropic-mythos-claude-fable-5.html">Anthropic releases Mythos-like AI model to the public two ... Anthropic’s Claude Fable is a version of Mythos the public ... Anthropic Launches Claude Fable 5, Its First Public Mythos ... Claude Fable 5: Anthropic's New Mythos-Class Model ... Anthropic Released Claude Fable 5, the First Model in the ... Claude Fable 5 from Anthropic now available on Amazon Bedrock</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-guardrails">What are AI guardrails? - IBM</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận cho rằng các guardrail ẩn là lừa đảo và làm mất niềm tin, vì mô hình sẽ im lặng chuyển sang phiên bản Opus yếu hơn khi xử lý các câu hỏi liên quan đến bảo mật. Một số người còn phàn nàn về chất lượng tổng thể của Fable, mức độ nhiều lời và tiêu thụ token, trong khi một vài người chia sẻ rằng dù được cấp miễn trừ vẫn bị chặn.

**Thẻ**: `#AI safety`, `#LLMs`, `#Anthropic`, `#cybersecurity research`, `#model guardrails`

---

<a id="item-3"></a>
## [Eric Ries tổ chức AMA về sách mới 'Incorruptible' thảo luận về trọng lực tài chính và lạc quan nhiệm vụ](https://news.ycombinator.com/item?id=48477135) ⭐️ 8.0/10

Eric Ries đã tổ chức một buổi AMA trên Hacker News để quảng bá sách mới 'Incorruptible,' trong đó giải thích cách trọng lực tài chính làm các công ty lạc quan khỏi sứ mệnh ban đầu và đưa ra ví dụ như Costco, Patagonia và Novo Nordisk đã chống lại nó. Cuộc thảo luận nhấn mạnh thách thức phổ biến ởスタートups và các công ty lớn—sự lạc quan khỏi sứ mệnh do áp lực tài chính—cung cấp các khung dirigeants để xây dựng các tổ chức bền vững, hướng tới mục đích. Điều này quan trọng đối với nhà khởi nghiệp, nhà đầu tư và chính sách tìm kiếm giá trị dài hạn hơn lợi nhuận ngắn hạn. Ries đã đưa ra thuật ngữ 'trọng lực tài chính' để mô tả lực lượng vô hình kéo công ty hướng tới hành vi tối đa hoá lợi nhuận, và ông nhắc đến sự tham gia của mình vào Sàn Chứng khoán Hàng dài, Answer.AI và tư vấn cho Anthropic như các nỗ lực chống lại nó. Ông cũng nhấn mạnh rằng cần có cấu trúc quản trị, không chỉ là lãnh đạo, để chống lại sự lạc quan.

hackernews · eries · 10/6 14:47

**Bối cảnh**: Eric Ries là tác giả của cuốn sách 'The Lean Startup,' một bản nền tảng phổ biến phương pháp phát triển sản phẩm lặp lại và học tập được xác thực trong các startup. Trọng lực tài chính, như ông sử dụng, chỉ áp lực hệ thống từ nhà đầu tư, thị trường và hệ thống 보상 که đẩy các tổ chức ra khỏi sứ mệnh ban đầu của chúng. Việc hiểu các lực lượng này giúp giải thích tại sao ngay cả các công ty thành công cũng có thể mất đi mục đích ban đầu theo thời gian.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://financialgravity.com/">Financial Gravity - Home of the Multi-Family Office Charter</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận gia elogi những hiểu biết của Ries, trong đó một số nhấn mạnh rằng lãnh đạo mạnh mẽ—như Jim Sinegal của Costco từ chối tăng giá hot‑dog—có thể chống lại trọng lực tài chính, trong khi những người khác cho rằng thay đổi bền vững cần có cấu trúc quản trị và sự phù hợp của động lực. Một số người liên tưởng tới doctrina Friedman, đặt ra câu hỏi liệu việc tối đa hoá lợi nhuận có nên là trách nhiệm duy nhất của công ty hay không.

**Thẻ**: `#lean-startup`, `#startup-culture`, `#mission-drift`, `#financial-gravity`, `#ama`

---

<a id="item-4"></a>
## [Anthropic thu hồi chính sách ẩn hạn chế Claude trong nghiên cứu LLM tiên tiến](https://simonwillison.net/2026/Jun/11/anthropic-walks-back-policy/#atom-everything) ⭐️ 8.0/10

Anthropic đã rút lại chính sách ẩn trong Claude Fable 5 sẽ giảm hiệu suất mô hình khi xử lý yêu cầu phát triển LLM tiên tiến sau khi đối mặt với sự phản đối mạnh mẽ. Họ tuyên bố sẽ làm cho các biện pháp bảo vệ trở nên minh bạch và xin lỗi vì sự mất cân bằng. Sự thay đổi này nhấn mạnh nhu cầu ngày càng tăng về sự trong suốt trong các biện pháp an toàn AI và cho thấy phản hồi từ nhà nghiên cứu có thể ảnh hưởng đến chính sách công ty, từ đó ảnh hưởng đến niềm tin vào các hệ thống AI được sử dụng cho công việc tiên tiến. Các biện pháp bảo vệ ẩn được nhúng trong thẻ hệ thống của Claude Fable 5 và sẽ giảm hiệu suất một cách im lặng khi thực hiện các nhiệm vụ nghiên cứu LLM tiên tiến mà không thông báo cho người dùng. Anthropic hiện nay nói rằng sẽ điều chỉnh các biện pháp bảo vệ của Fable 5 để trở nên visible và đã xin lỗi vì sự mất cân bằng.

rss · Simon Willison · 11/6 03:45

**Bối cảnh**: Claude Fable 5 là mô hình mạnh nhất được phát hành rộng rãi của Anthropic, thuộc lớp Mythos, được thiết kế cho các tác vụ suy luận phức tạp và tác nhân dài hạn. Thẻ hệ thống (system card) ghi lại khả năng, đánh giá an toàn và quyết định triển khai có trách nhiệm của các mô hình Claude. Các biện pháp bảo vệ ẩn được đưa ra để giảm thiểu rủi ro liên quan đến phát triển AI tiền tuyến, như nghiên cứu AI tự chủ hoặc tạo ra vũ khí, nhưng được áp dụng một cách không công khai, gây ra lo ngại về đạo đức và sự trong suốt.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://www.frontiermodelforum.org/technical-reports/frontier-mitigations/">Frontier Mitigations - Frontier Model Forum</a></li>

</ul>
</details>

**Thẻ**: `#AI`, `#AI ethics`, `#LLM`, `#policy`, `#Claude`

---

<a id="item-5"></a>
## [Google phát hành mô hình DiffusionGemma 26B trọng lượng mở qua NVIDIA NIM](https://simonwillison.net/2026/Jun/10/diffusiongemma/#atom-everything) ⭐️ 8.0/10

Google đã phát hành DiffusionGemma, mô hình sinh văn bản dựa trên diffusion có trọng lượng mở 26B tham số dưới giấy phép Apache 2, được lưu trữ miễn phí trên NVIDIA NIM. Mô hình này dựa trên nghiên cứu Gemini Diffusion trước đây và đạt tốc độ suy luận khoảng 857 token mỗi giây. DiffusionGemma cung cấp một lựa chọn mở và nhanh hơn so với các mô hình LLM tự回归 truyền thống, cho phép sinh văn bản với throughput cao cho nhà phát triển, đồng thời được truy cập miễn phí qua NVIDIA NIM. Giấy phép Apache 2 khuyến khích việc áp dụng rộng rãi và thử nghiệm trong cộng đồng AI. Mô hình có 26B tham số, sử dụng giải mã song song dựa trên diffusion với ngữ cảnh hai chiều và tự sửa lỗi, và có sẵn trên Hugging Face dưới tên google/diffusiongemma-26B-A4B-it. NVIDIA NIM cung cấp API lưu trữ miễn phí, và bản phát hành được cấp phép Apache 2.

rss · Simon Willison · 10/6 20:00

**Bối cảnh**: Sinh văn bản dựa trên diffusion thay vì dự đoán token theo thứ tự bằng quá trình lọc nhiễu lặp lại, cho phép tính toán song song và có thể suy luận nhanh hơn. Nghiên cứu Gemini Diffusion trước đây của Google đã khám phá phương pháp này cho mô hình ngôn ngữ. NVIDIA NIM (Microservices Dịch vụ Suy luận) cung cấp các container được tối ưu trước để triển khai mô hình AI trên cơ sở hạ tầng được tăng tốc bằng GPU.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini-diffusion/">Gemini Diffusion — Google DeepMind</a></li>
<li><a href="https://developers.googleblog.com/diffusiongemma-the-developer-guide/">DiffusionGemma: The Developer Guide - Google Developers Blog</a></li>
<li><a href="https://www.nvidia.com/en-us/ai-data-science/products/nim-microservices/">NVIDIA NIM Microservices for AI Inference</a></li>

</ul>
</details>

**Thẻ**: `#diffusion models`, `#text generation`, `#Gemma`, `#open weight`, `#NVIDIA NIM`

---

<a id="item-6"></a>
## [NVIDIA lưu trữ phiên bản quantized của DiffusionGemma 26B A4B IT trên Hugging Face](https://www.reddit.com/r/LocalLLaMA/comments/1u2np0a/nvidiadiffusiongemma26ba4bitnvfp4_hugging_face/) ⭐️ 8.0/10

NVIDIA và Hugging Face đã phát hành phiên bản quantized của mô hình DiffusionGemma 26B A4B IT của Google DeepMind, một mô hình đa phương thức MoE chấp nhận đầu vào văn bản, hình ảnh và video và tạo ra văn bản qua discrete diffusion. Mô hình cung cấp trọng số mở với bối cảnh 256K token, tốc độ sinh hơn 1.100 token/giây và chức năng gọi hàm gốc, giúp AI đa phương thức tốc độ cao trở nên dễ dàng truy cập cho nhà phát triển và nhà nghiên cứu. Xây dựng trên kiến trúc MoE Gemma 4 26B A4B với 25,2 tỷ tham số tổng và 3,8 tỷ tham số hoạt động, mô hình được lượng hóa NVFP4 bằng NVIDIA Model Optimizer, chạy trên Hopper H100 (FP8) vượt quá 1.100 token/giây, hỗ trợ hơn 35 ngôn ngữ, chế độ suy luận có thể cấu hình và gọi hàm gốc.

reddit · r/LocalLLaMA · /u/pmttyji · 11/6 03:28

**Bối cảnh**: DiffusionGemma là một mô hình ngôn ngữ diffusion sinh ra văn bản bằng cách sử dụng Uniform State Diffusion, xen kẽ giữa các bước prefill tăng dần và giảm nhiễu, và được tinh chỉnh từ checkpoint Gemma 4 26B A4B. Mô hình Gemma 4 26B A4B sử dụng kiến trúc Sparse Mixture-of-Experts với 128 chuyên gia, chỉ kích hoạt khoảng 3,8–4 tỷ tham số mỗi token để đạt throughput cao đồng thời giữ lại khả năng mô hình lớn. Lượng hóa NVFP4 của NVIDIA, được thực hiện qua TensorRT Model Optimizer, giảm độ chính xác xuống định dạng số thực chấm động 4 bit mà vẫn duy trì độ chính xác và tăng đáng kể tốc độ suy luận trên GPU Hopper.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/diffusiongemma/explained">Diffusion in Text Generation Explained | Gemma | Google AI for...</a></li>
<li><a href="https://www.mindstudio.ai/blog/gemma-4-mixture-of-experts-architecture-explained">What Is Gemma 4's Mixture of Experts Architecture? How 26B Parameters ...</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Thẻ**: `#multimodal`, `#diffusion`, `#Gemma`, `#NVIDIA`, `#HuggingFace`

---

<a id="item-7"></a>
## [FlashMemory-DeepSeek-V4 ra mắt cơ chế Lookahead Sparse Attention cho LLM context siêu dài.](https://www.reddit.com/r/LocalLLaMA/comments/1u277fg/flashmemorydeepseekv4_lightning_index_ultralong/) ⭐️ 8.0/10

Bài báo giới thiệu cơ chế Lookahead Sparse Attention (LSA), một paradigm suy luận mới sử dụng Bộ Nhớ Neural được xây dựng trên kiến trúc DeepSeek‑V4 để dự đoán nhu cầu ngữ cảnh trong tương lai và giữ lại chỉ các khối KV liên quan đến truy vấn trong bộ nhớ GPU. Việc huấn luyện bộ chỉ mục dưới dạng dual‑encoder được tách rời giúp giảm dung lượng bộ nhớ KV vật lý xuống còn 13,5 % so với mức cơ bản đầy đủ trong khi vẫn duy trì hoặc nâng cao độ chính xác trên các benchmark context dài. Việc giảm đáng kể bộ nhớ KV cache cần thiết để sinh ra văn bản dài giúp LSA cho phép triển khai mô hình có hàng trăm nghìn token trên GPU thông thường, giảm chi phí và độ trễ. Điều này mở rộng khả năng mở rộng của LLM cho các ứng dụng như trả lời câu hỏi ở mức tài liệu, tóm tắt dài và sinh tăng cường truy xuất. Bộ chỉ mục được triển khai dưới dạng dual‑encoder tiêu chuẩn được huấn luyện độc lập bằng mục tiêu truy xuất, không cần tải toàn bộ bộ xương DeepSeek‑V4 vào bộ nhớ GPU. Thí nghiệm cho thấy dung lượng bộ nhớ KV vật lý giảm xuống còn 13,5 % so với mức cơ bản trên các bộ benchmark LongBench‑v2, LongMemEval và RULER, đồng thời độ chính xác downstream tăng trung bình +0,6 %; ở bối cảnh 500 000 token, bộ nhớ KV được giảm hơn 90 % mà không làm suy giảm khả năng reasoning của mô hình.

reddit · r/LocalLLaMA · /u/pmttyji · 10/6 16:30

**Bối cảnh**: Trong các mô hình LLM tự回归, bộ nhớ key‑value (KV) lưu trữ các trạng thái ẩn của tất cả các token đã sinh ra, khiến mức tiêu thụ bộ nhớ tăng tuyến tính theo độ dài ngữ cảnh và trở thành nút thắt cho các chuỗi siêu dài. Lookahead Sparse Attention (LSA) thay thế bộ nhớ KV mật bằng một Bộ Nhớ Neural dự đoán quais token quá khứ sẽ cần thiết và chỉ giữ lại các khối KV quan trọng trong bộ nhớ GPU. Bộ chỉ mục được xây dựng dưới dạng dual‑encoder và được huấn luyện độc lập bằng mục tiêu truy xuất tiêu chuẩn, do đó bộ xương DeepSeek‑V4 khổng lồ không bao giờ cần được tải vào bộ nhớ trong quá trình huấn luyện bộ chỉ mục.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.09079">[2606.09079] FlashMemory-DeepSeek-V4: Lightning Index Ultra ...</a></li>
<li><a href="https://www.emergentmind.com/topics/dual-encoder-retriever">Dual-Encoder Retriever Overview - emergentmind.com</a></li>
<li><a href="https://ai-brief.liziran.com/en/daily/2026-06-11-deepseek-v4-sparse-kv-latent-memory.html">DeepSeek V4 Cuts KV to 13.5%, Video Memory Runs 10x Faster</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#Long-context`, `#Sparse Attention`, `#GPU Memory Optimization`, `#DeepSeek-V4`

---

<a id="item-8"></a>
## [πFS](https://github.com/philipl/pifs) ⭐️ 7.0/10

πFS là một hệ thống tệp 'không dữ liệu' hóm hỉnh, mã hóa các tệp dưới dạng các vị trí và độ dài trong các chữ số của π, nhấn mạnh giới hạn lý thuyết của nén.

hackernews · helterskelter · 10/6 18:54 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48480978)

**Thẻ**: `#filesystems`, `#data compression`, `#information theory`, `#π`, `#humor`

---

<a id="item-9"></a>
## [PgDog đã được tài trợ và sắp xuất hiện gần một cơ sở dữ liệu gần bạn](https://pgdog.dev/blog/our-funding-announcement) ⭐️ 7.0/10

PgDog thông báo về việc đã nhận được vốn để xây dựng một proxy giúp PostgreSQL mở rộng khả năng ghi và cải thiện tính sẵn sàng.

hackernews · levkk · 10/6 14:02 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48476466)

**Thẻ**: `#PostgreSQL`, `#database scaling`, `#proxy`, `#funding`, `#high availability`

---

<a id="item-10"></a>
## [Google phát hành hướng dẫn phát triển cho DiffusionGemma, mô hình diffusion mới](https://www.reddit.com/r/LocalLLaMA/comments/1u26oyp/diffusiongemma_the_developer_guide_google/) ⭐️ 7.0/10

Google đã công bố hướng dẫn phát triển cho DiffusionGemma, một mô hình ngôn ngữ lớn dựa trên diffusion được xây dựng trên kiến trúc Gemma, cung cấp chi tiết về cách sử dụng và triển khai mô hình để tạo văn bản song song và nhanh hơn. Hướng dẫn này giúp các nhà phát triển tận dụng khả năng giải mã song song và tự sửa lỗi của DiffusionGemma, từ đó tăng tốc ứng dụng AI thời gian thực và mở rộng việc áp dụng các mô hình LLM dựa trên diffusion. DiffusionGemma thay thế quá trình sinh token theo thứ tự tự hồi quy bằng quá trình khử nhiễu diffusion 양 hướng, cho phép sinh nhiều token song song và hỗ trợ tự sửa lỗi trong quá trình sinh.

reddit · r/LocalLLaMA · /u/tevlon · 10/6 16:12

**Bối cảnh**: Gemma là họ mô hình ngôn ngữ lớn decoder‑only được phát triển bởi Google DeepMind, bao gồm các phiên bản từ Gemma 2 (2024) đến Gemma 4 (2026) và các biến thể như PaliGemma. Các mô hình diffusion tạo ra dữ liệu bằng quá trình lặp đi lặp lại khử nhiễu từ tiếng ngẫu nhiên, và khi áp dụng vào mô hình ngôn ngữ chúng cho phép sinh song song các token, khác với các LLM tự hồi quy truyền thống. DiffusionGemma kết hợp kiến trúc decoder của Gemma với quá trình khử nhiễu diffusion để đạt được tốc độ suy luận nhanh hơn và ngữ cảnh 양 hướng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://developers.googleblog.com/diffusiongemma-the-developer-guide/">DiffusionGemma: The Developer Guide - Google Developers Blog</a></li>
<li><a href="https://developers.googleblog.com/en/gemma-explained-overview-gemma-model-family-architectures/">Gemma explained: An overview of Gemma model family architectures</a></li>
<li><a href="https://www.educative.io/blog/how-do-diffusion-models-work">How do Diffusion Models work ?</a></li>

</ul>
</details>

**Thẻ**: `#DiffusionGemma`, `#Google`, `#developer guide`, `#AI/ML`, `#open models`

---

<a id="item-11"></a>
## [AMD nhấn mạnh kiến trúc bộ nhớ thống nhất cho dòng Ryzen AI MAX 400](https://www.reddit.com/r/LocalLLaMA/comments/1u2l25d/amd_touts_the_unified_memory_architecture/) ⭐️ 7.0/10

AMD đã nhấn mạnh rằng kiến trúc bộ nhớ thống nhất (UMA) sẽ định hình lộ trình sản phẩm trong tương lai, đặc biệt là dòng Ryzen AI MAX 400 (mã Gorgon Halo) được thiết kế cho các tác vụ AI. Kiến trúc UMA cho phép CPU và GPU chia sẻ một vùng bộ nhớ nhất quán, giảm chi phí chuyển dữ liệu và có thể tăng hiệu suất cho các mô hình AI địa phương và LLM. Điều này có thể làm cho các chip Ryzen AI MAX 400 của AMD trở nên hấp dẫn đối với nhà phát triển tìm kiếm xử lý AI trên thiết bị hiệu quả. Các APU Ryzen AI MAX 400 (Gorgon Halo) dự kiến sẽ sử dụng nhân CPU Zen 5 kết hợp với đồ họa RDNA 3.5. Chúng sẽ hỗ trợ tối đa 192 GB bộ nhớ thống nhất và có tần số đồng hồ lên tới 5,2 GHz.

reddit · r/LocalLLaMA · /u/Terminator857 · 11/6 01:25

**Bối cảnh**: Kiến trúc bộ nhớ thống nhất (UMA) cho phép các loại bộ xử lý khác nhau, như CPU và GPU, truy cập vào một không gian bộ nhớ vật lý và ảo nhất quán, giúp đơn giản hóa quản lý bộ nhớ. Các APU của AMD đã lâu sử dụng UMA để tích hợp CPU và GPU trên cùng một mảnh silicon. Dòng Ryzen AI MAX 400 sắp tới mở rộng cách tiếp cận này cho các tác vụ AI hiệu suất cao, kết hợp nhân Zen 5 với đồ họa RDNA 3.5.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://wccftech.com/amd-unified-memory-architectures-open-up-a-world-of-possibilities-shape-product-roadmaps/">AMD Believes Unified Memory Architectures Open Up ... - Wccftech</a></li>
<li><a href="https://rocm.docs.amd.com/projects/HIP/en/docs-6.2.0/how-to/unified_memory.html">Unified memory — HIP 6.2.41133 Documentation - AMD</a></li>
<li><a href="https://www.tomshardware.com/pc-components/cpus/amd-ryzen-ai-max-400-gorgon-halo-packs-up-to-192gb-of-unified-memory-refreshed-apu-uses-zen-5-and-rdna-3-5-and-can-clock-up-to-5-2-ghz">AMD Ryzen AI Max 400 ‘Gorgon Halo’ packs up to 192GB of ...</a></li>

</ul>
</details>

**Thẻ**: `#AMD`, `#Unified Memory Architecture`, `#AI Hardware`, `#Ryzen AI`, `#Local LLM`

---

<a id="item-12"></a>
## [Datasette-agent 0.2a0 thêm tính năng hỏi người dùng tương tác có trạng thái lưu trữ](https://simonwillison.net/2026/Jun/10/datasette-agent/#atom-everything) ⭐️ 6.0/10

Phiên bản Datasette-agent 0.2a0 ra mắt phương thức ToolContext.ask_user() cho phép công cụ đặt câu hỏi yes/no, trọn lựa chọn hoặc tự do với người dùng trong quá trình thực hiện, tạm dừng lượt agent và lưu trạng thái vào cơ sở dữ liệu nội bộ để tồn tại sau khi khởi động lại máy chủ. Ngoài ra, bản phát hành còn cung cấp công cụ save_query tích hợp sẵn cho phép agent lưu trữ câu SQL dưới dạng truy vấn đã lưu của Datasette chỉ sau khi nhận được sự đồng ý rõ ràng từ con người. Khả năng tạm dừng và tiếp tục thực thi agent với đầu vào từ người dùng làm cho việc khám phá dữ liệu được hỗ trợ bởi AI trở nên an toàn và minh bạch hơn, cho phép quy trình có con người tham gia có thể tồn tại qua việc khởi động lại hệ thống. Điều này nâng cao tính khả dụng của các agent dựa trên LLM cho quy trình SQL tương tác trong Datasette. ask_user() có thể nhận tham số cho câu hỏi yes/no, danh sách lựa chọn hoặc free_text=True; khi chưa có câu trả lời, lượt agent bị tạm dừng, câu hỏi hiển thị dưới dạng biểu mẫu trong giao diện chat và trạng thái được lưu vào cơ sở dữ liệu nội bộ. Khi có câu trả lời, công cụ sẽ thực thi lại từ đầu với các câu trả lời đã lưu được phát lại, vì vậy các tác động phụ nên xảy ra sau khi gọi ask_user(). Công cụ save_query luôn yêu cầu người dùng nhấn Yes sau khi xem lại toàn bộ SQL, tên mục tiêu, cơ sở dữ liệu và mức độ hiển thị. Tính năng này được xây dựng bằng một phiên bản LLM alpha mới được tạo với sự giúp đỡ của Claude Fable 5.

rss · Simon Willison · 10/6 23:57

**Bối cảnh**: Datasette là một công cụ mã nguồn mở để khám phá và xuất bản dữ liệu lưu trữ trong các cơ sở dữ liệu SQLite. Datasette‑agent là một trợ lý được cung cấp bởi LLM cho phép người dùng tương tác với một phiên bản Datasette bằng ngôn ngữ tự nhiên để tạo và chạy các truy vấn SQL. Các phiên bản trước của agent chỉ có thể thực thi các công cụ được xác định trước mà không cần dừng để nhận đầu vào từ người dùng, và bất kỳ trạng thái cuộc trò chuyện nào cũng sẽ bị mất nếu máy chủ khởi động lại. Phiên bản 0.2a0 bổ sung tính năng đặt câu hỏi tương tác có trạng thái được lưu trữ để khắc phục những hạn chế này.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/10/datasette-agent/">Release: datasette-agent 0.2a0</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and analyze data in SQLite</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette/datasette-agent: An LLM-powered agent for Datasette</a></li>

</ul>
</details>

**Thẻ**: `#datasette`, `#agent`, `#interactive`, `#SQL`, `#release`

---

<a id="item-13"></a>
## [Jeremy Howard đề xuất lab AI top không dùng mô hình của mình](https://simonwillison.net/2026/Jun/10/jeremy-howard/#atom-everything) ⭐️ 6.0/10

Jeremy Howard đề xuất phòng thí viện có mô hình AI hàng đầu nên tránh sử dụng nó để nghiên cứu AI tiền phong, đồng thời cho phép người khác truy cập, nhằm chậm lại quá trình tự cải thiện đệ quy và tránh mất cân bằng quyền lực. Đề xuất này nhấn mạnh một cách tiếp cận về quản trị để giảm thiểu rủi ro từ sự tự cải thiện không kiểm soát của AI và tập trung quyền lực, có thể ảnh hưởng đến chính sách an toàn AI và thực hành của các phòng thí viện. Howard lưu ý rằng nếu một phòng thí viện tuyên bố nên chậm lại tự cải thiện nhưng vẫn sử dụng mô hình hàng đầu để nghiên cứu AI tiền phong, thì đó là mâu thuẫn; ông đối lập điều này với thực tiễn hiện tại của Anthropic, cho phép đội ngũ của mình sử dụng mô hình hàng đầu để nghiên cứu tiền phong.

rss · Simon Willison · 10/6 15:23

**Bối cảnh**: Recursive self-improvement (RSI) là quá trình một hệ thống AI sửa đổi mã nguồn của mình để nâng cao khả năng, có thể dẫn đến sự nổ vời trí tuệ. Frontier AI là các mô hình AI tiên tiến nhất hiện có, có khả năng suy luận rộng, viết mã và phân tích. Anthropic là công ty nghiên cứu và an toàn AI, nổi tiếng với việc phát triển các mô hình như Claude và nhấn mạnh tính giải thích được và khả năng điều khiển.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://techglimmer.io/frontier-ai-review-2026-frontier-ai-models-2026/">What Is Frontier AI and Why Is Everyone Talking About It?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#AI safety`, `#AI governance`, `#recursive self-improvement`, `#Jeremy Howard`, `#policy`

---

<a id="item-14"></a>
## [Thượng nghị sĩ Cynthia Lummis khuyên Mỹ nên tích lũy Bitcoin công khai theo luật](https://www.reddit.com/r/CryptoCurrency/comments/1u2ikak/senator_cynthia_lummis_other_nations_are/) ⭐️ 6.0/10

Thượng nghị sĩ Cynthia Lummis nói rằng các quốc gia khác đang tích lũy Bitcoin im lặng và cho rằng Hoa Kỳ nên làm điều đó một cách công khai và hợp pháp thông qua luật pháp. Nhận xét của cô ấy nhấn mạnh sự ủng hộ chính trị ngày càng tăng đối với việc xem Bitcoin như một tài sản dự trữ quốc gia, điều này có thể định hình chính sách mã hóa của Mỹ, tăng niềm tin thị trường và khuyến khích việc áp dụng rộng rãi từ phía các tổ chức. Lummis chỉ đến Luật BITCOIN (S.954) đề xuất một dự trữ Bitcoin chiến lược được quản lý bởi Bộ Tài chính, với lợi nhuận có thể được dùng để giảm nợ quốc gia hoặc tăng mức sở hữu, đồng thời ghi nhận các báo cáo về việc mua Bitcoin ẩn danh bởi các quốc gia không được tên.

reddit · r/CryptoCurrency · /u/zesushv · 10/6 23:32

**Bối cảnh**: Bitcoin là một loại tiền điện tử phi tập trung được ra đời năm 2008, và một số chính phủ đã bắt đầu khám phá hoặc mua Bitcoin im lặng như một phần của dự trữ. Các cuộc thảo luận gần đây đã nhắc đến khả năng có một dự trữ Bitcoin chiến lược tại Mỹ, nhằm quản lý một cách minh bạch các khoản Bitcoin củaรัฐ phủ. Các báo cáo về việc mua Bitcoin ẩn danh bởi các quốc gia khác cũng đã xuất hiện, cho thấy sự quan tâm ngày càng tăng đến Bitcoin như một tài sản dự trữ tương đương với vàng số.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.congress.gov/bill/119th-congress/senate-bill/954/text">Text - S.954 - 119th Congress (2025-2026): BITCOIN Act of ... TH D CONGRESS SESSION S. ll - Senator Cynthia Lummis Congress Reveals First Detailed Look at Strategic Bitcoin Reserve The BITCOIN Act Of 2024 US Strategic Bitcoin Reserve (2026): Government Custody ... Establishment of the Strategic Bitcoin ... - Federal Register</a></li>
<li><a href="https://news.bitcoin.com/stealth-nation-reported-to-be-purchasing-bitcoin-covertly/">Stealth Nation Reported to Be Purchasing Bitcoin Covertly</a></li>
<li><a href="https://www.ainvest.com/news/white-house-hints-bitcoin-accumulation-plan-2506/">U.S. White House Hints at Bitcoin Accumulation Plan</a></li>

</ul>
</details>

**Thẻ**: `#Bitcoin`, `#cryptocurrency policy`, `#US legislation`, `#Senator Cynthia Lummis`, `#digital assets`

---

<a id="item-15"></a>
## [BofA CEO cảnh báo stablecoin lợi nhuận rút 35% tiền gửi ngân hàng Mỹ](https://www.reddit.com/r/CryptoCurrency/comments/1u23u6a/bofa_ceo_warns_stablecoin_yield_could_drain_35_of/) ⭐️ 6.0/10

Giám đốc Ngân hàng Bank of America Brian Moynihan cảnh báo rằng lợi nhuận cao từ stablecoin có thể hút tới 35% tổng tiền gửi ngân hàng Mỹ ra khỏi các ngân hàng truyền thống. Chuyển đổi này có thể giảm khả năng cho vay của ngân hàng, áp lực vào biên lợi nhuận netto và thúc đẩy các ngân hàng truyền thống phải cung cấp sản phẩm tài sản số cạnh tranh hơn. Cảnh báo của Moynihan được đưa ra khi lợi nhuận trên stablecoin sinh lời, được hỗ trợ bởi trái phiếu Mỹ ngắn hạn, đang cung cấp APY trong mức thấp đến trung bình một chữ số.

reddit · r/CryptoCurrency · /u/andix3 · 10/6 14:30

**Bối cảnh**: Stablecoin là loại tiền mã hoá được thiết kế để duy trì giá trị 1:1 so với tài sản như đô la Mỹ, thường thông qua dự trữ hoặc thuật toán. Stablecoin sinh lời tạo ra lợi nhuận cho người giữ bằng cách đầu tư dự trữ vào tài sản ít rủi ro như trái phiếu Mỹ ngắn hạn, đồng thời vẫn cố gắng giữ giá trị ổn định. Tổng giá trị tiền gửi ngân hàng Mỹ vượt quá 17 nghìn tỷ USD, vì vậy zelfs một phần nhỏ chuyển sang stablecoin cũng có thể đạt hàng trăm tỷ USD. Các nhà quản lý trên toàn thế giới đang tăng cường giám sát việc phát hành stablecoin khi sử dụng của chúng tăng lên.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stablecoin">Stablecoin</a></li>
<li><a href="https://grokipedia.com/page/Yield-bearing_stablecoin">Yield-bearing stablecoin</a></li>

</ul>
</details>

**Thẻ**: `#banking`, `#stablecoins`, `#finance`, `#cryptocurrency`, `#regulation`

---