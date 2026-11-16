# family-timezone

三地視訊時間協調器（🇺🇸 底特律・🇩🇪 漢諾威・🇹🇼 台北）。

- **下次視訊公告**：頁面頂部顯示 `schedule.json` 裡的下次時間，三地同時換算（Poyao 更新 JSON，家人打開就能看到）
- **自由換算**：任一地輸入日期時間，其他兩地自動同步；夏令／冬令時間自動處理（`Intl.DateTimeFormat`）
- 24 小時色條：綠＝適合視訊、黃＝有點早／晚、灰＝睡覺時間

## 用法

打開 <https://poyao-wang.github.io/family-timezone/> 即可。

`schedule.json` 欄位：

```json
{
  "next": "2026-11-20T15:30",   // 下次視訊時間（tz 欄位所指時區的當地時間）
  "tz": "Europe/Berlin",        // next 所用的時區（IANA 名稱）
  "note": "任意備註"             // 可省略
}
```

純靜態頁面，無後端、無追蹤、無上傳。
