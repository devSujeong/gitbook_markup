# πͺ show & hide

## case

κ²μ μ λ°ν¬λͺ λ°°κ²½μ²λΌ, μμμ κ³΅κ°μ κ·Έλλ‘ μ°¨μ§νκ³  μμ΄λ λ μ΄μμμ λ¬Έμ κ° μλ κ²½μ°μλ `visibility`λ₯Ό νμ©ν΄μ `transition`μΌλ‘ `animation`μ κ΅¬νν  μ μμ΅λλ€. `display`λ `transition`μ΄ λμ§ μμ΅λλ€.

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
