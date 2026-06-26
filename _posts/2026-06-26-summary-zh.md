---
layout: default
title: "Horizon Summary: 2026-06-26 (ZH)"
date: 2026-06-26
lang: zh
---

> Đã chọn 9 tin quan trọng từ 11 nội dung.

---

1. [Đọc được toàn bộ cuộn Herculaneum lần đầu nhờ AI và giải mở ảo](#item-1) ⭐️ 9.0/10
2. [JetSpec: Phân Cây Song Song Tăng Tốc Suy Diễn LLM Lên 9.64×](#item-2) ⭐️ 9.0/10
3. [Thời đại 'giấy tờ, xin vui lòng' trên internet sẽ phá hủy quyền riêng tư của bạn](#item-3) ⭐️ 8.0/10
4. [Toà án Đức quy định Google chịu trách nhiệm về lỗi trong AI Overviews.](#item-4) ⭐️ 8.0/10
5. [audio.cpp: 12 mô hình âm thanh (Qwen3-TTS, PocketTTS, VeVo2 v.v.) trong một runtime C++/ggml — TTS nhanh hơn Python lên đến 5 lần trên CUDA](#item-5) ⭐️ 8.0/10
6. [Ornith-1.0 được phát hành trên Hugging Face với mô hình 9B‑397B](#item-6) ⭐️ 8.0/10
7. [OpenMontage ra mắt hệ thống sản xuất video agentic mã nguồn mở](#item-7) ⭐️ 8.0/10
8. [Om Malik, Nhà Báo Công Nghệ Ảnh Hưởng, Tử Vong Tại Tuổi 60](#item-8) ⭐️ 6.0/10
9. [Apple bỏ M6 Pro/Max, ưu tiên M7 cho AI địa phương.](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Đọc được toàn bộ cuộn Herculaneum lần đầu nhờ AI và giải mở ảo](https://scrollprize.org/firstscroll) ⭐️ 9.0/10

Các nhà nghiên cứu đã thành công trong việc giải mở ảo và đọc toàn bộ một cuộn Herculaneum bằng cách sử dụng phân đoạn và phát hiện mực dựa trên AI, do đó tiết lộ văn bản Hy Lạp cổ đại lần đầu tiên. Công trình này chứng minh rằng việc sử dụng AI và hình ảnh tiên tiến có thể mở khóa di sản văn hóa không thể tiếp cận, mở khả năng đọc hàng trăm cuộn khác bị hoà than tại Villa of the Papyri và cách mạng hóa nghiên cứu khảo cổ. Quy trình bao gồm quét cuộn bằng CT X‑ray độ phân giải cao, phân đoạn lớp giấy bông trong không gian 3D và huấn luyện mô hình học máy để phát hiện mực carbon dựa trên dữ liệu dưới đỏ ground truth. Mặc dù thành công, phương pháp hiện tại hoạt động tốt nhất trên các phần relativamente phẳng, chưa được cuộn và đòi hỏi tài nguyên tính toán lớn, đồng thời văn bản được khôi phục vẫn còn khoảng trống do hư hỏng và việc phát hiện mực chưa hoàn chỉnh.

hackernews · verditelabs · 25/6 15:48 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48675179)

**Bối cảnh**: Các cuộn Herculaneum là những bản ghi trên giấy bông bị hoà than do sự phun trào của núi Vesuvius năm 79 AD, được phát hiện trong Villa of the Papyri. Việc mở ra vật lý thường làm hỏng các cuộn này, vì vậy các nhà nghiên cứu sử dụng kỹ thuật giải mở ảo qua quét CT và AI để xem lớp bên trong mà không làm ảnh hưởng đến cuộn. Cuộc thi Vesuvius Challenge đã thúc đẩy sự tiến bộ trong việc phát hiện mực và phân đoạn, cung cấp giải thưởng cho các nhóm khôi phục được văn bản đọc được. Cho tới nay đã trao hơn 1,8 triệu USD.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://scrollprize.org/unwrapping">Virtual Unwrapping | Vesuvius Challenge</a></li>
<li><a href="https://scrollprize.org/">Vesuvius Challenge — Reading the Herculaneum Scrolls with AI</a></li>
<li><a href="https://scrollprize.org/tutorial5">Tutorial: Ink Detection | Vesuvius Challenge</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận viên thể hiện sự kỳ vọng và ngưỡng mộ trước kỳ tích kỹ thuật này và mối liên hệ với các triết gia cổ đại, đồng thời một thành viên trong đội ngũ提出 sẵn sàng trả lời câu hỏi về quá trình phân đoạn và phát hiện mực. Nhiều người chỉ ra khả năng tồn tại của nhiều cuộn Herculaneum chưa được khám phá và xem công việc này như một dấu hiệu tích cực chống lại những câu chuyện tiêu cực về công nghệ. Một số người cũng nhắc tới tiến bộ bổ sung từ việc giải mở thêm các cuộn khác, cho thấy tốc độ phát hiện đang tăng nhanh.

**Thẻ**: `#archaeology`, `#AI`, `#imaging`, `#Vesuvius Challenge`, `#cultural heritage`

---

<a id="item-2"></a>
## [JetSpec: Phân Cây Song Song Tăng Tốc Suy Diễn LLM Lên 9.64×](https://www.reddit.com/r/LocalLLaMA/comments/1ufntl5/research_jetspec_speculative_decoding_with/) ⭐️ 9.0/10

JetSpec giới thiệu phương pháp phác thảo cây song song nhân quả để giải mã suy đoán, đạt được tăng tốc vô mất mát lên tới 9.64× trên MATH-500 và khoảng 1000 token mỗi giây trên một GPU B200. Đột phá này đẩy suy diễn LLM hướng tới các ứng dụng tương tác thời gian thực bằng cách giảm trễ đáng kể mà vẫn giữ nguyên chất lượng output, mang lại lợi ích cho nhà phát triển và người dùng các mô hình ngôn ngữ lớn. JetSpec sử dụng đầu phác thảo cây song song nhân quả một lần qua, kết hợp CUDA graph và tối ưu kernel để giảm chi phí phác thảo đồng thời duy trì tính nhất quán tự hồi quy, đạt 4.58× tăng tốc trên benchmark chat mở.

reddit · r/LocalLLaMA · /u/No_Yogurtcloset_7050 · 25/6 21:55

**Bối cảnh**: Giải mã suy đoán tăng tốc việc sinh ra token của LLM bằng cách sử dụng một mô hình phác thảo nhẹ để đề xuất chuỗi token, sau đó được mô hình đích xác thực, từ đó giảm số bước tự hồi quy. Phác thảo có cấu trúc cây mở rộng ý tưởng này bằng việc tạo ra một tập hợp các ứng viên token có nhánh song song, cho phép chấp nhận tiền tố dài hơn khi phác thảo phù hợp với phân phối của mô hình đích. CUDA graph ghi lại chuỗi các thao tác GPU để phát lại nhanh, giảmภาระ khởi động kernel và tăng throughput trong các công việc lặp như sinh token theo từng bước.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00735/128189/OPT-Tree-Speculative-Decoding-with-Adaptive-Draft">OPT-Tree: Speculative Decoding with Adaptive Draft Tree Structure | Transactions of the Association for Computational Linguistics | MIT Press</a></li>
<li><a href="https://arxiv.org/html/2410.05589v1">ParallelSpec: Parallel Drafter for Efficient Speculative Decoding</a></li>
<li><a href="https://deepwiki.com/harleyszhang/llm_note/4.2-cuda-graph-optimization">CUDA Graph Optimization | harleyszhang/llm_note | DeepWiki</a></li>

</ul>
</details>

**Thẻ**: `#LLM inference`, `#speculative decoding`, `#parallel tree drafting`, `#GPU optimization`, `#performance improvement`

---

<a id="item-3"></a>
## [Thời đại 'giấy tờ, xin vui lòng' trên internet sẽ phá hủy quyền riêng tư của bạn](https://expression.fire.org/p/the-papers-please-era-of-the-internet) ⭐️ 8.0/10

Bài viết cảnh báo rằng việc mở rộng yêu cầu xác thực tuổi và giấy tờ trực tuyến ('giấy tờ, xin vui lòng') làm suy giảm quyền riêng tư của người dùng, gây ra tranh luận về các giải pháp kỹ thuật và những trade-off xã hội.

hackernews · bilsbie · 25/6 21:44 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48679608)

**Thẻ**: `#privacy`, `#age verification`, `#internet regulation`, `#anonymous credentials`, `#security`

---

<a id="item-4"></a>
## [Toà án Đức quy định Google chịu trách nhiệm về lỗi trong AI Overviews.](https://simonwillison.net/2026/Jun/25/ai-and-liability/#atom-everything) ⭐️ 8.0/10

Toà án khu vực Đức đã tuyên bố Google chịu trách nhiệm trực tiếp về các tuyên bố sai trong AI Overviews, coi nội dung tạo bởi AI như là lời nói của Google; Bruce Schneier bình luận rằng AI nên được xem là tác nhân của người triển khai. Quyết định này có thể tạo ra precedente để chịu trách nhiệm về những ảo 觉 của AI, ảnh hưởng đến cách các công ty triển khai AI sinh tạo và ảnh hưởng đến các luật trách nhiệm AI trong tương lai trên toàn cầu. Toà án phát hiện AI Overviews của Google đã sai lầm liên kết hai nhà xuất bản với gian lobal và đưa ra các tuyên bố không xuất hiện trong nguồn gốc, từ đó loại bỏ bảo vệ trách nhiệm hữu hạn thường áp dụng cho các nhà điều tra công cụ tìm kiếm.

rss · Simon Willison · 25/6 22:28

**Bối cảnh**: AI Overviews là một tính năng của Google Search cung cấp bản tóm tắt được tạo bởi AI cho kết quả tìm kiếm, được ra mắt lần đầu như một phần của Trải nghiệm Tạo sinh của Tìm kiếm vào năm 2023 và được đổi tên lại vào năm 2024. Các nhà pháp lý đã tranh luận về việc liệu hệ thống AI có nên được xem là tác nhân của người triển khai để xác định trách nhiệm, với một số lý thuyết hiện có đã đặt trách nhiệm trực tiếp lên người vận hành AI.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://the-decoder.com/landmark-german-ruling-declares-googles-ai-overviews-are-googles-own-words-and-makes-it-liable-for-false-answers/">Landmark German ruling declares Google's AI Overviews are ...</a></li>
<li><a href="https://www.technology.org/2026/06/12/german-court-google-ai-overviews-liable/">German Court Holds Google Liable for AI Lies - Technology Org</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>

</ul>
</details>

**Thẻ**: `#AI liability`, `#legal policy`, `#Google AI overviews`, `#Bruce Schneier`, `#AI ethics`

---

<a id="item-5"></a>
## [audio.cpp: 12 mô hình âm thanh (Qwen3-TTS, PocketTTS, VeVo2 v.v.) trong một runtime C++/ggml — TTS nhanh hơn Python lên đến 5 lần trên CUDA](https://www.reddit.com/r/LocalLLaMA/comments/1ufpnm6/audiocpp_12_audio_models_qwen3tts_pockettts_vevo2/) ⭐️ 8.0/10

audio.cpp cung cấp một framework suy luận C++ gốc hỗ trợ 12 mô hình âm thanh (TTS, ASR, chuyển đổi giọng nói) với cải thiện tốc độ đáng kể so với các giải pháp dựa trên Python.

reddit · r/LocalLLaMA · /u/Acceptable-Cycle4645 · 25/6 23:10

**Thẻ**: `#C++`, `#TTS`, `#audio models`, `#ggml`, `#performance`

---

<a id="item-6"></a>
## [Ornith-1.0 được phát hành trên Hugging Face với mô hình 9B‑397B](https://www.reddit.com/r/LocalLLaMA/comments/1ufc9vp/ornith10_released_on_hugging_face/) ⭐️ 8.0/10

Ornith-1.0 ra mắt một họ mô hình ngôn ngữ dense và mixture-of-experts có quy mô từ 9 B đến 397 B tham số, được phát hành trên Hugging Face và tuyên bố đạt kết quả state‑of‑the‑art trên nhiều benchmark. Phát hành này cung cấp cho cộng đồng nghiên cứu các mô hình trọng lượng mở lớn, chuyên biệt cho mã hóa tác động (agentic coding), có thể tăng tốc phát triển các trợ lý phần mềm do AI 駕駛 và giảm thiểu rào cản để thử nghiệm LLM hiệu suất cao. Gia đình bao gồm các biến thể 9B dense, 31B dense, 35B MoE và 397B MoE, đều được cấp phép MIT, phát hành vào ngày 26/06/2026, không có giới hạn khu vực và tập trung vào các tác vụ mã hóa tác động.

reddit · r/LocalLLaMA · /u/paf1138 · 25/6 14:52

**Bối cảnh**: Kiến trúc Mixture‑of‑Experts (MoE) là một mạng nơ-ron phân phối các token đầu vào cho các mạng con chuyên gia cụ thể, cho phép mô hình lớn vẫn tính toán hiệu quả. Các mô hình ngôn ngữ lớn (LLM) như GPT‑4 và Claude đã đạt tới hàng trăm tỷ tham số, và các thiết kế MoE như trong Mixtral hoặc DeepSeek‑V3 giúp mở rộng quy mô mà vẫn giữ số tham số hoạt động ở mức hợp lý. Hugging Face là nền tảng lưu trữ và chia sẻ các mô hình nguồn mở, trong khi mã hóa tác động (agentic coding) mô tả khả năng của LLM tự viết, kiểm tra và cải thiện mã nguồn như một phần của quy trình phát triển phần mềm dựa trên AI.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE) Mixture of Experts in Large Language Models - arXiv.org Applying Mixture of Experts in LLM Architectures | NVIDIA ... Understanding Mixture of Experts (MoE): The Architecture ... What is Mixture of Experts (MoE)? - GeeksforGeeks Understanding Mixture of Experts (MoE) Neural Networks</a></li>
<li><a href="https://arxiv.org/html/2507.11181v2">Mixture of Experts in Large Language Models - arXiv.org</a></li>
<li><a href="https://huggingface.co/collections/deepreinforce-ai/ornith-10">Ornith-1.0 - a deepreinforce-ai Collection - Hugging Face</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#Mixture-of-Experts`, `#Hugging Face`, `#model release`, `#AI research`

---

<a id="item-7"></a>
## [OpenMontage ra mắt hệ thống sản xuất video agentic mã nguồn mở](https://github.com/calesthio/OpenMontage) ⭐️ 8.0/10

OpenMontage, một hệ thống sản xuất video agentic mã nguồn mở mới, đã được phát hành trên GitHub, cung cấp 12 pipeline, 52 công cụ và hơn 500 kỹ năng agent để biến trợ lý AI viết mã studio video đầy đủ.

ossinsight · calesthio · 26/6 04:03

**Thẻ**: `#video-production`, `#AI`, `#open-source`, `#agentic`, `#python`

---

<a id="item-8"></a>
## [Om Malik, Nhà Báo Công Nghệ Ảnh Hưởng, Tử Vong Tại Tuổi 60](https://om.co/2026/06/24/1966-2026/) ⭐️ 6.0/10

Om Malik, một nhà báo và blogger công nghệ nổi tiếng với sự bình luận trung thực và tư vấn mentor, đã chết ở tuổi 60, như được công bố trên trang web cá nhân om.co vào ngày 24 tháng 6 năm 2026. Sự mất mát của ông loại bỏ một voix tin cậy trong báo chí công nghệ, người đã hướng dẫn nhiều nhà viết và startup mới, và cái chết của ông đã khiến cộng đồng công nghệ bày tỏ lòng biết ơn sâu sắc. ông đã sáng lập GigaOm, viết cho Fast Company, Red Herring và Light Reading, là tác giả của cuốn sách Broadbandits, và được tôn vinh vì phản hồi trung thực khắc nghiệt và sẵn sàng giúp đỡ người khác mà không tìm kiếm tranh cãi.

hackernews · minimaxir · 25/6 20:33 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48678852)

**Bối cảnh**: Om Malik là một nhà báo công nghệ 베те랑, bắt đầu sự nghiệp từ đầu những năm 2000 và trở nên nổi nhờ blog và mạng lưới GigaOm. Ông đã viết cho các xuất bản như Fast Company, Red Herring và Light Reading, và là tác giả của cuốn sách Broadbandits về ngành broadband đầu tiên. Trong suốt sự nghiệp, ông được tôn trọng vì sự phân tích thẳng thắn, sự hướng dẫn cho các blogger trẻ và nỗ lực thúc đẩy lành mạnh trong Silicon Valley.

**Thảo luận cộng đồng**: Các bình luận viên bày tỏ sự sốc và buồn đau, khen ngợi sự trung thực, tư vấn mentor và tính không gây drama của Malik, vai trò làm người điều hòa và ảnh hưởng đến sự nghiệp cũng như các startup của họ.

**Thẻ**: `#obituary`, `#tech journalism`, `#blogging`, `#Silicon Valley`, `#community`

---

<a id="item-9"></a>
## [Apple bỏ M6 Pro/Max, ưu tiên M7 cho AI địa phương.](https://www.reddit.com/r/LocalLLaMA/comments/1ufhu3s/report_apple_to_skip_m6_promax_chips_fasttrack_m7/) ⭐️ 6.0/10

Một báo cáo cho rằng Apple sẽ bỏ qua các biến thể chip M6 Pro và Max, thay vào đó sẽ tăng tốc phát hành loạt M7 để tốt hơn hỗ trợ các tác vụ AI trên thiết bị. Chuyển đổi này có thể cung cấp cho nhà phát triển truy cập sớm vào phần cứng AI mạnh hơn trên Mac, tăng tốc suy luận mô hình địa phương và giảm sự phụ thuộc vào dịch vụ đám mây. Theo Macworld, các phiên bản M7 Pro và Max (mã H19S và H19C) dự kiến ra mắt cuối năm 2027, M7 Ultra (H19D) vào 2028, và sẽ có băng thông bộ nhớ vượt quá 1 TB/s nhờ quy trình 2 nm của TSMC.

reddit · r/LocalLLaMA · /u/fallingdowndizzyvr · 25/6 18:11

**Bối cảnh**: Các chip hệ thống trên một chip (SoC) M‑series của Apple cung cấp năng lực cho dòng sản phẩm Mac, mỗi thế hệ thường mang lại cải tiến về CPU, GPU và nhân thần 经. Các tác vụ AI địa phương chạy mô hình trực tiếp trên thiết bị, hưởng lợi từ băng thông bộ nhớ cao và các accelerator AI chuyên dụng. Với việc bỏ qua M6 Pro/Max và chuyển thẳng sang M7 tập trung vào AI, Apple mong muốn cung cấp hiệu suất AI trên thiết bị đáng kể hơn sớm hơn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.macworld.com/article/3177046/report-apple-to-skip-m6-pro-max-chips-fast-track-m7-for-local-ai.html">Report: Apple to skip M 6 Pro / Max chips , fast-track M7 for... | Macworld</a></li>
<li><a href="https://memeburn.com/apple-m6-chip-release/">Apple M 6 Chip : Release Date, Specs , New Products... - Memeburn</a></li>

</ul>
</details>

**Thẻ**: `#Apple Silicon`, `#M-series chips`, `#local AI`, `#hardware roadmap`, `#rumor`

---