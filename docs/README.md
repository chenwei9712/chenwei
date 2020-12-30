# 1年度充值汇总

> 支持表格以excel、csv下载

>  1.1获取表格字段

 - URL:`./api/chargeIncomePercent/GetGYSStructField`

+ 方法：GET

+ response：

  成功：

  ```json
  {
      "code": 0,
      "data": [
          "id",
          "gid",
          ...
      ],
  }
  ```

  失败：

  ```json
  {
      "code": 7,
      "data": {
          "reload": true
      },
      "msg": "未登录或非法访问"
  }
  ```

> 1.2根据字段选中字段 下载数据

+ URL:`./api/chargeGameYearSummary/downloadChargeGameYearSummaryList?field=gid&field=game_name&filename=good.xlsx&type=xlsx`

+ 方法：GET

+ body：

  ```json
  {
      "filename": 	"new.xlsx",| "new.csv"
      "field":		["id","gid",...],
      "type":		"xlsx" | "csv"
  }
  ```

# 2道具收入月度汇总

> 支持表格以excel、csv下载

>  2.1获取表格字段

 - URL:`./api/chargeIncomePercent/GetCIPStructField`

+ 方法：GET

+ response：

  成功：

  ```json
  {
      "code": 0,
      "data": [
          "id",
          "gid",
          ...
      ],
  }
  ```

  失败：

  ```json
  {
      "code": 7,
      "data": {
          "reload": true
      },
      "msg": "未登录或非法访问"
  }
  ```

> 2.2根据字段选中字段 下载数据

+ URL : `./api/chargeGameYearSummary/chargeIncomePercent?field=gid&field=game_name&filename=good.csv&type=csv`

+ 方法：GET

+ body：

  ```json
  {
      "filename": 	"new.xlsx",| "new.csv"
      "field":		["id","gid",...],
      "type":		"xlsx" | "csv"
  }
  ```





