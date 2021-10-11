# scroll

## scroll bar style control

검색하면 여러 가지가 나온다. 스크롤을 없애는 방식은 아래와 같다.

```scss
::-webkit-scrollbar {
    display: none;
}
```

## overscroll 제어

스크롤이 될 때, (특히 slidebar 같은 경우) 해당 컨텐츠 안에서 스크롤을 하면 그 안에서만 스크롤이 되고 배경까지 스크롤이 넘어가지 않도록 하기 위한 css이다. 그러나 그 컨텐츠 밖에서 스크롤 하는 것은 제어할 수 없다.

```scss
overscroll-behavior: contain;
```

