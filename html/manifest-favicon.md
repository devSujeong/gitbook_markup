# manifest, favicon

## manifest란?

모바일 시대가 오면서 웹도 앱처럼 보이기 위해 파비콘 이상의 다양한 대응책들이 필요해졌습니다. 애플과 구글의 자체적인 방법들이 나오다가 web app manifest file로 정리되었습니다.

```markup
<link rel="manifest" href="manifest.json">
```

## Manifest file

```javascript
{
  "name": "HackerWeb",
  "short_name": "HackerWeb",
  "start_url": ".",
  "display": "standalone",
  "background_color": "#fff",
  "description": "A simply readable Hacker News app.",
  "icons": [{
    "src": "images/touch/homescreen48.png",
    "sizes": "48x48",
    "type": "image/png"
  }, {
    "src": "images/touch/homescreen72.png",
    "sizes": "72x72",
    "type": "image/png"
  }, {
    "src": "images/touch/homescreen96.png",
    "sizes": "96x96",
    "type": "image/png"
  }, {
    "src": "images/touch/homescreen144.png",
    "sizes": "144x144",
    "type": "image/png"
  }, {
    "src": "images/touch/homescreen168.png",
    "sizes": "168x168",
    "type": "image/png"
  }, {
    "src": "images/touch/homescreen192.png",
    "sizes": "192x192",
    "type": "image/png"
  }],
  "related_applications": [{
    "platform": "play",
    "url": "https://play.google.com/store/apps/details?id=cheeaun.hackerweb"
  }]
}
```

* name: 웹어플리케이션의 이름
* short\_name: 짧은 웹어플리케이션 이름
* display: 유저에게 보여지길 원하는 형식. fullscreen \| standalone \| minimal-ui \| browser\(default\)
* background\_color: 스타일시트가 적용되기 전에 보일 배경색
* description: 웹어플리케이션에 대한 설명
* icons: 다양한 어플리케이션 상황 별로 대응할 이미지 아이콘.

