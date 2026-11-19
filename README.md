# 驗證碼沒交出去，還是到了別人手上：讀區塊勢〈別再用簡訊驗證碼！〉

區塊勢 2026-11-19 影片〈別再用簡訊驗證碼！即便你沒給任何人，它還是會被攔截！〉的深度導讀。這篇導讀整理簡訊驗證碼在電信網路、電信櫃檯、使用者手機三處被讀走的方式，以及驗證器 App 與通行密鑰各擋住哪一段；重要說法對照 Enea、FBI IC3、CISA、NIST、Google、TVBS、中華電信等一手來源。

## 製作聲明

本導讀的分析、撰稿、查證、審稿與插圖皆由 AI 模型完成，不是人類分析，也沒有經過人工逐句校稿。

- 主控與撰稿：Claude Opus 5.5
- 逐字稿：影片沒有字幕軌。由 Claude Opus 5.5 逐張讀取影片畫面上的燒入字幕擷取，再以本機 Whisper 交叉比對；時間軸依畫面字幕切換點偵測。
- 查證：agy（gemini-3.8-flash-high）與 Claude Opus 子代理人各自獨立查證。重要說法須兩方一致且有官方或第一手來源，才寫成確定事實。
- 資安分析：依資安導師框架整理成分析備忘。
- 審稿：兩位 Claude Opus 審稿人分別把關事實、編輯，再由一位 Claude Opus 終審，最後由 Claude Opus 依一份潤稿準則調整語句。
- 圖片：四張流程圖是 SVG 腳本，沒有使用 AI 生圖。分享預覽圖（og-hero.jpg）由第一張流程圖加標題截圖而成。

## 檔案

| 檔案 | 說明 |
|---|---|
| `sms-otp-silentair-passkey.md` | 導讀正文（Markdown） |
| `index.html` | 導讀網頁（可直接用瀏覽器開啟） |
| `player.html` | 中文字幕播放器（嵌入 YouTube，字幕依畫面燒入字幕擷取） |
| `images/` | 四張流程圖 SVG（各有桌面、手機版）、分享預覽圖 og-hero.jpg |
| `share_post.md` | 社群分享文（資安角度） |

## 原始資料

- 影片：區塊勢〈別再用簡訊驗證碼！即便你沒給任何人，它還是會被攔截！重要帳號該換掉簡訊驗證〉，2026-11-19，https://www.youtube.com/watch?v=pA9gXxCqkYQ
- 逐字稿：依影片畫面燒入字幕擷取的 133 句，收在 `player.html` 內；製作過程紀錄（證據帳本、審稿報告）留在本機，不公開

## 重要來源

- Enea：The Enemy Within. Tracking LIMINAL PANDA and SilentAir through Mobile Networks（2026-11-11）https://www.enea.com/insights/the-enemy-within-tracking-liminal-panda-and-silentair-through-mobile-networks/
- CISA：Mobile Communications Best Practice Guidance（2024-12-18）https://www.cisa.gov/sites/default/files/2024-12/guidance-mobile-communications-best-practices.pdf
- NIST SP 800-63B（800-63-4）https://pages.nist.gov/800-63-4/sp800-63b.html
- FBI IC3 PSA220208（2022-02-08）https://www.ic3.gov/PSA/2022/PSA220208
- TVBS（2022-01-31）https://news.tvbs.com.tw/life/1705527
- Google Online Security Blog（2024-02-06）、Google 帳戶說明（Authenticator、密碼金鑰）
- 中華電信新聞稿（2025-07-09）https://www.cht.com.tw/zh-tw/home/cht/messages/2025/0709-1550

## 狀態

已發布（2026-11-19，commit d881796）：https://lushinshang.github.io/sms-otp-silentair-passkey/ ；repo：https://github.com/lushinshang/sms-otp-silentair-passkey
