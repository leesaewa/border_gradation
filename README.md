# border_gradation

input border gradation with SVG

## Goal

- `input`이 `hover`와 `focus`되었을 때 `border gradient`가 나오도록 할 것.
- 반드시 `border-radius`가 포함되어야 함.

## 시도

### border-image

```
.container .input-box label:hover {}
```

- `border-image` `border-image-slice`속성을 이용해서 그라데이션을 넣을 수 있음.
- 하지만 `border-radius`가 적용되지 않음.

## 해결법

- `SVG`로 `border-radius`가 포함된 선을 그리기
- `opacity`로 가리고 `hover`했을 때에만 `opacity` 값을 `1`로 변경
