# If

## If?

javascript의 if처럼 조건문을 만듭니다.

```scss
@mixin pos-center-x($type: absolute) { 
    @if ($type == fixed or $type == absolute) { 
        position: $type; 
        left: 50%; 
        transform: translateX(-50%); 
    } 
}
```

