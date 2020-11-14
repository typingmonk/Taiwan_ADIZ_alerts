# Taiwan_ADIZ_Records
Collect open records about Taiwan ADIZ(防空識別區) reports around the world.

## 說明
- 每一則紀錄存放在一個 json 檔裡頭，檔名是根據即時軍事動態頁面的 Key 值命名。
- 相片紀錄存放在 img 裡頭，檔名開頭的數字對應即時軍事動態頁面的 Key 值。
- json key 說明：
  - `title`: 記錄標題
  - `title_en`: 同上，改以英文描述，Optional
  - `date`: 記錄日期，僅記錄至日期，不會記錄到事件當下的時間
  - `date_en`: 同上，改以英文描述，Optional
  - `craft_types`: 軍機、飛行器型號
  - `craft_types_en`: 同上，改以英文描述，Optional
  - `map_imgs`: 航線記錄地圖，檔案在 `img` 資料夾裡
  - `reaction`: 台灣國軍反應及處置
  - `reaction_en`: 同上，改以英文描述，Optional
  - `craft_imgs`: 軍機、飛行器的相片紀錄，檔案在 `img` 資料夾裡
  - `source_url`: 資料網址來源

## To do list(lots of)
- 資料清理
  - Format 日期格式
  - 目前 `craft_types` 內包含飛機的架數，尚須分離出來
  - `reaction` 的儲存格式要統一存成 `array`，目前有些是 `string`。

## 資料來源
[中華民國國防部即時軍事動態](https://www.mnd.gov.tw/PublishTable.aspx?Types=%E5%8D%B3%E6%99%82%E8%BB%8D%E4%BA%8B%E5%8B%95%E6%85%8B&title=%E5%9C%8B%E9%98%B2%E6%B6%88%E6%81%AF)
