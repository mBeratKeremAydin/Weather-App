# Weather app (HTML, CSS, JavaScript)

A small single-page weather app: type a city name and it shows the current temperature (°C), humidity and wind speed, with an icon for the weather type. The data comes from the [OpenWeatherMap](https://openweathermap.org/) current-weather API, called from the browser with `fetch`.

## Setup

1. Get a free API key from OpenWeatherMap.
2. Copy `config.example.js` to `config.js` and put your key in it. `config.js` is git-ignored, so the key stays out of the repository.
3. Add the icon images the page references under `images/`: `clear.png`, `clouds.png`, `drizzle.png`, `humidity.png`, `mist.png`, `rain.png`, `search.png`, `wind.png`. They are not included in this repository.
4. Open `index.html` in a browser.

## Notes

- The key is used in the browser, so anyone who can open a deployed copy of the page can read it. Do not deploy this page publicly with a personal key; restrict or rotate the key if you do.
- Only the weather types Clouds, Clear, Rain, Drizzle and Mist have an icon; other types keep the previous icon.
- Only a 404 response is handled as "city not found".

## Türkçe özet

Şehir adı yazınca anlık sıcaklık, nem ve rüzgar hızını gösteren küçük bir hava durumu sayfası (OpenWeatherMap API). API anahtarı koda gömülü değildir: `config.example.js` dosyasını `config.js` olarak kopyalayıp kendi anahtarınızı yazın (`config.js` git'e eklenmez). İkon görselleri bu depoda yoktur.
