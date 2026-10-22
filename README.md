# Wingswind 工作成果網站

公開靜態網站。旅遊網站 wi-trip 維持獨立。

## 目錄

- public/index.html：工作成果入口。
- public/taoyuan-corridor/：桃園路廊六點現勘。
- 未來專案以 public/<project-slug>/ 增加，再更新首頁連結。

## Cloudflare Pages

建立獨立Pages專案（建議名稱 wi-work），連接 wingswinding/Wi，正式分支 main。
Framework preset：None；Build command：留白；Build output directory：public。
首次部署成功後，在 Custom domains 加入 work.wingswind.org，依畫面建立DNS並等待HTTPS生效。
最終網址規劃：https://work.wingswind.org/taoyuan-corridor/ 。設定前不可視為已上線。

首頁與現勘網頁公開瀏覽；筆記只保存在各人的瀏覽器，可匯出文字或列印，不會跨使用者同步。
發布內容只包含展示網頁及必要圖片，未包含原始GIS、專案備份、權屬或內部分析紀錄。

## 本機預覽

在儲存庫目錄執行：python -m http.server 8000 --directory public
瀏覽 http://localhost:8000/ 。無須建置、API金鑰或後端。

Cloudflare Pages專案wi-work已建立，Git來源為本儲存庫main分支；自訂網域設定狀態須以Cloudflare為準。
