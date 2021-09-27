# 설치 및 사용법

## Node-sass

node환경에서 sass를 사용할 수 있게 해주는 라이브러리.

> node-sass \[options\] &lt;input url&gt; &lt;output url&gt;

* -w: styles/main.scss의 변경이 생기면 자동으로 style.css로 변환시켜 줌.
* -r: 잘 모르겠는데 w할 때 같이 쓰는 것 같음...
* --source-map true: 개발자도구에서 컴파일 된 css말고 어디 scss파일에서 온 것인지 알려

```bash
node-sass -wr --source-map true styles/main.scss style.css
```

