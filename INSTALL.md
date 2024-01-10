## Source
~~~console
git clone https://github.com/pushdown99/atalk
cd atalk
~~~

tool 설치 (make.exe coreutils.exe)


~~~console
npm install --legacy-peer-deps
npm audit fix --force
npm start
~~~

## Run
~~~console
webpack.config.js <- IP  주소변경
~~~

## Localization
~~~console
1. /image/watermark.svg
2. interface_config.js의 JITSI_WATERMARK_LINK
3. lang/main.json의 headerTitle
4. react/features/welcome/components/WelcomePage.web.js의 footer 주석
5. images/favicon.ico
6. title.html 수정
7. interface_config.js의 APP_NAME 변경
~~~

## Build
~~~console
mingw32-make dev
~~~