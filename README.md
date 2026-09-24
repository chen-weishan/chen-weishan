### 陳維杉 Vincent Chen

**Java 後端工程師**｜Spring Boot · Spring Security · Angular 19 · PostgreSQL / MySQL

我寫 Spring Boot 後端，也用 Angular 串自己的 API。下面三個專案都是公開 repo，可以直接看程式碼跟 commit 紀錄。
2026/10/15 職訓結訓，10/16 起可全職到職。

---

#### 關於我

- **學歷**：國立臺南大學 生物科技學系 學士
- **職訓**：Java 全端整合實務運用就業養成班（2026/05～2026/10）
- **寫程式以前**：威秀影城影廳巡檢（輪班、定時讀值、固定用語回報、當班紀錄與交接）。杏一醫療用品門市，處理血壓計、血糖機與復健輔具的售後判斷
- **英文**：多益 850（2022/01）
- **所在地**：台南市／新北市，兩地都可到職

#### 技術

| 類別 | 使用過的 |
|---|---|
| 語言 | Java 21、TypeScript、SQL |
| 後端 | Spring Boot、Spring Security（JWT 流程自建）、Spring Data JPA、JdbcClient、Gradle |
| 資料庫 | MySQL 8、PostgreSQL（Supabase）、Flyway、最小權限角色設計 |
| 前端 | Angular 19、RxJS、Reactive Forms、Tailwind CSS、Angular Material |
| 測試 | JUnit 5、Mockito、Testcontainers |
| 工具 | Git（Conventional Commits）、Docker、Postman、Eclipse、VS Code |

#### 專案

[**AI 選品輔助系統（後端）**](https://github.com/chen-weishan/ai-products-selection-backend)｜五人團隊，我負責評分引擎與情境權重<br>
Spring Boot · PostgreSQL · Flyway
- 模型只能從四組具名權重擇一，不能自己填數值。連續數值沒辦法人工審核，也重現不了。
- 共用資料庫出過一次全組起不來的事故。之後我把日常連線改成最小權限角色，並用 Testcontainers 從 V1 重建驗證。
- 我把排行頁的讀取改用 JdbcClient 手寫 SQL，避開 JPA 的 N+1。寫入仍走 JPA。

[**dynamic-survey**](https://github.com/chen-weishan/dynamic-survey)｜個人專案｜[Demo 影片](https://youtu.be/Ehe9MjT852c)<br>
Spring Boot · Angular 19 · Tailwind CSS · MySQL
- 我沒用現成的 starter，自己寫了 JwtUtil、JwtAuthFilter、SecurityConfig 來做 JWT 驗證。
- GlobalExceptionHandler 搭自訂 BizException，把回應格式跟錯誤碼收成一份契約。

[**Expense-Splitter**](https://github.com/chen-weishan/Expense-Splitter)｜個人專案<br>
純 Java，無框架
- 金額全程 BigDecimal。除不盡的那一分錢由 RemainderStrategy 決定歸屬，新增規則不用動計算流程。
- 零和稽核：所有人的餘額加總恆為零，不成立就擋下來。

#### 我寫程式的習慣

- 讀跟寫可以用不同工具，看查詢長什麼樣子再選。
- 出過事故的地方，我會把規則寫成文件。下一個接手的人只能靠文件，沒辦法靠問我。
- 用 AI 協作時，我會先定好哪些事它不能決定。

#### 聯絡

ia910928@gmail.com ｜ [LinkedIn](https://www.linkedin.com/in/chen-weishan) ｜ [CakeResume](https://www.cake.me/me/vincent-fb0340)
