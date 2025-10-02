# 👋 안녕하세요, 조수아입니다!

<!-- file: header.svg -->
<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="300" viewBox="0 0 1200 300" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Animated background">
  <!-- foreignObject 내부에 XHTML/CSS를 넣어 GitHub README에서 애니메이션을 동작시키는 기법 -->
  <foreignObject x="0" y="0" width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <style>
        /* 기본 레이아웃 */
        :root{
          --bg:#0f0c2d;
          --particle-size:5vmax;
        }
        *{box-sizing:border-box}
        html,body{
          margin:0;padding:0;width:100%;height:100%;
        }
        .hero{
          width:1200px;         /* SVG 뷰포트에 고정 폭 */
          height:300px;
          display:block;
          background: linear-gradient(135deg,var(--bg) 0%, #2b0e44 100%);
          overflow:hidden;
          position:relative;
          font-family: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
        }
        /* 중앙 텍스트 (옵션) */
        .center {
          position: absolute;
          left: 50%;
          top: 50%;
          transform: translate(-50%,-50%);
          color: #fff;
          text-align:center;
          font-weight:600;
          text-shadow:0 6px 18px rgba(0,0,0,0.6);
          pointer-events:none;
        }
        .center h1{ margin:0;font-size:28px;letter-spacing:0.6px; }
        .center p{ margin:4px 0 0 0;font-size:12px;opacity:0.85 }
        .background{ position:absolute; inset:0; width:100%; height:100%; }
        .background span{
          position:absolute;
          width:var(--particle-size);
          height:var(--particle-size);
          border-radius:50%;
          filter:blur(12px);
          opacity:0.9;
          transform: translate3d(0,0,0);
          animation: float linear infinite;
          mix-blend-mode: screen;
        }
        @keyframes float{
          0%   { transform: translateY(10vh) scale(0.85) rotate(0deg); opacity:0.7; }
          50%  { transform: translateY(-18vh) scale(1.05) rotate(90deg); opacity:1; }
          100% { transform: translateY(10vh) scale(0.9) rotate(180deg); opacity:0.7; }
        }
        .background span:nth-child(1){ left:6%;  top:30%;  background: #583C87; width:6vmax; height:6vmax; animation-duration:18s; animation-delay:-2s; box-shadow:0 0 40px #583C87;}
        .background span:nth-child(2){ left:18%; top:62%;  background: #E45A84; width:4.5vmax; animation-duration:14s; animation-delay:-4s; box-shadow:0 0 36px #E45A84;}
        .background span:nth-child(3){ left:30%; top:18%;  background: #FFACAC; width:5vmax; animation-duration:20s; animation-delay:-6s; box-shadow:0 0 44px #FFACAC;}
        .background span:nth-child(4){ left:44%; top:50%;  background: #6B34A8; width:7vmax; animation-duration:22s; animation-delay:-8s; box-shadow:0 0 48px #6B34A8;}
        .background span:nth-child(5){ left:56%; top:12%;  background: #F08FB3; width:4vmax; animation-duration:16s; animation-delay:-3s; box-shadow:0 0 34px #F08FB3;}
        .background span:nth-child(6){ left:68%; top:68%;  background: #FFD3A5; width:6vmax; animation-duration:19s; animation-delay:-5s; box-shadow:0 0 40px #FFD3A5;}
        .background span:nth-child(7){ left:80%; top:28%;  background: #9B6CF1; width:5.5vmax; animation-duration:24s; animation-delay:-7s; box-shadow:0 0 46px #9B6CF1;}
        .background span:nth-child(8){ left:88%; top:58%;  background: #FF7AA2; width:4.2vmax; animation-duration:15s; animation-delay:-1s; box-shadow:0 0 32px #FF7AA2;}
        .background span:nth-child(9){ left:10%; top:8%;   background: #3E1E68; width:5vmax; animation-duration:21s; animation-delay:-9s; box-shadow:0 0 42px #3E1E68;}
        .background span:nth-child(10){ left:22%; top:82%; background: #FFB4C6; width:3.8vmax; animation-duration:13s; animation-delay:-11s; box-shadow:0 0 30px #FFB4C6;}
        .background span:nth-child(11){ left:36%; top:72%; background: #A56CF0; width:6.5vmax; animation-duration:23s; animation-delay:-2s; box-shadow:0 0 50px #A56CF0;}
        .background span:nth-child(12){ left:48%; top:26%; background: #E96A7C; width:4.6vmax; animation-duration:17s; animation-delay:-6s; box-shadow:0 0 36px #E96A7C;}
        .background span:nth-child(13){ left:60%; top:46%; background: #FFB9B9; width:5.2vmax; animation-duration:18s; animation-delay:-8s; box-shadow:0 0 38px #FFB9B9;}
        .background span:nth-child(14){ left:72%; top:10%; background: #7C3B9B; width:7.2vmax; animation-duration:25s; animation-delay:-12s; box-shadow:0 0 52px #7C3B9B;}
        .background span:nth-child(15){ left:4%;  top:54%; background: #E45A84; width:4.8vmax; animation-duration:14s; animation-delay:-3s; box-shadow:0 0 34px #E45A84;}
        .background span:nth-child(16){ left:92%; top:6%;  background: #FF9FB7; width:5vmax; animation-duration:16s; animation-delay:-4s; box-shadow:0 0 36px #FF9FB7;}
        .background span:nth-child(17){ left:62%; top:82%; background: #CFA6FF; width:6vmax; animation-duration:20s; animation-delay:-9s; box-shadow:0 0 44px #CFA6FF;}
        .background span:nth-child(18){ left:28%; top:40%; background: #5D3B8D; width:3.6vmax; animation-duration:12s; animation-delay:-2s; box-shadow:0 0 30px #5D3B8D;}
        .background span:nth-child(19){ left:46%; top:86%; background: #FFB4A2; width:4.1vmax; animation-duration:15s; animation-delay:-7s; box-shadow:0 0 34px #FFB4A2;}
        .background span:nth-child(20){ left:76%; top:36%; background: #FF8FB6; width:5.7vmax; animation-duration:19s; animation-delay:-6s; box-shadow:0 0 40px #FF8FB6;}
        /* 반응형(뷰포트에 따라 줄임) */
        @media (max-width:800px){
          svg{height:200px}
          .hero{height:200px;width:100%}
          .center h1{font-size:20px}
        }
      </style>
      <div class="hero" aria-hidden="true">
        <div class="background" role="presentation">
          <!-- 20개의 span: CodePen의 'bokeh' 스타일을 단순화/정적화한 버전 -->
          <span></span><span></span><span></span><span></span><span></span>
          <span></span><span></span><span></span><span></span><span></span>
          <span></span><span></span><span></span><span></span><span></span>
          <span></span><span></span><span></span><span></span><span></span>
        </div>
        <!-- 가운데 텍스트는 선택사항입니다. 원하면 수정/삭제하세요 -->
        <div class="center">
        </div>
      </div>
    </div>
  </foreignObject>
</svg>


## 👨‍💻 소개
- 🏫 한신대학교 재학 중
- 💡 [게임, 아이돌 덕질에 대해 관심 있음]
- 🌱 [AISW계열에서 웹프로그래밍 과목을 배우고 있음]

## 🛠️ 기술 스택
*   [2종 보통 자동 운전면허 보유]

## 👨‍💻 경력
*   [수학학원 조교 아르바이트 (2025.01~2025.07)]
*   [카페 파트타임 아르바이트 (2025.02~현재)]

<!--
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black">
</p>
-->

## 📫 연락처
- email📧: [josua6767@hs.ac.kr]
- 깃허브: [https://github.com/CHOSUA6767]
- instargram: [https://www.instagram.com/jotsua_67/]