# 🪂 slide up & down

제이쿼리 시절에서는 메서드 하나면 해결되었다. `slideup`, `slidedown` 으로 말이다. 제이쿼리를 안쓰기 시작하면서 이를 css로 구현해야겠는데 여전히 잘 몰랐다. display요소로 작업하는 건 슬라이딩이 되지 않으니까. 부드럽게 조차도 되지 않았다. 그것은 transition이 되지 않으므로..

## slide의 key "max-height"

height이 바뀔 요소에 transition, max-height:0, overflow: hidden을 적용한다.

```scss
content {
    transition: max-height 200ms ease-in-out;
    max-height: 0;
    overflow: hidden;
}
```

상태가 바뀌는 클래스가 붙을 때, 계산한 max-height값을 넣어준다. 이 때, 값이 고정이라 scss로 계산하여 넣을 수 있다면 계산값을 변수화하여 넣겠지만, 높이가 가변형이라면 javascript로 값을 계산하여 넣어주어야 한다.

```
content {
  &.is-open {
    max-height: _calculate-max-content-height($community-length);
  }
}
```
