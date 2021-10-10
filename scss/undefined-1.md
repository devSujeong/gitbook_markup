# 사용하기 좋은 자잘한 룰

## @content

확장해서 다른 곳에서 사용할 때 외부 스타일 요소를 받아옴. react의 children같은 녀석

```scss
@mixin responsive($screen) { 
    @if ($screen == ’T’) { 
        @media screen and (min-width: $md-breakpoint) { 
            @content;
        }
    }
}
```

## type-of

‌ 파라미터 값을 scss의 타입으로 변환합니다.

```scss
@debug type-of(red) == color // true
```
