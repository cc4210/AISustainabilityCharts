<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI, Computing Efficiency &amp; US Electricity</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    background: #f8f7f4;
    color: #1a1a1a;
    padding: 24px;
    max-width: 960px;
    margin: 0 auto;
  }
  @media (prefers-color-scheme: dark) {
    body { background: #1a1918; color: #e8e6e0; }
    .card { background: #252420 !important; border-color: rgba(255,255,255,0.1) !important; }
    .metric-card { background: #2e2c28 !important; }
    .section-divider { border-color: rgba(255,255,255,0.1); }
  }
  h1 { font-size: 20px; font-weight: 500; margin-bottom: 6px; }
  h2 { font-size: 16px; font-weight: 500; margin-bottom: 6px; margin-top: 32px; }
  .subtitle { font-size: 13px; color: #666; margin-bottom: 20px; line-height: 1.5; }
  @media (prefers-color-scheme: dark) { .subtitle { color: #999; } }
  .card {
    background: #fff;
    border: 0.5px solid rgba(0,0,0,0.12);
    border-radius: 12px;
    padding: 20px 24px;
    margin-bottom: 20px;
  }
  .legend {
    display: flex; flex-wrap: wrap; gap: 14px;
    margin-bottom: 8px; font-size: 12px; color: #555;
  }
  @media (prefers-color-scheme: dark) { .legend { color: #aaa; } }
  .legend-item { display: flex; align-items: center; gap: 6px; }
  .legend-line { width: 18px; height: 3px; border-radius: 2px; flex-shrink: 0; }
  .legend-line.dashed { background: transparent; border-top: 2px dashed currentColor; height: 0; margin-top: 1px; }
  .chart-note { font-size: 11px; color: #888; margin-bottom: 14px; }
  .chart-wrapper { position: relative; width: 100%; }
  .section-label { font-size: 13px; font-weight: 500; color: #444; margin: 0 0 4px; }
  .section-sub { font-size: 11px; color: #888; margin-bottom: 10px; }
  @media (prefers-color-scheme: dark) {
    .section-label { color: #ccc; }
    .section-sub { color: #888; }
  }
  .metrics {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 10px; margin-bottom: 20px;
  }
  .metric-card { background: #f0ede6; border-radius: 8px; padding: 12px 14px; }
  .metric-label { font-size: 11px; color: #777; margin-bottom: 4px; line-height: 1.4; }
  .metric-value { font-size: 22px; font-weight: 500; line-height: 1.1; }
  .metric-sub { font-size: 11px; color: #888; margin-top: 2px; }
  @media (prefers-color-scheme: dark) {
    .metric-label { color: #999; }
    .metric-sub { color: #888; }
  }
  .source-note {
    font-size: 11px; color: #888; margin-top: 12px; line-height: 1.9;
    border-top: 0.5px solid rgba(0,0,0,0.08); padding-top: 10px;
  }
  @media (prefers-color-scheme: dark) {
    .source-note { border-color: rgba(255,255,255,0.08); color: #777; }
  }
  .source-note a { color: #1d9e75; text-decoration: none; }
  .source-note a:hover { text-decoration: underline; }
  @media (prefers-color-scheme: dark) { .source-note a { color: #4ecda4; } }
  .src-label { font-weight: 500; color: #555; }
  @media (prefers-color-scheme: dark) { .src-label { color: #aaa; } }
  .section-divider {
    border: none;
    border-top: 1px solid rgba(0,0,0,0.1);
    margin: 36px 0 28px;
  }
</style>
</head>
<body>

<!-- ═══════════════════════════════════════════════════
     SECTION 1: MOORE'S LAW / KOOMEY'S LAW / DATA CENTER ENERGY
     ═══════════════════════════════════════════════════ -->

<h1>Comparing Computing Efficiency &amp; Data Center Energy Growth</h1>
<p class="subtitle">Moore's Law (transistors/chip) and Koomey's Law (computations/kWh) have each improved by ~10 billion times since 1971 — yet global data center energy consumption has also grown, not shrunk. This is the empirical signature of the <a href="https://www.npr.org/sections/planet-money/2025/02/04/g-s1-46018/ai-deepseek-economics-jevons-paradox">Jevons Paradox in computing</a>.</p>

<div class="card">
  <div class="legend">
    <span class="legend-item"><span class="legend-line" style="background:#3266ad;"></span>Transistors/chip (Moore's Law)</span>
    <span class="legend-item"><span class="legend-line" style="background:#1d9e75;"></span>Computations/kWh (Koomey's Law)</span>
    <span class="legend-item"><span class="legend-line" style="background:#d85a30;"></span>Global data center energy (TWh) — historical</span>
    <span class="legend-item"><span class="legend-line dashed" style="color:#d85a30; width:18px;"></span>projected (IEA base case)</span>
  </div>
  <p class="chart-note">Left axis (log scale): transistors/chip and computations/kWh. Right axis (linear): global data center energy TWh/yr. Dashed = IEA projections to 2030.</p>
  <div class="chart-wrapper" style="height:340px;">
    <canvas id="mooresChart" role="img"
      aria-label="Log-scale chart from 1971 to 2030. Transistor count and compute efficiency per kWh have grown exponentially by roughly 10 billion times. Global data center energy grew from under 10 TWh in 1990 to 415 TWh in 2024, projected to 945 TWh by 2030. Efficiency is growing but total energy consumption is also growing — the Jevons Paradox.">
    </canvas>
  </div>

  <div class="source-note">
    <span class="src-label">Transistor counts (Moore's Law):</span> Public chip specifications — Intel 4004 (1971) through modern GPUs (2024). See
    <a href="https://ourworldindata.org/moores-law" target="_blank" rel="noopener">Our World in Data — Moore's Law</a> for compiled dataset.
    <br>
    <span class="src-label">Compute efficiency (Koomey's Law):</span>
    <a href="https://ieeexplore.ieee.org/document/5440129/" target="_blank" rel="noopener">Koomey et al. (2011), <em>IEEE Annals of the History of Computing</em>, 33(3), 46–54</a>
    and subsequent updates.
    <br>
    <span class="src-label">Global data center energy — historical:</span>
    <a href="https://www.science.org/doi/10.1126/science.aba3758" target="_blank" rel="noopener">Masanet et al. (2020), <em>Science</em>, 367, 984–986</a> ·
    <a href="https://eta-publications.lbl.gov/publications/2024-lbnl-data-center-energy-usage-report" target="_blank" rel="noopener">LBNL — 2024 US Data Center Energy Usage Report</a>
    <br>
    <span class="src-label">Global data center energy — projected:</span>
    <a href="https://www.iea.org/reports/energy-and-ai" target="_blank" rel="noopener">IEA — Energy and AI (2025)</a>
  </div>
</div>

<hr class="section-divider">

<!-- ═══════════════════════════════════════════════════
     SECTION 2: US ELECTRICITY DEMAND CHARTS
     ═══════════════════════════════════════════════════ -->

<h2>US Electricity: Data Centers vs Demand &amp; Renewables</h2>
<p class="subtitle">Year-on-year % growth rates and sectoral demand drivers, 2010–2030 (projected).</p>

<div class="metrics">
  <div class="metric-card">
    <div class="metric-label">Data centers share of new US electricity demand</div>
    <div class="metric-value">~50%</div>
    <div class="metric-sub">projected 2024–2030</div>
  </div>
  <div class="metric-card">
    <div class="metric-label">US data center share of US electricity</div>
    <div class="metric-value">4.4% → 12%</div>
    <div class="metric-sub">2023 → 2028 (DOE/LBNL est.)</div>
  </div>
  <div class="metric-card">
    <div class="metric-label">US electricity demand — flat for</div>
    <div class="metric-value">~15 yrs</div>
    <div class="metric-sub">2007–2022 (EIA)</div>
  </div>
  <div class="metric-card">
    <div class="metric-label">2024 demand spike driven by heatwaves</div>
    <div class="metric-value">~25 TWh</div>
    <div class="metric-sub">of 128 TWh rise (Ember)</div>
  </div>
</div>

<div class="card">
  <div class="legend">
    <span class="legend-item"><span class="legend-line" style="background:#888780;"></span>US electricity demand</span>
    <span class="legend-item"><span class="legend-line" style="background:#1d9e75;"></span>US renewable generation</span>
    <span class="legend-item"><span class="legend-line" style="background:#d85a30;"></span>US data center energy</span>
    <span class="legend-item"><span class="legend-line dashed" style="color:#aaa; width:18px;"></span>projected</span>
    <span class="legend-item"><span class="legend-line dashed" style="color:#d85a30; width:18px; opacity:0.55;"></span>data center high scenario</span>
  </div>
  <p class="chart-note">Annualised % growth rates. Multi-year intervals are CAGRs. Shaded band = data center base-to-high scenario range. † = COVID distortion (2020).</p>
  <div class="chart-wrapper" style="height:300px;">
    <canvas id="pctChart" role="img" aria-label="US electricity demand was flat 2010-2020, now rising 2-3% per year. Renewables growing 8-12% per year. Data centers 10-20% per year historically, projected 12-15% to 2030."></canvas>
  </div>
</div>

<div class="card">
  <p class="section-label">What's actually driving US electricity demand changes?</p>
  <p class="section-sub">Approximate annual TWh shift by demand driver. Bars above zero = growth; below zero = decline.</p>
  <div class="chart-wrapper" style="height:280px;">
    <canvas id="sectorChart" role="img" aria-label="Stacked bar chart showing residential and industrial demand near flat or declining due to efficiency, while data centers are the fastest-growing demand driver projected to dominate new load post-2024."></canvas>
  </div>

  <div class="source-note">
    <span class="src-label">US electricity demand &amp; renewables:</span>
    <a href="https://www.eia.gov/outlooks/steo/" target="_blank" rel="noopener">EIA Short-Term Energy Outlook (Apr 2026)</a> ·
    <a href="https://www.eia.gov/outlooks/aeo/" target="_blank" rel="noopener">EIA Annual Energy Outlook 2026</a> ·
    <a href="https://www.eia.gov/electricity/annual/" target="_blank" rel="noopener">EIA Electric Power Annual 2024</a> ·
    <a href="https://www.eia.gov/totalenergy/data/monthly/" target="_blank" rel="noopener">EIA Monthly Energy Review</a>
    <br>
    <span class="src-label">Data center energy (US):</span>
    <a href="https://eta-publications.lbl.gov/publications/2024-lbnl-data-center-energy-usage-report" target="_blank" rel="noopener">LBNL — 2024 United States Data Center Energy Usage Report</a> ·
    <a href="https://www.iea.org/reports/energy-and-ai" target="_blank" rel="noopener">IEA — Energy and AI (2025)</a>
    <br>
    <span class="src-label">Sectoral breakdown &amp; 2024 weather analysis:</span>
    <a href="https://ember-energy.org/latest-insights/us-electricity-2025-special-report/2024-in-review/" target="_blank" rel="noopener">Ember — US Electricity 2025 Special Report</a>
    (25 TWh of 128 TWh 2024 rise attributable to heatwave temperatures vs. 2023)
    <br>
    <span class="src-label">Notes:</span> Projections use IEA base case; high scenario from IEA Lift-Off case. Growth rates for multi-year intervals are annualised CAGRs. Sectoral TWh contributions are approximate.
  </div>
</div>

<!-- ═══════════════════════════════════════════════════
     SCRIPTS
     ═══════════════════════════════════════════════════ -->
<script>
const isDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
const gridCol = isDark ? 'rgba(255,255,255,0.08)' : 'rgba(0,0,0,0.07)';
const tickCol = isDark ? '#aaa' : '#555';

// ── CHART 1: MOORE'S / KOOMEY'S LAW ──────────────────────────────────
const mooreYears = [1971,1974,1978,1982,1985,1989,1993,1997,2000,2003,2006,2009,2012,2015,2018,2020,2022,2024,2026,2028,2030];
const transistors = [2300,6000,29000,134000,275000,1e6,3.1e6,7.5e6,42e6,125e6,291e6,904e6,2.27e9,4.31e9,8.5e9,15e9,50e9,80e9,null,null,null];
const koomey      = [1e5,3e5,2e6,1.2e7,5e7,2e8,1.2e9,7e9,5e10,3e11,2e12,1.2e13,8e13,5e14,3e15,1e16,3e16,6e16,null,null,null];
const dcGlobal    = [null,null,null,null,null,null,null,null,7,14,30,60,130,180,205,250,340,415,560,750,945];
const dcGlobalS   = dcGlobal.map((v,i) => i <= 17 ? v : null);
const dcGlobalD   = dcGlobal.map((v,i) => i >= 17 ? v : null);

new Chart(document.getElementById('mooresChart'), {
  type: 'line',
  data: { labels: mooreYears, datasets: [
    { label:'Transistors/chip', data:transistors, yAxisID:'yLeft',
      borderColor:'#3266ad', backgroundColor:'transparent',
      pointRadius:3, pointBackgroundColor:'#3266ad', borderWidth:2, tension:0.3, spanGaps:false },
    { label:'Computations/kWh', data:koomey, yAxisID:'yLeft',
      borderColor:'#1d9e75', backgroundColor:'transparent',
      pointRadius:3, pointBackgroundColor:'#1d9e75', borderWidth:2, tension:0.3, spanGaps:false },
    { label:'Data center energy — historical', data:dcGlobalS, yAxisID:'yRight',
      borderColor:'#d85a30', backgroundColor:'rgba(216,90,48,0.07)', fill:true,
      pointRadius:3, pointBackgroundColor:'#d85a30', borderWidth:2.5, tension:0.3, spanGaps:false },
    { label:'Data center energy — projected', data:dcGlobalD, yAxisID:'yRight',
      borderColor:'#d85a30', backgroundColor:'rgba(216,90,48,0.04)', fill:true,
      pointRadius:3, pointBackgroundColor:'#d85a30',
      borderDash:[6,4], borderWidth:2.5, tension:0.3, spanGaps:false },
  ]},
  options: {
    responsive:true, maintainAspectRatio:false,
    interaction:{mode:'index',intersect:false},
    plugins:{
      legend:{display:false},
      tooltip:{callbacks:{
        label: ctx => {
          if(ctx.raw==null) return null;
          const v = ctx.raw;
          const n = ctx.dataset.label.replace(' — historical','').replace(' — projected','');
          if(ctx.datasetIndex <= 1) {
            if(v>=1e15) return n+': '+(v/1e15).toFixed(1)+'P';
            if(v>=1e12) return n+': '+(v/1e12).toFixed(1)+'T';
            if(v>=1e9)  return n+': '+(v/1e9).toFixed(1)+'B';
            if(v>=1e6)  return n+': '+(v/1e6).toFixed(1)+'M';
            if(v>=1e3)  return n+': '+(v/1e3).toFixed(0)+'K';
            return n+': '+v;
          }
          return 'Data center energy: '+v+' TWh';
        }
      }}
    },
    scales:{
      x:{
        ticks:{color:tickCol, font:{size:11}, maxRotation:0,
          callback:(v,i)=>[1971,1980,1990,2000,2010,2020,2030].includes(mooreYears[i])?mooreYears[i]:''},
        grid:{color:gridCol}
      },
      yLeft:{
        type:'logarithmic', position:'left',
        title:{display:true, text:'Log scale (transistors/chip  or  computations/kWh)', color:tickCol, font:{size:11}},
        ticks:{color:tickCol, font:{size:10}, callback:v=>{
          const log=Math.log10(v);
          if(Number.isInteger(Math.round(log))){
            if(v>=1e15) return (v/1e15).toFixed(0)+'P';
            if(v>=1e12) return (v/1e12).toFixed(0)+'T';
            if(v>=1e9)  return (v/1e9).toFixed(0)+'B';
            if(v>=1e6)  return (v/1e6).toFixed(0)+'M';
            if(v>=1e3)  return (v/1e3).toFixed(0)+'K';
            return v;
          }
          return '';
        }},
        grid:{color:gridCol}
      },
      yRight:{
        type:'linear', position:'right',
        title:{display:true, text:'Global data center energy (TWh/yr)', color:'#d85a30', font:{size:11}},
        min:0, max:1050,
        ticks:{color:'#d85a30', font:{size:10}, callback:v=>v+' TWh'},
        grid:{drawOnChartArea:false}
      }
    }
  }
});

// ── CHART 2: US GROWTH RATES ──────────────────────────────────────────
const years   = [2010,2012,2014,2016,2018,2020,2022,2023,2024,2025,2026,2028,2030];
const usElec  = [4120,4050,4090,4080,4230,3800,4270,4178,4310,4430,4520,4700,4900];
const usRenew = [420,530,600,700,840,970,1200,1350,1500,1650,1780,2080,2430];
const usDc    = [60,80,100,130,155,160,175,180,180,240,290,350,420];
const usDcHi  = [60,80,100,130,155,160,175,180,180,260,340,480,650];

function cagr(arr) {
  return arr.map((v,i)=>{
    if(i===0) return null;
    const prev=arr[i-1], yrs=years[i]-years[i-1];
    return Math.round((Math.pow(v/prev,1/yrs)-1)*1000)/10;
  });
}
const elecPct=cagr(usElec), renewPct=cagr(usRenew), dcPct=cagr(usDc), dcHiPct=cagr(usDcHi);
const H=8;
const sp=arr=>arr.map((v,i)=>i<=H?v:null);
const dp=arr=>arr.map((v,i)=>i>=H?v:null);

const covidPlugin={
  id:'covidNote',
  afterDraw(chart){
    const ctx=chart.ctx,xS=chart.scales.x,yS=chart.scales.y;
    const i2020=years.indexOf(2020); if(i2020<0)return;
    const x=xS.getPixelForValue(i2020);
    const yv=elecPct[i2020]; if(yv==null)return;
    const y=yS.getPixelForValue(yv)-16;
    ctx.save();
    ctx.font='10px sans-serif';
    ctx.fillStyle=isDark?'rgba(200,200,200,0.6)':'rgba(80,80,80,0.6)';
    ctx.textAlign='center';
    ctx.fillText('† COVID',x,y);
    ctx.restore();
  }
};

new Chart(document.getElementById('pctChart'),{
  type:'line', plugins:[covidPlugin],
  data:{labels:years, datasets:[
    {label:'US electricity — historical',   data:sp(elecPct),  borderColor:'#888780',backgroundColor:'transparent',pointRadius:4,pointBackgroundColor:'#888780',borderWidth:2.5,tension:0.35,spanGaps:false},
    {label:'US electricity — projected',    data:dp(elecPct),  borderColor:'#888780',backgroundColor:'transparent',pointRadius:3,pointBackgroundColor:'#888780',borderDash:[6,4],borderWidth:2,tension:0.35,spanGaps:false},
    {label:'Renewables — historical',       data:sp(renewPct), borderColor:'#1d9e75',backgroundColor:'transparent',pointRadius:4,pointBackgroundColor:'#1d9e75',borderWidth:2.5,tension:0.35,spanGaps:false},
    {label:'Renewables — projected',        data:dp(renewPct), borderColor:'#1d9e75',backgroundColor:'transparent',pointRadius:3,pointBackgroundColor:'#1d9e75',borderDash:[6,4],borderWidth:2,tension:0.35,spanGaps:false},
    {label:'Data centers — historical',     data:sp(dcPct),    borderColor:'#d85a30',backgroundColor:'transparent',pointRadius:4,pointBackgroundColor:'#d85a30',borderWidth:2.5,tension:0.35,spanGaps:false},
    {label:'Data centers — base projected', data:dp(dcPct),    borderColor:'#d85a30',backgroundColor:'transparent',pointRadius:3,pointBackgroundColor:'#d85a30',borderDash:[6,4],borderWidth:2,tension:0.35,spanGaps:false},
    {label:'Data centers — high scenario',  data:dp(dcHiPct),  borderColor:'#d85a30',backgroundColor:'rgba(216,90,48,0.07)',fill:'-1',pointRadius:2,pointBackgroundColor:'#d85a30',borderDash:[3,3],borderWidth:1.5,tension:0.35,spanGaps:false},
  ]},
  options:{
    responsive:true, maintainAspectRatio:false,
    interaction:{mode:'index',intersect:false},
    plugins:{
      legend:{display:false},
      tooltip:{callbacks:{
        label:ctx=>{
          if(ctx.raw==null)return null;
          const n=ctx.dataset.label.replace(/ — (historical|projected|base projected|high scenario).*/i,'');
          const s=ctx.dataset.label.includes('high')?' (high)':'';
          return n+s+': '+ctx.raw.toFixed(1)+'%/yr';
        },
        footer:items=>{const yr=years[items[0].dataIndex];return yr===2020?['† Rate depressed by COVID demand shock']:[];}
      }}
    },
    scales:{
      x:{ticks:{color:tickCol,font:{size:11},maxRotation:0},grid:{color:gridCol},
         title:{display:true,text:'← historical   |   projected →',color:tickCol,font:{size:10},padding:{top:4}}},
      y:{title:{display:true,text:'% growth rate (annualised)',color:tickCol,font:{size:11}},
         ticks:{color:tickCol,font:{size:10},callback:v=>v+'%'},grid:{color:gridCol}}
    }
  }
});

// ── CHART 3: SECTORAL CONTRIBUTIONS ──────────────────────────────────
const sYears=[2012,2014,2016,2018,2020,2022,2023,2024,2026,2028,2030];
const residential=[-20,30,-10,80,-200,180,-45,80,40,50,60];
const industrial =[-30,-20,-30,20,-100,70,-30,30,30,40,40];
const commExDC   =[10,20,10,30,-80,100,20,40,40,50,60];
const efficiency =[-40,-45,-45,-40,0,-30,-20,-30,-40,-40,-40];
const datacenter =[10,10,15,13,3,8,3,25,55,30,35];

new Chart(document.getElementById('sectorChart'),{
  type:'bar',
  data:{labels:sYears, datasets:[
    {label:'Efficiency savings',             data:efficiency,  backgroundColor:isDark?'rgba(59,109,17,0.65)' :'rgba(59,109,17,0.55)',  stack:'s',borderRadius:2},
    {label:'Industrial',                     data:industrial,  backgroundColor:isDark?'rgba(95,94,90,0.70)'  :'rgba(95,94,90,0.65)',   stack:'s',borderRadius:2},
    {label:'Residential',                    data:residential, backgroundColor:isDark?'rgba(136,135,128,0.70)':'rgba(136,135,128,0.65)',stack:'s',borderRadius:2},
    {label:'Commercial (excl. data centers)',data:commExDC,    backgroundColor:isDark?'rgba(29,158,117,0.50)':'rgba(29,158,117,0.45)',stack:'s',borderRadius:2},
    {label:'Data centers',                   data:datacenter,  backgroundColor:isDark?'rgba(216,90,48,0.85)' :'rgba(216,90,48,0.80)', stack:'s',borderRadius:2},
  ]},
  options:{
    responsive:true, maintainAspectRatio:false,
    interaction:{mode:'index',intersect:false},
    plugins:{
      legend:{display:true,position:'bottom',labels:{color:tickCol,font:{size:11},boxWidth:12,padding:14}},
      tooltip:{callbacks:{label:ctx=>{if(ctx.raw==null)return null;const s=ctx.raw>=0?'+':'';return ctx.dataset.label+': '+s+Math.round(ctx.raw)+' TWh/yr';}}}
    },
    scales:{
      x:{stacked:true,ticks:{color:tickCol,font:{size:11},maxRotation:0},grid:{color:gridCol},
         title:{display:true,text:'← historical   |   projected →',color:tickCol,font:{size:10},padding:{top:4}}},
      y:{stacked:true,title:{display:true,text:'Approx. annual TWh change',color:tickCol,font:{size:11}},
         ticks:{color:tickCol,font:{size:10},callback:v=>(v>0?'+':'')+v+' TWh'},grid:{color:gridCol}}
    }
  }
});
</script>
</body>
</html>
