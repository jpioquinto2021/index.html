<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nutresa CEO Challenge — Contabilidad Financiera · Politécnico Grancolombiano</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.44.0/tabler-icons.min.css">
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{--poli-navy:#1a3a5c;--poli-blue:#4e9cd8;--poli-line:#4e9cd8}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;background:#f4f4f0;color:#1a1a18;min-height:100vh}
.poli-header{background:var(--poli-navy);padding:1rem 1.5rem;display:flex;align-items:center;gap:1.4rem}
.poli-logo-svg{flex-shrink:0;width:160px}
.poli-divider{width:1px;height:56px;background:rgba(255,255,255,.2);flex-shrink:0}
.poli-course-info{display:flex;flex-direction:column;gap:3px}
.poli-course-info .modulo{font-size:10px;color:rgba(255,255,255,.55);text-transform:uppercase;letter-spacing:.07em}
.poli-course-info .titulo{font-size:17px;font-weight:500;color:#fff}
.poli-course-info .codigo{font-size:12px;color:rgba(255,255,255,.5)}
.poli-professor{margin-left:auto;text-align:right;flex-shrink:0}
.poli-professor .label{font-size:10px;color:rgba(255,255,255,.45);text-transform:uppercase;letter-spacing:.05em}
.poli-professor .prof-name{font-size:14px;font-weight:500;color:#fff}
.poli-professor .role{font-size:11px;color:rgba(255,255,255,.5)}
.poli-underline{height:3px;background:var(--poli-blue)}
.content{padding:1.2rem 1.5rem}
.tip{background:#e6f1fb;border:0.5px solid #85b7eb;border-radius:8px;padding:.6rem 1rem;font-size:12px;color:#185fa5;margin-bottom:12px}
.panel{background:#fff;border:0.5px solid #d3d1c7;border-radius:12px;padding:1rem 1.25rem;margin-bottom:12px}
.section-title{font-size:14px;font-weight:500;margin-bottom:10px;color:#1a1a18}
.top-row{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px}
.game-title{font-size:18px;font-weight:500;color:#1a1a18;margin:0}
.game-sub{font-size:12px;color:#5f5e5a;margin:2px 0 0}
.metric-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:10px;margin-bottom:12px}
.metric{background:#f4f4f0;border-radius:8px;padding:.75rem 1rem}
.metric-label{font-size:12px;color:#5f5e5a;margin-bottom:4px}
.metric-val{font-size:22px;font-weight:500;color:#1a1a18}
.metric-sub{font-size:11px;color:#888780;margin-top:2px}
.slider-row{display:flex;align-items:center;gap:10px;margin-bottom:.9rem}
.slider-row i{font-size:18px;color:#888780;flex-shrink:0}
.slider-label{font-size:13px;color:#5f5e5a;min-width:200px}
.slider-val{font-size:13px;font-weight:500;min-width:48px;text-align:right;color:#1a1a18}
input[type=range]{flex:1;accent-color:#1a3a5c;height:4px;cursor:pointer}
table{width:100%;font-size:13px;border-collapse:collapse}
th{font-size:11px;font-weight:500;color:#888780;text-align:right;padding:5px 8px;border-bottom:0.5px solid #d3d1c7}
th:first-child{text-align:left}
td{padding:5px 8px;text-align:right;color:#1a1a18}
td:first-child{text-align:left;color:#5f5e5a}
tr.hl td{font-weight:500;color:#1a1a18;border-top:0.5px solid #d3d1c7}
.badge{display:inline-block;font-size:11px;padding:2px 8px;border-radius:6px}
.bu{background:#eaf3de;color:#3b6d11}.bd{background:#fcebeb;color:#a32d2d}
.alert{border-radius:8px;padding:.7rem 1rem;font-size:14px;font-weight:500;text-align:center;margin-top:8px}
.alert-red{background:#fcebeb;color:#a32d2d;border:0.5px solid #f09595}
.alert-yellow{background:#faeeda;color:#854f0b;border:0.5px solid #ef9f27}
.alert-green{background:#eaf3de;color:#3b6d11;border:0.5px solid #97c459}
.reset-btn{background:transparent;border:0.5px solid #b4b2a9;border-radius:8px;padding:6px 14px;font-size:12px;color:#5f5e5a;cursor:pointer}
.reset-btn:hover{background:#f4f4f0}
.footer{background:var(--poli-navy);color:rgba(255,255,255,.45);font-size:11px;text-align:center;padding:.8rem 1.5rem;margin-top:1rem}
.footer span{color:var(--poli-blue)}
@media(max-width:600px){.poli-professor{display:none}.slider-label{min-width:110px;font-size:12px}.poli-logo-svg{width:120px}}
</style>
</head>
<body>

<div class="poli-header">
  <!-- Logo SVG recreado fielmente del sitio poli.edu.co -->
  <svg class="poli-logo-svg" viewBox="0 0 200 70" xmlns="http://www.w3.org/2000/svg">
    <!-- Ícono curvo / swoosh -->
    <g>
      <!-- Forma angular izquierda estilo poli -->
      <path d="M8 58 L8 16 Q8 8 16 8 L30 8 Q44 8 44 22 Q44 34 32 36 L22 38 L22 58 Z" fill="none" stroke="#4e9cd8" stroke-width="4" stroke-linejoin="round"/>
      <path d="M22 38 L36 58" fill="none" stroke="#4e9cd8" stroke-width="4" stroke-linecap="round"/>
      <!-- Reflejo interior -->
      <path d="M14 54 L14 18 Q14 14 18 14 L28 14 Q36 14 36 22 Q36 30 28 32 L22 34" fill="none" stroke="rgba(78,156,216,0.35)" stroke-width="2"/>
    </g>
    <!-- POLI texto grande -->
    <text x="52" y="42" font-family="Arial Black,Arial,sans-serif" font-size="28" font-weight="900" fill="#ffffff" letter-spacing="1">POLI</text>
    <!-- Texto pequeño debajo -->
    <text x="52" y="54" font-family="Arial,sans-serif" font-size="7.5" font-weight="600" fill="rgba(255,255,255,0.8)" letter-spacing="1.2">POLITÉCNICO</text>
    <text x="52" y="63" font-family="Arial,sans-serif" font-size="7.5" font-weight="600" fill="rgba(255,255,255,0.8)" letter-spacing="1.2">GRANCOLOMBIANO</text>
    <text x="52" y="70" font-family="Arial,sans-serif" font-size="5.5" fill="rgba(255,255,255,0.5)" letter-spacing=".8">INSTITUCIÓN UNIVERSITARIA</text>
    <!-- Línea azul debajo del logo -->
    <line x1="52" y1="47" x2="196" y2="47" stroke="#4e9cd8" stroke-width="0.8" opacity="0.3"/>
  </svg>

  <div class="poli-divider"></div>

  <div class="poli-course-info">
    <span class="modulo">Módulo · Especialización en Gerencia Financiera</span>
    <span class="titulo">Contabilidad Financiera</span>
    <span class="codigo">Código: ECA52814 · Sesión 1</span>
  </div>

  <div class="poli-professor">
    <p class="label">Docente</p>
    <p class="prof-name">Pio Quinto</p>
    <p class="role">Director de Formación</p>
  </div>
</div>
<div class="poli-underline"></div>

<div class="content">
  <div class="top-row">
    <div>
      <p class="game-title">Nutresa CEO Challenge</p>
      <p class="game-sub">Tablero de decisiones operativas · Análisis vertical y horizontal</p>
    </div>
    <button class="reset-btn" onclick="resetAll()"><i class="ti ti-refresh"></i> Resetear</button>
  </div>

  <div class="tip"><i class="ti ti-bulb"></i> <strong>Misión:</strong> Llevar el Margen EBITDA al 18% usando las 3 palancas. ¿Cuál combinación usarías y por qué?</div>

  <div class="panel">
    <p class="section-title">Palancas de decisión gerencial</p>
    <div class="slider-row">
      <i class="ti ti-trending-up"></i>
      <span class="slider-label">Variación en ventas (precio / volumen)</span>
      <input type="range" min="-5" max="15" step="1" value="0" id="sl-ventas" oninput="update()">
      <span class="slider-val" id="sv-ventas">0%</span>
    </div>
    <div class="slider-row">
      <i class="ti ti-package"></i>
      <span class="slider-label">Eficiencia cadena de suministro (↓ costo ventas)</span>
      <input type="range" min="-10" max="5" step="1" value="0" id="sl-costo" oninput="update()">
      <span class="slider-val" id="sv-costo">0%</span>
    </div>
    <div class="slider-row">
      <i class="ti ti-settings"></i>
      <span class="slider-label">Optimización gastos fijos (adm. y ventas)</span>
      <input type="range" min="-8" max="5" step="1" value="0" id="sl-gastos" oninput="update()">
      <span class="slider-val" id="sv-gastos">0%</span>
    </div>
  </div>

  <div class="metric-grid">
    <div class="metric"><p class="metric-label">Ingresos operacionales</p><p class="metric-val" id="m-ingresos">$21.200</p><p class="metric-sub" id="m-ingresos-sub">Base año 2025</p></div>
    <div class="metric"><p class="metric-label">Utilidad bruta</p><p class="metric-val" id="m-ub">$8.690</p><p class="metric-sub" id="m-ub-sub">Margen: 41,0%</p></div>
    <div class="metric"><p class="metric-label">EBIT (utilidad operativa)</p><p class="metric-val" id="m-ebit">$2.754</p><p class="metric-sub" id="m-ebit-sub">Margen: 13,0%</p></div>
    <div class="metric"><p class="metric-label">EBITDA</p><p class="metric-val" id="m-ebitda">$3.434</p><p class="metric-sub" id="m-ebitda-sub">Margen: 16,2%</p></div>
  </div>

  <div class="panel">
    <p class="section-title">Estado de resultados proyectado (miles de millones COP)</p>
    <table>
      <thead><tr><th>Cuenta</th><th>Base 2025</th><th>Proyectado</th><th>Variación</th></tr></thead>
      <tbody>
        <tr><td>Ingresos operacionales</td><td>$21.200</td><td id="t-ing">$21.200</td><td id="t-ing-v"><span class="badge bu">+0%</span></td></tr>
        <tr><td>(-) Costo de ventas</td><td>$12.510</td><td id="t-costo">$12.510</td><td id="t-costo-v"><span class="badge bu">+0%</span></td></tr>
        <tr class="hl"><td>Utilidad bruta</td><td>$8.690</td><td id="t-ub">$8.690</td><td id="t-ub-v"><span class="badge bu">+0%</span></td></tr>
        <tr><td>(-) Gastos de operación</td><td>$5.936</td><td id="t-gasto">$5.936</td><td id="t-gasto-v"><span class="badge bu">+0%</span></td></tr>
        <tr class="hl"><td>EBIT (utilidad operativa)</td><td>$2.754</td><td id="t-ebit">$2.754</td><td id="t-ebit-v"><span class="badge bu">+0%</span></td></tr>
        <tr><td>(+) Depreciaciones y amortizaciones</td><td>$680</td><td>$680</td><td>—</td></tr>
        <tr class="hl"><td>EBITDA</td><td>$3.434</td><td id="t-ebitda">$3.434</td><td id="t-ebitda-v"><span class="badge bu">+0%</span></td></tr>
      </tbody>
    </table>
  </div>

  <div id="alert-box" class="alert alert-yellow">
    <i class="ti ti-chart-bar"></i> Margen EBITDA: 16,2% — Desempeño estándar. Monitorear inflación de materias primas.
  </div>
</div>

<div class="footer">
  Datos académicos adaptados de Grupo Nutresa S.A. · <span>Politécnico Grancolombiano</span> · ECA52814 · Uso exclusivamente educativo
</div>

<script>
const BASE={ingresos:21200,costo:12510,gastos:5936,dep:680};
function fmt(n){return '$'+Math.round(n).toLocaleString('es-CO');}
function pct(n){return n.toFixed(1)+'%';}
function varBadge(v){const s=v>=0?'+':'';const c=v>=0?'bu':'bd';return`<span class="badge ${c}">${s}${v.toFixed(1)}%</span>`;}
function update(){
  const dV=parseInt(document.getElementById('sl-ventas').value);
  const dC=parseInt(document.getElementById('sl-costo').value);
  const dG=parseInt(document.getElementById('sl-gastos').value);
  document.getElementById('sv-ventas').textContent=(dV>=0?'+':'')+dV+'%';
  document.getElementById('sv-costo').textContent=(dC>=0?'+':'')+dC+'%';
  document.getElementById('sv-gastos').textContent=(dG>=0?'+':'')+dG+'%';
  const ing=BASE.ingresos*(1+dV/100);
  const costo=BASE.costo*(1+dC/100);
  const gastos=BASE.gastos*(1+dG/100);
  const ub=ing-costo;const ebit=ub-gastos;const ebitda=ebit+BASE.dep;
  const mUB=ub/ing*100;const mEBIT=ebit/ing*100;const mEBITDA=ebitda/ing*100;
  document.getElementById('m-ingresos').textContent=fmt(ing);
  document.getElementById('m-ingresos-sub').textContent=dV===0?'Base año 2025':(dV>0?'▲ ':'▼ ')+Math.abs(dV)+'% vs base';
  document.getElementById('m-ub').textContent=fmt(ub);document.getElementById('m-ub-sub').textContent='Margen: '+pct(mUB);
  document.getElementById('m-ebit').textContent=fmt(ebit);document.getElementById('m-ebit-sub').textContent='Margen: '+pct(mEBIT);
  document.getElementById('m-ebitda').textContent=fmt(ebitda);document.getElementById('m-ebitda-sub').textContent='Margen: '+pct(mEBITDA);
  document.getElementById('t-ing').textContent=fmt(ing);document.getElementById('t-ing-v').innerHTML=varBadge((ing/BASE.ingresos-1)*100);
  document.getElementById('t-costo').textContent=fmt(costo);document.getElementById('t-costo-v').innerHTML=varBadge((costo/BASE.costo-1)*100);
  document.getElementById('t-ub').textContent=fmt(ub);document.getElementById('t-ub-v').innerHTML=varBadge((ub/(BASE.ingresos-BASE.costo)-1)*100);
  document.getElementById('t-gasto').textContent=fmt(gastos);document.getElementById('t-gasto-v').innerHTML=varBadge((gastos/BASE.gastos-1)*100);
  document.getElementById('t-ebit').textContent=fmt(ebit);document.getElementById('t-ebit-v').innerHTML=varBadge((ebit/(BASE.ingresos-BASE.costo-BASE.gastos)-1)*100);
  document.getElementById('t-ebitda').textContent=fmt(ebitda);document.getElementById('t-ebitda-v').innerHTML=varBadge((ebitda/(BASE.ingresos-BASE.costo-BASE.gastos+BASE.dep)-1)*100);
  const ab=document.getElementById('alert-box');ab.className='alert';
  if(mEBITDA<14){ab.classList.add('alert-red');ab.innerHTML='<i class="ti ti-alert-circle"></i> Margen EBITDA: '+pct(mEBITDA)+' — Destrucción de valor operativo. Los costos absorben la capacidad de maniobra de Nutresa.';}
  else if(mEBITDA<=17){ab.classList.add('alert-yellow');ab.innerHTML='<i class="ti ti-chart-bar"></i> Margen EBITDA: '+pct(mEBITDA)+' — Desempeño estándar. Monitorear inflación de materias primas.';}
  else{ab.classList.add('alert-green');ab.innerHTML='<i class="ti ti-rocket"></i> Margen EBITDA: '+pct(mEBITDA)+' — Excelente gestión de valor. Nutresa libera caja masiva para expansión.';}
}
function resetAll(){['sl-ventas','sl-costo','sl-gastos'].forEach(id=>document.getElementById(id).value=0);update();}
</script>
</body>
</html>
