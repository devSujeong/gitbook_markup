# Mixin

## Mixin

‌mixin은 재사용 가능한 스타일을 정의하여 사용하는 것입니다. @mixin으로 정의하여 함수처럼 만들어 사용하고(리턴은 없다) @include로 불러와 사용할 수 있습니다. 파라미터의 : 값으로 기본 값을 설정할 수 있습니다.

```scss
@mixin flexbox($jc: center, $ai: center) { 
    display: flex; 
    justify-content: _get-flex-value($jc);
    align-items: _get-flex-value($ai); 
}

.name {
    @include flexbox(start);
}
```

