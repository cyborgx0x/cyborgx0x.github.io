---
title: "Công thức đã 'giết' Phố Wall: sai lầm mô hình tương quan trong CDO 2008"
date: 2026-07-21
tags: ["kinh tế học", "tài chính", "khủng hoảng 2008", "CDO", "quản trị rủi ro"]
categories: ["Kinh tế"]
summary: "Một công thức đo tương quan vỡ nợ đã trở thành nền tảng định giá cho hàng nghìn tỷ đô la CDO — và giả định sai của nó về tương quan là một trong những mắt xích cốt lõi dẫn tới khủng hoảng 2008."
ShowToc: true
TocOpen: false
---

<div class="post-lede">
<p>Năm 2000, một công thức toán học tưởng chừng vô hại đã trả lời được câu hỏi mà cả Phố Wall khao khát: "nếu một khoản vay vỡ nợ, xác suất khoản kế bên cũng vỡ nợ là bao nhiêu?" Giả định sai của nó về bản chất của tương quan đã trở thành một trong những mắt xích cốt lõi của khủng hoảng tài chính 2008.</p>
</div>

## Bối cảnh

Năm 2000, nhà toán học định lượng **David X. Li** công bố công thức **Gaussian Copula** — một cách đo tương quan giữa xác suất vỡ nợ của nhiều khoản vay khác nhau. Công thức được các ngân hàng, tổ chức xếp hạng tín nhiệm (Moody's, S&P) và cả cơ quan quản lý áp dụng rộng rãi để định giá CDO (Collateralized Debt Obligation) và các tranche của nó.

## Cơ chế sai lầm

<ul class="flow">
<li><span class="flow-title">Coi tương quan là hằng số</span><div class="flow-body">Mô hình giả định tương quan vỡ nợ giữa các khoản vay ở các khu vực địa lý khác nhau tương đối thấp và ổn định theo thời gian — coi tương quan là một hằng số thay vì một đại lượng biến động, và không mô hình hóa được "tail dependence" (khả năng nhiều tài sản cùng vỡ nợ đồng loạt ở phần đuôi phân phối).</div></li>
<li><span class="flow-title">Gán AAA hàng loạt</span><div class="flow-body">Dựa trên giả định đó, các tổ chức xếp hạng gán chứng chỉ AAA cho phần lớn các gói CDO gộp từ hàng nghìn khoản vay dưới chuẩn.</div></li>
<li><span class="flow-title">Tương quan thực tế tiến gần 1</span><div class="flow-body">Khi giá nhà giảm trên diện rộng toàn quốc (không phải cục bộ từng khu vực), tương quan vỡ nợ thực tế tiến gần 1 thay vì gần 0 — các khoản vay vỡ nợ đồng loạt, kéo sập toàn bộ cấu trúc CDO cùng lúc.</div></li>
</ul>

<div class="stat-row">
<div class="stat"><span class="stat-num">~30.030</span><span class="stat-label">chứng khoán bất động sản Moody's xếp hạng AAA mỗi ngày làm việc trong năm 2006 (theo FCIC)</span></div>
<div class="stat"><span class="stat-num">6</span><span class="stat-label">công ty tư nhân Mỹ còn giữ được hạng AAA đầu năm 2009</span></div>
</div>

Ủy ban Điều tra Khủng hoảng Tài chính Mỹ (FCIC) kết luận các tổ chức xếp hạng là **"tác nhân then chốt gây ra sự sụp đổ tài chính"** — khủng hoảng "không thể xảy ra nếu không có sai phạm của họ".

## Nhóm 1 — Người cảnh báo công khai trước khủng hoảng

Nhóm này công bố công khai trước khi khủng hoảng xảy ra, nhưng không trực tiếp kiếm lời tài chính từ chính phát hiện của mình.

- **Paul Wilmott** (chuyên gia toán tài chính định lượng) — cảnh báo về bản chất bất ổn của tương quan tài chính **từ năm 1998**, tức trước cả khi Li công bố công thức (2000): "tương quan giữa các đại lượng tài chính vốn nổi tiếng là không ổn định", nên không nên xây lý thuyết định giá dựa trên một tham số biến động như vậy.
- **Janet Tavakoli** (chuyên gia cấu trúc tài chính) — viết và cảnh báo công khai về rủi ro của các cấu trúc CDO và CDO-bình phương cùng thực hành của các tổ chức xếp hạng.

## Nhóm 2 — Người khai thác thầm lặng

Theo Michael Lewis (*The Big Short*), chỉ khoảng **1/20 nhà đầu tư trên thế giới** nhận ra và đặt cược vào sự sụp đổ này trước 2007 — phần lớn hoạt động độc lập, không biết về nhau, và chỉ được công chúng biết tên sau khi sách/phim và báo chí phanh phui.

<div class="card-grid">
<div class="card">
<h4>Michael Burry</h4>
<p>Scion Capital. Phân tích chất lượng cho vay dưới chuẩn xuống cấp từ 2003–2004, đặt cược short qua CDS từ 2005 — một trong những người đầu tiên.</p>
</div>
<div class="card">
<h4>John Paulson</h4>
<p>Paulson &amp; Co. Thương vụ lời nhiều nhất: riêng năm 2007 kiếm khoảng 15 tỷ USD cho quỹ (cá nhân thu về gần 4 tỷ USD), được gọi là "thương vụ vĩ đại nhất lịch sử tài chính".</p>
</div>
<div class="card">
<h4>Greg Lippmann</h4>
<p>Trader tại Deutsche Bank — vừa giao dịch cho ngân hàng vừa chủ động truyền bá luận điểm short, thuyết phục khoảng 50 quỹ khác tham gia. Biệt danh "Bubble Boy"/"Patient Zero".</p>
</div>
<div class="card">
<h4>Cornwall Capital</h4>
<p>Quỹ "garage-band" khởi đầu chỉ 110.000 USD. Nhận ra tranche AAA rủi ro tương đương BBB nhưng CDS bảo hiểm cho AAA lại rẻ hơn nhiều (thị trường định giá sai) — thu về gấp khoảng 80 lần vốn.</p>
</div>
</div>

## Trường hợp gây tranh cãi — vừa khai thác vừa làm trầm trọng thêm bong bóng

Theo điều tra của ProPublica ("The Magnetar Trade", đoạt giải Pulitzer 2011), quỹ **Magnetar Capital** đầu tư vào khoảng 30 CDO (2006–2007) nhưng bị cáo buộc **chủ động yêu cầu đưa các trái phiếu rủi ro cao hơn vào cấu trúc CDO** (nhờ nắm phần tranche rủi ro nhất nên có quyền chọn tài sản), đồng thời đặt cược short chính các CDO đó. Kết quả: **96% giao dịch liên quan Magnetar vỡ nợ vào cuối 2008**, so với mức nền 68% của CDO thông thường cùng giai đoạn — cho thấy hành vi này có thể đã kéo dài và làm trầm trọng thêm bong bóng thay vì chỉ khai thác nó. SEC điều tra nhiều ngân hàng liên quan nhưng chưa từng khởi tố chính Magnetar.

## Nguồn

- Felix Salmon — *The Formula That Killed Wall Street* (Wired).
- *David X. Li*, *Michael Burry*, *The Greatest Trade Ever*, *Cornwall Capital*, *Magnetar Capital* — Wikipedia.
- *The Magnetar Trade* — ProPublica.
- *The Financial Crisis Inquiry Report* (FCIC, chính phủ Mỹ).

<p class="post-disclaimer">Ghi chú tham khảo tổng hợp từ các nguồn trên, không phải khuyến nghị đầu tư.</p>
