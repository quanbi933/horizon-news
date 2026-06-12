---
layout: default
title: "Horizon Summary: 2026-06-12 (ZH)"
date: 2026-06-12
lang: zh
---

> Đã chọn 10 tin quan trọng từ 19 nội dung.

---

1. [Bài báo năm 2001 nhấn mạnh sự thiếu công nhận cho công việc phòng ngừa](#item-1) ⭐️ 8.0/10
2. [Claude Fable 5 thể hiện hành động chủ động không ngừng.](#item-2) ⭐️ 8.0/10
3. [Homebrew 6.0.0 ra mắt: Tap Trust, sandbox Linux, hỗ trợ macOS 27](#item-3) ⭐️ 8.0/10
4. [Nếu bạn đang tìm kiếm sự chú ý của con người, hãy thể hiện sự nỗ lực của con người](#item-4) ⭐️ 8.0/10
5. [Anthropic xin lỗi vì các guardrails vô hình trong Claude Fable](#item-5) ⭐️ 8.0/10
6. [Yêu cầu rút lại Luật C-22 của Canada gây tranh cãi](#item-6) ⭐️ 8.0/10
7. [Xiaomi phát hành MiMo Code, trợ lý AI mã nguồn mở cho terminal](#item-7) ⭐️ 7.0/10
8. [Zed ra mắt DeltaDB, hệ thống kiểm soát phiên bản ở mức độ thao tác](#item-8) ⭐️ 7.0/10
9. [Datasette 1.0a33 bổ sung JSON extras cho truy vấn và hàng](#item-9) ⭐️ 7.0/10
10. [Kho agent-skills của Addy Osmani đạt 85 sao trong 24 giờ](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Bài báo năm 2001 nhấn mạnh sự thiếu công nhận cho công việc phòng ngừa](https://web.mit.edu/nelsonr/www/Repenning=Sterman_CMR_su01_.pdf) ⭐️ 8.0/10

Bài báo năm 2001 của Repenning và Sterman cho rằng các tổ chức thường thưởng cho việcดับ cháy hiển nhiên sau khi xảy ra lỗi, trong khi bỏ qua công việc phòng ngừa ngăn ngừa vấn đề trước khi xảy ra. Nhận thức này giải thích tại sao công nợ kỹ thuật tích lũy và tại sao việc phản ứng sự cố được ca ngợi, ảnh hưởng đến các đội phát triển phần mềm, quản lý và bất kỳ ai thiết kế hệ thống khích lệ. Bài báo được công bố năm 2001, do Nelson Repenning và John Sterman viết, và đã được nhắc lại trong các cuộc thảo luận liên hệ công việc phòng ngừa với công nợ kỹ thuật và hành vi tổ chức.

hackernews · sam_bristow · 12/6 00:38 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48498385)

**Bối cảnh**: Trong kỹ thuật phần mềm, bảo trì phòng ngừa bao gồm các hoạt động định kỳ như xem lại mã và tái cấu trúc để giảm lỗi trong tương lai, trong khi bảo trì phản ứng (đánh cháy) xử lý các sự cố sau khi chúng xảy ra. Các tổ chức thường thiếu chỉ số để đo lường giá trị của các vấn đề đã được ngăn ngừa, dẫn đến cấu trúc phần thưởng ưu tiên việc phản ứng khẩn cấp hiển nhiên. Sự lệch này khuyến khích tích lũy công nợ kỹ thuật vì việc cứu 援 ngắn hạn được công nhận hơn là ổn định dài hạn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_maintenance">Software maintenance - Wikipedia</a></li>
<li><a href="https://www.mrpeasy.com/blog/predictive-maintenance/">Predictive Maintenance, Preventive Maintenance, or Firefighting – what’s the best?</a></li>
<li><a href="https://docs.gitscrum.com/en/best-practices/managing-technical-debt-in-agile-teams">Technical Debt Agile | Sprint Allocation & Paydown · GitScrum Docs</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận cho thấy các nhóm tạo ra khủng hoảng thường được khen ngợi vì các biện pháp sửa chữa hào hùng, trong khi các nhóm ngăn ngừa vấn đề nhận được rất weinig sự công nhận. Một số người khác chỉ ra rằng các giải pháp đơn giản, tinh tế thường bị bỏ qua để cho những công việc phức tạp, ấn tượng hơn, vàแสดง sự quan tâm đến dữ liệu về tỷ lệ CEO có nền tảng kỹ thuật. Thảo luận này củng cố主張 của bài báo, với nhiều người chia sẻ trải nghiệm cá nhân minh họa cho sự thiên vị hệ thống chống lại công việc phòng ngừa.

**Thẻ**: `#organizational behavior`, `#software engineering`, `#technical debt`, `#management`, `#systems thinking`

---

<a id="item-2"></a>
## [Claude Fable 5 thể hiện hành động chủ động không ngừng.](https://simonwillison.net/2026/Jun/11/fable-is-relentlessly-proactive/#atom-everything) ⭐️ 8.0/10

Simon Willison thấy Claude Fable 5 tự động chẩn đoán và sửa lỗi thanh cuộn ngang trong Datasette Agent bằng cách viết script Python để chụp ảnh màn hình qua API Quartz của macOS, mà không cần hướng dẫn cụ thể. Điều này cho thấy mức độ tự chủ ngày càng tăng của các trợ lý mã AI, thể hiện khả năng thực hiện các tác vụ hệ thống phức tạp, đồng thời gây ra lo ngại về tiêu thụ token, chi phí và an toàn khi các tác nhân hoạt động bên ngoài môi trường cát bãi. Fable đã chạy một lệnh Python một dòng qua `uv run --with pyobjc-framework-Quartz` để liệt kê các cửa sổ macOS, lọc những cửa sổ Safari có chuỗi 'textarea', lấy ID cửa sổ và sau đó sử dụng công cụ `screencapture` để chụp ảnh PNG của các trang HTML thử nghiệm mà nó tự tạo ra.

rss · Simon Willison · 11/6 23:35 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48498573)

**Bối cảnh**: Claude Fable 5 được ra mắt vào ngày 9 / 6 / 2026 là mô hình Fable thông minh nhất của Anthropic, được tối ưu cho công việc mã hóa và các tác nhân với khả năng suy luận nâng cao. Datasette Agent là một trợ lý AI mở rộng được xây dựng trên Datasette, cho phép người dùng truy vấn và trực quan hoá dữ liệu SQLite qua các lời nhắc ngôn ngữ tự nhiên với nhiều mô hình LLM khác nhau. Khi kết hợp, chúng cho phép các nhà phát triển 委托 việc gỡ lỗi cho một AI có thể kiểm tra mã, chạy lệnh và tương tác với hệ thống máy chủ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://ai.azure.com/catalog/models/claude-fable-5">Claude Fable 5</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận đã cảm thấy 惊叹 với khả năng tự chủ của Fable trong việc thực hiện các tác vụ hệ thống cấp thấp, nhưng cũng cảnh báo rằng quyền lực như vậy đòi hỏi phải có cát bãi bảo mật mạnh và tiềm ẩn rủi ro an toàn. Một số người chỉ ra mức tiêu thụ token và chi phí cao do sự kiên 持 không ngừng của mô hình, so sánh với các tác nhân khác cũng thể hiện hành động mạnh mẽ tương tự. Tổng thể, cuộc thảo luận nêu lên sự excitement về khả năng phát triển của các tác nhân AI, đồng thời kêu gọi thận trọng về việc sử dụng tài nguyên và bảo mật.

**Thẻ**: `#AI agents`, `#Claude Fable`, `#proactive AI`, `#coding assistants`, `#AI safety`

---

<a id="item-3"></a>
## [Homebrew 6.0.0 ra mắt: Tap Trust, sandbox Linux, hỗ trợ macOS 27](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 8.0/10

Homebrew 6.0.0 được phát hành ngày 11/6/2026, giới thiệu cơ chế bảo mật tap trust mới, API JSON nội bộ nhanh hơn và nhỏ hơn, sandbox trên Linux và hỗ trợ ban đầu cho macOS 27 (Golden Gate). Các thay đổi này nâng cao bảo mật chuỗi cung cấp bằng cách yêu cầu tin tưởng rõ ràng cho tap bên thứ ba, nâng hiệu suất nhờ API JSON gọn hơn và mở rộng khả năng sử dụng Homebrew trên macOS sắp tới và môi trường Linux được cô lập. Tính năng tap trust bắt buộc người dùng phải rõ ràng tin tưởng bất kỳ tap bên thứ ba nào trước khi mã Ruby không được sandbox chạy, trong khi tap chính thức vẫn được tin tưởng mặc định; API JSON mới giảm lượng dữ liệu cần thiết để tải manifest của bottle, và sandbox trên Linux sử dụng không gian tên người dùng để cô lập việc thực thi công thức.

hackernews · mikemcquaid · 11/6 13:24 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48490024)

**Bối cảnh**: Homebrew là một trình quản lý gói miễn phí và mã nguồn mở giúp cài đặt phần mềm trên macOS và Linux dễ dàng hơn bằng cách sử dụng các công thức được lưu trữ trong các kho gọi là taps. Cơ chế tap trust được bổ sung để nâng cao bảo mật chuỗi cung cấp bằng cách giới hạn việc thực thi mã của tap bên thứ ba trừ khi được Clearly tin tưởng. API JSON nội bộ cung cấp một cách nhẹ để Homebrew lấy metadata của bottle, và việc thiết kế lại trong phiên bản 6.0 làm cho nó nhanh hơn và nhỏ hơn. Sandbox trên Linux sử dụng cách cô lập giống container để ngăn công thức ảnh hưởng đến hệ thống máy chủ, trong khi hỗ trợ ban đầu cho macOS 27 chuẩn bị Homebrew cho hệ điều hành sắp tới của Apple.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://docs.brew.sh/Tap-Trust">Homebrew Documentation: Tap Trust</a></li>
<li><a href="https://en.wikipedia.org/wiki/MacOS_27_Golden_Gate">MacOS 27 Golden Gate</a></li>
<li><a href="https://github.com/Homebrew/brew/issues/19204">Improve JSON API for Install Performance Improvements #19204</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận khen ngộ sự tận huyết của người duy trì lâu năm, lưu ý về môi trường phát triển thay thế như mise giúp giảm sự phụ thuộc vào Homebrew, nhấn mạnh việc sử dụng Homebrew trong các bản phân phối Linux không thể thay đổi như Bazzite của Universal Blue, so sánh có lợi hơn Nix về hỗ trợ macOS và trải nghiệm người dùng, và kêu gọi tài trợ để duy trì dự án chạy bởi tình nguyện viên.

**Thẻ**: `#Homebrew`, `#package manager`, `#macOS`, `#Linux`, `#release`

---

<a id="item-4"></a>
## [Nếu bạn đang tìm kiếm sự chú ý của con người, hãy thể hiện sự nỗ lực của con người](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

Bài viết cho rằng để nhận được sự chú ý của con người (ví dụ: trong quá trình review mã), người đóng góp phải thể hiện sự nỗ lực thực sự của con người, thay vì gửi các bài viết do AI tạo ra với mức độ nỗ lực thấp, gây gánh nặng cho người review.

hackernews · jjfoooo4 · 11/6 23:01 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48497609)

**Thẻ**: `#AI-assisted development`, `#code review`, `#software engineering`, `#team dynamics`, `#human-AI collaboration`

---

<a id="item-5"></a>
## [Anthropic xin lỗi vì các guardrails vô hình trong Claude Fable](https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail) ⭐️ 8.0/10

Anthropic đã xin lỗi vì đã triển khai các guardrails vô hình trong mô hình Claude Fable 5, chúng thầm lặng thay đổi prompt của người dùng mà không công khai, gây ra lo ngại về sự trong suốt và sự căn chỉnh AI. Sự việc này nhấn mạnh sự đối lập giữa các biện pháp an toàn AI và niềm tin của người dùng, cho thấy những can thiệp ẩn có thể làm suy giảm độ tin cậy và sự mở trong các hệ thống AI. Các guardrails vô hình được triển khai như một distillation guardrail để ngăn chặn việc distillation mô hình, chúng thay đổi prompt theo thời gian thực mà không người dùng biết; Anthropic nói rằng sẽ làm cho các guardrails này trở nên rõ ràng như các biện pháp an toàn khác.

hackernews · rarisma · 11/6 12:05 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48489229)

**Bối cảnh**: Claude Fable 5 là mô hình mạnh mẽ nhất được phát hành rộng rãi của Anthropic, được thiết kế cho các tác vụ suy luận đòi hỏi cao và tác động dài hạn. Guardrails là cơ chế an toàn hạn chế đầu ra của mô hình để ngăn chặn hành vi có hại hoặc không mong muốn; chúng có thể là可见 (rõ ràng trong system prompt) hoặc vô hình (được nhúng trong mô hình). Anthropic đã sử dụng guardrails vô hình distillation để cụ thể ngăn chặn việc distillation mô hình—a kỹ thuật sử dụng đầu ra của mô hình lớn để huấn luyện một mô hình nhỏ cạnh tranh—cùng với mục tiêu đưa mô hình ra thị trường nhanh chóng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail">Anthropic apologizes for invisible Claude Fable guardrails</a></li>
<li><a href="http://anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 - Anthropic</a></li>
<li><a href="https://radarkilat.com/en/article/claude-fable-and-the-invisible-distillation-guardrail-dilemma-in-modern-ai-design">Claude Fable: Invisible Guardrails and AI Transparency</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận viên bày tỏ sự không tin, so sánh việc thay đổi prompt ẩn với Excel tự động điều chỉnh công thức trong nền, và phê bình cách tiếp cận cha mẹ của Anthropic. Một số người thừa nhận lời xin lỗi nhưng cảnh báo rằng các guardrails vô hình có thể được giữ lại một cách bí mật, làm suy giảm niềm tin vào dịch vụ.

**Thẻ**: `#AI safety`, `#Anthropic`, `#Claude`, `#guardrails`, `#transparency`

---

<a id="item-6"></a>
## [Yêu cầu rút lại Luật C-22 của Canada gây tranh cãi](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 8.0/10

Một petición trên trang web của Thượng viện Canada yêu cầu rút lại Luật C-22, một luật an toàn mạng được đề xuất sẽ yêu cầu các nhà cung cấp viễn thông và nền tảng số lưu trữ siêu dữ liệu lên đến một năm và có thể ảnh hưởng đến tiêu chuẩn mã hoá. Yêu cầu này đã được chia sẻ trên Hacker News, gây ra cuộc tranh luận về tác động đến quyền riêng tư và tiềm 在对加拿大科技行业的影响。 Luật C-22 đã gặp phản đối từ các công nghệ lớn như Apple, Google và Signal, họ cảnh báo luật này có thể làm suy yếu mã hoá và làm giảm quyền riêng tư của người dùng; kết quả của nó có thể định hình khả năng cạnh tranh của ngành công nghệ Canada và ảnh hưởng đến các cuộc tranh luận toàn cầu về truy cập hợp pháp và an toàn mạng. Yêu cầu này phản ánh lo ngại ngày càng tăng rằng luật có thể đẩy đổi mới và đầu tư sang Mỹ. Luật C-22 sẽ bắt buộc các nhà cung cấp viễn thông và nền tảng số phải lưu trữ siêu dữ liệu của người dùng lên đến 12 tháng và trao cho các cơ quan quyền lực mở rộng khả năng intercept, gây ra lo ngại về quét phía client và sự suy giảm của mã hoá端到端. Những người bình luận cũng lưu ý về luật C-34 liên quan, sẽ làm giảm thêm mức độ bảo vệ quyền riêng tư.

hackernews · hmokiguess · 11/6 15:37 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48491830)

**Bối cảnh**: Luật C-22 được 提出 bởi Chính phủ Liberal của Thủ tướng Mark Carney, được trình bày là biện pháp an toàn mạng nhằm chống lại nội dung có hại nhưng bao gồm các quy định về lưu trữ siêu dữ liệu bắt buộc và mở rộng quyền truy cập hợp pháp. Các công nghệ lớn và người bảo vệ quyền riêng tư đã cảnh báo rằng các biện pháp này có thể làm suy yếu mã hoá và tạo ra rủi ro giám sát. Luật hiện đang được xem xét theo từng điều trong Ủy viên An ninh và Phụ cấp khẩn cấp (SECU) của Thượng viện, dự kiến sẽ có sự bỏ phiếu sớm.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://refdesk.ca/blog/canada-bill-c22-lawful-access-encryption-metadata-may-17-2026-users-businesses-privacy-guide">Bill C-22 Lawful Access: U.S. Tech Giants and Congress Push Back as ...</a></li>
<li><a href="https://www.cbc.ca/news/politics/bill-c-22-encryption-cybersecurity-9.7213776">Liberals to amend police data interception bill following searing ...</a></li>
<li><a href="https://www.wionews.com/world/what-is-canada-s-online-safety-bill-why-tech-giants-like-apple-google-oppose-it-what-it-means-for-user-privacy-wion-decodes-1779886628323">What is Canada's online safety bill? Why tech giants like ... - WION</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những người bình luận biểu hiện nghi ngờ rằng petición sẽ không thay đổi số phận của luật nhưng nhấn mạnh tầm quan trọng của việc tạo ra tiếng ồn để nâng cao nhận thức. Một số người lưu ý về cuộc họp sắp tới của Ủy viên SECU và cung cấp liên kết đến luồng trực tiếp ParlVu, trong khi những người khác đặt câu hỏi về tính hợp pháp của trang petición. Tổng thể, cảm xúc tập trung vào lo ngại rằng luật có thể gây hại cho ngành công nghệ Canada và đẩy giá trị sang các công ty Mỹ.

**Thẻ**: `#privacy`, `#legislation`, `#Canada`, `#tech policy`, `#online safety`

---

<a id="item-7"></a>
## [Xiaomi phát hành MiMo Code, trợ lý AI mã nguồn mở cho terminal](https://mimo.xiaomi.com/mimocode) ⭐️ 7.0/10

Xiaomi đã phát hành MiMo Code như một trợ lý AI mã nguồn mở, chạy trên terminal, được fork từ OpenCode, có bộ nhớ bền bỉ và khả năng tự động. Việc phát hành này giảm chi phí chuyển đổi cho nhà phát triển bằng cách cung cấp một lựa chọn mã nguồn mở, minh bạch thay cho các công cụ AI đóng, khuyến khích cải tiến do cộng đồng dẫn dắt và thúc đẩy việc sử dụng rộng rãi của lập trình hỗ trợ bởi AI. MiMo Code giữ lại các tính năng lõi của OpenCode—nhiều nhà cung cấp LLM, giao diện TUI, hỗ trợ LSP/MCP và hệ thống plugin— đồng thời bổ sung bộ nhớ bền bỉ, quản lý bối cảnh thông minh, điều phối subagent, vòng lặp tự động hướng mục tiêu, quy trình làm việc có thể kết hợp và tự cải thiện qua cơ chế dream/distill.

hackernews · apeters · 11/6 14:27 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48490826)

**Bối cảnh**: Các trợ lý AI mã nguồn chạy trong terminal cho phép nhà phát triển tương tác với các mô hình LLM qua giao diện dòng lệnh để chỉnh sửa mã, chạy lệnh và quản lý phiên bản mà không cần rời khỏi terminal. Các dự án như Aider, Goose (của Block) và Snowflake CoCo là ví dụ về cách tiếp cận này, cung cấp tính năng lập trình song song, tích hợp với stack dữ liệu và công cụ mở rộng. OpenCode là một harness mã nguồn mở cung cấp nền tảng mô-đun cho các trợ lý như vậy, hỗ trợ nhiều nhà cung cấp LLM, giao thức máy chủ ngôn ngữ và hệ thống plugin. MiMo Code dựa trên nền tảng này bằng cách thêm bộ nhớ bền bỉ và khả năng tự động để cho phép nhận thức dự án dài hạn và cải thiện tự định hướng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.reddit.com/r/vibecoding/comments/1r2gp17/terminalbased_coding_assistant_recommendations/">Terminal-based coding assistant recommendations? : r/vibecoding</a></li>
<li><a href="https://aider.chat/">Aider - AI Pair Programming in Your Terminal</a></li>
<li><a href="https://www.snowflake.com/en/product/snowflake-coco/">Snowflake CoCo: Snowflake-Native AI Coding Agent for Data</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận chúc mừng việc Xiaomi phát hành mã nguồn mở MiMo Code, cho rằng điều này giảm thiểu sự phụ thuộc vào nhà cung cấp và tăng tính minh bạch, trong khi một số người chỉ责 xu hướng đóng của các công cụ như Claude Code và Gemini CLI bị ngừng phát triển. Một số người dùng cũng nhấn mạnh tính kế thừa từ OpenCode và các tính năng mới như bộ nhớ bền bỉ và vòng lặp tự động, đồng thời khen ngợi sự tiến bộ nhanh chóng của Xiaomi trong phát triển mô hình AI và chính sách giá cả.

**Thẻ**: `#AI coding assistant`, `#open source`, `#Xiaomi`, `#developer tools`, `#LLM`

---

<a id="item-8"></a>
## [Zed ra mắt DeltaDB, hệ thống kiểm soát phiên bản ở mức độ thao tác](https://zed.dev/blog/introducing-deltadb) ⭐️ 7.0/10

Zed đã công bố DeltaDB, một hệ thống ghi lại mọi thao tác chỉnh sửa giữa các commit Git để cung cấp lịch sử thay đổi mã nguồn chi tiết và mịn. DeltaDB cho phép nhà phát triển xem lại và hiểu chính xác chuỗi các thay đổi trong quá trình phát triển, từ đó cải thiện việc gỡ lỗi,審查 mã và hợp tác với các tác nhân AI. DeltaDB hoạt động như một lớp kiểm soát phiên bản dựa trên thao tác, hoạt động song song với Git, lưu trữ mỗi chỉnh sửa dưới dạng delta thay vì ảnh chụp nhanh, và tích hợp với trình soạn thảo Zed để bảo tồn thông tin cho con người và AI.

hackernews · jeremy_k · 11/6 16:28 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48492533)

**Bối cảnh**: Git là một hệ thống kiểm soát phiên bản phân tán ghi lại trạng thái dự án dưới dạng ảnh chụp nhanh tại mỗi commit, khiến việc xem các thay đổi trung gian trở nên khó khăn. Theo dõi thao tác mịn màng nhằm ghi lại mọi chỉnh sửa, chẳng hạn như việc chèn hoặc xóa ký tự, giữa các ảnh chụp này. Công cụ như DeltaDB mở rộng kiểm soát phiên bản đến mức độ thao tác, cung cấp lịch sử chi tiết về các hành động của nhà phát triển. Cách tiếp cận này có thể hỗ trợ hợp tác phong phú hơn và phát triển được hỗ trợ bởi AI bằng cách lưu giữ toàn bộ luồng chỉnh sửa.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor)</a></li>
<li><a href="https://news.ycombinator.com/item?id=48492533">Software is made between commits | Hacker News</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0164121220300522">On tracking Java methods with Git mechanisms - ScienceDirect.com</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận chia rẽ: một số người đánh giá cao tiềm năng của lịch sử chi tiết và khả năng 審查 mã tốt hơn, trong khi những người khác cho rằng các chỉnh sửa trung gian là tiếng ồn và họ thích giữ chỉ những commit có ý nghĩa. Đã được nêu ra những lo ngại về quyền riêng tư, cảm giác bị giám sát liên tục, và niềm tin rằng Git đã xử lý tốt các commit tự động thường xuyên. Tổng thể, cuộc thảo luận cho thấy sự hoài nghi về tính hữu ích của việc theo dõi ở mức độ thao tác bên cạnh các thực hành Git hiện có.

**Thẻ**: `#software development`, `#version control`, `#DeltaDB`, `#Git`, `#developer tools`

---

<a id="item-9"></a>
## [Datasette 1.0a33 bổ sung JSON extras cho truy vấn và hàng](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 ra mắt tham số truy vấn `_extra=` trong API JSON, cho phép người dùng yêu cầu siêu dữ liệu bổ sung như tên cột, kiểu dữ liệu và số lượng hàng cho cả truy vấn và hàng, mở rộng mẫu trước đây chỉ có sẵn cho bảng. Cải thiện này làm cho API của Datasette trở nên linh hoạt và tự mô tả hơn, giảm nhu cầu gọi tài liệu riêng và cho phép công cụ phong phú hơn, đưa dự án gần hơn đến bản phát hành ổn định 1.0. Tính năng này hoạt động với cả endpoint bảng và truy vấn SQL tùy chỉnh, được ghi lại đầy đủ trong hướng dẫn API JSON, và đã được thể hiện qua một trình khám phá extras tùy chỉnh được xây dựng bằng Claude Fable 5 và GPT‑5.5 xhigh.

rss · Simon Willison · 11/6 15:26

**Bối cảnh**: Datasette là công cụ mã nguồn mở để khám phá, trực quan hóa và xuất bản dữ liệu dưới dạng API JSON chỉ đọc. Mẫu `_extra=` cho phép khách hàng yêu cầu siêu dữ liệu bổ sung bên cạnh dữ liệu chính, một khả năng trước đây chỉ giới hạn ở phản hồi bảng. Khi mở rộng mẫu này cho truy vấn và hàng, Datasette 1.0a33 đưa dự án hướng tới sự ổn định và đầy đủ mong đợi cho phiên bản 1.0.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="http://anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 - Anthropic</a></li>

</ul>
</details>

**Thẻ**: `#datasette`, `#release`, `#API`, `#JSON`, `#open-source`

---

<a id="item-10"></a>
## [Kho agent-skills của Addy Osmani đạt 85 sao trong 24 giờ](https://github.com/addyosmani/agent-skills) ⭐️ 7.0/10

Kho GitHub addyosmani/agent-skills đã đạt 85 sao trong 24 giờ qua, cung cấp các kỹ năng engineering sản xuất cho các agent mã hóa AI. Sự tăng trưởng nhanh chóng cho thấy sự quan tâm mạnh mẽ của nhà phát triển đối với bộ kỹ năng sẵn sàng dùng cho mã hóa hỗ trợ bởi AI, có thể tăng tốc việc áp dụng agent mã hóa AI trong môi trường sản xuất. Kho này được viết chủ yếu bằng Shell, đã nhận được 3 fork và 2 push gần đây, và cung cấp các kỹ năng engineering sản xuất nhằm cải thiện hiệu suất của agent mã hóa AI.

ossinsight · addyosmani · 12/6 04:20

**Thẻ**: `#AI`, `#coding agents`, `#developer tools`, `#open-source`, `#GitHub`

---