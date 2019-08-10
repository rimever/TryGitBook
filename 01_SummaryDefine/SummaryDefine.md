# 要件定義書


## 現状

* ExcelやWord

## 課題

* 共有して編集するのが手間
* マージが出来ない


## plantuml

```uml
@startuml

	Class Stage
	Class Timeout {
		+constructor:function(cfg)
		+timeout:function(ctx)
		+overdue:function(ctx)
		+stage: Stage
	}
 	Stage <|-- Timeout

@enduml
```