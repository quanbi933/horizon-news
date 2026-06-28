---
layout: default
title: "Horizon Summary: 2026-06-28 (ZH)"
date: 2026-06-28
lang: zh
---

> Đã chọn 4 tin quan trọng từ 8 nội dung.

---

1. [OpenRA: Máy moteurs RTS mã nguồn mở tái hiện trò chơi Westwood](#item-1) ⭐️ 8.0/10
2. [OpenMontage: framework agentic video mã nguồn mở 500+ kỹ năng](#item-2) ⭐️ 8.0/10
3. [Chạy GLM5.2 trên phần cứng dưới 2500 USD bằng GPU P40 đã dùng](#item-3) ⭐️ 6.0/10
4. [Máy chủ LLM gia đình với bốn GPU RTX 4090 mod trên cổng sấy](#item-4) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenRA: Máy moteurs RTS mã nguồn mở tái hiện trò chơi Westwood](https://www.openra.net/) ⭐️ 8.0/10

Vào ngày 30 tháng 3 năm 2025, OpenRA đã phát hành bản cập nhật cho engine dựa trên C# nhằm cải thiện cân bằng, thêm tính năng mới và hỗ trợ các nền tảng hiện đại, đồng thời giữ nguyên gameplay clássic của Red Alert, Command & Conquer và Dune 2000. OpenRA cho phép bảo tồn và chơi được các trò chơi RTS quan trọng trên phần cứng hiện đại, thúc đẩy cách tiếp cận do cộng đồng dẫn đầu trong việc bảo존 trò chơi. Nó cũng minh họa cách các dự án mã nguồn mở có thể duy trì phần mềm cũ mà không cần sự hỗ trợ của nhà xuất bản gốc. Engine được viết bằng C# sử dụng SDL và OpenGL, chạy trên Windows, Linux, *BSD và macOS, và được phát hành dưới giấy phép GPLv3. Nó cung cấp API Lua, SDK mod và hỗ trợ quy tắc tùy chỉnh qua các file YAML.

hackernews · tosh · 27/6 12:10 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48697560)

**Bối cảnh**: Trò chơi chiến lược thời gian thực (RTS) yêu cầu người chơi quản lý tài nguyên và đơn vị liên tục trong khi đối đầu với đối thủ. Các tiêu đề Westwood cổ điển như Command & Conquer: Red Alert đã xác định thể loại này vào những năm 1990 nhưng không còn được hỗ trợ chính thức trên hệ điều hành hiện đại. Các dự án mã nguồn mở như OpenRA tái tạo lại các trò chơi này từ đầu, cho phép chúng chạy trên phần cứng hiện đại và bảo tồn di sản văn hóa của chúng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://github.com/OpenRA/OpenRA">GitHub - OpenRA/OpenRA: Open Source real-time strategy game ... OpenRA - Classic strategy games rebuilt for the modern era Releases · OpenRA/OpenRA - GitHub OpenRA in 2026: How Open-Source Engine Preserves Classic RTS ... OpenRA download | SourceForge.net</a></li>
<li><a href="https://www.openra.net/">OpenRA - Classic strategy games rebuilt for the modern era</a></li>
<li><a href="https://en.m.wikipedia.org/wiki/Video_game_preservation">Video game preservation - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Nhiều người bình luận đã khen OpenRA vì đã cải thiện cân bằng và thêm tính năng khiến các trò chơi RTS cổ điển trở nên thú vị hơn trên hệ thống hiện đại. Một số người dùng nhớ về trò chơi gốc và chỉ ra các cải tiến cụ thể như khoảng cách bắn của pháo tăng. Ngoài ra, có người cảm ơn EA vì cho phép dự án này tồn tại và kêu gọi nhiều nhà xuất bản hơn nên phát hành mã nguồn của các trò chơi cũ.

**Thẻ**: `#open-source`, `#RTS`, `#game preservation`, `#retro gaming`, `#community`

---

<a id="item-2"></a>
## [OpenMontage: framework agentic video mã nguồn mở 500+ kỹ năng](https://github.com/calesthio/OpenMontage) ⭐️ 8.0/10

Trong 24 giờ qua, kho lưu trữ calesthio/OpenMontage đã tăng 85 sao, giới thiệu một framework Python mã nguồn mở cho phép các tác nhân AI tự động hoá sản xuất video bằng hơn 500 kỹ năng trên 12 đường ống. Sự tăng trưởng nhanh này cho thấy sự quan tâm mạnh mẽ của cộng đồng đối với AI agentic trong truyền thông, và cách tiếp cận end‑to‑end của OpenMontage có thể làm dân chủ hoá sản xuất video bằng cách cho phép người không chuyên tạo ra video chất lượng chuyên nghiệp qua lời nhắc ngôn ngữ tự nhiên. Framework bao gồm 12 đường ống sản xuất, 52 công cụ chuyên dụng cho xử lý video/ audio/ hình ảnh và hơn 500 kỹ năng tác nhân bao gồm viết, thiết kế, tổng hợp âm thanh, chỉnh sửa và kiểm soát chất lượng, tất cả được điều phối qua hướng dẫn ngôn ngữ tự nhiên bằng Python.

ossinsight · calesthio · 28/6 04:10

**Bối cảnh**: AI agentic đề cập đến các hệ thống trong đó các tác nhân AI tự chủ chọn và thực hiện các công cụ phù hợp để hoàn thành các nhiệm vụ phức tạp, thay vì tuân theo một kịch bản cố định. Sản xuất video truyền thống đòi hỏi phải điều khiển nhiều ứng dụng riêng biệt cho việc viết kịch bản, tạo tài sản, tổng hợp giọng nói, chỉnh sửa và render. OpenMontage tích hợp các khả năng này vào một framework thống nhất, cho phép một tác nhân AI quản lý toàn bộ quy trình từ kịch bản đến video cuối cùng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://pyshine.com/OpenMontage-Agentic-Video-Production-System/">OpenMontage - Agentic Video Production System with 12 Pipelines and 500+ Skills | PyShine</a></li>
<li><a href="https://github.com/calesthio/OpenMontage">GitHub - calesthio/OpenMontage: World's first open-source ...</a></li>

</ul>
</details>

**Thẻ**: `#video-production`, `#AI-agents`, `#open-source`, `#Python`, `#multimedia`

---

<a id="item-3"></a>
## [Chạy GLM5.2 trên phần cứng dưới 2500 USD bằng GPU P40 đã dùng](https://www.reddit.com/r/LocalLLaMA/comments/1uh8r1j/running_glm52_on_budget_hardware_2500/) ⭐️ 6.0/10

Bài viết trên Reddit cung cấp hướng dẫn chi tiết để chạy mô hình ngôn ngữ lớn GLM‑5.2 trên một cấu hình giá dưới 2.500 USD, sử dụng hai GPU Tesla P40 đã dùng, bo mạch chủ/CPU giá rẻ và 512 GB RAM DDR4. Điều này cho thấy các mô hình mã nguồn mở hiện đại có thể được chạy tại local mà không cần dịch vụ đám mây đắt tiền, giảm thiểu rào cản cho người hobby, sinh viên và nhóm nhỏ để thử nghiệm các mô hình LLMs có bối cảnh dài. Chi phí thành phần chính khoảng 1.920 USD, cộng thêm 580 USD cho PSU, lưu trữ và làm mát để đạt ngưỡng 2.500 USD; người dùng lưu ý rằng hiệu suất sẽ chậm nhưng đủ để thực hiện các tác vụ lập kế hoạch và gỡ lỗi.

reddit · r/LocalLLaMA · /u/segmond · 27/6 17:33

**Bối cảnh**: GLM‑5.2 là một mô hình AI mã nguồn mở của Trung Quốc được thiết kế cho các nhiệm vụ mã hóa dài, có bối cảnh 1 triệu token và đã được huấn luyện đặc biệt cho các tác nhân mã hóa. GPU Nvidia Tesla P40 là một card dựa trên kiến trúc Pascal ra mắt năm 2016, có 24 GB VRAM và hiệu suất suy luận INT8 lên tới 47 TOPS, phù hợp với các workloads suy luận học sâu. Các công cụ như llama.cpp cho phép chạy các mô hình LLMs đã được lượng tử hoá trên phần cứng này bằng cách giảm kích thước mô hình mà vẫn giữ được khả năng sử dụng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.businessinsider.com/what-is-glm-5-2-chinese-ai-coding-model-2026-6">What is GLM-5.2? Another open-source Chinese AI model has ...</a></li>
<li><a href="https://www.techpowerup.com/gpu-specs/tesla-p40.c2878">NVIDIA Tesla P40 Specs | TechPowerUp GPU Database</a></li>
<li><a href="https://medium.com/red-buffer/ultimate-guide-to-running-quantized-llms-on-cpu-with-llama-cpp-1a26c34bb6dd">Ultimate Guide to Running Quantized LLMs on CPU with LLaMA.cpp | by Mubashir Iqbal | Red Buffer | Medium</a></li>

</ul>
</details>

**Thẻ**: `#GLM5.2`, `#budget hardware`, `#LLM inference`, `#GPU`, `#local AI`

---

<a id="item-4"></a>
## [Máy chủ LLM gia đình với bốn GPU RTX 4090 mod trên cổng sấy](https://www.reddit.com/r/LocalLLaMA/comments/1uhcy02/if_it_doesnt_make_my_pp_better_i_dont_want_it/) ⭐️ 6.0/10

Một người dùng Reddit chia sẻ máy chủ LLM gia đình được lắp ráp từ bốn GPU RTX 4090 đã mod (mỗi card 48 GB VRAM, tổng 192 GB) được cấp nguồn qua đường 240 V/30 A của máy sấy, kèm UPS chuyển đổi kép và quạt thoát nhiệt để quản lý nhiệt và tiếng ồn. Cấu hình này minh họa cách người đam mê có thể đẩy phần cứng tiêu dùng để chạy các mô hình ngôn ngữ lớn tại nhà, nhấn mạnh những thách thức thực tế về nguồn điện, làm mát và tiếng ồn ảnh hưởng đến khả năng mở rộng của phòng lab AI cá nhân. Hệ thống sử dụng PSU 3000 W, gặp hiện tượng ngắt GFCI gây phiền phù trên circuito máy sấy, và dự định thêm UPS chuyển đổi kép pure sine wave; nhiệt độ GPU khi idle khoảng 71 °C, quạt thoát nhiệt bật khi khoảng 79 °F.

reddit · r/LocalLLaMA · /u/dangerous_inference · 27/6 20:23

**Bối cảnh**: Modded RTX 4090 GPUs có VRAM được mở rộng từ 24 GB gốc lên 48 GB bằng cách thêm hoặc thay đổi mô-đun bộ nhớ trên PCB của card, cho phép chạy mô hình ngôn ngữ lớn hơn trên phần cứng tiêu dùng. UPS chuyển đổi kép (online) liên tục chuyển đổi điện AC nhập thành DC rồi ngược lại thành sóng sine AC trong lành, cách ly thiết bị khỏi các rối loạn điện. Ổ cắt GFCI bảo vệ chống lỗi đất nhưng có thể ngắt ngắt gây phiền phù khi thiết bị như máy giặt hoặc máy sấyรั่ว dòng nhỏ xuống đất, đặc biệt khi chia sẻ circuito.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://www.hardware-corner.net/48gb-rtx-4090-first-tests/">First Teardown: 48GB RTX 4090 Mod RUNS 70B LLMs Flawlessly</a></li>
<li><a href="https://www.eastpwr.com/blog/what-is-a-double-conversion-ups--double-conversion-ups-explained">What is a Double Conversion UPS? Double Conversion UPS Explained</a></li>
<li><a href="https://diyself.blog/washing-machine-trips-gfci-fix-fast">Why Your Washing Machine Trips the GFCI & How to Fix It Fast</a></li>

</ul>
</details>

**Thẻ**: `#LLM hardware`, `#GPU server`, `#power management`, `#home lab`, `#cooling`

---