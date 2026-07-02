---
title: frog-im
description: frog-im official app support, web apps, and store links.
---

<style>
  :root {
    color-scheme: light;
    --bg: #f6f8fb;
    --panel: #ffffff;
    --ink: #172033;
    --muted: #5f6f86;
    --line: #dce4ef;
    --primary: #0f766e;
    --primary-dark: #115e59;
    --accent: #f5b301;
    --soft: #e7f5f2;
    --shadow: 0 18px 50px rgba(23, 32, 51, 0.12);
  }

  body {
    margin: 0;
    background: var(--bg);
    color: var(--ink);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Noto Sans KR", Arial, sans-serif;
  }

  .page {
    width: min(1120px, calc(100% - 32px));
    margin: 0 auto;
  }

  .hero {
    display: grid;
    grid-template-columns: minmax(0, 1.08fr) minmax(280px, 0.92fr);
    gap: 28px;
    align-items: center;
    padding: 56px 0 34px;
  }

  .eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    margin: 0 0 14px;
    padding: 7px 11px;
    border: 1px solid rgba(15, 118, 110, 0.2);
    border-radius: 999px;
    background: var(--soft);
    color: var(--primary-dark);
    font-size: 14px;
    font-weight: 700;
  }

  h1 {
    margin: 0;
    color: var(--ink);
    font-size: clamp(38px, 7vw, 68px);
    line-height: 1.02;
    letter-spacing: 0;
  }

  .lead {
    margin: 18px 0 0;
    max-width: 660px;
    color: var(--muted);
    font-size: 18px;
    line-height: 1.7;
  }

  .actions {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 28px;
  }

  .button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 48px;
    padding: 0 18px;
    border-radius: 8px;
    border: 1px solid transparent;
    font-weight: 800;
    text-decoration: none;
  }

  .button.primary {
    background: var(--primary);
    color: #ffffff;
  }

  .button.secondary {
    background: var(--panel);
    color: var(--ink);
    border-color: var(--line);
  }

  .button.store {
    background: #202633;
    color: #ffffff;
  }

  .showcase {
    position: relative;
    min-height: 360px;
    border-radius: 8px;
    overflow: hidden;
    background:
      radial-gradient(circle at 72% 20%, rgba(245, 179, 1, 0.45), transparent 26%),
      linear-gradient(145deg, #0f766e, #123b55);
    box-shadow: var(--shadow);
  }

  .phone {
    position: absolute;
    inset: 36px 52px 28px auto;
    width: 230px;
    min-height: 292px;
    border: 10px solid #182235;
    border-radius: 30px;
    background: #f9fbff;
    box-shadow: 0 22px 46px rgba(0, 0, 0, 0.24);
  }

  .phone-screen {
    padding: 24px 18px;
  }

  .ticket-title {
    margin: 0 0 18px;
    color: #143f6b;
    font-size: 18px;
    font-weight: 900;
  }

  .balls {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .ball {
    display: grid;
    width: 52px;
    height: 52px;
    place-items: center;
    border-radius: 999px;
    background: var(--accent);
    color: #172033;
    font-size: 20px;
    font-weight: 900;
    box-shadow: inset 0 -5px 0 rgba(0, 0, 0, 0.12);
  }

  .mini-card {
    position: absolute;
    left: 28px;
    bottom: 32px;
    width: 190px;
    padding: 18px;
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.92);
    color: var(--ink);
  }

  .mini-card strong {
    display: block;
    margin-bottom: 6px;
    font-size: 18px;
  }

  .section {
    padding: 30px 0;
  }

  .section h2 {
    margin: 0 0 16px;
    font-size: 28px;
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 14px;
  }

  .card {
    border: 1px solid var(--line);
    border-radius: 8px;
    background: var(--panel);
    padding: 18px;
  }

  .card h3 {
    margin: 0 0 8px;
    font-size: 19px;
  }

  .card p {
    margin: 0 0 14px;
    color: var(--muted);
    line-height: 1.6;
  }

  .link-list {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 10px;
  }

  .small-link {
    color: var(--primary-dark);
    font-weight: 800;
    text-decoration: none;
  }

  .small-note {
    color: var(--muted);
    font-weight: 700;
  }

  .support {
    margin: 22px 0 54px;
    border: 1px solid var(--line);
    border-radius: 8px;
    background: var(--panel);
    overflow: hidden;
  }

  .support summary {
    cursor: pointer;
    padding: 18px;
    font-weight: 900;
  }

  .support-content {
    padding: 0 18px 18px;
    color: var(--muted);
    line-height: 1.7;
  }

  .support-content table {
    width: 100%;
    border-collapse: collapse;
    margin: 14px 0;
    color: var(--ink);
  }

  .support-content th,
  .support-content td {
    padding: 10px;
    border: 1px solid var(--line);
    text-align: left;
  }

  @media (max-width: 820px) {
    .hero,
    .grid {
      grid-template-columns: 1fr;
    }

    .hero {
      padding-top: 34px;
    }

    .showcase {
      min-height: 330px;
    }

    .phone {
      right: 22px;
      width: 210px;
    }

    .mini-card {
      left: 18px;
      width: 150px;
    }
  }
</style>

<main class="page">
  <section class="hero" aria-labelledby="home-title">
    <div>
      <p class="eyebrow">frog-im official website</p>
      <h1 id="home-title">frog-im</h1>
      <p class="lead">
        앱 지원, 개인정보처리방침, 스토어 링크와 웹에서 바로 실행할 수 있는 Power Lucky Lotto를 한 곳에서 제공합니다.
      </p>
      <div class="actions">
        <a class="button primary" href="/picker/">뽑기박스 웹 실행</a>
        <a class="button primary" href="/lotto/">Power Lucky Lotto 웹 실행</a>
        <a class="button store" href="https://play.google.com/store/apps/details?id=com.github.frogim.powerluckylotto&pcampaignid=web_share">Power Lucky Lotto 스토어</a>
        <a class="button secondary" href="#support">지원 문의</a>
      </div>
    </div>

    <div class="showcase" aria-label="Power Lucky Lotto preview">
      <div class="phone">
        <div class="phone-screen">
          <p class="ticket-title">Power Lucky Lotto</p>
          <div class="balls" aria-hidden="true">
            <span class="ball">7</span>
            <span class="ball">12</span>
            <span class="ball">19</span>
            <span class="ball">28</span>
            <span class="ball">34</span>
            <span class="ball">41</span>
          </div>
        </div>
      </div>
      <div class="mini-card">
        <strong>Web app</strong>
        설치 없이 브라우저에서 바로 실행
      </div>
    </div>
  </section>

  <section class="section" aria-labelledby="quick-links">
    <h2 id="quick-links">바로가기</h2>
    <div class="grid">
      <article class="card">
        <h3>Lucky Pick Box Web</h3>
        <p>사다리, 돌림판, 제비뽑기, 팀 나누기 등을 웹에 맞춘 작업대 UI로 실행합니다.</p>
        <a class="button primary" href="/picker/">/picker 열기</a>
      </article>
      <article class="card">
        <h3>Power Lucky Lotto Web</h3>
        <p>기존 Flutter Web 빌드를 GitHub Pages의 `/lotto` 경로에서 실행합니다.</p>
        <a class="button primary" href="/lotto/">/lotto 열기</a>
      </article>
      <article class="card">
        <h3>Google Play</h3>
        <p>Power Lucky Lotto의 Google Play 스토어 페이지로 이동합니다.</p>
        <a class="button store" href="https://play.google.com/store/apps/details?id=com.github.frogim.powerluckylotto&pcampaignid=web_share">스토어 이동</a>
      </article>
      <article class="card">
        <h3>Support</h3>
        <p>앱 문의, 결제 문제, 데이터 삭제 요청은 이메일로 접수합니다.</p>
        <a class="button secondary" href="mailto:g.ns.0700g@gmail.com">g.ns.0700g@gmail.com</a>
      </article>
    </div>
  </section>

  <section class="section" aria-labelledby="apps">
    <h2 id="apps">앱과 정책</h2>
    <div class="grid">
      <article class="card">
        <h3>Power Lucky Lotto</h3>
        <p>로또 번호 생성 앱입니다. 웹앱과 Google Play 모두 제공됩니다.</p>
        <div class="link-list">
          <a class="small-link" href="/lotto/">웹앱</a>
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.powerluckylotto&pcampaignid=web_share">Google Play</a>
          <a class="small-link" href="/privacy/Power%20lucky%20lotto/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>LyriFloat</h3>
        <p>Power Audio Tag Editor 앱 지원 및 개인정보처리방침입니다.</p>
        <div class="link-list">
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.lyrifloat&pcampaignid=web_share">Google Play</a>
          <a class="small-link" href="/privacy/bbo-music-player/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>Air Caption</h3>
        <p>Power Subtitle Editor & Player 앱 지원 및 개인정보처리방침입니다.</p>
        <div class="link-list">
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.aircaption.air_caption&pcampaignid=web_share">Google Play</a>
          <a class="small-link" href="/privacy/Subtitle%20Player%20%26%20Editor/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>KnowMe</h3>
        <p>KnowMe 앱 지원 및 개인정보처리방침입니다.</p>
        <div class="link-list">
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.knowme&pcampaignid=web_share">Google Play</a>
          <a class="small-link" href="/privacy/know%20me/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>QDiary</h3>
        <p>QuestDiary 앱 지원, 개인정보처리방침, 데이터 삭제 요청입니다.</p>
        <div class="link-list">
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.pr.confessionjournal.confession_journal&pcampaignid=web_share">Google Play</a>
          <a class="small-link" href="/privacy/Quest_Diary/en/">개인정보처리방침</a>
          <a class="small-link" href="https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog">데이터 삭제</a>
        </div>
      </article>
      <article class="card">
        <h3>Lucky Pick Box</h3>
        <p>랜덤 뽑기 도구 모음입니다. 웹 버전과 Google Play에서 제공됩니다.</p>
        <div class="link-list">
          <a class="small-link" href="/picker/">웹앱</a>
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.drawing_lots">Google Play</a>
          <a class="small-link" href="/privacy/Lucky%20Pick%20Box/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>TimeBack</h3>
        <p>과거의 기록을 돌아볼 수 있는 앱입니다. Google Play와 개인정보처리방침을 제공합니다.</p>
        <div class="link-list">
          <a class="small-link" href="https://play.google.com/store/apps/details?id=com.github.frogim.timeBack.time_back">Google Play</a>
          <a class="small-link" href="/privacy/TimeBack/ko/">개인정보처리방침</a>
        </div>
      </article>
      <article class="card">
        <h3>FileGuard</h3>
        <p>파일을 안전하게 보관하는 신규 앱입니다.</p>
        <div class="link-list">
          <span class="small-note">Google Play 링크 추가 예정</span>
          <a class="small-link" href="/privacy/File%20Guard/ko/">개인정보처리방침</a>
        </div>
      </article>
    </div>
  </section>

  <details id="support" class="support" open>
    <summary>App Support</summary>
    <div class="support-content">
      <p><strong>Developer:</strong> frog-im<br>
      <strong>Support Email:</strong> <a href="mailto:g.ns.0700g@gmail.com">g.ns.0700g@gmail.com</a><br>
      <strong>Response Time:</strong> Within 3 business days<br>
      <strong>Business Hours:</strong> Mon-Fri, 10:00-17:00 KST</p>

      <p>본 페이지는 frog-im이 배포하는 앱의 공식 지원 페이지이며 Google Play 개발자 연락처 웹사이트로 제공됩니다.</p>

      <table>
        <thead>
          <tr>
            <th>요청 유형</th>
            <th>처리 방법</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>버그 제보</td>
            <td>앱 이름, 앱 버전, 기기, OS 버전, 재현 방법, 스크린샷 또는 녹화 영상을 이메일에 포함해 주세요.</td>
          </tr>
          <tr>
            <td>결제 및 환불</td>
            <td>Google Play 결제 및 환불 정책을 따릅니다. 주문번호 또는 영수증을 함께 보내 주세요.</td>
          </tr>
          <tr>
            <td>개인정보 및 데이터 삭제</td>
            <td>앱 이름, 요청 유형, 관련 계정 또는 데이터를 확인하는 데 필요한 정보를 포함해 이메일로 요청해 주세요.</td>
          </tr>
        </tbody>
      </table>
    </div>
  </details>
</main>
