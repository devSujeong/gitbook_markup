# 🪂 show & hide

## case

검정색 반투명 배경처럼, 요소의 공간을 그대로 차지하고 있어도 레이아웃의 문제가 없는 경우에는 `visibility`를 활용해서 `transition`으로 `animation`을 구현할 수 있습니다. `display`는 `transition`이 되지 않습니다.

```scss
.overlay {
  position: fixed;
  top: 0;
  left: 0;
  z-index: $overlay-level;
  width: 100%;
  height: 100vh;
  background: rgba($primary, 0.5);
  opacity: 0;
  visibility: hidden;

  &.is-active {
    transition: opacity 300ms ease-in-out, visibility 300ms ease-in-out;
    opacity: 1;
    visibility: visible;
  }
}

```
