# 動領領養平台 🐾

一個以「領養代替購買」為核心理念的動物領養平台，旨在提供使用者友善、透明的流浪動物資訊，促進更多溫暖的收養行為。

---

## 📌 專案簡介

本平台是一個基於 **PHP + MySQL** 架構開發的動物領養網站，整合前後端功能，提供完整的會員與動物管理功能。包含訪客導覽、會員系統、領養刊登、後台控管等模組。

- **首頁 (animals.html)**：介紹領養理念、領養流程、推薦影片，建立用戶對「領養」的認同與行動意願。
- **公立領養頁 (animal_data.html)**：整合公立收容所資料，提供縣市 / 性別 / 種類篩選功能，並以卡片形式展示動物資訊。
- **領養認養頁 (adopt_list.html)**：由有送養需求的民眾上傳後整合的頁面。
- **領養刊登管理頁 (adopt_manage.html)**：送養寵物上傳頁面,此頁面需登入後才會出現。
- **後臺控制-使用者管理頁面 (animember.html)**：管理使用者資訊及角色。
---
### 首頁（理念介紹與影音推薦）
![首頁截圖](images/首頁.png)

---

### 公立動物領養頁（篩選功能 + 卡片列表）
![公立領養頁](images/screenshot-animal-list.png)

---

### 註冊與登入彈窗（含 SweetAlert2 驗證提示）
![註冊登入](images/screenshot-login-register.png)

---

### 會員管理後台（管理員專用）
![會員管理](images/screenshot-admin-member.png)

---

### 領養刊登管理頁（會員專屬）
![刊登管理](images/screenshot-adopt-manage.png)

## 🔐 核心功能

### 👤 會員系統
- 註冊 / 登入 / 登出（帳號長度與 Email 驗證）
- 帳號重複檢查
- 角色區分（user / admin）
- 使用 Cookie 管理登入狀態

### 🏠 前台功能（訪客 & 會員）
- 動物列表：以卡片顯示詳細資訊（照片、性別、絕育狀態、收容所資訊）
- 篩選功能：依「縣市 / 性別 / 種類」即時過濾
- 影音推薦：YouTube 嵌入式影片說明領養觀念
- 領養流程圖解說明
- 註冊/登入 Modal 彈窗互動提示

### 🛠️ 會員後台功能
- **領養刊登管理**（一般會員）：
  - 上傳 / 編輯 / 刪除自己刊登的動物資料
- **後台管理系統**（管理員）：
  - 顯示會員列表（由 `ani_get_members.php` 提供）
  - 即時搜尋功能（依帳號 / Email）
  - 編輯會員資料（`ani_update_members.php`）
  - 刪除會員帳號（`ani_delete_members.php`）

---

## 🔧 使用技術

### 🖥️ 前端

- **HTML / CSS**：
  - Bootstrap 5（響應式設計）
  - 自訂樣式 `myall.css`, `color.css`
  - Font Awesome（圖標）
  - Animate.css + WOW.js（動畫效果）

- **JavaScript**：
  - jQuery（事件監聽與 AJAX）
  - Bootstrap Bundle（Modal 與下拉選單）
  - SweetAlert2（提示視窗）
  - CounterUp2（數字動畫）

### 🔙 後端

- **PHP**：
  - API 控制（登入、註冊、查重、會員管理）
  - 動物資料 CRUD 操作

- **MySQL**：
  - 資料庫名稱：`animal`
  - 資料表：
    - `member`：會員資訊
    - `adopt_animals`：領養動物資料

### 🔄 其他

- **AJAX**：前後端即時資料傳遞
- **FormData**：表單與圖片上傳
- **Cookie**：登入驗證與角色判斷
- **Cloudflare**：安全與快取優化（如部署時使用）

---

## 📂 聯絡方式

陳芷柔  
GMAIL:zhirou022@gmail.com
📫 歡迎合作或交流！
