<!DOCTYPE html>
<html lang="ko" class="scroll-smooth">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Symbio Republic — 인간과 AI가 공존하는 가상 국가</title>
  <meta name="description" content="Symbio Republic: 인간과 AI의 공존을 실험하고 홍보하는 가상 국가 프로젝트" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <!-- Tailwind CSS (CDN) -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: { sans: ['Inter', 'ui-sans-serif', 'system-ui'] },
          colors: {
            brand: {
              50: '#eff6ff', 100: '#dbeafe', 200: '#bfdbfe', 300: '#93c5fd',
              400: '#60a5fa', 500: '#3b82f6', 600: '#2563eb', 700: '#1d4ed8',
              800: '#1e40af', 900: '#1e3a8a'
            },
          },
          boxShadow: {
            glow: '0 0 0 2px rgba(59,130,246,0.15), 0 10px 25px -5px rgba(59,130,246,0.35)'
          },
          animation: {
            'float': 'float 6s ease-in-out infinite',
            'pulse-soft': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
          },
          keyframes: {
            float: {
              '0%, 100%': { transform: 'translateY(0px)' },
              '50%': { transform: 'translateY(-8px)' }
            }
          }
        }
      },
      darkMode: 'class'
    }
  </script>
  <style>
    .glass { backdrop-filter: blur(10px); background: linear-gradient(180deg, rgba(255,255,255,0.7), rgba(255,255,255,0.4)); }
    .dark .glass { background: linear-gradient(180deg, rgba(17,24,39,0.7), rgba(17,24,39,0.4)); }
  </style>
</head>
<body class="bg-white text-gray-800 dark:bg-gray-950 dark:text-gray-100">
  <!-- Header / Nav -->
  <header id="top" class="sticky top-0 z-40 backdrop-blur border-b border-gray-200/70 dark:border-gray-800/80 bg-white/60 dark:bg-gray-950/60">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="flex h-16 items-center justify-between">
        <a href="#top" class="flex items-center gap-2 group">
          <span class="inline-flex h-9 w-9 items-center justify-center rounded-xl bg-brand-600 text-white shadow-glow animate-float">SR</span>
          <div class="leading-tight">
            <p class="font-extrabold tracking-tight">Symbio Republic</p>
            <p class="text-xs text-gray-500 group-hover:text-gray-700 dark:text-gray-400 dark:group-hover:text-gray-200">인간 × AI 공존</p>
          </div>
        </a>
        <nav class="hidden md:flex items-center gap-6 text-sm">
          <a href="#vision" class="hover:text-brand-600">비전</a>
          <a href="#charter" class="hover:text-brand-600">공존 헌장</a>
          <a href="#governance" class="hover:text-brand-600">거버넌스</a>
          <a href="#sim" class="hover:text-brand-600">정책 시뮬레이터</a>
          <a href="#citizenship" class="hover:text-brand-600">시민권</a>
          <a href="#faq" class="hover:text-brand-600">FAQ</a>
        </nav>
        <div class="flex items-center gap-2">
          <button id="themeToggle" class="rounded-xl px-3 py-2 text-sm border border-gray-200 dark:border-gray-800 hover:shadow-glow transition" aria-label="Toggle dark mode">🌙/☀️</button>
          <a href="#citizenship" class="hidden sm:inline-flex items-center gap-2 rounded-xl bg-brand-600 px-4 py-2 text-sm font-semibold text-white shadow-glow hover:bg-brand-700 transition">시민 신청</a>
        </div>
      </div>
    </div>
  </header>

  <!-- Hero -->
  <section class="relative overflow-hidden">
    <div class="absolute inset-0 -z-10 bg-gradient-to-b from-brand-50 to-white dark:from-gray-900 dark:to-gray-950"></div>
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8 py-16 sm:py-24">
      <div class="grid lg:grid-cols-2 gap-10 items-center">
        <div>
          <h1 class="text-4xl sm:text-6xl font-extrabold tracking-tight leading-tight">
            인간과 AI가 <span class="text-brand-600">함께 번영</span>하는
            <br class="hidden sm:block"/> 가상 국가
          </h1>
          <p class="mt-5 text-lg text-gray-600 dark:text-gray-300">Symbio Republic은 교육, 윤리, 혁신을 축으로 인간과 AI의 협력 모델을 실험하는 <span class="font-semibold">학생 주도</span> 프로젝트 국가입니다.</p>
          <div class="mt-8 flex flex-wrap gap-3">
            <a href="#sim" class="rounded-xl bg-brand-600 px-5 py-3 text-white font-semibold shadow-glow hover:bg-brand-700 transition">정책 시뮬레이터 체험</a>
            <a href="#charter" class="rounded-xl border px-5 py-3 font-semibold hover:shadow-glow transition border-gray-200 dark:border-gray-800">공존 헌장 보기</a>
          </div>
          <div class="mt-6 flex items-center gap-4 text-sm text-gray-500 dark:text-gray-400">
            <span class="inline-flex items-center gap-1">✅ 오픈 거버넌스</span>
            <span class="inline-flex items-center gap-1">✅ 윤리·투명성 우선</span>
            <span class="inline-flex items-center gap-1">✅ 청소년 주권</span>
          </div>
        </div>
        <div class="relative">
          <div class="glass rounded-3xl p-6 shadow-xl border border-white/40 dark:border-white/10">
            <div class="grid sm:grid-cols-2 gap-4">
              <div class="rounded-2xl p-4 bg-white/70 dark:bg-gray-900/70 border border-gray-200/70 dark:border-gray-800/70">
                <p class="text-xs uppercase tracking-wider text-gray-500 mb-1">핵심 지표</p>
                <h3 class="text-2xl font-bold">신뢰 지수</h3>
                <p class="text-4xl font-extrabold mt-1">92</p>
                <p class="text-xs text-gray-500 mt-2">설명 가능한 AI 비율, 개인정보 보호 준수율 기반</p>
              </div>
              <div class="rounded-2xl p-4 bg-white/70 dark:bg-gray-900/70 border border-gray-200/70 dark:border-gray-800/70">
                <p class="text-xs uppercase tracking-wider text-gray-500 mb-1">교육</p>
                <h3 class="text-2xl font-bold">리터러시</h3>
                <p class="text-4xl font-extrabold mt-1">A+</p>
                <p class="text-xs text-gray-500 mt-2">시민 AI 리터러시 인증율 87%</p>
              </div>
              <div class="rounded-2xl p-4 bg-white/70 dark:bg-gray-900/70 border border-gray-200/70 dark:border-gray-800/70">
                <p class="text-xs uppercase tracking-wider text-gray-500 mb-1">혁신</p>
                <h3 class="text-2xl font-bold">오픈랩</h3>
                <p class="text-4xl font-extrabold mt-1">36</p>
                <p class="text-xs text-gray-500 mt-2">학생-AI 공동 프로젝트 수</p>
              </div>
              <div class="rounded-2xl p-4 bg-white/70 dark:bg-gray-900/70 border border-gray-200/70 dark:border-gray-800/70">
                <p class="text-xs uppercase tracking-wider text-gray-500 mb-1">윤리</p>
                <h3 class="text-2xl font-bold">감사 로그</h3>
                <p class="text-4xl font-extrabold mt-1">100%</p>
                <p class="text-xs text-gray-500 mt-2">모든 의사결정에 공개 로그 적용</p>
              </div>
            </div>
          </div>
          <div class="absolute -z-10 blur-3xl bg-brand-400/30 dark:bg-brand-700/30 rounded-full w-72 h-72 -top-6 -right-8"></div>
        </div>
      </div>
    </div>
  </section>

  <!-- Vision -->
  <section id="vision" class="py-20">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-2xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">비전과 원칙</h2>
        <p class="mt-4 text-gray-600 dark:text-gray-300">우리는 기술을 목적으로 쓰지 않고, <span class="font-semibold">사람 중심의 공익</span>을 위해 설계합니다. 아래 세 축은 정책과 제품 모두를 안내합니다.</p>
      </div>
      <div class="mt-10 grid md:grid-cols-3 gap-6">
        <div class="rounded-2xl border p-6 hover:shadow-glow transition border-gray-200 dark:border-gray-800">
          <h3 class="text-xl font-bold">교육 우선</h3>
          <p class="mt-2 text-gray-600 dark:text-gray-300">모든 시민에게 AI 리터러시 교육을 제공하고, 오남용을 줄입니다.</p>
          <ul class="mt-4 space-y-2 text-sm text-gray-600 dark:text-gray-300 list-disc pl-4">
            <li>공개 커리큘럼과 실습</li>
            <li>모델 편향·한계 교육</li>
          </ul>
        </div>
        <div class="rounded-2xl border p-6 hover:shadow-glow transition border-gray-200 dark:border-gray-800">
          <h3 class="text-xl font-bold">윤리·투명성</h3>
          <p class="mt-2 text-gray-600 dark:text-gray-300">설명 가능한 의사결정, 프라이버시 보호, 감사 가능한 로그.</p>
          <ul class="mt-4 space-y-2 text-sm text-gray-600 dark:text-gray-300 list-disc pl-4">
            <li>데이터 최소 수집</li>
            <li>결정 경로 공개</li>
          </ul>
        </div>
        <div class="rounded-2xl border p-6 hover:shadow-glow transition border-gray-200 dark:border-gray-800">
          <h3 class="text-xl font-bold">공동 번영</h3>
          <p class="mt-2 text-gray-600 dark:text-gray-300">AI가 창출한 가치를 사회로 환류하는 토큰·참여 보상 모델.</p>
          <ul class="mt-4 space-y-2 text-sm text-gray-600 dark:text-gray-300 list-disc pl-4">
            <li>기여 기반 보상</li>
            <li>공익 프로젝트 펀딩</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Charter -->
  <section id="charter" class="py-20 bg-gray-50 dark:bg-gray-900/40">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-2xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">인간–AI 공존 헌장 (요약)</h2>
        <p class="mt-4 text-gray-600 dark:text-gray-300">국가 운영의 기준이 되는 7개 조항입니다. 전문은 깃허브/문서로 공개합니다.</p>
      </div>
      <div class="mt-8 grid md:grid-cols-2 gap-6">
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제1조 존엄과 안전</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">AI는 인간의 존엄과 안전을 최우선으로 한다.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제2조 투명성</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">중요 결정에는 설명 가능한 근거를 제공한다.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제3조 프라이버시</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">개인정보는 최소 수집·목적 제한을 따른다.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제4조 공정성</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">모델 편향을 측정·감축하며 영향 평가를 공개한다.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제5조 책임성</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">인간 최종 책임·이의제기 절차 보장.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제6조 개방성</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">핵심 정책·데이터셋 문서 공개, 연구 복제 허용.</p>
        </article>
        <article class="rounded-2xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <h3 class="font-bold">제7조 공익 환류</h3>
          <p class="text-gray-600 dark:text-gray-300 mt-2">AI 수익의 일정 비율을 공익 기금으로 환원.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- Governance -->
  <section id="governance" class="py-20">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-5 gap-10 items-start">
        <div class="lg:col-span-2">
          <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">거버넌스 구조</h2>
          <p class="mt-4 text-gray-600 dark:text-gray-300">사람과 AI의 <span class="font-semibold">이중 의회</span>와 <span class="font-semibold">중재 법원</span>으로 구성됩니다.</p>
          <ul class="mt-6 space-y-3 text-gray-700 dark:text-gray-300">
            <li>👥 시민의회: 정책 제안·투표</li>
            <li>🤖 AI 평의회: 분석·시뮬레이션·영향평가</li>
            <li>⚖️ 중재 법원: 분쟁 조정·권리 보장</li>
          </ul>
        </div>
        <div class="lg:col-span-3">
          <div class="rounded-3xl border p-6 border-gray-200 dark:border-gray-800">
            <div class="grid md:grid-cols-3 gap-4">
              <div class="rounded-2xl p-4 bg-gray-50 dark:bg-gray-900">
                <h3 class="font-bold">시민의회</h3>
                <p class="text-sm text-gray-600 dark:text-gray-300 mt-1">제안·토론·투표. 1인 1표, 공론화 룸.</p>
              </div>
              <div class="rounded-2xl p-4 bg-gray-50 dark:bg-gray-900">
                <h3 class="font-bold">AI 평의회</h3>
                <p class="text-sm text-gray-600 dark:text-gray-300 mt-1">정책 효과 예측, 리스크 모니터링.</p>
              </div>
              <div class="rounded-2xl p-4 bg-gray-50 dark:bg-gray-900">
                <h3 class="font-bold">중재 법원</h3>
                <p class="text-sm text-gray-600 dark:text-gray-300 mt-1">권리 침해·편향 판정 이의 제기.</p>
              </div>
            </div>
            <p class="mt-4 text-sm text-gray-500 dark:text-gray-400">※ 실제 운영은 모의 환경이며, 모든 데이터는 교육 목적입니다.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Policy Simulator -->
  <section id="sim" class="py-20 bg-gray-50 dark:bg-gray-900/40">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-3xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">정책 시뮬레이터 (데모)</h2>
        <p class="mt-3 text-gray-600 dark:text-gray-300">세 가지 정책 레버를 조정해 보세요. 경제 성장, 신뢰, 혁신 점수가 어떻게 달라지는지 실시간으로 확인합니다.</p>
      </div>
      <div class="mt-8 grid lg:grid-cols-2 gap-8">
        <div class="rounded-3xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <label class="block text-sm font-semibold">AI 자율성 (0–100)</label>
          <input id="autonomy" type="range" min="0" max="100" value="50" class="w-full mt-2">
          <label class="block mt-6 text-sm font-semibold">투명성 규제 강도 (0–100)</label>
          <input id="transparency" type="range" min="0" max="100" value="70" class="w-full mt-2">
          <label class="block mt-6 text-sm font-semibold">개인정보 보호 수준 (0–100)</label>
          <input id="privacy" type="range" min="0" max="100" value="80" class="w-full mt-2">
          <p class="mt-6 text-xs text-gray-500 dark:text-gray-400">※ 단순 모델: 시연용 선형·비선형 가중치 조합</p>
        </div>
        <div class="rounded-3xl border p-6 bg-white/70 dark:bg-gray-950/40 border-gray-200 dark:border-gray-800">
          <div class="grid sm:grid-cols-3 gap-4">
            <div>
              <p class="text-xs text-gray-500">경제 성장</p>
              <p id="growthScore" class="text-4xl font-extrabold">–</p>
              <div class="mt-2 h-2 w-full bg-gray-200 dark:bg-gray-800 rounded-full overflow-hidden">
                <div id="growthBar" class="h-full bg-brand-600" style="width: 50%"></div>
              </div>
            </div>
            <div>
              <p class="text-xs text-gray-500">사회적 신뢰</p>
              <p id="trustScore" class="text-4xl font-extrabold">–</p>
              <div class="mt-2 h-2 w-full bg-gray-200 dark:bg-gray-800 rounded-full overflow-hidden">
                <div id="trustBar" class="h-full bg-emerald-500" style="width: 50%"></div>
              </div>
            </div>
            <div>
              <p class="text-xs text-gray-500">혁신성</p>
              <p id="innovationScore" class="text-4xl font-extrabold">–</p>
              <div class="mt-2 h-2 w-full bg-gray-200 dark:bg-gray-800 rounded-full overflow-hidden">
                <div id="innovationBar" class="h-full bg-indigo-500" style="width: 50%"></div>
              </div>
            </div>
          </div>
          <div class="mt-6 text-sm text-gray-600 dark:text-gray-300" id="insight">슬라이더를 조정해 보세요.</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Citizenship -->
  <section id="citizenship" class="py-20">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-3xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">시민권 신청</h2>
        <p class="mt-3 text-gray-600 dark:text-gray-300">학생·교사 누구나 무료로 참여할 수 있는 ‘가상 시민권’. 프로젝트 소식과 오픈랩 초대장을 보내드립니다.</p>
      </div>
      <form class="mt-8 grid md:grid-cols-2 gap-6" name="citizenship" method="POST" data-netlify="true">
        <input type="hidden" name="form-name" value="citizenship" />
        <div class="md:col-span-1">
          <label class="block text-sm font-semibold">이름</label>
          <input name="name" required class="mt-2 w-full rounded-xl border px-4 py-2 focus:outline-none focus:ring-2 focus:ring-brand-500 border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-900" placeholder="홍길동" />
        </div>
        <div class="md:col-span-1">
          <label class="block text-sm font-semibold">이메일</label>
          <input name="email" type="email" required class="mt-2 w-full rounded-xl border px-4 py-2 focus:outline-none focus:ring-2 focus:ring-brand-500 border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-900" placeholder="you@example.com" />
        </div>
        <div class="md:col-span-2">
          <label class="block text-sm font-semibold">관심 분야</label>
          <select name="interest" class="mt-2 w-full rounded-xl border px-4 py-2 border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-900">
            <option>AI 리터러시 교육</option>
            <option>윤리·법·정책</option>
            <option>데이터 사이언스</option>
            <option>오픈소스 개발</option>
            <option>디자인·커뮤니케이션</option>
          </select>
        </div>
        <div class="md:col-span-2">
          <label class="block text-sm font-semibold">한 줄 포부</label>
          <textarea name="motivation" rows="3" class="mt-2 w-full rounded-xl border px-4 py-2 border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-900" placeholder="이 프로젝트에서 이루고 싶은 것을 적어주세요."></textarea>
        </div>
        <div class="md:col-span-2 flex items-center justify-between">
          <label class="inline-flex items-center gap-2 text-sm"><input type="checkbox" required class="rounded"> 개인정보 수집·이용에 동의합니다. (교육 목적)</label>
          <button class="rounded-xl bg-brand-600 px-5 py-3 text-white font-semibold shadow-glow hover:bg-brand-700 transition" type="submit">신청하기</button>
        </div>
        <p class="md:col-span-2 text-xs text-gray-500 dark:text-gray-400">※ 백엔드 없이도 작동하도록 Netlify Forms 속성 포함. 다른 호스팅을 사용할 경우 구글 폼/시트 연동을 권장합니다.</p>
      </form>
    </div>
  </section>

  <!-- Roadmap -->
  <section id="roadmap" class="py-20 bg-gray-50 dark:bg-gray-900/40">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-2xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">로드맵</h2>
        <p class="mt-3 text-gray-600 dark:text-gray-300">3단계 파일럿 → 오픈랩 확장 → 커뮤니티 자치로 이어집니다.</p>
      </div>
      <ol class="mt-8 grid md:grid-cols-3 gap-6">
        <li class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <p class="text-xs text-gray-500">Phase 1</p>
          <h3 class="font-semibold mt-1">학교 파일럿</h3>
          <p class="text-sm text-gray-600 dark:text-gray-300 mt-2">AI 리터러시 워크숍, 정책 토론회, 간단한 데이터 윤리 실험.</p>
        </li>
        <li class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <p class="text-xs text-gray-500">Phase 2</p>
          <h3 class="font-semibold mt-1">오픈랩 확장</h3>
          <p class="text-sm text-gray-600 dark:text-gray-300 mt-2">외부 멘토·동아리 연계, 오픈소스 프로젝트 공개.</p>
        </li>
        <li class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <p class="text-xs text-gray-500">Phase 3</p>
          <h3 class="font-semibold mt-1">커뮤니티 자치</h3>
          <p class="text-sm text-gray-600 dark:text-gray-300 mt-2">시민 제안 상시 접수, 투표 기반 예산 배분.</p>
        </li>
      </ol>
    </div>
  </section>

  <!-- FAQ -->
  <section id="faq" class="py-20">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="max-w-2xl">
        <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">자주 묻는 질문</h2>
        <p class="mt-3 text-gray-600 dark:text-gray-300">가상의 국가지만, 실제 문제의식과 학습을 위한 실험 공간입니다.</p>
      </div>
      <div class="mt-8 space-y-4" id="faqList">
        <details class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <summary class="font-semibold cursor-pointer">진짜 국가인가요?</summary>
          <p class="mt-2 text-gray-600 dark:text-gray-300">법적 국가는 아니며, 교육과 연구를 위한 커뮤니티 기반 가상 국가입니다.</p>
        </details>
        <details class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <summary class="font-semibold cursor-pointer">AI가 결정을 내리나요?</summary>
          <p class="mt-2 text-gray-600 dark:text-gray-300">중요 결정은 항상 인간의 최종 책임 하에 이루어집니다. AI는 분석과 제안을 담당합니다.</p>
        </details>
        <details class="rounded-2xl border p-6 border-gray-200 dark:border-gray-800 bg-white/70 dark:bg-gray-950/40">
          <summary class="font-semibold cursor-pointer">데이터는 안전한가요?</summary>
          <p class="mt-2 text-gray-600 dark:text-gray-300">최소 수집 원칙과 암호화 저장을 지향합니다. 본 데모 사이트는 개인 데이터를 서버에 저장하지 않습니다.</p>
        </details>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="border-t border-gray-200 dark:border-gray-800 py-10">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-6">
        <div>
          <p class="font-bold">Symbio Republic</p>
          <p class="text-sm text-gray-500 dark:text-gray-400">© <span id="year"></span> 학생 주도 프로젝트. All rights reserved.</p>
        </div>
        <div class="text-sm text-gray-500 dark:text-gray-400">
          <a href="#top" class="hover:text-brand-600">맨 위로 ▲</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Scripts -->
  <script>
    // Year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Theme toggle (persist in localStorage)
    const root = document.documentElement;
    const themeToggle = document.getElementById('themeToggle');
    const storedTheme = localStorage.getItem('theme');
    if (storedTheme === 'dark' || (!storedTheme && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
      root.classList.add('dark');
    }
    themeToggle.addEventListener('click', () => {
      root.classList.toggle('dark');
      localStorage.setItem('theme', root.classList.contains('dark') ? 'dark' : 'light');
    });

    // Simple Policy Simulator Model
    const sliders = ['autonomy','transparency','privacy'].map(id => document.getElementById(id));
    const growthScoreEl = document.getElementById('growthScore');
    const trustScoreEl = document.getElementById('trustScore');
    const innovationScoreEl = document.getElementById('innovationScore');
    const growthBar = document.getElementById('growthBar');
    const trustBar = document.getElementById('trustBar');
    const innovationBar = document.getElementById('innovationBar');
    const insight = document.getElementById('insight');

    function clamp(x){ return Math.max(0, Math.min(100, Math.round(x))); }

    function updateScores() {
      const A = parseFloat(sliders[0].value); // autonomy
      const T = parseFloat(sliders[1].value); // transparency
      const P = parseFloat(sliders[2].value); // privacy

      // Toy model: choose weights & trade-offs
      const growth = clamp(0.6*A + 0.2*T + 0.2*P - 0.003*(T-60)**2 - 0.003*(P-50)**2);
      const trust  = clamp(0.15*A + 0.5*T + 0.35*P - 0.002*(A-40)**2);
      const innov  = clamp(0.55*A + 0.25*T + 0.2*P - 0.002*(T-40)**2);

      growthScoreEl.textContent = growth;
      trustScoreEl.textContent = trust;
      innovationScoreEl.textContent = innov;

      growthBar.style.width = growth + '%';
      trustBar.style.width = trust + '%';
      innovationBar.style.width = innov + '%';

      // Insight message
      let msg = '';
      if (A > 70 && T > 70) msg = '높은 자율성과 투명성의 조합 → 혁신과 신뢰의 동시 확보!';
      else if (A > 70 && P < 40) msg = '자율성 ↑, 프라이버시 ↓ → 혁신은 늘지만 신뢰 리스크 주의';
      else if (T > 80 && P > 80) msg = '매우 높은 규제·보호 → 신뢰 높지만 성장 둔화 가능';
      else msg = '정책 간 균형을 탐색해 보세요.';
      insight.textContent = msg;
    }

    sliders.forEach(sl => sl.addEventListener('input', updateScores));
    updateScores();
  </script>
</body>
</html>
# -
