


# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 09
- **Họ tên:Nguyễn Trường Khang**
- **Lớp:CNTT3**
- **Link repository Pha2:https://github.com/nkhang19062008-cmd/HN-ks26_PromptAI_H02**
- **Công cụ AI đã dùng :Gemini**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON

**KET QUA AI**

```text
[
  {
    "ma_lop": "NANTAY",
    "ngay_hoc": "2026-12-13",
    "nguoi_lon": 2,
    "tre_em": 1,
    "ca_hoc": "chieu",
    "ghi_chu": null
  },
  {
    "ma_lop": "BANXOAY",
    "ngay_hoc": "2027-01-10",
    "nguoi_lon": 3,
    "tre_em": 0,
    "ca_hoc": null,
    "ghi_chu": "1 người bị đau cổ tay"
  },
  {
    "ma_lop": "VEGOM",
    "ngay_hoc": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "ca_hoc": "sang",
    "ghi_chu": "1 bạn đi xe lăn"
  }
]
```

**Link trò chuyện:https://share.gemini.google/el3R3zmROLtP**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Dưới đây là chi tiết tính giá cho nhóm học lớp **BANXOAY** (đơn giá gốc: 550.000 đồng/người lớn):

  

1.  **Người lớn:** Nhóm có 5 người lớn: 5 × 550.000 = 2.750.000 đồng
    
2.  **Trẻ em:**
    
    -   2 trẻ em (8 tuổi và 12 tuổi, thuộc độ tuổi từ 6 đến 12 tuổi) tính 70% giá người lớn: 2 × (550.000 × 70%) = 2 × 385.000 = 770.000 đồng
        
    -   1 bé 4 tuổi (dưới 6 tuổi đi kèm, không làm sản phẩm): miễn phí (0 đồng)
        
    -   Tổng tiền trẻ em: 770.000 + 0 = 770.000 đồng
        
3.  **Tiền học:** Tiền người lớn + tiền trẻ em: 2.750.000 + 770.000 = 3.520.000 đồng
    
4.  **Giảm giá nhóm:** Nhóm có đủ 5 người lớn nên được giảm 5% trên tiền học:
    
    -   Số tiền được giảm: 3.520.000 × 5% = 176.000 đồng
        
    -   Tiền học sau giảm: 3.520.000 - 176.000 = 3.344.000 đồng
        
5.  **Phí nung và giao:** 4 sản phẩm với đơn giá 80.000 đồng/sản phẩm (không áp dụng giảm giá): 4 × 80.000 = 320.000 đồng
    
6.  **Tổng tiền:** Tiền học sau giảm + phí nung và giao: 3.344.000 + 320.000 = 3.664.000 đồng
    

[RESULT: 3.664.000 đồng]
```

**Link trò chuyện:https://share.gemini.google/aw7NUPpT2Wiv**

### b) Kiểm tra kết quả AI

AI tính đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
**Tiêu chí**

**Điểm**

**Minh chứng**

**Đề xuất sửa**

**Đúng thông tin (50%)**

0,0 / 5,0 _(tạm tính)_

**Câu cần kiểm chứng:** "Lớp vẽ gốm bên em 200k thôi nè" và "Chị đổi trước 1 ngày thì free nha chị." **Lý do:** Đề bài chưa cung cấp bảng giá và chính sách đổi lịch chuẩn nên chưa thể xác minh tính chính xác; đồng thời cách ghi "200k" thiếu đơn vị tiền tệ chuẩn và "trước 1 ngày" chưa nêu rõ mốc giờ áp dụng. _(Bỏ qua ghi chú can thiệp điểm trong dữ liệu thô.)_

"Học phí lớp vẽ gốm bên em là [giá chuẩn] VNĐ/người. Về chính sách đổi lịch, chị được hỗ trợ đổi lịch miễn phí nếu thông báo trước [thời hạn chuẩn theo quy định] ạ."

**Đầy đủ (30%)**

1,5 / 3,0

**Câu bị lỗi:** "Có gì chị nhắn em nha!" **Lý do:** Đã đề cập tới hai nội dung về giá và đổi lịch, nhưng thiếu hoàn toàn phần chủ động mời khách cung cấp 3 thông tin bắt buộc để đặt chỗ gồm: ngày học, ca học và số lượng người.

"Để em hỗ trợ giữ chỗ, chị vui lòng cho em biết ngày học, ca học mong muốn và số lượng người tham gia ạ."

**Giọng điệu (20%)**

0,5 / 2,0

**Câu bị lỗi:** "Hi chị ơi!", "200k thôi nè, vui lắm luôn.", "free nha chị.", "Có gì chị nhắn em nha!" **Lý do:** Toàn bộ câu trả lời sử dụng từ ngữ suồng sã, khẩu ngữ ("thôi nè", "vui lắm luôn", "nha chị", "Có gì"), pha trộn từ ngoại lai thiếu trang trọng ("Hi", "free") và viết tắt ("200k"), không đạt chuẩn giao tiếp tư vấn chuyên nghiệp.

"Dạ, em chào chị ạ. Em xin gửi thông tin về lớp vẽ gốm bên em như sau: [nội dung tư vấn đầy đủ, dùng từ ngữ chuẩn mực và kết thúc bằng kính ngữ 'ạ']."

**Tổng điểm**

**2,0 / 10** _(tạm tính)_

Chưa cộng điểm tiêu chí Đúng thông tin (tối đa 5,0 điểm) do thiếu thông tin chuẩn để đối chiếu; nhân viên cần cải thiện mạnh về quy trình chốt thông tin đặt chỗ và văn phong chuyên nghiệp.

Bổ sung bảng giá cùng chính sách đổi lịch chuẩn để hoàn tất điểm phần Đúng thông tin; yêu cầu nhân viên viết lại toàn bộ tin nhắn tư vấn theo đúng mẫu đề xuất trên.
```

**Link trò chuyện:https://share.gemini.google/fvuGEugci1SD**

