GitHub 與 BitBucket HTML 預覽
-------------------------------

#### 許多 GitHub 儲存庫並未使用 GitHub Pages 來託管其 HTML 檔案。**GitHub & BitBucket HTML 預覽** 讓您無需克隆或下載整個儲存庫，即可渲染這些檔案。這是一個利用 CORS 代理來擷取資源的客戶端解決方案。

#### 若您嘗試直接從 GitHub 在網頁瀏覽器中開啟任何 HTML、CSS 或 JS 檔案的原始版本，您看到的將僅是原始碼。GitHub 強制這些檔案使用「text/plain」內容類型，因此瀏覽器無法解析它們。此腳本透過使用 CORS 代理伺服器來覆寫此設定。

## 用法(Usage)

#### 若要使用此功能，只需在任何 HTML 檔案的 URL 前加上以下片段：**[https://htmlpreview.github.io/?](https://htmlpreview.github.io/?)** 例如：

 - https://htmlpreview.github.io/?https://github.com/twbs/bootstrap/gh-pages/2.3.2/index.html
 - https://htmlpreview.github.io/?https://github.com/documentcloud/backbone/blob/master/examples/todos/index.html

#### 其運作方式是：先透過 CORS 代理伺服器載入 HTML，接著處理所有連結、框架、腳本及樣式，並透過 CORS 代理伺服器載入這些元素，以便瀏覽器能對其進行解析。

#### **GitHub 與 BitBucket HTML 預覽功能** 已於最新版的 Google Chrome 和 Mozilla Firefox 進行測試。

## 授權(License)

#### &copy;2019 Jerzy Głowacki，採用 Apache 2.0 授權條款。
