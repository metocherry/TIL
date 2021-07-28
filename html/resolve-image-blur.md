# Resolve Image Blur

```css
.img {
  // 크롬, 사파리 등 브라우저에서 대비를 최적화
  image-rendering: -webkit-optimize-contrast;
  // z축을 0으로 적용하여 깊이감 제거
  transform: translateZ(0);
  // 뒷면을 보이지 않게 함으로써 2번과 유사하게 입체감을 제거
  backface-visibility: hidden;
}
```
