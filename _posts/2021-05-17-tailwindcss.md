vscode tailwind inteligence 설치 권장

### setting & install ###

 * sample prj 가이드에서 vue 를 사용하여 vue 도 설치함 
 * IE 11 지원을 위해 VUE2 버전 사용 VUE3, tailwindcss 2.x.x 부터는 IE 지원 전혀 고려 않음


prefix flow

bg- : background
sm: , md:, lg:, xl: responsive
text-
m: margin, mx: margin x-side, my : margin-y-side
shadow- : shadow
rounded-
hover:   : hover state
focus:     focus:outline-none focus:shadow-outline 으로 주면 focus outline round 가 외곽선과 통일되어 보기 좋다. 


custom design 적용 

tailwindcss.config.js  에서 기본 컬러 파렛트와 커스텀디자인에 필요한 요소들을 설정하고 build 하면 적용된 최종 css로 빌드할 수 있다. 