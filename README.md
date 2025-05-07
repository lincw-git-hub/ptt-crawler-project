
# PTT 熱門文章爬蟲與關鍵詞分析專案

本專案是利用 Python 撰寫的 PTT 爬蟲工具，爬取指定看板的熱門文章，並進行關鍵字統計與視覺化分析（包含長條圖與中文詞雲）。本專案適合對資料爬蟲與文本分析有興趣的新手學習者，專案執行環境為 Jupyter Notebook，使用 macOS 開發。

---

## 📌 使用技術

- Python
- Requests + BeautifulSoup：網頁資料擷取
- Pandas：資料整理與輸出
- Jieba：中文斷詞
- Matplotlib：長條圖視覺化
- WordCloud：中文詞雲圖產生

---

## 📁 專案結構

```
ptt-crawler-project/
├── ptt_scraper.ipynb             # PTT 爬蟲主程式
├── keyword_analysis.ipynb        # 關鍵詞分析
├── visualize.ipynb               # 圖像視覺化
├── NotoSansTC-Regular.otf        # 中文字型（用於詞雲）
├── README.md                     # 本說明文件
└── data/
    ├── articles.csv              # 爬蟲結果 CSV
    ├── top_push.png              # 推文數最多文章圖
    └── wordcloud.png             # 中文詞雲圖
```

---

## 🚀 執行步驟

1. 安裝套件（只需一次）：
   ```bash
   pip install requests beautifulsoup4 pandas jieba matplotlib wordcloud
   ```

2. 依序執行：
   - `ptt_scraper.ipynb` → 爬文章並儲存成 `articles.csv`
   - `keyword_analysis.ipynb` → 分析關鍵字出現頻率
   - `visualize.ipynb` → 畫出圖表與詞雲

---

## 📝 資料來源

本專案以 PTT 批踢踢實業坊的公開網頁資料為分析對象，僅供學術研究與練習用途。

---

## 👩‍💻 作者

by lincw-git-hub
