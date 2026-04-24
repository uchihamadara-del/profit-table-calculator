<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Forex Profit Calculator — 10 Pips / 1 Lot</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@300;400;500&family=Syne:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --bg:        #0b0e14;
    --surface:   #11151e;
    --surface2:  #181d29;
    --border:    rgba(255,255,255,0.07);
    --border2:   rgba(255,255,255,0.13);
    --text:      #e8ecf4;
    --muted:     #6b7690;
    --accent:    #00e5a0;
    --accent2:   #0099ff;
    --gold:      #f5c542;
    --red:       #ff5e5e;

    --eur: #7b6cf5;
    --gbp: #f97bb0;
    --usd: #00e5a0;
    --jpy: #f5c542;
    --chf: #4eb6ff;
    --cad: #ff8c5e;
    --aud: #6dd67a;
    --nzd: #d06bf5;
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Syne', sans-serif;
    min-height: 100vh;
    padding: 40px 20px 80px;
  }

  /* ── Header ─────────────────────────────────── */
  header {
    max-width: 1100px;
    margin: 0 auto 40px;
    display: flex;
    flex-wrap: wrap;
    align-items: flex-end;
    justify-content: space-between;
    gap: 20px;
  }

  .brand { line-height: 1.2; }
  .brand-label {
    font-size: 10px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 6px;
  }
  .brand-title {
    font-size: clamp(26px, 4vw, 40px);
    font-weight: 800;
    background: linear-gradient(90deg, var(--accent), var(--accent2));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    letter-spacing: -0.02em;
  }
  .brand-sub {
    font-size: 13px;
    color: var(--muted);
    margin-top: 4px;
    font-family: 'DM Mono', monospace;
    font-weight: 300;
  }

  .inputs {
    display: flex;
    gap: 14px;
    flex-wrap: wrap;
    align-items: flex-end;
  }
  .input-group { display: flex; flex-direction: column; gap: 5px; }
  .input-group label {
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
  }
  .input-group input {
    width: 90px;
    background: var(--surface);
    border: 0.5px solid var(--border2);
    border-radius: 8px;
    color: var(--text);
    font-family: 'DM Mono', monospace;
    font-size: 15px;
    padding: 8px 12px;
    outline: none;
    transition: border-color 0.2s;
  }
  .input-group input:focus { border-color: var(--accent); }

  /* ── Stats bar ───────────────────────────────── */
  .stats-bar {
    max-width: 1100px;
    margin: 0 auto 32px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 12px;
  }
  .stat-card {
    background: var(--surface);
    border: 0.5px solid var(--border);
    border-radius: 12px;
    padding: 16px 20px;
  }
  .stat-label {
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 6px;
  }
  .stat-value {
    font-family: 'DM Mono', monospace;
    font-size: 22px;
    font-weight: 500;
    color: var(--accent);
  }
  .stat-pair {
    font-size: 11px;
    color: var(--muted);
    margin-top: 2px;
    font-family: 'DM Mono', monospace;
  }

  /* ── Filter tabs ─────────────────────────────── */
  .filter-section {
    max-width: 1100px;
    margin: 0 auto 20px;
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    align-items: center;
  }
  .filter-label {
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    margin-right: 4px;
  }
  .filter-btn {
    background: var(--surface);
    border: 0.5px solid var(--border);
    border-radius: 6px;
    color: var(--muted);
    cursor: pointer;
    font-family: 'Syne', sans-serif;
    font-size: 12px;
    font-weight: 600;
    letter-spacing: 0.08em;
    padding: 6px 14px;
    transition: all 0.18s;
    text-transform: uppercase;
  }
  .filter-btn:hover { border-color: var(--border2); color: var(--text); }
  .filter-btn.active {
    color: var(--bg);
    border-color: transparent;
  }
  .filter-btn[data-currency="ALL"].active { background: var(--accent); }
  .filter-btn[data-currency="EUR"].active { background: var(--eur); }
  .filter-btn[data-currency="GBP"].active { background: var(--gbp); }
  .filter-btn[data-currency="USD"].active { background: var(--usd); }
  .filter-btn[data-currency="JPY"].active { background: var(--jpy); }
  .filter-btn[data-currency="CHF"].active { background: var(--chf); }
  .filter-btn[data-currency="CAD"].active { background: var(--cad); }
  .filter-btn[data-currency="AUD"].active { background: var(--aud); }
  .filter-btn[data-currency="NZD"].active { background: var(--nzd); }

  /* ── Table ───────────────────────────────────── */
  .table-wrap {
    max-width: 1100px;
    margin: 0 auto;
    overflow-x: auto;
    border-radius: 14px;
    border: 0.5px solid var(--border);
  }

  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 13px;
    min-width: 680px;
  }

  thead th {
    background: var(--surface2);
    font-size: 10px;
    font-weight: 600;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--muted);
    padding: 14px 18px;
    text-align: left;
    border-bottom: 0.5px solid var(--border);
    white-space: nowrap;
    cursor: pointer;
    user-select: none;
    transition: color 0.15s;
  }
  thead th:hover { color: var(--text); }
  thead th.sorted { color: var(--accent); }
  .sort-icon { margin-left: 4px; opacity: 0.4; }
  thead th.sorted .sort-icon { opacity: 1; }

  /* Group header rows */
  tr.group-header td {
    background: var(--surface2);
    padding: 10px 18px 8px;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    border-bottom: 0.5px solid var(--border);
    border-top: 0.5px solid var(--border);
  }
  tr.group-header .group-pill {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 3px 12px 3px 8px;
    border-radius: 20px;
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 0.1em;
  }
  tr.group-header .group-dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    display: inline-block;
  }

  tbody tr.data-row {
    transition: background 0.12s;
    border-bottom: 0.5px solid var(--border);
  }
  tbody tr.data-row:hover { background: rgba(255,255,255,0.025); }
  tbody tr.data-row:last-child { border-bottom: none; }

  td { padding: 11px 18px; vertical-align: middle; }

  td.symbol {
    font-family: 'DM Mono', monospace;
    font-size: 14px;
    font-weight: 500;
    letter-spacing: 0.06em;
    white-space: nowrap;
  }
  .sym-base { color: var(--text); }
  .sym-sep  { color: var(--muted); margin: 0 1px; }
  .sym-quote { color: var(--muted); }

  td.rate {
    font-family: 'DM Mono', monospace;
    font-size: 12px;
    color: var(--muted);
  }

  td.pip-val {
    font-family: 'DM Mono', monospace;
    font-size: 13px;
    color: var(--muted);
  }

  td.profit {
    font-family: 'DM Mono', monospace;
    font-size: 15px;
    font-weight: 500;
    color: var(--accent);
  }

  td.quote-badge { width: 60px; }
  .badge {
    display: inline-block;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 0.1em;
    padding: 3px 9px;
    border-radius: 20px;
  }

  .badge-EUR { background: rgba(123,108,245,0.15); color: var(--eur); }
  .badge-GBP { background: rgba(249,123,176,0.15); color: var(--gbp); }
  .badge-USD { background: rgba(0,229,160,0.12); color: var(--usd); }
  .badge-JPY { background: rgba(245,197,66,0.15); color: var(--jpy); }
  .badge-CHF { background: rgba(78,182,255,0.15); color: var(--chf); }
  .badge-CAD { background: rgba(255,140,94,0.15); color: var(--cad); }
  .badge-AUD { background: rgba(109,214,122,0.15); color: var(--aud); }
  .badge-NZD { background: rgba(208,107,245,0.15); color: var(--nzd); }

  /* Group color dots */
  .dot-EUR { background: var(--eur); }
  .dot-GBP { background: var(--gbp); }
  .dot-USD { background: var(--usd); }
  .dot-JPY { background: var(--jpy); }
  .dot-CHF { background: var(--chf); }
  .dot-CAD { background: var(--cad); }
  .dot-AUD { background: var(--aud); }
  .dot-NZD { background: var(--nzd); }

  /* Group pill text colors */
  .pill-EUR { color: var(--eur); background: rgba(123,108,245,0.1); }
  .pill-GBP { color: var(--gbp); background: rgba(249,123,176,0.1); }
  .pill-USD { color: var(--usd); background: rgba(0,229,160,0.08); }
  .pill-JPY { color: var(--jpy); background: rgba(245,197,66,0.1); }
  .pill-CHF { color: var(--chf); background: rgba(78,182,255,0.1); }
  .pill-CAD { color: var(--cad); background: rgba(255,140,94,0.1); }
  .pill-AUD { color: var(--aud); background: rgba(109,214,122,0.1); }
  .pill-NZD { color: var(--nzd); background: rgba(208,107,245,0.1); }

  .hidden { display: none; }

  /* ── No results ───────────────────────────────── */
  .empty-state {
    text-align: center;
    padding: 60px 20px;
    color: var(--muted);
    font-size: 14px;
    display: none;
  }

  /* ── Footer note ─────────────────────────────── */
  .foot-note {
    max-width: 1100px;
    margin: 24px auto 0;
    font-size: 11px;
    color: var(--muted);
    font-family: 'DM Mono', monospace;
    line-height: 1.8;
    border-top: 0.5px solid var(--border);
    padding-top: 16px;
  }

  @media (max-width: 600px) {
    .inputs { gap: 10px; }
    .input-group input { width: 80px; font-size: 14px; }
    td, th { padding: 10px 12px; }
  }
</style>
</head>
<body>

<header>
  <div class="brand">
    <div class="brand-label">Forex Analytics</div>
    <div class="brand-title">Profit Calculator</div>
    <div class="brand-sub">1 lot · 10 points · USD result</div>
  </div>
  <div class="inputs">
    <div class="input-group">
      <label>Lots</label>
      <input type="number" id="lots" value="1" min="0.01" step="0.01">
    </div>
    <div class="input-group">
      <label>Points</label>
      <input type="number" id="points" value="10" min="1" step="1">
    </div>
  </div>
</header>

<div class="stats-bar" id="stats-bar"></div>

<div class="filter-section">
  <span class="filter-label">Base currency</span>
  <button class="filter-btn active" data-currency="ALL">All</button>
  <button class="filter-btn" data-currency="EUR">EUR</button>
  <button class="filter-btn" data-currency="GBP">GBP</button>
  <button class="filter-btn" data-currency="USD">USD</button>
  <button class="filter-btn" data-currency="JPY">JPY</button>
  <button class="filter-btn" data-currency="CHF">CHF</button>
  <button class="filter-btn" data-currency="CAD">CAD</button>
  <button class="filter-btn" data-currency="AUD">AUD</button>
  <button class="filter-btn" data-currency="NZD">NZD</button>
</div>

<div class="table-wrap">
  <table id="main-table">
    <thead>
      <tr>
        <th onclick="sortBy('symbol')">Symbol <span class="sort-icon" id="sort-symbol">↕</span></th>
        <th onclick="sortBy('rate')">Rate <span class="sort-icon" id="sort-rate">↕</span></th>
        <th onclick="sortBy('pipUSD')">Pip value <span class="sort-icon" id="sort-pipUSD">↕</span></th>
        <th onclick="sortBy('profit')">Profit (USD) <span class="sort-icon" id="sort-profit">↕</span></th>
        <th>Quote</th>
      </tr>
    </thead>
    <tbody id="tbody"></tbody>
  </table>
  <div class="empty-state" id="empty">No pairs match this filter.</div>
</div>

<div class="foot-note" id="foot-note">
  ⓘ Rates: approximate April 2026 market values &nbsp;·&nbsp;
  Standard lot = 100,000 units &nbsp;·&nbsp;
  Pip size: 0.0001 (non-JPY) | 0.01 (JPY) &nbsp;·&nbsp;
  Cross pairs converted via USD rates &nbsp;·&nbsp;
  Grouped by base currency
</div>

<script>
const BASE_RATES = {
  EURUSD:1.1340, GBPUSD:1.3320, USDJPY:142.50, USDCHF:0.8180,
  AUDUSD:0.6390, NZDUSD:0.5930, USDCAD:1.3840,
  EURJPY:161.60, AUDNZD:1.0780, EURNZD:1.9120, AUDCAD:0.8840,
  EURCAD:1.5700, AUDCHF:0.5230, GBPCHF:1.0900, AUDJPY:91.05,
  GBPJPY:189.90, CHFJPY:174.20, CADCHF:0.5910, EURGBP:0.8510,
  CADJPY:103.00, EURAUD:1.7750, GBPAUD:2.0840, EURCHF:0.9280,
  GBPCAD:1.8430, GBPNZD:2.2470, NZDJPY:84.50, NZDCAD:0.8200, NZDCHF:0.4870
};

const CURRENCY_ORDER = ['EUR','GBP','USD','AUD','NZD','CAD','CHF','JPY'];
const COLOR_MAP = {EUR:'var(--eur)',GBP:'var(--gbp)',USD:'var(--usd)',AUD:'var(--aud)',NZD:'var(--nzd)',CAD:'var(--cad)',CHF:'var(--chf)',JPY:'var(--jpy)'};

function pipValueUSD(sym, rate) {
  const quote = sym.slice(3);
  const pip = sym.includes('JPY') ? 0.01 : 0.0001;
  const piq = 100000 * pip;
  if (quote==='USD') return piq;
  if (quote==='JPY') return piq / rate;
  if (quote==='CHF') return piq / BASE_RATES.USDCHF;
  if (quote==='CAD') return piq / BASE_RATES.USDCAD;
  if (quote==='AUD') return piq * BASE_RATES.AUDUSD;
  if (quote==='NZD') return piq * BASE_RATES.NZDUSD;
  if (quote==='GBP') return piq * BASE_RATES.GBPUSD;
  if (quote==='EUR') return piq * BASE_RATES.EURUSD;
  return piq;
}

let sortKey='profit', sortDir=-1, activeFilter='ALL';

function sortBy(key) {
  if (sortKey===key) sortDir*=-1; else {sortKey=key; sortDir=1;}
  render();
}

function render() {
  const lots   = parseFloat(document.getElementById('lots').value)||1;
  const points = parseFloat(document.getElementById('points').value)||10;

  // Build data
  let rows = Object.entries(BASE_RATES).map(([sym,rate])=>({
    symbol: sym,
    base:   sym.slice(0,3),
    quote:  sym.slice(3),
    rate,
    pipUSD: pipValueUSD(sym,rate),
    profit: pipValueUSD(sym,rate)*lots*points
  }));

  // Filter
  if (activeFilter!=='ALL') rows=rows.filter(r=>r.base===activeFilter);

  // Sort within each group
  rows.sort((a,b)=>{
    const va=a[sortKey], vb=b[sortKey];
    return typeof va==='string'? va.localeCompare(vb)*sortDir : (va-vb)*sortDir;
  });

  // Group by base
  const groups={};
  CURRENCY_ORDER.forEach(c=>{ groups[c]=[]; });
  rows.forEach(r=>{ if(groups[r.base]) groups[r.base].push(r); });

  // Sort icons
  ['symbol','rate','pipUSD','profit'].forEach(k=>{
    const el=document.getElementById('sort-'+k);
    if(!el) return;
    el.textContent = sortKey===k ? (sortDir===1?'↑':'↓') : '↕';
    el.parentElement.className = sortKey===k ? 'sorted' : '';
  });

  // Build tbody HTML
  const tbody = document.getElementById('tbody');
  let html='', totalRows=0;
  CURRENCY_ORDER.forEach(base=>{
    const group=groups[base];
    if(!group||!group.length) return;
    totalRows+=group.length;
    html+=`<tr class="group-header">
      <td colspan="5">
        <span class="group-pill pill-${base}">
          <span class="group-dot dot-${base}"></span>
          ${base} pairs &nbsp;<span style="opacity:0.6;font-size:10px;">(${group.length})</span>
        </span>
      </td>
    </tr>`;
    group.forEach(r=>{
      const rateStr = r.symbol.includes('JPY')? r.rate.toFixed(2) : r.rate.toFixed(4);
      html+=`<tr class="data-row" data-base="${r.base}">
        <td class="symbol">
          <span class="sym-base">${r.base}</span><span class="sym-sep">/</span><span class="sym-quote">${r.quote}</span>
        </td>
        <td class="rate">${rateStr}</td>
        <td class="pip-val">$${r.pipUSD.toFixed(3)}</td>
        <td class="profit">$${r.profit.toFixed(2)}</td>
        <td class="quote-badge"><span class="badge badge-${r.quote}">${r.quote}</span></td>
      </tr>`;
    });
  });
  tbody.innerHTML=html;

  // Empty state
  document.getElementById('empty').style.display = totalRows===0?'block':'none';
  document.getElementById('main-table').style.display = totalRows===0?'none':'table';

  // Stats
  const allRows = Object.values(groups).flat();
  const total = allRows.reduce((s,r)=>s+r.profit,0);
  const max   = allRows.reduce((m,r)=>r.profit>m.profit?r:m, allRows[0]||{profit:-Infinity,symbol:'—'});
  const min   = allRows.reduce((m,r)=>r.profit<m.profit?r:m, allRows[0]||{profit:Infinity,symbol:'—'});
  const avg   = allRows.length ? total/allRows.length : 0;

  document.getElementById('stats-bar').innerHTML=`
    <div class="stat-card">
      <div class="stat-label">Pairs shown</div>
      <div class="stat-value" style="color:var(--text)">${totalRows}</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">Avg profit / trade</div>
      <div class="stat-value">$${avg.toFixed(2)}</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">Highest profit</div>
      <div class="stat-value" style="font-size:18px;color:var(--accent)">$${(max.profit||0).toFixed(2)}</div>
      <div class="stat-pair">${max.symbol||'—'}</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">Lowest profit</div>
      <div class="stat-value" style="font-size:18px;color:var(--muted)">$${(min.profit||0).toFixed(2)}</div>
      <div class="stat-pair">${min.symbol||'—'}</div>
    </div>
    <div class="stat-card">
      <div class="stat-label">Total (all pairs)</div>
      <div class="stat-value" style="font-size:18px">$${total.toFixed(2)}</div>
    </div>
  `;
}

// Filter buttons
document.querySelectorAll('.filter-btn').forEach(btn=>{
  btn.addEventListener('click',()=>{
    document.querySelectorAll('.filter-btn').forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');
    activeFilter=btn.dataset.currency;
    render();
  });
});

document.getElementById('lots').addEventListener('input', render);
document.getElementById('points').addEventListener('input', render);

render();
</script>
</body>
</html>
