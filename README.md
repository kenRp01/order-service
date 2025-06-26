# order-service

## 参考
https://www.youtube.com/watch?v=vdAkGFCq-M4&list=PLSVW22jAG8pDeU80nDzbUgr8qqzEMppi8&index=3&ab_channel=ProgrammingTechie

## はまったポイント
* propertiesファイルに書いているmysqlパスワードが誤っていた
* flywayで一度誤った環境を作成してしまい、リセットするのが手間取った
mvn flyway:repair -Dflyway.url=jdbc:mysql://localhost:3306/order_service -Dflyway.user=root -Dflyway.password=mysql
* init.sqlで誤ったテーブルを作成した際に削除に困った(workbenchで消した)
