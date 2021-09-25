# 색 활용법

## currentColor

fill 값에 currentColor를 넣어주면 svg를 감싼 태그에 색 정보를 넣어줬을 때 그 색으로 바뀔 수 있다.

```markup
<svg width="130" height="38" viewBox="0 0 130 38" fill="none" xmlns="http://www.w3.org/2000/svg">
<path 
    d="M27.7009 1V15.0984H22.4064V1.20492H18.826V35.3852H22.4064V18.9098H27.7009V36H31.2813V1H27.7009ZM4.6947 30.3033V2.18853H1V33.9098H8.46558C11.3985 33.9098 14.5218 33.459 16.4644 32.5574V28.9508C14.4838 29.7705 11.6651 30.3033 8.88457 30.3033H4.6947Z" 
    fill="currentColor"
/>
</svg>
```

