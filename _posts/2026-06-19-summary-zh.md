---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> Đã chọn 4 tin quan trọng từ 10 nội dung.

---

1. [Nhà nghiên cứu phát hiện khoảng 10.000 kho GitHub lan truyền phần mềm Tròjan](#item-1) ⭐️ 8.0/10
2. [Plugin Datasette Apps cho phép ứng dụng HTML/JS trong sandbox có truy cập SQL](#item-2) ⭐️ 7.0/10
3. [datasette-acl 0.6a0 mở rộng chia sẻ tài nguyên chung](#item-3) ⭐️ 7.0/10
4. [Robot vali sử dụng cảm biến MQ-2 để điều chỉnh động LLM sampling](#item-4) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Nhà nghiên cứu phát hiện khoảng 10.000 kho GitHub lan truyền phần mềm Tròjan](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 8.0/10

Một nhà nghiên cứu bảo mật đã phát hiện khoảng 10.000 kho GitHub chứa phần mềm Tròjan, tạo thành một cuộc tấn công chuỗi cung ứng rộng lớn nhắm vào các nhà phát triển. Mã độc được giấu trong các dự án có vẻ hợp pháp và được cập nhật thường xuyên để tránh phát hiện. Kampanye này đe dọa tính toàn vẹn của chuỗi cung ứng phần mềm mã nguồn mở, có thể làm suy giảm vô số dự án downstream không biết đã tích hợp mã độc. Nó nhấn mạnh rủi ro tăng cao của các cuộc tấn công tự động nhắm vào nhà phát triển và nhu cầu kiểm tra sự phụ thuộc chặt chẽ hơn. Các kẻ tấn công tạo ra các kho mới, xóa các commit cũ và đẩy commit mới mỗi vài giờ để luôn đứng đầu danh sách 'Last Updated', khiến phiên bản Tròjan của họ xuất hiện trong các tìm kiếm tự động của các công cụ phụ thuộc. Họ thường sao chép tên các dự án hợp pháp phổ biến để lừa nhà phát triển và bot sao chép mã độc.

hackernews · theorchid · 18/6 11:45 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48583928)

**Bối cảnh**: Một cuộc tấn công chuỗi cung ứng xảy ra khi kẻ tấn công xâm nhập thành phần bên thứ ba đáng tin cậy—ví dụ như một thư viện hoặc kho mã—to phân phối phần mềm độc hại cho tất cả người dùng downstream. Trong bối cảnh phần mềm, điều này có nghĩa là tiêm mã độc vào các gói mã nguồn mở mà nhà phát triển thường xuyên tích hợp vào ứng dụng của họ. Tròjan là một loại phần mềm độc hại che giấu mình dưới dạng phần mềm hợp pháp, lừa người dùng thực thi nó đồng thời mang theo payload gây hại ẩn.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trojan_horse_(computing)">Trojan horse (computing) - Wikipedia</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Các bình luận nhận thấy rằng kẻ tấn công tập trung vào các kho newly created và thường xuyên viết lại commit để đứng đầu danh sách 'Last Updated', nhắm vào các tác nhân tự động tìm kiếm các phụ thuộc mới. Một số người dùng báo cáo họ thấy tên dự án của mình được sao chép bởi các kẻ độc hại, gây ra lo ngại về việc mạo danh và khó khăn trong việc phát hiện các cuộc tấn công như vậy.

**Thẻ**: `#security`, `#malware`, `#GitHub`, `#supply-chain`, `#cybersecurity`

---

<a id="item-2"></a>
## [Plugin Datasette Apps cho phép ứng dụng HTML/JS trong sandbox có truy cập SQL](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

Simon Willison đã phát hành plugin datasette-apps, cho phép phát triển các ứng dụng HTML+JavaScript tự chứa trong Datasette qua một iframe sandbox có thể thực hiện truy vấn SQL chỉ đọc và có thể cấu hình để ghi. Plugin này giảm thiểu rào cản để xây dựng công cụ nội bộ trên Datasette bằng cách cung cấp một cách an toàn để nhúng UI tùy chỉnh có thể trực tiếp truy vấn và sửa đổi dữ liệu, mở rộng tính hữu ích của Datasette vượt quá chỉ là API JSON. Các ứng dụng chạy trong <iframe sandbox="allow-scripts allow-forms"> có tiêu đề CSP được chèn để chặn yêu cầu HTTP ngoài và truy cập cookie hoặc localStorage, trong khi JavaScript có thể thực hiện truy vấn SQL qua API của Datasette, khả năng ghi được bật qua các truy vấn được lưu trữ.

rss · Simon Willison · 18/6 23:58

**Bối cảnh**: Datasette là công cụ mã nguồn mở xuất bản cơ sở dữ liệu SQLite dưới dạng API JSON có thể duyệt và giao diện web. Hệ thống plugin của Datasette cho phép nhà phát triển thêm tính năng mới như trực quan hoá dữ liệu hoặc phương thức xác thực. Plugin datasette‑apps sử dụng iframe sandbox với cờ allow‑scripts và allow‑forms kèm tiêu đề CSP hạn chế để cô lập mã HTML/JS không đáng tin. Truyền SQL có thể ghi được thực hiện qua các truy vấn được lưu trữ của Datasette, có thể được cấp quyền bổ sung để thực hiện INSERT/UPDATE/DELETE.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-apps/">Datasette Apps: Host custom HTML applications inside Datasette</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/HTMLIFrameElement/sandbox">HTMLIFrameElement: sandbox property - Web APIs | MDN</a></li>
<li><a href="https://docs.datasette.io/en/latest/sql_queries.html">Running SQL queries - Datasette documentation</a></li>

</ul>
</details>

**Thẻ**: `#datasette`, `#plugin`, `#web-apps`, `#SQL`, `#iframe-sandbox`

---

<a id="item-3"></a>
## [datasette-acl 0.6a0 mở rộng chia sẻ tài nguyên chung](https://simonwillison.net/2026/Jun/18/datasette-acl/#atom-everything) ⭐️ 7.0/10

Phiên bản 0.6a0 của plugin datasette-acl mở rộng mô hình quyền từ chỉ kiểm soát bảng sang một hệ thống chia sẻ tài nguyên chung, cho phép kiểm soát truy cập chi tiết cho các phiên bản Datasette đa người dùng. Thay đổi này cho phép quản trị viên xác định ai có thể xem hoặc chỉnh sửa bất kỳ tài nguyên nào—not chỉ bảng—làm cho Datasette phù hợp hơn với việc xuất bản dữ liệu cộng tác và đa thuê. Phát hành này là phiên bản alpha (0.6a0) và yêu cầu Datasette 1.0a15 hoặc cao hơn; quyền tiếp tục được lưu trữ trong cơ sở dữ liệu nội bộ của Datasette.

rss · Simon Willison · 18/6 19:03

**Bối cảnh**: Datasette là một công cụ mã nguồn mở cho phép người dùng khám phá, phân tích và xuất bản bất kỳ bộ dữ liệu nào dưới dạng trang web tương tác và API. Hệ thống quyền nội bộ của Datasette trả lời câu hỏi liệu một hành động có thể được thực hiện bởi một người dùng trên một tài nguyên cụ thể, và có thể được mở rộng bằng các plugin như datasette‑acl. Trước phiên bản 0.6a0, plugin datasette‑acl chỉ hỗ trợ thiết lập quyền cho từng bảng riêng lẻ, gây hạn chế trong việc kiểm soát chi tiết cho các môi trường đa người dùng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>
<li><a href="https://docs.datasette.io/en/latest//authentication.html">Authentication and permissions - Datasette documentation</a></li>
<li><a href="https://pypi.org/project/datasette-acl/">datasette-acl · PyPI</a></li>

</ul>
</details>

**Thẻ**: `#datasette`, `#datasette-acl`, `#plugin`, `#permissions`, `#alex-garcia`

---

<a id="item-4"></a>
## [Robot vali sử dụng cảm biến MQ-2 để điều chỉnh động LLM sampling](https://www.reddit.com/r/LocalLLaMA/comments/1u9a17y/my_suitcase_robot_gets_high_now_off_a_real_gas/) ⭐️ 6.0/10

Người tạo đã nối cảm biến MQ-2 vào robot vali ngoại tuyến, sử dụng đọc khói trực tiếp để điều chỉnh tham số temperature, top_p và top_k của LLM, khiến lời nói của robot trở nên càng loạn và không lặp lại. Hack này thể hiện cách mới kết nối dữ liệu cảm biến thực tế với hành vi mô hình sinh tạo, mở ra khả năng cho AI có thân thể thích ứng sáng tạo dựa trên dấu hiệu môi trường. Cảm biến được đọc mỗi 0,5 s, được ánh xạ sang giai đoạn 0‑10 làm thay đổi temperature từ 1,0 lên khoảng 1,6, top_p từ 0,95 lên 0,99 và top_k từ 64 lên 120; mỗi giai đoạn có một lời nhắc persona thay đổi lựa chọn từ mà không cần nói explícit 'cao', và hiệu ứng giảm dần trong vài phút.

reddit · r/LocalLLaMA · /u/CreativelyBankrupt · 18/6 15:52

**Bối cảnh**: Cảm biến MQ-2 phát hiện khói và các hợp chất hữu cơ bay hơi bằng cách thay đổi điện trở nội bộ khi tiếp xúc với gas, cung cấp tín hiệu analog pouvant được hiệu chỉnh so với mức không khí trong lành. Trong các mô hình LLM, tham số temperature điều chỉnh mức độ ngẫu nhiên trong việc chọn token, top_p (nucleus sampling) giới hạn việc chọn token trong tập hợp nhỏ nhất có xác suất tích lũy vượt qua ngưỡng nhất định, còn top_k giới hạn chọn chỉ trong k token có xác suất cao nhất. Kỹ thuật baseline thích ứng liên tục cập nhật mức điện trở tham chiếu của cảm biến để bù đrift, cho phép đo lường đáng tin cậy các mức độ gas thay đổi theo thời gian.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://lastminuteengineers.com/mq2-gas-senser-arduino-tutorial/">How MQ2 Gas/Smoke Sensor Works? & Interface it with Arduino How to Use MQ-2 GAS SENSOR: Examples, Pinouts, and Specs MQ-2 Smoke/Gas Sensor: Datasheet, Pinout & Working MQ-2 Gas Sensor Arduino: Complete Guide to Smoke and LPG ... MQ-2 Gas & Smoke Sensor Tutorial: LPG, Propane, Methane ... Images Arduino - Gas Sensor | Arduino Tutorial How MQ-2 Gas Smoke Sensor Works: A Complete Guide to ...</a></li>
<li><a href="https://aviralrma.medium.com/understanding-llm-parameters-c2db4b07f0ee">Understanding temperature, top_p, top_k, logit_bias in LLM parameters | by Aviral Verma</a></li>
<li><a href="https://www.sensorbee.com/post/high-accuracy-gas-sensors-with-automatic-baseline-calibration-the-future-of-environmental-monitorin">High-Accuracy Gas Sensors with Automatic Baseline Calibration ...</a></li>

</ul>
</details>

**Thẻ**: `#LLM`, `#robotics`, `#sensor integration`, `#generative AI`, `#creative hacking`

---