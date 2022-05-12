```css
@media (prefers-reduced-motion: reduce) {
  *, ::before, ::after {
    animation-delay: -1ms !important;
    animation-duration: 1ms !important;
    animation-iteration-count: 1 !important;
    background-attachment: initial !important;
    scroll-behavior: auto !important;
    transition-duration: 0s !important;
    transition-delay: 0s !important;
  }
}
```
위 코드의 의미는 애니메이션 기본설정을 축소한 모든 웹사이트에서 강제로 움직임 감소

## prefers-reduced-motion ##

기본 설정을 표시한 사용자를 위해 사이트의 모션 축소 변형을 설계할 수 있는 사용자 기본 설정 미디어 쿼리

1. no-preference: 사용자가 기본 운영 체제에서 기본 설정을 지정하지 않았음을 나타냅니다. 이 키워드 값은 부울 컨텍스트에서 false로 평가됩니다.
2. reduce: 사용자가 인터페이스가 움직임이나 애니메이션을 최소화해야 함을 나타내는 운영 체제 기본 설정을 지정했음을 나타냅니다. 바람직하지 않은 모든 움직임이 제거되는 지점까지입니다.