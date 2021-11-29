# F2E-WEEK3 全台公車動態時刻查詢應用服務

## [GitPage頁面連結](https://th1230.github.io/F2E-WEEK3/)

## 使用的相關工具以及框架

#### 框架
* angular 

#### 地圖工具&圖資
* leaflet 
* 圖資mapbox

#### github上傳工具
* angular-cli-ghpages [npm連結](https://www.npmjs.com/package/angular-cli-ghpages)

#### 使用的OpenAPI 
* TDX運輸資料流通服務 [API連結](https://tdx.transportdata.tw/api-service/swagger)

## 網頁結構

#### 頁面簡介

1. home(為初始頁面，搜尋會分別通過route跳轉至各個分頁顯示)
2. bus-info(為公車的主要顯示畫面，可以通過點擊站牌(地圖左側的站點圖標--不是在地圖裡)跳轉至stop-info頁面)
3. road-bus-info(為公路客運顯示頁面)
4. stop-info(為站牌的主要顯示畫面，顯示經過此站牌的路線，通過點擊路線圖標可跳轉至公車頁面)

#### 組件分類

1. 頁面組件-----page資料夾
2. 其他組件-----components資料夾

#### api管理(使用angular service)

* api-manager.server.ts檔案中

#### other service

1. /page/home/apidata-store.service.ts-----用於管理主頁home與其他頁面的資料
2. /components/map/map-data-service.ts-----用於將搜尋後的資料傳輸至map組件並管理

#### interceptor

* 主要為所有api加上header

#### 圖片

* 所有靜態圖片放置在assets/images中

## 心得

##### 非常開心能夠完賽，在過程中遇到不少問題，花了很多時間去處理，從week1~week3每一個實作都花費我整週的時間，但這讓我感到很充實並且也讓我對angular這格框架的使用更加的熟悉，希望下次的f2e還有即會再次參加!!!!
