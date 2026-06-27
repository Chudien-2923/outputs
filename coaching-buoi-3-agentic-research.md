# BUỔI 3 — Agentic Workflow cho Nghiên cứu (OS Wiki)
## Giáo án chi tiết · Coaching 1:1 "Agentic AI & OS Second Brains"

> **Đối tượng buổi này:** một người **quản lý khách sạn** đang muốn đưa AI vào vận hành.
> **Mục tiêu Buổi 3:** hiểu **workflow nghiên cứu tri thức** của OSSB chạy ra sao (nguồn → raw → wiki → output → áp vào dự án) · biết **vì sao tri thức sẵn của AI chưa đủ** · nắm cơ chế **AI tự đi nghiên cứu** + **4 đường nạp nguồn** (YouTube · X · GitHub · blog) · tự tay biến nghiên cứu thành **một bản tổng hợp dùng được**.
> **Nền tảng:** Claude Code · OS Second Brains (OSSB).
> **Cách dùng file này:** đây là **tài liệu nguồn cho NotebookLM** — đổ vào làm "nguồn" rồi yêu cầu *"tạo slide thuyết trình từ nguồn này"*. Mỗi mục có **🎯 Điểm chốt** = câu sẵn-sàng-lên-slide.
> **Nguyên tắc giảng:** mọi thuật ngữ đều quy về ví dụ đời thường — dạy *cách nghĩ*, không dạy *nút bấm*.

---

# 1. Workflow nghiên cứu tri thức của OSSB — dòng chảy thật

Buổi 2 anh đã biết **WTA** (Workflow–Tools–Agent) và rằng chữ **W — Workflow** = "dây chuyền nhiều bước AI chạy theo thứ tự". Buổi này ta đi vào **một workflow cụ thể, quan trọng bậc nhất** của OSSB: **workflow biến tri thức ngoài đời thành tài sản trong hệ thống của anh.**

Đừng hình dung nó là một định nghĩa. Hãy nhìn nó là một **dòng chảy 4 chặng** — thứ gì đi vào ở đầu này, đi ra thành cái gì ở đầu kia:

```
   NGUỒN ngoài        →     raw/         →      wiki/          →     output/
 (YouTube, X,             (kho thô,           (AI biên thành        (kết luận
  GitHub, blog…)           giữ NGUYÊN,         "cẩm nang nhà mình"   để HÀNH ĐỘNG
                           không sửa)          có liên kết)          trong dự án)
```

| Chặng | Tên | Chuyện gì xảy ra (vỡ lòng) |
|---|---|---|
| **1** | **Nguồn** | Một thứ đáng học ngoài đời: video YouTube, thread trên X, repo GitHub, bài blog |
| **2** | **`raw/`** (kho thô) | Đưa nguyên văn nguồn đó vào kho — **giữ y nguyên, không bao giờ sửa** (để sau này còn đối chiếu gốc) |
| **3** | **`wiki/`** (tri thức) | AI **đọc kho thô → biên lại** thành các trang gọn, có liên kết với nhau: tóm tắt nguồn → gom vào chủ đề → rút ra khái niệm |
| **4** | **`output/`** (hành động) | Khi anh hỏi "vậy tôi nên làm gì", AI **tổng hợp từ wiki → ra một bản kết luận để LÀM**, áp thẳng vào dự án |

> **Ẩn dụ cốt lõi:** giống một **toà soạn báo**. Phóng viên mang tin thô về (raw) → biên tập viên viết thành bài có mục lục, liên kết bài cũ (wiki) → cuối cùng ra một **bản tin hành động** cho sếp đọc để ra quyết (output). Anh là tổng biên tập; AI làm cả phóng viên lẫn biên tập.

### Flow ứng dụng vào một dự án THỰC TẾ (ví dụ khách sạn)
Để thấy nó không phải lý thuyết — đây là một vòng chảy trọn vẹn:
1. Anh muốn **tăng khách quay lại** cho khách sạn → đặt câu hỏi: *"các khách sạn nhỏ đang chạy chương trình khách-thân-thiết (loyalty) kiểu gì?"*
2. AI **đi nghiên cứu** (mục 3) → mang về vài nguồn thật, để vào **raw**.
3. AI **biên thành wiki**: 1 trang tóm tắt mỗi nguồn + 1 trang chủ đề *"Loyalty cho khách sạn nhỏ"* + vài khái niệm (vd "ưu đãi đặt-trực-tiếp").
4. Anh hỏi *"vậy khách sạn tôi nên làm gì?"* → AI ra **output**: một bản đề xuất 3 bước áp cho đúng quy mô của anh.
5. Bản output đó **nằm lại trong hệ thống** — lần sau bàn chuyện loyalty, AI đã có sẵn nền, không bắt đầu từ số 0.

> 🎯 **Điểm chốt:** Workflow nghiên cứu của OSSB là một **dòng chảy 4 chặng**: Nguồn → `raw/` (giữ thô) → `wiki/` (AI biên thành tri thức có liên kết) → `output/` (kết luận để làm trong dự án). Nó biến *cái hay ngoài đời* thành *tài sản nằm lại trong hệ thống của anh*.

---

# 2. Vì sao phải đi nghiên cứu? — Tri thức sẵn trong AI có 3 lỗ hổng

Câu hỏi tự nhiên: *"AI đã biết cả internet rồi, hỏi thẳng nó chả được sao, đi nghiên cứu làm gì?"* — Phải hiểu chỗ này thật chắc, vì nó là **lý do tồn tại của cả buổi học**.

Phần kiến thức **có sẵn trong đầu** AI (gọi là *tri thức nội tại — internal knowledge*) đúng là khổng lồ, nhưng nó có **3 lỗ hổng chí mạng**:

| # | Lỗ hổng | Nghĩa là gì |
|---|---|---|
| **1** | **Không biết riêng anh** | Nó học kiến thức *chung* của thế giới, nhưng **không có một dòng nào về khách sạn của anh** — phong cách, khách, giá, vùng của anh |
| **2** | **Bị cũ** | Đầu nó "chốt sổ" tại một thời điểm (gọi là *cutoff*) — tin tức, công cụ, xu hướng **sau mốc đó nó không biết** |
| **3** | **Bịa rất tự tin** | Khi không chắc, nó vẫn **đoán và nói như thật** (anh đã gặp ở Buổi 1 — *ảo giác*): bịa số liệu, bịa tên |

> **Ẩn dụ (cốt lõi):** Tri thức sẵn của AI giống **một chuyên gia tư vấn vừa đáp máy bay tới gặp anh** — người này đã đọc qua cả triệu cuốn sách, kiến thức rộng kinh khủng, **nhưng chưa từng bước chân vào khách sạn của anh ngày nào**, cuốn sách mới nhất họ đọc thì **in từ năm ngoái**, và khi bị hỏi điều không chắc họ vẫn **trả lời trơn tru cho đỡ mất mặt**.
>
> → Anh sẽ không để một người như vậy tự ý ra quyết cho khách sạn. Anh sẽ bảo họ: *"đi khảo sát thực tế, đọc tài liệu mới nhất, rồi mang bằng chứng về đây."* — **Đó chính là "đi nghiên cứu".**

### Ví dụ khách sạn (thấy ngay lỗ hổng)
Hỏi thẳng *"phần mềm quản lý đặt phòng nào tốt nhất 2026?"*:
- **Dựa tri thức sẵn:** nó kể vài tên quen → nhưng có thể **đã đổi giá, ra bản mới, hoặc khai tử** mà nó không biết; tệ hơn là **bịa một cái tên** nghe hợp lý.
- **Bắt nó đi nghiên cứu:** nó tra nguồn thật mới nhất → trả lời kèm **dẫn nguồn để anh kiểm** → dùng được.

> 🎯 **Điểm chốt:** Tri thức sẵn của AI **rộng nhưng 3 lỗ hổng**: *không biết riêng anh · bị cũ · bịa tự tin*. Vì vậy việc quan trọng **không hỏi chay** — phải bắt AI **đi nghiên cứu nguồn thật** rồi mới tin.

---

# 3. AI tự đi nghiên cứu — cơ chế & 4 đường nạp nguồn

## 3.1. "AI tự nghiên cứu" chạy thế nào?
Nó **không phải phép màu** — chỉ là cái **vòng lặp Quan sát → Suy nghĩ → Hành động** (anh dạy ở Buổi 1) áp vào việc *đi tìm tin*:

```
  Anh ra 1 câu hỏi  →  AI tự tra nhiều nguồn  →  đọc & rút ý chính
         ↑                                              │
         └────── "còn thiếu góc nào?" → tra tiếp ───────┘
                            ↓ (đủ rồi)
              Một bản tổng hợp gọn, CÓ DẪN NGUỒN thật
```

**Khác Google ở đâu?** — Google đưa anh **10 cái link để anh tự ngồi đọc**. AI nghiên cứu thì **đọc thay anh cả chục nguồn, rồi giao lại một bản tóm gọn** đã sàng lọc. Và vì ta bắt nó **dẫn nguồn ra**, nó hết đường bịa — anh bấm vào kiểm được.

> **Ẩn dụ:** giống anh sai **một trợ lý đi khảo sát thị trường**: anh chỉ nói chủ đề, trợ lý tự đi gặp nhiều nơi, đọc nhiều tài liệu, rồi mang về **một tập hồ sơ tóm tắt + ghi rõ lấy ở đâu** — chứ không quăng cho anh nguyên đống tài liệu thô.

## 3.2. Bốn đường nạp nguồn vào `raw/` — và công cụ đi kèm
Tri thức ngoài đời nằm ở nhiều dạng. OSSB **đã dựng sẵn "đường ống"** (playbook) để hút từng dạng vào kho thô — anh không phải copy-paste tay:

| Nguồn | Công cụ nạp (đã có sẵn) | Hợp để học gì |
|---|---|---|
| **YouTube** 🎥 | `watch-cli` — tự tải video, **bóc lời thoại (transcript)** + chụp hình minh hoạ | Bài giảng, talk hội thảo, demo công cụ mới |
| **X / Twitter** 🐦 | Web Clipper / AI tự đọc trang (WebFetch) | Tip ngắn, thread chuyên gia, tin nóng trong ngành |
| **GitHub** 💻 | `gh` (lấy mô tả + cấu trúc + file chính của một dự án code) | Hiểu **một công cụ/công nghệ mới làm được gì** mà không cần biết code |
| **Blog / báo** 📰 | Web Clipper / AI tự đọc trang | Bài phân tích, hướng dẫn, case study |

> **Lưu ý vàng:** kho `raw/` là **bất biến — không bao giờ sửa**. Vì sao? Để nguồn gốc luôn nguyên vẹn mà đối chiếu, phòng khi AI biên sai ở bước sau còn lần về gốc kiểm được. (Giống **bản gốc hợp đồng** cất két — mọi người chỉ làm việc trên bản photo.)

## 3.3. Mục đích KÉP — đây mới là chỗ "lợi hại"
Đi nghiên cứu không chỉ để *học ngành mình*. Nó còn để **soi ra hướng nâng cấp chính cái hệ thống của anh**:

- **Hướng 1 — học ngành:** nghiên cứu "xu hướng tiện ích khách sạn boutique 2026" → áp vào vận hành.
- **Hướng 2 — nâng cấp hệ thống & cách làm việc:** thấy một **công cụ/quy trình hay** trên YouTube hay GitHub → **nạp vào `raw/`** → bảo AI *"đọc hộ, cái này lắp vào OSSB của tôi được không, lắp kiểu gì?"* → AI ra output đề xuất. Đây là cách **hệ thống tự lớn lên** thay vì đứng yên.

> **Ẩn dụ Hướng 2:** giống ông chủ đi hội chợ ngành, thấy một **máy pha cà phê đời mới** ở gian hàng khác → mang catalog về, hỏi quản lý *"lắp con này vào quy trình buổi sáng của mình được không?"*. Hệ thống nào cũng phải **liên tục hút cái mới về để tự nâng cấp**.

> 🎯 **Điểm chốt:** "AI tự nghiên cứu" = vòng **Quan sát→Suy nghĩ→Hành động** đi tìm tin, đọc thay anh rồi **giao bản tóm tắt có dẫn nguồn**. OSSB có sẵn **4 đường nạp** (YouTube · X · GitHub · blog) vào kho `raw/` *bất biến*. Mục đích **kép**: học ngành mình **và** soi hướng nâng cấp chính hệ thống của mình.

---

# 4. From Research → Wiki → Output: chắt thành tri thức DÙNG MÃI

Nghiên cứu xong mà để đó thì **lần sau lại phải nghiên cứu lại từ đầu** — phí. Sức mạnh thật nằm ở chỗ **chắt nó thành tri thức nằm lại**, dùng mãi. Đây là lúc dòng chảy ở mục 1 hoàn tất chặng `wiki/` và `output/`.

### AI "biên" kho thô thành wiki như thế nào (vỡ lòng)
Từ một nguồn trong `raw/`, AI tạo/cập nhật vài loại trang nối với nhau:

| Loại trang | Trả lời câu hỏi | Ví dụ khách sạn |
|---|---|---|
| **Trang nguồn** (source) | "Nguồn này nói gì?" | Tóm tắt 1 video về loyalty khách sạn |
| **Trang chủ đề** (topic) | "Tất cả những gì tôi biết về X?" | Hub *"Giữ chân khách khách sạn nhỏ"* gom mọi nguồn |
| **Trang khái niệm** (concept) | "Nguyên lý này là gì?" | *"Ưu đãi đặt-trực-tiếp"* — dùng lại cho nhiều chủ đề |

Các trang **liên kết với nhau** bằng đường dẫn (giống chú thích "xem thêm" trong sách), và có một **trang mục lục** (`index.md`) để AI biết "câu hỏi này thì lật tới trang nào".

> **Ẩn dụ "biên dịch":** giống **biên một cuốn cẩm nang nội bộ** từ đống tài liệu rời. Tài liệu rời = `raw/`. Người biên tập (AI) = đọc hết, viết lại gọn, **đánh số trang + làm mục lục + ghi "xem thêm trang…"**. Cuốn cẩm nang đã đóng gáy = `wiki/`. Lần sau cần, anh **lật mục lục là ra**, khỏi đọc lại đống thô.

### Compounding — vì sao càng dùng càng mạnh
Mỗi nguồn nạp vào **nằm lại vĩnh viễn** và **nối với cái đã có**. Nghiên cứu thứ 10 không bắt đầu từ số 0 — nó **đứng trên vai 9 cái trước**. Đây là điều một cuộc chat ChatGPT rời rạc **không bao giờ có** (chat xong là quên).

> 🎯 **Điểm chốt:** Nghiên cứu chỉ thành **tài sản** khi được **chắt vào wiki** (trang nguồn → chủ đề → khái niệm, có mục lục + liên kết) rồi ra **output để làm**. Tri thức **nằm lại và cộng dồn** — càng nạp, hệ thống càng khôn. Đây là khác biệt gốc giữa "hỏi AI" và "có một bộ não thứ hai".

---

# 5. 🛠 Thực hành tại chỗ — ra tài sản thứ ba cầm về

**Việc:** bắt AI **đi nghiên cứu một chủ đề thật của khách sạn anh** → ra một **bản tổng hợp có dẫn nguồn, dùng được ngay**. Chạy đúng nhịp **R→P→E→V** (Buổi 1) + mở màn bằng **prompt GCAO** (Buổi 1).

### Chọn 1 chủ đề (gợi ý — anh lấy cái nào nóng nhất với mình)
- *"Cách tăng đánh giá 5 sao trên Booking/Google cho khách sạn nhỏ."*
- *"Các chương trình giữ chân khách (loyalty) khách sạn quy mô nhỏ đang chạy."*
- *"Xu hướng tiện ích phòng được khách 2026 tìm kiếm nhiều."*

### Các bước thực thi

**Bước 1 — Mở Claude Code**, gõ prompt nghiên cứu theo **GCAO**:
> *"**[G]** Nghiên cứu giúp tôi: cách tăng lượng đánh giá 5 sao trên Booking & Google cho một khách sạn nhỏ. **[C]** Khách sạn ~20 phòng, phong cách ấm cúng, khách chính là cặp đôi đi nghỉ cuối tuần; tôi muốn cách làm thực tế, hợp quy mô nhỏ, không tốn ngân sách lớn. **[A]** Đi tìm nhiều nguồn thật, đọc, tổng hợp lại; **mỗi ý phải dẫn nguồn** để tôi kiểm; nói rõ chỗ nào các nguồn mâu thuẫn nhau. **[O]** Một bản tổng hợp gọn: 5–7 cách làm, mỗi cách 1–2 câu + nguồn; cuối bài ghi 3 việc tôi nên làm trước."*

**Bước 2 — (Plan) AI trình kế hoạch nghiên cứu** (định tra những góc nào, nguồn dạng gì) → anh đọc, gật *"ok làm đi"* hoặc bảo nó thêm góc.

**Bước 3 — (Execute) AI đi nghiên cứu** → trả về bản tổng hợp **có dẫn nguồn**.

**Bước 4 — (Verify) Anh kiểm** — đây là **cổng bắt buộc** (vì AI có thể bịa, Buổi 1): bấm thử 1–2 nguồn xem có thật không, đọc xem cách làm có hợp khách sạn anh không → bảo nó chỉnh chỗ chưa sát.

**Bước 5 — Cất thành tài sản:** bảo AI *"lưu bản này lại để lần sau dùng tiếp"* → nó đưa vào `output/` của hệ thống. (Nếu sau này anh muốn nó thành tri thức nền lâu dài, đây chính là nguyên liệu để **nạp vào wiki** — ta làm sâu hơn ở các buổi sau.)

> **Tài sản cầm về:** một **bản tổng hợp nghiên cứu có dẫn nguồn** về đúng một việc thật của khách sạn anh — **dùng để ra quyết ngay**, và đã nằm lại trong hệ thống.

> 🎯 **Điểm chốt:** Nghiên cứu một chủ đề thật chạy đúng **R→P→E→V**, mở bằng **GCAO**, **bắt dẫn nguồn** và **tự mình Verify** trước khi tin. Sản phẩm là một bản tổng hợp dùng-được, không phải một câu trả lời chat trôi mất.

---

# Nối dài (nhắc thoáng — để dành buổi sau)
Hai hướng mở rộng, chỉ giới thiệu tên cho anh biết có đường đi tiếp, **chưa làm sâu ở buổi này**:
- **Nạp chính thức vào wiki:** biến bản nghiên cứu thành các trang wiki có mục lục + liên kết (mục 4) để cộng dồn lâu dài.
- **AI tự cải tiến hệ thống:** ngoài "đi tìm tin", AI còn có thể chạy **vòng lặp tự thử – đo – giữ cái tốt hơn** để tối ưu một quy trình có "điểm số" (đây là nghĩa thứ hai của *autoresearch*, kiểu Karpathy) — một chủ đề nâng cao.

---

*Tài liệu nguồn cho NotebookLM → slide thuyết trình. Ví dụ ngành: quản lý khách sạn.*
*Khung gốc: [[master-curriculum-8-sessions]] (Buổi 3). Buổi trước: [[session-2-ossb-and-wta]]. Nền khái niệm (OS Wiki): LLM Wiki Architecture (raw→wiki→output) · AutoResearch Pattern · Compounding Knowledge Loop · Core Agent Loop.*
