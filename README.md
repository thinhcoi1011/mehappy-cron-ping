# mehappy-cron-ping

Bộ hẹn giờ (GitHub Actions) gọi endpoint nhắc lịch của meHappy Command Center mỗi 5 phút,
để nhắc từng việc đúng giờ hẹn (Vercel Free chỉ cron 1 lần/ngày).

- Endpoint: `https://command.mehappy.click/api/my-tasks/reminders/tick`
- Xác thực: header `Authorization: Bearer <CRON_SECRET>` — giá trị lưu ở **Settings → Secrets → Actions → CRON_SECRET**, KHÔNG nằm trong repo.
- Public repo để Actions miễn phí không giới hạn phút. Repo không chứa dữ liệu/secret nào.
