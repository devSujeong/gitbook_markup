# 🪂 sidebar left

## sidebar

sidebar에서 화면 밖으로 나갔다가 active 상태에서는 화면 안으로 들어오는 것을 구현할 때, 그래픽 카드의 가속을 위해서 3d로 사용하는 게 한끗 차이입니다.

```
.sidebar {
    transform: translate3d(-#{$sidebar-width}, 0, 0);
    transition: transform 300ms ease-in-out;
    
    &.is-active {
        transform: translate3d(0, 0, 0);
    }
}
```
