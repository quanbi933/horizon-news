---
layout: default
title: "Horizon Summary: 2026-06-17 (ZH)"
date: 2026-06-17
lang: zh
---

> Đã chọn 7 tin quan trọng từ 17 nội dung.

---

1. [GrapheneOS đã được port sang Android 17, bản phát hành chính thức sắp tới](#item-1) ⭐️ 8.0/10
2. [Chạy mô hình địa phương hiện nay tốt hơn](#item-2) ⭐️ 7.0/10
3. [Bài viết trên Hacker News khuyên ngừng sử dụng JWT cho phiên trình duyệt.](#item-3) ⭐️ 7.0/10
4. [Coinbase ra mắt cổ phiếu mã hóa trên chuỗi trả cổ tức](#item-4) ⭐️ 7.0/10
5. [Bash /dev/tcp cho phép gửi yêu cầu HTTP mà không cần curl](#item-5) ⭐️ 6.0/10
6. [Georgi Gerganov khẳng định Qwen3.6-27B là mô hình tốt cho công việc mã hóa](#item-6) ⭐️ 6.0/10
7. [Kiểm soát xuất khẩu Fable 5 gây hại cho phòng thủ mạng Mỹ](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GrapheneOS đã được port sang Android 17, bản phát hành chính thức sắp tới](https://discuss.grapheneos.org/d/36469-grapheneos-has-been-ported-to-android-17-and-official-releases-are-coming-soon) ⭐️ 8.0/10

GrapheneOS đã được port thành công lên Android 17, và dự án thông báo rằng các bản phát hành chính thức dựa trên nền Android mới sẽ sắp ra mắt. Việc port này mở rộng các tính năng cứngened về quyền riêng tư và bảo mật của GrapheneOS lên nền Android mới nhất, cung cấp cho người dùng bảo mật hiện đại trên phần cứng mới nhất. Port này duy trì các tính năng cứngened cốt lõi của GrapheneOS như giảm thiểu lỗ hổng, sandbox ứng dụng và giảm bề mặt tấn công, đồng thời thích ứng với thay đổi API và bản vá bảo mật của Android 17.

hackernews · Cider9986 · 16/6 20:34 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48561654)

**Bối cảnh**: GrapheneOS là một hệ điều hành di động mã nguồn mở, tập trung vào quyền riêng tư, được xây dựng trên Android Open Source Project với các tính năng giảm thiểu lỗ hổng, quyền ứng dụng chặt chẽ và verified boot. Android 17 là bản cập nhật chính lớn tiếp theo của nền tảng di động của Google, dự kiến ra mắt năm 2026, mang lại các thay đổi UI do AI dẫn dắt và các bản cập nhật bảo mật mới.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://drfone.wondershare.com/android-unlock/grapheneos-phone.html">Secure Your Pixel with GrapheneOS : Full Guide And Support List</a></li>
<li><a href="https://developer.android.com/about/versions/17/get">Get Android 17 | Android Developers</a></li>
<li><a href="https://www.androidauthority.com/android-17-release-date-3639790/">Android 17 release date: The next major update is... - Android Authority</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Người dùng khen ngợi GrapheneOS về quyền riêng tư và ổn định, chỉ cho thấy một số hồi quy về tính năng sử dụng như mấtGesture di chuyển con trỏ và thay đổi phản hồi trong ứng dụng nhắn tin. Một số người báo cáo vấn đề tương thích với các ứng dụng ngân hàng và Strava, trong khi những người khác mong đợi sự hỗ trợ rộng hơn trên các thiết bị ngoài Pixel.

**Thẻ**: `#GrapheneOS`, `#Android 17`, `#privacy`, `#mobile security`, `#open-source OS`

---

<a id="item-2"></a>
## [Chạy mô hình địa phương hiện nay tốt hơn](https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/) ⭐️ 7.0/10

Bài viết trên blog cho rằng việc chạy mô hình ngôn ngữ địa phương đã trở nên thực tiễn, khi xem xét các họ mô hình khác nhau, hiệu ứng lượng tử hóa và yêu cầu phần cứng. Xu hướng này cho thấy sự quan tâm tăng vững đến việc triển khai AI riêng tư và tiết kiệm chi phí, có thể giảm sự phụ thuộc vào dịch vụ LLM dựa trên đám mây và ảnh hưởng đến chiến lược giá của các nhà cung cấp. Bài viết nhắc đến các mô hình đặc trưng như Qwen 27B và Gemma 31B, các mô hình Mixture‑of‑Experts như Gemma 26B và Qwen 35B, và chỉ ra rằng lượng tử hóa 4‑bit là phổ biến nhưng có thể làm yếu khả năng gọi công cụ, đồng thời cần đủ VRAM/RAM để hoạt động mượt mà.

hackernews · jfb · 16/6 14:36 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48555993)

**Bối cảnh**: Việc chạy các mô hình ngôn ngữ lớn ở local đòi hỏi đủ bộ nhớ GPU (VRAM) hoặc RAM hệ thống để tải trọng số mô hình, khiến phần cứng trở thành yếu tố chính. Các kỹ thuật lượng tử hóa như QLoRA và GTPQ nén kích thước mô hình bằng cách ánh xạ các trọng số độ chính xác cao sang biểu diễn độ chính xác thấp, cho phép triển khai trên phần cứng tiêu dùng. Kiến trúc Mixture‑of‑Experts (MoE) nâng cao hiệu quả bằng cách chỉ kích hoạt một phần phụ mạng expert cho mỗi đầu vào, cho phép các mô hình lớn chạy với ít tài nguyên tính toán hơn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://medium.com/@AILearningHub/mixture-of-experts-moe-5d0ab118d6c4">Mixture of Experts (MoE) in Deep Learning | by S. Moazeni... | Medium</a></li>
<li><a href="https://symbl.ai/developers/blog/a-guide-to-quantization-in-llms/">A Guide to Quantization in LLMs | Symbl.ai</a></li>
<li><a href="https://medium.com/@tahmidefaz/local-llm-101-running-llms-locally-e938685ddc5a">Local LLM 101: Running LLMs locally | by Tahmid Efaz | Medium</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những bình luận cho thấy cảm xúc hỗn hợp, khi người dùng chú ý rằng các mô hình đặc trưng như Qwen 27B vẫn chậm dù thông minh, trong khi các mô hình MoE nhanh hơn nhưng hay 犯错. Nhiều người chỉ ra rằng lượng tử hóa 4‑bit mạnh làm yếu khả năng gọi công cụ, khiến mô hình địa phương cảm thấy không đáng tin cậy cho một số quy trình. Một số người dùng nói họ sẽ thích sử dụng mô hình địa phương thay vì trả tiền cho dịch vụ đám mây, nhắc đến cả tiết kiệm chi phí và sự phiền phức vì lời nói nhiều và có thành kiến của các mô hình proprietery.

**Thẻ**: `#local LLMs`, `#model quantization`, `#Mixture of Experts`, `#AI deployment`, `#Hacker News discussion`

---

<a id="item-3"></a>
## [Bài viết trên Hacker News khuyên ngừng sử dụng JWT cho phiên trình duyệt.](https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452) ⭐️ 7.0/10

Bài viết trên Hacker News tuyên bố rằng JWT không phù hợp cho phiên người dùng dựa trên trình duyệt vì chúng không thể thu hồi dễ dàng và thường có thời gian hiệu lực quá lâu, dẫn đến một cuộc tranh luận chi tiết với 166 bình luận. Cuộc tranh luận nhấn mạnh sự đối 立 liên tục giữa cách tiếp cận token không trạng thái và lưu trữ phiên truyền thống, ảnh hưởng đến lựa chọn cơ chế xác thực của các nhà phát triển cho các ứng dụng web bảo mật. Các bình luận cho thấy JWT không thể thu hồi dễ dàng, yêu cầu thời gian sống ngắn hoặc sử dụng refresh token để giảm rủi ro, và vẫn phù hợp cho truyền thông dịch vụ‑to‑dịch vụ khi các phiên trạng thái không thực tế.

hackernews · dzonga · 16/6 16:49 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48558147)

**Bối cảnh**: JSON Web Token (JWT) là một định dạng nhỏ gọn, an toàn với URL để biểu diễn các claim giữa hai bên, thường được dùng để xác thực không trạng thái trong các ứng dụng web. Vì JWT chứa đầy đủ thông tin trong chính nó, chúng không thể bị thu hồi mà không cần máy chủ lưu trữ trạng thái, gây ra thách thức về việc hủy token. Xác thực dựa trên phiên lưu trữ trạng thái trên máy chủ, cho phép đăng xuất ngay lập tức. Nhiều nhà phát triển kết hợp JWT có thời gian sống ngắn với refresh token hoặc chọn sử dụng phiên truyền thống để cân bằng giữa bảo mật và khả năng sử dụng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://portswigger.net/web-security/jwt">JWT attacks | Web Security Academy</a></li>
<li><a href="https://javascript.plainenglish.io/auth-wars-session-vs-jwt-vs-oauth2-the-ultimate-2025-showdown-f5b08b1e9e50">Auth Wars: Session vs JWT vs OAuth 2 — The Ultimate 2025...</a></li>
<li><a href="https://www.vaadata.com/en/blog/jwt-json-web-token-vulnerabilities-common-attacks-and-security-best-practices/">JWT: Vulnerabilities, Attacks & Security Best Practices</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận chia rẽ: một số đồng ý rằng JWT gây ra vấn đề về thu hồi và thời gian hiệu lực khi dùng cho phiên trình duyệt, trong khi những người khác bảo vệ việc sử dụng JWT cho API và truyền thông dịch vụ‑to‑dịch vụ, nhấn mạnh việc sử dụng thời gian sống ngắn, refresh token và quản lý khóa thích hợp. Một số người cũng chỉ ra rằng OAuth2 vẫn là tiêu chuẩn vững chắc cho truy cập được ủy quyền, và một cách tiếp cận kết hợp—sử dụng phiên cho các trang render trên máy chủ và JWT cho API—có thể hiệu quả. Tổng thể, cuộc thảo luận nhấn mạnh rằng sự lựa chọn phụ thuộc vào mô hình đe dọa và chi tiết triển khai thay vì từ chối hoàn toàn JWT.

**Thẻ**: `#JWT`, `#authentication`, `#web security`, `#OAuth2`, `#session management`

---

<a id="item-4"></a>
## [Coinbase ra mắt cổ phiếu mã hóa trên chuỗi trả cổ tức](https://www.reddit.com/r/CryptoCurrency/comments/1u7r3de/coinbase_joins_tokenized_stock_race_with_onchain/) ⭐️ 7.0/10

Coinbase thông báo về việc ra mắt cổ phiếu mã hóa trên chuỗi trả cổ tức, tham gia vào cuộc đua cổ phiếu mã hóa. Bước đi này cho thấy một sàn giao dịch crypto lớn đang bước vào không gian chứng권 mã hóa được quy định, có thể tăng cường việc chấp nhận rộng rãi và gây ra sự kiểm tra chặt chẽ của các cơ quan quản lý. Điều này phản ánh sự quan tâm tăng cao của các tổ chức đối với thị trường cổ phiếu dựa trên blockchain. Các cổ phiếu mã hóa được phát hành trên chuỗi và cho phép người sở hữu nhận trực tiếp tiền cổ tức qua blockchain, có thể sử dụng stablecoin hoặc tiền điện tử, không cần trung gian. Không có chi tiết kỹ thuật cụ thể nào được công bố trong thông báo.

reddit · r/CryptoCurrency · /u/CrossPuffs · 16/6 21:41

**Bối cảnh**: Cổ phiếu mã hóa biểu diễn các cổ phiếu truyền thống dưới dạng mã thông số trên chuỗi khối, cho phép quyết toán gần tức thời và truy minh sở hữu trên chuỗi. Việc trả cổ tức trên chuỗi có thể được tự động hóa bằng hợp đồng thông minh hoặc cơ chế escrow, giảm sự phụ thuộc vào clearinghouse truyền thống. Đây là một phần của xu hướng rộng hơn khi các tổ chức tài chính khám phá blockchain để phát hành chứng권 và thực hiện các hành động công ty hiệu quả hơn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://chain.link/education-hub/tokenized-stocks-equities-explained">Tokenized Stocks & Equities Explained | Chainlink</a></li>
<li><a href="https://www.taurushq.com/blog/equity-tokenization-how-to-pay-dividend-on-chain-using-cmtat/">Taurus Blog - Equity Tokenization: How to Pay Dividend On-Chain Using CMTAT</a></li>
<li><a href="https://www.coindesk.com/business/2026/05/14/here-is-why-wall-street-is-racing-to-tokenize-the-entire-stock-market">Here is why Wall Street is racing to tokenize the entire stock market</a></li>

</ul>
</details>

**Thẻ**: `#Coinbase`, `#tokenized stocks`, `#blockchain`, `#dividends`, `#cryptocurrency`

---

<a id="item-5"></a>
## [Bash /dev/tcp cho phép gửi yêu cầu HTTP mà không cần curl](https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/) ⭐️ 6.0/10

Một bài viết TIL hướng dẫn cách sử dụng thiết bị /dev/tcp tích hợp trong Bash để mở socket TCP và gửi yêu cầu HTTP GET thô, qua lệnh như `exec 3<>/dev/tcp/example.com/80` và `printf` để gửi yêu cầu, sau đó `cat` để đọc phản hồi, không cần công cụ bên ngoài như curl hoặc wget. Kỹ thuật này hữu ích để gỡ lỗi dịch vụ mạng, làm việc trong các container tối thiểu, hoặc học hỏi về mạng ở mức thấp, cho thấy Bash có thể hoạt động như một client TCP đơn giản; nhưng do thiếu khả năng phân tích HTTP đúng đắn, nó không phù hợp để sử dụng trong môi trường sản xuất. /dev/tcp không phải là một file thực trên hệ thống; Bash chặn các đường dẫn dạng /dev/tcp/host/port và tạo socket TCP, yêu cầu người dùng tự định dạng các header HTTP với ký tự CRLF và tự xử lý luồng phản hồi, không hỗ trợ HTTPS, chuyển hướng hoặc đóng kết nối tự động.

hackernews · mrshu · 16/6 16:40 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48558018)

**Bối cảnh**: Bash cung cấp một thiết bị đặc biệt /dev/tcp không phải là file thực mà là một tính năng của shell cho phép mở kết nối TCP qua redirection. Khi một script tham chiếu đến /dev/tcp/host/port, Bash sẽ cố gắng tạo socket TCP tới host và port đã cho, trả về một mô tả file có thể đọc hoặc ghi. Tính năng này có sẵn trong các phiên bản Bash được biên dịch với hỗ trợ chuyển hướng mạng và thường được dùng để kiểm tra mạng nhanh hoặc tạo client đơn giản.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.reddit.com/r/bash/comments/1qa7chp/what_is_devtcp_in_linux_and_how_does_it_work_can/">What is /dev/tcp in Linux, and how does it work? Can someone explain ...</a></li>
<li><a href="https://unix.stackexchange.com/questions/525653/why-are-or-required-to-use-dev-tcp">Why are required to use /dev/tcp</a></li>
<li><a href="https://medium.com/@stefanos.kalandaridis/bash-ing-your-network-f7069ab7c5f4">Bash-ing your network. /dev/tcp is a file descriptor of bash… - Medium</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Những người bình luận nhớ lại trải nghiệm hồi tưởng khi trò chuyện thủ công với máy chủ qua telnet, khen đây là một mẹo hay và hữu ích cho gỡ lỗi hoặc môi trường container, nhưng cũng cảnh báo rằng việc tự tay tạo yêu cầu HTTP là dễ vỡ và không phù hợp để sử dụng không giám sát hoặc trong sản xuất.

**Thẻ**: `#bash`, `#networking`, `#/dev/tcp`, `#HTTP`, `#Linux`

---

<a id="item-6"></a>
## [Georgi Gerganov khẳng định Qwen3.6-27B là mô hình tốt cho công việc mã hóa](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 6.0/10

Georgi Gerganov, nhà tạo ra llama.cpp, khẳng định ông đã sử dụng Qwen3.6-27B gần như hàng ngày để thực hiện các tác vụ mã hóa trên thiết bị M2 Ultra hoặc RTX 5090 trong vòng một tháng và một nửa qua. Lời khẳng định trực tiếp của ông nhấn mạnh sự ngày càng khả thi của việc chạy các mô hình LLM mã nguồn mở mạnh mẽ ở local để phát triển phần mềm, cung cấp một tín hiệu đáng tin cậy cho các nhà phát triển đang cân nhắc sử dụng trợ lý AI local. Gerganov chạy mô hình qua pi coding agent bằng lệnh `pi -nc --offline` và một system prompt ngắn để phù hợp phong cách, chủ yếu dùng cho các tác vụ nhỏ, thường ngày tại ggml‑org.

rss · Simon Willison · 16/6 16:04

**Bối cảnh**: Qwen3.6-27B là một mô hình LLM có kiến trúc hybrid mật từ系列 Qwen của Alibaba, được thiết kế để triển khai hiệu quả ở local. Llama.cpp, được tạo ra bởi Georgi Gerganov, là một thư viện C/C++ phổ biến cho phép chạy các mô hình LLM trên phần cứng tiêu dùng mà không cần dịch vụ đám mây. Pi coding agent là một trợ lý mã hóa dựa trên terminal, nhẹ và hoạt động offline với prompts tối thiểu, phù hợp để hỗ trợ nhanh trong việc viết mã.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3.6">GitHub - QwenLM/ Qwen 3 . 6 : Qwen 3 . 6 is the large language model ...</a></li>
<li><a href="https://pi.dev/">Pi Coding Agent</a></li>
<li><a href="https://www.banandre.com/blog/qwen3-6-27b-shatters-local-llm-expectations">Qwen 3 . 6 - 27 B : The Dense Model That Just Made MoE... - Banandre</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#local AI`, `#coding assistance`, `#Qwen3`, `#Georgi Gerganov`

---

<a id="item-7"></a>
## [Kiểm soát xuất khẩu Fable 5 gây hại cho phòng thủ mạng Mỹ](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 6.0/10

Ngày 16/6/2026, Simon Willison báo cáo rằng các quy định xuất khẩu mới của Mỹ đối với mô hình Fable 5 của Anthropic được kích hoạt bởi một lời nhắc đơn giản 'fix this code', mà các nhà bảo vệ sử dụng để vá lỗi mã. Ông trích dẫn chuyên gia bảo mật Kate Moussouris, người xác nhận rằng yêu cầu này là một hành động phòng thủ hợp pháp, không phải là jailbreak. Việc hạn chế truy cập vào mô hình AI viết code hàng đầu làm giảm khả năng của các nhà bảo vệ tự động tìm, sửa và kiểm tra lỗ hổng, có thể làm suy giảm khả năng phục hồi mạng của Mỹ. Điều này minh họa cách các biện pháp kiểm soát xuất khẩu AI quá rộng có thể vô tình chặn các công cụ phòng thủ hữu ích mà lại không ngăn chặn được việc sử dụng xấu. Fable 5 là một mô hình Mythos‑class đứng đầu FrontierBench về tác vụ coding; cosiddetto jailbreak chỉ là lời nhắc 'fix this code', khiến mô hình sinh ra sửa code hợp lệ và tạo test, nhưng các cơ chế bảo mật khiến nó từ chối xem xét mã có lỗ hổng. Quy định xuất khẩu được áp dụng chỉ vài ngày sau khi Fable 5 được phát hành công khai, cho thấy chính sách có thể phản ứng nhanh với rủi ro được coi là tiềm ẩn.

rss · Simon Willison · 16/6 05:20

**Bối cảnh**: Fable 5 là mô hình AI Mythos‑class mới nhất của Anthropic, được mô tả là tiên tiến nhất về coding, reasoning và nhiều tiêu chuẩn khác, và được phát hành để sử dụng chung vào giữa năm 2026. Các biện pháp kiểm soát xuất khẩu trên mô hình AI của Mỹ là các hạn chế pháp lý ngăn chặn việc chuyển 移 phần mềm nâng cao sang các thực thể nước ngoài, thường được đưa ra bởi lý do an ninh quốc gia. Một jailbreak prompt là đầu vào được thiết kế đặc biệt để vượt qua sự căn chỉnh an toàn của mô hình; trong trường hợp này, lời nhắc vô hại 'fix this code' bị gán nhãn sai là jailbreak, cho thấy bộ lọc an toàn có thể chặn những hành động phòng thủ hữu ích.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/06/13/inside-the-whirlwind-24-hours-that-led-the-white-house-to-slap-export-controls-on-anthropic-00961519">Inside the whirlwind 24 hours that led the White House to slap export ...</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://repello.ai/blog/understanding-ai-jailbreaking-techniques-and-safeguards-against-prompt-exploits">AI Jailbreak Prompts: How They Work, Why They Work, and How to Stop Them | Repello AI</a></li>

</ul>
</details>

**Thẻ**: `#AI`, `#export controls`, `#cybersecurity`, `#LLMs`, `#policy`

---