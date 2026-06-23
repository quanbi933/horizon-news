---
layout: default
title: "Horizon Summary: 2026-06-23 (ZH)"
date: 2026-06-23
lang: zh
---

> Đã chọn 4 tin quan trọng từ 10 nội dung.

---

1. [Prompt Injection dưới dạng nhầm lẫn vai trò](#item-1) ⭐️ 8.0/10
2. [Chuyển đổi mô hình inpainting ảnh Moebius 0.2B để chạy trên trình duyệt bằng Claude Code](#item-2) ⭐️ 8.0/10
3. [Steam Machine ra mắt hôm nay với hệ thống đặt chéo để giảm bot](#item-3) ⭐️ 7.0/10
4. [Thảo luận trên Hacker News về phần cứng cần chạy GLM-5.2 tại địa phương](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Prompt Injection dưới dạng nhầm lẫn vai trò](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Simon Willison tóm tắt một bài báo cho thấy mô hình ngôn ngữ nhầm lẫn văn bản hệ thống đặc quyền với đầu vào người dùng dựa trên phong cách, cho phép thực hiện các cuộc tấn công jailbreak qua prompt injection.

rss · Simon Willison · 22/6 23:59

**Thẻ**: `#LLM security`, `#prompt injection`, `#AI safety`, `#role confusion`, `#research summary`

---

<a id="item-2"></a>
## [Chuyển đổi mô hình inpainting ảnh Moebius 0.2B để chạy trên trình duyệt bằng Claude Code](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison đã port mô hình inpainting ảnh Moebius 0.2B sang WebGPU, cung cấp một demo tương tác để chỉnh sửa ảnh ở phía client.

rss · Simon Willison · 22/6 23:43

**Thẻ**: `#image inpainting`, `#WebGPU`, `#browser ML`, `#model porting`, `#Simon Willison`

---

<a id="item-3"></a>
## [Steam Machine ra mắt hôm nay với hệ thống đặt chéo để giảm bot](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 7.0/10

Steam Machine của Valve chính thức ra mắt hôm nay như một sản phẩm phần cứng PC chơi game mở, đi kèm với hệ thống đặt chéo nhằm giảm thiểu việc bot thực hiện mua bán. Việc ra mắt này nhấn mạnh cam kết của Valve đối với phần cứng mở, cho phép người dùng cài đặt bất kỳ hệ điều hành hoặc phần mềm nào, trong khi hệ thống đặt chéo nhằm làm cho phần cứng PC chơi game có nhu cầu cao trở nên dễ tiếp cận hơn với người dùng thường. Mẫu cơ bản bắt đầu từ 1.049 USD, việc đặt cọc mở từ ngày 22 đến 25 tháng 6 năm 2026, sử dụng hàng đợi ngẫu nhiên để ngăn chặn người mua lại, và phần cứng được bán như một PC mở có thể chạy Windows, Linux hoặc hệ điều hành khác.

hackernews · theschwa · 22/6 17:09 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48632884)

**Bối cảnh**: Valve trước đây đã đưa ra khái niệm Steam Machine để mang trò chơi PC lên phòng khách, ban đầu kết hợp với SteamOS và các nhà sản xuất bên thứ ba. Khác với các console truyền thống, Steam Machine được bán như một PC mở, cho phép người dùng cài đặt bất kỳ hệ điều hành hoặc phần mềm nào. Hệ thống đặt chéo ngẫu nhiên được đưa ra để chống lại hiện tượng mua lại do bot gây ra trong các ra mắt phần cứng có số lượng hạn chế trước đây.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.tomshardware.com/video-games/console-gaming/valve-opens-steam-machine-reservations-details-usd1-049-starting-price-randomized-queue-to-stop-scalpers-and-limited-inventory">Valve opens Steam Machine reservations — details $1,049 starting price, randomized queue to stop scalpers, and limited inventory | Tom's Hardware</a></li>
<li><a href="https://www.theverge.com/games/952191/valve-steam-machine-reservation-preorder-process">Here’s how you can reserve a Steam Machine | The Verge</a></li>
<li><a href="https://www.pcgamer.com/hardware/gaming-pcs/steam-machine-review-2026/">Steam Machine review | PC Gamer</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều bình luận elogi hệ thống đặt chéo vì giảm lợi thế của bot và đánh giá cao tính mở của phần cứng, cho phép họ cài đặt hệ điều hành riêng. Một số người thảo luận về giá và thông số kỹ thuật, trong khi những người khác nhấn mạnh video chơi game thực tế cho thấy mọi người chơi Cuphead. Tổng thể, cảm xúc là tích cực, có sự entusiasmo nhưng cũng có lo ngại về giá và khả năng có hàng.

**Thẻ**: `#Steam Machine`, `#Valve`, `#gaming hardware`, `#PC gaming`, `#open hardware`

---

<a id="item-4"></a>
## [Thảo luận trên Hacker News về phần cứng cần chạy GLM-5.2 tại địa phương](https://unsloth.ai/docs/models/glm-5.2) ⭐️ 7.0/10

Luồng thảo luận trên Hacker News chia sẻ trải nghiệm của người dùng khi chạy GLM-5.2 tại địa phương, mô tả các cấu hình phần cứng như 512 GB RAM cùng hai GPU RTX 3090 để chạy quantization Q4_K_XL đạt khoảng 6.000 token/giây. Những bình luận khác cho biết việc có 192 GB RAM cộng với một RTX 3090 có thể chạy gần đầy đủ mô hình, nhưng để offload MoE hoàn toàn cần 256 GB RAM và 24 GB VRAM. Các cuộc thảo luận này nhấn mạnh sự quan tâm ngày càng tăng về việc chạy các mô hình LLM nguồn mở lớn ở local, hiện ra những rào cản phần cứng và các trade‑off về hiệu năng mà các nhà phát triển muốn triển khai không dùng API phải đối mặt. Việc hiểu những yêu cầu này giúp cộng đồng lập kế hoạch ngân sách và dự đoán những cải tiến phần cứng trong tương lai có thể làm cho việc truy cập các mô hình như GLM-5.2 trở nên dân dụng hơn. Các cấu hình cụ thể được báo cáo bao gồm: quantization Q4_K_XL trên 512 GB RAM + 2× RTX 3090 cho khoảng 6.000 token/giây, khi sử dụng RAM DDR4 nhanh hơn và CPU EPYC có nhiều nhân hơn thì tốc độ có thể tăng lên khoảng 9.000–11.000 token/giây; cấu hình 192 GB RAM + RTX 3090 có thể chạy gần đầy đủ mô hình nhưng cần 256 GB RAM để offload MoE; việc xử lý prompt sẽ chậm đáng kể nếu không offload hoàn toàn lên GPU, khiến mô hình cảm thấy chậm chạp trên các hệ thống chỉ dùng CPU.

hackernews · TechTechTech · 22/6 21:21 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48636377)

**Bối cảnh**: GLM-5.2 là mô hình LLM nguồn mở flagship mới nhất của ZAI, được tối ưu cho việc viết mã và các nhiệm vụ dài hạn với bối cảnh 1 triệu token và giấy phép MIT. Nó vượt qua tiền nhiệm GLM-5.1 trên các tiêu chuẩn coding như Terminal‑Bench và SWE‑bench. Để chạy các mô hình lớn như vậy tại local, các nhà thực hành thường sử dụng kỹ thuật quantization (víeu quantization (ví dụ Q4_K_XL 4‑bit) giúp giảm kích thước mô hình lên tới 75 % trong khi vẫn giữ được hiệu năng, cho phép suy luận trên phần cứng tiêu dùng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 | OpenLM.ai</a></li>
<li><a href="https://github.com/zai-org/GLM-5">GLM-5.2 & GLM-5.1 & GLM-5 - GitHub</a></li>
<li><a href="https://localllm.in/blog/quantization-explained">The Complete Guide to LLM Quantization - localllm.in</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận bày tỏ sự 흥분을 khi có thể chạy mô hình này tại nhà, nhưng nhiều người cũng tiếc rằng chi phí phần cứng cần thiết rất cao và hiệu năng của các cấu hình pre‑budget rất chậm. Một số người mong chờ các máy tính AI để bàn tới với chip GB10 và các giải pháp VRAM được cụm tập để giảm thiểu rào cản, trong khi những người khác cho rằng quantization và quy trình làm việc kết hợp CPU‑GPU hiện là duy nhất khả thi để thử nghiệm mô hình tại địa phương.

**Thẻ**: `#LLM`, `#local inference`, `#GLM-5.2`, `#hardware requirements`, `#quantization`

---