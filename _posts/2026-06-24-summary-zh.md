---
layout: default
title: "Horizon Summary: 2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> Đã chọn 5 tin quan trọng từ 14 nội dung.

---

1. [Datasette 1.0a35 thêm giao diện và API JSON để tạo và thay đổi bảng](#item-1) ⭐️ 8.0/10
2. [FUTO phát hành mô hình gõ vuốt mới để cải thiện độ chính xác và quyền riêng tư](#item-2) ⭐️ 7.0/10
3. [Simon Willison minh họa harness OPFS + Pyodide để chỉnh sửa SQLite 持久 trong Datasette Lite](#item-3) ⭐️ 7.0/10
4. [Headroom giảm sử dụng token LLM 60-95%.](#item-4) ⭐️ 7.0/10
5. [Trong kỷ niệm người đã đặt dấu gạch ngòi đỏ và xanh dưới từ](#item-5) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Datasette 1.0a35 thêm giao diện và API JSON để tạo và thay đổi bảng](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Phiên bản Datasette 1.0a35 ra mắt giao diện mới 'Create table' và API JSON (/<database>/-/create) cũng như 'Alter table' và API JSON (/<database>/<table>/-/alter), cho phép người dùng xác định cột, khóa, ràng buộc, giá trị mặc định và sửa đổi bảng hiện tại trực tiếp. Các tính năng này biến Datasette từ công cụ chỉ khám phá dữ liệu thành nền tảng định nghĩa dữ liệu nhẹ, giúp nhà phát triển và nhà phân tích dễ dàng tạo nguyên mẫu và phát triển lược đồ SQLite mà không cần rời khỏi giao diện. Giao diện tạo bảng hỗ trợ định nghĩa cột, khóa chính, ràng buộc NOT NULL, giá trị mặc định literal và biểu thức, loại cột tùy chỉnh và khóa ngoại đơn cột; giao diện thay đổi bảng cho phép thêm, đổi tên, sắp xếp lại, xóa cột, thay đổi kiểu, giá trị mặc định, ràng buộc, khóa chính/khóa ngoại, đổi tên bảng và có nút xóa bảng.

rss · Simon Willison · 23/6 21:34

**Bối cảnh**: Datasette là một ứng dụng mã nguồn mở viết bằng Python cho phép người dùng khám phá, trực quan hóa và xuất bản cơ sở dữ liệu SQLite qua giao diện web và API JSON tương ứng. Trước phiên bản 1.0a35, công cụ này chủ yếu chỉ đọc dữ liệu, yêu cầu các lệnh SQL bên ngoài để thay đổi lược đồ bảng. Các điểm cuối tạo và thay đổi bảng mới mở rộng API JSON của Datasette để hỗ trợ các thao tác định nghĩa dữ liệu (DDL) đầy đủ trực tiếp qua giao diện hoặc theo cách lập trình.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2022/Nov/9/designing-a-write-api-for-datasette/">Designing a write API for Datasette - Simon Willison's Weblog</a></li>
<li><a href="https://github.com/simonw/datasette/pull/2789">Create table, alter table - APIs and modals by simonw · Pull Request #2789 · simonw/datasette</a></li>

</ul>
</details>

**Thẻ**: `#datasette`, `#database`, `#SQL`, `#data-exploration`, `#open-source`

---

<a id="item-2"></a>
## [FUTO phát hành mô hình gõ vuốt mới để cải thiện độ chính xác và quyền riêng tư](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO đã phát hành một mô hình gõ vuốt mới nhằm cải thiện độ chính xác và quyền riêng tư cho bàn phím di động, có sẵn trong ứng dụng bàn phím Android offline‑first của FUTO và dưới dạng mô hình có thể tải xuống. Mô hình này giải quyết các lỗi thường gặp trong gõ vuốt như ranh giới từ mơ hồ và trùng lặp chữ cái, cung cấp một lựa chọn tập trung vào quyền riêng tư thay cho bàn phím phụ thuộc vào đám mây như Gboard. Điều này có thể thúc đẩy xu hướng người dùng chuyển sang các phương pháp nhập mã nguồn mở, hoạt động offline trên thiết bị di động. Mô hình gõ vuốt sử dụng mạng neural để phát hiện mẫu cử chỉ chỉ ra các chữ cái mục tiêu, được phát hành dưới giấy phép GPLv3 cho thư viện trong khi ứng dụng bàn phím Android sử dụng Giấy phép FUTO. Người dùng báo cáo độ chính xác cải thiện nhưng vẫn gặp một số vấn đề như viết hoa ngẫu nhiên và gợi ý thiếu bối cảnh.

hackernews · futohq · 23/6 17:50 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48648619)

**Bối cảnh**: Gõ vuốt cho phép người dùng trượt ngón tay trên các phím để tạo từ, dựa vào nhận dạng mẫu để suy ra văn bản mục tiêu. Các bàn phím tập trung vào quyền riêng tư nhằm giữ tất cả xử lý trên thiết bị để tránh gửi keystrokes lên máy chủ. FUTO là một dự án mã nguồn mở xây dựng công cụ hoạt động offline‑first, bao gồm ứng dụng bàn phím và mô hình AI, để đưa quyền kiểm soát dữ liệu cho người dùng.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://news.ycombinator.com/item?id=48648619">FUTO Swipe – A new swipe typing model - Hacker News</a></li>
<li><a href="https://windowsforum.com/threads/futo-keyboard-the-offline-first-android-keyboard-for-true-on-device-privacy.405419/">FUTO Keyboard: The Offline First Android Keyboard for True On-Device Privacy | Windows Forum</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: Người dùng khen ngợi mô hình gõ vuốt mới vì tốc độ và khả năng sử dụng một tay, cho biết nó đã đạt mức 相当 với Gboard sau bản cập nhật gần đây, nhưng họ cũng chỉ ra các vấn đề như viết hoa ngẫu nhiên, thiếu gợi ý dựa trên bối cảnh và occasional mis‑swipes như “whats” thay vì “what’s”. Một số người đánh giá cao cách tiếp cận tập trung vào quyền riêng tư và việc đóng góp dữ liệu gõ vuốt của họ để cải thiện mô hình.

**Thẻ**: `#swipe typing`, `#mobile keyboard`, `#privacy`, `#input method`, `#FUTO`

---

<a id="item-3"></a>
## [Simon Willison minh họa harness OPFS + Pyodide để chỉnh sửa SQLite 持久 trong Datasette Lite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 7.0/10

Simon Willison đã xây dựng một harness kiểm tra kết hợp Hệ thống File Riêng Tư Gốc (OPFS) với Pyodide để cho Datasette Lite có thể chỉnh sửa các file SQLite 持久 trực tiếp trong trình duyệt. Điều này chứng minh một con đường thực tế để các ứng dụng Python phía client có thể giữ dữ liệu người dùng giữa các phiên mà không cần máy chủ, thúc đẩy các công cụ như Datasette Lite cho việc làm việc dữ liệu ngoại tuyến. Harness sử dụng API đồng bộ của OPFS từ Web Workers để thực hiện I/O nhanh và dựa trên micropip của Pyodide để cài đặt Datasette và các mở rộng SQLite; nó hoạt động trên các trình duyệt hỗ trợ File System API như Chrome và Edge.

rss · Simon Willison · 23/6 18:58

**Bối cảnh**: Hệ thống File Riêng Tư Gốc (OPFS) là một hệ thống file được cung cấp bởi API File System, riêng tư với nguồn gốc trang, không hiển thị cho người dùng và duy trì qua các phiên. Pyodide biên dịch trình thông dịch CPython sang WebAssembly, cho phép chạy các gói Python như NumPy và Pandas trong trình duyệt và kết nối với JavaScript qua micropip. Datasette Lite chạy Datasette hoàn toàn trong trình duyệt bằng Pyodide, nhưng trước đây chỉ có thể làm việc với các file SQLite được tải vào bộ nhớ.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN - MDN Web Docs</a></li>
<li><a href="https://pyodide.com/">Pyodide – Run Python in Browser with WebAssembly</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**Thẻ**: `#browsers`, `#pyodide`, `#opfs`, `#datasette-lite`, `#webassembly`

---

<a id="item-4"></a>
## [Headroom giảm sử dụng token LLM 60-95%.](https://github.com/chopratejas/headroom) ⭐️ 7.0/10

Kho lưu trữ GitHub chopratejas/headroom đã nhận được 92 sao trong 24 giờ, ra mắt một thư viện và proxy Python nén đầu ra công cụ, nhật ký, tệp và các đoạn RAG trước khi chúng đến LLM, giảm sử dụng token 60-95% mà vẫn giữ chất lượng câu trả lời. Bằng cách giảm đáng kể số token gửi đến LLM, Headroom giúp giảm chi phí API và độ trễ, làm cho các ứng dụng AI hiệu quả và mở rộng hơn. Headroom hoạt động dưới dạng thư viện, proxy hoặc máy chủ MCP, hỗ trợ nén nhiều loại dữ liệu và tuyên bố không mất chất lượng câu trả lời sau khi giải nén.

ossinsight · chopratejas · 24/6 03:55

**Bối cảnh**: Các mô hình ngôn ngữ lớn xử lý đầu vào dưới dạng token, và lượng token 過多 sẽ tăng chi phí và độ trễ. Kỹ thuật nén ngữ cảnh nhằm giảm số token bằng cách tóm tắt hoặc trích xuất thông tin liên quan trước khi đưa vào mô hình. Giao thức Mô hình Ngữ cảnh (MCP) xác định cách các tác nhân AI (host) tương tác với máy chủ MCP để truy cập công cụ và dữ liệu, cho phép lớp như Headroom đặt giữa tác nhân và LLM. Trong hệ thống Retrieval-Augmented Generation (RAG), các đoạn được truy xuất thường lớn; việc nén các đoạn này có thể cải thiện hiệu suất mà không làm giảm chất lượng sinh ra.

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://andrew.ooo/posts/headroom-context-compression-llm-agents-review/">Headroom Review: 60-95% LLM Token Compression (2026)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://www.runlocalai.co/learn/courses/advanced-rag/chapter-17-context-compression">Context Compression — Advanced RAG — Chunking ... | RunLocalAI</a></li>

</ul>
</details>

**Thẻ**: `#LLM optimization`, `#token compression`, `#Python library`, `#AI infrastructure`, `#developer tools`

---

<a id="item-5"></a>
## [Trong kỷ niệm người đã đặt dấu gạch ngòi đỏ và xanh dưới từ](https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451) ⭐️ 6.0/10

Bài viết 向纪念那位微软工程师，他的想法在文字处理器中引入了实时拼写检查，用红色波浪线标记拼写错误，用绿色波浪线标记语法错误。文章描述了这一创新如何将拼写检查从手动批处理转变为实时的内联反馈。 这一微小的界面变化已成为现代文本编辑器和 IDE 中无处不在的功能，塑造了用户获得即时写作反馈的方式。它说明了单个设计决策如何能够对生产力和用户体验产生持久影响。 红色下划线标记潜在的拼写错误，而绿色下划线则指示可能的语法问题；该功能作为后台进程运行，在用户输入时实时检查文纟。虽然这一概念最初在 Microsoft Word 95 中流行，但已被许多编辑器采用，尽管在多语言环境中可能会产生误报。

hackernews · saikatsg · 23/6 18:10 · [Thảo luận cộng đồng](https://news.ycombinator.com/item?id=48648959)

**Bối cảnh**: 在实时拼写检查出现之前，用户必须运行单独的拼写检查命令才能在完成文档后看到错误。波浪线的引入提供了即时的内联警告，减少了对显式检查的需求。这一做法建立在诸如 Sector Software 的 Spellbound（1987）等早期交互式拼写检查器之上，并在 Word 95 起成为 Word 的标准功能。

<details><summary>Liên kết tham khảo</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spell_checker">Spell checker - Wikipedia</a></li>
<li><a href="https://support.microsoft.com/en-us/office/check-spelling-and-grammar-in-office-5cdeced7-d81d-47de-9096-efd0ee909227">Check spelling and grammar in Office | Microsoft Support</a></li>
<li><a href="https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451">In memory of the man who put red and green squiggles under words - The Old New Thing</a></li>

</ul>
</details>

**Thảo luận cộng đồng**: 评论者觉得这篇文章有趣，注意到维基百科的自引用引用，表达了在多语言环境中语言检测不准确的挫败感，欣赏这则历史轶事，希望文章能更早发表，并开玩笑地建议用黄色波浪线标记逻辑错误。

**Thẻ**: `#spellcheck`, `#UI history`, `#Microsoft`, `#software engineering`, `#Hacker News`

---