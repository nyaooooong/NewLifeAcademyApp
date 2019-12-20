## 작업 히스토리
- 12.10 : 
<br/> index.html, navigator.xml, script.js 추가.
<br/> 기본적인 동작 구현
- 12.11 : 
<br/> readbible.webmanifest 추가.
<br/> icon 및 theme color 설정.
- 12.12 : 
<br/> service worker 추가.
<br/> navigator.xml을 월단위로 분리.
<br/> 지속적으로 테스트 했으나 PWA화되지 않음.
- 12.13 :
<br/> PWA화 되지 않은 이유가 https 로 접속하지 않아서 였음을 확인함.
<br/> HTTP redirect를 위해서는 server(nginx) 설정을 변경해야 하지만 glitch console에서는 sudo 가 안먹힘.
<br/> node.js의 express를 사용해서 http to https redirect를 구현한 소스를 확인 --> express를 사용하도록 변경 시작.
<br/> app 처럼 menu bar가 나오도록 추가. (CSS를 사용하면 text만으로 상당히 멋있는 menu bar를 만들 수 있음.)
- 12.15 :
<br/> express 를 적용해서 http to https redirect를 구현했다. req.secure 사용은 실패했고 x-forwarded-proto 를 사용한 버전으로 성공했다.
<br/> menu bar를 추가해보자

## 참고자료
+ pwa sample : 
<br/> https://github.com/mdn/pwa-examples/tree/master/js13kpwa
+ svg to png : 
<br/> http://svgtopng.com/
+ Material Icon : 
<br/> https://material.io/resources/icons/
+ svg 크기 변환 : 
<br/> https://www.iloveimg.com/ko/resize-image/resize-svg
+ http to https sample :
<br/> http://large-patch.glitch.me
+ menu bar sample 모음 : 
<br/> https://medium.com/level-up-web/20-responsive-navigation-solutions-examples-codes-21644390afeb
+ menu bar sample :
<br/> https://inspirationalpixels.com/creating-a-responsive-menu-with-html-css-jquery/
