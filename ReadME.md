# GreedDownloaderBot
Live Demo: https://t.me/GreedDownloaderbot
<1s Instagram Reel downloader - Deploy with Telebot Creator TPY code!

# Features
•Downloads Reels/Posts in under 1 second         
•HD quality, no watermarks.      
•30s cooldown prevents spam.       
•Auto-detects Instagram URLs.    
•Clean UI with message deletion.     

# 🚀 Deployment Steps

| Step | Action | File Used |
|------|--------|-----------|
| 1 | `@BotFather` → `/newbot` → Copy token | - |
| 2 | [telebotcreator.com](https://telebotcreator.com) → Login → New Bot | - |
| 3 | **Command 1**: Set trigger `/start` → Paste `start_command.tpy` content | `start_command.tpy` |
| 4 | **Command 2**: Set trigger `*` → Paste `url_handler.tpy` content | `url_handler.tpy` |
| 5 | Click **Activate Bot** (should show green status) | Done! |
| 6 | Test: `t.me/YOUR_BOT_USERNAME` → `/start` | ✅ Live |

**Total time: 3 minutes**

## 🔧 Code Features Table

| Feature | File | Description |
|---------|------|-------------|
| **Colorful Welcome** | `start_command.tpy` | Rainbow banner + channel invite button |
| **Smart URL Detection** | `url_handler.tpy` | Regex validates `instagram.com/p`, `/reel`, `/tv` links |
| **30s Rate Limiting** | `url_handler.tpy` | `User.getData("insta_last")` prevents spam |
| **Clean Interface** | `url_handler.tpy` | Auto-deletes user message + loading message |
| **<1s Downloads** | `url_handler.tpy` | `tele-social.vercel.app/down` API (25s timeout) |
| **Video+Photo Auto** | `url_handler.tpy` | Detects `mtype` → `sendVideo()` or `sendPhoto()` |
| **Error Handling** | `url_handler.tpy` | Edits "Downloading..." → "❌ Failed" on error |
| **Branding** | Both | "GREED" + backup channel links everywhere |

Made by BrahmjotCodez(1ttp)
