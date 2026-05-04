[index.html](https://github.com/user-attachments/files/27328032/index.html)
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>오지혜 · Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Pretendard:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#ffffff;
  --bg2:#f7f6f3;
  --bg3:#efede9;
  --text:#1a1a1a;
  --text2:#666;
  --text3:#999;
  --border:#e8e6e1;
  --teal-bg:#e1f5ee;--teal-text:#0f6e56;
  --purple-bg:#eeedfe;--purple-text:#3c3489;
  --blue-bg:#e6f1fb;--blue-text:#0c447c;
  --amber-bg:#faeeda;--amber-text:#854f0b;
  --coral-bg:#faece7;--coral-text:#993c1d;
  --gray-bg:#f1efe8;--gray-text:#444441;
  --green-bg:#eaf3de;--green-text:#3b6d11;
  --radius:8px;
  --radius-lg:12px;
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Pretendard',-apple-system,BlinkMacSystemFont,sans-serif;background:var(--bg);color:var(--text);line-height:1.6;font-size:15px}
a{color:inherit;text-decoration:none}

.page{max-width:780px;margin:0 auto;padding:3rem 2rem 6rem}

/* 헤더 */
.header-card{background:var(--bg2);border-radius:var(--radius-lg);border:0.5px solid var(--border);padding:2rem 2rem 1.75rem;margin-bottom:2rem}
.header-top{display:flex;align-items:center;gap:16px;margin-bottom:1rem}
.avatar{width:52px;height:52px;border-radius:50%;background:var(--teal-bg);display:flex;align-items:center;justify-content:center;font-size:15px;font-weight:600;color:var(--teal-text);flex-shrink:0;letter-spacing:.02em}
.name{font-size:22px;font-weight:600;margin-bottom:3px}
.subtitle{font-size:13px;color:var(--text2)}
.intro{font-size:13.5px;color:var(--text2);line-height:1.75;margin-bottom:1.25rem}
.badges{display:flex;flex-wrap:wrap;gap:5px;margin-bottom:1.25rem}
.badge{display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:500}
.b-teal{background:var(--teal-bg);color:var(--teal-text)}
.b-purple{background:var(--purple-bg);color:var(--purple-text)}
.b-blue{background:var(--blue-bg);color:var(--blue-text)}
.b-amber{background:var(--amber-bg);color:var(--amber-text)}
.b-coral{background:var(--coral-bg);color:var(--coral-text)}
.b-gray{background:var(--gray-bg);color:var(--gray-text)}
.b-green{background:var(--green-bg);color:var(--green-text)}
.contact{display:flex;gap:1.5rem;font-size:12.5px;color:var(--text3)}
.contact a{color:var(--blue-text);transition:opacity .15s}
.contact a:hover{opacity:.7}

/* 섹션 */
.sec-label{font-size:11px;font-weight:600;color:var(--text3);letter-spacing:.07em;text-transform:uppercase;margin-bottom:.875rem;margin-top:2.25rem}

/* 메트릭 */
.metric-grid{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:10px}
.metric{background:var(--bg2);border-radius:var(--radius);border:0.5px solid var(--border);padding:.875rem 1rem}
.metric-val{font-size:22px;font-weight:600;color:var(--text);margin-bottom:2px}
.metric-lbl{font-size:11.5px;color:var(--text3)}

/* 탭 */
.tab-row{display:flex;gap:6px;flex-wrap:wrap;margin-bottom:1.125rem}
.tab{font-size:12.5px;padding:4px 14px;border-radius:20px;border:0.5px solid var(--border);color:var(--text2);cursor:pointer;transition:all .15s;background:var(--bg)}
.tab:hover{background:var(--bg2)}
.tab.active{background:var(--bg2);color:var(--text);font-weight:500;border-color:transparent}

/* 프로젝트 그리드 */
.proj-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:.875rem}
.proj-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1.125rem 1.25rem;transition:box-shadow .2s}
.proj-card:hover{box-shadow:0 2px 12px rgba(0,0,0,.06)}
.proj-tag{font-size:11.5px;color:var(--text3);margin-bottom:.35rem}
.proj-title{font-size:14px;font-weight:600;margin-bottom:.5rem;line-height:1.4}
.proj-desc{font-size:12.5px;color:var(--text2);line-height:1.65;margin-bottom:.75rem}
.proj-results{list-style:none;margin-bottom:.75rem}
.proj-results li{font-size:12.5px;color:var(--text);display:flex;gap:7px;align-items:flex-start;margin-bottom:4px;line-height:1.5}
.proj-results li::before{content:'';width:5px;height:5px;border-radius:50%;flex-shrink:0;margin-top:6px}
.dot-teal::before{background:var(--teal-text)}
.dot-blue::before{background:var(--blue-text)}
.dot-purple::before{background:var(--purple-text)}
.dot-coral::before{background:var(--coral-text)}
.proj-tags{display:flex;flex-wrap:wrap;gap:4px}

/* PM 역할 */
.pm-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1.25rem 1.5rem}
.pm-example{font-size:12.5px;color:var(--text3);margin-bottom:1.125rem;padding-bottom:.875rem;border-bottom:0.5px solid var(--border)}
.steps{display:flex;flex-direction:column;gap:.875rem}
.step{display:flex;gap:12px;align-items:flex-start}
.step-num{width:24px;height:24px;border-radius:50%;background:var(--teal-bg);color:var(--teal-text);font-size:11px;font-weight:600;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px}
.step-title{font-size:13px;font-weight:600;margin-bottom:2px}
.step-desc{font-size:12.5px;color:var(--text2);line-height:1.6}

/* 스킬 */
.skill-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1.125rem 1.5rem}
.skill-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:.5rem}
.skill-item{font-size:13px;color:var(--text2);display:flex;align-items:center;gap:7px}
.skill-dot{width:6px;height:6px;border-radius:50%;flex-shrink:0}

/* 경력 */
.career-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1.125rem 1.5rem}
.career-row{display:flex;justify-content:space-between;align-items:flex-start;padding:.75rem 0;border-bottom:0.5px solid var(--border)}
.career-row:first-child{padding-top:0}
.career-row:last-child{border-bottom:none;padding-bottom:0}
.career-company{font-size:14px;font-weight:600;margin-bottom:3px}
.career-role{font-size:12.5px;color:var(--text2)}
.career-period{font-size:12px;color:var(--text3);text-align:right;white-space:nowrap;flex-shrink:0;margin-left:1rem}

/* 프리랜서 */
.freelance-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:.75rem}
.fl-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1rem 1.125rem}
.fl-title{font-size:13px;font-weight:600;margin-bottom:4px;line-height:1.4}
.fl-desc{font-size:12px;color:var(--text2);line-height:1.6}

/* 타임라인 배너 */
.timeline-banner{background:var(--bg2);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:1.25rem 1.5rem;margin-bottom:.75rem}
.tl-title{font-size:13px;font-weight:600;margin-bottom:.875rem;color:var(--text2)}
.tl-track{display:flex;flex-direction:column;gap:.5rem}
.tl-row{display:flex;align-items:center;gap:10px;font-size:12.5px}
.tl-dot{width:9px;height:9px;border-radius:50%;flex-shrink:0}
.tl-period{color:var(--text3);min-width:110px;flex-shrink:0}
.tl-company{font-weight:600;min-width:130px}
.tl-role{color:var(--text2)}
.tl-line{width:1.5px;background:var(--border);height:18px;margin-left:4px}

/* 자격증 */
.cert-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:.75rem}
.cert-card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius-lg);padding:.875rem 1rem}
.cert-year{font-size:11px;color:var(--text3);margin-bottom:3px}
.cert-name{font-size:13px;font-weight:600}

/* 반응형 */
@media(max-width:600px){
  .proj-grid{grid-template-columns:1fr}
  .metric-grid{grid-template-columns:repeat(2,1fr)}
  .freelance-grid{grid-template-columns:1fr}
  .cert-grid{grid-template-columns:repeat(2,1fr)}
  .page{padding:2rem 1.25rem 4rem}
}
</style>
</head>
<body>
<div class="page">

<!-- 헤더 -->
<div class="header-card">
  <div class="header-top">
    <div class="avatar">JO</div>
    <div>
      <div class="name">오지혜 · Jihye Oh</div>
      <div class="subtitle">Globalization PM · Localization Strategy · Content Production</div>
    </div>
  </div>
  <div class="intro">
    7년간 콘텐츠·게임 분야에서 스페인어 현지화 전략 수립, 7개 언어 인하우스팀 LPM, 콘텐츠 기획 PM을 담당했습니다. 단순 번역 관리에 머물지 않고 문화 적합성 기반의 현지화 전략을 직접 설계하고 실행해왔습니다.
  </div>
  <div class="badges">
    <span class="badge b-teal">현지화 전략</span>
    <span class="badge b-purple">7개 언어 LPM</span>
    <span class="badge b-blue">콘텐츠 기획 PM</span>
    <span class="badge b-amber">스페인어 C2</span>
    <span class="badge b-coral">게임 현지화</span>
    <span class="badge b-gray">AI 번역 워크플로우</span>
  </div>
  <div class="contact">
    <a href="mailto:jihye.oh@email.com">jihye.oh@email.com</a>
    <a href="https://linkedin.com/in/jihyeoh" target="_blank">linkedin.com/in/jihyeoh</a>
  </div>
</div>

<!-- 핵심 성과 -->
<div class="sec-label">핵심 성과 한눈에 보기</div>
<div class="metric-grid">
  <div class="metric"><div class="metric-val">7년+</div><div class="metric-lbl">현지화 총 경력</div></div>
  <div class="metric"><div class="metric-val">7개</div><div class="metric-lbl">인하우스 관리 언어</div></div>
  <div class="metric"><div class="metric-val">1,000만</div><div class="metric-lbl">스페인어 채널 구독자</div></div>
  <div class="metric"><div class="metric-val">700편+</div><div class="metric-lbl">현지화 콘텐츠 처리량</div></div>
</div>

<!-- 커리어 타임라인 -->
<div class="sec-label">커리어 타임라인</div>
<div class="timeline-banner">
  <div class="tl-title">경력 흐름 — 언제 무엇을 중점적으로 했는가</div>
  <div class="tl-track">
    <div class="tl-row">
      <div class="tl-dot" style="background:#888"></div>
      <div class="tl-period">2017 – 2018</div>
      <div class="tl-company">펠리스 학원</div>
      <div class="tl-role">스페인어 강사</div>
    </div>
    <div style="display:flex"><div style="width:4px"></div><div class="tl-line"></div></div>
    <div class="tl-row">
      <div class="tl-dot" style="background:#1D9E75"></div>
      <div class="tl-period">2019 – 2022</div>
      <div class="tl-company">더핑크퐁컴퍼니</div>
      <div class="tl-role">콘텐츠 기획 PM · 스페인어 현지화</div>
    </div>
    <div style="display:flex"><div style="width:4px"></div><div class="tl-line"></div></div>
    <div class="tl-row">
      <div class="tl-dot" style="background:#7F77DD"></div>
      <div class="tl-period">2022 – 현재</div>
      <div class="tl-company">Devsisters</div>
      <div class="tl-role">게임 현지화 PM · 7개 언어 LPM · 30명 관리</div>
    </div>
    <div style="display:flex"><div style="width:4px"></div><div class="tl-line"></div></div>
    <div class="tl-row">
      <div class="tl-dot" style="background:#1D9E75;border:2px solid #0F6E56"></div>
      <div class="tl-period" style="color:#0F6E56;font-weight:600">현재</div>
      <div class="tl-company" style="color:#0F6E56">다음 포지션 탐색 중</div>
      <div class="tl-role">콘텐츠 결과물에 더 직접적으로 기여할 수 있는 역할</div>
    </div>
  </div>
</div>

<!-- 프로젝트 -->
<div class="sec-label">프로젝트</div>
<div class="tab-row">
  <span class="tab active">전체</span>
  <span class="tab">콘텐츠 기획</span>
  <span class="tab">게임 현지화</span>
  <span class="tab">인하우스 운영</span>
  <span class="tab">프리랜서</span>
</div>
<div class="proj-grid">

  <div class="proj-card">
    <div class="proj-tag">더핑크퐁컴퍼니 · 2019–2022 · 콘텐츠 기획 PM</div>
    <div class="proj-title">스페인어 채널 성장 전략 — 구독자 200만 → 1,000만</div>
    <div class="proj-desc">스페인어권 현지 문화를 반영한 로컬 오리지널 콘텐츠 기획·제작 총괄. 시장 조사부터 스튜디오 선정, 성우 캐스팅, 녹음 디렉팅, 포스트 프로덕션까지 전 과정 PM.</div>
    <ul class="proj-results">
      <li class="dot-teal">3년 만에 구독자 5배 성장, 경쟁사 벤치마킹 사례로 업계 확산</li>
      <li class="dot-teal">Samsung TV PLUS 멕시코 Baby Shark — 오픈 1달 키즈 카테고리 2위</li>
    </ul>
    <div class="proj-tags">
      <span class="badge b-teal" style="font-size:11px">콘텐츠 전략</span>
      <span class="badge b-amber" style="font-size:11px">스페인어</span>
      <span class="badge b-blue" style="font-size:11px">제작 PM</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-tag">Devsisters · 2022–현재 · 게임 현지화 PM</div>
    <div class="proj-title">쿠키런: 킹덤 스페인어 현지화 — 20만 단어 · 커뮤니티 바이럴</div>
    <div class="proj-desc">한글→스페인어 현지화 및 LQA 수행. 캐릭터 특성을 살린 초월번역으로 스페인어권·영미권 커뮤니티 자발적 바이럴 달성 (reddit, X, Facebook).</div>
    <ul class="proj-results">
      <li class="dot-blue">총 200,000단어 처리, 용어집·스타일 가이드 신규 수립</li>
      <li class="dot-blue">Don Carlos 현지화 — 업데이트 당시 스페인어권 커뮤니티 최다 바이럴</li>
    </ul>
    <div class="proj-tags">
      <span class="badge b-coral" style="font-size:11px">게임 현지화</span>
      <span class="badge b-amber" style="font-size:11px">LQA</span>
      <span class="badge b-purple" style="font-size:11px">용어집 수립</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-tag">Devsisters · 2022–현재 · 인하우스 LPM</div>
    <div class="proj-title">7개 언어 인하우스팀 운영 + AI 번역 워크플로우 전환</div>
    <div class="proj-desc">영어·스페인어·프랑스어·독일어·일본어·중국어·태국어 7개 언어 번역팀 LPM. 30명 관리. 사내 AI 번역 툴 TF 현지화 PM으로 인력 중심 공정을 AI 워크플로우로 전환.</div>
    <ul class="proj-results">
      <li class="dot-purple">운영 효율화: 2인 1제품 → 1인 2제품 체제 전환</li>
      <li class="dot-purple">AI 프롬프트·Post-processing 로직 설계, 스페인어 QA 기준 수립</li>
    </ul>
    <div class="proj-tags">
      <span class="badge b-purple" style="font-size:11px">팀 리더십</span>
      <span class="badge b-teal" style="font-size:11px">워크플로우 설계</span>
      <span class="badge b-gray" style="font-size:11px">AI 번역</span>
    </div>
  </div>

  <div class="proj-card">
    <div class="proj-tag">더핑크퐁컴퍼니 · 콘텐츠 기획</div>
    <div class="proj-title">스페인어 오리지널 동요 시리즈 기획 — Chumbala Cachumbala</div>
    <div class="proj-desc">스페인어권 전래동요를 재해석한 오리지널 시리즈 10편 기획·제작 PM. 스튜디오 선정, 성우 캐스팅, 녹음 디렉팅 전담.</div>
    <ul class="proj-results">
      <li class="dot-teal">대표 영상 8천만, 시리즈 합산 조회수 2억 6천만</li>
      <li class="dot-teal">경쟁사 벤치마킹 사례로 업계 확산</li>
    </ul>
    <div class="proj-tags">
      <span class="badge b-teal" style="font-size:11px">오리지널 기획</span>
      <span class="badge b-amber" style="font-size:11px">스페인어</span>
      <span class="badge b-blue" style="font-size:11px">음원 PM</span>
    </div>
  </div>

</div>

<!-- PM 역할 가시화 -->
<div class="sec-label">PM 역할 가시화 — 내가 실제로 한 것</div>
<div class="pm-card">
  <div class="pm-example">예시: 스페인어 채널 성장 프로젝트 (더핑크퐁컴퍼니)</div>
  <div class="steps">
    <div class="step">
      <div class="step-num">1</div>
      <div>
        <div class="step-title">상황 파악</div>
        <div class="step-desc">스페인어 채널 구독자 정체. 기존 번역 콘텐츠는 현지 문화 반영 없이 직역 위주 → 이탈률 높음. 경쟁 채널 대비 로컬 콘텐츠 부재.</div>
      </div>
    </div>
    <div class="step">
      <div class="step-num">2</div>
      <div>
        <div class="step-title">내 판단과 제안</div>
        <div class="step-desc">스페인어권 전래동요 기반 로컬 오리지널 시리즈 기획 제안. 직접 시장 조사 수행 후 프로덕션 방향·예산 수립하여 내부 승인 획득.</div>
      </div>
    </div>
    <div class="step">
      <div class="step-num">3</div>
      <div>
        <div class="step-title">실행</div>
        <div class="step-desc">스튜디오 선정·계약, 성우 캐스팅 기준 수립, 가사 감수, 녹음 디렉팅, 포스트 프로덕션 QA, 일정·예산·리소스 관리 전담.</div>
      </div>
    </div>
    <div class="step">
      <div class="step-num">4</div>
      <div>
        <div class="step-title">결과</div>
        <div class="step-desc">3년 내 구독자 200만→1,000만. Chumbala Cachumbala 시리즈 합산 조회수 2억 6천만. 경쟁사 벤치마킹 사례로 업계 확산.</div>
      </div>
    </div>
  </div>
</div>

<!-- 프리랜서 -->
<div class="sec-label">프리랜서 경력</div>
<div class="freelance-grid">
  <div class="fl-card">
    <div class="proj-tags" style="margin-bottom:6px"><span class="badge b-coral" style="font-size:11px">Netflix</span></div>
    <div class="fl-title">수리남 스페인어 후시 녹음 디렉팅</div>
    <div class="fl-desc">넷플릭스 오리지널 드라마 스페인어 더빙 디렉팅. 립싱크·자막 타이밍 정밀 검수.</div>
  </div>
  <div class="fl-card">
    <div class="proj-tags" style="margin-bottom:6px"><span class="badge b-blue" style="font-size:11px">Disney+</span></div>
    <div class="fl-title">나인퍼즐 스페인어 후시 녹음 디렉팅</div>
    <div class="fl-desc">디즈니+ 오리지널 스페인어 더빙 디렉팅. 고품질 현지화 납품.</div>
  </div>
  <div class="fl-card">
    <div class="proj-tags" style="margin-bottom:6px"><span class="badge b-teal" style="font-size:11px">콘텐츠</span></div>
    <div class="fl-title">Lotty Friends 동요 현지화 (10국)</div>
    <div class="fl-desc">스페인어 동요 시리즈 10개국 동시 현지화 PM.</div>
  </div>
</div>

<!-- 보유 스킬 -->
<div class="sec-label">보유 스킬</div>
<div class="skill-card">
  <div class="skill-grid">
    <div class="skill-item"><div class="skill-dot" style="background:#1D9E75"></div>Lokalise · Trados · Smartcat</div>
    <div class="skill-item"><div class="skill-dot" style="background:#1D9E75"></div>TM / TB / 스타일 가이드 구축</div>
    <div class="skill-item"><div class="skill-dot" style="background:#378ADD"></div>스페인어 C2 (원어민 수준)</div>
    <div class="skill-item"><div class="skill-dot" style="background:#378ADD"></div>영어 비즈니스 레벨</div>
    <div class="skill-item"><div class="skill-dot" style="background:#7F77DD"></div>콘텐츠 기획 · 음원·영상 기획</div>
    <div class="skill-item"><div class="skill-dot" style="background:#7F77DD"></div>후시 녹음 디렉팅 · LQA</div>
    <div class="skill-item"><div class="skill-dot" style="background:#BA7517"></div>AI 번역 프롬프트 설계</div>
    <div class="skill-item"><div class="skill-dot" style="background:#BA7517"></div>Notion · Jira · Asana · Zapier</div>
  </div>
</div>

<!-- 경력 -->
<div class="sec-label">경력</div>
<div class="career-card">
  <div class="career-row">
    <div>
      <div class="career-company">Devsisters</div>
      <div class="career-role">현지화 프로젝트 매니저 & 팀 리더 · 7개 언어 인하우스 LPM</div>
    </div>
    <div class="career-period">2022.09 – 현재</div>
  </div>
  <div class="career-row">
    <div>
      <div class="career-company">더핑크퐁컴퍼니</div>
      <div class="career-role">스페인어 유튜브 콘텐츠 기획 PM · 스페인어 현지화 매니저</div>
    </div>
    <div class="career-period">2019.01 – 2022.03</div>
  </div>
  <div class="career-row">
    <div>
      <div class="career-company">펠리스 스페인어 학원</div>
      <div class="career-role">스페인어 강사</div>
    </div>
    <div class="career-period">2017.06 – 2018.12</div>
  </div>
</div>

<!-- 자격증 -->
<div class="sec-label">자격증</div>
<div class="cert-grid">
  <div class="cert-card">
    <div class="cert-year">2016.11</div>
    <div class="cert-name">DELE C2</div>
  </div>
  <div class="cert-card">
    <div class="cert-year">2018.08</div>
    <div class="cert-name">SNULT 스페인어 1급</div>
  </div>
  <div class="cert-card">
    <div class="cert-year">2018.09</div>
    <div class="cert-name">FLEX 스페인어 1A급</div>
  </div>
</div>

</div>
</body>
</html>
