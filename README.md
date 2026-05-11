# Weegle: Domain-Specific Search Engine for Wego School | 薇閣校園資訊搜尋引擎

"Weegle" is a specialized search engine designed to solve the keyword ambiguity problem associated with "Wego" (薇閣). While standard search engines often mix results from boutiques, hotels, and care centers, Weegle uses custom filtering and weighting algorithms to provide high-relevance data specifically for Taipei Wego Private Senior High School.
「Weegle」是一款針對「薇閣」關鍵字設計的專用搜尋引擎。解決了通用搜尋引擎在處理歧義詞時的痛點（如：薇閣精品旅館、薇閣產後護理之家），透過自定義過濾與權重演算，精準呈現與薇閣中學相關的學術、入學及新聞資訊。

> **程式設計課程專案 · Final Project Report · Group 10**

---

## 🎯 Objective | 分析目標
The primary goal is to save time for students and parents by filtering out "noise" (irrelevant commercial data) and rearranging search results based on academic relevance. It aims to reduce the chance of missing important school announcements due to search engine clutter.
核心目標是為學生與家長節省篩選資訊的時間。透過過濾無關的商業數據（如旅館、服飾店），並根據學術相關度重新排列搜尋結果，確保使用者不會在雜亂的搜尋結果中遺漏重要的學校公告。

---

## 🛠 Pipeline | 處理流程
1. **Keyword Ambiguity Analysis:** Identifying common irrelevant search results for "Wego" (e.g., Wego Boutique Hotel, Wego Clothing). / 歧義分析：識別搜尋「薇閣」時常見的無關結果。
2. **Data Collection:** Using web crawlers to collect and count keyword frequencies from various web pages. / 資料收集：使用爬蟲收集各網頁資訊並統計關鍵字頻率。
3. **Weighting & Scoring:** Implementing an algorithm to score websites based on school-related keyword density. / 權重評分：實作演算法，根據校園相關關鍵字的密度對網頁進行評分。
4. **Result Filtering:** Pre-pending school-specific terms to search queries to grasp domain-related data. / 結果過濾：在搜尋字串中加入特定詞彙以精準抓取校園數據。
5. **GUI Implementation:** Developing a user-friendly search interface ("Weegle") for data presentation. / 介面開發：設計易於操作的 "Weegle" 搜尋介面。

---

## 💻 Tech Stack | 技術棧
* **Programming Language:** Python / Java (as per course environment)
* **Techniques:** Web Scraping (Crawler), Keyword Weighting Algorithm, GUI Design
* **Algorithms:** Relevance Scoring, Data Filtering

---

## 🧠 Key Challenges & Solutions | 核心挑戰與對策
* **Q: How to filter out irrelevant "Wego Boutique Hotel" results?**
  * **A:** We pre-processed the search queries and used a domain-specific filter to ensure the crawler only focused on "Taipei Wego Private Senior High School."
* **Q: How to rearrange results by importance?**
  * **A:** We assigned different weights to keywords. Websites with higher frequencies of academic terms (e.g., "admission," "student," "senior high") were ranked higher in the results.

---

## 👥 Team Members | 團隊成員
* **黃筠茜 (Athena Huang)**
* **楊鵑慈**
* **黃慧如**
* **花巧臻**
* **黃任謙**

---

## 中文簡介
本專案為程式設計課程之期末作品，旨在開發一款垂直領域的搜尋引擎「Weegle」。動機來自於組員身為薇閣中學校友的親身經歷：在網路上搜尋母校資訊時，往往會被「薇閣精品旅館」或「薇閣產後護理之家」等無關訊息淹沒。我們透過建立自定義的關鍵字權重系統，對爬取到的資料進行評分與重新排序，確保搜尋結果的前幾頁皆為家長與學生真正需要的校園新聞、入學資訊及活動公告。
