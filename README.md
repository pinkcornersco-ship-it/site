<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Pink Corners — Junk Removal</title>
  <meta name="description" content="Fast, friendly junk removal across the Sacramento area. Pink Corners." />
  <style>
    :root {
      --pink: #ff2e8a;
      --text: #111;
      --muted: #555;
      --bg0: #f7f7f8; /* top */
      --bg1: #ededf0;
      --bg2: #e3e3e8;
      --bg3: #d9d9df; /* bottom */
    }
    html, body {
      height: 100%;
    }
    body {
      margin: 0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Inter, Arial, sans-serif;
      color: var(--text);
      background: linear-gradient(180deg, var(--bg0), var(--bg3));
      display: grid;
      place-items: center;
    }
    .card {
      position: relative;
      width: min(880px, 92vw);
      border-radius: 24px;
      background: white;
      box-shadow: 0 10px 30px rgba(0,0,0,.07);
      overflow: hidden;
    }
    .wrap { padding: clamp(20px, 4vw, 40px); }
    header { display: flex; align-items: center; justify-content: space-between; gap: 16px; }
    .brand { display: flex; align-items: center; gap: 12px; font-weight: 800; letter-spacing: .4px; }
    .brand .dot { width: 12px; height: 12px; background: var(--pink); border-radius: 3px; transform: rotate(45deg); }
    .brand b { font-size: clamp(20px, 3vw, 28px); }
    .call {
      display: inline-flex; align-items: center; gap: .6rem;
      border: 2px solid var(--pink); color: var(--pink); text-decoration: none; font-weight: 700;
      padding: .6rem 1rem; border-radius: 999px; transition: .15s ease;
    }
    .call:hover { background: var(--pink); color: white; }

    .hero { margin: clamp(20px, 3vw, 32px) 0 10px; }
    h1 { font-size: clamp(28px, 5vw, 44px); margin: 0 0 10px; line-height: 1.08; }
    p.lead { margin: 0; color: var(--muted); font-size: clamp(14px, 2.5vw, 18px); }

    .badges { display: flex; flex-wrap: wrap; gap: 10px; margin: 22px 0 4px; }
    .badge { border: 1px solid #e7e7ea; background: #fafafb; padding: 8px 12px; border-radius: 999px; font-size: 14px; }

    footer { display: grid; gap: 6px; margin-top: 24px; font-size: 14px; color: #666; }

    /* signature pink corners */
    .corner { position: absolute; width: 64px; height: 64px; border: 6px solid var(--pink); border-left: none; border-bottom: none; transform: rotate(45deg); opacity: .9; }
    .corner.tr { top: -18px; right: -18px; }
    .corner.bl { bottom: -18px; left: -18px; transform: rotate(225deg); }

    @media (prefers-color-scheme: dark) {
      body { color: #e9e9ef; }
      .card { background: #121216; }
      .badge { border-color: #2a2a32; background: #17171c; }
      .call { border-color: var(--pink); color: var(--pink); }
    }
  </style>
</head>
<body>
  <main class="card" role="main">
    <i aria-hidden class="corner tr"></i>
    <i aria-hidden class="corner bl"></i>

    <div class="wrap">
      <header>
        <div class="brand"><span class="dot"></span><b>Pink Corners</b><span class="sub" style="font-weight:600;color:#666">Junk Removal</span></div>
        <a class="call" href="tel:9165005555" aria-label="Call Pink Corners">Call 916‑500‑5555</a>
      </header>

      <section class="hero">
        <h1>Fast, friendly junk removal.</h1>
        <p class="lead">From Sacramento to Granite Bay and beyond — same‑day pickups, transparent pricing, and a tidy finish.</p>
        <div class="badges">
          <span class="badge">18 cu yd trailer</span>
          <span class="badge">Cash • Cards • Apple/Google/Samsung Pay • Checks</span>
          <span class="badge">Licensed & Insured</span>
        </div>
      </section>

      <footer>
        <span>Service area: Sacramento, Fair Oaks, Carmichael, Orangevale, Folsom, Granite Bay, Roseville, Citrus Heights, Antelope, Rio Linda, Rocklin, Lincoln, Auburn, North Auburn, Newcastle, Loomis.</span>
        <span>Email: <a href="mailto:hello@pinkcorners.example">hello@pinkcorners.example</a></span>
      </footer>
    </div>
  </main>
</body>
</html>
