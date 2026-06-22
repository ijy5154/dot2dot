# 📱 dot2dot (Dots and Boxes)

> **HTML 파일 단 하나**로 실행되는 모바일 최적화 2인용 클래식 보드 게임, **dot2dot**입니다.  
> 별도의 빌드 도구나 의존성 없이 Tailwind CSS와 Vanilla JavaScript만을 활용하여 미니멀하고 기민하게 작동합니다.

<br />

## ✨ Key Features (주요 기능)

* **Single-File Architecture**: HTML, CSS, JS가 단 하나의 파일로 구성되어 배포와 커스텀이 매우 가볍습니다.
* **Mobile-First Design**: 스마트폰을 바닥에 내려놓고 마주 앉아 플레이하기 최적화된 상/하 분할 레이아웃을 제공합니다.
* **Fat-Finger Prevention (터치 영역 확장)**: 모바일 환경에서 얇은 선을 오동작 없이 쉽게 누를 수 있도록 눈에 보이지 않는 넉넉한 터치 패딩 영역(Hitbox)을 설계했습니다.
* **Native App-like UX**: 모바일 브라우저에서 연속 터치 시 발생하는 반투명 파란색 하이라이트 잔상과 롱프레스 이벤트를 CSS로 완벽히 차단하여 부드러운 조작감을 제공합니다.
* **Real-time State Management**: 순수 JavaScript 객체와 DOM 제어만으로 스코어 킹, 턴 체인지, 박스 점령 이펙트를 실시간 동기화합니다.

<br />

## 🛠️ Tech Stack (기술 스택)

* **Frontend**: HTML5
* **Styling**: [Tailwind CSS](https://tailwindcss.com) (via CDN)
* **Logic**: Vanilla JavaScript (ES6+)

<br />

## 🕹️ How to Play (게임 방법)

1. **Player 1(Blue)**과 **Player 2(Red)**가 차례대로 돌아가며 점과 점 사이의 회색 선을 터치해 선을 채웁니다.
2. 선을 연결하여 사각형(Box)의 **마지막 4번째 면을 닫는 플레이어**가 해당 박스를 점령(P1/P2)하고 1점을 획득합니다.
3. 박스를 획득한 플레이어는 **턴을 한 번 더** 가져갑니다.
4. 모든 격자가 채워졌을 때, 더 많은 박스를 점령한 플레이어가 최종 승리합니다.
