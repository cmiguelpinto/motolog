<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="theme-color" content="#f6f7f9" />
    <meta name="description" content="MotoLog — a calm, modern home for every car expense." />
    <title>MotoLog — Car expenses, simplified</title>
    <style>
      #boot-screen{min-height:100vh;display:grid;place-items:center;background:#f4f6f5;color:#1d2724;font-family:Arial,sans-serif}
      #boot-card{width:min(430px,calc(100% - 40px));padding:36px;background:#fff;border:1px solid #e4e8e6;border-radius:22px;text-align:center;box-shadow:0 24px 70px #173f3515}
      #boot-logo{width:50px;height:50px;display:grid;place-items:center;margin:0 auto 18px;border-radius:14px;background:#173f35;color:#fff;font-size:24px;font-weight:700}
      #boot-card h1{margin:0 0 8px;font-size:25px}#boot-card p{margin:0;color:#75807c;font-size:13px;line-height:1.5}
      #boot-error{display:none;margin-top:18px;padding:12px;border-radius:10px;background:#fff1ee;color:#8f3c2d;font-size:11px;text-align:left;word-break:break-word}
    </style>
    <script>
      window.__motologBootError = function (message) {
        var box = document.getElementById('boot-error');
        var status = document.getElementById('boot-status');
        if (status) status.textContent = 'The app could not start.';
        if (box) { box.style.display = 'block'; box.textContent = String(message || 'Unknown startup error'); }
      };
      window.addEventListener('error', function (event) { window.__motologBootError(event.message || 'A required app file did not load.'); });
      window.addEventListener('unhandledrejection', function (event) { window.__motologBootError(event.reason && (event.reason.message || event.reason)); });
    </script>
    <script type="module" crossorigin src="./assets/index-BqBqy4JD.js"></script>
    <link rel="stylesheet" crossorigin href="./assets/index-tAOtGQOW.css">
  </head>
  <body>
    <div id="root">
      <div id="boot-screen"><div id="boot-card"><div id="boot-logo">M</div><h1>MotoLog</h1><p id="boot-status">Starting your garage…</p><div id="boot-error"></div></div></div>
    </div>
  </body>
</html>
