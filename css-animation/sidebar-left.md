# πͺ sidebar left

## sidebar

sidebarμμ νλ©΄ λ°μΌλ‘ λκ°λ€κ° active μνμμλ νλ©΄ μμΌλ‘ λ€μ΄μ€λ κ²μ κ΅¬νν  λ, κ·Έλν½ μΉ΄λμ κ°μμ μν΄μ 3dλ‘ μ¬μ©νλ κ² νλ μ°¨μ΄μλλ€.

```
.sidebar {
    transform: translate3d(-#{$sidebar-width}, 0, 0);
    transition: transform 300ms ease-in-out;
    
    &.is-active {
        transform: translate3d(0, 0, 0);
    }
}
```
