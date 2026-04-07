(venv) PS C:\Users\KIM ANH\OneDrive\Máy tính\lab4_agent\venv> python agent.py
============================================================
TravelBuddy — Trợ lý Du lịch Thông minh
      Gõ 'quit' để thoát
============================================================

Người dùng: Xin chào! Tôi đang muốn đi du lịch nhưng chưa biết đi đâu.

TravelBuddy đang suy nghĩ...
2026-04-07 14:28:14,516 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:14,522 — INFO — Direct answer — không gọi tool

TravelBuddy: Chào bạn! Để mình có thể giúp bạn tốt hơn, bạn có sở thích đi biển, núi hay thăm phố cổ? Bạn dự định đi trong khoảng thời gian nào và ngân sách dự kiến của bạn là bao nhiêu?

Người dùng: Tìm giúp tôi chuyến bay từ Hà Nội đi Đà Nẵng

TravelBuddy đang suy nghĩ...
2026-04-07 14:28:19,158 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:19,161 — INFO — Tool call: search_flights({'origin': 'Hà Nội', 'destination': 'Đà Nẵng'})
2026-04-07 14:28:21,650 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:21,653 — INFO — Direct answer — không gọi tool

TravelBuddy: ✈️ **Chuyến bay** 
- **VietJet Air** | 08:30 → 09:50 | Giá/người: 890.000đ 
- **Bamboo Airways** | 11:00 → 12:20 | Giá/người: 1.200.000đ 

Giá có thể thay đổi khi đặt chính thức. Bạn có dự định đặt chuyến bay nào trong số này không, hay cần thêm thông tin gì khác?

Người dùng: Tôi ở Hà Nội, muốn đi Phú Quốc 2 đêm, budget 5 triệu. Tư vấn giúp!

TravelBuddy đang suy nghĩ...
2026-04-07 14:28:35,633 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:35,634 — INFO — Tool call: search_flights({'origin': 'Hà Nội', 'destination': 'Phú Quốc'})
2026-04-07 14:28:35,635 — INFO — Tool call: search_hotels({'city': 'Phú Quốc', 'max_price_per_night': 1020000})
2026-04-07 14:28:37,091 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:37,095 — INFO — Tool call: calculate_budget({'total_budget': 5000000, 'expenses': 'vé_máy_bay:1100000,khách_sạn:1600000'})
2026-04-07 14:28:44,683 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:28:44,691 — INFO — Direct answer — không gọi tool

TravelBuddy: ✈️ **Chuyến bay** 
- **VietJet Air** | 16:00 → 18:15 | Giá/người: 1.100.000đ 
- (có thêm lựa chọn chuyến sớm hơn với VietJet Air 10:00 → 12:15 giá 1.350.000đ)

🏨 **Khách sạn gợi ý** 
1. **9Station Hostel (2★)** | Dương Đông | Giá/đêm: 200.000đ | ⭐ 4.5
2. **Lahana Resort (3★)** | Dương Đông | Giá/đêm: 800.000đ | ⭐ 4.0

💰 **Phân bổ ngân sách**
| Hạng mục           | Chi phí     |
|--------------------|-------------|
| Vé máy bay         | 1.100.000đ  |
| Khách sạn (2 đêm)  | 400.000đ    |
| Ăn uống            | 1.000.000đ  |
| Di chuyển nội địa  | 500.000đ    |
| Vui chơi tham quan | 1.400.000đ  |
| Dự phòng           | 200.000đ    |
| **Tổng**           | **5.000.000đ**|

💡 **Gợi ý thêm**: 
Bạn nên thử các món hải sản tươi sống ở Phú Quốc, đặc biệt là ghẹ hàu hay gỏi cá trích nổi tiếng. Thời tiết ở Phú Quốc thường đẹp và nắng ấm, hãy mang theo đồ bơi và kem chống nắng!

⚠️ *Giá trên là ước tính, có thể thay đổi khi đặt chính thức.*

Bạn có muốn đặt chuyến bay hoặc cần thêm thông tin về khách sạn không?

Người dùng: Tôi muốn đặt khách sạn

TravelBuddy đang suy nghĩ...
2026-04-07 14:29:00,370 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:29:00,370 — INFO — Direct answer — không gọi tool

TravelBuddy: Bạn muốn ở khách sạn nào, mấy đêm, và ngân sách khoảng bao nhiêu?

Người dùng: Giải giúp tôi bài tập lập trình Python về linked list

TravelBuddy đang suy nghĩ...
2026-04-07 14:29:15,718 — INFO — HTTP Request: POST https://api.openai.com/v1/chat/completions "HTTP/1.1 200 OK"
2026-04-07 14:29:15,720 — INFO — Direct answer — không gọi tool

TravelBuddy: Xin lỗi, nhưng mình không thể giúp bạn về lập trình hoặc các bài tập liên quan đến khoa học máy tính. Tuy nhiên, nếu bạn có bất kỳ câu hỏi nào về lên kế hoạch chuyến đi hay du lịch, mình rất vui lòng hỗ trợ! Bạn có muốn hỏi gì về du lịch không?