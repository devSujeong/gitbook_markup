# ๐ช slide up & down

์ ์ด์ฟผ๋ฆฌ ์์ ์์๋ ๋ฉ์๋ ํ๋๋ฉด ํด๊ฒฐ๋์๋ค. `slideup`, `slidedown` ์ผ๋ก ๋ง์ด๋ค. ์ ์ด์ฟผ๋ฆฌ๋ฅผ ์์ฐ๊ธฐ ์์ํ๋ฉด์ ์ด๋ฅผ css๋ก ๊ตฌํํด์ผ๊ฒ ๋๋ฐ ์ฌ์ ํ ์ ๋ชฐ๋๋ค. display์์๋ก ์์ํ๋ ๊ฑด ์ฌ๋ผ์ด๋ฉ์ด ๋์ง ์์ผ๋๊น. ๋ถ๋๋ฝ๊ฒ ์กฐ์ฐจ๋ ๋์ง ์์๋ค. ๊ทธ๊ฒ์ transition์ด ๋์ง ์์ผ๋ฏ๋ก..

## slide์ key "max-height"

height์ด ๋ฐ๋ ์์์ transition, max-height:0, overflow: hidden์ ์ ์ฉํ๋ค.

```scss
content {
    transition: max-height 200ms ease-in-out;
    max-height: 0;
    overflow: hidden;
}
```

์ํ๊ฐ ๋ฐ๋๋ ํด๋์ค๊ฐ ๋ถ์ ๋, ๊ณ์ฐํ max-height๊ฐ์ ๋ฃ์ด์ค๋ค. ์ด ๋, ๊ฐ์ด ๊ณ ์ ์ด๋ผ scss๋ก ๊ณ์ฐํ์ฌ ๋ฃ์ ์ ์๋ค๋ฉด ๊ณ์ฐ๊ฐ์ ๋ณ์ํํ์ฌ ๋ฃ๊ฒ ์ง๋ง, ๋์ด๊ฐ ๊ฐ๋ณํ์ด๋ผ๋ฉด javascript๋ก ๊ฐ์ ๊ณ์ฐํ์ฌ ๋ฃ์ด์ฃผ์ด์ผ ํ๋ค.

```
content {
  &.is-open {
    max-height: _calculate-max-content-height($community-length);
  }
}
```
