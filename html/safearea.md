# Safearea

전체 화면 설정

```html
<meta name='viewport' content='initial-scale=1, viewport-fit=cover'>
```

## iphone `env` 속성

```css
/* iOS 11.0 버전 */

.app {
  constant(safe-area-inset-top)
  constant(safe-area-inset-right)
  constant(safe-area-inset-bottom)
  constant(safe-area-inset-left)
}

/* iOS 11.2 이상 */
.app {
  env(safe-area-inset-top)
  env(safe-area-inset-right)
  env(safe-area-inset-bottom)
  env(safe-area-inset-left)
}
```
