  ## Introduction
   Google Developers Progressive Web App를 참고한 일기예보 Web App.

  ---

  ## Requirements

  - Chrome 52 이상
  - Web Server for Chrome 또는 Web Server

  ---

  ## Installation

   “`
   git clone https://github.com/kmmdong/ProgressiveWebApp.git
   “`

  ---

  ## What is a Progressive Web App?

  - Progressive - Works for every user, regardless of browser choice because it's built with progressive enhancement as a core tenet.
  - Responsive - Fits any form factor: desktop, mobile, tablet, or whatever is next.
  - Connectivity independent - Enhanced with service workers to work offline or on low-quality networks.
  - App-like - Feels like an app, because the app shell model separates the application functionality from application content .
  - Fresh - Always up-to-date thanks to the service worker update process.
  - Safe - Served via HTTPS to prevent snooping and to ensure content hasn't been tampered with.
  - Discoverable - Is identifiable as an "application" thanks to W3C manifest and service worker registration scope, allowing search engines to find it.
  - Re-engageable - Makes re-engagement easy through features like push notifications.
  - Installable - Allows users to add apps they find most useful to their home screen without the hassle of an app store.
  - Linkable - Easily share the application via URL, does not require complex installation.

  ---

   ## Keyword
  - app shell : 최소한의 사용자 인터페이스를 구성하는 HTML, CSS, Javascript의 모음. Service Worker를 통해 캐시된다.
  - service worker : 브라우저가 백그라운로 실행하는 스크립트. 일종의 프로그래밍 가능한 네트워크 프록시.
  - web app manifest : 일종의 홈화면의 아이콘과 비슷한 역할을 하는 JSON 파일.

  ---

   ## Things to do
    static resource들을 서비스 워커를 통해 캐싱 해놓고 빠르게 로딩한다. 오프라인 상황에서도 백그라운드로 돌아가고 있는 서비스 워커와 상호작용한다.
    온라인 상황 일때 최신 데이터로 다시 캐싱하고 업데이트를 한다. 덕분에 App처럼 오프라인에서도 작동하고, Push Notification, Background Sync등이 가능하다.
    접근성이 뛰어난 Web의 장점과 Native App의 장점을 고루 지니고 있는거 같다.
