<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nutresa CEO Challenge — Contabilidad Financiera · Politécnico Grancolombiano</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.44.0/tabler-icons.min.css">
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{--poli-red:#C41230;--poli-navy:#1C2B4A;--poli-red-light:#f5e6e9}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;background:#f4f4f0;color:#1a1a18;min-height:100vh}

/* HEADER INSTITUCIONAL */
.poli-header{background:var(--poli-navy);padding:0;margin-bottom:0}
.poli-topbar{background:var(--poli-red);padding:6px 1.5rem;display:flex;align-items:center;gap:8px}
.poli-topbar span{color:#fff;font-size:11px;font-weight:500;letter-spacing:.03em}
.poli-main-header{padding:1.2rem 1.5rem 1rem;display:flex;align-items:center;gap:1.2rem}
.poli-logo-box{display:flex;align-items:center;gap:10px;flex-shrink:0}
.poli-logo-icon{width:52px;height:52px;background:#fff;border-radius:6px;display:flex;align-items:center;justify-content:center;padding:6px}
.poli-logo-icon svg{width:100%;height:100%}
.poli-logo-text{display:flex;flex-direction:column}
.poli-logo-text .inst{font-size:9px;color:rgba(255,255,255,.65);letter-spacing:.08em;text-transform:uppercase;font-weight:500}
.poli-logo-text .name{font-size:17px;font-weight:500;color:#fff;line-height:1.2}
.poli-logo-text .name span{color:#ef8c9b}
.poli-divider{width:1px;height:48px;background:rgba(255,255,255,.2);flex-shrink:0}
.poli-course-info{display:flex;flex-direction:column;gap:3px}
.poli-course-info .modulo{font-size:11px;color:rgba(255,255,255,.6);text-transform:uppercase;letter-spacing:.06em}
.poli-course-info .titulo{font-size:16px;font-weight:500;color:#fff}
.poli-course-info .codigo{font-size:12px;color:rgba(255,255,255,.55)}
.poli-professor{margin-left:auto;text-align:right;flex-shrink:0}
.poli-professor .label{font-size:10px;color:rgba(255,255,255,.5);text-transform:uppercase;letter-spacing:.05em}
.poli-professor .prof-name{font-size:13px;font-weight:500;color:#fff}
.poli-professor .role{font-size:11px;color:rgba(255,255,255,.55)}

/* CONTENIDO */
.content{padding:1.2rem 1.5rem}
.tip{background:#e6f1fb;border:0.5px solid #85b7eb;border-radius:8px;padding:.6rem 1rem;font-size:12px;color:#185fa5;margin-bottom:12px}
.panel{background:#fff;border:0.5px solid #d3d1c7;border-radius:12px;padding:1rem 1.25rem;margin-bottom:12px}
.section-title{font-size:14px;font-weight:500;margin-bottom:10px;color:#1a1a18}
.metric-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:10px;margin-bottom:12px}
.metric{background:#f4f4f0;border-radius:8px;padding:.75rem 1rem}
.metric-label{font-size:12px;color:#5f5e5a;margin-bottom:4px}
.metric-val{font-size:22px;font-weight:500;color:#1a1a18}
.metric-sub{font-size:11px;color:#888780;margin-top:2px}
.slider-row{display:flex;align-items:center;gap:10px;margin-bottom:.9rem}
.slider-row i{font-size:18px;color:#888780;flex-shrink:0}
.slider-label{font-size:13px;color:#5f5e5a;min-width:200px}
.slider-val{font-size:13px;font-weight:500;min-width:48px;text-align:right;color:#1a1a18}
input[type=range]{flex:1;accent-color:#C41230;height:4px;cursor:pointer}
table{width:100%;font-size:13px;border-collapse:collapse}
th{font-size:11px;font-weight:500;color:#888780;text-align:right;padding:5px 8px;border-bottom:0.5px solid #d3d1c7}
th:first-child{text-align:left}
td{padding:5px 8px;text-align:right;color:#1a1a18}
td:first-child{text-align:left;color:#5f5e5a}
tr.hl td{font-weight:500;color:#1a1a18;border-top:0.5px solid #d3d1c7}
.badge{display:inline-block;font-size:11px;padding:2px 8px;border-radius:6px}
.bu{background:#eaf3de;color:#3b6d11}
.bd{background:#fcebeb;color:#a32d2d}
.alert{border-radius:8px;padding:.7rem 1rem;font-size:14px;font-weight:500;text-align:center;margin-top:8px}
.alert-red{background:#fcebeb;color:#a32d2d;border:0.5px solid #f09595}
.alert-yellow{background:#faeeda;color:#854f0b;border:0.5px solid #ef9f27}
.alert-green{background:#eaf3de;color:#3b6d11;border:0.5px solid #97c459}
.reset-btn{background:transparent;border:0.5px solid #b4b2a9;border-radius:8px;padding:6px 14px;font-size:12px;color:#5f5e5a;cursor:pointer}
.reset-btn:hover{background:#f4f4f0}
.footer{background:var(--poli-navy);color:rgba(255,255,255,.5);font-size:11px;text-align:center;padding:.8rem 1.5rem;margin-top:1rem}
.footer span{color:var(--poli-red);font-weight:500}
@media(max-width:600px){.poli-professor{display:none}.slider-label{min-width:120px;font-size:12px}.poli-logo-text .name{font-size:14px}}
</style>
</head>
<body>

<!-- HEADER INSTITUCIONAL -->
<div class="poli-header">
  <div class="poli-topbar">
    <span>Institución Universitaria</span>
    <span style="color:rgba(255,255,255,.4)">·</span>
    <span>Escuela de Negocios · Especialización en Gerencia Financiera</span>
  </div>
  <div class="poli-main-header">
    <div class="poli-logo-box">
      <!-- Logo SVG del Politécnico Grancolombiano -->
      <div class="poli-logo-icon">
        <svg viewBox="0 0 80 80" xmlns="http://www.w3.org/2000/svg">
          <!-- Escudo simplificado estilo Poli -->
          <rect x="8" y="4" width="64" height="72" rx="6" fill="#1C2B4A"/>
          <rect x="8" y="4" width="64" height="22" rx="0" fill="#C41230"/>
          <rect x="8" y="4" width="64" height="6" rx="3" fill="#C41230"/>
          <!-- Franja roja superior -->
          <rect x="8" y="4" width="64" height="20" rx="4" fill="#C41230"/>
          <rect x="8" y="20" width="64" height="4" fill="#C41230"/>
          <!-- P estilizada -->
          <text x="40" y="52" text-anchor="middle" font-family="Georgia,serif" font-size="32" font-weight="bold" fill="#ffffff">P</text>
          <!-- Líneas decorativas -->
          <rect x="18" y="62" width="44" height="2" rx="1" fill="rgba(255,255,255,.3)"/>
          <rect x="24" y="67" width="32" height="2" rx="1" fill="rgba(255,255,255,.15)"/>
        </svg>
      </div>
      <div class="poli-logo-text">
        <span class="inst">Institución Universitaria</span>
        <span class="name">Politécnico<br><span>Grancolombiano</span></span>
      </div>
    </div>

    <div class="poli-divider"></div>

    <div class="poli-course-info">
      <span class="modulo">Módulo</span>
      <span class="titulo">Contabilidad Financiera</span>
      <span class="codigo">Código: ECA52814 · Especialización en Gerencia Financiera</span>
    </div>

    <div class="poli-professor">
      <p class="label">Docente</p>
      <p class="prof-name">Pio Quinto</p>
      <p class="role">Director de Formación</p>
    </div>
  </div>
</div>

<!-- CONTENIDO PRINCIPAL -->
<div class="content">

<div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:10px">
  <div>
    <p style="font-size:18px;font-weight:500;color:#1a1a18;margin:0">Nutresa CEO Challenge</p>
    <p style="font-size:12px;color:#5f5e5a;margin:2px 0 0">Tablero de decisiones operativas · Sesión 1</p>
  </div>
  <button class="reset-btn" onclick="resetAll()"><i class="ti ti-refresh"></i> Resetear</button>
</div>

<div class="tip">
  <i class="ti ti-bulb"></i> <strong>Misión:</strong> Llevar el Margen EBITDA al 18% usando las 3 palancas. ¿Cuál es tu combinación ganadora y por qué?
</div>

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
  <div class="metric">
    <p class="metric-label">Ingresos operacionales</p>
    <p class="metric-val" id="m-ingresos">$21.200</p>
    <p class="metric-sub" id="m-ingresos-sub">Base año 2025</p>
  </div>
  <div class="metric">
    <p class="metric-label">Utilidad bruta</p>
    <p class="metric-val" id="m-ub">$8.690</p>
    <p class="metric-sub" id="m-ub-sub">Margen: 41,0%</p>
  </div>
  <div class="metric">
    <p class="metric-label">EBIT (utilidad operativa)</p>
    <p class="metric-val" id="m-ebit">$2.754</p>
    <p class="metric-sub" id="m-ebit-sub">Margen: 13,0%</p>
  </div>
  <div class="metric">
    <p class="metric-label">EBITDA</p>
    <p class="metric-val" id="m-ebitda">$3.434</p>
    <p class="metric-sub" id="m-ebitda-sub">Margen: 16,2%</p>
  </div>
</div>

<div class="panel">
  <p class="section-title">Estado de resultados proyectado (miles de millones COP)</p>
  <table>
    <thead>
      <tr><th>Cuenta</th><th>Base 2025</th><th>Proyectado</th><th>Variación</th></tr>
    </thead>
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

</div><!-- /content -->

<div class="footer">
  Datos académicos adaptados de Grupo Nutresa S.A. · <span>Politécnico Grancolombiano</span> · Módulo ECA52814 · Uso exclusivamente educativo
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
  document.getElementById('m-ub').textContent=fmt(ub);
  document.getElementById('m-ub-sub').textContent='Margen: '+pct(mUB);
  document.getElementById('m-ebit').textContent=fmt(ebit);
  document.getElementById('m-ebit-sub').textContent='Margen: '+pct(mEBIT);
  document.getElementById('m-ebitda').textContent=fmt(ebitda);
  document.getElementById('m-ebitda-sub').textContent='Margen: '+pct(mEBITDA);
  document.getElementById('t-ing').textContent=fmt(ing);
  document.getElementById('t-ing-v').innerHTML=varBadge((ing/BASE.ingresos-1)*100);
  document.getElementById('t-costo').textContent=fmt(costo);
  document.getElementById('t-costo-v').innerHTML=varBadge((costo/BASE.costo-1)*100);
  document.getElementById('t-ub').textContent=fmt(ub);
  document.getElementById('t-ub-v').innerHTML=varBadge((ub/(BASE.ingresos-BASE.costo)-1)*100);
  document.getElementById('t-gasto').textContent=fmt(gastos);
  document.getElementById('t-gasto-v').innerHTML=varBadge((gastos/BASE.gastos-1)*100);
  document.getElementById('t-ebit').textContent=fmt(ebit);
  document.getElementById('t-ebit-v').innerHTML=varBadge((ebit/(BASE.ingresos-BASE.costo-BASE.gastos)-1)*100);
  document.getElementById('t-ebitda').textContent=fmt(ebitda);
  document.getElementById('t-ebitda-v').innerHTML=varBadge((ebitda/(BASE.ingresos-BASE.costo-BASE.gastos+BASE.dep)-1)*100);
  const ab=document.getElementById('alert-box');
  ab.className='alert';
  if(mEBITDA<14){ab.classList.add('alert-red');ab.innerHTML='<i class="ti ti-alert-circle"></i> Margen EBITDA: '+pct(mEBITDA)+' — Destrucción de valor operativo. Los costos absorben la capacidad de maniobra de Nutresa.';}
  else if(mEBITDA<=17){ab.classList.add('alert-yellow');ab.innerHTML='<i class="ti ti-chart-bar"></i> Margen EBITDA: '+pct(mEBITDA)+' — Desempeño estándar. Monitorear inflación de materias primas.';}
  else{ab.classList.add('alert-green');ab.innerHTML='<i class="ti ti-rocket"></i> Margen EBITDA: '+pct(mEBITDA)+' — Excelente gestión de valor. Nutresa libera caja masiva para expansión.';}
}
function resetAll(){['sl-ventas','sl-costo','sl-gastos'].forEach(id=>document.getElementById(id).value=0);update();}
</script>
</body>
</html>
