# Oploverz Rest API Made by Yuzaki
[`Oploverz Official Website`](https://oploverz.bz)
## **Documentation**
| No | Features | Query | Description |
| :---: | ------ | :------: | :--------: |
| 1 | Homepage | ❌ | Info pembaruan anime |
| 2 | GenreSearch | ✔ | Mencari anime melalui genre | 
| 3 | Search | ✔ | Mencari anime |
| 5 | Popular | ❌ | List Anime-anime dengan rating yang tinggi |
| 6 | Season | ✔ | Mencari anime melalui nama musim |

## **Usage**
```
$ npm i oploverz-scraper
```
#### **Code Example ~ Tanpa Query**
```js
const api = require('oploverz-scraper');

(async () => {
    api.Homepage().then(res => {
        console.log(res);
    })
})()
```
#### **Code Example ~ Query Metode**
```js
const api = require('oploverz-scraper');

(async () => {
    const query = 'zankyou no terror'
    api.Search(query).then(res => {
        console.log(res);
    })
})()
```
#### **Result**
```json
{
  "message": "Sukses!",
  "error": false,
  "data": [
    {
      "judul": "Zankyou no Terror",
      "status": "Completed",
      "studio": "MAPPA",
      "tahun": "2014",
      "durasi": "22 min. per ep.",
      "musim": "Summer 2014",
      "tipe": "TV",
      "jumlahEps": "11",
      "pembaruanTerakhir": "Dirilis pada: Desember 16, 2020",
      "genres": ["Mystery", "Psychological", "Thriller"],
      "rating": "8.13",
      "sinopsis": "Dalam versi alternatif masa kini, Tokyo telah hancur oleh serangan teroris yang mengejutkan, dan satu-satunya petunjuk mengenai identitas pelakunya adalah video aneh yang diunggah ke internet. Polisi bingung dengan petunjuk yang masih samar ini, dan tak berdaya menghentikan paranoia (ketakutan berlebihan) yang menyebar pada seluruh penduduk. Sementara itu, saat dunia mencari dalang kriminal yang harus bertanggung jawab atas tragedi ini, dua anak misterius yang seharusnya tak pernah ada, memiliki keahlian dalam melaksanakan rencana keji mereka. Perbuatan yang dikutuk oleh dunia ini dan mereka menyebut diri mereka Nine dan Twelve, dua orang tersebut bergabung  membentuk “Sphinx,” kegelapan  untuk membangunkan orang-orang dari tidur mereka 
dan menarik ancaman pada dunia ini.",
      "thumb": "https://i2.wp.com/oploverz.bz/wp-content/uploads/2020/12/Zankyou-no-Terror-Sub-Indo.jpg",
      "url": "https://oploverz.bz/anime/zankyou-no-terror/"
    }
  ]
}
```
## **Terima kasih telah berkunjung!**
[![NPM INSTALL](http://img.shields.io/badge/npm-install-blue.svg?style=flat&logo=npm)](https://docs.npmjs.com/getting-started/installing-npm-packages-locally) ![NODE JS](http://img.shields.io/badge/Node-JS-teal.svg?style=flat&logo=node.js)

* [`Buy Me A Coffee☕ ~ Saweria`](https://saweria.co/Natsu062)