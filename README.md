# Waitlist (Free) + Monitoring
Fields: email, farcaster, twitter (X), wallet. Data disimpan privat di Vercel Blob.
Sudah termasuk: /api/submit, /admin, /api/list, /api/export-csv, /api/health, region sin1.

## Deploy
1) Import ke Vercel.
2) Storage → Blob → Create Store → Generate Read-Write Token.
3) Settings → Env Vars:
   - BLOB_READ_WRITE_TOKEN
   - ADMIN_TOKEN
4) Deploy.

## Monitor
- UptimeRobot → monitor HTTP ke /api/health.
- Logs: Vercel → Functions → Logs.

## Notif Telegram (opsional)
Tambahkan TELEGRAM_BOT_TOKEN dan TELEGRAM_CHAT_ID; submit.js akan kirim pesan otomatis.
