# 花蓮慈濟醫院 公共傳播室

**線上網址：** https://petertseng0517.github.io/hlm-pc/

花蓮慈濟醫院公共傳播室的對外品牌首頁與院內工具平台，同時整合 Joomla 網站管理教學文件。
- [Joomla教育訓練簡報](https://gamma.app/docs/-hkiod2cqkwmqfme)
---

## 頁面結構

| 頁面 | 路徑 | 說明 |
|---|---|---|
| 品牌首頁 | `/` | 公傳室對外形象頁，含載入動畫、霧氣特效、作品展示 |
| 公傳服務總覽 | `/pc.html` | 院內同仁服務窗口（需院內網路） |
| 傳播成效儀表板 | `/dashboard.html` | YouTube、社群、GA 統計數據 |
| Joomla 教學文件 | `/joomla_study/` | 醫院官網管理教學（MkDocs 生成） |
| 圖片轉 WebP 工具 | `/tools/image-to-webp.html` | 上傳前裁切並轉換格式 |
| 網站管理後台入口 | `/web-admin.html` | Joomla 後台連結頁 |

---

## 品牌首頁功能

- **載入動畫**：「報真導正」毛筆字 → Logo → 四角直線畫出 → 進入頁面
- **Hero 區**：院區實景照片 + 多層飄動霧氣動畫
- **敘事段落**：人文紀錄 / 慈濟人文 / 研究與成就（視差捲動）
- **公傳成果**：40 周年慶專網、醫療科技展、YouTube 頻道、VR 虛擬導覽、[員工特約廠商查詢](https://hlm.tzuchi.com.tw/store/)（LINE@ 綁定 + Lotus Notes COM 同步）
- **服務入口**：公傳服務總覽 / Joomla 教學 / 傳播成效儀表板

---

## 傳播成效儀表板

- **YouTube 訂閱人數**：透過 YouTube Data API v3 即時拉取（頻道 ID：`UC4cGxfjbE0dPnBOhHo0igTA`）
- **社群媒體**：FB 粉絲數、IG 追蹤數（手動更新）
- **年度業務量**：新聞稿、媒體露出、影片製作、攝影服務、設計案件、活動場次（手動更新）
- **GA 流量**：待連結 Looker Studio 嵌入報表

---

## Joomla 教學文件

使用 [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) 建置，內容位於 `docs/` 目錄。

**適用對象**

| 部門 | 教學內容 |
|---|---|
| 所有管理者 | 帳號申請、登入、文章編輯、圖片與連結 |
| 醫務部 | 醫療科首頁、醫師資料、衛教、最新消息 |
| 醫事室 | 門診表更新、疫苗公告 |
| 總務室 | 招標公告、樓層介紹 |

**本地預覽**

```bash
pip install mkdocs-material
mkdocs serve
```

---

## 技術架構

- **靜態網站**：GitHub Pages 託管
- **教學文件**：MkDocs + Material Theme
- **字型**：Cormorant Garamond、Noto Serif TC、Ma Shan Zheng（Google Fonts）
- **YouTube API**：Data API v3，限制 HTTP referrer 為本站網域

---

## 聯絡

花蓮慈濟醫院 公共傳播室 · peter.qfx@gmail.com
