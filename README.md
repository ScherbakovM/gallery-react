
# Реакт галерея   

![image](https://github.com/ScherbakovM/gallery-react/assets/109952823/bce095ca-3d7b-4875-b1d8-e7ea483b4b7e)   

## При загрузке страницы фото загружаются c json-servera 
## Так же можно загрузить фото добавив ссылку на фото

### для того чтобы  json-server заработал необходимо выполнить его установку   
```
npm install -g json-server
```

### В package.json добавляем скрипт для запуска сервера 

```
"server": "json-server -w server/db.json -p 4200"
```

### Чтобы одновременно запустить сервер и реакт приложение устанавливаем [concurrently](https://www.npmjs.com/package/concurrently)

### После этого обновляем package.json, добавляем скрипт который обьеденит запуск реакт приложения и json-servera

```
"start": "concurrently \"npm run dev\" \"npm run server\"",
```
![image](https://github.com/ScherbakovM/gallery-react/assets/109952823/3fd099fc-ab91-4729-af3f-dc0b31cc1fc6)
