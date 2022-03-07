# Fitur bot
[![fitur-bot](https://github-readme-stats.vercel.app/api/pin/?username=MuhammadRestu999&repo=fitur-bot)](https://github.com/MuhammadRestu999/fitur-bot)

## List
- [Atas](#fitur-bot)
- [List](#list)
- [Deskripsi](#deskripsi)
- [Penggunaan](#penggunaan)
  - [NodeJS](#nodejs)
  - [Python](#python)
- [Kontribusi](#kontribusi)

## Deskripsi
Fitur-fitur yang dapat digunakan untuk bot / web api

## Penggunaan
### NodeJS
Install modul axios / node-fetch dulu<br>
Disini saya akan menggunakan axios<br>
```bash
npm install axios
```

File katakata.js :
```javascript
let axios = require("axios");
let result = {};
axios.get("https://raw.githubusercontent.com/MuhammadRestu999/fitur-bot/main/random/text/KataKataAnime.json").then((res) => {
  result = res.data[Math.floor(Math.random() * res.data.length)]
});
console.log(result);
```

Jalankan dengan perintah
```bash
node katakata.js
```

### Python
Install requests
```bash
pip install requests
```

File katakata.py :
```python
import requests
from random import choice

res = requests.get("https://raw.githubusercontent.com/MuhammadRestu999/fitur-bot/main/random/text/KataKataAnime.json")
json = res.json()
result = choice(json)

print(result)
```
Jalankan dengan perintah
```bash
python katakata.py
```

## Kontribusi
1. (Tidak ada)
