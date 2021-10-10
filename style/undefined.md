# 말줄임

## Use case

말줄임표는 타이틀이나 설명 글들을 보여줄 때, 어느 영역을 벗어나면 말줄임표로 표시하는 기법을 말합니다. 말줄임표를 이용하여 깨지지 않는 레이아웃을 만들어봅시다:)

## case: 한 줄 말줄임

```scss
.username {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
}
```

‌ 무조건 한 줄로 나타내야 하므로 white-space 를 nowrap으로 설정하여 줄바꿈을 못하게 합니다. overflow: hidden은 영역을 벗어나 한 줄로 늘어난 글을 내가 설정한 영역까지만 보이도록 하는 기능이며, 글자가 넘치는 부분은 말줄임표로 표시하기 위해 text-overflow를 ellipsis로 설정합니다.

만일, 부모가 flex인 경우에 overflow가 동작하지 않을 수 있습니다. 이때는, 해당 요소에 min-width:0을 주면 의도대로 동작합니다. 왜 동작하는지까지는 모르겠습니다. ‌

## case: 두 줄 말줄임

```scss
.two-line{
    display:-webkit-box;
    -webkit-line-clamp:3;
    -webkit-box-orient:vertical;
    width:200px;
    height:40px;
    line-height:20px;
    overflow:hidden;
    text-overflow:ellipsis;
}
```

두 줄 이상은 줄 사이의 간격인 line-height도 고려해야 하고 줄을 계산할 수 있는 -webkit-box 디스플레이도 필요합니다. line-clamp는 줄 수를 나타냅니다.
