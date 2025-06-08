# peg-alert-bot

Telegram bot theo dõi peg x33/SHADOW, gửi cảnh báo SL/TP khi peg đạt ngưỡng. Đã tối ưu để deploy miễn phí trên Railway.

## 📦 Nội dung

- `main.py` — Script Python chính kiểm tra peg và gửi tin qua Telegram.
- `requirements.txt` — Thư viện cần thiết.

## ▶️ Triển khai trên Railway

1. **Tạo repository** trên GitHub với cấu trúc trên.
2. **Import project** vào Railway (Login rồi chọn "Deploy from GitHub").
3. **Thiết lập biến môi trường**:
   - `BOT_TOKEN` = `TOKEN`
   - `CHAT_ID` = `YOUR_CHAT_ID`
4. **Command khi chạy**: `python main.py`
5. **Chỉnh `main.py` nếu cần thay ngưỡng SL/TP**:
   ```python
   STOP_LOSS = 0.880
   TAKE_PROFIT_1 = 0.970
   TAKE_PROFIT_2 = 0.995
