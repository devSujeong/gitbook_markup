# Map

## Map이란

‌ $변수명: ( key: value, …) 형태로 사용합니다. javascript의 객체 느낌입니다.

```scss
$flex-map: ( 
    start: flex-start, 
    end: flex-end, 
    center: center, 
    stretch: stretch, 
    between: space-between, 
    around: space-around
);
```

## 활용

‌ map-get함수를 이용하면 맵의 키를 가지고 밸류를 얻을 수 있습니다.

```scss
map-get($flex-map, start);
```
