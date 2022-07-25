```docker-compose up```


### swagger-editorで確認する方法

```npm install -g @apidevtools/swagger-cli```

ファイルを分割して記述しているため、以下のコマンドでファイルを結合させる

```swagger-cli bundle api/openapi.yaml --outfile _build/openapi.yaml --type yaml```

localhost:8082へ移動し、Import fileを選択。結合させたファイルを読み込んでもらう。

<img width="1325" alt="スクリーンショット 2022-07-26 7 45 13" src="https://user-images.githubusercontent.com/81734783/180886969-a54ad654-f3dd-4eb4-ab0f-d920a1625697.png">


| service | url 
|:-----------|------------
| swagger-ui| localhost:8081
| swagger-editor| localhost:8082
| swagger-api | localhost:8003

