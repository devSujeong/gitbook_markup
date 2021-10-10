# selector

## placeholder selector

css에 렌더되지 않고, 스타일 속성들을 정의할 수 있는 scss에만 존재하는 특별한 셀렉터입니다. 공통속성들을 placeholder selector에 넣어놓고 불러와 사용하기에 좋습니다.

```scss
%avatar-base { 
display: block; overflow: hidden; border-radius: 50%; background: url(‘../../assets/images/img-user-default.png’) no-repeat center center; background-size: contain;
img { width: 100%; height: 100%; object-fit: cover; } }
.avatar-24 { @extend %avatar-base; width: 24px; height: 24px; }
```

