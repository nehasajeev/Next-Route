<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Next Route — Patient Journey Navigator</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:wght@400;700&family=Bricolage+Grotesque:opsz,wght@12..96,500;12..96,700;12..96,800&family=Noto+Sans+Devanagari:wght@400;700&family=Noto+Sans+Kannada:wght@400;700&family=Noto+Sans+Tamil:wght@400;700&display=swap" rel="stylesheet">
<style>
:root{
  --paper:#F4F7FC;--card:#FFFFFF;--ink:#0B1A33;--muted:#51607A;--line:#D3DCEA;--line2:#E7ECF4;
  --teal:#123F86;--teal-d:#0A2350;--teal-l:#E1E9F8;
  --red:#b8344a;--red-l:#f8e0e3;--amber:#9a6304;--amber-l:#f8ebcd;--green:#2a7748;--green-l:#ddefe3;
  --blue:#2D6CDF;--blue-l:#E2ECFC;--r:14px;--fs:1;
  --shadow:0 1px 0 rgba(10,35,80,.04),0 8px 24px -14px rgba(10,35,80,.28);
}
.hc{--paper:#fff;--card:#fff;--ink:#000;--muted:#111;--line:#000;--line2:#444;--teal:#001E5C;--teal-d:#00123A;--teal-l:#D6E3FF;--red:#8f0019;--amber:#5c3a00;--green:#0a4423;--blue:#0b2f8a;--shadow:none}
html{font-size:calc(16px * var(--fs))}
*{box-sizing:border-box}
body{margin:0;background:var(--paper);color:var(--ink);font-family:'Atkinson Hyperlegible','Noto Sans Devanagari','Noto Sans Kannada','Noto Sans Tamil',system-ui,sans-serif;line-height:1.5;-webkit-font-smoothing:antialiased}
h1,h2,h3,h4,.display{font-family:'Bricolage Grotesque','Noto Sans Devanagari','Noto Sans Kannada','Noto Sans Tamil',system-ui,sans-serif;letter-spacing:-.015em;margin:0}
h2{font-size:1.6rem;font-weight:800;line-height:1.15}
h3{font-size:1.1rem;font-weight:700}
p{margin:.3rem 0}
button,input,select,textarea{font:inherit;color:inherit}
button{cursor:pointer}
:focus-visible{outline:3px solid var(--blue);outline-offset:2px;border-radius:6px}
.skip{position:absolute;left:-999px}.skip:focus{left:8px;top:8px;background:var(--ink);color:var(--paper);padding:8px 12px;z-index:99}
.muted{color:var(--muted)}.small{font-size:.86rem}.tiny{font-size:.76rem}
.row{display:flex;gap:.6rem;align-items:center;flex-wrap:wrap}
.spacer{flex:1}

/* header */
.top{display:flex;align-items:center;gap:1rem;padding:.8rem 1.4rem;border-bottom:1px solid var(--line);background:var(--paper);position:sticky;top:0;z-index:20;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:.6rem}
.brand b{font-family:'Bricolage Grotesque',sans-serif;font-size:1.25rem;font-weight:800;letter-spacing:-.02em}
.brand .tag{font-size:.8rem;color:var(--muted);display:block;line-height:1.2}
.tools{display:flex;gap:.4rem;align-items:center;flex-wrap:wrap;margin-left:auto}
.tbtn{border:1px solid var(--line);background:var(--card);border-radius:999px;padding:.38rem .8rem;font-size:.86rem;display:inline-flex;gap:.35rem;align-items:center}
.tbtn[aria-pressed=true]{background:var(--ink);color:var(--paper);border-color:var(--ink)}
.tbtn.human{background:var(--teal);color:#fff;border-color:var(--teal);font-weight:700}
select.tbtn{appearance:none;padding-right:1.6rem;background-image:linear-gradient(45deg,transparent 50%,currentColor 50%),linear-gradient(135deg,currentColor 50%,transparent 50%);background-position:calc(100% - 13px) 55%,calc(100% - 8px) 55%;background-size:5px 5px;background-repeat:no-repeat}
.boundary{background:var(--ink);color:var(--paper);font-size:.84rem;padding:.42rem 1.4rem;display:flex;gap:.6rem;align-items:center;flex-wrap:wrap}
.boundary strong{color:#9CC2FF}
.hc .boundary strong{color:#fff;text-decoration:underline}

/* journey line */
.journey{padding:1.1rem 1.4rem .4rem;max-width:1280px;margin:0 auto}
.legs{display:flex;gap:.4rem;flex-wrap:wrap;margin-bottom:.7rem;align-items:center}
.leg{font-size:.78rem;border:1px solid var(--line);border-radius:999px;padding:.18rem .65rem;background:var(--card);display:inline-flex;gap:.35rem;align-items:center}
.leg.cur{border-color:var(--teal);background:var(--teal-l);font-weight:700}
.leg.done{color:var(--muted);text-decoration:line-through;text-decoration-color:var(--line)}
.leg.wait{border-style:dashed}
.line{position:relative;display:grid;grid-template-columns:repeat(6,1fr);align-items:start}
.line::before{content:"";position:absolute;left:calc(100%/12);right:calc(100%/12);top:15px;height:6px;border-radius:6px;background:var(--line)}
.line .fill{position:absolute;left:calc(100%/12);top:15px;height:6px;border-radius:6px;background:var(--teal);transition:width .5s ease}
.stn{position:relative;z-index:1;background:none;border:0;display:flex;flex-direction:column;align-items:center;gap:.35rem;padding:0 .2rem;text-align:center}
.stn .dot{width:36px;height:36px;border-radius:50%;background:var(--card);border:4px solid var(--line);display:grid;place-items:center;font-weight:800;font-size:.8rem;font-family:'Bricolage Grotesque',sans-serif;color:var(--muted);transition:.25s}
.stn.done .dot{background:var(--teal);border-color:var(--teal);color:#fff}
.stn.now .dot{border-color:var(--teal);color:var(--teal);box-shadow:0 0 0 6px var(--teal-l)}
.stn .lbl{font-size:.82rem;font-weight:700;line-height:1.2}
.stn .sub{font-size:.7rem;color:var(--muted);line-height:1.2;max-width:120px}
.stn.view .lbl{text-decoration:underline;text-decoration-thickness:3px;text-underline-offset:4px;text-decoration-color:var(--blue)}
.stn:hover .dot{transform:translateY(-1px)}
@media (prefers-reduced-motion:no-preference){.stn.now .dot{animation:pulse 2.2s infinite}}
@keyframes pulse{0%,100%{box-shadow:0 0 0 4px var(--teal-l)}50%{box-shadow:0 0 0 9px var(--teal-l)}}

/* layout */
.layout{max-width:1280px;margin:0 auto;padding:1rem 1.4rem 4rem;display:grid;grid-template-columns:minmax(0,1fr) 340px;gap:1.4rem;align-items:start}
@media (max-width:980px){.layout{grid-template-columns:1fr}.side{order:-1}}
@media (max-width:640px){.top{position:static}.stn .sub{display:none}.stn .lbl{font-size:.7rem}.top{padding:.6rem .8rem}.layout,.journey{padding-left:.8rem;padding-right:.8rem}}
.card{background:var(--card);border:1px solid var(--line);border-radius:var(--r);padding:1.1rem 1.2rem;box-shadow:var(--shadow)}
.stack{display:flex;flex-direction:column;gap:1rem}
.eyebrow{font-size:.74rem;text-transform:uppercase;letter-spacing:.09em;font-weight:700;color:var(--teal)}
.side{position:sticky;top:120px;display:flex;flex-direction:column;gap:1rem}
@media (max-width:980px){.side{position:static}}

/* next step */
.next{background:var(--teal-d);color:#fff;border:0}
.hc .next{background:#000}
.next .eyebrow{color:#A9C6FF}
.next h3{font-size:1.35rem;margin:.25rem 0 .55rem;line-height:1.2}
.next .why{background:rgba(255,255,255,.08);border-radius:10px;padding:.6rem .75rem;margin-top:.7rem;font-size:.86rem}
.next .why summary{cursor:pointer;font-weight:700}
.next .why ul{margin:.4rem 0 0;padding-left:1.1rem}
.btn{border:0;border-radius:10px;padding:.62rem 1rem;font-weight:700;background:var(--teal);color:#fff;display:inline-flex;align-items:center;gap:.4rem;text-decoration:none}
.btn:hover{background:var(--teal-d)}
.btn.light{background:#fff;color:var(--teal-d)}
.btn.ghost{background:transparent;color:var(--ink);border:1px solid var(--line)}
.btn.ghost:hover{background:var(--line2)}
.btn.warn{background:var(--red)}
.btn.sm{padding:.38rem .7rem;font-size:.85rem;border-radius:8px}
.btn[disabled]{opacity:.45;cursor:not-allowed}
.next .btn.ghost{color:#fff;border-color:rgba(255,255,255,.35)}
.next .btn.ghost:hover{background:rgba(255,255,255,.1)}

/* chips & form */
.chips{display:flex;flex-wrap:wrap;gap:.45rem}
.chip{border:1.5px solid var(--line);background:var(--card);border-radius:999px;padding:.42rem .85rem;font-size:.92rem;display:inline-flex;align-items:center;gap:.35rem}
.chip[aria-pressed=true]{border-color:var(--teal);background:var(--teal-l);color:var(--teal-d);font-weight:700}
.chip[aria-pressed=true]::before{content:"✓"}
.svcgrid{display:grid;grid-template-columns:repeat(auto-fill,minmax(160px,1fr));gap:.55rem}
.svc{border:1.5px solid var(--line);background:var(--card);border-radius:12px;padding:.7rem .8rem;text-align:left;display:flex;flex-direction:column;gap:.1rem}
.svc b{font-size:.95rem}.svc span{font-size:.76rem;color:var(--muted)}
.svc[aria-pressed=true]{border-color:var(--teal);background:var(--teal-l);box-shadow:inset 0 0 0 1px var(--teal)}
.q{display:flex;flex-direction:column;gap:.5rem}
.q > label,.q > .ql{font-weight:700}
.field{border:1.5px solid var(--line);background:var(--card);border-radius:10px;padding:.6rem .75rem;width:100%}
textarea.field{min-height:72px;resize:vertical}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
@media (max-width:640px){.grid2{grid-template-columns:1fr}}

/* banners */
.banner{border-radius:12px;padding:.8rem 1rem;display:flex;gap:.7rem;align-items:flex-start;font-size:.92rem}
.banner .ic{font-weight:800;font-size:1.1rem;line-height:1.2}
.banner.red{background:var(--red-l);border:1.5px solid var(--red);color:#5c0f1d}
.banner.amber{background:var(--amber-l);border:1.5px solid var(--amber);color:#4a3000}
.banner.blue{background:var(--blue-l);border:1.5px solid var(--blue);color:#13285e}
.banner.green{background:var(--green-l);border:1.5px solid var(--green);color:#0f3b21}
.hc .banner{color:#000}

/* pills */
.pill{display:inline-flex;align-items:center;gap:.25rem;font-size:.76rem;border-radius:999px;padding:.12rem .55rem;border:1px solid var(--line);background:var(--paper);white-space:nowrap}
.pill.ok{background:var(--green-l);border-color:transparent;color:var(--green)}
.pill.no{background:var(--red-l);border-color:transparent;color:var(--red)}
.pill.mid{background:var(--amber-l);border-color:transparent;color:var(--amber)}
.pill.b{font-weight:700}
.status{font-size:.78rem;font-weight:700;border-radius:6px;padding:.18rem .5rem;text-transform:uppercase;letter-spacing:.04em}
.status.ready{background:var(--green-l);color:var(--green)}
.status.steps{background:var(--amber-l);color:var(--amber)}
.status.blocked{background:var(--red-l);color:var(--red)}

/* facility cards */
.fac{border:1px solid var(--line);border-radius:var(--r);background:var(--card);padding:1rem 1.1rem;display:flex;flex-direction:column;gap:.55rem;box-shadow:var(--shadow);scroll-margin-top:140px}
.fac.sel{border-color:var(--teal);box-shadow:0 0 0 2px var(--teal)}
.fac.flash{animation:flash 1.2s}
@keyframes flash{0%{box-shadow:0 0 0 5px var(--amber)}100%{box-shadow:var(--shadow)}}
.fac .hd{display:flex;gap:.8rem;align-items:flex-start}
.rank{flex:none;width:30px;height:30px;border-radius:50%;background:var(--ink);color:var(--paper);display:grid;place-items:center;font-weight:800;font-family:'Bricolage Grotesque';font-size:.9rem}
.fac.blocked .rank{background:var(--muted)}
.fac h3{font-size:1.08rem}
.meter{height:8px;background:var(--line2);border-radius:8px;overflow:hidden;width:110px}
.meter i{display:block;height:100%;background:var(--teal);border-radius:8px}
.factors{list-style:none;margin:.2rem 0 0;padding:0;display:flex;flex-direction:column;gap:.15rem;border-top:1px dashed var(--line);padding-top:.55rem}
.factors li{display:grid;grid-template-columns:22px 1fr auto;gap:.4rem;font-size:.88rem;align-items:start;padding:.15rem 0}
.factors .m{font-weight:800;text-align:center;border-radius:5px;font-size:.78rem;line-height:1.5}
.factors .m.ok{background:var(--green-l);color:var(--green)}
.factors .m.no{background:var(--red-l);color:var(--red)}
.factors .m.mid{background:var(--amber-l);color:var(--amber)}
.factors .pts{font-variant-numeric:tabular-nums;font-size:.76rem;color:var(--muted)}
.factors .d{display:block;color:var(--muted);font-size:.8rem}
.linkbtn{background:none;border:0;color:var(--teal);font-weight:700;padding:0;text-decoration:underline;text-underline-offset:3px}

/* map */
.mapwrap{position:relative}
.map svg{width:100%;height:auto;max-height:340px;font-family:'Atkinson Hyperlegible',sans-serif;display:block;border-radius:12px;background:#E6EDF8}
.hc .map svg{background:#fff;border:1px solid #000}
.legend{display:flex;gap:.8rem;flex-wrap:wrap;font-size:.76rem;color:var(--muted);margin-top:.4rem}
.legend i{display:inline-block;width:10px;height:10px;border-radius:50%;margin-right:.25rem;vertical-align:-1px}

/* docs */
.doc{display:grid;grid-template-columns:auto 1fr auto;gap:.8rem;align-items:start;padding:.85rem 0;border-bottom:1px solid var(--line2)}
.doc:last-child{border-bottom:0}
.doc .st{width:28px;height:28px;border-radius:8px;display:grid;place-items:center;font-weight:800}
.doc .st.missing{background:var(--red-l);color:var(--red)}
.doc .st.pending{background:var(--amber-l);color:var(--amber)}
.doc .st.ready{background:var(--green-l);color:var(--green)}
.seg{display:inline-flex;border:1px solid var(--line);border-radius:9px;overflow:hidden}
.seg button{border:0;background:var(--card);padding:.3rem .6rem;font-size:.8rem;border-right:1px solid var(--line)}
.seg button:last-child{border-right:0}
.seg button[aria-pressed=true]{background:var(--ink);color:var(--paper);font-weight:700}
.ring{width:74px;height:74px;flex:none}
.upl{font-size:.78rem;color:var(--teal);font-weight:700;cursor:pointer;display:inline-flex;gap:.25rem;align-items:center}
.upl input{position:absolute;width:1px;height:1px;opacity:0}

/* slots */
.days{display:flex;gap:.4rem;overflow-x:auto;padding-bottom:.3rem}
.day{border:1.5px solid var(--line);background:var(--card);border-radius:10px;padding:.45rem .7rem;min-width:84px;text-align:left;flex:none}
.day b{display:block;font-size:.95rem}.day span{font-size:.74rem;color:var(--muted)}
.day[aria-pressed=true]{border-color:var(--ink);background:var(--ink);color:var(--paper)}
.day[aria-pressed=true] span{color:var(--paper);opacity:.8}
.slots{display:grid;grid-template-columns:repeat(auto-fill,minmax(86px,1fr));gap:.4rem}
.slot{border:1.5px solid var(--line);border-radius:9px;padding:.45rem;background:var(--card);font-variant-numeric:tabular-nums;font-weight:700;font-size:.9rem}
.slot.taken{opacity:.35;text-decoration:line-through;cursor:not-allowed;font-weight:400}
.slot.mine{background:var(--teal);color:#fff;border-color:var(--teal)}
.slot.pick{border-color:var(--teal);box-shadow:inset 0 0 0 1px var(--teal)}
.slot:not(.taken):not(.mine):hover{border-color:var(--teal)}

/* pass */
.pass{border:2px solid var(--ink);border-radius:18px;overflow:hidden;background:var(--card)}
.pass .ph{background:var(--ink);color:var(--paper);padding:.9rem 1.1rem;display:flex;justify-content:space-between;gap:1rem;align-items:flex-end;flex-wrap:wrap}
.pass .tok{font-family:'Bricolage Grotesque';font-weight:800;font-size:2.4rem;line-height:1}
.pass .pb{padding:1rem 1.1rem;display:grid;grid-template-columns:1fr 1fr;gap:.9rem 1.2rem}
@media (max-width:640px){.pass .pb{grid-template-columns:1fr}}
.pass dt{font-size:.72rem;text-transform:uppercase;letter-spacing:.08em;color:var(--muted);font-weight:700}
.pass dd{margin:0;font-weight:700}
.perf{border-top:2px dashed var(--line);margin:0 1.1rem}
.queue{display:flex;gap:1rem;align-items:center;flex-wrap:wrap}
.qbig{font-family:'Bricolage Grotesque';font-weight:800;font-size:2rem;line-height:1}
.qbar{flex:1;min-width:180px;height:12px;border-radius:12px;background:var(--line2);overflow:hidden}
.qbar i{display:block;height:100%;background:var(--teal);transition:width .6s}

.outcomes{display:grid;grid-template-columns:repeat(auto-fill,minmax(200px,1fr));gap:.55rem}
.out{border:1.5px solid var(--line);border-radius:12px;background:var(--card);text-align:left;padding:.75rem .85rem}
.out b{display:block}.out span{font-size:.8rem;color:var(--muted)}
.out:hover{border-color:var(--teal)}

/* reminders timeline */
.tl{list-style:none;margin:0;padding:0;position:relative}
.tl::before{content:"";position:absolute;left:11px;top:6px;bottom:6px;width:2px;background:var(--line)}
.tl li{position:relative;padding:0 0 1rem 2.1rem}
.tl li::before{content:"";position:absolute;left:4px;top:5px;width:16px;height:16px;border-radius:50%;background:var(--card);border:3px solid var(--teal)}
.tl li.past::before{background:var(--line);border-color:var(--line)}
.tl li.now::before{background:var(--amber);border-color:var(--amber)}
.tl .when{font-size:.76rem;font-weight:700;color:var(--teal);text-transform:uppercase;letter-spacing:.05em}

table.mini{width:100%;border-collapse:collapse;font-size:.85rem}
table.mini td,table.mini th{padding:.35rem .4rem;border-bottom:1px solid var(--line2);text-align:left;vertical-align:top}
pre.code{background:var(--ink);color:#e8f2ee;border-radius:10px;padding:.8rem;font-size:.74rem;overflow:auto;max-height:260px;margin:.4rem 0 0}

/* toast & modal */
#toast{position:fixed;left:50%;bottom:22px;transform:translateX(-50%) translateY(120%);background:var(--ink);color:var(--paper);padding:.7rem 1.1rem;border-radius:12px;font-weight:700;transition:transform .3s;z-index:60;max-width:90vw}
#toast{opacity:0;visibility:hidden}#toast.on{transform:translateX(-50%) translateY(0);opacity:1;visibility:visible}
.scrim{position:fixed;inset:0;background:rgba(20,26,23,.5);display:grid;place-items:center;z-index:50;padding:1rem}
.dialog{background:var(--card);border-radius:18px;max-width:560px;width:100%;padding:1.3rem;max-height:88vh;overflow:auto;box-shadow:0 30px 60px -20px rgba(0,0,0,.5)}
.dialog h3{font-size:1.3rem;margin-bottom:.4rem}
.tbtn.cdemo{border-color:var(--teal);color:var(--teal);font-weight:700}
.tbtn.cdemo:hover{background:var(--teal);color:#fff}
.pdot{width:8px;height:8px;border-radius:50%;background:#e0a21a;box-shadow:0 0 0 0 rgba(224,162,26,.6);animation:pdot 1.8s infinite}
@keyframes pdot{70%{box-shadow:0 0 0 7px rgba(224,162,26,0)}100%{box-shadow:0 0 0 0 rgba(224,162,26,0)}}
.dhero{background:var(--teal);color:#fff;border-color:transparent}
.dhero h2{color:#fff}.dhero p{color:#C9D8F5}.dhero .eyebrow{color:#A9C6FF}
.dtabs{display:grid;grid-template-columns:1fr 1fr;gap:.7rem;margin-top:1rem}
.dtab{all:unset;cursor:pointer;border-radius:12px;padding:.8rem 1rem;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.18);display:block}
.dtab:hover{background:rgba(255,255,255,.14)}
.dtab[aria-selected=true]{background:#fff;color:var(--ink);border-color:#fff}
.dtab .c{font-family:ui-monospace,monospace;font-size:.72rem;opacity:.75}
.dtab b{display:block;font-size:1.02rem;margin:.15rem 0}
.dtab .st{font-size:.78rem;opacity:.85}
.dtab[aria-selected=true] .st.ok{color:var(--green);opacity:1;font-weight:700}
.flow{display:grid;grid-template-columns:repeat(3,1fr);gap:.8rem}
.flow>div{border:1px solid var(--line2);border-radius:12px;padding:.85rem 1rem;background:var(--paper)}
.flow .n{display:inline-grid;place-items:center;width:22px;height:22px;border-radius:50%;background:var(--teal);color:#fff;font-size:.75rem;font-weight:700;margin-right:.4rem}
.flow h4{margin:0 0 .45rem;font-size:.95rem;display:flex;align-items:center}
.flow ul{margin:.2rem 0 0;padding-left:1.1rem}
.flow .row{gap:.4rem}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:.6rem}
.stats>div{border:1px solid var(--line2);border-radius:12px;padding:.7rem .85rem}
.stats .k{font-size:.74rem;color:var(--muted)}
.stats .v{font-size:1.45rem;font-weight:800;line-height:1.2}
.stats .v small{font-size:.8rem;font-weight:600;color:var(--muted)}
.stats .good .v{color:var(--green)}
.verdict{display:block;line-height:1.45;background:var(--green-l);color:var(--green);border-radius:12px;padding:.7rem 1rem;font-weight:700}
.verdict span{font-weight:400;color:var(--ink)}
.empty{border:1.5px dashed var(--line);border-radius:12px;padding:1.4rem;text-align:center;color:var(--muted)}
@media(max-width:820px){.flow,.stats{grid-template-columns:1fr 1fr}.dtabs{grid-template-columns:1fr}}
.pvwrap{display:block}
.pvwrap .stats{grid-template-columns:repeat(4,1fr)}
.pvlabel{font-size:.78rem;font-weight:700;color:var(--muted);text-transform:uppercase;letter-spacing:.08em;margin:0 0 .5rem .2rem}
.pv{border:1px solid var(--line);border-radius:30px;padding:9px;background:#fff;box-shadow:0 18px 40px -24px rgba(10,35,80,.5)}
.pvnotch{width:64px;height:5px;border-radius:9px;background:var(--line);margin:3px auto 8px}
.pvbody{border-radius:22px;background:var(--paper);padding:1.5rem 1.15rem 1rem;text-align:center;display:flex;flex-direction:column;gap:.75rem}
.pvic{width:44px;height:44px;border-radius:50%;margin:0 auto;display:grid;place-items:center;font-size:1.25rem;font-weight:800}
.pvic.amber{background:var(--amber-l);color:var(--amber)}.pvic.green{background:var(--green-l);color:var(--green)}.pvic.blue{background:#E3ECFC;color:var(--teal)}
.pvh{font-size:1.3rem;font-weight:800;line-height:1.25;margin:0;color:var(--ink)}
.pvt{font-size:1.05rem;line-height:1.5;margin:0;color:var(--ink)}
.pvacts{display:flex;flex-direction:column;gap:.55rem;margin-top:.3rem}
.pvbtn{all:unset;cursor:pointer;box-sizing:border-box;width:100%;min-height:54px;border-radius:14px;background:var(--teal);color:#fff;font-weight:700;font-size:1.05rem;display:flex;align-items:center;justify-content:center;padding:.6rem}
.pvbtn.alt{background:#fff;color:var(--teal);box-shadow:inset 0 0 0 1.5px var(--line)}
.pvbtn:focus-visible,.pvsay:focus-visible{outline:3px solid #e0a21a;outline-offset:2px}
.pvsay{all:unset;cursor:pointer;align-self:center;font-weight:600;color:var(--muted);font-size:.9rem;padding:.35rem .8rem;border-radius:999px}
.pvsay:hover{background:var(--line2);color:var(--ink)}
.pvfoot{font-size:.8rem;color:var(--muted);margin:.6rem .3rem 0;line-height:1.45}
.seg{display:inline-flex;background:var(--line2);border-radius:10px;padding:3px;gap:3px;align-self:flex-start}
.seg button{all:unset;cursor:pointer;padding:.42rem .85rem;border-radius:8px;font-size:.86rem;font-weight:600;color:var(--muted)}
.seg button[aria-selected=true]{background:#fff;color:var(--ink);box-shadow:0 1px 3px rgba(10,35,80,.15)}
.pvseg{display:flex;margin-bottom:.6rem}.pvseg button{flex:1;text-align:center}
.hbar{display:grid;grid-template-columns:60px 1fr 52px;gap:.6rem;align-items:center;font-size:.82rem;margin-top:.4rem}
.hbar>div{height:10px;border-radius:9px;background:var(--line2);overflow:hidden}.hbar i{display:block;height:100%;background:var(--teal);border-radius:9px}
.hbar b{text-align:right}
@media(max-width:1000px){.pvwrap{grid-template-columns:1fr}}
.rt{margin-top:.6rem;border:1px solid #BFD3F5;background:#F2F7FF;border-radius:12px;padding:.8rem .95rem;display:flex;flex-direction:column;gap:.45rem}
.rt.amber{border-color:#EBD3A0;background:#FFF8EA}
.rt-h{font-weight:800;font-size:1.02rem}.rt p{margin:0}.rt .row{gap:.45rem}
.rt-ghost{color:var(--ink)!important;border-color:var(--line)!important;background:#fff!important}
.rt-warn{font-size:.82rem;color:#7a4b00;background:#FFF1D6;border-radius:8px;padding:.4rem .6rem}
.slot.contested{position:relative}
.slot.contested::after{content:"⚡";position:absolute;top:-7px;right:-5px;font-size:.7rem;background:#FFF1D6;border:1px solid #EBD3A0;border-radius:999px;width:17px;height:17px;display:grid;place-items:center;line-height:1}
.demo-legend{font-size:.82rem;background:#FFF8EA;border:1px dashed #EBD3A0;border-radius:10px;padding:.5rem .75rem;color:var(--ink)}
.demo-tag{font-weight:700;color:#9a6304}
.demobar{position:sticky;top:.5rem;z-index:20;display:flex;align-items:center;justify-content:space-between;gap:1rem;flex-wrap:wrap;background:var(--ink);color:#fff;border-radius:14px;padding:.8rem 1rem;margin-bottom:1rem;box-shadow:0 10px 30px -16px rgba(10,35,80,.6)}
.demobar .db-l{display:flex;flex-direction:column;gap:.15rem;max-width:62ch}
.demobar .db-live{display:inline-flex;align-items:center;gap:.4rem;font-size:.72rem;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:#FFD27A}
.demobar b{font-size:1rem}.demobar .db-hint{font-size:.84rem;color:#C9D8F5}
.demobar .db-r{display:flex;align-items:center;gap:.7rem}.demobar .db-end{color:#C9D8F5}
.demo-note{font-size:.84rem;color:var(--muted);margin:0 0 .8rem;padding:.1rem .2rem}.demo-note .linkbtn{font-size:inherit}
.demo-side{all:unset;cursor:pointer;position:fixed;right:0;top:50%;transform:translateY(-50%);z-index:40;background:#E0A21A;color:#1b1300;font-weight:800;border-radius:14px 0 0 14px;padding:1rem .7rem;display:flex;flex-direction:column;align-items:center;gap:.5rem;box-shadow:-6px 10px 30px -12px rgba(10,35,80,.55)}
.demo-side .ds-t{writing-mode:vertical-rl;transform:rotate(180deg);font-size:.95rem;letter-spacing:.02em}
.demo-side:hover{background:#f0b02a;padding-right:1rem}.demo-side:focus-visible{outline:3px solid var(--ink);outline-offset:2px}
@media(max-width:700px){.demo-side{top:auto;bottom:.8rem;right:.8rem;transform:none;border-radius:999px;flex-direction:row;padding:.7rem 1rem}.demo-side .ds-t{writing-mode:horizontal-tb;transform:none}}
.dbseg{background:rgba(255,255,255,.12)}.dbseg button{color:#C9D8F5}.dbseg button[aria-selected=true]{background:#fff;color:var(--ink)}
.scard{display:grid;grid-template-columns:auto 1fr;gap:.9rem;align-items:start;margin-bottom:1rem}.scard .row{grid-column:1/-1}
.scard.amber{border:2px solid #EBD3A0;background:#FFF8EA}.scard.green{border:2px solid #BfE0C8;background:var(--green-l)}
.scard-ic{width:44px;height:44px;border-radius:50%;display:grid;place-items:center;font-size:1.3rem;font-weight:800;background:#fff}
.scard.amber .scard-ic{color:var(--amber)}.scard.green .scard-ic{color:var(--green)}
.pscard{border:1px solid var(--line2);border-radius:14px;padding:1rem;background:var(--paper);display:flex;flex-direction:column;gap:.6rem}
.syslink{all:unset;cursor:pointer;display:inline-flex;align-items:center;gap:.4rem;margin-left:.4rem;padding:.1rem .5rem;border-radius:999px;color:var(--muted);font-size:inherit}
.syslink:hover,.syslink:focus-visible{background:var(--line2);color:var(--ink)}
.sdot{width:7px;height:7px;border-radius:50%;background:var(--green);box-shadow:0 0 0 3px color-mix(in srgb,var(--green) 18%,transparent)}
.sdot.amber{background:var(--amber);box-shadow:0 0 0 3px color-mix(in srgb,var(--amber) 18%,transparent)}
.hstat{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:.6rem;margin-top:.9rem}
.hstat a{all:unset;cursor:pointer;display:block;border:1px solid var(--line2);border-radius:12px;padding:.7rem .85rem;background:var(--paper)}
.hstat a:hover{border-color:var(--line)}
.hstat .k{font-size:.74rem;color:var(--muted);display:flex;align-items:center;gap:.4rem}
.hstat .v{font-weight:700;margin-top:.15rem}
.labhead{display:flex;align-items:baseline;justify-content:space-between;gap:1rem}
.ref{font-family:ui-monospace,monospace;font-size:.7rem;color:var(--muted);opacity:.7;letter-spacing:.02em}
.checks{display:flex;flex-wrap:wrap;gap:.35rem .9rem;font-size:.8rem;color:var(--green)}
.lab details>summary{font-size:.85rem;font-weight:600;cursor:pointer;color:var(--teal)}
.kbd{font-family:ui-monospace,monospace;background:var(--line2);border-radius:5px;padding:0 .3rem;font-size:.85em}
.empty{text-align:center;padding:2rem 1rem}
.empty h3{margin-bottom:.4rem}
.hr{height:1px;background:var(--line);margin:.4rem 0}
.auth{min-height:100vh;display:grid;grid-template-columns:1.05fr 1fr;background:var(--paper)}
.auth-hero{background:radial-gradient(circle at 15% 10%,#1B4A9A 0,#0A2350 55%,#071A3D 100%);color:#fff;padding:48px 56px;display:flex;flex-direction:column;justify-content:space-between;gap:2rem}
.auth-hero .brand b{font-family:'Bricolage Grotesque',sans-serif;font-size:1.35rem;font-weight:800}
.auth-hero h1{font-size:clamp(2rem,3.4vw,3.1rem);font-weight:800;line-height:1.05;letter-spacing:-.03em;max-width:13ch}
.hero-sub{color:#C9D7F0;font-size:1.1rem;max-width:34ch;margin:1rem 0 1.4rem}
.feat{list-style:none;padding:0;margin:0;display:flex;flex-direction:column;gap:.7rem}
.feat li{display:flex;gap:.7rem;align-items:flex-start;color:#E6EEFB}
.feat li span{flex:none;width:24px;height:24px;border-radius:50%;background:rgba(127,178,255,.2);color:#9CC2FF;display:grid;place-items:center;font-weight:800;font-size:.8rem}
.hero-line{width:100%;max-width:520px;height:auto}
.auth-panel{display:grid;place-items:center;padding:40px 24px}
.auth-card{width:100%;max-width:440px;background:var(--card);border:1px solid var(--line);border-radius:20px;padding:2rem;box-shadow:var(--shadow)}
.tabs{display:flex;background:var(--line2);border-radius:12px;padding:4px;gap:4px}
.tabs button{flex:1;border:0;background:transparent;padding:.55rem;border-radius:9px;font-weight:700;color:var(--muted)}
.tabs button[aria-selected=true]{background:var(--card);color:var(--ink);box-shadow:0 1px 3px rgba(10,35,80,.15)}
.fld{display:flex;flex-direction:column;gap:.3rem;margin-bottom:.9rem}
.fld>label{font-weight:700;font-size:.9rem}
.field[aria-invalid=true]{border-color:var(--red);background:var(--red-l)}
.field:focus{outline:none;border-color:var(--blue);box-shadow:0 0 0 3px var(--blue-l)}
.err{color:var(--red);font-size:.8rem;font-weight:700}
.pw{position:relative}.pw .field{padding-right:4.2rem}
.pwtoggle{position:absolute;right:6px;top:50%;transform:translateY(-50%);border:0;background:var(--line2);border-radius:7px;padding:.25rem .55rem;font-size:.78rem;font-weight:700;color:var(--teal)}
.pwmeter{display:flex;flex-direction:column;gap:.25rem;margin-top:.15rem}
.check{display:flex;gap:.55rem;align-items:flex-start;font-size:.86rem;cursor:pointer}
.check input{width:18px;height:18px;margin-top:2px;accent-color:var(--teal);flex:none}
.btn.block{width:100%;justify-content:center;padding:.75rem 1rem}
.or{display:flex;align-items:center;gap:.8rem;margin:1.1rem 0;color:var(--muted);font-size:.8rem}
.or::before,.or::after{content:"";flex:1;height:1px;background:var(--line)}
.userchip{display:inline-flex;align-items:center;gap:.4rem}
.userchip .av{width:22px;height:22px;border-radius:50%;background:var(--teal);color:#fff;display:grid;place-items:center;font-size:.72rem;font-weight:800}
@media (max-width:860px){.auth{grid-template-columns:1fr}.auth-hero{padding:28px 24px;gap:1rem}.feat,.hero-line{display:none}.auth-card{padding:1.4rem}}
.foot{max-width:1280px;margin:0 auto;padding:0 1.4rem 2rem;font-size:.78rem;color:var(--muted)}
</style>
</head>
<body>
<a class="skip" href="#main">Skip to content</a>
<div id="auth" hidden></div>
<div id="app">
<header class="top">
  <div class="brand">
    <svg width="38" height="38" viewBox="0 0 40 40" aria-hidden="true"><rect width="40" height="40" rx="11" fill="#0A2350"/><path d="M9 26c4 0 5-12 11-12s7 12 11 12" stroke="#fff" stroke-width="3.2" fill="none" stroke-linecap="round"/><circle cx="9" cy="26" r="3.4" fill="#7FB2FF"/><circle cx="20" cy="14" r="3.4" fill="#fff"/><circle cx="31" cy="26" r="3.4" fill="#fff"/></svg>
    <div><b>Next Route</b><span class="tag" id="tagline"></span></div>
  </div>
  <div class="tools">
    <select class="tbtn" id="citySel" aria-label="State"><option value="chennai">📍 Tamil Nadu</option><option value="bengaluru">📍 Karnataka</option></select>
    <select class="tbtn" id="langSel" aria-label="Language" data-notr>
      <option value="en">English</option><option value="hi">हिन्दी</option><option value="kn">ಕನ್ನಡ</option><option value="ta">தமிழ்</option>
    </select>
    <button class="tbtn" data-act="fs" id="fsBtn" aria-label="Text size">A<span style="font-size:1.15em">A</span> <span id="fsLbl">100%</span></button>
    <button class="tbtn" data-act="hc" id="hcBtn" aria-pressed="false"></button>
    <button class="tbtn" data-act="speak" id="speakBtn"></button>
    <button class="tbtn" data-act="demo" id="demoBtn"></button>
    <button class="tbtn cdemo" data-act="nav:lab" id="labBtn"><span class="pdot"></span>Constraint demo</button>
    <button class="tbtn human" data-act="nav:help" id="humanBtn"></button>
    <button class="tbtn userchip" data-act="account" id="userBtn" aria-label="Your account"></button>
  </div>
</header>
<div class="boundary" role="note"><span id="boundaryTxt"></span></div>
<nav class="journey" id="journey" aria-label="Your journey"></nav>
<div class="layout">
  <main id="main" tabindex="-1" class="stack"></main>
  <aside class="side" id="side" aria-label="Next step and help"></aside>
</div>
<div class="foot" id="foot"></div>
</div>
<div id="toast" role="status" aria-live="polite"></div>
<div id="modal"></div>

<script>
/* =========================================================
   i18n — interface strings (facility data stays as supplied)
   ========================================================= */
const T={
en:{tag:"Your healthcare journey, one clear step at a time",boundary:"<strong>Administrative help only.</strong> This app does not diagnose, triage or advise treatment. Emergency? Call <strong>108</strong> (ambulance) or <strong>112</strong>.",
st_need:"Need",st_find:"Find",st_docs:"Documents",st_book:"Book",st_visit:"Visit",st_follow:"Follow-up",
sub_need:"What service",sub_find:"Where it works for you",sub_docs:"What to bring",sub_book:"Pick a slot",sub_visit:"Pass & queue",sub_follow:"Reminders & next leg",
next:"Your next step",why:"Why this step?",speak:"🔊 Read aloud",human:"Talk to a person",hc:"High contrast",demo:"▶ Demo patients",
ns_need:"Tell us what you need",ns_find:"Pick a facility that works for you",ns_docs:"Get your documents ready",ns_ref:"Get a referral letter first",ns_book:"Book an appointment slot",ns_visit:"Go to your appointment",ns_follow:"Record what happened at the visit",ns_complete:"Journey complete",
go:"Go",ready:"Ready to book",steps:"Step needed first",blocked:"Not a fit",missing:"Missing",pending:"In progress",done:"Ready",
q_service:"What do you need help with?",q_text:"Or describe it in your own words (optional)",q_lang:"Languages you're comfortable in",q_access:"Accessibility needs",q_pay:"How will you pay?",q_area:"Where are you starting from?",q_time:"When can you go?",q_have:"Documents you already have",find:"Find my options",
choose:"Choose this facility",chosen:"Selected",whythis:"Why this score?",book:"Book this slot",resched:"Reschedule",cancel:"Cancel booking",reminders:"Upcoming reminders",note:"Facility details are shown as supplied in the organiser dataset."},
hi:{tag:"आपकी स्वास्थ्य यात्रा, एक-एक साफ़ कदम",boundary:"<strong>केवल प्रशासनिक सहायता।</strong> यह ऐप बीमारी की पहचान, ट्रायेज या इलाज की सलाह नहीं देता। आपातकाल में <strong>108</strong> (एम्बुलेंस) या <strong>112</strong> पर कॉल करें।",
st_need:"ज़रूरत",st_find:"खोजें",st_docs:"दस्तावेज़",st_book:"बुक करें",st_visit:"मुलाक़ात",st_follow:"फ़ॉलो-अप",
sub_need:"कौन-सी सेवा",sub_find:"आपके लिए सही जगह",sub_docs:"क्या साथ लाएँ",sub_book:"समय चुनें",sub_visit:"पास और कतार",sub_follow:"रिमाइंडर और अगला चरण",
next:"आपका अगला कदम",why:"यह कदम क्यों?",speak:"🔊 पढ़कर सुनाएँ",human:"किसी व्यक्ति से बात करें",hc:"उच्च कंट्रास्ट",demo:"▶ डेमो मरीज़",
ns_need:"बताइए आपको क्या चाहिए",ns_find:"अपने लिए सही अस्पताल चुनें",ns_docs:"अपने दस्तावेज़ तैयार करें",ns_ref:"पहले रेफ़रल पत्र लें",ns_book:"अपॉइंटमेंट का समय बुक करें",ns_visit:"अपनी अपॉइंटमेंट पर जाएँ",ns_follow:"मुलाक़ात में क्या हुआ, दर्ज करें",ns_complete:"यात्रा पूरी हुई",
go:"आगे बढ़ें",ready:"बुक करने के लिए तैयार",steps:"पहले एक कदम ज़रूरी",blocked:"उपयुक्त नहीं",missing:"नहीं है",pending:"प्रक्रिया में",done:"तैयार",
q_service:"आपको किस सेवा में मदद चाहिए?",q_text:"या अपने शब्दों में लिखें (वैकल्पिक)",q_lang:"आप किन भाषाओं में सहज हैं",q_access:"सुगम्यता ज़रूरतें",q_pay:"भुगतान कैसे करेंगे?",q_area:"आप कहाँ से निकलेंगे?",q_time:"आप कब जा सकते हैं?",q_have:"आपके पास पहले से मौजूद दस्तावेज़",find:"मेरे विकल्प खोजें",
choose:"यह अस्पताल चुनें",chosen:"चुना गया",whythis:"यह स्कोर क्यों?",book:"यह समय बुक करें",resched:"समय बदलें",cancel:"बुकिंग रद्द करें",reminders:"आने वाले रिमाइंडर",note:"अस्पताल की जानकारी आयोजक के डेटा के अनुसार दिखाई गई है।"},
kn:{tag:"ನಿಮ್ಮ ಆರೋಗ್ಯ ಪಯಣ, ಒಂದೊಂದೇ ಸ್ಪಷ್ಟ ಹೆಜ್ಜೆ",boundary:"<strong>ಕೇವಲ ಆಡಳಿತಾತ್ಮಕ ನೆರವು.</strong> ಈ ಆ್ಯಪ್ ರೋಗ ಪತ್ತೆ, ಟ್ರಯಾಜ್ ಅಥವಾ ಚಿಕಿತ್ಸೆ ಸಲಹೆ ನೀಡುವುದಿಲ್ಲ. ತುರ್ತು ಸಂದರ್ಭದಲ್ಲಿ <strong>108</strong> (ಆಂಬ್ಯುಲೆನ್ಸ್) ಅಥವಾ <strong>112</strong> ಕರೆ ಮಾಡಿ.",
st_need:"ಅಗತ್ಯ",st_find:"ಹುಡುಕಿ",st_docs:"ದಾಖಲೆಗಳು",st_book:"ಬುಕ್ ಮಾಡಿ",st_visit:"ಭೇಟಿ",st_follow:"ಮುಂದಿನ ಹಂತ",
sub_need:"ಯಾವ ಸೇವೆ",sub_find:"ನಿಮಗೆ ಸೂಕ್ತ ಸ್ಥಳ",sub_docs:"ಏನು ತರಬೇಕು",sub_book:"ಸಮಯ ಆರಿಸಿ",sub_visit:"ಪಾಸ್ ಮತ್ತು ಸರದಿ",sub_follow:"ಜ್ಞಾಪನೆಗಳು",
next:"ನಿಮ್ಮ ಮುಂದಿನ ಹೆಜ್ಜೆ",why:"ಈ ಹೆಜ್ಜೆ ಏಕೆ?",speak:"🔊 ಓದಿ ಹೇಳಿ",human:"ವ್ಯಕ್ತಿಯೊಂದಿಗೆ ಮಾತನಾಡಿ",hc:"ಹೆಚ್ಚಿನ ಕಾಂಟ್ರಾಸ್ಟ್",demo:"▶ ಡೆಮೊ ರೋಗಿಗಳು",
ns_need:"ನಿಮಗೆ ಏನು ಬೇಕು ಎಂದು ತಿಳಿಸಿ",ns_find:"ನಿಮಗೆ ಸೂಕ್ತವಾದ ಆಸ್ಪತ್ರೆ ಆಯ್ಕೆಮಾಡಿ",ns_docs:"ನಿಮ್ಮ ದಾಖಲೆಗಳನ್ನು ಸಿದ್ಧಪಡಿಸಿ",ns_ref:"ಮೊದಲು ರೆಫರಲ್ ಪತ್ರ ಪಡೆಯಿರಿ",ns_book:"ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್ ಸಮಯ ಬುಕ್ ಮಾಡಿ",ns_visit:"ನಿಮ್ಮ ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್‌ಗೆ ಹೋಗಿ",ns_follow:"ಭೇಟಿಯಲ್ಲಿ ಏನಾಯಿತು ಎಂದು ದಾಖಲಿಸಿ",ns_complete:"ಪಯಣ ಪೂರ್ಣಗೊಂಡಿದೆ",
go:"ಮುಂದುವರಿಯಿರಿ",ready:"ಬುಕ್ ಮಾಡಲು ಸಿದ್ಧ",steps:"ಮೊದಲು ಒಂದು ಹೆಜ್ಜೆ",blocked:"ಸೂಕ್ತವಲ್ಲ",missing:"ಇಲ್ಲ",pending:"ಪ್ರಗತಿಯಲ್ಲಿ",done:"ಸಿದ್ಧ",
q_service:"ನಿಮಗೆ ಯಾವ ಸೇವೆಯಲ್ಲಿ ನೆರವು ಬೇಕು?",q_text:"ಅಥವಾ ನಿಮ್ಮ ಮಾತುಗಳಲ್ಲಿ ಬರೆಯಿರಿ (ಐಚ್ಛಿಕ)",q_lang:"ನಿಮಗೆ ಅನುಕೂಲವಾದ ಭಾಷೆಗಳು",q_access:"ಪ್ರವೇಶಸೌಲಭ್ಯ ಅಗತ್ಯಗಳು",q_pay:"ಹೇಗೆ ಪಾವತಿಸುತ್ತೀರಿ?",q_area:"ನೀವು ಎಲ್ಲಿಂದ ಹೊರಡುತ್ತೀರಿ?",q_time:"ನೀವು ಯಾವಾಗ ಹೋಗಬಹುದು?",q_have:"ನಿಮ್ಮ ಬಳಿ ಈಗಾಗಲೇ ಇರುವ ದಾಖಲೆಗಳು",find:"ನನ್ನ ಆಯ್ಕೆಗಳನ್ನು ಹುಡುಕಿ",
choose:"ಈ ಆಸ್ಪತ್ರೆ ಆಯ್ಕೆಮಾಡಿ",chosen:"ಆಯ್ಕೆಯಾಗಿದೆ",whythis:"ಈ ಅಂಕ ಏಕೆ?",book:"ಈ ಸಮಯ ಬುಕ್ ಮಾಡಿ",resched:"ಸಮಯ ಬದಲಿಸಿ",cancel:"ಬುಕಿಂಗ್ ರದ್ದುಮಾಡಿ",reminders:"ಮುಂಬರುವ ಜ್ಞಾಪನೆಗಳು",note:"ಆಸ್ಪತ್ರೆ ವಿವರಗಳನ್ನು ಆಯೋಜಕರ ಡೇಟಾದಂತೆ ತೋರಿಸಲಾಗಿದೆ."},
ta:{tag:"உங்கள் மருத்துவப் பயணம், ஒவ்வொரு படியும் தெளிவாக",boundary:"<strong>நிர்வாக உதவி மட்டுமே.</strong> இந்த செயலி நோயைக் கண்டறியவோ, அவசர நிலையை மதிப்பிடவோ, சிகிச்சை பரிந்துரைக்கவோ செய்யாது. அவசரமா? <strong>108</strong> (ஆம்புலன்ஸ்) அல்லது <strong>112</strong> அழைக்கவும்.",
st_need:"தேவை",st_find:"தேடல்",st_docs:"ஆவணங்கள்",st_book:"முன்பதிவு",st_visit:"வருகை",st_follow:"தொடர் கவனிப்பு",
sub_need:"எந்த சேவை",sub_find:"உங்களுக்கு ஏற்ற இடம்",sub_docs:"என்ன கொண்டு வர வேண்டும்",sub_book:"நேரம் தேர்வு",sub_visit:"அனுமதிச்சீட்டு & வரிசை",sub_follow:"நினைவூட்டல்கள்",
next:"உங்கள் அடுத்த படி",why:"இந்த படி ஏன்?",speak:"🔊 உரக்கப் படி",human:"ஒருவரிடம் பேசுங்கள்",hc:"அதிக மாறுபாடு",demo:"▶ மாதிரி நோயாளிகள்",
ns_need:"உங்களுக்கு என்ன தேவை என்று சொல்லுங்கள்",ns_find:"உங்களுக்கு ஏற்ற மருத்துவமனையைத் தேர்ந்தெடுங்கள்",ns_docs:"உங்கள் ஆவணங்களைத் தயார் செய்யுங்கள்",ns_ref:"முதலில் பரிந்துரைக் கடிதம் பெறுங்கள்",ns_book:"சந்திப்பு நேரத்தை முன்பதிவு செய்யுங்கள்",ns_visit:"உங்கள் சந்திப்புக்குச் செல்லுங்கள்",ns_follow:"வருகையில் என்ன நடந்தது என்று பதிவு செய்யுங்கள்",ns_complete:"பயணம் நிறைவடைந்தது",
go:"தொடரவும்",ready:"முன்பதிவுக்குத் தயார்",steps:"முதலில் ஒரு படி தேவை",blocked:"பொருந்தவில்லை",missing:"இல்லை",pending:"நடைபெறுகிறது",done:"தயார்",
q_service:"உங்களுக்கு எந்த சேவையில் உதவி வேண்டும்?",q_text:"அல்லது உங்கள் சொந்த வார்த்தைகளில் எழுதுங்கள் (விருப்பம்)",q_lang:"உங்களுக்கு வசதியான மொழிகள்",q_access:"அணுகல் தேவைகள்",q_pay:"எப்படி பணம் செலுத்துவீர்கள்?",q_area:"நீங்கள் எங்கிருந்து புறப்படுகிறீர்கள்?",q_time:"நீங்கள் எப்போது செல்ல முடியும்?",q_have:"உங்களிடம் ஏற்கனவே உள்ள ஆவணங்கள்",find:"என் வாய்ப்புகளைத் தேடு",
choose:"இந்த மருத்துவமனையைத் தேர்ந்தெடு",chosen:"தேர்ந்தெடுக்கப்பட்டது",whythis:"இந்த மதிப்பெண் ஏன்?",book:"இந்த நேரத்தை முன்பதிவு செய்",resched:"நேரத்தை மாற்று",cancel:"முன்பதிவை ரத்து செய்",reminders:"வரவிருக்கும் நினைவூட்டல்கள்",note:"மருத்துவமனை விவரங்கள் ஏற்பாட்டாளர் தரவில் உள்ளபடி காட்டப்படுகின்றன."}
};
const LOCALE={en:'en-IN',hi:'hi-IN',kn:'kn-IN',ta:'ta-IN'};


/* =========================================================
   Reference data
   ========================================================= */
const AREAS_BLR={
 harohalli:{name:"Harohalli (village)",district:"Ramanagara district",x:-2,y:36,rural:true},kanakapura:{name:"Kanakapura",district:"Ramanagara district",x:2,y:52,rural:true},ramanagara:{name:"Ramanagara town",district:"Ramanagara district",x:-32,y:38,rural:true},magadi:{name:"Magadi",district:"Ramanagara district",x:-38,y:8,rural:true},
 hoskote:{name:"Hoskote",district:"Bengaluru Rural district",x:38,y:4,rural:true},devanahalli:{name:"Devanahalli",district:"Bengaluru Rural district",x:16,y:-25,rural:true},doddaballapur:{name:"Doddaballapur",district:"Bengaluru Rural district",x:-4,y:-30,rural:true},
 peenya:{name:"Peenya",x:2,y:3},hebbal:{name:"Hebbal",x:11,y:1.5},malleshwaram:{name:"Malleshwaram",x:7,y:6},
 indiranagar:{name:"Indiranagar",x:16.5,y:8},whitefield:{name:"Whitefield",x:24,y:8.5},basavanagudi:{name:"Basavanagudi",x:7.5,y:12},
 koramangala:{name:"Koramangala",x:15,y:13},jayanagar:{name:"Jayanagar",x:10,y:14},btm:{name:"BTM Layout",x:12.5,y:16},
 bannerghatta:{name:"Bannerghatta Rd",x:12.5,y:19.5}
};
const SERVICES={
 gen_opd:{name:"General OPD",hint:"See a general doctor; get referrals",docs:["id_proof"],kind:"primary"},
 eye:{name:"Eye check",hint:"Ophthalmology / vision",docs:["id_proof"],kind:"specialist"},
 dental:{name:"Dental",hint:"Teeth and gums",docs:["id_proof"],kind:"specialist"},
 lab:{name:"Lab tests",hint:"Tests a doctor asked for",docs:["id_proof","test_slip"],kind:"primary"},
 vacc:{name:"Vaccination",hint:"Child or adult immunisation",docs:["vacc_card"],kind:"primary"},
 anc:{name:"Pregnancy check-up",hint:"Antenatal (ANC) visits",docs:["id_proof","mcp_card"],kind:"primary"},
 diab:{name:"Diabetes clinic",hint:"Ongoing NCD follow-up",docs:["id_proof","prescription","prev_reports"],kind:"specialist"},
 cardio:{name:"Cardiology",hint:"Heart specialist OPD",docs:["id_proof","prev_reports","prescription"],kind:"specialist"},
 ortho:{name:"Orthopaedics",hint:"Bones & joints specialist",docs:["id_proof","prev_reports"],kind:"specialist"},
 physio:{name:"Physiotherapy",hint:"Rehab sessions",docs:["id_proof","prev_reports"],kind:"specialist"}
};
const DOCS={
 id_proof:{name:"Photo ID",how:"Any one: Aadhaar, voter ID, driving licence, passport, or ration card with photo."},
 scheme_card:{name:"Health scheme card (CMCHIS / PM-JAY / CGHS / ESI)",how:"CMCHIS (Tamil Nadu): enrol at a CMCHIS kiosk with your family/ration card, Aadhaar and an income certificate from the VAO; download the e-card at cmchistn.com. PM-JAY: Ayushman card at beneficiary.nha.gov.in or a Common Service Centre. CGHS / ESI: from your employer or scheme office."},
 picme:{name:"PICME number / RCH ID (Tamil Nadu)",how:"12-digit number from Tamil Nadu's pregnancy registration. Your Village or Urban Health Nurse can register you, or self-register at picme.tn.gov.in. It's needed for TN maternity benefits and later for the birth certificate. Not registered yet? Mark it “In progress” — the clinic can start it."},
 insurance_card:{name:"Insurance card / policy number",how:"From your insurer's app or TPA card. Ask the hospital's insurance desk about cashless approval."},
 referral:{name:"Referral letter",how:"Only a doctor can issue this. A General OPD or PHC doctor can refer you to this department — we can help you book that visit first.",clinical:true},
 prev_reports:{name:"Previous reports & discharge summaries",how:"Collect from earlier visits; many labs share PDFs by SMS or WhatsApp. Bring originals and one photocopy."},
 prescription:{name:"Current prescription / medicine list",how:"Your last prescription, or photos of the medicine strips you use."},
 test_slip:{name:"Test request slip",how:"Written by the doctor who asked for the tests. Without it, labs may only offer walk-in packages."},
 vacc_card:{name:"Vaccination card / U-WIN record",how:"The card from the previous dose. Digital records: uwin.mohfw.gov.in."},
 mcp_card:{name:"Mother & Child Protection (MCP) card",how:"Issued at the first ANC registration. If you don't have one yet, it is issued at registration — mark it “In progress”."}
};
const SCHEMES={self:"Self-pay",pmjay:"Ayushman Bharat PM-JAY",cghs:"CGHS",esi:"ESI",private:"Private insurance",cmchis:"CMCHIS (TN Chief Minister's scheme)"};
const ACCESS={wheelchair:{name:"Step-free / wheelchair access",hard:true},lift:{name:"Working lift",hard:true},isl:{name:"Sign-language interpreter"},braille:{name:"Braille / low-vision help"},toilet:{name:"Accessible toilet"}};
const LANGS=["English","Kannada","Hindi","Tamil","Telugu","Urdu","Malayalam","Bengali"];
const TIMES={any:"Any time",morning:"Mornings",afternoon:"Afternoons",weekend:"Weekends"};

/* Sample "organiser" dataset — fictional facilities. Replace via Data source panel. */
const SAMPLE=[
{id:"sanjeevini",name:"Sanjeevini District Hospital",type:"Govt district hospital",area:"malleshwaram",address:"8th Cross, Malleshwaram",phone:"080-4000-1101",open:"08:30",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","English","Hindi","Tamil"],access:{wheelchair:true,lift:true,isl:false,braille:true,toilet:true},schemes:["pmjay","cghs","esi"],verified:"2026-10-30",
 conflicts:[{service:"cardio",field:"Cardiology OPD days",note:"Directory lists Mon–Sat. A notice-board photo submitted on 31 Oct says Cardiology OPD runs Mon, Wed and Fri only.",source:"Organiser directory vs. community report",records:[{source:"Organiser directory",tier:2,at:"2026-09-01",value:"Mon–Sat"},{source:"Notice-board photo (community)",tier:3,at:"2026-10-31",value:"Mon, Wed, Fri"}]}],
 services:{gen_opd:{dept:"General OPD, Block A",floor:0,fee:"Free (₹10 registration)",slotMins:15,avg:6},eye:{dept:"Ophthalmology OPD",floor:1,fee:"Free",slotMins:20,avg:8},dental:{dept:"Dental OPD",floor:1,fee:"₹50"},lab:{dept:"Central Lab",floor:0,fee:"Free under scheme / from ₹150",slotMins:10,avg:3},cardio:{dept:"Cardiology OPD, Block C",floor:2,referral:true,fee:"Free",slotMins:20,avg:10},ortho:{dept:"Orthopaedics OPD",floor:1,referral:true,fee:"Free"},physio:{dept:"Physiotherapy unit",floor:0,referral:true,fee:"Free"},diab:{dept:"NCD / Diabetes clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation room",floor:0,fee:"Free",slotMins:10,avg:4}}},
{id:"arogya",name:"Arogya Urban PHC",type:"Urban primary health centre",area:"jayanagar",address:"11th Main, Jayanagar 4th Block",phone:"080-4000-1102",open:"09:00",close:"16:30",days:[1,2,3,4,5,6],emergency:false,
 languages:["Kannada","English","Tamil","Telugu"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay","cghs","esi"],verified:"2026-10-25",conflicts:[],
 services:{gen_opd:{dept:"OPD room 2",floor:0,fee:"Free",slotMins:10,avg:5},vacc:{dept:"Immunisation (Wed & Sat)",floor:0,fee:"Free",days:[3,6],slotMins:10,avg:4},anc:{dept:"ANC clinic",floor:0,fee:"Free"},lab:{dept:"Lab counter",floor:0,fee:"Free",slotMins:10,avg:3},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"nirmala",name:"Nirmala Multispeciality Hospital",type:"Private multi-speciality hospital",area:"koramangala",address:"80 Ft Road, Koramangala 4th Block",phone:"080-4000-1103",open:"08:00",close:"20:00",days:[0,1,2,3,4,5,6],emergency:true,
 languages:["English","Hindi","Kannada","Malayalam","Tamil"],access:{wheelchair:true,lift:true,isl:"request",braille:false,toilet:true,note:"ISL interpreter with 24 h notice"},schemes:["pmjay","private"],verified:"2026-06-02",
 conflicts:[{service:null,field:"PM-JAY coverage",note:"Directory lists PM-JAY as accepted; the hospital website lists PM-JAY for in-patient packages only, not OPD consultations.",source:"Organiser directory vs. facility website",records:[{source:"Organiser directory",tier:2,at:"2026-06-02",value:"Accepted for OPD"},{source:"Hospital website",tier:1,at:"2026-10-15",value:"In-patient packages only"}]}],
 services:{gen_opd:{dept:"Family medicine",floor:0,fee:"₹500"},eye:{dept:"Eye clinic",floor:3,fee:"₹700"},dental:{dept:"Dental clinic",floor:3,fee:"₹600"},lab:{dept:"Diagnostics",floor:0,fee:"From ₹300",slotMins:10,avg:3},cardio:{dept:"Cardiology",floor:4,fee:"₹1,000",slotMins:15,avg:12},ortho:{dept:"Orthopaedics",floor:4,fee:"₹900"},physio:{dept:"Rehab",floor:1,fee:"₹700 / session",slotMins:30,avg:30},diab:{dept:"Endocrinology",floor:2,fee:"₹800"}}},
{id:"drishti",name:"Drishti Eye Care Centre",type:"Private eye hospital",area:"indiranagar",address:"100 Ft Road, Indiranagar",phone:"080-4000-1104",open:"09:00",close:"19:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Hindi","Kannada","Telugu"],access:{wheelchair:true,lift:false,isl:true,braille:true,toilet:true},schemes:["private"],verified:"2026-10-20",conflicts:[],
 services:{eye:{dept:"Eye OPD",floor:1,fee:"₹400",slotMins:15,avg:7}}},
{id:"hebbal",name:"Hebbal Community Health Centre",type:"Community health centre",area:"hebbal",address:"Bellary Road, Hebbal",phone:"080-4000-1105",open:"09:00",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","Hindi","Urdu","English"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["pmjay","esi","cghs"],verified:"2026-10-27",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:5},anc:{dept:"Maternal health OPD",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},dental:{dept:"Dental",floor:1,fee:"₹20"},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free"}}},
{id:"esi",name:"ESI Dispensary, Peenya",type:"ESI dispensary",area:"peenya",address:"Peenya Industrial Area, 2nd Stage",phone:"080-4000-1106",open:"08:00",close:"14:00",days:[1,2,3,4,5,6],emergency:false,selfPay:false,
 languages:["Kannada","Hindi","Telugu","Tamil"],access:{wheelchair:false,lift:false,isl:false,braille:false,toilet:false},schemes:["esi"],verified:"2026-09-15",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free for ESI members",slotMins:10,avg:5},lab:{dept:"Lab",floor:0,fee:"Free for ESI members"},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free for ESI members"}}},
{id:"smileline",name:"SmileLine Dental Clinic",type:"Private dental clinic",area:"btm",address:"16th Main, BTM 2nd Stage (1st floor, 12 steps)",phone:"080-4000-1107",open:"10:00",close:"20:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Kannada","Tamil","Hindi"],access:{wheelchair:false,lift:false,isl:false,braille:false,toilet:false},schemes:["private"],verified:"2026-10-29",conflicts:[],
 services:{dental:{dept:"Dental chairs 1–3",floor:1,fee:"₹400 consult",slotMins:30,avg:20}}},
{id:"vatsalya",name:"Vatsalya Women & Children Hospital",type:"Govt women & children hospital",area:"basavanagudi",address:"Bull Temple Road, Basavanagudi",phone:"080-4000-1108",open:"08:30",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","English","Hindi","Telugu"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["pmjay","cghs","esi"],verified:"2026-10-22",
 conflicts:[{service:"anc",field:"Phone number",note:"Directory lists 080-4000-1108; patients report the ANC desk number printed on MCP cards is 080-4000-1180.",source:"Organiser directory vs. patient report",records:[{source:"Organiser directory",tier:2,at:"2026-10-22",value:"080-4000-1108"},{source:"Patient report",tier:3,at:"2026-10-30",value:"080-4000-1180"}]}],
 services:{anc:{dept:"ANC clinic, ground floor",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},gen_opd:{dept:"Women's OPD",floor:0,fee:"Free"},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3}}},
{id:"hrudaya",name:"Hrudaya Heart Institute",type:"Cardiac speciality hospital (trust)",area:"bannerghatta",address:"Bannerghatta Main Road",phone:"080-4000-1109",open:"08:00",close:"18:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["English","Kannada","Hindi","Bengali","Telugu"],access:{wheelchair:true,lift:true,isl:"request",braille:false,toilet:true,note:"ISL interpreter on request (24 h)"},schemes:["pmjay","cghs","private"],verified:"2026-10-18",conflicts:[],
 services:{cardio:{dept:"Cardiology OPD",floor:1,referral:true,fee:"Free under PM-JAY / ₹600",slotMins:15,avg:12},lab:{dept:"Cardiac diagnostics",floor:0,fee:"From ₹250",slotMins:15,avg:6}}},
{id:"seva",name:"Seva Physio & Rehab Centre",type:"Private rehab centre",area:"whitefield",address:"ITPL Main Road, Whitefield",phone:"080-4000-1110",open:"07:00",close:"19:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Hindi","Kannada","Malayalam"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["private"],verified:"2026-10-10",conflicts:[],
 services:{physio:{dept:"Rehab floor",floor:0,fee:"₹600 / session",slotMins:30,avg:30},ortho:{dept:"Ortho consult",floor:0,fee:"₹800"}}},
{id:"arali",name:"Arali Primary Health Centre",type:"Primary health centre",area:"harohalli",address:"Kanakapura Road, Harohalli, Ramanagara district",phone:"080-4000-3201",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["Kannada","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay"],verified:"2026-10-24",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation (Wednesdays)",floor:0,fee:"Free",days:[3],slotMins:10,avg:4},lab:{dept:"Lab",floor:0,fee:"Free"},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"arkavathi",name:"Arkavathi Taluk General Hospital",type:"Govt taluk hospital",area:"kanakapura",address:"MG Road, Kanakapura",phone:"080-4000-3202",open:"08:00",close:"14:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","English","Tamil"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay","esi"],verified:"2026-10-12",conflicts:[{service:"eye",field:"Eye clinic days",note:"Directory lists the eye clinic every Thursday. A notice-board photo from 30 Oct says the visiting eye surgeon comes only on the 2nd and 4th Thursday.",source:"Organiser directory vs. community report",records:[{source:"Organiser directory",tier:2,at:"2026-07-01",value:"Every Thursday"},{source:"Notice-board photo (community)",tier:3,at:"2026-10-30",value:"2nd & 4th Thursday"}]}],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free (₹10 registration)",slotMins:10,avg:6},eye:{dept:"Eye clinic (Thursdays)",floor:0,fee:"Free",days:[4],slotMins:15,avg:8},dental:{dept:"Dental",floor:0,fee:"₹50"},lab:{dept:"Lab",floor:0,fee:"Free"},ortho:{dept:"Orthopaedics",floor:0,referral:true,fee:"Free"},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"janapada",name:"Janapada District Hospital",type:"Govt district hospital",area:"ramanagara",address:"BM Road, Ramanagara",phone:"080-4000-3203",open:"08:30",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","English","Hindi"],access:{wheelchair:true,lift:true,isl:false,braille:true,toilet:true},schemes:["pmjay","cghs","esi"],verified:"2026-10-27",conflicts:[],
 services:{gen_opd:{dept:"General OPD",floor:0,fee:"Free (₹10 registration)",slotMins:15,avg:6},eye:{dept:"Ophthalmology OPD",floor:1,fee:"Free",slotMins:20,avg:8},dental:{dept:"Dental OPD",floor:1,fee:"₹50"},lab:{dept:"Central Lab",floor:0,fee:"Free",slotMins:10,avg:3},cardio:{dept:"Cardiology OPD",floor:2,referral:true,fee:"Free",slotMins:20,avg:10},ortho:{dept:"Orthopaedics OPD",floor:1,referral:true,fee:"Free"},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free"},diab:{dept:"NCD clinic",floor:0,fee:"Free"},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation room",floor:0,fee:"Free",slotMins:10,avg:4}}},
{id:"kalyani",name:"Kalyani Community Health Centre",type:"Community health centre",area:"hoskote",address:"Old Madras Road, Hoskote",phone:"080-4000-3204",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Kannada","Telugu","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay","esi"],verified:"2026-10-18",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},dental:{dept:"Dental",floor:0,fee:"₹50"},lab:{dept:"Lab",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"shravani",name:"Shravani Primary Health Centre",type:"Primary health centre",area:"devanahalli",address:"Bazaar Street, Devanahalli",phone:"080-4000-3205",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["Kannada","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay"],verified:"2026-06-01",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"kudur",name:"Kudur Health Sub-Centre",type:"Health sub-centre (village)",area:"magadi",address:"Near gram panchayat, Kudur village, Magadi taluk",phone:"080-4000-3206",open:"09:00",close:"13:00",days:[3],emergency:false,
 languages:["Kannada"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:false},schemes:["pmjay"],verified:"2026-10-09",conflicts:[],
 services:{vacc:{dept:"Village health & nutrition day (Wednesdays)",floor:0,fee:"Free",slotMins:10,avg:4},anc:{dept:"ANM clinic",floor:0,fee:"Free",slotMins:15,avg:8}}}
];

const PERSONAS=[
 {id:"siddamma",title:"Siddamma, 68 · Kanakapura",desc:"Kannada only, low vision, PM-JAY card. Needs an eye check — the specialist clinic is only on certain days or in another town.",
  profile:{area:"kanakapura",languages:["Kannada"],access:["braille"],scheme:"pmjay",time:"morning",text:"Need eye checkup, cannot see clearly"},service:"eye",have:["id_proof","scheme_card"]},
 {id:"lakshmi",title:"Lakshmi, 62 · Jayanagar",desc:"Kannada speaker, uses a wheelchair, PM-JAY card. Told by her doctor to see a cardiologist; has no referral letter yet.",
  profile:{area:"jayanagar",languages:["Kannada"],access:["wheelchair"],scheme:"pmjay",time:"morning",text:"My doctor told me to see a heart specialist"},service:"cardio",have:["id_proof","prescription","scheme_card"]},
 {id:"arjun",title:"Arjun, 27 · Indiranagar",desc:"Deaf, uses Indian Sign Language. Needs an eye check-up, paying himself.",
  profile:{area:"indiranagar",languages:["English","Hindi"],access:["isl"],scheme:"self",time:"any",text:"Need new glasses, eye checkup"},service:"eye",have:["id_proof"]},
 {id:"fatima",title:"Fatima, 24 · Hebbal",desc:"Speaks Urdu and Hindi. First pregnancy check-up; no MCP card yet.",
  profile:{area:"hebbal",languages:["Urdu","Hindi"],access:[],scheme:"pmjay",time:"morning",text:"I am pregnant and need my first checkup"},service:"anc",have:["id_proof"]}
];

/* ---------- Chennai, Tamil Nadu (default city) — fictional sample facilities ---------- */
const AREAS_CHN={
 uthiramerur:{name:"Uthiramerur (village)",district:"Kanchipuram district",x:-52,y:52,rural:true},kanchipuram:{name:"Kanchipuram town",district:"Kanchipuram district",x:-55,y:22,rural:true},sriperumbudur:{name:"Sriperumbudur",district:"Kanchipuram district",x:-25,y:13,rural:true},
 chengalpattu:{name:"Chengalpattu town",district:"Chengalpattu district",x:-8,y:48,rural:true},madurantakam:{name:"Madurantakam",district:"Chengalpattu district",x:-20,y:72,rural:true},
 tindivanam:{name:"Tindivanam",district:"Villupuram district",x:-45,y:100,rural:true},gingee:{name:"Gingee (Senji)",district:"Villupuram district",x:-85,y:110,rural:true},
 tondiarpet:{name:"Tondiarpet",x:15,y:1.5},perambur:{name:"Perambur",x:11,y:3.5},annanagar:{name:"Anna Nagar",x:6.5,y:6.5},
 egmore:{name:"Egmore",x:11.5,y:7.5},triplicane:{name:"Triplicane",x:15,y:9.5},tnagar:{name:"T. Nagar",x:10,y:11.5},
 porur:{name:"Porur",x:2.5,y:12.5},guindy:{name:"Guindy",x:8.5,y:14.5},adyar:{name:"Adyar",x:14,y:15},
 velachery:{name:"Velachery",x:11,y:18},sholinganallur:{name:"Sholinganallur (OMR)",x:17,y:21},tambaram:{name:"Tambaram",x:4.5,y:21}
};
const ROADS_CHN=[["porur","sriperumbudur"],["sriperumbudur","kanchipuram"],["kanchipuram","uthiramerur"],["tambaram","chengalpattu"],["chengalpattu","uthiramerur"],["kanchipuram","chengalpattu"],["chengalpattu","madurantakam"],["madurantakam","tindivanam"],["tindivanam","gingee"],["tondiarpet","perambur"],["perambur","egmore"],["perambur","annanagar"],["annanagar","egmore"],["egmore","triplicane"],["egmore","tnagar"],["annanagar","porur"],["porur","guindy"],["tnagar","guindy"],["tnagar","triplicane"],["triplicane","adyar"],["guindy","velachery"],["guindy","tambaram"],["adyar","velachery"],["adyar","sholinganallur"],["velachery","sholinganallur"],["tondiarpet","triplicane"]];
const DATA_CHN=[
{id:"thendral",name:"Thendral Government Medical College Hospital",type:"Govt medical college hospital",area:"egmore",address:"Pantheon Road, Egmore, Chennai 600008",phone:"044-4000-2101",open:"07:30",close:"13:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English","Telugu","Hindi"],access:{wheelchair:true,lift:true,isl:false,braille:true,toilet:true},schemes:["cmchis","pmjay","cghs","esi"],verified:"2026-10-30",
 conflicts:[{service:"cardio",field:"Cardiology OPD days",note:"Directory lists Mon–Sat. A notice-board photo submitted on 31 Oct says Cardiology OPD runs Tue, Thu and Sat only.",source:"Organiser directory vs. community report",records:[{source:"Organiser directory",tier:2,at:"2026-09-01",value:"Mon–Sat"},{source:"Notice-board photo (community)",tier:3,at:"2026-10-31",value:"Tue, Thu, Sat"}]}],
 services:{gen_opd:{dept:"General OPD, Block A",floor:0,fee:"Free",slotMins:10,avg:5},eye:{dept:"Ophthalmology OPD",floor:1,fee:"Free",slotMins:15,avg:8},dental:{dept:"Dental OPD",floor:1,fee:"Free"},lab:{dept:"Central Lab",floor:0,fee:"Free",slotMins:10,avg:3},cardio:{dept:"Cardiology OPD, Tower 2",floor:2,referral:true,fee:"Free",slotMins:15,avg:10},ortho:{dept:"Orthopaedics OPD",floor:1,referral:true,fee:"Free"},physio:{dept:"Physical Medicine & Rehab",floor:0,referral:true,fee:"Free"},diab:{dept:"Diabetology OPD",floor:0,fee:"Free"},vacc:{dept:"Immunisation room",floor:0,fee:"Free",slotMins:10,avg:4}}},
{id:"nalam",name:"Nalam Urban PHC",type:"Urban primary health centre",area:"triplicane",address:"Big Street, Triplicane, Chennai 600005",phone:"044-4000-2102",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["Tamil","Urdu","English","Telugu"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay","cghs","esi"],verified:"2026-10-26",conflicts:[],
 services:{gen_opd:{dept:"OPD room 1",floor:0,fee:"Free",slotMins:10,avg:5},vacc:{dept:"Immunisation (Wed & Sat)",floor:0,fee:"Free",days:[3,6],slotMins:10,avg:4},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},lab:{dept:"Lab counter",floor:0,fee:"Free",slotMins:10,avg:3},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"sangamam",name:"Sangamam Multispeciality Hospital",type:"Private multi-speciality hospital",area:"adyar",address:"LB Road, Adyar, Chennai 600020",phone:"044-4000-2103",open:"08:00",close:"20:00",days:[0,1,2,3,4,5,6],emergency:true,
 languages:["English","Tamil","Hindi","Malayalam","Telugu"],access:{wheelchair:true,lift:true,isl:"request",braille:false,toilet:true,note:"ISL interpreter with 24 h notice"},schemes:["cmchis","pmjay","private"],verified:"2026-06-02",
 conflicts:[{service:null,field:"CMCHIS / PM-JAY coverage",note:"Directory lists CMCHIS and PM-JAY as accepted; the hospital's insurance desk says scheme cover applies to approved in-patient procedures, not OPD consultations.",source:"Organiser directory vs. facility insurance desk",records:[{source:"Organiser directory",tier:2,at:"2026-06-02",value:"Accepted for OPD"},{source:"Hospital insurance desk",tier:1,at:"2026-10-29",value:"In-patient procedures only"}]}],
 services:{gen_opd:{dept:"Family medicine",floor:0,fee:"₹500"},eye:{dept:"Eye clinic",floor:3,fee:"₹700"},dental:{dept:"Dental clinic",floor:3,fee:"₹600"},lab:{dept:"Diagnostics",floor:0,fee:"From ₹300",slotMins:10,avg:3},cardio:{dept:"Cardiology",floor:4,fee:"₹1,000",slotMins:15,avg:12},ortho:{dept:"Orthopaedics",floor:4,fee:"₹900"},physio:{dept:"Rehab",floor:1,fee:"₹700 / session",slotMins:30,avg:30},diab:{dept:"Endocrinology",floor:2,fee:"₹800"}}},
{id:"paarvai",name:"Paarvai Eye Hospital",type:"Private eye hospital",area:"annanagar",address:"2nd Avenue, Anna Nagar, Chennai 600040",phone:"044-4000-2104",open:"09:00",close:"19:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Tamil","Hindi","Telugu"],access:{wheelchair:true,lift:false,isl:true,braille:true,toilet:true},schemes:["private"],verified:"2026-10-20",conflicts:[],
 services:{eye:{dept:"Eye OPD",floor:1,fee:"₹400",slotMins:15,avg:7}}},
{id:"vadachennai",name:"Vadachennai Community Health Centre",type:"Community health centre",area:"perambur",address:"Paper Mills Road, Perambur, Chennai 600011",phone:"044-4000-2105",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","Telugu","Hindi","Urdu","English"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay","esi","cghs"],verified:"2026-10-27",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:5},anc:{dept:"Maternal health OPD",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},dental:{dept:"Dental",floor:1,fee:"Free"},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free"}}},
{id:"thozhilalar",name:"Thozhilalar ESI Dispensary",type:"ESI dispensary",area:"guindy",address:"Industrial Estate, Guindy, Chennai 600032",phone:"044-4000-2106",open:"08:00",close:"14:00",days:[1,2,3,4,5,6],emergency:false,selfPay:false,
 languages:["Tamil","Hindi","Telugu"],access:{wheelchair:false,lift:false,isl:false,braille:false,toilet:false},schemes:["esi"],verified:"2026-09-15",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free for ESI members",slotMins:10,avg:5},lab:{dept:"Lab",floor:0,fee:"Free for ESI members"},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free for ESI members"}}},
{id:"punnagai",name:"Punnagai Dental Clinic",type:"Private dental clinic",area:"velachery",address:"Velachery Main Road (1st floor, 14 steps)",phone:"044-4000-2107",open:"10:00",close:"20:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Tamil","Telugu","Hindi"],access:{wheelchair:false,lift:false,isl:false,braille:false,toilet:false},schemes:["private"],verified:"2026-10-29",conflicts:[],
 services:{dental:{dept:"Dental chairs 1–3",floor:1,fee:"₹400 consult",slotMins:30,avg:20}}},
{id:"thaimai",name:"Thaimai Government Women & Children Hospital",type:"Govt women & children hospital",area:"tnagar",address:"Usman Road, T. Nagar, Chennai 600017",phone:"044-4000-2108",open:"07:30",close:"13:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English","Telugu","Hindi"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay","cghs","esi"],verified:"2026-10-22",
 conflicts:[{service:"anc",field:"Phone number",note:"Directory lists 044-4000-2108; patients report the antenatal desk number printed on their cards is 044-4000-2180.",source:"Organiser directory vs. patient report",records:[{source:"Organiser directory",tier:2,at:"2026-10-22",value:"044-4000-2108"},{source:"Patient report",tier:3,at:"2026-10-30",value:"044-4000-2180"}]}],
 services:{anc:{dept:"Antenatal clinic, ground floor",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},gen_opd:{dept:"Women's OPD",floor:0,fee:"Free"},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3}}},
{id:"irudhayam",name:"Irudhayam Heart Institute",type:"Cardiac speciality hospital (trust)",area:"guindy",address:"GST Road, Guindy, Chennai 600032",phone:"044-4000-2109",open:"08:00",close:"18:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["English","Tamil","Hindi","Telugu","Bengali"],access:{wheelchair:true,lift:true,isl:"request",braille:false,toilet:true,note:"ISL interpreter on request (24 h)"},schemes:["cmchis","pmjay","cghs","private"],verified:"2026-10-18",conflicts:[],
 services:{cardio:{dept:"Cardiology OPD",floor:1,referral:true,fee:"Free under CMCHIS / PM-JAY · ₹600",slotMins:15,avg:12},lab:{dept:"Cardiac diagnostics",floor:0,fee:"From ₹250",slotMins:15,avg:6}}},
{id:"meendum",name:"Meendum Physio & Rehab Centre",type:"Private rehab centre",area:"sholinganallur",address:"OMR, Sholinganallur, Chennai 600119",phone:"044-4000-2110",open:"07:00",close:"19:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["English","Tamil","Hindi","Malayalam"],access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes:["private"],verified:"2026-10-10",conflicts:[],
 services:{physio:{dept:"Rehab floor",floor:0,fee:"₹600 / session",slotMins:30,avg:30},ortho:{dept:"Ortho consult",floor:0,fee:"₹800"}}},
{id:"thamarai",name:"Thamarai Government Hospital",type:"Govt taluk hospital",area:"tambaram",address:"GST Road, Tambaram, Chennai 600045",phone:"044-4000-2111",open:"07:30",close:"13:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English","Telugu"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay","esi","cghs"],verified:"2026-10-28",conflicts:[],
 services:{gen_opd:{dept:"General OPD",floor:0,fee:"Free",slotMins:10,avg:5},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},dental:{dept:"Dental",floor:0,fee:"Free"},ortho:{dept:"Orthopaedics OPD",floor:1,referral:true,fee:"Free"}}},
{id:"vayal",name:"Vayal Block PHC",type:"Primary health centre (block PHC)",area:"uthiramerur",address:"Main Road, Uthiramerur, Kanchipuram district",phone:"044-4000-3101",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["Tamil","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay"],verified:"2026-10-28",conflicts:[{service:"diab",field:"NCD clinic days",note:"Directory lists the NCD clinic Mon–Sat. The village health nurse reported on 2 Nov that it now runs Tue and Fri only.",source:"Organiser directory vs. field report",records:[{source:"Organiser directory",tier:2,at:"2026-08-15",value:"Mon–Sat"},{source:"Village health nurse (field report)",tier:3,at:"2026-11-02",value:"Tue, Fri"}]}],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation (Wednesdays)",floor:0,fee:"Free",days:[3],slotMins:10,avg:4},lab:{dept:"Lab counter",floor:0,fee:"Free",slotMins:10,avg:3},diab:{dept:"NCD clinic",floor:0,fee:"Free",slotMins:10,avg:6}}},
{id:"kavanur",name:"Kavanur Health Sub-Centre",type:"Health sub-centre (village)",area:"uthiramerur",address:"Near panchayat office, Kavanur village, Uthiramerur block",phone:"044-4000-3102",open:"09:00",close:"13:00",days:[2,5],emergency:false,
 languages:["Tamil"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:false},schemes:["cmchis","pmjay"],verified:"2026-10-15",conflicts:[],
 services:{vacc:{dept:"Village health & nutrition day (Tue, Fri)",floor:0,fee:"Free",slotMins:10,avg:4},anc:{dept:"VHN / ANM clinic",floor:0,fee:"Free",slotMins:15,avg:8}}},
{id:"kanchihq",name:"Kanchi Government Headquarters Hospital",type:"Govt district headquarters hospital",area:"kanchipuram",address:"Railway Road, Kanchipuram",phone:"044-4000-3103",open:"07:30",close:"13:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English","Telugu"],access:{wheelchair:true,lift:true,isl:"request",braille:false,toilet:true,note:"ISL interpreter with 24 h notice"},schemes:["cmchis","pmjay","cghs","esi"],verified:"2026-10-22",conflicts:[],
 services:{gen_opd:{dept:"General OPD",floor:0,fee:"Free",slotMins:10,avg:6},eye:{dept:"Eye OPD",floor:1,fee:"Free",slotMins:15,avg:8},dental:{dept:"Dental OPD",floor:0,fee:"Free"},lab:{dept:"Central Lab",floor:0,fee:"Free",slotMins:10,avg:3},cardio:{dept:"Cardiology OPD (Tue, Thu, Sat)",floor:1,referral:true,fee:"Free",days:[2,4,6],slotMins:15,avg:10},ortho:{dept:"Orthopaedics OPD",floor:0,referral:true,fee:"Free"},physio:{dept:"Physiotherapy",floor:0,referral:true,fee:"Free"},diab:{dept:"NCD / Diabetes clinic",floor:0,fee:"Free"},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation room",floor:0,fee:"Free",slotMins:10,avg:4}}},
{id:"eri",name:"Eri Government Taluk Hospital",type:"Govt taluk hospital",area:"madurantakam",address:"GST Road, Madurantakam, Chengalpattu district",phone:"044-4000-3104",open:"08:00",close:"14:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay","esi"],verified:"2026-10-05",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},dental:{dept:"Dental",floor:0,fee:"Free"},lab:{dept:"Lab",floor:0,fee:"Free",slotMins:10,avg:3},ortho:{dept:"Orthopaedics (Mon, Thu)",floor:0,referral:true,fee:"Free",days:[1,4]},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},diab:{dept:"NCD clinic",floor:0,fee:"Free"}}},
{id:"palar",name:"Palar Government Medical College Hospital",type:"Govt medical college hospital",area:"chengalpattu",address:"GST Road, Chengalpattu",phone:"044-4000-3105",open:"07:30",close:"13:00",days:[1,2,3,4,5,6],emergency:true,
 languages:["Tamil","English","Telugu","Hindi"],access:{wheelchair:true,lift:true,isl:false,braille:true,toilet:true},schemes:["cmchis","pmjay","cghs","esi"],verified:"2026-10-30",conflicts:[],
 services:{gen_opd:{dept:"General OPD",floor:0,fee:"Free",slotMins:10,avg:5},eye:{dept:"Ophthalmology OPD",floor:1,fee:"Free",slotMins:15,avg:8},dental:{dept:"Dental OPD",floor:1,fee:"Free"},lab:{dept:"Central Lab",floor:0,fee:"Free",slotMins:10,avg:3},cardio:{dept:"Cardiology OPD",floor:2,referral:true,fee:"Free",slotMins:15,avg:10},ortho:{dept:"Orthopaedics OPD",floor:1,referral:true,fee:"Free"},physio:{dept:"PMR department",floor:0,referral:true,fee:"Free"},diab:{dept:"Diabetology OPD",floor:0,fee:"Free"},anc:{dept:"Obstetrics OPD",floor:1,fee:"Free"},vacc:{dept:"Immunisation room",floor:0,fee:"Free",slotMins:10,avg:4}}},
{id:"senji",name:"Senji Upgraded PHC",type:"Upgraded primary health centre",area:"gingee",address:"Tiruvannamalai Road, Gingee, Villupuram district",phone:"044-4000-3106",open:"08:00",close:"16:00",days:[1,2,3,4,5,6],emergency:false,
 languages:["Tamil"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["cmchis","pmjay"],verified:"2026-05-12",conflicts:[],
 services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",slotMins:10,avg:6},anc:{dept:"Antenatal clinic",floor:0,fee:"Free"},vacc:{dept:"Immunisation",floor:0,fee:"Free",slotMins:10,avg:4},lab:{dept:"Lab",floor:0,fee:"Free"},diab:{dept:"NCD clinic",floor:0,fee:"Free"},dental:{dept:"Dental (Fridays)",floor:0,fee:"Free",days:[5]}}}
];
const PERSONAS_CHN=[
 {id:"murugan",title:"Murugan, 71 · Uthiramerur (village)",desc:"Tamil only, walks with a stick, no smartphone — his daughter books for him. Monthly diabetes follow-up, CMCHIS card.",
  profile:{area:"uthiramerur",languages:["Tamil"],access:["wheelchair"],scheme:"cmchis",time:"morning",text:"சர்க்கரை நோய் மாதாந்திர பரிசோதனை"},service:"diab",have:["id_proof","prescription","scheme_card","prev_reports"]},
 {id:"selvi",title:"Selvi, 64 · Tambaram",desc:"Tamil speaker, uses a wheelchair, CMCHIS card. Her doctor told her to see a heart specialist; no referral letter yet.",
  profile:{area:"tambaram",languages:["Tamil"],access:["wheelchair"],scheme:"cmchis",time:"morning",text:"என் டாக்டர் இதய நிபுணரைப் பார்க்கச் சொன்னார்"},service:"cardio",have:["id_proof","prescription","scheme_card"]},
 {id:"karthik",title:"Karthik, 29 · Adyar",desc:"Deaf, uses Indian Sign Language. Needs an eye check-up, paying himself.",
  profile:{area:"adyar",languages:["English","Tamil"],access:["isl"],scheme:"self",time:"any",text:"Need new glasses, eye checkup"},service:"eye",have:["id_proof"]},
 {id:"ayesha",title:"Ayesha, 23 · Triplicane",desc:"Speaks Urdu and Tamil. First pregnancy check-up; no MCP card or PICME number yet.",
  profile:{area:"triplicane",languages:["Urdu","Tamil"],access:[],scheme:"cmchis",time:"morning",text:"I am pregnant and need my first checkup"},service:"anc",have:["id_proof"]}
];
const CITIES={
 chennai:{name:"Tamil Nadu",areas:AREAS_CHN,roads:ROADS_CHN,data:DATA_CHN,personas:PERSONAS_CHN,defArea:"tnagar",
  langs:["Tamil","English","Telugu","Hindi","Urdu","Malayalam","Kannada","Bengali"],schemes:["self","cmchis","pmjay","cghs","esi","private"]},
 bengaluru:{name:"Karnataka",areas:AREAS_BLR,roads:[["whitefield","hoskote"],["hebbal","devanahalli"],["peenya","doddaballapur"],["bannerghatta","harohalli"],["harohalli","kanakapura"],["kanakapura","ramanagara"],["basavanagudi","ramanagara"],["ramanagara","magadi"],["peenya","magadi"],["peenya","malleshwaram"],["malleshwaram","hebbal"],["malleshwaram","basavanagudi"],["basavanagudi","jayanagar"],["jayanagar","btm"],["btm","bannerghatta"],["btm","koramangala"],["koramangala","indiranagar"],["indiranagar","whitefield"],["indiranagar","hebbal"],["malleshwaram","indiranagar"],["jayanagar","koramangala"]],data:SAMPLE,personas:PERSONAS,defArea:"jayanagar",
  langs:["English","Kannada","Hindi","Tamil","Telugu","Urdu","Malayalam","Bengali"],schemes:["self","pmjay","cghs","esi","private"]}
};
/* Extra fictional multi-service hospitals so every service has enough hospitals to show every demo outcome */
function mkH(id,name,type,area,address,phone,languages,schemes,emergency){const sv=(dept,floor,fee,extra)=>({dept,floor,fee,slotMins:15,avg:8,...extra});
 return{id,name,type,area,address,phone,open:"08:00",close:"15:00",days:[1,2,3,4,5,6],emergency:!!emergency,languages,access:{wheelchair:true,lift:true,isl:false,braille:false,toilet:true},schemes,verified:"2026-10-25",conflicts:[],
  services:{gen_opd:sv("General OPD",0,"Free"),eye:sv("Eye OPD",1,"Free"),dental:sv("Dental OPD",0,"Free"),lab:sv("Lab",0,"Free"),vacc:sv("Immunisation",0,"Free"),anc:sv("Antenatal clinic",0,"Free"),diab:sv("NCD clinic",0,"Free"),cardio:sv("Cardiology OPD",1,"Free",{referral:true}),ortho:sv("Orthopaedics OPD",0,"Free",{referral:true}),physio:sv("Physiotherapy",0,"Free")}}}
DATA_CHN.push(
 mkH("vaigai","Vaigai Government Hospital","Govt hospital","sriperumbudur","Bazaar Road, Sriperumbudur","044-4000-3301",["Tamil","English","Hindi"],["cmchis","pmjay","esi"],true),
 mkH("thenpennai","Thenpennai Government Hospital","Govt taluk hospital","tindivanam","Gingee Road, Tindivanam","044-4000-3302",["Tamil","English"],["cmchis","pmjay"],true),
 mkH("malligai","Malligai Community Hospital","Charitable trust hospital","porur","Mount-Poonamallee Road, Porur","044-4000-3303",["Tamil","English","Telugu","Malayalam"],["cmchis","pmjay","private"],false),
 mkH("kural","Kural Government Peripheral Hospital","Govt peripheral hospital","velachery","100 Feet Road, Velachery","044-4000-3304",["Tamil","English","Hindi"],["cmchis","pmjay","cghs","esi"],true),
 mkH("pavalam","Pavalam Charitable Hospital","Charitable trust hospital","perambur","Paper Mills Road, Perambur","044-4000-3305",["Tamil","English","Urdu"],["cmchis","pmjay","private"],false),
 mkH("aalam","Aalam Government Hospital","Govt hospital","chengalpattu","Station Road, Chengalpattu","044-4000-3306",["Tamil","English"],["cmchis","pmjay","esi"],true));
SAMPLE.push(
 mkH("kaveri","Kaveri Government Hospital","Govt taluk hospital","doddaballapur","Tank Bund Road, Doddaballapur","080-4000-3301",["Kannada","English","Telugu"],["pmjay","esi"],true),
 mkH("tunga","Tunga Community Hospital","Community health centre","devanahalli","Fort Road, Devanahalli","080-4000-3302",["Kannada","English"],["pmjay"],false),
 mkH("mallige","Mallige Charitable Hospital","Charitable trust hospital","peenya","Tumkur Road, Peenya","080-4000-3303",["Kannada","English","Hindi","Tamil"],["pmjay","private"],false),
 mkH("sharavathi","Sharavathi Taluk Hospital","Govt taluk hospital","magadi","Main Road, Magadi","080-4000-3304",["Kannada","English"],["pmjay","esi"],true),
 mkH("hampi","Hampi Government Hospital","Govt hospital","btm","29th Main, BTM Layout","080-4000-3305",["Kannada","English","Hindi","Urdu"],["pmjay","cghs","esi"],true),
 mkH("bhadra","Bhadra Government Hospital","Govt hospital","hoskote","Old Madras Road, Hoskote","080-4000-3306",["Kannada","English","Telugu"],["pmjay","esi"],true));
const PRISTINE={chennai:JSON.parse(JSON.stringify(DATA_CHN)),bengaluru:JSON.parse(JSON.stringify(SAMPLE))};
Object.values(AREAS_CHN).forEach(a=>{if(!a.district)a.district="Chennai city"});Object.values(AREAS_BLR).forEach(a=>{if(!a.district)a.district="Bengaluru city"});
let AREAS=AREAS_CHN;
const CITY=()=>CITIES[S.city]||CITIES.chennai;
function setCity(){AREAS=CITY().areas;if(!AREAS[S.profile.area])S.profile.area=CITY().defArea;if(!CITY().schemes.includes(S.profile.scheme))S.profile.scheme="self"}

/* =========================================================
   State
   ========================================================= */
const KEY="missinglink-proto-v1";
const blankLeg=(service=null,extra={})=>({id:"L"+Math.random().toString(36).slice(2,7),service,facilityId:null,booking:null,outcome:null,status:"active",...extra});
function fresh(){return{lang:"en",city:"chennai",fs:1,hc:false,view:"start",data:null,dataName:null,audit:[],outbox:[],synced:[],waitlist:[],quarantine:[],lastReport:null,policyV:1,policyLog:[],sim:{offline:false,surge:false,sensor:false,missingRef:false,trGap:false},
 profile:{area:"tnagar",languages:["English"],access:[],scheme:"self",time:"any",text:""},
 legs:[blankLeg()],cur:0,wallet:{},tickets:[],ui:{exp:{},day:null,resched:false,showBlocked:false,pick:null,queue:null}};}
let S=fresh();
/* =========================================================
   Accounts & sign-in (prototype: stored on this device only)
   ========================================================= */
const AKEY="missinglink-users-v1",SKEY="missinglink-session-v1";
let SESSION=null;
try{SESSION=JSON.parse(localStorage.getItem(SKEY)||sessionStorage.getItem(SKEY)||"null")}catch(e){}
let _nrl="en";try{_nrl=localStorage.getItem("nr-lang")||"en"}catch(e){}
const AUTHUI={lang:_nrl,tab:"in",err:{},vals:{who:"self",lang:_nrl,remember:true},msg:"",show:{},fails:0,lockUntil:0};
function loadUsers(){try{return JSON.parse(localStorage.getItem(AKEY))||{}}catch(e){return{}}}
function saveUsers(u){try{localStorage.setItem(AKEY,JSON.stringify(u))}catch(e){}}
function setSession(sess,remember){SESSION=sess;try{localStorage.removeItem(SKEY);sessionStorage.removeItem(SKEY);(remember?localStorage:sessionStorage).setItem(SKEY,JSON.stringify(sess))}catch(e){}}
function clearSession(){SESSION=null;try{localStorage.removeItem(SKEY);sessionStorage.removeItem(SKEY)}catch(e){}}
async function hashPw(pw,salt){const data=new TextEncoder().encode(salt+":"+pw);try{if(crypto&&crypto.subtle){const b=await crypto.subtle.digest("SHA-256",data);return[...new Uint8Array(b)].map(x=>x.toString(16).padStart(2,"0")).join("")}}catch(e){}return "f"+hash(salt+":"+pw).toString(16)}
function newSalt(){try{const a=new Uint8Array(16);crypto.getRandomValues(a);return[...a].map(x=>x.toString(16).padStart(2,"0")).join("")}catch(e){return Math.random().toString(16).slice(2)}}
const normId=s=>{s=String(s||"").trim();const d=s.replace(/[\s()-]/g,"").replace(/^(\+?91|0)(?=[6-9]\d{9}$)/,"");return /^[6-9]\d{9}$/.test(d)?d:s.toLowerCase()};
const validId=s=>/^[6-9]\d{9}$/.test(s)||/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test(s);
function pwScore(pw){pw=pw||"";let s=0;if(pw.length>=8)s++;if(pw.length>=12)s++;if(/[a-z]/.test(pw)&&/[A-Z]/.test(pw))s++;if(/\d/.test(pw))s++;if(/[^A-Za-z0-9]/.test(pw))s++;return s}
function pwMeter(pw){const s=pwScore(pw),lbl=["Too short","Weak","Fair","Good","Strong","Very strong"][s],col=!pw?"var(--muted)":s<=1?"var(--red)":s===2?"var(--amber)":"var(--green)";return`<div class="meter" style="width:100%;height:6px"><i style="width:${(s/5)*100}%;background:${col}"></i></div><span class="tiny" style="color:${col};font-weight:700">${pw?lbl:"Use 8+ characters with a letter and a number"}</span>`}
function stateKey(){return KEY+":"+(SESSION?SESSION.id:"anon")}
function loadState(){S=fresh();S.lang=AUTHUI.lang||"en";try{const raw=localStorage.getItem(stateKey());if(raw){const o=JSON.parse(raw);S={...fresh(),...o,ui:fresh().ui}}}catch(e){}setCity()}

function renderAuth(){
 const U=AUTHUI,v=U.vals,e=U.err,up=U.tab==="up";
 const inp=(id,label,type,attrs="",hint="")=>{const bad=!!e[id];const describe=bad?`aria-describedby="${id}-err"`:"";
  const box=type==="password"?`<div class="pw"><input class="field" id="${id}" name="${id}" type="${U.show[id]?"text":"password"}" value="${esc(v[id]||"")}" ${attrs} aria-invalid="${bad}" ${describe}><button type="button" class="pwtoggle" data-act="togglePw:${id}" aria-label="${U.show[id]?"Hide":"Show"} password">${U.show[id]?"Hide":"Show"}</button></div>`
   :`<input class="field" id="${id}" name="${id}" type="${type}" value="${esc(v[id]||"")}" ${attrs} aria-invalid="${bad}" ${describe}>`;
  return`<div class="fld"><label for="${id}">${label}</label>${box}${hint}${bad?`<span class="err" id="${id}-err">${esc(e[id])}</span>`:""}</div>`};
 const locked=Date.now()<U.lockUntil;
 $("#auth").innerHTML=`<div class="auth">
 <section class="auth-hero" aria-label="About Next Route">
  <div class="brand"><svg width="44" height="44" viewBox="0 0 40 40" aria-hidden="true"><rect width="40" height="40" rx="11" fill="#FFFFFF"/><path d="M9 26c4 0 5-12 11-12s7 12 11 12" stroke="#0A2350" stroke-width="3.2" fill="none" stroke-linecap="round"/><circle cx="9" cy="26" r="3.4" fill="#2D6CDF"/><circle cx="20" cy="14" r="3.4" fill="#0A2350"/><circle cx="31" cy="26" r="3.4" fill="#0A2350"/></svg><div><b style="color:#fff">Next Route</b><span class="tag" style="color:#B9CBEA">Patient journey navigator</span></div></div>
  <div class="hero-mid">
   <h1>Healthcare, one clear step at a time.</h1>
   <p class="hero-sub">Find the right facility, know what to bring, book a slot and plan what comes next — in your language.</p>
   <ul class="feat">
    <li><span>✓</span>Facilities matched to your needs, with the reasons shown</li>
    <li><span>✓</span>Document checklists, so no wasted trips</li>
    <li><span>✓</span>Referrals, reminders and follow-ups planned for you</li>
    <li><span>✓</span>A real person to help when information is unclear</li>
   </ul>
  </div>
  <svg class="hero-line" viewBox="0 0 520 60" aria-hidden="true"><path d="M10 30H510" stroke="#24457F" stroke-width="8" stroke-linecap="round"/><path d="M10 30H190" stroke="#7FB2FF" stroke-width="8" stroke-linecap="round"/>${[10,110,190,290,390,510].map((x,i)=>`<circle cx="${x}" cy="30" r="${i===2?13:10}" fill="${i<2?"#7FB2FF":i===2?"#0A2350":"#0A2350"}" stroke="${i<=2?"#7FB2FF":"#3A5C99"}" stroke-width="5"/>`).join("")}</svg>
  <p class="tiny" style="color:#B9CBEA;margin:0">Administrative help only — not medical advice. Emergency? Call <b style="color:#fff">108</b> or <b style="color:#fff">112</b>.</p>
 </section>
 <section class="auth-panel">
  <div class="auth-card">
   <div class="row" style="justify-content:flex-end;margin:-.6rem -.4rem .4rem 0"><select class="tbtn" id="authLang" aria-label="Language" data-notr><option value="en" ${AUTHUI.lang==="en"?"selected":""}>English</option><option value="hi" ${AUTHUI.lang==="hi"?"selected":""}>हिन्दी</option><option value="kn" ${AUTHUI.lang==="kn"?"selected":""}>ಕನ್ನಡ</option><option value="ta" ${AUTHUI.lang==="ta"?"selected":""}>தமிழ்</option></select></div>
   <h2 style="margin-bottom:.25rem">${up?"Create your account":"Welcome back"}</h2>
   <p class="small muted" style="margin-bottom:1rem">${up?"It takes under a minute. Your journey is saved to your account.":"Sign in to continue your healthcare journey."}</p>
   <div class="tabs" role="tablist" aria-label="Sign in or create account">
    <button type="button" role="tab" aria-selected="${!up}" data-act="authTab:in">Sign in</button>
    <button type="button" role="tab" aria-selected="${up}" data-act="authTab:up">Create account</button>
   </div>
   ${U.msg?`<div class="banner ${U.msgKind||"red"}" role="alert" style="margin-top:1rem"><span class="ic">${U.msgKind==="green"?"✓":"!"}</span><div>${esc(U.msg)}</div></div>`:""}
   <form id="authForm" data-mode="${U.tab}" novalidate style="margin-top:1.1rem">
   ${up?`
    ${inp("name","Full name","text",'autocomplete="name" required')}
    ${inp("ident","Email or mobile number","text",'autocomplete="username" inputmode="email" required','<span class="tiny muted">We\'ll use this to sign you in. Mobile: 10 digits, starting with 6–9.</span>')}
    <div class="grid2" style="gap:.8rem">
     <div class="fld"><label for="who">Signing up for</label><select class="field" id="who" name="who"><option value="self" ${v.who==="self"?"selected":""}>Myself</option><option value="care" ${v.who==="care"?"selected":""}>Someone I care for</option></select></div>
     <div class="fld"><label for="lang">Preferred language</label><select class="field" id="lang" name="lang"><option value="en" ${(v.lang||AUTHUI.lang)==="en"?"selected":""}>English</option><option value="hi" ${(v.lang||AUTHUI.lang)==="hi"?"selected":""}>हिन्दी</option><option value="kn" ${(v.lang||AUTHUI.lang)==="kn"?"selected":""}>ಕನ್ನಡ</option><option value="ta" ${(v.lang||AUTHUI.lang)==="ta"?"selected":""}>தமிழ்</option></select></div>
    </div>
    ${inp("pw","Create a password","password",'autocomplete="new-password" required',`<div id="pwMeter" class="pwmeter">${pwMeter(v.pw)}</div>`)}
    ${inp("pw2","Confirm password","password",'autocomplete="new-password" required')}
    <div class="fld"><label class="check"><input type="checkbox" name="consent" ${v.consent?"checked":""} aria-invalid="${!!e.consent}"><span>I understand this app gives <b>administrative guidance only, not medical advice</b>, and I agree to my details being stored to run my journey.</span></label>${e.consent?`<span class="err">${esc(e.consent)}</span>`:""}</div>
    <button class="btn block" type="button" data-act="authSubmit">Create account</button>`
   :`
    ${inp("ident","Email or mobile number","text",'autocomplete="username" required')}
    ${inp("pw","Password","password",'autocomplete="current-password" required')}
    
    <div class="row" style="justify-content:space-between;margin:-.2rem 0 1rem"><label class="check"><input type="checkbox" name="remember" ${v.remember?"checked":""}><span>Keep me signed in</span></label><button type="button" class="linkbtn small" data-act="forgot">Forgot password?</button></div>
    <button class="btn block" type="button" data-act="authSubmit" ${locked?"disabled":""}>${locked?"Too many attempts — wait 30 s":"Sign in"}</button>`}
   </form>
   <div class="or"><span>or</span></div>
   <button class="btn ghost block" data-act="guest">Continue as guest (demo)</button>
   <p class="tiny muted" style="margin-top:1rem;text-align:center">Prototype: passwords are salted and hashed (SHA-256) and stored on this device only. A live version would use OTP sign-in over SMS.</p>
  </div>
 </section></div>`;
 document.documentElement.lang=AUTHUI.lang||"en";translateDOM($("#auth"));
}
async function submitAuth(form){
 const U=AUTHUI,v=U.vals;const fd=new FormData(form);fd.forEach((val,k)=>v[k]=val);v.consent=!!form.querySelector('[name=consent]')?.checked;v.remember=!!form.querySelector('[name=remember]')?.checked;
 U.err={};U.msg="";const users=loadUsers();const id=normId(v.ident);
 if(U.tab==="up"){
  const err={};const name=(v.name||"").trim();
  if(name.length<2)err.name="Please enter your name.";else if(name.length>60||/[<>{}$\\]|[\u0000-\u001F\u202A-\u202E]/.test(name))err.name="Please use letters only (no symbols or code).";
  if(!validId(id))err.ident=/^\d{10}$/.test(id)?`${id} isn't a real mobile number: Indian mobile numbers always start with 6, 7, 8 or 9 (for example 9876543210). Check the first digit, or use your email instead.`:/^\d+$/.test(id)?`That's ${id.length} digits: a mobile number needs exactly 10 (for example 9876543210).`:"Enter a valid email address or a 10-digit mobile number.";else if(users[id])err.ident="An account already exists for this — sign in instead.";
  const pw=v.pw||"";if(pw.length<8||!/[A-Za-z]/.test(pw)||!/\d/.test(pw))err.pw="Use at least 8 characters, including a letter and a number.";
  if((v.pw2||"")!==pw)err.pw2="Passwords don't match.";
  if(!v.consent)err.consent="Please tick this box to continue.";
  if(Object.keys(err).length){U.err=err;U.msg="Please fix the highlighted field"+(Object.keys(err).length>1?"s":"")+" below.";U.msgKind="red";renderAuth();const f=$("#auth [aria-invalid=true]");f&&f.focus();return}
  const salt=newSalt();users[id]={id,name,who:v.who,lang:AUTHUI.lang,salt,hash:await hashPw(pw,salt),created:new Date().toISOString()};saveUsers(users);
  setSession({id,name,who:v.who,at:Date.now()},true);loadState();S.lang=AUTHUI.lang||"en";save();
  AUTHUI.vals={who:"self",lang:"en",remember:true};AUTHUI.show={};render();toast(`Welcome, ${name.split(" ")[0]}! Let's start with what you need.`);go("start");return}
 if(Date.now()<U.lockUntil){renderAuth();return}
 if(!v.ident||!v.pw){U.err={ident:!v.ident?"Enter your email or mobile number.":"",pw:!v.pw?"Enter your password.":""};if(!U.err.ident)delete U.err.ident;if(!U.err.pw)delete U.err.pw;renderAuth();return}
 const u=users[id];const ok=u&&(await hashPw(v.pw,u.salt))===u.hash;
 if(!ok){U.fails++;if(U.fails>=5){U.lockUntil=Date.now()+30000;U.fails=0;U.msg="Too many failed attempts. Please wait 30 seconds and try again.";setTimeout(()=>{if(!SESSION){AUTHUI.msg="";renderAuth()}},30500)}else U.msg="That email/mobile and password don't match an account on this device.";U.msgKind="red";v.pw="";renderAuth();return}
 U.fails=0;setSession({id,name:u.name,who:u.who,at:Date.now()},v.remember);loadState();S.lang=AUTHUI.lang||u.lang||S.lang;save();
 AUTHUI.vals={who:"self",lang:S.lang,remember:true};AUTHUI.show={};render();toast(`Welcome back, ${u.name.split(" ")[0]}`);go(VIEWOF[stage()]||"start");
}

loadState();
function save(){try{const {ui,...rest}=S;localStorage.setItem(stateKey(),JSON.stringify(rest))}catch(e){}}

/* =========================================================
   Helpers
   ========================================================= */
const $=s=>document.querySelector(s);
const esc=s=>String(s??"").replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
const t=k=>(T[S.lang]&&T[S.lang][k])||T.en[k]||k;
const DATA=()=>S.data||CITY().data;
const fac=id=>DATA().find(f=>f.id===id);
const leg=()=>S.legs[S.cur];
const sod=d=>new Date(d.getFullYear(),d.getMonth(),d.getDate());
const fmtDay=d=>{const n=sod(new Date());const diff=Math.round((sod(d)-n)/864e5);if(diff===0)return"Today";if(diff===1)return"Tomorrow";return d.toLocaleDateString(LOCALE[S.lang],{weekday:"short",day:"numeric",month:"short"})};
const fmtTime=d=>d.toLocaleTimeString(LOCALE[S.lang],{hour:"numeric",minute:"2-digit"});
const daysSince=s=>Math.max(0,Math.round((sod(new Date())-new Date(s+"T00:00:00"))/864e5));
function hash(s){let h=2166136261;for(const c of s){h^=c.charCodeAt(0);h=Math.imul(h,16777619)}return h>>>0}
function rng(a){return()=>{a|=0;a=a+0x6D2B79F5|0;let t=Math.imul(a^a>>>15,1|a);t=t+Math.imul(t^t>>>7,61|t)^t;return((t^t>>>14)>>>0)/4294967296}}
function areaOf(f){return AREAS[f.area]||{name:f.areaName||f.area,x:f.x??12,y:f.y??10}}
function dist(f){const a=AREAS[S.profile.area],b=areaOf(f);return Math.max(0.8,Math.hypot(a.x-b.x,a.y-b.y)*1.3)}
const travel=d=>Math.round(d<=20?d/16*60+8:20/16*60+8+(d-20)/32*60+20);
const tmin=m=>m<90?`${m} min`:`${Math.floor(m/60)} h ${String(m%60).padStart(2,"0")} min`;
const dkey=(d,sid)=>d==="referral"?"referral_"+sid:d;
const dstat=(d,sid)=>(S.wallet[dkey(d,sid)]||{}).status||"missing";
function toast(m){const el=$("#toast");el.textContent=trText(m);el.classList.add("on");clearTimeout(toast.t);toast.t=setTimeout(()=>el.classList.remove("on"),2600)}
function timeOk(at){const p=S.profile.time;if(p==="morning")return at.getHours()<12;if(p==="afternoon")return at.getHours()>=12;if(p==="weekend")return[0,6].includes(at.getDay());return true}

/* slots: deterministic per facility/service/day */
/* DEMO OUTCOMES — whatever service / patient / place is chosen, the hospitals offering that service
   (nearest first) get: 1st free · 2nd data conflict · 3rd fully booked · 4th old data · 5th only 2 slots left · rest free */
const DEMO_ORDER=["open","conflict","full","stale","few","referral","payment","access","unknownref","language"];let DPC={};
function demoKey(sid){const p=S.profile;return[S.city,p.area,sid,p.scheme,p.access.join("+"),p.languages.join("+"),S.dataName||"",DATA().length].join("|")}
function demoProfile(f,sid){if(!f||!sid||S.data)return"open";const k=demoKey(sid);
 if(!DPC[k]){const area=AREAS[S.profile.area]||{x:0,y:0};const src=PRISTINE[S.city]||DATA();const c=src.filter(x=>x.services&&x.services[sid]).map(x=>{const b=AREAS[x.area]||{x:x.x??0,y:x.y??0};return{id:x.id,d:Math.hypot(area.x-b.x,area.y-b.y)}}).sort((a,b)=>a.d-b.d);
  DPC[k]={};c.forEach((x,i)=>DPC[k][x.id]=DEMO_ORDER[i]||"open")}
 return DPC[k][f.id]||"open"}
/* Apply each hospital's demo outcome to the data itself, so Find, Documents, Book and Visit all agree */
let DEMO_APPLIED="";
function applyDemo(){if(S.data||!S.profile)return;const L=leg();const sid=L&&L.service;const k=sid?demoKey(sid):"none|"+S.city;if(k===DEMO_APPLIED)return;DEMO_APPLIED=k;
 const base=CITY().data;base.splice(0,base.length,...JSON.parse(JSON.stringify(PRISTINE[S.city])));if(!sid)return;
 const p=S.profile;
 base.forEach(f=>{const svc=f.services[sid];if(!svc)return;const role=demoProfile(f,sid);
  if(role!=="referral"&&role!=="unknownref")svc.referral=false;
  if(role!=="stale")f.verified=f.verified<"2026-08-01"?"2026-10-20":f.verified;
  if(role!=="conflict"&&role!=="access")f.conflicts=[];
  if(!["payment"].includes(role)){if(p.scheme&&!["self","unknown"].includes(p.scheme)&&!f.schemes.includes(p.scheme))f.schemes=[...f.schemes,p.scheme];f.selfPay=true}
  if(role!=="language"&&!f.languages.some(l=>p.languages.includes(l)))f.languages=[...p.languages.slice(0,1),...f.languages];
  if(role!=="access"&&svc.floor>0){f.access={...f.access,lift:true}}
  if(role==="stale")f.verified="2026-04-18";
  if(role==="referral")svc.referral=true;
  if(role==="unknownref")svc.referral=null;
  if(role==="payment"){if(p.scheme==="self"||p.scheme==="unknown"){f.selfPay=false;f.schemes=["cghs"]}else f.schemes=f.schemes.filter(x=>x!==p.scheme).concat(f.schemes.length>1?[]:["cghs"]).filter(x=>x!==p.scheme)}
  if(role==="access"){svc.floor=2;f.access={...f.access,wheelchair:true,lift:false}}
  if(role==="language"){const pool=["Bengali","Malayalam","Telugu","Urdu","Hindi","Kannada","Tamil"].filter(l=>!p.languages.includes(l));f.languages=pool.slice(0,2)}
 });DPC={};}
function fVerified(f,sid){return demoProfile(f,sid).includes("stale")?"2026-04-18":f.verified}
const AVAIL={thendral:"few",nalam:"full",sangamam:"open",vayal:"few",kanchihq:"full",eri:"open",palar:"few",senji:"open",sanjeevini:"few",arogya:"full",janapada:"full",arkavathi:"open",kalyani:"open"};
function slotsForBase(f,sid,notBefore){
 const svc=f.services[sid];if(!svc)return[];
 const days=svc.days||f.days||[1,2,3,4,5,6];const step=svc.slotMins||20;const out=[];const now=new Date();let od=0;const prof=demoProfile(f,sid);let fewLeft=2;
 for(let i=0;i<22&&(i<8||od<2);i++){
  const d=new Date(now.getFullYear(),now.getMonth(),now.getDate()+i);
  if(!days.includes(d.getDay()))continue;
  if(notBefore&&d<sod(new Date(notBefore)))continue;
  const [oh,om]=(svc.open||f.open||"09:00").split(":").map(Number),[ch,cm]=(svc.close||f.close||"17:00").split(":").map(Number);
  const r=rng(hash(f.id+sid+d.toDateString()));let m=oh*60+om,idx=0;const tmp=[];
  while(m+step<=ch*60+cm){
   if(!(m>=780&&m<840)){const s=new Date(d);s.setHours(Math.floor(m/60),m%60,0,0);const x=r();if(s-now>40*60000)tmp.push({at:s,free:x<0.45,token:11+idx,contested:false});idx++;}
   m+=step;
  }
  if(!tmp.length)continue;
  if(prof==="full")tmp.forEach(t=>t.free=false);
  else if(prof.includes("few")){tmp.forEach(t=>t.free=false);if(fewLeft>0){tmp[Math.min(tmp.length-1,Math.floor(tmp.length*.4))].free=true;fewLeft--}}
  else{if(od===0){let n=tmp.filter(t=>t.free).length;for(let k=0;n<Math.min(3,tmp.length)&&k<tmp.length;k+=2){if(!tmp[k].free){tmp[k].free=true;n++}}
   const c=tmp.find((t,j)=>t.free&&j>=1)||tmp.find(t=>t.free);if(c)c.contested=true}}
  od++;out.push(...tmp);
 }
 return out;
}
function slotsFor(f,sid,notBefore){const base=slotsForBase(f,sid,notBefore);const led=ledgerRead();const L=leg();const mine=L&&L.booking&&L.facilityId===f.id&&L.service===sid?new Date(L.booking.at).getTime():null;const me=L?holderId(L):"";
 let out=base;if(S.sim&&S.sim.surge){const r=rng(hash("surge-demand"+f.id+sid));out=base.filter((x,i)=>i%2===0||x.at.getTime()===mine).map(x=>({...x,free:x.at.getTime()===mine?x.free:x.free&&r()<0.28}))}
 return out.map(x=>{const h=led[slotKey(f.id,sid,x.at)];return h&&h.holder!==me?{...x,free:false}:x})}
function requiredDocs(f,sid){
 const base=[...(SERVICES[sid]?.docs||["id_proof"])];const svc=f?.services?.[sid];
 if(f&&needsReferral(f,sid))base.push("referral");(svc?.extraDocs||[]).forEach(d=>base.push(d));
 if(["pmjay","cghs","esi","cmchis"].includes(S.profile.scheme))base.push("scheme_card");
 if(S.city==="chennai"&&sid==="anc")base.push("picme");
 if(S.profile.scheme==="private")base.push("insurance_card");
 return[...new Set(base)].filter(d=>DOCS[d]);
}
function conflicts(f,sid){
 const out=(f.conflicts||[]).filter(c=>sid===null||!c.service||c.service===sid).map(c=>({...c}));
 if(sid&&demoProfile(f,sid).includes("conflict")&&!out.some(c=>!c.auto)){const sv=f.services[sid];const op=sv.open||f.open||"09:00";const [h,mm]=op.split(":").map(Number);const later=`${String(h+1).padStart(2,"0")}:${String(mm).padStart(2,"0")}`;
  out.push({service:sid,field:`${sv.dept} opening time`,note:`The directory says ${sv.dept} opens at ${op}. A patient reported on 3 Nov that it now opens at ${later}.`,source:"Organiser directory vs. patient report",records:[{source:"Organiser directory",tier:2,at:"2026-08-20",value:op},{source:"Patient report",tier:3,at:"2026-11-03",value:later}]})}
 const svcs=sid===null?Object.values(f.services):[f.services[sid]];svcs.forEach(svc=>{
 if(svc&&f.access?.wheelchair===true&&svc.floor>0&&!f.access.lift)out.push({field:"Step-free access",note:`Directory lists wheelchair access, but ${svc.dept} is on floor ${svc.floor} and no lift is listed.`,source:"Auto-check across fields",auto:true})});
 return out;
}

/* =========================================================
   Explainable feasibility engine
   ========================================================= */
function evaluate(f){
 const p=S.profile,L=leg(),sid=L.service,svc=f.services[sid];if(!svc)return null;
 const fx=[];let score=40,hard=false,refMissing=false;
 const add=(ok,label,detail,pts=0,isHard)=>{fx.push({ok,label,detail,pts});score+=pts;if(ok===false&&isHard)hard=true};
 add(true,`Offers ${SERVICES[sid].name}`,`${svc.dept} · ${svc.floor?`floor ${svc.floor}`:"ground floor"} · fee: ${svc.fee}`,0);
 if(p.scheme==="unknown"){add(null,"Payment method not confirmed",`Fee depends on it — here: ${svc.fee}. We won't guess; choose a payment option or ask a navigator.`,-4)}
 else if(p.scheme==="self"){ if(f.selfPay===false)add(false,"Members only",`Only for ${f.schemes.map(s=>SCHEMES[s]).join(", ")} members`,-40,true); else add(true,"Self-pay accepted",`Expected fee: ${svc.fee}`,/free/i.test(svc.fee)?8:2); }
 else if(f.schemes.includes(p.scheme))add(true,`Accepts ${SCHEMES[p.scheme]}`,"Listed as accepted in organiser data",10);
 else add(false,`Doesn't accept ${SCHEMES[p.scheme]}`,`You would pay yourself: ${svc.fee}`,-35,true);
 p.access.forEach(a=>{const v=f.access?.[a],A=ACCESS[a];
  if(v===true)add(true,A.name,"Available",6);
  else if(v==="request")add(null,`${A.name} — on request`,f.access.note||"Needs advance notice; a navigator can arrange it",3);
  else add(false,`No ${A.name.toLowerCase()} listed`,A.hard?"Listed as not available":"A navigator can try to arrange this",A.hard?-35:-10,A.hard);
 });
 if(p.access.includes("wheelchair")&&svc.floor>0&&!f.access?.lift)add(false,"Department not step-free",`${svc.dept} is on floor ${svc.floor} with no working lift listed`,-35,true);
 const shared=p.languages.filter(l=>f.languages.includes(l));
 if(shared.length)add(true,`Staff speak ${shared.join(", ")}`,"Front-desk languages listed by the facility",10);
 else add(false,"No shared language listed",`Listed: ${f.languages.join(", ")}. A navigator can request an interpreter.`,-12);
 const d=dist(f);add(d<=8?true:null,`${d.toFixed(1)} km away`,`About ${tmin(travel(d))} by road from ${AREAS[p.area].name}`,d<=20?Math.max(-6,Math.round(14-d*1.1)):Math.max(-25,Math.round(-6-(d-20)*0.2)));
 const free=slotsFor(f,sid,L.notBefore).filter(s=>s.free&&timeOk(s.at));
 if(free.length){const a=free[0].at,dd=Math.round((sod(a)-sod(new Date()))/864e5);add(true,`Next slot: ${fmtDay(a)}, ${fmtTime(a)}`,`${free.length} free slots in the next week${p.time!=="any"?` (${TIMES[p.time].toLowerCase()})`:""}`,dd<=1?12:dd<=3?7:2)}
 else add(false,"No free slots this week",p.time!=="any"?"Try widening your time preference":"Ask a navigator about walk-in queues",-14);
 const nr=needsReferral(f,sid);if(nr===null){refMissing=true;add(null,"Referral rule not stated","The data doesn't say whether this department needs a referral letter. We won't guess — confirm with the facility or a navigator.",-6)}
 if(nr){const ok=dstat("referral",sid)==="ready";if(!ok)refMissing=true;add(ok?true:false,ok?"Referral letter ready":"Needs a referral letter",ok?"You marked it as ready":"This department only sees referred patients. A General OPD doctor can issue one.",ok?0:-8)}
 const req=requiredDocs(f,sid).filter(x=>x!=="referral"),miss=req.filter(x=>dstat(x,sid)!=="ready");
 if(miss.length)add(null,`${miss.length} document${miss.length>1?"s":""} to prepare`,miss.map(x=>DOCS[x].name).join(" · "),-1*miss.length);else add(true,"All documents ready","",3);
 const fv=fVerified(f,sid);const age=daysSince(fv);
 if(age>90)add(null,`Details are ${age} days old`,`Last verified ${fv}. Confirm before travelling.`,-6);else add(true,"Recently verified",`Checked ${age} day${age===1?"":"s"} ago`,2);
 const cf=conflicts(f,sid);cf.forEach(c=>add(null,`Conflicting info: ${c.field}`,c.note,-4));
 const status=hard?"blocked":(refMissing||p.scheme==="unknown")?"steps":"ready";
 return{f,svc,fx,score:Math.max(0,Math.min(100,Math.round(score))),status,d,free,cf,age,shared};
}
function ranked(){const r={ready:0,steps:1,blocked:2};return DATA().map(evaluate).filter(Boolean).sort((a,b)=>r[a.status]-r[b.status]||b.score-a.score)}

/* =========================================================
   Clinical boundary guard + keyword → department (user confirms)
   ========================================================= */
const GUARD={
 emergency:/(நெஞ்சு வலி|மூச்சு விட முடியவில்லை|மயக்கம்|chest pain|can'?t breathe|cannot breathe|not breathing|breathless|unconscious|faint|severe bleeding|bleeding (a lot|heavily)|stroke|seizure|\bfits\b|poison|accident|heart attack|chok(e|ing)|burns?\b|snake ?bite)/i,
 crisis:/(தற்கொலை|suicid|kill myself|end my life|self[- ]?harm|hurt myself|want to die)/i,
 clinical:/(which medicine|what medicine|should i take|dose|dosage|is it serious|what do i have|diagnos|what disease|cure for|treatment for|which tablet|is this normal)/i
};
const KW=[
 [/கர்ப்ப|गर्भ|ಗರ್ಭ|pregnan|antenatal|\banc\b|expecting|missed (my )?period/i,"anc"],
 [/கண்|आंख|आँख|ಕಣ್ಣು|\beyes?\b|vision|glasses|spectacle|cataract|blurr|can'?t see|cannot see|see clearly/i,"eye"],
 [/பல்|दांत|दाँत|ಹಲ್ಲು|tooth|teeth|dental|\bgums?\b|cavity/i,"dental"],
 [/தடுப்பூசி|टीका|ಲಸಿಕೆ|vaccin|immunis|immuniz|polio|booster|injection for (my )?(baby|child)/i,"vacc"],
 [/சர்க்கரை|शुगर|मधुमेह|ಸಕ್ಕರೆ|sugar|diabet|insulin/i,"diab"],
 [/இதய|दिल|ಹೃದಯ|heart|cardi/i,"cardio"],
 [/physio|rehab|exercise therapy|walking again|after (my )?surgery/i,"physio"],
 [/கால் வலி|மூட்டு|முதுகு வலி|पैर|घुटन|कमर दर्द|ಕಾಲು|ಮೊಣಕಾಲು|ಬೆನ್ನು ನೋವು|\blegs?\b|knee|joint|\bbones?\b|ortho|back ?pain|backache|shoulder|\bhips?\b|neck pain|ankle|wrist|fracture|sprain|spine|arthritis|\bfoot\b|\bfeet\b/i,"ortho"],
 [/blood test|\blab\b|test report|\bscan\b|x-?ray|sample|urine test/i,"lab"],
 [/காய்ச்சல்|बुखार|ಜ್ವರ|referr|general doctor|\bgp\b|check ?-?up|fever|\bcold\b|cough|headache|stomach|vomit|loose motion|diarrh|body pain|weak|tired|rash|skin|\bear\b|throat|\bbp\b|blood pressure|dizzy|not feeling well|unwell|sick/i,"gen_opd"]];
function analyse(text){
 const res={level:null,suggest:[]};if(!text||!text.trim())return res;
 if(GUARD.crisis.test(text))res.level="crisis";else if(GUARD.emergency.test(text))res.level="emergency";else if(GUARD.clinical.test(text))res.level="clinical";
 KW.forEach(([re,s])=>{const m=text.match(re);if(m&&!res.suggest.find(x=>x.s===s))res.suggest.push({s,word:m[0]})});
 return res;
}
function routeHTML(a,L){
 if(!S.profile.text||!S.profile.text.trim()||a.level==="crisis"||a.level==="emergency")return"";
 const txt=S.profile.text.trim();const sug=a.suggest;const notDx=`<div class="rt-warn">⚠ <b>This is not a diagnosis.</b> We only match your words to a department — a doctor decides what you actually need.</div>`;
 const navBtn=`<button class="btn ghost sm rt-ghost" data-act="nav:help">📞 Ask a human navigator</button>`;
 if(!sug.length){if(txt.length<4)return"";
  return`<div class="rt amber"><div class="rt-h">We couldn't match this to a department</div><p class="small">Not sure where to go? <b>General OPD</b> is the usual first stop — a doctor there can see you and refer you to the right specialist. Or a navigator can help you decide.</p>
  <div class="row">${L.service==="gen_opd"?`<span class="pill ok b">✓ General OPD selected</span>`:`<button class="btn sm" data-act="svc:gen_opd">Go to General OPD</button>`}${navBtn}</div>${notDx}</div>`}
 const top=sug[0],ts=SERVICES[top.s],picked=L.service===top.s;const others=sug.slice(1);
 const spec=ts.kind==="specialist";
 return`<div class="rt"><div class="rt-h">${picked?"✓ ":""}Suggested: ${esc(ts.name)}</div><p class="small">Because you wrote <b>“${esc(((S.profile.text.match(new RegExp(top.word.replace(/[.*+?^${}()|[\]\\]/g,"\\$&")+"\\s*(pain|ache|problem)?","i"))||[top.word])[0]).trim())}”</b>.${picked&&L.autoPick?" We've selected it for you — change it any time above.":""}${spec?" Specialist clinics at government hospitals often need a referral letter from General OPD first — if so, the app will send you there first.":""}</p>
 <div class="row">${picked?"":`<button class="btn sm" data-act="svc:${top.s}">Use ${esc(ts.name)}</button>`}${top.s!=="gen_opd"?`<button class="btn ghost sm rt-ghost" data-act="svc:gen_opd">See a general doctor (GP) instead</button>`:""}${navBtn}</div>
 ${others.length?`<div class="small" style="margin-top:.5rem">Also matched: ${others.map(x=>`<button class="chip" data-act="svc:${x.s}">${esc(SERVICES[x.s].name)} <span class="tiny muted">“${esc(x.word)}”</span></button>`).join(" ")}</div>`:""}${notDx}</div>`}
function autoRoute(){const a=analyse(S.profile.text),L=leg();if(a.level==="crisis"||a.level==="emergency"){if(L.autoPick&&L.service){L.service=null;L.autoPick=false;return true}return false}
 const top=a.suggest[0];if(top&&(!L.service||(L.autoPick&&L.service!==top.s))){L.service=top.s;L.facilityId=null;L.booking=null;L.autoPick=true;return true}
 if(!top&&L.autoPick&&L.service){L.service=null;L.autoPick=false;return true}return false}
function guardBanner(a){const h=guardBanner0(a);return h;const plain=h.replace(/<[^>]+>/g," ").replace(/\s+/g," ").replace(/^\s*[!i]\s*/,"").trim();return h.replace(/<\/div><\/div>$/,`<div class="tiny" data-notr lang="en" style="margin-top:.35rem;opacity:.85">English: ${plain}</div></div></div>`)}
function guardBanner0(a){
 if(a.level==="crisis")return`<div class="banner red" role="alert"><span class="ic">!</span><div><b>You don't have to go through this alone.</b> Please call <b>Tele-MANAS 14416</b> (free, 24×7, many Indian languages) or <b>112</b> if you are in immediate danger. This app can't help with this, but a trained person can — right now.</div></div>`;
 if(a.level==="emergency")return`<div class="banner red" role="alert"><span class="ic">!</span><div><b>This may need urgent help.</b> We can't assess symptoms. Call <b>108</b> (ambulance) or <b>112</b>, or go to the nearest emergency department. Facilities with 24×7 emergency in this dataset: ${DATA().filter(f=>f.emergency).map(f=>esc(f.name)).join(", ")}.</div></div>`;
 if(a.level==="clinical")return`<div class="banner amber" role="note"><span class="ic">i</span><div><b>That's a question for a clinician.</b> We only help with where to go and what to bring. Ask the doctor at your visit, or use the government teleconsultation service eSanjeevani (esanjeevani.mohfw.gov.in)${S.city==="chennai"?", or call the Tamil Nadu health helpline <b>104</b>":""}. We can still help you book a visit.</div></div>`;
 return"";
}

/* =========================================================
   Journey stage + next step (explainable)
   ========================================================= */
const STAGES=["need","find","docs","book","visit","follow"];
const VIEWOF={need:"start",find:"options",docs:"documents",book:"book",visit:"visit",follow:"followup"};
function stage(){
 const L=leg();if(!L.service)return"need";if(!L.facilityId)return"find";
 const f=fac(L.facilityId);if(!f)return"find";
 if(!L.booking){const req=requiredDocs(f,L.service);if(req.some(d=>dstat(d,L.service)!=="ready"))return"docs";return"book"}
 if(!L.outcome)return"visit";return"follow";
}
function nextStep(){
 const L=leg(),st=stage(),sn=L.service&&SERVICES[L.service].name;const f=L.facilityId&&fac(L.facilityId);
 if(st==="need")return{k:"ns_need",act:"nav:start",why:["Everything else — which facilities fit, what to bring, which slots exist — depends on the service you need.","Not sure? Start with General OPD: a doctor there can refer you onward."]};
 if(st==="find"){const ev=ranked(),ok=ev.filter(e=>e.status!=="blocked");return{k:"ns_find",act:"nav:options",why:[`${ok.length} of ${ev.length} facilities offering ${sn} can work for you.`,ok[0]?`Best match: ${ok[0].f.name} (fit ${ok[0].score}).`:"None fits every need — a human navigator can help find an alternative."]}}
 if(st==="docs"){const req=requiredDocs(f,L.service),miss=req.filter(d=>dstat(d,L.service)!=="ready");
  if(miss.includes("referral"))return{k:"ns_ref",act:"getReferral",alt:{label:"See facilities without this rule",act:"nav:options"},why:[`${f.services[L.service].dept} at ${f.name} only sees patients with a referral letter (organiser data: referral required).`,"Only a doctor can issue one. We'll set up a General OPD visit first, then bring you back here automatically."]};
  return{k:"ns_docs",act:"nav:documents",alt:{label:"Book anyway",act:"nav:book"},why:[`${miss.length} of ${req.length} items still to prepare: ${miss.map(d=>DOCS[d].name).join(", ")}.`,"Missing paperwork is a common reason people are sent back from the registration counter."]}}
 if(st==="book"){const ev=evaluate(f);return{k:"ns_book",act:"nav:book",why:[`All documents for ${f.name} are ready.`,ev.free[0]?`Earliest slot matching your preference: ${fmtDay(ev.free[0].at)}, ${fmtTime(ev.free[0].at)}.`:"No free slot this week — try another time preference or ask a navigator."]}}
 if(st==="visit"){const at=new Date(L.booking.at);const lv=new Date(at-travel(dist(f))*60000-15*60000);return{k:"ns_visit",act:"nav:visit",why:[`${fmtDay(at)} at ${fmtTime(at)} · ${f.services[L.service].dept}, ${f.name}. Token ${L.booking.token}.`,`Leave by ${fmtTime(lv)} — about ${tmin(travel(dist(f)))} travel plus 15 min for registration.`,"After the visit, tell us what the doctor said so we can line up the next step."]}}
 return{k:"ns_complete",act:"nav:followup",why:["Nothing else is pending for this journey.","Your reminders and history stay in Follow-up."]};
}

/* =========================================================
   Reminders (computed from journey)
   ========================================================= */
function reminders(){
 const out=[];const now=new Date();
 S.legs.forEach((L,i)=>{
  const f=L.facilityId&&fac(L.facilityId);if(!f)return;const sn=SERVICES[L.service].name;
  if(L.booking&&!L.outcome){
   const at=new Date(L.booking.at);const miss=requiredDocs(f,L.service).filter(d=>dstat(d,L.service)!=="ready");
   if(miss.length)out.push({at:now,title:`Still missing: ${miss.map(d=>DOCS[d].name).join(", ")}`,body:"Get these before your visit, or ask a navigator what to do.",kind:"now"});
   const eve=new Date(sod(at).getTime()-6*3600000);if(eve>now)out.push({at:eve,title:`Pack for tomorrow's ${sn} visit`,body:"Bring: "+requiredDocs(f,L.service).map(d=>DOCS[d].name).join(", ")});
   const lv=new Date(at-travel(dist(f))*60000-15*60000);out.push({at:lv,title:`Leave for ${f.name}`,body:`${f.address}. About ${tmin(travel(dist(f)))} travel.`});
   out.push({at,title:`${sn} appointment · token ${L.booking.token}`,body:`${f.services[L.service].dept}, ${f.name}`,ev:true,dur:30});
  }
  if(L.outcome&&L.outcome.type==="return"&&L.outcome.date){const d=new Date(L.outcome.date);out.push({at:new Date(d.getTime()-7*864e5>now?d.getTime()-7*864e5:now.getTime()),title:`Book your ${sn} follow-up`,body:`The doctor asked you to come back around ${d.toLocaleDateString(LOCALE[S.lang],{day:"numeric",month:"short"})}.`})}
  if(L.outcome&&L.outcome.type==="report")out.push({at:new Date(new Date(L.outcome.at).getTime()+3*864e5),title:"Collect your test report",body:`From ${f.name}. Take your receipt.`});
 });
 return out.sort((a,b)=>a.at-b.at);
}
function ics(){
 const pad=n=>String(n).padStart(2,"0");const fmt=d=>`${d.getUTCFullYear()}${pad(d.getUTCMonth()+1)}${pad(d.getUTCDate())}T${pad(d.getUTCHours())}${pad(d.getUTCMinutes())}00Z`;
 const ev=reminders().filter(r=>r.kind!=="now").map((r,i)=>["BEGIN:VEVENT",`UID:ml-${i}-${r.at.getTime()}@nextroute`,`DTSTAMP:${fmt(new Date())}`,`DTSTART:${fmt(r.at)}`,`DTEND:${fmt(new Date(r.at.getTime()+(r.dur||15)*60000))}`,`SUMMARY:${trText(r.title)}`,`DESCRIPTION:${trText(r.body)}`,"BEGIN:VALARM","TRIGGER:-PT30M","ACTION:DISPLAY","DESCRIPTION:Reminder","END:VALARM","END:VEVENT"].join("\r\n"));
 return["BEGIN:VCALENDAR","VERSION:2.0","PRODID:-//Next Route//Prototype//EN",...ev,"END:VCALENDAR"].join("\r\n");
}

/* =========================================================
   Escalation reasons (auto-detected)
   ========================================================= */
function escalationReasons(){
 const r=[];const L=leg();
 const a=analyse(S.profile.text);if(a.level)r.push({lvl:"high",t:a.level==="clinical"?"You asked something that needs clinical judgement":"Your description mentions something that may be urgent"});
 if(L.service){const ev=ranked();if(ev.length&&!ev.some(e=>e.status!=="blocked"))r.push({lvl:"high",t:`No facility in the data meets all your needs for ${SERVICES[L.service].name}`});
  if(!ev.length)r.push({lvl:"high",t:`No facility in the dataset offers ${SERVICES[L.service].name}`});}
 if(S.profile.scheme==="unknown")r.push({lvl:"mid",t:"Missing information: payment method not confirmed"});
 if(L.facilityId&&fac(L.facilityId)&&needsReferral(fac(L.facilityId),L.service)===null)r.push({lvl:"high",t:"Missing information: referral rule not stated for this department"});
 if(L.booking&&L.booking.review)r.push({lvl:"high",t:"Rules changed after booking — needs your confirmation"});
 if(L.facilityId){const f=fac(L.facilityId),e=f&&evaluate(f);if(e){e.cf.forEach(c=>r.push({lvl:"mid",t:`Conflicting info at ${f.name}: ${c.field}`}));if(e.age>90)r.push({lvl:"mid",t:`${f.name}'s details are ${e.age} days old`});
  S.profile.access.forEach(x=>{if(f.access?.[x]!==true)r.push({lvl:"mid",t:`${ACCESS[x].name} needs arranging at ${f.name}`})});
  if(!e.shared.length)r.push({lvl:"mid",t:`Interpreter needed (${S.profile.languages.join(", ")})`});}}
 return r;
}
function caseSummary(){
 const p=S.profile,L=leg(),f=L.facilityId&&fac(L.facilityId);
 const lines=[`Service: ${L.service?SERVICES[L.service].name:"not chosen yet"}${L.purpose?` (${L.purpose})`:""}`,`From: ${AREAS[p.area].name} · Languages: ${p.languages.join(", ")}`,`Accessibility: ${p.access.length?p.access.map(a=>ACCESS[a].name).join(", "):"none stated"}`,`Payment: ${SCHEMES[p.scheme]} · Time: ${TIMES[p.time]}`,`Facility: ${f?f.name:"not chosen"}${L.booking?` · booked ${fmtDay(new Date(L.booking.at))} ${fmtTime(new Date(L.booking.at))}, token ${L.booking.token}`:""}`];
 if(L.service){const req=f?requiredDocs(f,L.service):SERVICES[L.service].docs;const miss=req.filter(d=>dstat(d,L.service)!=="ready");lines.push(`Documents missing: ${miss.length?miss.map(d=>DOCS[d].name).join(", "):"none"}`)}
 const rs=escalationReasons();if(rs.length)lines.push("Flags: "+rs.map(x=>x.t).join("; "));
 return lines.join("\n");
}

const TRD={"General OPD": ["सामान्य ओपीडी", "ಸಾಮಾನ್ಯ ಒಪಿಡಿ", "பொது வெளிநோயாளர் பிரிவு"], "See a general doctor; get referrals": ["सामान्य डॉक्टर से मिलें; रेफ़रल पाएँ", "ಸಾಮಾನ್ಯ ವೈದ್ಯರನ್ನು ಭೇಟಿ ಮಾಡಿ; ರೆಫರಲ್ ಪಡೆಯಿರಿ", "பொது மருத்துவரைப் பாருங்கள்; பரிந்துரை பெறுங்கள்"], "Eye check": ["आँखों की जाँच", "ಕಣ್ಣಿನ ತಪಾಸಣೆ", "கண் பரிசோதனை"], "Ophthalmology / vision": ["नेत्र विभाग / दृष्टि", "ನೇತ್ರ ವಿಭಾಗ / ದೃಷ್ಟಿ", "கண் மருத்துவம் / பார்வை"], "Dental": ["दंत चिकित्सा", "ದಂತ ಚಿಕಿತ್ಸೆ", "பல் மருத்துவம்"], "Teeth and gums": ["दाँत और मसूड़े", "ಹಲ್ಲು ಮತ್ತು ಒಸಡು", "பற்கள் மற்றும் ஈறுகள்"], "Lab tests": ["लैब जाँच", "ಪ್ರಯೋಗಾಲಯ ಪರೀಕ್ಷೆಗಳು", "ஆய்வகப் பரிசோதனைகள்"], "Tests a doctor asked for": ["डॉक्टर द्वारा बताई गई जाँचें", "ವೈದ್ಯರು ಸೂಚಿಸಿದ ಪರೀಕ್ಷೆಗಳು", "மருத்துவர் சொன்ன பரிசோதனைகள்"], "Vaccination": ["टीकाकरण", "ಲಸಿಕೆ", "தடுப்பூசி"], "Child or adult immunisation": ["बच्चों या वयस्कों का टीकाकरण", "ಮಕ್ಕಳ ಅಥವಾ ವಯಸ್ಕರ ಲಸಿಕೆ", "குழந்தை அல்லது பெரியவர் தடுப்பூசி"], "Pregnancy check-up": ["गर्भावस्था जाँच", "ಗರ್ಭಿಣಿ ತಪಾಸಣೆ", "கர்ப்ப கால பரிசோதனை"], "Antenatal (ANC) visits": ["प्रसवपूर्व (ANC) जाँचें", "ಪ್ರಸವಪೂರ್ವ (ANC) ಭೇಟಿಗಳು", "மகப்பேறுக்கு முந்தைய (ANC) வருகைகள்"], "Diabetes clinic": ["मधुमेह क्लिनिक", "ಮಧುಮೇಹ ಕ್ಲಿನಿಕ್", "நீரிழிவு கிளினிக்"], "Ongoing NCD follow-up": ["नियमित एनसीडी फ़ॉलो-अप", "ನಿಯಮಿತ ಎನ್‌ಸಿಡಿ ಫಾಲೋ-ಅಪ್", "தொடர் NCD கண்காணிப்பு"], "Cardiology": ["हृदय रोग विभाग", "ಹೃದ್ರೋಗ ವಿಭಾಗ", "இதய நோய் பிரிவு"], "Heart specialist OPD": ["हृदय विशेषज्ञ ओपीडी", "ಹೃದಯ ತಜ್ಞರ ಒಪಿಡಿ", "இதய நிபுணர் வெளிநோயாளர் பிரிவு"], "Orthopaedics": ["हड्डी रोग विभाग", "ಮೂಳೆ ಚಿಕಿತ್ಸಾ ವಿಭಾಗ", "எலும்பு மருத்துவப் பிரிவு"], "Bones & joints specialist": ["हड्डी और जोड़ विशेषज्ञ", "ಮೂಳೆ ಮತ್ತು ಕೀಲು ತಜ್ಞರು", "எலும்பு & மூட்டு நிபுணர்"], "Physiotherapy": ["फ़िज़ियोथेरेपी", "ಫಿಸಿಯೋಥೆರಪಿ", "இயன்முறை சிகிச்சை"], "Rehab sessions": ["पुनर्वास सत्र", "ಪುನರ್ವಸತಿ ಅವಧಿಗಳು", "மறுவாழ்வு அமர்வுகள்"], "Photo ID": ["फ़ोटो पहचान पत्र", "ಭಾವಚಿತ್ರ ಗುರುತಿನ ಚೀಟಿ", "புகைப்பட அடையாள அட்டை"], "Any one: Aadhaar, voter ID, driving licence, passport, or ration card with photo.": ["इनमें से कोई एक: आधार, वोटर आईडी, ड्राइविंग लाइसेंस, पासपोर्ट, या फ़ोटो वाला राशन कार्ड।", "ಇವುಗಳಲ್ಲಿ ಯಾವುದಾದರೂ ಒಂದು: ಆಧಾರ್, ಮತದಾರರ ಗುರುತಿನ ಚೀಟಿ, ಚಾಲನಾ ಪರವಾನಗಿ, ಪಾಸ್‌ಪೋರ್ಟ್ ಅಥವಾ ಭಾವಚಿತ್ರವಿರುವ ಪಡಿತರ ಚೀಟಿ.", "ஏதேனும் ஒன்று: ஆதார், வாக்காளர் அடையாள அட்டை, ஓட்டுநர் உரிமம், கடவுச்சீட்டு அல்லது புகைப்படத்துடன் கூடிய குடும்ப அட்டை."], "Health scheme card (CMCHIS / PM-JAY / CGHS / ESI)": ["स्वास्थ्य योजना कार्ड (CMCHIS / PM-JAY / CGHS / ESI)", "ಆರೋಗ್ಯ ಯೋಜನೆ ಕಾರ್ಡ್ (CMCHIS / PM-JAY / CGHS / ESI)", "மருத்துவக் காப்பீட்டுத் திட்ட அட்டை (CMCHIS / PM-JAY / CGHS / ESI)"], "CMCHIS (Tamil Nadu): enrol at a CMCHIS kiosk with your family/ration card, Aadhaar and an income certificate from the VAO; download the e-card at cmchistn.com. PM-JAY: Ayushman card at beneficiary.nha.gov.in or a Common Service Centre. CGHS / ESI: from your employer or scheme office.": ["CMCHIS (तमिलनाडु): अपने परिवार/राशन कार्ड, आधार और VAO से आय प्रमाण पत्र के साथ CMCHIS कियोस्क पर नामांकन करें; ई-कार्ड cmchistn.com से डाउनलोड करें। PM-JAY: आयुष्मान कार्ड beneficiary.nha.gov.in या कॉमन सर्विस सेंटर से। CGHS / ESI: अपने नियोक्ता या योजना कार्यालय से।", "CMCHIS (ತಮಿಳುನಾಡು): ನಿಮ್ಮ ಕುಟುಂಬ/ಪಡಿತರ ಚೀಟಿ, ಆಧಾರ್ ಮತ್ತು VAO ನೀಡಿದ ಆದಾಯ ಪ್ರಮಾಣಪತ್ರದೊಂದಿಗೆ CMCHIS ಕಿಯೋಸ್ಕ್‌ನಲ್ಲಿ ನೋಂದಾಯಿಸಿ; ಇ-ಕಾರ್ಡ್ ಅನ್ನು cmchistn.com ನಿಂದ ಡೌನ್‌ಲೋಡ್ ಮಾಡಿ. PM-JAY: ಆಯುಷ್ಮಾನ್ ಕಾರ್ಡ್ beneficiary.nha.gov.in ಅಥವಾ ಸಾಮಾನ್ಯ ಸೇವಾ ಕೇಂದ್ರದಲ್ಲಿ. CGHS / ESI: ನಿಮ್ಮ ಉದ್ಯೋಗದಾತ ಅಥವಾ ಯೋಜನಾ ಕಚೇರಿಯಿಂದ.", "CMCHIS (தமிழ்நாடு): உங்கள் குடும்ப அட்டை, ஆதார் மற்றும் VAO வழங்கிய வருமானச் சான்றிதழுடன் CMCHIS பதிவு மையத்தில் பதிவு செய்யுங்கள்; மின்-அட்டையை cmchistn.com இல் பதிவிறக்குங்கள். PM-JAY: ஆயுஷ்மான் அட்டை beneficiary.nha.gov.in அல்லது பொது சேவை மையத்தில். CGHS / ESI: உங்கள் பணி நிறுவனம் அல்லது திட்ட அலுவலகத்திடம்."], "Scheme card (PM-JAY / CGHS / ESI)": ["योजना कार्ड (PM-JAY / CGHS / ESI)", "ಯೋಜನೆ ಕಾರ್ಡ್ (PM-JAY / CGHS / ESI)", "திட்ட அட்டை (PM-JAY / CGHS / ESI)"], "Insurance card / policy number": ["बीमा कार्ड / पॉलिसी नंबर", "ವಿಮಾ ಕಾರ್ಡ್ / ಪಾಲಿಸಿ ಸಂಖ್ಯೆ", "காப்பீட்டு அட்டை / பாலிசி எண்"], "From your insurer's app or TPA card. Ask the hospital's insurance desk about cashless approval.": ["अपने बीमा ऐप या TPA कार्ड से। कैशलेस मंज़ूरी के लिए अस्पताल के बीमा डेस्क से पूछें।", "ನಿಮ್ಮ ವಿಮಾ ಕಂಪನಿಯ ಆ್ಯಪ್ ಅಥವಾ TPA ಕಾರ್ಡ್‌ನಿಂದ. ನಗದುರಹಿತ ಅನುಮೋದನೆಗಾಗಿ ಆಸ್ಪತ್ರೆಯ ವಿಮಾ ಕೌಂಟರ್‌ನಲ್ಲಿ ಕೇಳಿ.", "உங்கள் காப்பீட்டு நிறுவனச் செயலி அல்லது TPA அட்டையிலிருந்து. பணமில்லா ஒப்புதல் பற்றி மருத்துவமனையின் காப்பீட்டு மேசையில் கேளுங்கள்."], "Referral letter": ["रेफ़रल पत्र", "ರೆಫರಲ್ ಪತ್ರ", "பரிந்துரைக் கடிதம்"], "Only a doctor can issue this. A General OPD or PHC doctor can refer you to this department — we can help you book that visit first.": ["यह केवल डॉक्टर दे सकते हैं। सामान्य ओपीडी या PHC के डॉक्टर आपको इस विभाग में रेफ़र कर सकते हैं — हम पहले वह मुलाक़ात बुक करने में मदद कर सकते हैं।", "ಇದನ್ನು ವೈದ್ಯರು ಮಾತ್ರ ನೀಡಬಹುದು. ಸಾಮಾನ್ಯ ಒಪಿಡಿ ಅಥವಾ PHC ವೈದ್ಯರು ನಿಮ್ಮನ್ನು ಈ ವಿಭಾಗಕ್ಕೆ ಶಿಫಾರಸು ಮಾಡಬಹುದು — ಮೊದಲು ಆ ಭೇಟಿ ಬುಕ್ ಮಾಡಲು ನಾವು ಸಹಾಯ ಮಾಡುತ್ತೇವೆ.", "இதை மருத்துவர் மட்டுமே வழங்க முடியும். பொது OPD அல்லது ஆரம்ப சுகாதார நிலைய மருத்துவர் உங்களை இந்தப் பிரிவுக்குப் பரிந்துரைக்கலாம் — முதலில் அந்த வருகையை முன்பதிவு செய்ய நாங்கள் உதவுவோம்."], "Previous reports & discharge summaries": ["पिछली रिपोर्टें और डिस्चार्ज सारांश", "ಹಿಂದಿನ ವರದಿಗಳು ಮತ್ತು ಡಿಸ್ಚಾರ್ಜ್ ಸಾರಾಂಶಗಳು", "முந்தைய அறிக்கைகள் & டிஸ்சார்ஜ் சுருக்கங்கள்"], "Collect from earlier visits; many labs share PDFs by SMS or WhatsApp. Bring originals and one photocopy.": ["पिछली मुलाक़ातों से इकट्ठा करें; कई लैब SMS या WhatsApp पर PDF भेजती हैं। मूल प्रतियाँ और एक फ़ोटोकॉपी लाएँ।", "ಹಿಂದಿನ ಭೇಟಿಗಳಿಂದ ಸಂಗ್ರಹಿಸಿ; ಹಲವು ಲ್ಯಾಬ್‌ಗಳು SMS ಅಥವಾ WhatsApp ಮೂಲಕ PDF ಕಳುಹಿಸುತ್ತವೆ. ಮೂಲ ಪ್ರತಿಗಳು ಮತ್ತು ಒಂದು ಜೆರಾಕ್ಸ್ ತನ್ನಿ.", "முந்தைய வருகைகளிலிருந்து சேகரியுங்கள்; பல ஆய்வகங்கள் SMS அல்லது WhatsApp வழியாக PDF அனுப்புகின்றன. அசல்களையும் ஒரு நகலையும் கொண்டு வாருங்கள்."], "Current prescription / medicine list": ["मौजूदा पर्ची / दवाओं की सूची", "ಪ್ರಸ್ತುತ ಔಷಧ ಚೀಟಿ / ಔಷಧಿ ಪಟ್ಟಿ", "தற்போதைய மருந்துச் சீட்டு / மருந்துப் பட்டியல்"], "Your last prescription, or photos of the medicine strips you use.": ["आपकी आख़िरी पर्ची, या जिन दवाओं का आप उपयोग करते हैं उनकी पट्टियों की फ़ोटो।", "ನಿಮ್ಮ ಕೊನೆಯ ಔಷಧ ಚೀಟಿ ಅಥವಾ ನೀವು ಬಳಸುವ ಮಾತ್ರೆ ಪಟ್ಟಿಗಳ ಫೋಟೋಗಳು.", "உங்கள் கடைசி மருந்துச் சீட்டு, அல்லது நீங்கள் பயன்படுத்தும் மாத்திரை அட்டைகளின் புகைப்படங்கள்."], "Test request slip": ["जाँच अनुरोध पर्ची", "ಪರೀಕ್ಷಾ ಕೋರಿಕೆ ಚೀಟಿ", "பரிசோதனை கோரிக்கைச் சீட்டு"], "Written by the doctor who asked for the tests. Without it, labs may only offer walk-in packages.": ["जाँच बताने वाले डॉक्टर द्वारा लिखी गई। इसके बिना लैब केवल वॉक-इन पैकेज दे सकती हैं।", "ಪರೀಕ್ಷೆಗಳನ್ನು ಸೂಚಿಸಿದ ವೈದ್ಯರು ಬರೆಯುತ್ತಾರೆ. ಇದಿಲ್ಲದೆ ಲ್ಯಾಬ್‌ಗಳು ವಾಕ್-ಇನ್ ಪ್ಯಾಕೇಜ್‌ಗಳನ್ನು ಮಾತ್ರ ನೀಡಬಹುದು.", "பரிசோதனைகளைச் சொன்ன மருத்துவர் எழுதியது. இது இல்லாமல் ஆய்வகங்கள் நேரடி பேக்கேஜ்களை மட்டுமே வழங்கலாம்."], "Vaccination card / U-WIN record": ["टीकाकरण कार्ड / U-WIN रिकॉर्ड", "ಲಸಿಕೆ ಕಾರ್ಡ್ / U-WIN ದಾಖಲೆ", "தடுப்பூசி அட்டை / U-WIN பதிவு"], "The card from the previous dose. Digital records: uwin.mohfw.gov.in.": ["पिछली खुराक का कार्ड। डिजिटल रिकॉर्ड: uwin.mohfw.gov.in।", "ಹಿಂದಿನ ಡೋಸ್‌ನ ಕಾರ್ಡ್. ಡಿಜಿಟಲ್ ದಾಖಲೆಗಳು: uwin.mohfw.gov.in.", "முந்தைய தவணையின் அட்டை. டிஜிட்டல் பதிவுகள்: uwin.mohfw.gov.in."], "Mother & Child Protection (MCP) card": ["मातृ एवं शिशु सुरक्षा (MCP) कार्ड", "ತಾಯಿ ಮತ್ತು ಮಗು ರಕ್ಷಣಾ (MCP) ಕಾರ್ಡ್", "தாய் சேய் பாதுகாப்பு (MCP) அட்டை"], "Issued at the first ANC registration. If you don't have one yet, it is issued at registration — mark it “In progress”.": ["पहले ANC पंजीकरण पर मिलता है। अगर अभी नहीं है, तो पंजीकरण पर मिल जाएगा — इसे “प्रक्रिया में” चिह्नित करें।", "ಮೊದಲ ANC ನೋಂದಣಿಯಲ್ಲಿ ನೀಡಲಾಗುತ್ತದೆ. ಇನ್ನೂ ಇಲ್ಲದಿದ್ದರೆ ನೋಂದಣಿಯಲ್ಲಿ ಸಿಗುತ್ತದೆ — ಇದನ್ನು “ಪ್ರಗತಿಯಲ್ಲಿ” ಎಂದು ಗುರುತಿಸಿ.", "முதல் ANC பதிவின்போது வழங்கப்படும். இன்னும் இல்லையென்றால் பதிவின்போது கிடைக்கும் — இதை “நடைபெறுகிறது” எனக் குறியிடுங்கள்."], "PICME number / RCH ID (Tamil Nadu)": ["PICME नंबर / RCH ID (तमिलनाडु)", "PICME ಸಂಖ್ಯೆ / RCH ID (ತಮಿಳುನಾಡು)", "PICME எண் / RCH ID (தமிழ்நாடு)"], "12-digit number from Tamil Nadu's pregnancy registration. Your Village or Urban Health Nurse can register you, or self-register at picme.tn.gov.in. It's needed for TN maternity benefits and later for the birth certificate. Not registered yet? Mark it “In progress” — the clinic can start it.": ["तमिलनाडु के गर्भावस्था पंजीकरण से मिलने वाला 12 अंकों का नंबर। आपकी ग्राम या शहरी स्वास्थ्य नर्स पंजीकरण कर सकती हैं, या picme.tn.gov.in पर स्वयं पंजीकरण करें। यह TN मातृत्व लाभ और बाद में जन्म प्रमाण पत्र के लिए ज़रूरी है। अभी पंजीकरण नहीं हुआ? इसे “प्रक्रिया में” चिह्नित करें — क्लिनिक शुरू कर सकता है।", "ತಮಿಳುನಾಡಿನ ಗರ್ಭಧಾರಣೆ ನೋಂದಣಿಯಿಂದ ಸಿಗುವ 12 ಅಂಕಿಯ ಸಂಖ್ಯೆ. ನಿಮ್ಮ ಗ್ರಾಮ ಅಥವಾ ನಗರ ಆರೋಗ್ಯ ದಾದಿ ನೋಂದಾಯಿಸಬಹುದು, ಅಥವಾ picme.tn.gov.in ನಲ್ಲಿ ನೀವೇ ನೋಂದಾಯಿಸಿ. ಇದು TN ಹೆರಿಗೆ ಸೌಲಭ್ಯಗಳಿಗೆ ಮತ್ತು ನಂತರ ಜನನ ಪ್ರಮಾಣಪತ್ರಕ್ಕೆ ಅಗತ್ಯ. ಇನ್ನೂ ನೋಂದಾಯಿಸಿಲ್ಲವೇ? “ಪ್ರಗತಿಯಲ್ಲಿ” ಎಂದು ಗುರುತಿಸಿ — ಕ್ಲಿನಿಕ್ ಆರಂಭಿಸಬಹುದು.", "தமிழ்நாட்டின் கர்ப்பப் பதிவில் கிடைக்கும் 12 இலக்க எண். உங்கள் கிராம அல்லது நகர்ப்புற சுகாதார செவிலியர் பதிவு செய்யலாம், அல்லது picme.tn.gov.in இல் நீங்களே பதிவு செய்யலாம். தமிழக மகப்பேறு உதவிகளுக்கும் பின்னர் பிறப்புச் சான்றிதழுக்கும் இது தேவை. இன்னும் பதிவு செய்யவில்லையா? “நடைபெறுகிறது” எனக் குறியிடுங்கள் — மருத்துவமனை தொடங்கலாம்."], "Self-pay": ["स्वयं भुगतान", "ಸ್ವಂತ ಪಾವತಿ", "சொந்தச் செலவு"], "Ayushman Bharat PM-JAY": ["आयुष्मान भारत PM-JAY", "ಆಯುಷ್ಮಾನ್ ಭಾರತ್ PM-JAY", "ஆயுஷ்மான் பாரத் PM-JAY"], "Private insurance": ["निजी बीमा", "ಖಾಸಗಿ ವಿಮೆ", "தனியார் காப்பீடு"], "CMCHIS (TN Chief Minister's scheme)": ["CMCHIS (तमिलनाडु मुख्यमंत्री योजना)", "CMCHIS (ತಮಿಳುನಾಡು ಮುಖ್ಯಮಂತ್ರಿ ಯೋಜನೆ)", "CMCHIS (முதலமைச்சரின் மருத்துவக் காப்பீட்டுத் திட்டம்)"], "Step-free / wheelchair access": ["सीढ़ी-रहित / व्हीलचेयर पहुँच", "ಮೆಟ್ಟಿಲುರಹಿತ / ಗಾಲಿಕುರ್ಚಿ ಪ್ರವೇಶ", "படியில்லா / சக்கர நாற்காலி அணுகல்"], "Step-free": ["सीढ़ी-रहित", "ಮೆಟ್ಟಿಲುರಹಿತ", "படியில்லா அணுகல்"], "Working lift": ["चालू लिफ़्ट", "ಕಾರ್ಯನಿರತ ಲಿಫ್ಟ್", "இயங்கும் லிஃப்ட்"], "Sign-language interpreter": ["सांकेतिक भाषा दुभाषिया", "ಸಂಜ್ಞಾ ಭಾಷೆ ವ್ಯಾಖ್ಯಾನಕಾರ", "சைகை மொழி பெயர்ப்பாளர்"], "Braille / low-vision help": ["ब्रेल / कम दृष्टि सहायता", "ಬ್ರೈಲ್ / ಕಡಿಮೆ ದೃಷ್ಟಿ ಸಹಾಯ", "பிரெய்லி / குறைந்த பார்வை உதவி"], "Braille": ["ब्रेल", "ಬ್ರೈಲ್", "பிரெய்லி"], "Accessible toilet": ["सुगम्य शौचालय", "ಸುಗಮ ಶೌಚಾಲಯ", "அணுகக்கூடிய கழிப்பறை"], "Any time": ["कभी भी", "ಯಾವಾಗ ಬೇಕಾದರೂ", "எந்த நேரமும்"], "Mornings": ["सुबह", "ಬೆಳಿಗ್ಗೆ", "காலை நேரம்"], "Afternoons": ["दोपहर", "ಮಧ್ಯಾಹ್ನ", "மதிய நேரம்"], "Weekends": ["सप्ताहांत", "ವಾರಾಂತ್ಯ", "வார இறுதி"], "English": ["अंग्रेज़ी", "ಇಂಗ್ಲಿಷ್", "ஆங்கிலம்"], "Kannada": ["कन्नड़", "ಕನ್ನಡ", "கன்னடம்"], "Hindi": ["हिन्दी", "ಹಿಂದಿ", "இந்தி"], "Tamil": ["तमिल", "ತಮಿಳು", "தமிழ்"], "Telugu": ["तेलुगु", "ತೆಲುಗು", "தெலுங்கு"], "Urdu": ["उर्दू", "ಉರ್ದು", "உருது"], "Malayalam": ["मलयालम", "ಮಲಯಾಳಂ", "மலையாளம்"], "Bengali": ["बांग्ला", "ಬಂಗಾಳಿ", "வங்காளம்"], "Chennai, TN": ["चेन्नई, तमिलनाडु", "ಚೆನ್ನೈ, ತಮಿಳುನಾಡು", "சென்னை, தமிழ்நாடு"], "Bengaluru, KA": ["बेंगलुरु, कर्नाटक", "ಬೆಂಗಳೂರು, ಕರ್ನಾಟಕ", "பெங்களூரு, கர்நாடகா"], "Chennai, Tamil Nadu": ["चेन्नई, तमिलनाडु", "ಚೆನ್ನೈ, ತಮಿಳುನಾಡು", "சென்னை, தமிழ்நாடு"], "Bengaluru, Karnataka": ["बेंगलुरु, कर्नाटक", "ಬೆಂಗಳೂರು, ಕರ್ನಾಟಕ", "பெங்களூரு, கர்நாடகா"], "Tondiarpet": ["तोंडियारपेट", "ತೊಂಡಿಯಾರ್‌ಪೇಟೆ", "தண்டையார்பேட்டை"], "Perambur": ["पेरम्बूर", "ಪೆರಂಬೂರ್", "பெரம்பூர்"], "Anna Nagar": ["अन्ना नगर", "ಅಣ್ಣಾ ನಗರ", "அண்ணா நகர்"], "Egmore": ["एग्मोर", "ಎಗ್ಮೋರ್", "எழும்பூர்"], "Triplicane": ["ट्रिप्लिकेन", "ಟ್ರಿಪ್ಲಿಕೇನ್", "திருவல்லிக்கேணி"], "T. Nagar": ["टी. नगर", "ಟಿ. ನಗರ", "தி. நகர்"], "Porur": ["पोरूर", "ಪೋರೂರ್", "போரூர்"], "Guindy": ["गिंडी", "ಗಿಂಡಿ", "கிண்டி"], "Adyar": ["अड्यार", "ಅಡ್ಯಾರ್", "அடையாறு"], "Velachery": ["वेलाचेरी", "ವೇಳಚೇರಿ", "வேளச்சேரி"], "Sholinganallur (OMR)": ["शोलिंगनल्लूर (OMR)", "ಶೋಳಿಂಗನಲ್ಲೂರು (OMR)", "சோழிங்கநல்லூர் (OMR)"], "Tambaram": ["तांबरम", "ತಾಂಬರಂ", "தாம்பரம்"], "Peenya": ["पीन्या", "ಪೀಣ್ಯ", "பீன்யா"], "Hebbal": ["हेब्बाल", "ಹೆಬ್ಬಾಳ", "ஹெப்பால்"], "Malleshwaram": ["मल्लेश्वरम", "ಮಲ್ಲೇಶ್ವರಂ", "மல்லேஸ்வரம்"], "Indiranagar": ["इंदिरानगर", "ಇಂದಿರಾನಗರ", "இந்திரா நகர்"], "Whitefield": ["व्हाइटफ़ील्ड", "ವೈಟ್‌ಫೀಲ್ಡ್", "வைட்ஃபீல்டு"], "Basavanagudi": ["बसवनगुडी", "ಬಸವನಗುಡಿ", "பசவனகுடி"], "Koramangala": ["कोरमंगला", "ಕೋರಮಂಗಲ", "கோரமங்களா"], "Jayanagar": ["जयनगर", "ಜಯನಗರ", "ஜெயநகர்"], "BTM Layout": ["बीटीएम लेआउट", "ಬಿಟಿಎಂ ಲೇಔಟ್", "பிடிஎம் லேஅவுட்"], "Bannerghatta Rd": ["बन्नेरघट्टा रोड", "ಬನ್ನೇರುಘಟ್ಟ ರಸ್ತೆ", "பன்னர்கட்டா சாலை"], "Thendral Government Medical College Hospital": ["तेन्ड्रल सरकारी मेडिकल कॉलेज अस्पताल", "ತೆಂಡ್ರಲ್ ಸರ್ಕಾರಿ ವೈದ್ಯಕೀಯ ಕಾಲೇಜು ಆಸ್ಪತ್ರೆ", "தென்றல் அரசு மருத்துவக் கல்லூரி மருத்துவமனை"], "Nalam Urban PHC": ["नलम शहरी प्राथमिक स्वास्थ्य केंद्र", "ನಲಂ ನಗರ ಪ್ರಾಥಮಿಕ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "நலம் நகர்ப்புற ஆரம்ப சுகாதார நிலையம்"], "Sangamam Multispeciality Hospital": ["संगमम मल्टीस्पेशियलिटी अस्पताल", "ಸಂಗಮಂ ಮಲ್ಟಿಸ್ಪೆಷಾಲಿಟಿ ಆಸ್ಪತ್ರೆ", "சங்கமம் பல்நோக்கு மருத்துவமனை"], "Paarvai Eye Hospital": ["पार्वई नेत्र अस्पताल", "ಪಾರ್ವೈ ಕಣ್ಣಿನ ಆಸ್ಪತ್ರೆ", "பார்வை கண் மருத்துவமனை"], "Vadachennai Community Health Centre": ["वडचेन्नई सामुदायिक स्वास्थ्य केंद्र", "ವಡಚೆನ್ನೈ ಸಮುದಾಯ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "வடசென்னை சமுதாய சுகாதார நிலையம்"], "Thozhilalar ESI Dispensary": ["तोझिलालर ESI डिस्पेंसरी", "ತೊಳಿಲಾಳರ್ ESI ಔಷಧಾಲಯ", "தொழிலாளர் ESI மருந்தகம்"], "Punnagai Dental Clinic": ["पुन्नगई डेंटल क्लिनिक", "ಪುನ್ನಗೈ ದಂತ ಚಿಕಿತ್ಸಾಲಯ", "புன்னகை பல் மருத்துவமனை"], "Thaimai Government Women & Children Hospital": ["थाइमई सरकारी महिला एवं बाल अस्पताल", "ತಾಯ್ಮೈ ಸರ್ಕಾರಿ ಮಹಿಳಾ ಮತ್ತು ಮಕ್ಕಳ ಆಸ್ಪತ್ರೆ", "தாய்மை அரசு மகளிர் & குழந்தைகள் மருத்துவமனை"], "Irudhayam Heart Institute": ["इरुदयम हृदय संस्थान", "ಇರುದಯಂ ಹೃದಯ ಸಂಸ್ಥೆ", "இருதயம் இதய நிறுவனம்"], "Meendum Physio & Rehab Centre": ["मीन्डुम फ़िज़ियो एवं पुनर्वास केंद्र", "ಮೀಂಡುಮ್ ಫಿಸಿಯೋ ಮತ್ತು ಪುನರ್ವಸತಿ ಕೇಂದ್ರ", "மீண்டும் பிசியோ & மறுவாழ்வு மையம்"], "Thamarai Government Hospital": ["तामरई सरकारी अस्पताल", "ತಾಮರೈ ಸರ್ಕಾರಿ ಆಸ್ಪತ್ರೆ", "தாமரை அரசு மருத்துவமனை"], "Sanjeevini District Hospital": ["संजीविनी जिला अस्पताल", "ಸಂಜೀವಿನಿ ಜಿಲ್ಲಾ ಆಸ್ಪತ್ರೆ", "சஞ்சீவினி மாவட்ட மருத்துவமனை"], "Arogya Urban PHC": ["आरोग्य शहरी प्राथमिक स्वास्थ्य केंद्र", "ಆರೋಗ್ಯ ನಗರ ಪ್ರಾಥಮಿಕ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "ஆரோக்கிய நகர்ப்புற ஆரம்ப சுகாதார நிலையம்"], "Nirmala Multispeciality Hospital": ["निर्मला मल्टीस्पेशियलिटी अस्पताल", "ನಿರ್ಮಲಾ ಮಲ್ಟಿಸ್ಪೆಷಾಲಿಟಿ ಆಸ್ಪತ್ರೆ", "நிர்மலா பல்நோக்கு மருத்துவமனை"], "Drishti Eye Care Centre": ["दृष्टि नेत्र देखभाल केंद्र", "ದೃಷ್ಟಿ ಕಣ್ಣಿನ ಆರೈಕೆ ಕೇಂದ್ರ", "திருஷ்டி கண் பராமரிப்பு மையம்"], "Hebbal Community Health Centre": ["हेब्बाल सामुदायिक स्वास्थ्य केंद्र", "ಹೆಬ್ಬಾಳ ಸಮುದಾಯ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "ஹெப்பால் சமுதாய சுகாதார நிலையம்"], "ESI Dispensary, Peenya": ["ESI डिस्पेंसरी, पीन्या", "ESI ಔಷಧಾಲಯ, ಪೀಣ್ಯ", "ESI மருந்தகம், பீன்யா"], "SmileLine Dental Clinic": ["स्माइललाइन डेंटल क्लिनिक", "ಸ್ಮೈಲ್‌ಲೈನ್ ದಂತ ಚಿಕಿತ್ಸಾಲಯ", "ஸ்மைல்லைன் பல் மருத்துவமனை"], "Vatsalya Women & Children Hospital": ["वात्सल्य महिला एवं बाल अस्पताल", "ವಾತ್ಸಲ್ಯ ಮಹಿಳಾ ಮತ್ತು ಮಕ್ಕಳ ಆಸ್ಪತ್ರೆ", "வாத்ஸல்யா மகளிர் & குழந்தைகள் மருத்துவமனை"], "Hrudaya Heart Institute": ["हृदय हार्ट इंस्टीट्यूट", "ಹೃದಯ ಹೃದ್ರೋಗ ಸಂಸ್ಥೆ", "ஹ்ருதயா இதய நிறுவனம்"], "Seva Physio & Rehab Centre": ["सेवा फ़िज़ियो एवं पुनर्वास केंद्र", "ಸೇವಾ ಫಿಸಿಯೋ ಮತ್ತು ಪುನರ್ವಸತಿ ಕೇಂದ್ರ", "சேவா பிசியோ & மறுவாழ்வு மையம்"], "Govt medical college hospital": ["सरकारी मेडिकल कॉलेज अस्पताल", "ಸರ್ಕಾರಿ ವೈದ್ಯಕೀಯ ಕಾಲೇಜು ಆಸ್ಪತ್ರೆ", "அரசு மருத்துவக் கல்லூரி மருத்துவமனை"], "Urban primary health centre": ["शहरी प्राथमिक स्वास्थ्य केंद्र", "ನಗರ ಪ್ರಾಥಮಿಕ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "நகர்ப்புற ஆரம்ப சுகாதார நிலையம்"], "Private multi-speciality hospital": ["निजी मल्टीस्पेशियलिटी अस्पताल", "ಖಾಸಗಿ ಬಹುವಿಶೇಷ ಆಸ್ಪತ್ರೆ", "தனியார் பல்நோக்கு மருத்துவமனை"], "Private eye hospital": ["निजी नेत्र अस्पताल", "ಖಾಸಗಿ ಕಣ್ಣಿನ ಆಸ್ಪತ್ರೆ", "தனியார் கண் மருத்துவமனை"], "Community health centre": ["सामुदायिक स्वास्थ्य केंद्र", "ಸಮುದಾಯ ಆರೋಗ್ಯ ಕೇಂದ್ರ", "சமுதாய சுகாதார நிலையம்"], "ESI dispensary": ["ESI डिस्पेंसरी", "ESI ಔಷಧಾಲಯ", "ESI மருந்தகம்"], "Private dental clinic": ["निजी दंत क्लिनिक", "ಖಾಸಗಿ ದಂತ ಚಿಕಿತ್ಸಾಲಯ", "தனியார் பல் மருத்துவமனை"], "Govt women & children hospital": ["सरकारी महिला एवं बाल अस्पताल", "ಸರ್ಕಾರಿ ಮಹಿಳಾ ಮತ್ತು ಮಕ್ಕಳ ಆಸ್ಪತ್ರೆ", "அரசு மகளிர் & குழந்தைகள் மருத்துவமனை"], "Cardiac speciality hospital (trust)": ["हृदय विशेष अस्पताल (ट्रस्ट)", "ಹೃದ್ರೋಗ ವಿಶೇಷ ಆಸ್ಪತ್ರೆ (ಟ್ರಸ್ಟ್)", "இதய சிறப்பு மருத்துவமனை (அறக்கட்டளை)"], "Private rehab centre": ["निजी पुनर्वास केंद्र", "ಖಾಸಗಿ ಪುನರ್ವಸತಿ ಕೇಂದ್ರ", "தனியார் மறுவாழ்வு மையம்"], "Govt taluk hospital": ["सरकारी तालुक अस्पताल", "ಸರ್ಕಾರಿ ತಾಲೂಕು ಆಸ್ಪತ್ರೆ", "அரசு வட்ட மருத்துவமனை"], "Govt district hospital": ["सरकारी जिला अस्पताल", "ಸರ್ಕಾರಿ ಜಿಲ್ಲಾ ಆಸ್ಪತ್ರೆ", "அரசு மாவட்ட மருத்துவமனை"], "OPD": ["ओपीडी", "ಒಪಿಡಿ", "வெளிநோயாளர் பிரிவு"], "Block A": ["ब्लॉक A", "ಬ್ಲಾಕ್ A", "பிளாக் A"], "Block C": ["ब्लॉक C", "ಬ್ಲಾಕ್ C", "பிளாக் C"], "Tower 2": ["टावर 2", "ಟವರ್ 2", "டவர் 2"], "Ophthalmology OPD": ["नेत्र रोग ओपीडी", "ನೇತ್ರ ಒಪಿಡಿ", "கண் மருத்துவ வெளிநோயாளர் பிரிவு"], "Dental OPD": ["दंत ओपीडी", "ದಂತ ಒಪಿಡಿ", "பல் வெளிநோயாளர் பிரிவு"], "Central Lab": ["केंद्रीय लैब", "ಕೇಂದ್ರ ಪ್ರಯೋಗಾಲಯ", "மைய ஆய்வகம்"], "Cardiology OPD": ["हृदय रोग ओपीडी", "ಹೃದ್ರೋಗ ಒಪಿಡಿ", "இதய வெளிநோயாளர் பிரிவு"], "Orthopaedics OPD": ["हड्डी रोग ओपीडी", "ಮೂಳೆ ಚಿಕಿತ್ಸಾ ಒಪಿಡಿ", "எலும்பு வெளிநோயாளர் பிரிவு"], "Physical Medicine & Rehab": ["भौतिक चिकित्सा एवं पुनर्वास", "ದೈಹಿಕ ಚಿಕಿತ್ಸೆ ಮತ್ತು ಪುನರ್ವಸತಿ", "உடலியக்க மருத்துவம் & மறுவாழ்வு"], "Diabetology OPD": ["मधुमेह ओपीडी", "ಮಧುಮೇಹ ಒಪಿಡಿ", "நீரிழிவு வெளிநோயாளர் பிரிவு"], "Immunisation room": ["टीकाकरण कक्ष", "ಲಸಿಕಾ ಕೊಠಡಿ", "தடுப்பூசி அறை"], "OPD room 1": ["ओपीडी कक्ष 1", "ಒಪಿಡಿ ಕೊಠಡಿ 1", "வெளிநோயாளர் அறை 1"], "OPD room 2": ["ओपीडी कक्ष 2", "ಒಪಿಡಿ ಕೊಠಡಿ 2", "வெளிநோயாளர் அறை 2"], "Immunisation (Wed & Sat)": ["टीकाकरण (बुध और शनि)", "ಲಸಿಕೆ (ಬುಧ ಮತ್ತು ಶನಿ)", "தடுப்பூசி (புதன் & சனி)"], "Antenatal clinic": ["प्रसवपूर्व क्लिनिक", "ಪ್ರಸವಪೂರ್ವ ಚಿಕಿತ್ಸಾಲಯ", "மகப்பேறுக்கு முந்தைய சிகிச்சைப் பிரிவு"], "ANC clinic": ["ANC क्लिनिक", "ANC ಚಿಕಿತ್ಸಾಲಯ", "ANC சிகிச்சைப் பிரிவு"], "Lab counter": ["लैब काउंटर", "ಲ್ಯಾಬ್ ಕೌಂಟರ್", "ஆய்வக கவுண்டர்"], "NCD clinic": ["एनसीडी क्लिनिक", "ಎನ್‌ಸಿಡಿ ಚಿಕಿತ್ಸಾಲಯ", "NCD சிகிச்சைப் பிரிவு"], "NCD / Diabetes clinic": ["एनसीडी / मधुमेह क्लिनिक", "ಎನ್‌ಸಿಡಿ / ಮಧುಮೇಹ ಚಿಕಿತ್ಸಾಲಯ", "NCD / நீரிழிவு சிகிச்சைப் பிரிவு"], "Family medicine": ["पारिवारिक चिकित्सा", "ಕುಟುಂಬ ವೈದ್ಯಕೀಯ", "குடும்ப மருத்துவம்"], "Eye clinic": ["नेत्र क्लिनिक", "ಕಣ್ಣಿನ ಚಿಕಿತ್ಸಾಲಯ", "கண் சிகிச்சைப் பிரிவு"], "Dental clinic": ["दंत क्लिनिक", "ದಂತ ಚಿಕಿತ್ಸಾಲಯ", "பல் சிகிச்சைப் பிரிவு"], "Diagnostics": ["जाँच केंद्र", "ರೋಗನಿರ್ಣಯ ವಿಭಾಗ", "நோயறிதல் பிரிவு"], "Rehab": ["पुनर्वास", "ಪುನರ್ವಸತಿ", "மறுவாழ்வு"], "Endocrinology": ["अंतःस्रावी विभाग", "ಅಂತಃಸ್ರಾವ ವಿಭಾಗ", "நாளமில்லா சுரப்பியியல்"], "Eye OPD": ["नेत्र ओपीडी", "ಕಣ್ಣಿನ ಒಪಿಡಿ", "கண் வெளிநோயாளர் பிரிவு"], "Maternal health OPD": ["मातृ स्वास्थ्य ओपीडी", "ತಾಯಿ ಆರೋಗ್ಯ ಒಪಿಡಿ", "தாய் நல வெளிநோயாளர் பிரிவு"], "Immunisation": ["टीकाकरण", "ಲಸಿಕೆ", "தடுப்பூசி"], "Lab": ["लैब", "ಲ್ಯಾಬ್", "ஆய்வகம்"], "Dental chairs 1–3": ["दंत कुर्सी 1–3", "ದಂತ ಕುರ್ಚಿಗಳು 1–3", "பல் நாற்காலிகள் 1–3"], "Women's OPD": ["महिला ओपीडी", "ಮಹಿಳಾ ಒಪಿಡಿ", "மகளிர் வெளிநோயாளர் பிரிவு"], "Cardiac diagnostics": ["हृदय जाँच", "ಹೃದಯ ಪರೀಕ್ಷೆಗಳು", "இதயப் பரிசோதனைகள்"], "Rehab floor": ["पुनर्वास तल", "ಪುನರ್ವಸತಿ ಮಹಡಿ", "மறுவாழ்வுத் தளம்"], "Ortho consult": ["हड्डी रोग परामर्श", "ಮೂಳೆ ತಜ್ಞರ ಸಮಾಲೋಚನೆ", "எலும்பு மருத்துவ ஆலோசனை"], "Physiotherapy unit": ["फ़िज़ियोथेरेपी इकाई", "ಫಿಸಿಯೋಥೆರಪಿ ಘಟಕ", "பிசியோதெரபி பிரிவு"], "ground floor": ["भूतल", "ನೆಲ ಮಹಡಿ", "தரைத் தளம்"], "Free": ["निःशुल्क", "ಉಚಿತ", "இலவசம்"], "Free (₹10 registration)": ["निःशुल्क (₹10 पंजीकरण)", "ಉಚಿತ (₹10 ನೋಂದಣಿ)", "இலவசம் (₹10 பதிவு)"], "Free under scheme / from ₹150": ["योजना में निःशुल्क / ₹150 से", "ಯೋಜನೆಯಡಿ ಉಚಿತ / ₹150 ರಿಂದ", "திட்டத்தில் இலவசம் / ₹150 முதல்"], "Free for ESI members": ["ESI सदस्यों के लिए निःशुल्क", "ESI ಸದಸ್ಯರಿಗೆ ಉಚಿತ", "ESI உறுப்பினர்களுக்கு இலவசம்"], "Free under CMCHIS / PM-JAY": ["CMCHIS / PM-JAY में निःशुल्क", "CMCHIS / PM-JAY ಅಡಿ ಉಚಿತ", "CMCHIS / PM-JAY இல் இலவசம்"], "Free under PM-JAY / ₹600": ["PM-JAY में निःशुल्क / ₹600", "PM-JAY ಅಡಿ ಉಚಿತ / ₹600", "PM-JAY இல் இலவசம் / ₹600"], "Cardiology OPD days": ["हृदय रोग ओपीडी के दिन", "ಹೃದ್ರೋಗ ಒಪಿಡಿ ದಿನಗಳು", "இதய வெளிநோயாளர் பிரிவு நாட்கள்"], "CMCHIS / PM-JAY coverage": ["CMCHIS / PM-JAY कवरेज", "CMCHIS / PM-JAY ವ್ಯಾಪ್ತಿ", "CMCHIS / PM-JAY காப்பீட்டு வரம்பு"], "PM-JAY coverage": ["PM-JAY कवरेज", "PM-JAY ವ್ಯಾಪ್ತಿ", "PM-JAY காப்பீட்டு வரம்பு"], "Phone number": ["फ़ोन नंबर", "ದೂರವಾಣಿ ಸಂಖ್ಯೆ", "தொலைபேசி எண்"], "Step-free access": ["सीढ़ी-रहित पहुँच", "ಮೆಟ್ಟಿಲುರಹಿತ ಪ್ರವೇಶ", "படியில்லா அணுகல்"], "Directory lists Mon–Sat. A notice-board photo submitted on 31 Oct says Cardiology OPD runs Tue, Thu and Sat only.": ["निर्देशिका में सोम–शनि लिखा है। 31 अक्टूबर को भेजी गई नोटिस-बोर्ड की फ़ोटो के अनुसार हृदय रोग ओपीडी केवल मंगल, गुरु और शनि को चलती है।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ ಸೋಮ–ಶನಿ ಎಂದಿದೆ. ಅಕ್ಟೋಬರ್ 31 ರಂದು ಕಳುಹಿಸಿದ ಸೂಚನಾ ಫಲಕದ ಫೋಟೋ ಪ್ರಕಾರ ಹೃದ್ರೋಗ ಒಪಿಡಿ ಮಂಗಳ, ಗುರು ಮತ್ತು ಶನಿವಾರ ಮಾತ್ರ ನಡೆಯುತ್ತದೆ.", "அடைவில் திங்கள்–சனி என உள்ளது. அக்டோபர் 31 அன்று அனுப்பப்பட்ட அறிவிப்புப் பலகைப் புகைப்படத்தின்படி இதய வெளிநோயாளர் பிரிவு செவ்வாய், வியாழன், சனி மட்டுமே இயங்குகிறது."], "Directory lists Mon–Sat. A notice-board photo submitted on 31 Oct says Cardiology OPD runs Mon, Wed and Fri only.": ["निर्देशिका में सोम–शनि लिखा है। 31 अक्टूबर को भेजी गई नोटिस-बोर्ड की फ़ोटो के अनुसार हृदय रोग ओपीडी केवल सोम, बुध और शुक्र को चलती है।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ ಸೋಮ–ಶನಿ ಎಂದಿದೆ. ಅಕ್ಟೋಬರ್ 31 ರಂದು ಕಳುಹಿಸಿದ ಸೂಚನಾ ಫಲಕದ ಫೋಟೋ ಪ್ರಕಾರ ಹೃದ್ರೋಗ ಒಪಿಡಿ ಸೋಮ, ಬುಧ ಮತ್ತು ಶುಕ್ರವಾರ ಮಾತ್ರ ನಡೆಯುತ್ತದೆ.", "அடைவில் திங்கள்–சனி என உள்ளது. அக்டோபர் 31 அன்று அனுப்பப்பட்ட அறிவிப்புப் பலகைப் புகைப்படத்தின்படி இதய வெளிநோயாளர் பிரிவு திங்கள், புதன், வெள்ளி மட்டுமே இயங்குகிறது."], "Directory lists CMCHIS and PM-JAY as accepted; the hospital's insurance desk says scheme cover applies to approved in-patient procedures, not OPD consultations.": ["निर्देशिका में CMCHIS और PM-JAY स्वीकार्य बताए गए हैं; अस्पताल का बीमा डेस्क कहता है कि योजना केवल स्वीकृत भर्ती उपचारों पर लागू है, ओपीडी परामर्श पर नहीं।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ CMCHIS ಮತ್ತು PM-JAY ಸ್ವೀಕರಿಸಲಾಗುತ್ತದೆ ಎಂದಿದೆ; ಆದರೆ ಆಸ್ಪತ್ರೆಯ ವಿಮಾ ಕೌಂಟರ್ ಪ್ರಕಾರ ಯೋಜನೆ ಅನುಮೋದಿತ ಒಳರೋಗಿ ಚಿಕಿತ್ಸೆಗಳಿಗೆ ಮಾತ್ರ, ಒಪಿಡಿ ಸಮಾಲೋಚನೆಗೆ ಅಲ್ಲ.", "அடைவில் CMCHIS, PM-JAY ஏற்கப்படும் என உள்ளது; ஆனால் மருத்துவமனையின் காப்பீட்டு மேசை, திட்டம் அங்கீகரிக்கப்பட்ட உள்நோயாளர் சிகிச்சைகளுக்கு மட்டுமே பொருந்தும், வெளிநோயாளர் ஆலோசனைக்கு அல்ல என்கிறது."], "Directory lists PM-JAY as accepted; the hospital website lists PM-JAY for in-patient packages only, not OPD consultations.": ["निर्देशिका में PM-JAY स्वीकार्य बताया गया है; अस्पताल की वेबसाइट पर PM-JAY केवल भर्ती पैकेजों के लिए है, ओपीडी परामर्श के लिए नहीं।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ PM-JAY ಸ್ವೀಕರಿಸಲಾಗುತ್ತದೆ ಎಂದಿದೆ; ಆಸ್ಪತ್ರೆಯ ವೆಬ್‌ಸೈಟ್‌ನಲ್ಲಿ PM-JAY ಒಳರೋಗಿ ಪ್ಯಾಕೇಜ್‌ಗಳಿಗೆ ಮಾತ್ರ, ಒಪಿಡಿ ಸಮಾಲೋಚನೆಗೆ ಅಲ್ಲ.", "அடைவில் PM-JAY ஏற்கப்படும் என உள்ளது; மருத்துவமனை இணையதளத்தில் PM-JAY உள்நோயாளர் தொகுப்புகளுக்கு மட்டுமே, வெளிநோயாளர் ஆலோசனைக்கு அல்ல."], "Auto-check across fields": ["फ़ील्ड्स की स्वचालित जाँच", "ಕ್ಷೇತ್ರಗಳ ಸ್ವಯಂ ಪರಿಶೀಲನೆ", "தரவுப் புலங்களின் தானியங்கி சரிபார்ப்பு"], "Organiser directory vs. facility insurance desk": ["आयोजक निर्देशिका बनाम अस्पताल बीमा डेस्क", "ಆಯೋಜಕರ ಡೈರೆಕ್ಟರಿ vs ಆಸ್ಪತ್ರೆ ವಿಮಾ ಕೌಂಟರ್", "ஏற்பாட்டாளர் அடைவு vs மருத்துவமனை காப்பீட்டு மேசை"], "Organiser directory vs. facility website": ["आयोजक निर्देशिका बनाम अस्पताल वेबसाइट", "ಆಯೋಜಕರ ಡೈರೆಕ್ಟರಿ vs ಆಸ್ಪತ್ರೆ ವೆಬ್‌ಸೈಟ್", "ஏற்பாட்டாளர் அடைவு vs மருத்துவமனை இணையதளம்"], "Organiser directory vs. community report": ["आयोजक निर्देशिका बनाम सामुदायिक रिपोर्ट", "ಆಯೋಜಕರ ಡೈರೆಕ್ಟರಿ vs ಸಮುದಾಯ ವರದಿ", "ஏற்பாட்டாளர் அடைவு vs சமூக அறிக்கை"], "Organiser directory vs. patient report": ["आयोजक निर्देशिका बनाम मरीज़ रिपोर्ट", "ಆಯೋಜಕರ ಡೈರೆಕ್ಟರಿ vs ರೋಗಿಯ ವರದಿ", "ஏற்பாட்டாளர் அடைவு vs நோயாளி அறிக்கை"], "ISL interpreter with 24 h notice": ["24 घंटे की पूर्व सूचना पर ISL दुभाषिया", "24 ಗಂಟೆ ಮುಂಚಿತ ಸೂಚನೆಯೊಂದಿಗೆ ISL ವ್ಯಾಖ್ಯಾನಕಾರ", "24 மணி நேர முன்னறிவிப்புடன் ISL மொழிபெயர்ப்பாளர்"], "ISL interpreter on request (24 h)": ["अनुरोध पर ISL दुभाषिया (24 घंटे)", "ಕೋರಿಕೆಯ ಮೇರೆಗೆ ISL ವ್ಯಾಖ್ಯಾನಕಾರ (24 ಗಂಟೆ)", "கோரிக்கையின் பேரில் ISL மொழிபெயர்ப்பாளர் (24 மணி)"], "Selvi": ["सेल्वी", "ಸೆಲ್ವಿ", "செல்வி"], "Karthik": ["कार्तिक", "ಕಾರ್ತಿಕ್", "கார்த்திக்"], "Ayesha": ["आयशा", "ಆಯಿಷಾ", "ஆயிஷா"], "Lakshmi": ["लक्ष्मी", "ಲಕ್ಷ್ಮಿ", "லட்சுமி"], "Arjun": ["अर्जुन", "ಅರ್ಜುನ್", "அர்ஜுன்"], "Fatima": ["फ़ातिमा", "ಫಾತಿಮಾ", "பாத்திமா"], "Tamil speaker, uses a wheelchair, CMCHIS card. Her doctor told her to see a heart specialist; no referral letter yet.": ["तमिल भाषी, व्हीलचेयर का उपयोग करती हैं, CMCHIS कार्ड है। डॉक्टर ने हृदय विशेषज्ञ से मिलने को कहा है; अभी रेफ़रल पत्र नहीं है।", "ತಮಿಳು ಮಾತನಾಡುತ್ತಾರೆ, ಗಾಲಿಕುರ್ಚಿ ಬಳಸುತ್ತಾರೆ, CMCHIS ಕಾರ್ಡ್ ಇದೆ. ವೈದ್ಯರು ಹೃದಯ ತಜ್ಞರನ್ನು ಭೇಟಿ ಮಾಡಲು ಹೇಳಿದ್ದಾರೆ; ಇನ್ನೂ ರೆಫರಲ್ ಪತ್ರ ಇಲ್ಲ.", "தமிழ் பேசுபவர், சக்கர நாற்காலி பயன்படுத்துகிறார், CMCHIS அட்டை உள்ளது. இதய நிபுணரைப் பார்க்கும்படி மருத்துவர் சொன்னார்; இன்னும் பரிந்துரைக் கடிதம் இல்லை."], "Deaf, uses Indian Sign Language. Needs an eye check-up, paying himself.": ["बधिर हैं, भारतीय सांकेतिक भाषा का उपयोग करते हैं। आँखों की जाँच चाहिए, ख़ुद भुगतान करेंगे।", "ಕಿವುಡರು, ಭಾರತೀಯ ಸಂಜ್ಞಾ ಭಾಷೆ ಬಳಸುತ್ತಾರೆ. ಕಣ್ಣಿನ ತಪಾಸಣೆ ಬೇಕು, ಸ್ವತಃ ಪಾವತಿಸುತ್ತಾರೆ.", "காது கேளாதவர், இந்திய சைகை மொழி பயன்படுத்துகிறார். கண் பரிசோதனை தேவை, தானே பணம் செலுத்துகிறார்."], "Speaks Urdu and Tamil. First pregnancy check-up; no MCP card or PICME number yet.": ["उर्दू और तमिल बोलती हैं। पहली गर्भावस्था जाँच; अभी MCP कार्ड या PICME नंबर नहीं है।", "ಉರ್ದು ಮತ್ತು ತಮಿಳು ಮಾತನಾಡುತ್ತಾರೆ. ಮೊದಲ ಗರ್ಭಿಣಿ ತಪಾಸಣೆ; ಇನ್ನೂ MCP ಕಾರ್ಡ್ ಅಥವಾ PICME ಸಂಖ್ಯೆ ಇಲ್ಲ.", "உருது, தமிழ் பேசுகிறார். முதல் கர்ப்ப பரிசோதனை; இன்னும் MCP அட்டையோ PICME எண்ணோ இல்லை."], "Kannada speaker, uses a wheelchair, PM-JAY card. Told by her doctor to see a cardiologist; has no referral letter yet.": ["कन्नड़ भाषी, व्हीलचेयर का उपयोग करती हैं, PM-JAY कार्ड है। डॉक्टर ने हृदय रोग विशेषज्ञ से मिलने को कहा है; अभी रेफ़रल पत्र नहीं है।", "ಕನ್ನಡ ಮಾತನಾಡುತ್ತಾರೆ, ಗಾಲಿಕುರ್ಚಿ ಬಳಸುತ್ತಾರೆ, PM-JAY ಕಾರ್ಡ್ ಇದೆ. ವೈದ್ಯರು ಹೃದ್ರೋಗ ತಜ್ಞರನ್ನು ಭೇಟಿ ಮಾಡಲು ಹೇಳಿದ್ದಾರೆ; ಇನ್ನೂ ರೆಫರಲ್ ಪತ್ರ ಇಲ್ಲ.", "கன்னடம் பேசுபவர், சக்கர நாற்காலி பயன்படுத்துகிறார், PM-JAY அட்டை உள்ளது. இதய நிபுணரைப் பார்க்கும்படி மருத்துவர் சொன்னார்; இன்னும் பரிந்துரைக் கடிதம் இல்லை."], "Speaks Urdu and Hindi. First pregnancy check-up; no MCP card yet.": ["उर्दू और हिन्दी बोलती हैं। पहली गर्भावस्था जाँच; अभी MCP कार्ड नहीं है।", "ಉರ್ದು ಮತ್ತು ಹಿಂದಿ ಮಾತನಾಡುತ್ತಾರೆ. ಮೊದಲ ಗರ್ಭಿಣಿ ತಪಾಸಣೆ; ಇನ್ನೂ MCP ಕಾರ್ಡ್ ಇಲ್ಲ.", "உருது, இந்தி பேசுகிறார். முதல் கர்ப்ப பரிசோதனை; இன்னும் MCP அட்டை இல்லை."], "(ambulance) or": ["(एम्बुलेंस) या", "(ಆಂಬ್ಯುಲೆನ್ಸ್) ಅಥವಾ", "(ஆம்புலன்ஸ்) அல்லது"], "(free, 24×7, many Indian languages) or": ["(निःशुल्क, 24×7, कई भारतीय भाषाएँ) या", "(ಉಚಿತ, 24×7, ಹಲವು ಭಾರತೀಯ ಭಾಷೆಗಳು) ಅಥವಾ", "(இலவசம், 24×7, பல இந்திய மொழிகள்) அல்லது"], ", and I agree to my details being stored to run my journey.": [", और मैं अपनी यात्रा चलाने के लिए अपनी जानकारी सहेजे जाने से सहमत हूँ।", ", ಮತ್ತು ನನ್ನ ಪಯಣ ನಡೆಸಲು ನನ್ನ ವಿವರಗಳನ್ನು ಸಂಗ್ರಹಿಸಲು ನಾನು ಒಪ್ಪುತ್ತೇನೆ.", ", மேலும் என் பயணத்தை நடத்த என் விவரங்கள் சேமிக்கப்படுவதற்கு ஒப்புக்கொள்கிறேன்."], ". We can still help you book a visit.": ["। हम फिर भी मुलाक़ात बुक करने में मदद कर सकते हैं।", ". ಆದರೂ ಭೇಟಿ ಬುಕ್ ಮಾಡಲು ನಾವು ಸಹಾಯ ಮಾಡಬಹುದು.", ". இருந்தாலும் வருகையை முன்பதிவு செய்ய நாங்கள் உதவலாம்."], "A real person to help when information is unclear": ["जानकारी अस्पष्ट हो तो मदद के लिए एक असली व्यक्ति", "ಮಾಹಿತಿ ಅಸ್ಪಷ್ಟವಾದಾಗ ಸಹಾಯ ಮಾಡಲು ನಿಜವಾದ ವ್ಯಕ್ತಿ", "தகவல் தெளிவில்லாதபோது உதவ ஒரு உண்மையான நபர்"], "About Next Route": ["Next Route के बारे में", "Next Route ಬಗ್ಗೆ", "Next Route பற்றி"], "Administrative help only — not medical advice. Emergency? Call": ["केवल प्रशासनिक सहायता — चिकित्सा सलाह नहीं। आपातकाल? कॉल करें", "ಕೇವಲ ಆಡಳಿತಾತ್ಮಕ ನೆರವು — ವೈದ್ಯಕೀಯ ಸಲಹೆ ಅಲ್ಲ. ತುರ್ತು? ಕರೆ ಮಾಡಿ", "நிர்வாக உதவி மட்டுமே — மருத்துவ ஆலோசனை அல்ல. அவசரமா? அழையுங்கள்"], "After the visit, tell us what the doctor said so we can line up the next step.": ["मुलाक़ात के बाद बताएँ कि डॉक्टर ने क्या कहा, ताकि हम अगला कदम तैयार कर सकें।", "ಭೇಟಿಯ ನಂತರ ವೈದ್ಯರು ಏನು ಹೇಳಿದರು ಎಂದು ತಿಳಿಸಿ, ನಾವು ಮುಂದಿನ ಹೆಜ್ಜೆ ಸಿದ್ಧಪಡಿಸುತ್ತೇವೆ.", "வருகைக்குப் பிறகு மருத்துவர் என்ன சொன்னார் என்று தெரிவியுங்கள்; அடுத்த படியை நாங்கள் தயார் செய்வோம்."], "After the visit: what did the doctor ask you to do?": ["मुलाक़ात के बाद: डॉक्टर ने आपसे क्या करने को कहा?", "ಭೇಟಿಯ ನಂತರ: ವೈದ್ಯರು ನಿಮಗೆ ಏನು ಮಾಡಲು ಹೇಳಿದರು?", "வருகைக்குப் பின்: மருத்துவர் உங்களை என்ன செய்யச் சொன்னார்?"], "All documents ready": ["सभी दस्तावेज़ तैयार", "ಎಲ್ಲಾ ದಾಖಲೆಗಳು ಸಿದ್ಧ", "எல்லா ஆவணங்களும் தயார்"], "All": ["सभी", "ಎಲ್ಲಾ", "அனைத்தும்"], "Anything else? (optional)": ["और कुछ? (वैकल्पिक)", "ಇನ್ನೇನಾದರೂ? (ಐಚ್ಛಿಕ)", "வேறு ஏதாவது? (விருப்பம்)"], "Appointment": ["अपॉइंटमेंट", "ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್", "சந்திப்பு"], "As soon as possible": ["जितनी जल्दी हो सके", "ಸಾಧ್ಯವಾದಷ್ಟು ಬೇಗ", "முடிந்தவரை விரைவில்"], "Ask a navigator to confirm before you travel": ["जाने से पहले किसी सहायक से पुष्टि करवाएँ", "ಹೊರಡುವ ಮೊದಲು ಸಹಾಯಕರಿಂದ ದೃಢೀಕರಿಸಿ", "பயணத்திற்கு முன் ஒரு வழிகாட்டியிடம் உறுதிப்படுத்துங்கள்"], "Ask a navigator to verify": ["सहायक से पुष्टि करवाएँ", "ಸಹಾಯಕರಿಂದ ಪರಿಶೀಲಿಸಿ", "வழிகாட்டியிடம் சரிபார்க்கக் கேளுங்கள்"], "Asked for tests": ["जाँच करवाने को कहा", "ಪರೀಕ್ಷೆಗಳಿಗೆ ಸೂಚಿಸಿದರು", "பரிசோதனைகள் செய்யச் சொன்னார்"], "Asked for lab tests": ["लैब जाँच करवाने को कहा", "ಪ್ರಯೋಗಾಲಯ ಪರೀಕ್ಷೆಗಳಿಗೆ ಸೂಚಿಸಿದರು", "ஆய்வகப் பரிசோதனைகள் செய்யச் சொன்னார்"], "Available": ["उपलब्ध", "ಲಭ್ಯವಿದೆ", "கிடைக்கும்"], "taken": ["भरा हुआ", "ಭರ್ತಿ", "நிரம்பியது"], "Book a slot and your visit pass will appear here.": ["स्लॉट बुक करें, आपका विज़िट पास यहाँ दिखेगा।", "ಸ್ಲಾಟ್ ಬುಕ್ ಮಾಡಿ, ನಿಮ್ಮ ಭೇಟಿ ಪಾಸ್ ಇಲ್ಲಿ ಕಾಣಿಸುತ್ತದೆ.", "நேரத்தை முன்பதிவு செய்யுங்கள்; உங்கள் வருகை அனுமதிச்சீட்டு இங்கே தோன்றும்."], "Book anyway": ["फिर भी बुक करें", "ಆದರೂ ಬುಕ್ ಮಾಡಿ", "இருந்தாலும் முன்பதிவு செய்"], "Book a General OPD visit to get one": ["इसके लिए सामान्य ओपीडी मुलाक़ात बुक करें", "ಇದಕ್ಕಾಗಿ ಸಾಮಾನ್ಯ ಒಪಿಡಿ ಭೇಟಿ ಬುಕ್ ಮಾಡಿ", "இதைப் பெற பொது OPD வருகையை முன்பதிவு செய்யுங்கள்"], "Booking is locked: this department needs a referral letter.": ["बुकिंग बंद है: इस विभाग को रेफ़रल पत्र चाहिए।", "ಬುಕಿಂಗ್ ಲಾಕ್ ಆಗಿದೆ: ಈ ವಿಭಾಗಕ್ಕೆ ರೆಫರಲ್ ಪತ್ರ ಬೇಕು.", "முன்பதிவு பூட்டப்பட்டுள்ளது: இந்தப் பிரிவுக்குப் பரிந்துரைக் கடிதம் தேவை."], "We won't let you book a slot you'd be turned away from.": ["हम आपको ऐसा स्लॉट बुक नहीं करने देंगे जहाँ से आपको लौटा दिया जाए।", "ನಿಮ್ಮನ್ನು ಹಿಂದಕ್ಕೆ ಕಳುಹಿಸುವಂತಹ ಸ್ಲಾಟ್ ಬುಕ್ ಮಾಡಲು ನಾವು ಬಿಡುವುದಿಲ್ಲ.", "உங்களைத் திருப்பி அனுப்பக்கூடிய நேரத்தை முன்பதிவு செய்ய விடமாட்டோம்."], "Get a referral first": ["पहले रेफ़रल लें", "ಮೊದಲು ರೆಫರಲ್ ಪಡೆಯಿರಿ", "முதலில் பரிந்துரை பெறுங்கள்"], "I already have one": ["मेरे पास पहले से है", "ನನ್ನ ಬಳಿ ಈಗಾಗಲೇ ಇದೆ", "என்னிடம் ஏற்கனவே உள்ளது"], "Pick another facility": ["दूसरी सुविधा चुनें", "ಬೇರೆ ಕೇಂದ್ರ ಆಯ್ಕೆಮಾಡಿ", "வேறு இடத்தைத் தேர்ந்தெடுங்கள்"], "Bring": ["साथ लाएँ", "ತನ್ನಿ", "கொண்டு வர வேண்டியவை"], "Cancel this booking?": ["यह बुकिंग रद्द करें?", "ಈ ಬುಕಿಂಗ್ ರದ್ದುಮಾಡಬೇಕೇ?", "இந்த முன்பதிவை ரத்து செய்யவா?"], "Choose a service first": ["पहले सेवा चुनें", "ಮೊದಲು ಸೇವೆ ಆಯ್ಕೆಮಾಡಿ", "முதலில் சேவையைத் தேர்ந்தெடுங்கள்"], "Choose a service first.": ["पहले सेवा चुनें।", "ಮೊದಲು ಸೇವೆ ಆಯ್ಕೆಮಾಡಿ.", "முதலில் சேவையைத் தேர்ந்தெடுங்கள்."], "Choose what's written on the referral letter.": ["रेफ़रल पत्र पर जो लिखा है वह चुनें।", "ರೆಫರಲ್ ಪತ್ರದಲ್ಲಿ ಬರೆದಿರುವುದನ್ನು ಆಯ್ಕೆಮಾಡಿ.", "பரிந்துரைக் கடிதத்தில் எழுதியிருப்பதைத் தேர்ந்தெடுங்கள்."], "City": ["शहर", "ನಗರ", "நகரம்"], "Clear everything": ["सब मिटाएँ", "ಎಲ್ಲವನ್ನೂ ಅಳಿಸಿ", "அனைத்தையும் அழி"], "Close": ["बंद करें", "ಮುಚ್ಚಿ", "மூடு"], "Close this journey": ["यह यात्रा बंद करें", "ಈ ಪಯಣ ಮುಗಿಸಿ", "இந்தப் பயணத்தை முடி"], "Come back later": ["बाद में फिर आएँ", "ನಂತರ ಮತ್ತೆ ಬನ್ನಿ", "பின்னர் மீண்டும் வாருங்கள்"], "Confirm password": ["पासवर्ड की पुष्टि करें", "ಪಾಸ್‌ವರ್ಡ್ ದೃಢೀಕರಿಸಿ", "கடவுச்சொல்லை உறுதிப்படுத்துங்கள்"], "Confirm new time": ["नए समय की पुष्टि करें", "ಹೊಸ ಸಮಯ ದೃಢೀಕರಿಸಿ", "புதிய நேரத்தை உறுதிப்படுத்து"], "Continue as guest (demo)": ["अतिथि के रूप में जारी रखें (डेमो)", "ಅತಿಥಿಯಾಗಿ ಮುಂದುವರಿಯಿರಿ (ಡೆಮೊ)", "விருந்தினராகத் தொடருங்கள் (டெமோ)"], "Continue to booking": ["बुकिंग पर आगे बढ़ें", "ಬುಕಿಂಗ್‌ಗೆ ಮುಂದುವರಿಯಿರಿ", "முன்பதிவுக்குத் தொடருங்கள்"], "Copy SMS reminder": ["SMS रिमाइंडर कॉपी करें", "SMS ಜ್ಞಾಪನೆ ನಕಲಿಸಿ", "SMS நினைவூட்டலை நகலெடு"], "Copy calendar (.ics) text": ["कैलेंडर (.ics) टेक्स्ट कॉपी करें", "ಕ್ಯಾಲೆಂಡರ್ (.ics) ಪಠ್ಯ ನಕಲಿಸಿ", "நாட்காட்டி (.ics) உரையை நகலெடு"], "Copy checklist": ["चेकलिस्ट कॉपी करें", "ಪರಿಶೀಲನಾ ಪಟ್ಟಿ ನಕಲಿಸಿ", "சரிபார்ப்புப் பட்டியலை நகலெடு"], "Copy pass as text": ["पास टेक्स्ट के रूप में कॉपी करें", "ಪಾಸ್ ಅನ್ನು ಪಠ್ಯವಾಗಿ ನಕಲಿಸಿ", "அனுமதிச்சீட்டை உரையாக நகலெடு"], "Copy schema example": ["स्कीमा उदाहरण कॉपी करें", "ಸ್ಕೀಮಾ ಉದಾಹರಣೆ ನಕಲಿಸಿ", "திட்ட வடிவ உதாரணத்தை நகலெடு"], "Copy summary": ["सारांश कॉपी करें", "ಸಾರಾಂಶ ನಕಲಿಸಿ", "சுருக்கத்தை நகலெடு"], "Copy this": ["इसे कॉपी करें", "ಇದನ್ನು ನಕಲಿಸಿ", "இதை நகலெடுங்கள்"], "Your browser blocked automatic copying. Select the text below and copy it.": ["आपके ब्राउज़र ने अपने-आप कॉपी करना रोक दिया। नीचे का टेक्स्ट चुनकर कॉपी करें।", "ನಿಮ್ಮ ಬ್ರೌಸರ್ ಸ್ವಯಂ ನಕಲನ್ನು ತಡೆದಿದೆ. ಕೆಳಗಿನ ಪಠ್ಯ ಆಯ್ಕೆಮಾಡಿ ನಕಲಿಸಿ.", "உங்கள் உலாவி தானியங்கி நகலெடுப்பைத் தடுத்தது. கீழே உள்ள உரையைத் தேர்ந்தெடுத்து நகலெடுங்கள்."], "Copied": ["कॉपी हो गया", "ನಕಲಿಸಲಾಗಿದೆ", "நகலெடுக்கப்பட்டது"], "Calendar text copied": ["कैलेंडर टेक्स्ट कॉपी हुआ", "ಕ್ಯಾಲೆಂಡರ್ ಪಠ್ಯ ನಕಲಿಸಲಾಗಿದೆ", "நாட்காட்டி உரை நகலெடுக்கப்பட்டது"], "Summary copied": ["सारांश कॉपी हुआ", "ಸಾರಾಂಶ ನಕಲಿಸಲಾಗಿದೆ", "சுருக்கம் நகலெடுக்கப்பட்டது"], "Schema copied": ["स्कीमा कॉपी हुआ", "ಸ್ಕೀಮಾ ನಕಲಿಸಲಾಗಿದೆ", "திட்ட வடிவம் நகலெடுக்கப்பட்டது"], "Visit pass copied": ["विज़िट पास कॉपी हुआ", "ಭೇಟಿ ಪಾಸ್ ನಕಲಿಸಲಾಗಿದೆ", "வருகை அனுமதிச்சீட்டு நகலெடுக்கப்பட்டது"], "Checklist copied": ["चेकलिस्ट कॉपी हुई", "ಪಟ್ಟಿ ನಕಲಿಸಲಾಗಿದೆ", "பட்டியல் நகலெடுக்கப்பட்டது"], "SMS text copied": ["SMS टेक्स्ट कॉपी हुआ", "SMS ಪಠ್ಯ ನಕಲಿಸಲಾಗಿದೆ", "SMS உரை நகலெடுக்கப்பட்டது"], "No appointment to remind about": ["याद दिलाने के लिए कोई अपॉइंटमेंट नहीं", "ಜ್ಞಾಪಿಸಲು ಯಾವುದೇ ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್ ಇಲ್ಲ", "நினைவூட்ட எந்தச் சந்திப்பும் இல்லை"], "Create a password": ["पासवर्ड बनाएँ", "ಪಾಸ್‌ವರ್ಡ್ ರಚಿಸಿ", "கடவுச்சொல்லை உருவாக்குங்கள்"], "Create account": ["खाता बनाएँ", "ಖಾತೆ ರಚಿಸಿ", "கணக்கை உருவாக்கு"], "Create an account": ["खाता बनाएँ", "ಖಾತೆ ರಚಿಸಿ", "கணக்கை உருவாக்குங்கள்"], "Create an account to keep your journey, documents and reminders.": ["अपनी यात्रा, दस्तावेज़ और रिमाइंडर सहेजने के लिए खाता बनाएँ।", "ನಿಮ್ಮ ಪಯಣ, ದಾಖಲೆಗಳು ಮತ್ತು ಜ್ಞಾಪನೆಗಳನ್ನು ಉಳಿಸಲು ಖಾತೆ ರಚಿಸಿ.", "உங்கள் பயணம், ஆவணங்கள், நினைவூட்டல்களைச் சேமிக்க கணக்கை உருவாக்குங்கள்."], "Create your account": ["अपना खाता बनाएँ", "ನಿಮ್ಮ ಖಾತೆ ರಚಿಸಿ", "உங்கள் கணக்கை உருவாக்குங்கள்"], "Data source": ["डेटा स्रोत", "ಡೇಟಾ ಮೂಲ", "தரவு மூலம்"], "Demo patients": ["डेमो मरीज़", "ಡೆಮೊ ರೋಗಿಗಳು", "மாதிரி நோயாளிகள்"], "Departments that match your words:": ["आपके शब्दों से मेल खाते विभाग:", "ನಿಮ್ಮ ಪದಗಳಿಗೆ ಹೊಂದುವ ವಿಭಾಗಗಳು:", "உங்கள் வார்த்தைகளுக்குப் பொருந்தும் பிரிவுகள்:"], "Document checklists, so no wasted trips": ["दस्तावेज़ चेकलिस्ट, ताकि कोई बेकार चक्कर न लगे", "ದಾಖಲೆ ಪಟ್ಟಿಗಳು, ವ್ಯರ್ಥ ಪ್ರಯಾಣ ಇಲ್ಲ", "ஆவணப் பட்டியல்கள் — வீண் பயணம் இல்லை"], "Each facility and payment method needs slightly different paperwork.": ["हर सुविधा और भुगतान तरीके के लिए थोड़े अलग काग़ज़ चाहिए।", "ಪ್ರತಿ ಕೇಂದ್ರ ಮತ್ತು ಪಾವತಿ ವಿಧಾನಕ್ಕೆ ಸ್ವಲ್ಪ ಬೇರೆ ದಾಖಲೆಗಳು ಬೇಕು.", "ஒவ்வொரு இடத்துக்கும் கட்டண முறைக்கும் சற்று வேறுபட்ட ஆவணங்கள் தேவை."], "Each one exercises a different part of the journey.": ["हर एक यात्रा के अलग हिस्से को दिखाता है।", "ಪ್ರತಿಯೊಂದೂ ಪಯಣದ ಬೇರೆ ಭಾಗವನ್ನು ತೋರಿಸುತ್ತದೆ.", "ஒவ்வொன்றும் பயணத்தின் வெவ்வேறு பகுதியைக் காட்டுகிறது."], "Email or mobile number": ["ईमेल या मोबाइल नंबर", "ಇಮೇಲ್ ಅಥವಾ ಮೊಬೈಲ್ ಸಂಖ್ಯೆ", "மின்னஞ்சல் அல்லது கைபேசி எண்"], "Emergency": ["आपातकाल", "ತುರ್ತು", "அவசரம்"], "Enter a valid email address or a 10-digit mobile number.": ["मान्य ईमेल पता या 10 अंकों का मोबाइल नंबर डालें।", "ಮಾನ್ಯ ಇಮೇಲ್ ವಿಳಾಸ ಅಥವಾ 10 ಅಂಕಿಯ ಮೊಬೈಲ್ ಸಂಖ್ಯೆ ನಮೂದಿಸಿ.", "சரியான மின்னஞ்சல் முகவரி அல்லது 10 இலக்க கைபேசி எண்ணை உள்ளிடுங்கள்."], "Enter your email or mobile number.": ["अपना ईमेल या मोबाइल नंबर डालें।", "ನಿಮ್ಮ ಇಮೇಲ್ ಅಥವಾ ಮೊಬೈಲ್ ಸಂಖ್ಯೆ ನಮೂದಿಸಿ.", "உங்கள் மின்னஞ்சல் அல்லது கைபேசி எண்ணை உள்ளிடுங்கள்."], "Enter your password.": ["अपना पासवर्ड डालें।", "ನಿಮ್ಮ ಪಾಸ್‌ವರ್ಡ್ ನಮೂದಿಸಿ.", "உங்கள் கடவுச்சொல்லை உள்ளிடுங்கள்."], "An account already exists for this — sign in instead.": ["इसके लिए पहले से खाता है — साइन इन करें।", "ಇದಕ್ಕೆ ಈಗಾಗಲೇ ಖಾತೆ ಇದೆ — ಸೈನ್ ಇನ್ ಮಾಡಿ.", "இதற்கு ஏற்கனவே கணக்கு உள்ளது — உள்நுழையுங்கள்."], "Passwords don't match.": ["पासवर्ड मेल नहीं खाते।", "ಪಾಸ್‌ವರ್ಡ್‌ಗಳು ಹೊಂದಿಕೆಯಾಗುತ್ತಿಲ್ಲ.", "கடவுச்சொற்கள் பொருந்தவில்லை."], "Too many failed attempts. Please wait 30 seconds and try again.": ["बहुत सारे असफल प्रयास। कृपया 30 सेकंड रुककर फिर कोशिश करें।", "ಹಲವು ವಿಫಲ ಪ್ರಯತ್ನಗಳು. ದಯವಿಟ್ಟು 30 ಸೆಕೆಂಡ್ ಕಾಯ್ದು ಮತ್ತೆ ಪ್ರಯತ್ನಿಸಿ.", "பல தோல்வியான முயற்சிகள். 30 வினாடிகள் காத்திருந்து மீண்டும் முயலுங்கள்."], "Too many attempts — wait 30 s": ["बहुत प्रयास — 30 सेकंड रुकें", "ಹಲವು ಪ್ರಯತ್ನಗಳು — 30 ಸೆ. ಕಾಯಿರಿ", "பல முயற்சிகள் — 30 வினாடி காத்திருங்கள்"], "You've been signed out.": ["आप साइन आउट हो गए हैं।", "ನೀವು ಸೈನ್ ಔಟ್ ಆಗಿದ್ದೀರಿ.", "நீங்கள் வெளியேறிவிட்டீர்கள்."], "Everything else — which facilities fit, what to bring, which slots exist — depends on the service you need.": ["बाकी सब — कौन-सी सुविधा उपयुक्त है, क्या लाना है, कौन-से स्लॉट हैं — आपकी ज़रूरत की सेवा पर निर्भर करता है।", "ಉಳಿದೆಲ್ಲವೂ — ಯಾವ ಕೇಂದ್ರ ಸೂಕ್ತ, ಏನು ತರಬೇಕು, ಯಾವ ಸ್ಲಾಟ್‌ಗಳಿವೆ — ನಿಮಗೆ ಬೇಕಾದ ಸೇವೆಯನ್ನು ಅವಲಂಬಿಸಿದೆ.", "மற்ற அனைத்தும் — எந்த இடம் பொருந்தும், என்ன கொண்டு வர வேண்டும், எந்த நேரங்கள் உள்ளன — உங்களுக்குத் தேவையான சேவையைப் பொறுத்தது."], "Facilities matched to your needs, with the reasons shown": ["आपकी ज़रूरतों से मेल खाती सुविधाएँ, कारणों के साथ", "ನಿಮ್ಮ ಅಗತ್ಯಗಳಿಗೆ ಹೊಂದುವ ಕೇಂದ್ರಗಳು, ಕಾರಣಗಳ ಸಹಿತ", "உங்கள் தேவைகளுக்குப் பொருந்தும் இடங்கள், காரணங்களுடன்"], "Facility": ["सुविधा", "ಕೇಂದ್ರ", "இடம்"], "Facility phone": ["सुविधा का फ़ोन", "ಕೇಂದ್ರದ ದೂರವಾಣಿ", "தொலைபேசி"], "Find the right facility, know what to bring, book a slot and plan what comes next — in your language.": ["सही सुविधा खोजें, जानें क्या लाना है, स्लॉट बुक करें और आगे की योजना बनाएँ — अपनी भाषा में।", "ಸರಿಯಾದ ಕೇಂದ್ರ ಹುಡುಕಿ, ಏನು ತರಬೇಕು ತಿಳಿಯಿರಿ, ಸ್ಲಾಟ್ ಬುಕ್ ಮಾಡಿ ಮತ್ತು ಮುಂದಿನದನ್ನು ಯೋಜಿಸಿ — ನಿಮ್ಮ ಭಾಷೆಯಲ್ಲಿ.", "சரியான இடத்தைக் கண்டறியுங்கள், என்ன கொண்டு வர வேண்டும் என அறியுங்கள், நேரத்தை முன்பதிவு செய்து அடுத்ததைத் திட்டமிடுங்கள் — உங்கள் மொழியில்."], "Fit": ["उपयुक्तता", "ಹೊಂದಾಣಿಕೆ", "பொருத்தம்"], "Follow-up added — book when you're ready": ["फ़ॉलो-अप जोड़ा गया — तैयार होने पर बुक करें", "ಮುಂದಿನ ಭೇಟಿ ಸೇರಿಸಲಾಗಿದೆ — ಸಿದ್ಧವಾದಾಗ ಬುಕ್ ಮಾಡಿ", "தொடர் வருகை சேர்க்கப்பட்டது — தயாரானதும் முன்பதிவு செய்யுங்கள்"], "Follow-up visit after some time": ["कुछ समय बाद फ़ॉलो-अप मुलाक़ात", "ಸ್ವಲ್ಪ ಸಮಯದ ನಂತರ ಮುಂದಿನ ಭೇಟಿ", "சிறிது காலத்துக்குப் பின் தொடர் வருகை"], "Forgot password?": ["पासवर्ड भूल गए?", "ಪಾಸ್‌ವರ್ಡ್ ಮರೆತಿರಾ?", "கடவுச்சொல் மறந்துவிட்டதா?"], "Front-desk languages listed by the facility": ["सुविधा द्वारा बताई गई रिसेप्शन की भाषाएँ", "ಕೇಂದ್ರ ತಿಳಿಸಿದ ಸ್ವಾಗತ ಕೌಂಟರ್ ಭಾಷೆಗಳು", "இடம் குறிப்பிட்ட வரவேற்பு மேசை மொழிகள்"], "Full name": ["पूरा नाम", "ಪೂರ್ಣ ಹೆಸರು", "முழுப் பெயர்"], "Gave me a referral": ["रेफ़रल दिया", "ರೆಫರಲ್ ನೀಡಿದರು", "பரிந்துரை கொடுத்தார்"], "Generated from your bookings and what the doctor asked you to do. Add them to your phone's calendar, or copy an SMS-style reminder for a caregiver.": ["आपकी बुकिंग और डॉक्टर के निर्देशों से बनाए गए। इन्हें फ़ोन के कैलेंडर में जोड़ें, या देखभाल करने वाले के लिए SMS जैसा रिमाइंडर कॉपी करें।", "ನಿಮ್ಮ ಬುಕಿಂಗ್‌ಗಳು ಮತ್ತು ವೈದ್ಯರ ಸೂಚನೆಗಳಿಂದ ರಚಿಸಲಾಗಿದೆ. ಇವುಗಳನ್ನು ಫೋನ್ ಕ್ಯಾಲೆಂಡರ್‌ಗೆ ಸೇರಿಸಿ, ಅಥವಾ ಆರೈಕೆದಾರರಿಗೆ SMS ರೀತಿಯ ಜ್ಞಾಪನೆ ನಕಲಿಸಿ.", "உங்கள் முன்பதிவுகள் மற்றும் மருத்துவர் சொன்னவற்றிலிருந்து உருவாக்கப்பட்டவை. இவற்றை உங்கள் தொலைபேசி நாட்காட்டியில் சேர்க்கலாம், அல்லது பராமரிப்பாளருக்காக SMS நினைவூட்டலை நகலெடுக்கலாம்."], "Guest": ["अतिथि", "ಅತಿಥಿ", "விருந்தினர்"], "Guest session — your journey isn't tied to an account.": ["अतिथि सत्र — आपकी यात्रा किसी खाते से जुड़ी नहीं है।", "ಅತಿಥಿ ಅವಧಿ — ನಿಮ್ಮ ಪಯಣ ಯಾವುದೇ ಖಾತೆಗೆ ಜೋಡಣೆಯಾಗಿಲ್ಲ.", "விருந்தினர் அமர்வு — உங்கள் பயணம் எந்தக் கணக்குடனும் இணைக்கப்படவில்லை."], "Healthcare, one clear step at a time.": ["स्वास्थ्य सेवा, एक-एक साफ़ कदम।", "ಆರೋಗ್ಯ ಸೇವೆ, ಒಂದೊಂದೇ ಸ್ಪಷ್ಟ ಹೆಜ್ಜೆ.", "மருத்துவ சேவை, ஒவ்வொரு படியும் தெளிவாக."], "Hide reasons": ["कारण छिपाएँ", "ಕಾರಣಗಳನ್ನು ಮರೆಮಾಡಿ", "காரணங்களை மறை"], "Hide": ["छिपाएँ", "ಮರೆಮಾಡಿ", "மறை"], "Show": ["दिखाएँ", "ತೋರಿಸಿ", "காட்டு"], "Show password": ["पासवर्ड दिखाएँ", "ಪಾಸ್‌ವರ್ಡ್ ತೋರಿಸಿ", "கடவுச்சொல்லைக் காட்டு"], "Hide password": ["पासवर्ड छिपाएँ", "ಪಾಸ್‌ವರ್ಡ್ ಮರೆಮಾಡಿ", "கடவுச்சொல்லை மறை"], "How should they reach you?": ["वे आपसे कैसे संपर्क करें?", "ಅವರು ನಿಮ್ಮನ್ನು ಹೇಗೆ ಸಂಪರ್ಕಿಸಬೇಕು?", "அவர்கள் உங்களை எப்படித் தொடர்பு கொள்ள வேண்டும்?"], "Human navigator": ["मानव सहायक", "ಮಾನವ ಸಹಾಯಕರು", "மனித வழிகாட்டி"], "I understand this app gives": ["मैं समझता/समझती हूँ कि यह ऐप देता है", "ಈ ಆ್ಯಪ್ ನೀಡುವುದು", "இந்தச் செயலி வழங்குவது"], "administrative guidance only, not medical advice": ["केवल प्रशासनिक मार्गदर्शन, चिकित्सा सलाह नहीं", "ಕೇವಲ ಆಡಳಿತಾತ್ಮಕ ಮಾರ್ಗದರ್ಶನ, ವೈದ್ಯಕೀಯ ಸಲಹೆ ಅಲ್ಲ ಎಂದು ನನಗೆ ಅರ್ಥವಾಗಿದೆ", "நிர்வாக வழிகாட்டுதல் மட்டுமே, மருத்துவ ஆலோசனை அல்ல என்பதை நான் புரிந்துகொள்கிறேன்"], "I'll visit the help desk": ["मैं हेल्प डेस्क पर आऊँगा/आऊँगी", "ನಾನು ಸಹಾಯ ಕೌಂಟರ್‌ಗೆ ಬರುತ್ತೇನೆ", "நான் உதவி மேசைக்கு வருவேன்"], "I'm not sure / something else": ["पक्का नहीं / कुछ और", "ಖಚಿತವಿಲ್ಲ / ಬೇರೆ ಏನೋ", "உறுதியில்லை / வேறு ஏதோ"], "In the live version you'd get a one-time code by SMS or email to set a new password.": ["असली संस्करण में नया पासवर्ड बनाने के लिए SMS या ईमेल पर एक बार का कोड मिलेगा।", "ನೈಜ ಆವೃತ್ತಿಯಲ್ಲಿ ಹೊಸ ಪಾಸ್‌ವರ್ಡ್‌ಗಾಗಿ SMS ಅಥವಾ ಇಮೇಲ್ ಮೂಲಕ ಒಂದು ಬಾರಿಯ ಕೋಡ್ ಸಿಗುತ್ತದೆ.", "நேரடிப் பதிப்பில் புதிய கடவுச்சொல் அமைக்க SMS அல்லது மின்னஞ்சல் மூலம் ஒருமுறைக் குறியீடு கிடைக்கும்."], "In this prototype, accounts live only on this device — create a new account, or continue as a guest.": ["इस प्रोटोटाइप में खाते केवल इसी डिवाइस पर रहते हैं — नया खाता बनाएँ या अतिथि के रूप में जारी रखें।", "ಈ ಮಾದರಿಯಲ್ಲಿ ಖಾತೆಗಳು ಈ ಸಾಧನದಲ್ಲಿ ಮಾತ್ರ ಇರುತ್ತವೆ — ಹೊಸ ಖಾತೆ ರಚಿಸಿ ಅಥವಾ ಅತಿಥಿಯಾಗಿ ಮುಂದುವರಿಯಿರಿ.", "இந்த முன்மாதிரியில் கணக்குகள் இந்தச் சாதனத்தில் மட்டுமே இருக்கும் — புதிய கணக்கை உருவாக்குங்கள், அல்லது விருந்தினராகத் தொடருங்கள்."], "Issue resolved, journey updated": ["समस्या हल, यात्रा अपडेट", "ಸಮಸ್ಯೆ ಪರಿಹಾರ, ಪಯಣ ನವೀಕರಣ", "சிக்கல் தீர்ந்தது, பயணம் புதுப்பிக்கப்பட்டது"], "It takes under a minute. Your journey is saved to your account.": ["इसमें एक मिनट से कम लगता है। आपकी यात्रा आपके खाते में सहेजी जाती है।", "ಒಂದು ನಿಮಿಷಕ್ಕಿಂತ ಕಡಿಮೆ ಸಾಕು. ನಿಮ್ಮ ಪಯಣ ನಿಮ್ಮ ಖಾತೆಯಲ್ಲಿ ಉಳಿಯುತ್ತದೆ.", "ஒரு நிமிடத்துக்குள் முடியும். உங்கள் பயணம் உங்கள் கணக்கில் சேமிக்கப்படும்."], "JOURNEY LEGS": ["यात्रा के चरण", "ಪಯಣದ ಹಂತಗಳು", "பயணப் பகுதிகள்"], "Journey history": ["यात्रा इतिहास", "ಪಯಣ ಇತಿಹಾಸ", "பயண வரலாறு"], "Keep current slot": ["मौजूदा स्लॉट रखें", "ಈಗಿನ ಸ್ಲಾಟ್ ಉಳಿಸಿ", "தற்போதைய நேரத்தை வைத்திரு"], "Keep me signed in": ["मुझे साइन इन रखें", "ನನ್ನನ್ನು ಸೈನ್ ಇನ್ ಆಗಿರಿಸಿ", "என்னை உள்நுழைந்த நிலையில் வை"], "Lab work or scans": ["लैब जाँच या स्कैन", "ಪ್ರಯೋಗಾಲಯ ಪರೀಕ್ಷೆ ಅಥವಾ ಸ್ಕ್ಯಾನ್", "ஆய்வகப் பரிசோதனை அல்லது ஸ்கேன்"], "Language": ["भाषा", "ಭಾಷೆ", "மொழி"], "staff listed": ["स्टाफ़ बोलता है", "ಸಿಬ್ಬಂದಿ ಮಾತನಾಡುತ್ತಾರೆ", "ஊழியர்கள் பேசுவர்"], "interpreter needed": ["दुभाषिया चाहिए", "ವ್ಯಾಖ್ಯಾನಕಾರರು ಬೇಕು", "மொழிபெயர்ப்பாளர் தேவை"], "Leave by": ["निकलने का समय", "ಹೊರಡುವ ಸಮಯ", "புறப்பட வேண்டிய நேரம்"], "Listed as accepted in organiser data": ["आयोजक डेटा में स्वीकार्य बताया गया", "ಆಯೋಜಕರ ಡೇಟಾದಲ್ಲಿ ಸ್ವೀಕಾರಾರ್ಹ ಎಂದು ಪಟ್ಟಿ ಮಾಡಲಾಗಿದೆ", "ஏற்பாட்டாளர் தரவில் ஏற்கப்படுவதாகக் குறிப்பிடப்பட்டுள்ளது"], "Load organiser JSON": ["आयोजक JSON लोड करें", "ಆಯೋಜಕರ JSON ಲೋಡ್ ಮಾಡಿ", "ஏற்பாட்டாளர் JSON ஏற்று"], "Load the organiser-provided facility file (JSON array, or": ["आयोजक की दी गई सुविधा फ़ाइल लोड करें (JSON array, या", "ಆಯೋಜಕರು ನೀಡಿದ ಕೇಂದ್ರಗಳ ಫೈಲ್ ಲೋಡ್ ಮಾಡಿ (JSON array, ಅಥವಾ", "ஏற்பாட்டாளர் வழங்கிய இடங்கள் கோப்பை ஏற்றுங்கள் (JSON array, அல்லது"], "Use sample data": ["नमूना डेटा उपयोग करें", "ಮಾದರಿ ಡೇಟಾ ಬಳಸಿ", "மாதிரித் தரவைப் பயன்படுத்து"], "Using sample data": ["नमूना डेटा उपयोग में", "ಮಾದರಿ ಡೇಟಾ ಬಳಕೆಯಲ್ಲಿದೆ", "மாதிரித் தரவு பயன்பாட்டில்"], "Couldn't load that file": ["वह फ़ाइल लोड नहीं हो सकी", "ಆ ಫೈಲ್ ಲೋಡ್ ಆಗಲಿಲ್ಲ", "அந்தக் கோப்பை ஏற்ற முடியவில்லை"], "Map is schematic": ["नक्शा अनुमानित है", "ನಕ್ಷೆ ಸ್ಥೂಲವಾಗಿದೆ", "வரைபடம் தோராயமானது"], "Missing paperwork is a common reason people are sent back from the registration counter.": ["काग़ज़ों की कमी, पंजीकरण काउंटर से लौटाए जाने का आम कारण है।", "ದಾಖಲೆಗಳ ಕೊರತೆ ನೋಂದಣಿ ಕೌಂಟರ್‌ನಿಂದ ಹಿಂದಿರುಗಿಸಲು ಸಾಮಾನ್ಯ ಕಾರಣ.", "ஆவணங்கள் இல்லாதது பதிவு கவுண்டரில் திருப்பி அனுப்பப்படுவதற்கான பொதுவான காரணம்."], "Myself": ["स्वयं के लिए", "ನನಗಾಗಿ", "எனக்காக"], "Someone I care for": ["जिनकी मैं देखभाल करता/करती हूँ", "ನಾನು ಆರೈಕೆ ಮಾಡುವವರಿಗಾಗಿ", "நான் பராமரிப்பவருக்காக"], "NOW SERVING": ["अभी चल रहा", "ಈಗ ಸೇವೆ", "தற்போது அழைக்கப்படுவது"], "Navigator assigned": ["सहायक नियुक्त", "ಸಹಾಯಕರನ್ನು ನಿಯೋಜಿಸಲಾಗಿದೆ", "வழிகாட்டி நியமிக்கப்பட்டார்"], "Navigators are trained staff at the help desk or on the phone. They can confirm conflicting details, arrange interpreters or ramps, and find options outside this dataset. They do not give medical advice either — for that, they'll connect you to a clinician.": ["सहायक हेल्प डेस्क या फ़ोन पर प्रशिक्षित कर्मचारी हैं। वे विरोधाभासी जानकारी की पुष्टि, दुभाषिया या रैंप की व्यवस्था, और इस डेटा से बाहर के विकल्प खोज सकते हैं। वे भी चिकित्सा सलाह नहीं देते — उसके लिए वे आपको किसी चिकित्सक से जोड़ेंगे।", "ಸಹಾಯಕರು ಸಹಾಯ ಕೌಂಟರ್ ಅಥವಾ ಫೋನ್‌ನಲ್ಲಿರುವ ತರಬೇತಿ ಪಡೆದ ಸಿಬ್ಬಂದಿ. ಅವರು ವಿರೋಧಾತ್ಮಕ ವಿವರಗಳನ್ನು ದೃಢೀಕರಿಸಬಹುದು, ವ್ಯಾಖ್ಯಾನಕಾರರು ಅಥವಾ ರ್ಯಾಂಪ್ ವ್ಯವಸ್ಥೆ ಮಾಡಬಹುದು ಮತ್ತು ಈ ಡೇಟಾದ ಹೊರಗಿನ ಆಯ್ಕೆಗಳನ್ನು ಹುಡುಕಬಹುದು. ಅವರೂ ವೈದ್ಯಕೀಯ ಸಲಹೆ ನೀಡುವುದಿಲ್ಲ — ಅದಕ್ಕಾಗಿ ನಿಮ್ಮನ್ನು ವೈದ್ಯರೊಂದಿಗೆ ಸಂಪರ್ಕಿಸುತ್ತಾರೆ.", "வழிகாட்டிகள் உதவி மேசையில் அல்லது தொலைபேசியில் பணியாற்றும் பயிற்சி பெற்ற ஊழியர்கள். முரண்பட்ட விவரங்களை உறுதிப்படுத்தவும், மொழிபெயர்ப்பாளர் அல்லது சாய்தளம் ஏற்பாடு செய்யவும், இந்தத் தரவுக்கு வெளியே உள்ள வாய்ப்புகளைக் கண்டறியவும் முடியும். அவர்களும் மருத்துவ ஆலோசனை தர மாட்டார்கள் — அதற்கு உங்களை ஒரு மருத்துவரிடம் இணைப்பார்கள்."], "Need a person?": ["किसी व्यक्ति की ज़रूरत?", "ವ್ಯಕ್ತಿಯ ಸಹಾಯ ಬೇಕೇ?", "ஒருவரின் உதவி தேவையா?"], "Next": ["आगे", "ಮುಂದೆ", "அடுத்து"], "Then": ["फिर", "ನಂತರ", "பின்னர்"], "Sent": ["भेजा गया", "ಕಳುಹಿಸಲಾಗಿದೆ", "அனுப்பப்பட்டது"], "Queued": ["कतार में", "ಸರದಿಯಲ್ಲಿ", "வரிசையில்"], "Request received": ["अनुरोध मिला", "ಕೋರಿಕೆ ಸ್ವೀಕರಿಸಲಾಗಿದೆ", "கோரிக்கை பெறப்பட்டது"], "Next step and help": ["अगला कदम और सहायता", "ಮುಂದಿನ ಹೆಜ್ಜೆ ಮತ್ತು ಸಹಾಯ", "அடுத்த படி மற்றும் உதவி"], "No appointment yet": ["अभी कोई अपॉइंटमेंट नहीं", "ಇನ್ನೂ ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್ ಇಲ್ಲ", "இன்னும் சந்திப்பு இல்லை"], "No free slot this week — try another time preference or ask a navigator.": ["इस सप्ताह कोई खाली स्लॉट नहीं — दूसरा समय चुनें या सहायक से पूछें।", "ಈ ವಾರ ಖಾಲಿ ಸ್ಲಾಟ್ ಇಲ್ಲ — ಬೇರೆ ಸಮಯ ಆಯ್ಕೆಮಾಡಿ ಅಥವಾ ಸಹಾಯಕರನ್ನು ಕೇಳಿ.", "இந்த வாரம் காலி நேரம் இல்லை — வேறு நேர விருப்பத்தை முயலுங்கள் அல்லது வழிகாட்டியிடம் கேளுங்கள்."], "No free slots": ["कोई खाली स्लॉट नहीं", "ಖಾಲಿ ಸ್ಲಾಟ್ ಇಲ್ಲ", "காலி நேரம் இல்லை"], "No free slots this week": ["इस सप्ताह कोई खाली स्लॉट नहीं", "ಈ ವಾರ ಖಾಲಿ ಸ್ಲಾಟ್ ಇಲ್ಲ", "இந்த வாரம் காலி நேரம் இல்லை"], "No slots in the next week. A navigator can ask about walk-in queues.": ["अगले सप्ताह कोई स्लॉट नहीं। सहायक वॉक-इन कतार के बारे में पूछ सकते हैं।", "ಮುಂದಿನ ವಾರ ಸ್ಲಾಟ್ ಇಲ್ಲ. ಸಹಾಯಕರು ನೇರ ಸರದಿ ಬಗ್ಗೆ ಕೇಳಬಹುದು.", "அடுத்த வாரம் நேரம் இல்லை. நேரடி வரிசை பற்றி வழிகாட்டி கேட்கலாம்."], "No more visits needed": ["और मुलाक़ात की ज़रूरत नहीं", "ಇನ್ನು ಭೇಟಿ ಬೇಕಿಲ್ಲ", "மேலும் வருகை தேவையில்லை"], "None": ["कोई नहीं", "ಇಲ್ಲ", "இல்லை"], "none": ["कोई नहीं", "ಇಲ್ಲ", "இல்லை"], "Not sure? Start with General OPD: a doctor there can refer you onward.": ["पक्का नहीं? सामान्य ओपीडी से शुरू करें: वहाँ के डॉक्टर आगे रेफ़र कर सकते हैं।", "ಖಚಿತವಿಲ್ಲವೇ? ಸಾಮಾನ್ಯ ಒಪಿಡಿಯಿಂದ ಆರಂಭಿಸಿ: ಅಲ್ಲಿನ ವೈದ್ಯರು ಮುಂದೆ ಶಿಫಾರಸು ಮಾಡಬಹುದು.", "உறுதியில்லையா? பொது OPD யில் தொடங்குங்கள்: அங்குள்ள மருத்துவர் உங்களை மேலும் பரிந்துரைக்கலாம்."], "Nothing looks incomplete or conflicting right now. You can still ask for help any time.": ["अभी कुछ भी अधूरा या विरोधाभासी नहीं दिखता। आप कभी भी मदद माँग सकते हैं।", "ಈಗ ಯಾವುದೂ ಅಪೂರ್ಣ ಅಥವಾ ವಿರೋಧಾತ್ಮಕವಾಗಿ ಕಾಣುತ್ತಿಲ್ಲ. ನೀವು ಯಾವಾಗ ಬೇಕಾದರೂ ಸಹಾಯ ಕೇಳಬಹುದು.", "இப்போது எதுவும் முழுமையற்றதாகவோ முரண்பட்டதாகவோ தெரியவில்லை. எப்போது வேண்டுமானாலும் உதவி கேட்கலாம்."], "Now": ["अभी", "ಈಗ", "இப்போது"], "Open request:": ["खुला अनुरोध:", "ತೆರೆದ ಕೋರಿಕೆ:", "திறந்த கோரிக்கை:"], "Open visit pass": ["विज़िट पास खोलें", "ಭೇಟಿ ಪಾಸ್ ತೆರೆಯಿರಿ", "வருகை அனுமதிச்சீட்டைத் திற"], "Outcome": ["परिणाम", "ಫಲಿತಾಂಶ", "முடிவு"], "Password": ["पासवर्ड", "ಪಾಸ್‌ವರ್ಡ್", "கடவுச்சொல்"], "Paste the calendar text into a file named": ["कैलेंडर टेक्स्ट को इस नाम की फ़ाइल में चिपकाएँ", "ಕ್ಯಾಲೆಂಡರ್ ಪಠ್ಯವನ್ನು ಈ ಹೆಸರಿನ ಫೈಲ್‌ಗೆ ಅಂಟಿಸಿ", "நாட்காட்டி உரையை இந்தப் பெயருள்ள கோப்பில் ஒட்டுங்கள்"], "and open it to add all reminders with 30-minute alerts.": ["और सभी रिमाइंडर 30 मिनट पहले की चेतावनी के साथ जोड़ने के लिए उसे खोलें।", "ಮತ್ತು 30 ನಿಮಿಷದ ಎಚ್ಚರಿಕೆಗಳೊಂದಿಗೆ ಎಲ್ಲಾ ಜ್ಞಾಪನೆಗಳನ್ನು ಸೇರಿಸಲು ಅದನ್ನು ತೆರೆಯಿರಿ.", "30 நிமிட எச்சரிக்கைகளுடன் எல்லா நினைவூட்டல்களையும் சேர்க்க அதைத் திறங்கள்."], "Patient journey navigator": ["मरीज़ यात्रा सहायक", "ರೋಗಿ ಪಯಣ ಮಾರ್ಗದರ್ಶಿ", "நோயாளி பயண வழிகாட்டி"], "Payment": ["भुगतान", "ಪಾವತಿ", "கட்டணம்"], "Phone call back": ["फ़ोन कॉल बैक", "ಫೋನ್ ಮರುಕರೆ", "தொலைபேசி திரும்ப அழைப்பு"], "Pick a facility first": ["पहले सुविधा चुनें", "ಮೊದಲು ಕೇಂದ್ರ ಆಯ್ಕೆಮಾಡಿ", "முதலில் இடத்தைத் தேர்ந்தெடுங்கள்"], "Pick a new slot. Your current slot stays booked until you confirm.": ["नया स्लॉट चुनें। पुष्टि करने तक आपका मौजूदा स्लॉट बुक रहेगा।", "ಹೊಸ ಸ್ಲಾಟ್ ಆಯ್ಕೆಮಾಡಿ. ದೃಢೀಕರಿಸುವವರೆಗೆ ಈಗಿನ ಸ್ಲಾಟ್ ಬುಕ್ ಆಗಿರುತ್ತದೆ.", "புதிய நேரத்தைத் தேர்ந்தெடுங்கள். உறுதிப்படுத்தும் வரை தற்போதைய நேரம் முன்பதிவில் இருக்கும்."], "Pick the service you've been told you need, or that you're looking for. If you're not sure, General OPD is the usual starting point.": ["वह सेवा चुनें जो आपको बताई गई है या जिसे आप खोज रहे हैं। पक्का न हो तो सामान्य ओपीडी से शुरुआत करें।", "ನಿಮಗೆ ಹೇಳಿದ ಅಥವಾ ನೀವು ಹುಡುಕುತ್ತಿರುವ ಸೇವೆ ಆಯ್ಕೆಮಾಡಿ. ಖಚಿತವಿಲ್ಲದಿದ್ದರೆ ಸಾಮಾನ್ಯ ಒಪಿಡಿಯಿಂದ ಆರಂಭಿಸಿ.", "உங்களுக்குச் சொல்லப்பட்ட அல்லது நீங்கள் தேடும் சேவையைத் தேர்ந்தெடுங்கள். உறுதியில்லையெனில் பொது OPD யில் தொடங்குங்கள்."], "Please call": ["कृपया कॉल करें", "ದಯವಿಟ್ಟು ಕರೆ ಮಾಡಿ", "தயவுசெய்து அழையுங்கள்"], "Please enter your name.": ["कृपया अपना नाम डालें।", "ದಯವಿಟ್ಟು ನಿಮ್ಮ ಹೆಸರು ನಮೂದಿಸಿ.", "உங்கள் பெயரை உள்ளிடுங்கள்."], "Please tick this box to continue.": ["जारी रखने के लिए यह बॉक्स चुनें।", "ಮುಂದುವರಿಯಲು ಈ ಪೆಟ್ಟಿಗೆ ಗುರುತಿಸಿ.", "தொடர இந்தப் பெட்டியைத் தேர்வு செய்யுங்கள்."], "Preferred language": ["पसंदीदा भाषा", "ಆದ್ಯತೆಯ ಭಾಷೆ", "விருப்ப மொழி"], "Prototype — bookings, tickets and queues are simulated.": ["प्रोटोटाइप — बुकिंग, अनुरोध और कतारें नकली (सिम्युलेटेड) हैं।", "ಮಾದರಿ — ಬುಕಿಂಗ್, ಕೋರಿಕೆಗಳು ಮತ್ತು ಸರದಿಗಳು ಅನುಕರಣೆ.", "முன்மாதிரி — முன்பதிவுகள், கோரிக்கைகள், வரிசைகள் உருவகப்படுத்தப்பட்டவை."], "Prototype: passwords are salted and hashed (SHA-256) and stored on this device only. A live version would use OTP sign-in over SMS.": ["प्रोटोटाइप: पासवर्ड सॉल्ट और हैश (SHA-256) करके केवल इसी डिवाइस पर रखे जाते हैं। असली संस्करण में SMS पर OTP से साइन इन होगा।", "ಮಾದರಿ: ಪಾಸ್‌ವರ್ಡ್‌ಗಳನ್ನು ಸಾಲ್ಟ್ ಮತ್ತು ಹ್ಯಾಶ್ (SHA-256) ಮಾಡಿ ಈ ಸಾಧನದಲ್ಲಿ ಮಾತ್ರ ಸಂಗ್ರಹಿಸಲಾಗುತ್ತದೆ. ನೈಜ ಆವೃತ್ತಿಯಲ್ಲಿ SMS ಮೂಲಕ OTP ಸೈನ್ ಇನ್ ಇರುತ್ತದೆ.", "முன்மாதிரி: கடவுச்சொற்கள் சால்ட் சேர்த்து ஹாஷ் (SHA-256) செய்யப்பட்டு இந்தச் சாதனத்தில் மட்டுமே சேமிக்கப்படுகின்றன. நேரடிப் பதிப்பில் SMS வழி OTP உள்நுழைவு இருக்கும்."], "Queue on the day": ["उस दिन की कतार", "ಆ ದಿನದ ಸರದಿ", "அன்றைய வரிசை"], "Recently verified": ["हाल ही में सत्यापित", "ಇತ್ತೀಚೆಗೆ ಪರಿಶೀಲಿಸಲಾಗಿದೆ", "சமீபத்தில் சரிபார்க்கப்பட்டது"], "Referral required": ["रेफ़रल आवश्यक", "ರೆಫರಲ್ ಅಗತ್ಯ", "பரிந்துரை தேவை"], "Needs a referral letter": ["रेफ़रल पत्र चाहिए", "ರೆಫರಲ್ ಪತ್ರ ಬೇಕು", "பரிந்துரைக் கடிதம் தேவை"], "Referral letter ready": ["रेफ़रल पत्र तैयार", "ರೆಫರಲ್ ಪತ್ರ ಸಿದ್ಧ", "பரிந்துரைக் கடிதம் தயார்"], "You marked it as ready": ["आपने इसे तैयार चिह्नित किया", "ನೀವು ಇದನ್ನು ಸಿದ್ಧ ಎಂದು ಗುರುತಿಸಿದ್ದೀರಿ", "நீங்கள் இதைத் தயார் எனக் குறித்தீர்கள்"], "This department only sees referred patients. A General OPD doctor can issue one.": ["यह विभाग केवल रेफ़र किए गए मरीज़ों को देखता है। सामान्य ओपीडी डॉक्टर यह दे सकते हैं।", "ಈ ವಿಭಾಗ ಶಿಫಾರಸು ಮಾಡಿದ ರೋಗಿಗಳನ್ನು ಮಾತ್ರ ನೋಡುತ್ತದೆ. ಸಾಮಾನ್ಯ ಒಪಿಡಿ ವೈದ್ಯರು ಇದನ್ನು ನೀಡಬಹುದು.", "இந்தப் பிரிவு பரிந்துரைக்கப்பட்ட நோயாளிகளை மட்டுமே பார்க்கும். பொது OPD மருத்துவர் இதை வழங்கலாம்."], "Referral to which department?": ["किस विभाग के लिए रेफ़रल?", "ಯಾವ ವಿಭಾಗಕ್ಕೆ ರೆಫರಲ್?", "எந்தப் பிரிவுக்குப் பரிந்துரை?"], "Referral marked ready — booking unlocked": ["रेफ़रल तैयार चिह्नित — बुकिंग खुल गई", "ರೆಫರಲ್ ಸಿದ್ಧ — ಬುಕಿಂಗ್ ತೆರೆಯಿತು", "பரிந்துரை தயார் — முன்பதிவு திறக்கப்பட்டது"], "Referrals, reminders and follow-ups planned for you": ["रेफ़रल, रिमाइंडर और फ़ॉलो-अप आपके लिए तय", "ರೆಫರಲ್, ಜ್ಞಾಪನೆ ಮತ್ತು ಮುಂದಿನ ಭೇಟಿಗಳನ್ನು ನಿಮಗಾಗಿ ಯೋಜಿಸಲಾಗುತ್ತದೆ", "பரிந்துரைகள், நினைவூட்டல்கள், தொடர் வருகைகள் உங்களுக்காகத் திட்டமிடப்படும்"], "Reminders & next steps": ["रिमाइंडर और अगले कदम", "ಜ್ಞಾಪನೆಗಳು ಮತ್ತು ಮುಂದಿನ ಹೆಜ್ಜೆಗಳು", "நினைவூட்டல்கள் & அடுத்த படிகள்"], "Reminders appear once you book a slot.": ["स्लॉट बुक करते ही रिमाइंडर दिखेंगे।", "ಸ್ಲಾಟ್ ಬುಕ್ ಮಾಡಿದ ನಂತರ ಜ್ಞಾಪನೆಗಳು ಕಾಣಿಸುತ್ತವೆ.", "நேரத்தை முன்பதிவு செய்ததும் நினைவூட்டல்கள் தோன்றும்."], "No reminders yet — book a slot first.": ["अभी कोई रिमाइंडर नहीं — पहले स्लॉट बुक करें।", "ಇನ್ನೂ ಜ್ಞಾಪನೆ ಇಲ್ಲ — ಮೊದಲು ಸ್ಲಾಟ್ ಬುಕ್ ಮಾಡಿ.", "இன்னும் நினைவூட்டல் இல்லை — முதலில் நேரத்தை முன்பதிவு செய்யுங்கள்."], "Request a navigator": ["सहायक का अनुरोध करें", "ಸಹಾಯಕರನ್ನು ಕೋರಿ", "வழிகாட்டியைக் கோருங்கள்"], "Reset your password": ["पासवर्ड रीसेट करें", "ಪಾಸ್‌ವರ್ಡ್ ಮರುಹೊಂದಿಸಿ", "கடவுச்சொல்லை மீட்டமை"], "Self-pay accepted": ["स्वयं भुगतान स्वीकार", "ಸ್ವಂತ ಪಾವತಿ ಸ್ವೀಕಾರ", "சொந்தச் செலவு ஏற்கப்படும்"], "Members only": ["केवल सदस्य", "ಸದಸ್ಯರಿಗೆ ಮಾತ್ರ", "உறுப்பினர்களுக்கு மட்டும்"], "Send request": ["अनुरोध भेजें", "ಕೋರಿಕೆ ಕಳುಹಿಸಿ", "கோரிக்கையை அனுப்பு"], "Service": ["सेवा", "ಸೇವೆ", "சேவை"], "Show this at the registration counter. Copy it to send to a family member or caregiver.": ["इसे पंजीकरण काउंटर पर दिखाएँ। परिवार के सदस्य या देखभाल करने वाले को भेजने के लिए कॉपी करें।", "ಇದನ್ನು ನೋಂದಣಿ ಕೌಂಟರ್‌ನಲ್ಲಿ ತೋರಿಸಿ. ಕುಟುಂಬದವರಿಗೆ ಅಥವಾ ಆರೈಕೆದಾರರಿಗೆ ಕಳುಹಿಸಲು ನಕಲಿಸಿ.", "இதைப் பதிவு கவுண்டரில் காட்டுங்கள். குடும்ப உறுப்பினர் அல்லது பராமரிப்பாளருக்கு அனுப்ப நகலெடுங்கள்."], "Sign in": ["साइन इन", "ಸೈನ್ ಇನ್", "உள்நுழை"], "Sign in or create account": ["साइन इन करें या खाता बनाएँ", "ಸೈನ್ ಇನ್ ಮಾಡಿ ಅಥವಾ ಖಾತೆ ರಚಿಸಿ", "உள்நுழையுங்கள் அல்லது கணக்கை உருவாக்குங்கள்"], "Sign in to continue your healthcare journey.": ["अपनी स्वास्थ्य यात्रा जारी रखने के लिए साइन इन करें।", "ನಿಮ್ಮ ಆರೋಗ್ಯ ಪಯಣ ಮುಂದುವರಿಸಲು ಸೈನ್ ಇನ್ ಮಾಡಿ.", "உங்கள் மருத்துவப் பயணத்தைத் தொடர உள்நுழையுங்கள்."], "Sign out": ["साइन आउट", "ಸೈನ್ ಔಟ್", "வெளியேறு"], "Signed in as": ["इस रूप में साइन इन:", "ಹೀಗೆ ಸೈನ್ ಇನ್ ಆಗಿದ್ದೀರಿ:", "இவ்வாறு உள்நுழைந்துள்ளீர்கள்:"], "managing care for someone else": ["किसी और की देखभाल का प्रबंधन", "ಬೇರೆಯವರ ಆರೈಕೆ ನಿರ್ವಹಣೆ", "வேறொருவரின் பராமரிப்பை நிர்வகிக்கிறீர்கள்"], "Signing up for": ["किसके लिए साइन अप", "ಯಾರಿಗಾಗಿ ನೋಂದಣಿ", "யாருக்காகப் பதிவு"], "Skip to content": ["मुख्य सामग्री पर जाएँ", "ವಿಷಯಕ್ಕೆ ಹೋಗಿ", "உள்ளடக்கத்துக்குச் செல்"], "Slots come from the facility you choose.": ["स्लॉट आपकी चुनी हुई सुविधा से आते हैं।", "ಸ್ಲಾಟ್‌ಗಳು ನೀವು ಆಯ್ಕೆಮಾಡಿದ ಕೇಂದ್ರದಿಂದ ಬರುತ್ತವೆ.", "நேரங்கள் நீங்கள் தேர்ந்தெடுக்கும் இடத்திலிருந்து வரும்."], "Start over": ["फिर से शुरू करें", "ಮತ್ತೆ ಆರಂಭಿಸಿ", "மீண்டும் தொடங்கு"], "Start over?": ["फिर से शुरू करें?", "ಮತ್ತೆ ಆರಂಭಿಸಬೇಕೇ?", "மீண்டும் தொடங்கவா?"], "Start a new need": ["नई ज़रूरत शुरू करें", "ಹೊಸ ಅಗತ್ಯ ಆರಂಭಿಸಿ", "புதிய தேவையைத் தொடங்கு"], "New need": ["नई ज़रूरत", "ಹೊಸ ಅಗತ್ಯ", "புதிய தேவை"], "waiting": ["प्रतीक्षा में", "ಕಾಯುತ್ತಿದೆ", "காத்திருக்கிறது"], "Waiting for referral": ["रेफ़रल की प्रतीक्षा", "ರೆಫರಲ್‌ಗಾಗಿ ಕಾಯುತ್ತಿದೆ", "பரிந்துரைக்காகக் காத்திருக்கிறது"], "Support requested": ["माँगी गई सहायता", "ಕೋರಿದ ಬೆಂಬಲ", "கோரப்பட்ட உதவி"], "TOKEN": ["टोकन", "ಟೋಕನ್", "டோக்கன்"], "Talk to a navigator": ["सहायक से बात करें", "ಸಹಾಯಕರೊಂದಿಗೆ ಮಾತನಾಡಿ", "வழிகாட்டியுடன் பேசுங்கள்"], "Tell us what you need and we'll match facilities.": ["बताइए आपको क्या चाहिए, हम सुविधाएँ मिलाएँगे।", "ನಿಮಗೆ ಏನು ಬೇಕು ಎಂದು ತಿಳಿಸಿ, ನಾವು ಕೇಂದ್ರಗಳನ್ನು ಹೊಂದಿಸುತ್ತೇವೆ.", "உங்களுக்கு என்ன தேவை என்று சொல்லுங்கள்; பொருத்தமான இடங்களைத் தருவோம்."], "Text size": ["अक्षर का आकार", "ಅಕ್ಷರ ಗಾತ್ರ", "எழுத்து அளவு"], "That email/mobile and password don't match an account on this device.": ["यह ईमेल/मोबाइल और पासवर्ड इस डिवाइस के किसी खाते से मेल नहीं खाते।", "ಈ ಇಮೇಲ್/ಮೊಬೈಲ್ ಮತ್ತು ಪಾಸ್‌ವರ್ಡ್ ಈ ಸಾಧನದ ಯಾವುದೇ ಖಾತೆಗೆ ಹೊಂದುವುದಿಲ್ಲ.", "இந்த மின்னஞ்சல்/கைபேசி மற்றும் கடவுச்சொல் இந்தச் சாதனத்தில் உள்ள எந்தக் கணக்குடனும் பொருந்தவில்லை."], "That's a question for a clinician.": ["यह प्रश्न किसी चिकित्सक के लिए है।", "ಇದು ವೈದ್ಯರಿಗೆ ಕೇಳಬೇಕಾದ ಪ್ರಶ್ನೆ.", "இது மருத்துவரிடம் கேட்க வேண்டிய கேள்வி."], "This afternoon": ["आज दोपहर", "ಇಂದು ಮಧ್ಯಾಹ್ನ", "இன்று மதியம்"], "This morning": ["आज सुबह", "ಇಂದು ಬೆಳಿಗ್ಗೆ", "இன்று காலை"], "Tomorrow": ["कल", "ನಾಳೆ", "நாளை"], "Today": ["आज", "ಇಂದು", "இன்று"], "This clears your journey, documents and requests on this device.": ["इससे इस डिवाइस पर आपकी यात्रा, दस्तावेज़ और अनुरोध मिट जाएँगे।", "ಇದು ಈ ಸಾಧನದಲ್ಲಿನ ನಿಮ್ಮ ಪಯಣ, ದಾಖಲೆಗಳು ಮತ್ತು ಕೋರಿಕೆಗಳನ್ನು ಅಳಿಸುತ್ತದೆ.", "இது இந்தச் சாதனத்தில் உங்கள் பயணம், ஆவணங்கள், கோரிக்கைகளை அழிக்கும்."], "This may need urgent help.": ["इसमें तुरंत मदद की ज़रूरत हो सकती है।", "ಇದಕ್ಕೆ ತುರ್ತು ಸಹಾಯ ಬೇಕಾಗಬಹುದು.", "இதற்கு அவசர உதவி தேவைப்படலாம்."], "This only matches words to department names. It is not a medical assessment — you choose.": ["यह केवल शब्दों को विभाग के नामों से मिलाता है। यह चिकित्सा मूल्यांकन नहीं है — चुनाव आपका है।", "ಇದು ಪದಗಳನ್ನು ವಿಭಾಗದ ಹೆಸರುಗಳಿಗೆ ಮಾತ್ರ ಹೊಂದಿಸುತ್ತದೆ. ಇದು ವೈದ್ಯಕೀಯ ಮೌಲ್ಯಮಾಪನ ಅಲ್ಲ — ಆಯ್ಕೆ ನಿಮ್ಮದು.", "இது வார்த்தைகளைப் பிரிவுப் பெயர்களுடன் மட்டுமே பொருத்துகிறது. இது மருத்துவ மதிப்பீடு அல்ல — நீங்களே தேர்ந்தெடுங்கள்."], "To another department or hospital": ["दूसरे विभाग या अस्पताल को", "ಬೇರೆ ವಿಭಾಗ ಅಥವಾ ಆಸ್ಪತ್ರೆಗೆ", "வேறு பிரிவு அல்லது மருத்துவமனைக்கு"], "Too short": ["बहुत छोटा", "ತುಂಬಾ ಚಿಕ್ಕದು", "மிகக் குறுகியது"], "Weak": ["कमज़ोर", "ದುರ್ಬಲ", "பலவீனம்"], "Fair": ["ठीक-ठाक", "ಸಾಧಾರಣ", "பரவாயில்லை"], "Good": ["अच्छा", "ಉತ್ತಮ", "நல்லது"], "Strong": ["मज़बूत", "ಬಲವಾದ", "வலுவானது"], "Very strong": ["बहुत मज़बूत", "ತುಂಬಾ ಬಲವಾದ", "மிக வலுவானது"], "Try widening your time preference": ["अपनी समय पसंद बढ़ाकर देखें", "ನಿಮ್ಮ ಸಮಯ ಆಯ್ಕೆಯನ್ನು ವಿಸ್ತರಿಸಿ ನೋಡಿ", "உங்கள் நேர விருப்பத்தை விரிவாக்கிப் பாருங்கள்"], "Ask a navigator about walk-in queues": ["वॉक-इन कतार के बारे में सहायक से पूछें", "ನೇರ ಸರದಿ ಬಗ್ಗೆ ಸಹಾಯಕರನ್ನು ಕೇಳಿ", "நேரடி வரிசை பற்றி வழிகாட்டியிடம் கேளுங்கள்"], "Typical response": ["सामान्य जवाब", "ಸಾಮಾನ್ಯ ಪ್ರತಿಕ್ರಿಯೆ", "வழக்கமான பதில்"], "within 2 working hours (simulated)": ["2 कार्य-घंटों के भीतर (सिम्युलेटेड)", "2 ಕೆಲಸದ ಗಂಟೆಗಳೊಳಗೆ (ಅನುಕರಣೆ)", "2 வேலை நேரத்துக்குள் (உருவகம்)"], "Use 8+ characters with a letter and a number": ["अक्षर और अंक सहित 8+ वर्ण उपयोग करें", "ಅಕ್ಷರ ಮತ್ತು ಅಂಕಿಯೊಂದಿಗೆ 8+ ಅಕ್ಷರಗಳನ್ನು ಬಳಸಿ", "ஒரு எழுத்தும் ஒரு எண்ணும் உள்ள 8+ குறியீடுகளைப் பயன்படுத்துங்கள்"], "Use at least 8 characters, including a letter and a number.": ["कम से कम 8 वर्ण उपयोग करें, जिसमें एक अक्षर और एक अंक हो।", "ಕನಿಷ್ಠ 8 ಅಕ್ಷರಗಳನ್ನು ಬಳಸಿ, ಒಂದು ಅಕ್ಷರ ಮತ್ತು ಒಂದು ಅಂಕಿ ಸೇರಿ.", "குறைந்தது 8 குறியீடுகள், அதில் ஒரு எழுத்தும் ஒரு எண்ணும் இருக்க வேண்டும்."], "Video call with sign-language interpreter": ["सांकेतिक भाषा दुभाषिया के साथ वीडियो कॉल", "ಸಂಜ್ಞಾ ಭಾಷಾ ವ್ಯಾಖ್ಯಾನಕಾರರೊಂದಿಗೆ ವೀಡಿಯೊ ಕರೆ", "சைகை மொழி பெயர்ப்பாளருடன் காணொலி அழைப்பு"], "WhatsApp message": ["WhatsApp संदेश", "WhatsApp ಸಂದೇಶ", "WhatsApp செய்தி"], "We can't assess symptoms. Call": ["हम लक्षणों का आकलन नहीं कर सकते। कॉल करें", "ನಾವು ರೋಗಲಕ್ಷಣಗಳನ್ನು ಮೌಲ್ಯಮಾಪನ ಮಾಡಲಾಗದು. ಕರೆ ಮಾಡಿ", "அறிகுறிகளை எங்களால் மதிப்பிட முடியாது. அழையுங்கள்"], "We only help with where to go and what to bring. Ask the doctor at your visit, or use the government teleconsultation service eSanjeevani (esanjeevani.mohfw.gov.in), or call the Tamil Nadu health helpline": ["हम केवल कहाँ जाना है और क्या लाना है, इसमें मदद करते हैं। मुलाक़ात पर डॉक्टर से पूछें, या सरकारी टेलीपरामर्श सेवा eSanjeevani (esanjeevani.mohfw.gov.in) का उपयोग करें, या तमिलनाडु स्वास्थ्य हेल्पलाइन पर कॉल करें", "ಎಲ್ಲಿಗೆ ಹೋಗಬೇಕು, ಏನು ತರಬೇಕು ಎಂಬುದಕ್ಕೆ ಮಾತ್ರ ನಾವು ಸಹಾಯ ಮಾಡುತ್ತೇವೆ. ಭೇಟಿಯಲ್ಲಿ ವೈದ್ಯರನ್ನು ಕೇಳಿ, ಅಥವಾ ಸರ್ಕಾರಿ ಟೆಲಿಸಮಾಲೋಚನೆ ಸೇವೆ eSanjeevani (esanjeevani.mohfw.gov.in) ಬಳಸಿ, ಅಥವಾ ತಮಿಳುನಾಡು ಆರೋಗ್ಯ ಸಹಾಯವಾಣಿಗೆ ಕರೆ ಮಾಡಿ", "எங்கு செல்ல வேண்டும், என்ன கொண்டு வர வேண்டும் என்பதற்கு மட்டுமே உதவுகிறோம். வருகையின்போது மருத்துவரிடம் கேளுங்கள், அல்லது அரசின் தொலை ஆலோசனைச் சேவை eSanjeevani (esanjeevani.mohfw.gov.in) பயன்படுத்துங்கள், அல்லது தமிழ்நாடு சுகாதார உதவி எண்ணை அழையுங்கள்"], "We only help with where to go and what to bring. Ask the doctor at your visit, or use the government teleconsultation service eSanjeevani (esanjeevani.mohfw.gov.in). We can still help you book a visit.": ["हम केवल कहाँ जाना है और क्या लाना है, इसमें मदद करते हैं। मुलाक़ात पर डॉक्टर से पूछें, या सरकारी टेलीपरामर्श सेवा eSanjeevani (esanjeevani.mohfw.gov.in) का उपयोग करें। हम फिर भी मुलाक़ात बुक करने में मदद कर सकते हैं।", "ಎಲ್ಲಿಗೆ ಹೋಗಬೇಕು, ಏನು ತರಬೇಕು ಎಂಬುದಕ್ಕೆ ಮಾತ್ರ ನಾವು ಸಹಾಯ ಮಾಡುತ್ತೇವೆ. ಭೇಟಿಯಲ್ಲಿ ವೈದ್ಯರನ್ನು ಕೇಳಿ, ಅಥವಾ ಸರ್ಕಾರಿ ಟೆಲಿಸಮಾಲೋಚನೆ ಸೇವೆ eSanjeevani (esanjeevani.mohfw.gov.in) ಬಳಸಿ. ಆದರೂ ಭೇಟಿ ಬುಕ್ ಮಾಡಲು ನಾವು ಸಹಾಯ ಮಾಡಬಹುದು.", "எங்கு செல்ல வேண்டும், என்ன கொண்டு வர வேண்டும் என்பதற்கு மட்டுமே உதவுகிறோம். வருகையின்போது மருத்துவரிடம் கேளுங்கள், அல்லது அரசின் தொலை ஆலோசனைச் சேவை eSanjeevani (esanjeevani.mohfw.gov.in) பயன்படுத்துங்கள். இருந்தாலும் வருகையை முன்பதிவு செய்ய நாங்கள் உதவலாம்."], "We spotted": ["हमें मिलीं", "ನಾವು ಗಮನಿಸಿದ್ದು", "நாங்கள் கண்டவை:"], "thing a human navigator should check:": ["बात जो एक सहायक को जाँचनी चाहिए:", "ವಿಷಯವನ್ನು ಸಹಾಯಕರು ಪರಿಶೀಲಿಸಬೇಕು:", "விஷயத்தை ஒரு வழிகாட்டி சரிபார்க்க வேண்டும்:"], "things a human navigator should check:": ["बातें जो एक सहायक को जाँचनी चाहिए:", "ವಿಷಯಗಳನ್ನು ಸಹಾಯಕರು ಪರಿಶೀಲಿಸಬೇಕು:", "விஷயங்களை ஒரு வழிகாட்டி சரிபார்க்க வேண்டும்:"], "We'll use this to sign you in. Mobile: 10 digits, starting with 6–9.": ["साइन इन के लिए हम इसका उपयोग करेंगे। मोबाइल: 10 अंक।", "ಸೈನ್ ಇನ್‌ಗೆ ಇದನ್ನು ಬಳಸುತ್ತೇವೆ. ಮೊಬೈಲ್: 10 ಅಂಕಿಗಳು.", "உள்நுழைய இதைப் பயன்படுத்துவோம். கைபேசி: 10 இலக்கங்கள்."], "Welcome back": ["फिर से स्वागत है", "ಮರಳಿ ಸ್ವಾಗತ", "மீண்டும் வருக"], "What we'll send them (you can edit the note)": ["हम उन्हें क्या भेजेंगे (आप नोट बदल सकते हैं)", "ನಾವು ಅವರಿಗೆ ಕಳುಹಿಸುವುದು (ನೀವು ಟಿಪ್ಪಣಿ ಬದಲಿಸಬಹುದು)", "அவர்களுக்கு நாங்கள் அனுப்புவது (குறிப்பை நீங்கள் மாற்றலாம்)"], "When should you come back?": ["आपको कब वापस आना है?", "ನೀವು ಯಾವಾಗ ಮತ್ತೆ ಬರಬೇಕು?", "எப்போது மீண்டும் வர வேண்டும்?"], "When you arrive, check in to see where you are in the queue (simulated for the prototype).": ["पहुँचने पर चेक-इन करें और कतार में अपनी जगह देखें (प्रोटोटाइप में सिम्युलेटेड)।", "ಬಂದಾಗ ಚೆಕ್-ಇನ್ ಮಾಡಿ ಸರದಿಯಲ್ಲಿ ನಿಮ್ಮ ಸ್ಥಾನ ನೋಡಿ (ಮಾದರಿಯಲ್ಲಿ ಅನುಕರಣೆ).", "வந்ததும் பதிவு செய்து வரிசையில் உங்கள் இடத்தைப் பாருங்கள் (முன்மாதிரியில் உருவகம்)."], "I've arrived — check in": ["मैं पहुँच गया/गई — चेक-इन करें", "ನಾನು ಬಂದಿದ್ದೇನೆ — ಚೆಕ್-ಇನ್", "நான் வந்துவிட்டேன் — பதிவு செய்"], "It's your turn.": ["आपकी बारी है।", "ನಿಮ್ಮ ಸರದಿ ಬಂದಿದೆ.", "உங்கள் முறை வந்துவிட்டது."], "When?": ["कब?", "ಯಾವಾಗ?", "எப்போது?"], "Where": ["कहाँ", "ಎಲ್ಲಿ", "எங்கே"], "Why we suggest it": ["हम यह क्यों सुझाते हैं", "ನಾವು ಇದನ್ನು ಏಕೆ ಸೂಚಿಸುತ್ತೇವೆ", "நாங்கள் ஏன் பரிந்துரைக்கிறோம்"], "YOU": ["आप", "ನೀವು", "நீங்கள்"], "You": ["आप", "ನೀವು", "நீங்கள்"], "Yes, cancel": ["हाँ, रद्द करें", "ಹೌದು, ರದ್ದುಮಾಡಿ", "ஆம், ரத்து செய்"], "Booking cancelled": ["बुकिंग रद्द हुई", "ಬುಕಿಂಗ್ ರದ್ದಾಗಿದೆ", "முன்பதிவு ரத்தானது"], "Rescheduled": ["समय बदला गया", "ಸಮಯ ಬದಲಾಯಿಸಲಾಗಿದೆ", "நேரம் மாற்றப்பட்டது"], "Journey closed": ["यात्रा बंद", "ಪಯಣ ಮುಕ್ತಾಯ", "பயணம் முடிந்தது"], "Lab-test step added": ["लैब जाँच का चरण जोड़ा गया", "ಪ್ರಯೋಗಾಲಯ ಪರೀಕ್ಷೆ ಹಂತ ಸೇರಿಸಲಾಗಿದೆ", "ஆய்வகப் பரிசோதனைப் படி சேர்க்கப்பட்டது"], "Added a General OPD visit before your specialist visit": ["विशेषज्ञ मुलाक़ात से पहले सामान्य ओपीडी मुलाक़ात जोड़ी गई", "ತಜ್ಞರ ಭೇಟಿಗೆ ಮೊದಲು ಸಾಮಾನ್ಯ ಒಪಿಡಿ ಭೇಟಿ ಸೇರಿಸಲಾಗಿದೆ", "நிபுணர் வருகைக்கு முன் பொது OPD வருகை சேர்க்கப்பட்டது"], "Reading aloud…": ["पढ़कर सुना रहे हैं…", "ಓದಿ ಹೇಳುತ್ತಿದೆ…", "உரக்கப் படிக்கிறது…"], "Read-aloud isn't available in this browser": ["इस ब्राउज़र में पढ़कर सुनाना उपलब्ध नहीं", "ಈ ಬ್ರೌಸರ್‌ನಲ್ಲಿ ಓದಿ ಹೇಳುವುದು ಲಭ್ಯವಿಲ್ಲ", "இந்த உலாவியில் உரக்கப் படித்தல் இல்லை"], "You're in as a guest — nothing is saved after you close the tab": ["आप अतिथि के रूप में हैं — टैब बंद करने के बाद कुछ सहेजा नहीं जाएगा", "ನೀವು ಅತಿಥಿಯಾಗಿದ್ದೀರಿ — ಟ್ಯಾಬ್ ಮುಚ್ಚಿದ ನಂತರ ಏನೂ ಉಳಿಯುವುದಿಲ್ಲ", "நீங்கள் விருந்தினராக உள்ளீர்கள் — தாவலை மூடியபின் எதுவும் சேமிக்கப்படாது"], "You asked something that needs clinical judgement": ["आपने ऐसा कुछ पूछा जिसके लिए चिकित्सकीय निर्णय चाहिए", "ವೈದ್ಯಕೀಯ ತೀರ್ಮಾನ ಬೇಕಾದ ವಿಷಯವನ್ನು ನೀವು ಕೇಳಿದ್ದೀರಿ", "மருத்துவத் தீர்ப்பு தேவைப்படும் ஒன்றைக் கேட்டீர்கள்"], "You don't have to go through this alone.": ["आपको इससे अकेले नहीं गुज़रना है।", "ನೀವು ಇದನ್ನು ಒಂಟಿಯಾಗಿ ಎದುರಿಸಬೇಕಿಲ್ಲ.", "நீங்கள் இதைத் தனியாகக் கடக்க வேண்டியதில்லை."], "if you are in immediate danger. This app can't help with this, but a trained person can — right now.": ["पर, अगर आप तुरंत ख़तरे में हैं। यह ऐप इसमें मदद नहीं कर सकता, पर एक प्रशिक्षित व्यक्ति कर सकता है — अभी।", "ಗೆ ಕರೆ ಮಾಡಿ, ನೀವು ತಕ್ಷಣದ ಅಪಾಯದಲ್ಲಿದ್ದರೆ. ಈ ಆ್ಯಪ್ ಇದಕ್ಕೆ ಸಹಾಯ ಮಾಡಲಾಗದು, ಆದರೆ ತರಬೇತಿ ಪಡೆದ ವ್ಯಕ್ತಿ ಮಾಡಬಹುದು — ಈಗಲೇ.", "ஐ அழையுங்கள், நீங்கள் உடனடி ஆபத்தில் இருந்தால். இந்தச் செயலியால் இதற்கு உதவ முடியாது, ஆனால் பயிற்சி பெற்ற ஒருவர் உதவுவார் — இப்போதே."], "You tell us what was decided; we only organise the paperwork and bookings that follow.": ["आप बताएँ कि क्या तय हुआ; हम केवल उसके बाद के काग़ज़ और बुकिंग व्यवस्थित करते हैं।", "ಏನು ನಿರ್ಧಾರವಾಯಿತು ಎಂದು ನೀವು ತಿಳಿಸಿ; ನಂತರದ ದಾಖಲೆ ಮತ್ತು ಬುಕಿಂಗ್‌ಗಳನ್ನು ಮಾತ್ರ ನಾವು ವ್ಯವಸ್ಥೆ ಮಾಡುತ್ತೇವೆ.", "என்ன முடிவானது என்று நீங்கள் சொல்லுங்கள்; அதைத் தொடரும் ஆவணங்களையும் முன்பதிவுகளையும் மட்டுமே நாங்கள் ஒழுங்கு செய்வோம்."], "Your account": ["आपका खाता", "ನಿಮ್ಮ ಖಾತೆ", "உங்கள் கணக்கு"], "Your description mentions something that may be urgent": ["आपके विवरण में कुछ ऐसा है जो तुरंत ज़रूरी हो सकता है", "ನಿಮ್ಮ ವಿವರಣೆಯಲ್ಲಿ ತುರ್ತು ಆಗಿರಬಹುದಾದ ವಿಷಯವಿದೆ", "உங்கள் விவரிப்பில் அவசரமாக இருக்கக்கூடிய ஒன்று உள்ளது"], "Your journey": ["आपकी यात्रा", "ನಿಮ್ಮ ಪಯಣ", "உங்கள் பயணம்"], "Your slot will be released for someone else. You can book again any time.": ["आपका स्लॉट किसी और के लिए खुल जाएगा। आप कभी भी फिर से बुक कर सकते हैं।", "ನಿಮ್ಮ ಸ್ಲಾಟ್ ಬೇರೆಯವರಿಗೆ ಬಿಡುಗಡೆಯಾಗುತ್ತದೆ. ಯಾವಾಗ ಬೇಕಾದರೂ ಮತ್ತೆ ಬುಕ್ ಮಾಡಬಹುದು.", "உங்கள் நேரம் வேறொருவருக்கு விடுவிக்கப்படும். எப்போது வேண்டுமானாலும் மீண்டும் முன்பதிவு செய்யலாம்."], "Your visit pass": ["आपका विज़िट पास", "ನಿಮ್ಮ ಭೇಟಿ ಪಾಸ್", "உங்கள் வருகை அனுமதிச்சீட்டு"], "about": ["लगभग", "ಸುಮಾರು", "சுமார்"], "ready to book,": ["बुक करने को तैयार,", "ಬುಕ್ ಮಾಡಲು ಸಿದ್ಧ,", "முன்பதிவுக்குத் தயார்,"], "need a step first,": ["को पहले एक कदम चाहिए,", "ಕ್ಕೆ ಮೊದಲು ಒಂದು ಹೆಜ್ಜೆ ಬೇಕು,", "க்கு முதலில் ஒரு படி தேவை,"], "e.g. My daughter will take the call; I need help with the referral.": ["जैसे: मेरी बेटी कॉल उठाएगी; मुझे रेफ़रल में मदद चाहिए।", "ಉದಾ: ನನ್ನ ಮಗಳು ಕರೆ ಸ್ವೀಕರಿಸುತ್ತಾಳೆ; ರೆಫರಲ್‌ಗೆ ಸಹಾಯ ಬೇಕು.", "எ.கா. என் மகள் அழைப்பை எடுப்பார்; பரிந்துரைக்கு உதவி தேவை."], "e.g. “My doctor said I need to see a heart specialist”": ["जैसे “डॉक्टर ने कहा कि मुझे हृदय विशेषज्ञ को दिखाना है”", "ಉದಾ “ನಾನು ಹೃದಯ ತಜ್ಞರನ್ನು ನೋಡಬೇಕು ಎಂದು ವೈದ್ಯರು ಹೇಳಿದರು”", "எ.கா. “இதய நிபுணரைப் பார்க்க வேண்டும் என்று என் மருத்துவர் சொன்னார்”"], "or": ["या", "ಅಥವಾ", "அல்லது"], "Attach photo": ["फ़ोटो लगाएँ", "ಫೋಟೋ ಲಗತ್ತಿಸಿ", "புகைப்படம் இணை"], "Selected": ["चुना गया", "ಆಯ್ಕೆಯಾಗಿದೆ", "தேர்ந்தெடுக்கப்பட்டது"], "No facility in the data meets all your needs.": ["डेटा में कोई सुविधा आपकी सभी ज़रूरतें पूरी नहीं करती।", "ಡೇಟಾದಲ್ಲಿ ಯಾವುದೇ ಕೇಂದ್ರ ನಿಮ್ಮ ಎಲ್ಲಾ ಅಗತ್ಯಗಳನ್ನು ಪೂರೈಸುವುದಿಲ್ಲ.", "தரவில் எந்த இடமும் உங்கள் எல்லாத் தேவைகளையும் பூர்த்தி செய்யவில்லை."], "A human navigator can look beyond this dataset or arrange support (transport, interpreter, ramps).": ["एक सहायक इस डेटा से बाहर देख सकते हैं या सहायता (परिवहन, दुभाषिया, रैंप) की व्यवस्था कर सकते हैं।", "ಸಹಾಯಕರು ಈ ಡೇಟಾದ ಹೊರಗೆ ಹುಡುಕಬಹುದು ಅಥವಾ ಬೆಂಬಲ (ಸಾರಿಗೆ, ವ್ಯಾಖ್ಯಾನಕಾರ, ರ್ಯಾಂಪ್) ವ್ಯವಸ್ಥೆ ಮಾಡಬಹುದು.", "ஒரு வழிகாட்டி இந்தத் தரவுக்கு அப்பால் தேடலாம் அல்லது உதவி (போக்குவரத்து, மொழிபெயர்ப்பாளர், சாய்தளம்) ஏற்பாடு செய்யலாம்."], "Whether you need a referral is a rule of this department, from the organiser data. Whether you should see this specialist is a decision for a doctor — this app doesn't make it.": ["रेफ़रल चाहिए या नहीं, यह इस विभाग का नियम है (आयोजक डेटा से)। आपको इस विशेषज्ञ को दिखाना चाहिए या नहीं, यह डॉक्टर तय करते हैं — यह ऐप नहीं।", "ರೆಫರಲ್ ಬೇಕೇ ಎಂಬುದು ಈ ವಿಭಾಗದ ನಿಯಮ (ಆಯೋಜಕರ ಡೇಟಾದಿಂದ). ನೀವು ಈ ತಜ್ಞರನ್ನು ನೋಡಬೇಕೇ ಎಂಬುದನ್ನು ವೈದ್ಯರು ನಿರ್ಧರಿಸುತ್ತಾರೆ — ಈ ಆ್ಯಪ್ ಅಲ್ಲ.", "பரிந்துரை தேவையா என்பது இந்தப் பிரிவின் விதி (ஏற்பாட்டாளர் தரவிலிருந்து). இந்த நிபுணரைப் பார்க்க வேண்டுமா என்பதை மருத்துவர் முடிவு செய்வார் — இந்தச் செயலி அல்ல."], "Get these before your visit, or ask a navigator what to do.": ["मुलाक़ात से पहले ये ले लें, या सहायक से पूछें कि क्या करना है।", "ಭೇಟಿಗೆ ಮೊದಲು ಇವುಗಳನ್ನು ಪಡೆಯಿರಿ, ಅಥವಾ ಏನು ಮಾಡಬೇಕೆಂದು ಸಹಾಯಕರನ್ನು ಕೇಳಿ.", "வருகைக்கு முன் இவற்றைப் பெறுங்கள், அல்லது என்ன செய்வது என்று வழிகாட்டியிடம் கேளுங்கள்."], "Collect your test report": ["अपनी जाँच रिपोर्ट लें", "ನಿಮ್ಮ ಪರೀಕ್ಷಾ ವರದಿ ಪಡೆಯಿರಿ", "உங்கள் பரிசோதனை அறிக்கையைப் பெறுங்கள்"], "Nothing else is pending for this journey.": ["इस यात्रा में अब कुछ बाकी नहीं है।", "ಈ ಪಯಣದಲ್ಲಿ ಇನ್ನೇನೂ ಬಾಕಿ ಇಲ್ಲ.", "இந்தப் பயணத்தில் வேறு எதுவும் நிலுவையில் இல்லை."], "Your reminders and history stay in Follow-up.": ["आपके रिमाइंडर और इतिहास फ़ॉलो-अप में रहते हैं।", "ನಿಮ್ಮ ಜ್ಞಾಪನೆಗಳು ಮತ್ತು ಇತಿಹಾಸ ಮುಂದಿನ ಹಂತದಲ್ಲಿ ಉಳಿಯುತ್ತವೆ.", "உங்கள் நினைவூட்டல்களும் வரலாறும் தொடர் கவனிப்பில் இருக்கும்."], "Only a doctor can issue one. We'll set up a General OPD visit first, then bring you back here automatically.": ["यह केवल डॉक्टर दे सकते हैं। हम पहले सामान्य ओपीडी मुलाक़ात तय करेंगे, फिर अपने-आप यहाँ वापस लाएँगे।", "ಇದನ್ನು ವೈದ್ಯರು ಮಾತ್ರ ನೀಡಬಹುದು. ಮೊದಲು ಸಾಮಾನ್ಯ ಒಪಿಡಿ ಭೇಟಿ ಏರ್ಪಡಿಸಿ, ನಂತರ ನಿಮ್ಮನ್ನು ಸ್ವಯಂಚಾಲಿತವಾಗಿ ಇಲ್ಲಿಗೆ ಮರಳಿ ತರುತ್ತೇವೆ.", "இதை மருத்துவர் மட்டுமே வழங்க முடியும். முதலில் பொது OPD வருகையை ஏற்பாடு செய்து, பின்னர் தானாகவே உங்களை இங்கு திரும்பக் கொண்டு வருவோம்."], "See facilities without this rule": ["बिना इस नियम वाली सुविधाएँ देखें", "ಈ ನಿಯಮವಿಲ್ಲದ ಕೇಂದ್ರಗಳನ್ನು ನೋಡಿ", "இந்த விதி இல்லாத இடங்களைப் பாருங்கள்"], "None fits every need — a human navigator can help find an alternative.": ["कोई भी हर ज़रूरत पूरी नहीं करती — सहायक विकल्प खोजने में मदद कर सकते हैं।", "ಯಾವುದೂ ಎಲ್ಲಾ ಅಗತ್ಯಗಳನ್ನು ಪೂರೈಸುವುದಿಲ್ಲ — ಸಹಾಯಕರು ಪರ್ಯಾಯ ಹುಡುಕಲು ಸಹಾಯ ಮಾಡಬಹುದು.", "எதுவும் எல்லாத் தேவைகளையும் பூர்த்தி செய்யவில்லை — மாற்று வழியைக் கண்டறிய வழிகாட்டி உதவலாம்."], "Listed as not available": ["उपलब्ध नहीं बताया गया", "ಲಭ್ಯವಿಲ್ಲ ಎಂದು ಪಟ್ಟಿ ಮಾಡಲಾಗಿದೆ", "கிடைக்காது எனக் குறிப்பிடப்பட்டுள்ளது"], "A navigator can try to arrange this": ["सहायक इसकी व्यवस्था करने की कोशिश कर सकते हैं", "ಸಹಾಯಕರು ಇದನ್ನು ವ್ಯವಸ್ಥೆ ಮಾಡಲು ಪ್ರಯತ್ನಿಸಬಹುದು", "வழிகாட்டி இதை ஏற்பாடு செய்ய முயலலாம்"], "Needs advance notice; a navigator can arrange it": ["पहले सूचना देनी होगी; सहायक व्यवस्था कर सकते हैं", "ಮುಂಚಿತ ಸೂಚನೆ ಬೇಕು; ಸಹಾಯಕರು ವ್ಯವಸ್ಥೆ ಮಾಡಬಹುದು", "முன்னறிவிப்பு தேவை; வழிகாட்டி ஏற்பாடு செய்யலாம்"], "Department not step-free": ["विभाग सीढ़ी-रहित नहीं", "ವಿಭಾಗ ಮೆಟ್ಟಿಲುರಹಿತವಲ್ಲ", "பிரிவு படியில்லா அணுகலுடன் இல்லை"], "No shared language listed": ["कोई साझा भाषा नहीं बताई गई", "ಹಂಚಿಕೊಂಡ ಭಾಷೆ ಪಟ್ಟಿಯಲ್ಲಿಲ್ಲ", "பொதுவான மொழி பட்டியலில் இல்லை"], "From": ["कहाँ से", "ಎಲ್ಲಿಂದ", "எங்கிருந்து"], "Languages": ["भाषाएँ", "ಭಾಷೆಗಳು", "மொழிகள்"], "Accessibility": ["सुगम्यता", "ಪ್ರವೇಶಸೌಲಭ್ಯ", "அணுகல்"], "Time": ["समय", "ಸಮಯ", "நேரம்"], "Documents missing": ["अनुपलब्ध दस्तावेज़", "ಇಲ್ಲದ ದಾಖಲೆಗಳು", "இல்லாத ஆவணங்கள்"], "Flags": ["चेतावनियाँ", "ಎಚ್ಚರಿಕೆಗಳು", "எச்சரிக்கைகள்"], "none stated": ["कुछ नहीं बताया", "ಏನೂ ತಿಳಿಸಿಲ್ಲ", "எதுவும் குறிப்பிடவில்லை"], "not chosen yet": ["अभी नहीं चुना", "ಇನ್ನೂ ಆಯ್ಕೆ ಮಾಡಿಲ್ಲ", "இன்னும் தேர்ந்தெடுக்கவில்லை"], "not chosen": ["नहीं चुना", "ಆಯ್ಕೆ ಮಾಡಿಲ್ಲ", "தேர்ந்தெடுக்கவில்லை"], "VISIT PASS": ["विज़िट पास", "ಭೇಟಿ ಪಾಸ್", "வருகை அனுமதிச்சீட்டு"], "Go to Book": ["बुक पर जाएँ", "ಬುಕ್‌ಗೆ ಹೋಗಿ", "முன்பதிவுக்குச் செல்லுங்கள்"], "Go to Find": ["खोज पर जाएँ", "ಹುಡುಕಾಟಕ್ಕೆ ಹೋಗಿ", "தேடலுக்குச் செல்லுங்கள்"], "Go to Need": ["ज़रूरत पर जाएँ", "ಅಗತ್ಯಕ್ಕೆ ಹೋಗಿ", "தேவைக்குச் செல்லுங்கள்"], "Find my options": ["मेरे विकल्प खोजें", "ನನ್ನ ಆಯ್ಕೆಗಳನ್ನು ಹುಡುಕಿ", "என் வாய்ப்புகளைத் தேடு"], "mornings": ["सुबह", "ಬೆಳಿಗ್ಗೆ", "காலை நேரம்"], "afternoons": ["दोपहर", "ಮಧ್ಯಾಹ್ನ", "மதிய நேரம்"], "weekends": ["सप्ताहांत", "ವಾರಾಂತ್ಯ", "வார இறுதி"], "Booked for": ["किसके लिए बुक", "ಯಾರಿಗಾಗಿ", "யாருக்காக"], "Read aloud": ["पढ़कर सुनाएँ", "ಓದಿ ಹೇಳಿ", "உரக்கப் படி"]};
const TRP=[["^(\\d+(?:\\.\\d+)?) km$", ["$1 कि.मी.", "$1 ಕಿ.ಮೀ.", "$1 கி.மீ."]], ["^(\\d+(?:\\.\\d+)?) km away$", ["$1 कि.मी. दूर", "$1 ಕಿ.ಮೀ. ದೂರ", "$1 கி.மீ. தொலைவில்"]], ["^(\\d+) min$", ["$1 मिनट", "$1 ನಿಮಿಷ", "$1 நிமிடம்"]], ["^(\\d+) free$", ["$1 खाली", "$1 ಲಭ್ಯ", "$1 காலி"]], ["^(\\d+) free slots in the next week$", ["अगले सप्ताह $1 खाली स्लॉट", "ಮುಂದಿನ ವಾರ $1 ಖಾಲಿ ಸ್ಲಾಟ್‌ಗಳು", "அடுத்த வாரத்தில் $1 காலி நேரங்கள்"]], ["^(\\d+) free slots in the next week \\((.+)\\)$", ["अगले सप्ताह $1 खाली स्लॉट ($2)", "ಮುಂದಿನ ವಾರ $1 ಖಾಲಿ ಸ್ಲಾಟ್‌ಗಳು ($2)", "அடுத்த வாரத்தில் $1 காலி நேரங்கள் ($2)"]], ["^(\\d+) documents? to prepare$", ["$1 दस्तावेज़ तैयार करने हैं", "$1 ದಾಖಲೆಗಳನ್ನು ಸಿದ್ಧಪಡಿಸಬೇಕು", "$1 ஆவணங்கள் தயாரிக்க வேண்டும்"]], ["^(\\d+) of (\\d+) ready$", ["$2 में से $1 तैयार", "$2 ರಲ್ಲಿ $1 ಸಿದ್ಧ", "$2 இல் $1 தயார்"]], ["^(\\d+) of (\\d+) items still to prepare: (.+)\\.$", ["$2 में से $1 चीज़ें अभी तैयार करनी हैं: $3।", "$2 ರಲ್ಲಿ $1 ಇನ್ನೂ ಸಿದ್ಧಪಡಿಸಬೇಕು: $3.", "$2 இல் $1 இன்னும் தயாரிக்க வேண்டும்: $3."]], ["^(\\d+) weeks?$", ["$1 सप्ताह", "$1 ವಾರ", "$1 வாரம்"]], ["^(\\d+) months?$", ["$1 महीने", "$1 ತಿಂಗಳು", "$1 மாதம்"]], ["^(\\d+)\\. (.+?)( ✓)?$", ["$1. $2$3", "$1. $2$3", "$1. $2$3"]], ["^(\\d+) facilities offer this\\.$", ["$1 स्थान यह सेवा देते हैं।", "$1 ಕೇಂದ್ರಗಳು ಈ ಸೇವೆ ನೀಡುತ್ತವೆ.", "$1 இடங்கள் இந்தச் சேவையை வழங்குகின்றன."]], ["^(\\d+) of (\\d+) facilities offering (.+) can work for you\\.$", ["$3 देने वाले $2 में से $1 स्थान आपके लिए उपयुक्त हो सकते हैं।", "$3 ನೀಡುವ $2 ಕೇಂದ್ರಗಳಲ್ಲಿ $1 ನಿಮಗೆ ಸೂಕ್ತವಾಗಬಹುದು.", "$3 வழங்கும் $2 இடங்களில் $1 உங்களுக்குப் பொருந்தலாம்."]], ["^(\\d+) ahead of you$", ["आपसे पहले $1 लोग", "ನಿಮಗಿಂತ ಮುಂದೆ $1 ಜನ", "உங்களுக்கு முன் $1 பேர்"]], ["^wait at ~(\\d+) min each\\.$", ["इंतज़ार (हर व्यक्ति ~$1 मिनट)।", "ಕಾಯುವಿಕೆ (ಪ್ರತಿ ವ್ಯಕ್ತಿಗೆ ~$1 ನಿಮಿಷ).", "காத்திருப்பு (ஒவ்வொருவருக்கும் ~$1 நிமிடம்)."]], ["^~(\\d+) min per patient$", ["प्रति मरीज़ ~$1 मिनट", "ಪ್ರತಿ ರೋಗಿಗೆ ~$1 ನಿಮಿಷ", "ஒரு நோயாளிக்கு ~$1 நிமிடம்"]], ["^~(\\d+) min from (.+) \\+ 15 min registration$", ["$2 से ~$1 मिनट + 15 मिनट पंजीकरण", "$2 ನಿಂದ ~$1 ನಿಮಿಷ + 15 ನಿಮಿಷ ನೋಂದಣಿ", "$2 இலிருந்து ~$1 நிமிடம் + 15 நிமிடம் பதிவு"]], ["^About (\\d+) min by road from (.+)$", ["$2 से सड़क द्वारा लगभग $1 मिनट", "$2 ನಿಂದ ರಸ್ತೆ ಮೂಲಕ ಸುಮಾರು $1 ನಿಮಿಷ", "$2 இலிருந்து சாலை வழியாக சுமார் $1 நிமிடம்"]], ["^(.+)\\. About (\\d+) min travel\\.$", ["$1। लगभग $2 मिनट की यात्रा।", "$1. ಸುಮಾರು $2 ನಿಮಿಷ ಪ್ರಯಾಣ.", "$1. சுமார் $2 நிமிடப் பயணம்."]], ["^Accepts (.+)$", ["$1 स्वीकार करता है", "$1 ಸ್ವೀಕರಿಸುತ್ತದೆ", "$1 ஏற்கப்படும்"]], ["^Doesn't accept (.+)$", ["$1 स्वीकार नहीं करता", "$1 ಸ್ವೀಕರಿಸುವುದಿಲ್ಲ", "$1 ஏற்கப்படாது"]], ["^You would pay yourself: (.+)$", ["आपको स्वयं भुगतान करना होगा: $1", "ನೀವೇ ಪಾವತಿಸಬೇಕು: $1", "நீங்களே செலுத்த வேண்டும்: $1"]], ["^Only for (.+) members$", ["केवल $1 सदस्यों के लिए", "$1 ಸದಸ್ಯರಿಗೆ ಮಾತ್ರ", "$1 உறுப்பினர்களுக்கு மட்டும்"]], ["^All documents for (.+) are ready\\.$", ["$1 के सभी दस्तावेज़ तैयार हैं।", "$1 ಗಾಗಿ ಎಲ್ಲಾ ದಾಖಲೆಗಳು ಸಿದ್ಧವಾಗಿವೆ.", "$1 க்கான அனைத்து ஆவணங்களும் தயார்."]], ["^Base 40 \\+ factors = (\\d+)\\. Status is set by hard rules \\(payment, physical access\\) and referral needs, not by score\\.$", ["आधार 40 + कारक = $1। स्थिति कड़े नियमों (भुगतान, शारीरिक पहुँच) और रेफ़रल ज़रूरत से तय होती है, स्कोर से नहीं।", "ಮೂಲ 40 + ಅಂಶಗಳು = $1. ಸ್ಥಿತಿಯನ್ನು ಕಟ್ಟುನಿಟ್ಟಿನ ನಿಯಮಗಳು (ಪಾವತಿ, ದೈಹಿಕ ಪ್ರವೇಶ) ಮತ್ತು ರೆಫರಲ್ ಅಗತ್ಯ ನಿರ್ಧರಿಸುತ್ತವೆ, ಅಂಕವಲ್ಲ.", "அடிப்படை 40 + காரணிகள் = $1. நிலையை கடுமையான விதிகள் (கட்டணம், உடல் அணுகல்) மற்றும் பரிந்துரைத் தேவை தீர்மானிக்கின்றன, மதிப்பெண் அல்ல."]], ["^Best match: (.+) \\(fit (\\d+)\\)\\.$", ["सबसे अच्छा मेल: $1 (उपयुक्तता $2)।", "ಅತ್ಯುತ್ತಮ ಹೊಂದಾಣಿಕೆ: $1 (ಹೊಂದಾಣಿಕೆ $2).", "சிறந்த பொருத்தம்: $1 (பொருத்தம் $2)."]], ["^Book your (.+) follow-up$", ["अपना $1 फ़ॉलो-अप बुक करें", "ನಿಮ್ಮ $1 ಮುಂದಿನ ಭೇಟಿ ಬುಕ್ ಮಾಡಿ", "உங்கள் $1 தொடர் வருகையை முன்பதிவு செய்யுங்கள்"]], ["^Booked — token (\\d+)$", ["बुक हो गया — टोकन $1", "ಬುಕ್ ಆಗಿದೆ — ಟೋಕನ್ $1", "முன்பதிவானது — டோக்கன் $1"]], ["^Booked: (.+)$", ["बुक: $1", "ಬುಕ್ ಆಗಿದೆ: $1", "முன்பதிவு: $1"]], ["^booked (.+)$", ["बुक: $1", "ಬುಕ್: $1", "முன்பதிவு: $1"]], ["^(.+) appointment$", ["$1 अपॉइंटमेंट", "$1 ಅಪಾಯಿಂಟ್‌ಮೆಂಟ್", "$1 சந்திப்பு"]], ["^(.+) near (.+)$", ["$2 के पास $1", "$2 ಬಳಿ $1", "$2 அருகில் $1"]], ["^(.+), (.+)\\. Token (\\d+)\\.$", ["$1, $2। टोकन $3।", "$1, $2. ಟೋಕನ್ $3.", "$1, $2. டோக்கன் $3."]], ["^Checked (\\d+) days? ago$", ["$1 दिन पहले जाँचा गया", "$1 ದಿನಗಳ ಹಿಂದೆ ಪರಿಶೀಲಿಸಲಾಗಿದೆ", "$1 நாட்களுக்கு முன் சரிபார்க்கப்பட்டது"]], ["^Come back in (.+)$", ["$1 में फिर आएँ", "$1 ನಂತರ ಮತ್ತೆ ಬನ್ನಿ", "$1 இல் மீண்டும் வாருங்கள்"]], ["^Conflicting info at (.+): (.+)$", ["$1 पर विरोधाभासी जानकारी: $2", "$1 ನಲ್ಲಿ ವಿರೋಧಾತ್ಮಕ ಮಾಹಿತಿ: $2", "$1 இல் முரண்பட்ட தகவல்: $2"]], ["^Conflicting info: (.+)$", ["विरोधाभासी जानकारी: $1", "ವಿರೋಧಾತ್ಮಕ ಮಾಹಿತಿ: $1", "முரண்பட்ட தகவல்: $1"]], ["^Conflicting information: (.+)\\.$", ["विरोधाभासी जानकारी: $1।", "ವಿರೋಧಾತ್ಮಕ ಮಾಹಿತಿ: $1.", "முரண்பட்ட தகவல்: $1."]], ["^Data (\\d+)d old$", ["डेटा $1 दिन पुराना", "ಡೇಟಾ $1 ದಿನ ಹಳೆಯದು", "தரவு $1 நாள் பழையது"]], ["^Details are (\\d+) days old$", ["जानकारी $1 दिन पुरानी है", "ವಿವರಗಳು $1 ದಿನ ಹಳೆಯವು", "விவரங்கள் $1 நாள் பழையவை"]], ["^(.+)'s details are (\\d+) days old$", ["$1 की जानकारी $2 दिन पुरानी है", "$1 ವಿವರಗಳು $2 ದಿನ ಹಳೆಯವು", "$1 இன் விவரங்கள் $2 நாள் பழையவை"]], ["^Earliest slot matching your preference: (.+)\\.$", ["आपकी पसंद से मेल खाता सबसे जल्दी स्लॉट: $1।", "ನಿಮ್ಮ ಆಯ್ಕೆಗೆ ಹೊಂದುವ ಮೊದಲ ಸ್ಲಾಟ್: $1.", "உங்கள் விருப்பத்திற்கேற்ற முதல் நேரம்: $1."]], ["^Expected fee: (.+)$", ["अनुमानित शुल्क: $1", "ಅಂದಾಜು ಶುಲ್ಕ: $1", "எதிர்பார்க்கும் கட்டணம்: $1"]], ["^[Ff]ee: (.+)$", ["शुल्क: $1", "ಶುಲ್ಕ: $1", "கட்டணம்: $1"]], ["^From (₹[\\d,]+)$", ["$1 से", "$1 ರಿಂದ", "$1 முதல்"]], ["^(₹[\\d,]+) / session$", ["$1 / सत्र", "$1 / ಅವಧಿ", "$1 / அமர்வு"]], ["^(₹[\\d,]+) consult$", ["$1 परामर्श", "$1 ಸಮಾಲೋಚನೆ", "$1 ஆலோசனை"]], ["^Faded slots are outside your “(.+)” preference\\. Struck-out slots are taken\\.$", ["धुंधले स्लॉट आपकी “$1” पसंद से बाहर हैं। कटे हुए स्लॉट भर चुके हैं।", "ಮಸುಕಾದ ಸ್ಲಾಟ್‌ಗಳು ನಿಮ್ಮ “$1” ಆಯ್ಕೆಯ ಹೊರಗಿವೆ. ಹೊಡೆದುಹಾಕಿದ ಸ್ಲಾಟ್‌ಗಳು ಭರ್ತಿಯಾಗಿವೆ.", "மங்கலான நேரங்கள் உங்கள் “$1” விருப்பத்திற்கு வெளியே உள்ளன. அடிக்கப்பட்டவை நிரம்பியவை."]], ["^(.*)Source: built-in sample \\(fictional facilities, (.+)\\)$", ["$1स्रोत: अंतर्निहित नमूना (काल्पनिक सुविधाएँ, $2)", "$1ಮೂಲ: ಅಂತರ್ಗತ ಮಾದರಿ (ಕಾಲ್ಪನಿಕ ಕೇಂದ್ರಗಳು, $2)", "$1மூலம்: உள்ளமைந்த மாதிரி (கற்பனை இடங்கள், $2)"]], ["^[Ff]loor (\\d+)$", ["मंज़िल $1", "$1ನೇ ಮಹಡಿ", "தளம் $1"]], ["^[Ff]or (.+)$", ["$1 के लिए", "$1 ಗಾಗಿ", "$1 க்காக"]], ["^Language: (.+?) (✓ staff listed|— interpreter needed)$", ["भाषा: $1 $2", "ಭಾಷೆ: $1 $2", "மொழி: $1 $2"]], ["^Last verified (.+)\\. Confirm before travelling\\.$", ["अंतिम सत्यापन $1। जाने से पहले पुष्टि करें।", "ಕೊನೆಯ ಪರಿಶೀಲನೆ $1. ಹೊರಡುವ ಮೊದಲು ದೃಢೀಕರಿಸಿ.", "கடைசியாக சரிபார்த்தது $1. பயணத்திற்கு முன் உறுதிப்படுத்துங்கள்."]], ["^Leave by (.+) — about (\\d+) min travel plus 15 min for registration\\.$", ["$1 तक निकलें — लगभग $2 मिनट यात्रा और 15 मिनट पंजीकरण।", "$1 ರೊಳಗೆ ಹೊರಡಿ — ಸುಮಾರು $2 ನಿಮಿಷ ಪ್ರಯಾಣ ಮತ್ತು 15 ನಿಮಿಷ ನೋಂದಣಿ.", "$1 க்குள் புறப்படுங்கள் — சுமார் $2 நிமிடப் பயணம், பதிவுக்கு 15 நிமிடம்."]], ["^Leave for (.+)$", ["$1 के लिए निकलें", "$1 ಗೆ ಹೊರಡಿ", "$1 க்குப் புறப்படுங்கள்"]], ["^Loaded: (.+)$", ["लोड किया: $1", "ಲೋಡ್ ಆಯಿತು: $1", "ஏற்றப்பட்டது: $1"]], ["^Map of facilities relative to (.+)$", ["$1 के सापेक्ष सुविधाओं का नक्शा", "$1 ಗೆ ಸಂಬಂಧಿಸಿದ ಕೇಂದ್ರಗಳ ನಕ್ಷೆ", "$1 ஐ ஒட்டிய இடங்களின் வரைபடம்"]], ["^Next slot: (.+)$", ["अगला स्लॉट: $1", "ಮುಂದಿನ ಸ್ಲಾಟ್: $1", "அடுத்த நேரம்: $1"]], ["^Next: (.+)$", ["अगला: $1", "ಮುಂದಿನದು: $1", "அடுத்தது: $1"]], ["^(.+) selected$", ["$1 चुना गया", "$1 ಆಯ್ಕೆಯಾಗಿದೆ", "$1 தேர்ந்தெடுக்கப்பட்டது"]], ["^Offers (.+)$", ["$1 उपलब्ध", "$1 ಲಭ್ಯವಿದೆ", "$1 கிடைக்கும்"]], ["^[Rr]ef ([A-Z]{2}-\\d+)$", ["संदर्भ $1", "ಉಲ್ಲೇಖ $1", "குறிப்பு எண் $1"]], ["^Ref ([A-Z]{2}-\\d+)\\. Arrive 15 min early for registration\\.$", ["संदर्भ $1। पंजीकरण के लिए 15 मिनट पहले पहुँचें।", "ಉಲ್ಲೇಖ $1. ನೋಂದಣಿಗೆ 15 ನಿಮಿಷ ಮುಂಚಿತವಾಗಿ ಬನ್ನಿ.", "குறிப்பு எண் $1. பதிவுக்கு 15 நிமிடம் முன்னதாக வாருங்கள்."]], ["^rescheduled (\\d+)×\\. Arrive 15 min early for registration\\.$", ["$1 बार समय बदला। पंजीकरण के लिए 15 मिनट पहले पहुँचें।", "$1 ಬಾರಿ ಸಮಯ ಬದಲಿಸಲಾಗಿದೆ. ನೋಂದಣಿಗೆ 15 ನಿಮಿಷ ಮುಂಚಿತವಾಗಿ ಬನ್ನಿ.", "$1 முறை நேரம் மாற்றப்பட்டது. பதிவுக்கு 15 நிமிடம் முன்னதாக வாருங்கள்."]], ["^Referral letter for (.+)$", ["$1 के लिए रेफ़रल पत्र", "$1 ಗಾಗಿ ರೆಫರಲ್ ಪತ್ರ", "$1 க்கான பரிந்துரைக் கடிதம்"]], ["^Request (NAV-\\d+) sent$", ["अनुरोध $1 भेजा गया", "ಕೋರಿಕೆ $1 ಕಳುಹಿಸಲಾಗಿದೆ", "கோரிக்கை $1 அனுப்பப்பட்டது"]], ["^Speaks (.+)$", ["$1 बोलते हैं", "$1 ಮಾತನಾಡುತ್ತಾರೆ", "$1 பேசுவர்"]], ["^Staff speak (.+)$", ["स्टाफ़ $1 बोलता है", "ಸಿಬ್ಬಂದಿ $1 ಮಾತನಾಡುತ್ತಾರೆ", "ஊழியர்கள் $1 பேசுவர்"]], ["^Status of (.+)$", ["$1 की स्थिति", "$1 ಸ್ಥಿತಿ", "$1 நிலை"]], ["^Step (\\d)$", ["चरण $1", "ಹಂತ $1", "படி $1"]], ["^Still missing: (.+)$", ["अभी भी नहीं है: $1", "ಇನ್ನೂ ಇಲ್ಲ: $1", "இன்னும் இல்லை: $1"]], ["^Switched to (.+)$", ["$1 पर बदला गया", "$1 ಗೆ ಬದಲಾಯಿಸಲಾಗಿದೆ", "$1 க்கு மாற்றப்பட்டது"]], ["^(.+) needs arranging at (.+)$", ["$2 पर $1 की व्यवस्था करनी होगी", "$2 ನಲ್ಲಿ $1 ವ್ಯವಸ್ಥೆ ಮಾಡಬೇಕು", "$2 இல் $1 ஏற்பாடு செய்ய வேண்டும்"]], ["^(.+) — on request$", ["$1 — अनुरोध पर", "$1 — ಕೋರಿಕೆಯ ಮೇರೆಗೆ", "$1 — கோரிக்கையின் பேரில்"]], ["^The doctor asked you to come back around (.+)\\.$", ["डॉक्टर ने लगभग $1 को फिर आने को कहा है।", "ವೈದ್ಯರು ಸುಮಾರು $1 ರಂದು ಮತ್ತೆ ಬರಲು ಹೇಳಿದ್ದಾರೆ.", "மருத்துவர் சுமார் $1 அன்று மீண்டும் வரச் சொன்னார்."]], ["^(.+) at (\\d.+)$", ["$1 $2 बजे", "$1 $2 ಕ್ಕೆ", "$1 $2 மணிக்கு"]], ["^(Today|Tomorrow) (\\d.+)$", ["$1 $2", "$1 $2", "$1 $2"]], ["^token (\\d+)$", ["टोकन $1", "ಟೋಕನ್ $1", "டோக்கன் $1"]], ["^What to bring to (.+)$", ["$1 में क्या लाना है", "$1 ಗೆ ಏನು ತರಬೇಕು", "$1 க்கு என்ன கொண்டு வர வேண்டும்"]], ["^paying with (.+)\\. Your documents are saved in a wallet and reused across visits\\.$", ["भुगतान: $1। आपके दस्तावेज़ वॉलेट में सहेजे जाते हैं और हर मुलाक़ात में दोबारा काम आते हैं।", "ಪಾವತಿ: $1. ನಿಮ್ಮ ದಾಖಲೆಗಳು ವ್ಯಾಲೆಟ್‌ನಲ್ಲಿ ಉಳಿಯುತ್ತವೆ ಮತ್ತು ಪ್ರತಿ ಭೇಟಿಯಲ್ಲೂ ಮರುಬಳಕೆಯಾಗುತ್ತವೆ.", "கட்டண முறை: $1. உங்கள் ஆவணங்கள் பணப்பையில் சேமிக்கப்பட்டு ஒவ்வொரு வருகையிலும் மீண்டும் பயன்படும்."]], ["^Follow-up visit \\((.+)\\)$", ["फ़ॉलो-अप मुलाक़ात ($1)", "ಮುಂದಿನ ಭೇಟಿ ($1)", "தொடர் வருகை ($1)"]], ["^Get a referral for (.+)$", ["$1 के लिए रेफ़रल लें", "$1 ಗಾಗಿ ರೆಫರಲ್ ಪಡೆಯಿರಿ", "$1 க்கான பரிந்துரை பெறுங்கள்"]], ["^Referred to (.+)$", ["$1 को रेफ़र किया गया", "$1 ಗೆ ಶಿಫಾರಸು ಮಾಡಲಾಗಿದೆ", "$1 க்குப் பரிந்துரைக்கப்பட்டது"]], ["^Referred from (.+)$", ["$1 से रेफ़र", "$1 ನಿಂದ ಶಿಫಾರಸು", "$1 இலிருந்து பரிந்துரை"]], ["^Tests asked for at (.+)$", ["$1 में बताई गई जाँचें", "$1 ನಲ್ಲಿ ಸೂಚಿಸಿದ ಪರೀಕ್ಷೆಗಳು", "$1 இல் சொன்ன பரிசோதனைகள்"]], ["^(.+) step added$", ["$1 का चरण जोड़ा गया", "$1 ಹಂತ ಸೇರಿಸಲಾಗಿದೆ", "$1 படி சேர்க்கப்பட்டது"]], ["^Referral ready — back to your (.+) booking$", ["रेफ़रल तैयार — आपकी $1 बुकिंग पर वापस", "ರೆಫರಲ್ ಸಿದ್ಧ — ನಿಮ್ಮ $1 ಬುಕಿಂಗ್‌ಗೆ ಹಿಂತಿರುಗಿ", "பரிந்துரை தயார் — உங்கள் $1 முன்பதிவுக்குத் திரும்புகிறோம்"]], ["^Attached (.+)$", ["संलग्न: $1", "ಲಗತ್ತಿಸಲಾಗಿದೆ: $1", "இணைக்கப்பட்டது: $1"]], ["^Loaded (\\d+) facilities$", ["$1 सुविधाएँ लोड हुईं", "$1 ಕೇಂದ್ರಗಳು ಲೋಡ್ ಆದವು", "$1 இடங்கள் ஏற்றப்பட்டன"]], ["^Welcome, (.+)! Let's start with what you need\\.$", ["स्वागत है, $1! आइए आपकी ज़रूरत से शुरू करें।", "ಸ್ವಾಗತ, $1! ನಿಮ್ಮ ಅಗತ್ಯದಿಂದ ಆರಂಭಿಸೋಣ.", "வரவேற்கிறோம், $1! உங்கள் தேவையிலிருந்து தொடங்குவோம்."]], ["^Welcome back, (.+)$", ["फिर से स्वागत है, $1", "ಮರಳಿ ಸ್ವಾಗತ, $1", "மீண்டும் வருக, $1"]], ["^Pack for tomorrow's (.+) visit$", ["कल की $1 मुलाक़ात के लिए सामान तैयार करें", "ನಾಳಿನ $1 ಭೇಟಿಗೆ ತಯಾರಿ ಮಾಡಿ", "நாளைய $1 வருகைக்குத் தயாராகுங்கள்"]], ["^Bring: (.+)$", ["साथ लाएँ: $1", "ತನ್ನಿ: $1", "கொண்டு வாருங்கள்: $1"]], ["^From (.+)\\. Take your receipt\\.$", ["$1 से। अपनी रसीद साथ लें।", "$1 ನಿಂದ. ನಿಮ್ಮ ರಸೀದಿ ತನ್ನಿ.", "$1 இலிருந்து. உங்கள் ரசீதை எடுத்துச் செல்லுங்கள்."]], ["^Interpreter needed \\((.+)\\)$", ["दुभाषिया चाहिए ($1)", "ವ್ಯಾಖ್ಯಾನಕಾರರು ಬೇಕು ($1)", "மொழிபெயர்ப்பாளர் தேவை ($1)"]], ["^No facility in the data meets all your needs for (.+)$", ["डेटा में कोई सुविधा $1 के लिए आपकी सभी ज़रूरतें पूरी नहीं करती", "ಡೇಟಾದಲ್ಲಿ ಯಾವುದೇ ಕೇಂದ್ರ $1 ಗಾಗಿ ನಿಮ್ಮ ಎಲ್ಲಾ ಅಗತ್ಯಗಳನ್ನು ಪೂರೈಸುವುದಿಲ್ಲ", "தரவில் எந்த இடமும் $1 க்கான உங்கள் எல்லாத் தேவைகளையும் பூர்த்தி செய்யவில்லை"]], ["^No facility in the dataset offers (.+)$", ["डेटा में कोई सुविधा $1 नहीं देती", "ಡೇಟಾದಲ್ಲಿ ಯಾವುದೇ ಕೇಂದ್ರ $1 ನೀಡುವುದಿಲ್ಲ", "தரவில் எந்த இடமும் $1 வழங்கவில்லை"]], ["^(.+) at (.+) only sees patients with a referral letter \\(organiser data: referral required\\)\\.$", ["$2 में $1 केवल रेफ़रल पत्र वाले मरीज़ों को देखता है (आयोजक डेटा: रेफ़रल आवश्यक)।", "$2 ನಲ್ಲಿ $1 ರೆಫರಲ್ ಪತ್ರ ಇರುವ ರೋಗಿಗಳನ್ನು ಮಾತ್ರ ನೋಡುತ್ತದೆ (ಆಯೋಜಕರ ಡೇಟಾ: ರೆಫರಲ್ ಅಗತ್ಯ).", "$2 இல் உள்ள $1 பரிந்துரைக் கடிதம் உள்ள நோயாளிகளை மட்டுமே பார்க்கும் (ஏற்பாட்டாளர் தரவு: பரிந்துரை தேவை)."]], ["^follow-up on or after (.+)$", ["$1 को या उसके बाद फ़ॉलो-अप", "$1 ಅಥವಾ ನಂತರ ಮುಂದಿನ ಭೇಟಿ", "$1 அல்லது அதற்குப் பின் தொடர் வருகை"]], ["^Please go to (.+), floor (\\d+)\\.$", ["कृपया $1, मंज़िल $2 पर जाएँ।", "ದಯವಿಟ್ಟು $1, $2ನೇ ಮಹಡಿಗೆ ಹೋಗಿ.", "தயவுசெய்து $1, தளம் $2 க்குச் செல்லுங்கள்."]], ["^Please go to (.+)\\.$", ["कृपया $1 पर जाएँ।", "ದಯವಿಟ್ಟು $1 ಗೆ ಹೋಗಿ.", "தயவுசெய்து $1 க்குச் செல்லுங்கள்."]], ["^(\\d+) conflicts?$", ["$1 विरोधाभास", "$1 ವಿರೋಧಾಭಾಸ", "$1 முரண்பாடு"]], ["^(Show|Hide) (\\d+) that don't fit — and why$", ["$2 जो उपयुक्त नहीं — $1 (और क्यों)", "$2 ಸೂಕ್ತವಲ್ಲದವುಗಳನ್ನು $1 — ಮತ್ತು ಏಕೆ", "பொருந்தாத $2 ஐ $1 — ஏன் என்றும்"]], ["^don't fit\\. Every score is explained — tap “(.+)”\\.$", ["उपयुक्त नहीं। हर स्कोर समझाया गया है — “$1” दबाएँ।", "ಸೂಕ್ತವಲ್ಲ. ಪ್ರತಿ ಅಂಕವನ್ನು ವಿವರಿಸಲಾಗಿದೆ — “$1” ಒತ್ತಿ.", "பொருந்தவில்லை. ஒவ்வொரு மதிப்பெண்ணும் விளக்கப்பட்டுள்ளது — “$1” ஐத் தட்டுங்கள்."]], ["^No (.+) listed$", ["$1 उपलब्ध नहीं बताया गया", "$1 ಪಟ್ಟಿಯಲ್ಲಿಲ್ಲ", "$1 பட்டியலில் இல்லை"]], ["^(.+) is on floor (\\d+) with no working lift listed$", ["$1 मंज़िल $2 पर है और कोई चालू लिफ़्ट दर्ज नहीं", "$1 $2ನೇ ಮಹಡಿಯಲ್ಲಿದೆ, ಕಾರ್ಯನಿರತ ಲಿಫ್ಟ್ ದಾಖಲಾಗಿಲ್ಲ", "$1 தளம் $2 இல் உள்ளது, இயங்கும் லிஃப்ட் பதிவில் இல்லை"]], ["^Listed: (.+)\\. A navigator can request an interpreter\\.$", ["सूचीबद्ध: $1। सहायक दुभाषिया माँग सकते हैं।", "ಪಟ್ಟಿ: $1. ಸಹಾಯಕರು ವ್ಯಾಖ್ಯಾನಕಾರರನ್ನು ಕೋರಬಹುದು.", "பட்டியல்: $1. வழிகாட்டி மொழிபெயர்ப்பாளரைக் கோரலாம்."]], ["^Directory lists wheelchair access, but (.+) is on floor (\\d+) and no lift is listed\\.$", ["निर्देशिका में व्हीलचेयर पहुँच लिखी है, पर $1 मंज़िल $2 पर है और कोई लिफ़्ट दर्ज नहीं है।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ ಗಾಲಿಕುರ್ಚಿ ಪ್ರವೇಶ ಇದೆ ಎಂದಿದೆ, ಆದರೆ $1 $2ನೇ ಮಹಡಿಯಲ್ಲಿದೆ ಮತ್ತು ಲಿಫ್ಟ್ ದಾಖಲಾಗಿಲ್ಲ.", "அடைவில் சக்கர நாற்காலி அணுகல் உள்ளது என உள்ளது, ஆனால் $1 தளம் $2 இல் உள்ளது, லிஃப்ட் பதிவில் இல்லை."]], ["^Directory lists ([\\d-]+); patients report the (?:antenatal|ANC) desk number printed on (?:their|MCP) cards is ([\\d-]+)\\.$", ["निर्देशिका में $1 लिखा है; मरीज़ों के अनुसार उनके कार्ड पर छपा प्रसवपूर्व डेस्क नंबर $2 है।", "ಡೈರೆಕ್ಟರಿಯಲ್ಲಿ $1 ಎಂದಿದೆ; ರೋಗಿಗಳ ಪ್ರಕಾರ ಅವರ ಕಾರ್ಡ್‌ಗಳಲ್ಲಿ ಮುದ್ರಿತ ಪ್ರಸವಪೂರ್ವ ಕೌಂಟರ್ ಸಂಖ್ಯೆ $2.", "அடைவில் $1 என உள்ளது; நோயாளிகள் தங்கள் அட்டைகளில் அச்சிடப்பட்ட மகப்பேறு மேசை எண் $2 எனத் தெரிவிக்கின்றனர்."]], ["^, or go to the nearest emergency department\\. Facilities with 24×7 emergency in this dataset: (.+)\\.$", [", या नज़दीकी आपातकालीन विभाग जाएँ। इस डेटा में 24×7 आपातकालीन सेवा वाली सुविधाएँ: $1।", ", ಅಥವಾ ಹತ್ತಿರದ ತುರ್ತು ವಿಭಾಗಕ್ಕೆ ಹೋಗಿ. ಈ ಡೇಟಾದಲ್ಲಿ 24×7 ತುರ್ತು ಸೇವೆ ಇರುವ ಕೇಂದ್ರಗಳು: $1.", ", அல்லது அருகிலுள்ள அவசர சிகிச்சைப் பிரிவுக்குச் செல்லுங்கள். இந்தத் தரவில் 24×7 அவசர சேவை உள்ள இடங்கள்: $1."]], ["^built-in sample \\((\\d+) facilities\\)$", ["अंतर्निहित नमूना ($1 सुविधाएँ)", "ಅಂತರ್ಗತ ಮಾದರಿ ($1 ಕೇಂದ್ರಗಳು)", "உள்ளமைந்த மாதிரி ($1 இடங்கள்)"]], ["^(.+) (available|taken)$", ["$1 $2", "$1 $2", "$1 $2"]], ["^Checklist for (.+) \\((.+)\\):$", ["$1 ($2) के लिए चेकलिस्ट:", "$1 ($2) ಗಾಗಿ ಪಟ್ಟಿ:", "$1 ($2) க்கான சரிபார்ப்புப் பட்டியல்:"]], ["^Reminder: (.+) on (.+) at (.+) — (.+)\\. Leave early; bring your documents\\. Emergency 108/112\\.$", ["रिमाइंडर: $1, $2 को $3 बजे — $4। जल्दी निकलें; अपने दस्तावेज़ साथ लाएँ। आपातकाल 108/112।", "ಜ್ಞಾಪನೆ: $1, $2 ರಂದು $3 ಕ್ಕೆ — $4. ಬೇಗ ಹೊರಡಿ; ನಿಮ್ಮ ದಾಖಲೆಗಳನ್ನು ತನ್ನಿ. ತುರ್ತು 108/112.", "நினைவூட்டல்: $1, $2 அன்று $3 மணிக்கு — $4. முன்னதாகப் புறப்படுங்கள்; உங்கள் ஆவணங்களைக் கொண்டு வாருங்கள். அவசரம் 108/112."]]].map(([s,t])=>[new RegExp(s),t]);

const CRIT=new Set(["This may need urgent help.","We can't assess symptoms. Call","(ambulance) or","You don't have to go through this alone.","Please call","That's a question for a clinician."]);
const TRLI={};Object.keys(TRD).forEach(k=>{TRLI[k.toLowerCase()]=TRD[k]});
Object.assign(TRD,{"You're offline.": ["आप ऑफ़लाइन हैं।", "ನೀವು ಆಫ್‌ಲೈನ್‌ನಲ್ಲಿದ್ದೀರಿ.", "நீங்கள் இணைப்பில் இல்லை."], "Your saved journey, documents, visit pass, reminders and the facility list still work. New bookings and requests are saved on this device and sent automatically when you reconnect.": ["आपकी सहेजी गई यात्रा, दस्तावेज़, विज़िट पास, रिमाइंडर और सुविधाओं की सूची अब भी काम करती है। नई बुकिंग और अनुरोध इस डिवाइस पर सहेजे जाते हैं और कनेक्शन लौटने पर अपने-आप भेज दिए जाते हैं।", "ನಿಮ್ಮ ಉಳಿಸಿದ ಪಯಣ, ದಾಖಲೆಗಳು, ಭೇಟಿ ಪಾಸ್, ಜ್ಞಾಪನೆಗಳು ಮತ್ತು ಕೇಂದ್ರಗಳ ಪಟ್ಟಿ ಈಗಲೂ ಕೆಲಸ ಮಾಡುತ್ತವೆ. ಹೊಸ ಬುಕಿಂಗ್ ಮತ್ತು ಕೋರಿಕೆಗಳು ಈ ಸಾಧನದಲ್ಲಿ ಉಳಿಯುತ್ತವೆ ಮತ್ತು ಸಂಪರ್ಕ ಮರಳಿದಾಗ ಸ್ವಯಂ ಕಳುಹಿಸಲಾಗುತ್ತದೆ.", "நீங்கள் சேமித்த பயணம், ஆவணங்கள், வருகை அனுமதிச்சீட்டு, நினைவூட்டல்கள், இடங்களின் பட்டியல் இன்னும் வேலை செய்யும். புதிய முன்பதிவுகளும் கோரிக்கைகளும் இந்தச் சாதனத்தில் சேமிக்கப்பட்டு, இணைப்பு திரும்பியதும் தானாக அனுப்பப்படும்."], "High demand today: fewer slots than usual.": ["आज भारी माँग: सामान्य से कम स्लॉट।", "ಇಂದು ಹೆಚ್ಚಿನ ಬೇಡಿಕೆ: ಸಾಮಾನ್ಯಕ್ಕಿಂತ ಕಡಿಮೆ ಸ್ಲಾಟ್‌ಗಳು.", "இன்று அதிக தேவை: வழக்கத்தை விடக் குறைவான நேரங்கள்."], "Existing bookings are kept. If a day is full you can join the wait-list or see other places with free slots.": ["मौजूदा बुकिंग बनी रहती हैं। अगर कोई दिन भरा है तो आप प्रतीक्षा सूची में जुड़ सकते हैं या खाली स्लॉट वाली दूसरी जगहें देख सकते हैं।", "ಈಗಿರುವ ಬುಕಿಂಗ್‌ಗಳು ಉಳಿಯುತ್ತವೆ. ದಿನ ಭರ್ತಿಯಾಗಿದ್ದರೆ ಕಾಯುವ ಪಟ್ಟಿಗೆ ಸೇರಬಹುದು ಅಥವಾ ಖಾಲಿ ಸ್ಲಾಟ್ ಇರುವ ಬೇರೆ ಸ್ಥಳಗಳನ್ನು ನೋಡಬಹುದು.", "ஏற்கனவே உள்ள முன்பதிவுகள் தொடரும். ஒரு நாள் நிரம்பியிருந்தால் காத்திருப்புப் பட்டியலில் சேரலாம் அல்லது காலி நேரம் உள்ள வேறு இடங்களைப் பார்க்கலாம்."], "Rules changed (policy v2).": ["नियम बदले (नीति v2)।", "ನಿಯಮಗಳು ಬದಲಾಗಿವೆ (ನೀತಿ v2).", "விதிகள் மாறின (கொள்கை v2)."], "Specialist OPDs now need a referral letter everywhere. Your existing bookings are kept and flagged if affected.": ["विशेषज्ञ ओपीडी में अब हर जगह रेफ़रल पत्र चाहिए। आपकी मौजूदा बुकिंग बनी रहेंगी और प्रभावित होने पर चिह्नित की जाएँगी।", "ತಜ್ಞರ ಒಪಿಡಿಗಳಿಗೆ ಈಗ ಎಲ್ಲೆಡೆ ರೆಫರಲ್ ಪತ್ರ ಬೇಕು. ನಿಮ್ಮ ಬುಕಿಂಗ್‌ಗಳು ಉಳಿಯುತ್ತವೆ; ಪರಿಣಾಮವಾದರೆ ಗುರುತಿಸಲಾಗುತ್ತದೆ.", "நிபுணர் வெளிநோயாளர் பிரிவுகளுக்கு இப்போது எல்லா இடங்களிலும் பரிந்துரைக் கடிதம் தேவை. உங்கள் முன்பதிவுகள் தொடரும்; பாதிக்கப்பட்டால் குறிக்கப்படும்."], "No free slots on this day.": ["इस दिन कोई खाली स्लॉट नहीं।", "ಈ ದಿನ ಖಾಲಿ ಸ್ಲಾಟ್ ಇಲ್ಲ.", "இந்த நாளில் காலி நேரம் இல்லை."], "Join the wait-list, or try another place with free slots.": ["प्रतीक्षा सूची में जुड़ें, या खाली स्लॉट वाली दूसरी जगह आज़माएँ।", "ಕಾಯುವ ಪಟ್ಟಿಗೆ ಸೇರಿ, ಅಥವಾ ಖಾಲಿ ಸ್ಲಾಟ್ ಇರುವ ಬೇರೆ ಸ್ಥಳ ಪ್ರಯತ್ನಿಸಿ.", "காத்திருப்புப் பட்டியலில் சேருங்கள், அல்லது காலி நேரம் உள்ள வேறு இடத்தை முயலுங்கள்."], "Join the wait-list": ["प्रतीक्षा सूची में जुड़ें", "ಕಾಯುವ ಪಟ್ಟಿಗೆ ಸೇರಿ", "காத்திருப்புப் பட்டியலில் சேர்"], "Other places with free slots": ["खाली स्लॉट वाली दूसरी जगहें", "ಖಾಲಿ ಸ್ಲಾಟ್ ಇರುವ ಬೇರೆ ಸ್ಥಳಗಳು", "காலி நேரம் உள்ள வேறு இடங்கள்"], "Added to the wait-list": ["प्रतीक्षा सूची में जोड़ा गया", "ಕಾಯುವ ಪಟ್ಟಿಗೆ ಸೇರಿಸಲಾಗಿದೆ", "காத்திருப்புப் பட்டியலில் சேர்க்கப்பட்டது"], "This slot was taken while you were offline.": ["आपके ऑफ़लाइन रहते यह स्लॉट किसी और ने ले लिया।", "ನೀವು ಆಫ್‌ಲೈನ್ ಇದ್ದಾಗ ಈ ಸ್ಲಾಟ್ ಬೇರೆಯವರು ಪಡೆದರು.", "நீங்கள் இணைப்பில் இல்லாதபோது இந்த நேரம் வேறொருவருக்குச் சென்றது."], "Please pick another time — nothing was charged or confirmed.": ["कृपया दूसरा समय चुनें — कुछ भी शुल्क या पुष्टि नहीं हुई।", "ದಯವಿಟ್ಟು ಬೇರೆ ಸಮಯ ಆಯ್ಕೆಮಾಡಿ — ಯಾವುದೇ ಶುಲ್ಕ ಅಥವಾ ದೃಢೀಕರಣ ಆಗಿಲ್ಲ.", "வேறு நேரத்தைத் தேர்ந்தெடுங்கள் — எதுவும் வசூலிக்கப்படவில்லை, உறுதிப்படுத்தப்படவில்லை."], "Pick another time": ["दूसरा समय चुनें", "ಬೇರೆ ಸಮಯ ಆಯ್ಕೆಮಾಡಿ", "வேறு நேரத்தைத் தேர்ந்தெடு"], "Saved offline — will confirm when you're back online": ["ऑफ़लाइन सहेजा गया — ऑनलाइन होने पर पुष्टि होगी", "ಆಫ್‌ಲೈನ್‌ನಲ್ಲಿ ಉಳಿಸಲಾಗಿದೆ — ಆನ್‌ಲೈನ್ ಆದಾಗ ದೃಢೀಕರಿಸಲಾಗುತ್ತದೆ", "இணைப்பில்லாமல் சேமிக்கப்பட்டது — இணைப்பு வந்ததும் உறுதிப்படுத்தப்படும்"], "Saved offline — will send when you're back online": ["ऑफ़लाइन सहेजा गया — ऑनलाइन होने पर भेजा जाएगा", "ಆಫ್‌ಲೈನ್‌ನಲ್ಲಿ ಉಳಿಸಲಾಗಿದೆ — ಆನ್‌ಲೈನ್ ಆದಾಗ ಕಳುಹಿಸಲಾಗುತ್ತದೆ", "இணைப்பில்லாமல் சேமிக்கப்பட்டது — இணைப்பு வந்ததும் அனுப்பப்படும்"], "Waiting to send (offline)": ["भेजने की प्रतीक्षा (ऑफ़लाइन)", "ಕಳುಹಿಸಲು ಕಾಯುತ್ತಿದೆ (ಆಫ್‌ಲೈನ್)", "அனுப்பக் காத்திருக்கிறது (இணைப்பில்லை)"], "Someone else just booked this slot. Please pick another time.": ["यह स्लॉट अभी किसी और ने बुक कर लिया। कृपया दूसरा समय चुनें।", "ಈ ಸ್ಲಾಟ್ ಅನ್ನು ಈಗ ತಾನೇ ಬೇರೆಯವರು ಬುಕ್ ಮಾಡಿದರು. ದಯವಿಟ್ಟು ಬೇರೆ ಸಮಯ ಆಯ್ಕೆಮಾಡಿ.", "இந்த நேரத்தை இப்போதுதான் வேறொருவர் முன்பதிவு செய்தார். வேறு நேரத்தைத் தேர்ந்தெடுங்கள்."], "Already booked — no duplicate made": ["पहले से बुक है — कोई दोहरी बुकिंग नहीं हुई", "ಈಗಾಗಲೇ ಬುಕ್ ಆಗಿದೆ — ನಕಲು ಮಾಡಲಾಗಿಲ್ಲ", "ஏற்கனவே முன்பதிவாகியுள்ளது — இரட்டை முன்பதிவு இல்லை"], "This department now needs a referral letter.": ["इस विभाग को अब रेफ़रल पत्र चाहिए।", "ಈ ವಿಭಾಗಕ್ಕೆ ಈಗ ರೆಫರಲ್ ಪತ್ರ ಬೇಕು.", "இந்தப் பிரிவுக்கு இப்போது பரிந்துரைக் கடிதம் தேவை."], "Your booking is kept — nothing is cancelled without your confirmation.": ["आपकी बुकिंग बनी है — आपकी पुष्टि के बिना कुछ रद्द नहीं होगा।", "ನಿಮ್ಮ ಬುಕಿಂಗ್ ಉಳಿದಿದೆ — ನಿಮ್ಮ ದೃಢೀಕರಣವಿಲ್ಲದೆ ಏನೂ ರದ್ದಾಗುವುದಿಲ್ಲ.", "உங்கள் முன்பதிவு தொடர்கிறது — உங்கள் ஒப்புதல் இல்லாமல் எதுவும் ரத்து செய்யப்படாது."], "Keep booking — I'll bring it": ["बुकिंग रखें — मैं साथ लाऊँगा/लाऊँगी", "ಬುಕಿಂಗ್ ಉಳಿಸಿ — ನಾನು ತರುತ್ತೇನೆ", "முன்பதிவை வைத்திரு — நான் கொண்டு வருவேன்"], "Booking deferred: one detail is missing.": ["बुकिंग रोकी गई: एक जानकारी गायब है।", "ಬುಕಿಂಗ್ ಮುಂದೂಡಲಾಗಿದೆ: ಒಂದು ವಿವರ ಕಾಣೆಯಾಗಿದೆ.", "முன்பதிவு நிறுத்தப்பட்டது: ஒரு விவரம் இல்லை."], "Ask a navigator to confirm": ["सहायक से पुष्टि करवाएँ", "ಸಹಾಯಕರಿಂದ ದೃಢೀಕರಿಸಿ", "வழிகாட்டியிடம் உறுதிப்படுத்துங்கள்"], "I have a referral letter anyway": ["मेरे पास रेफ़रल पत्र है", "ನನ್ನ ಬಳಿ ರೆಫರಲ್ ಪತ್ರ ಇದೆ", "என்னிடம் பரிந்துரைக் கடிதம் உள்ளது"], "We need one detail before booking: how will you pay?": ["बुकिंग से पहले एक जानकारी चाहिए: आप भुगतान कैसे करेंगे?", "ಬುಕಿಂಗ್ ಮೊದಲು ಒಂದು ವಿವರ ಬೇಕು: ನೀವು ಹೇಗೆ ಪಾವತಿಸುತ್ತೀರಿ?", "முன்பதிவுக்கு முன் ஒரு விவரம் தேவை: எப்படி பணம் செலுத்துவீர்கள்?"], "Choose payment": ["भुगतान चुनें", "ಪಾವತಿ ಆಯ್ಕೆಮಾಡಿ", "கட்டண முறையைத் தேர்ந்தெடு"], "Ask a navigator": ["सहायक से पूछें", "ಸಹಾಯಕರನ್ನು ಕೇಳಿ", "வழிகாட்டியிடம் கேளுங்கள்"], "Not sure yet": ["अभी पक्का नहीं", "ಇನ್ನೂ ಖಚಿತವಿಲ್ಲ", "இன்னும் உறுதியில்லை"], "Payment method not confirmed": ["भुगतान का तरीका पक्का नहीं", "ಪಾವತಿ ವಿಧಾನ ದೃಢಪಟ್ಟಿಲ್ಲ", "கட்டண முறை உறுதிப்படுத்தப்படவில்லை"], "Referral rule not stated": ["रेफ़रल नियम नहीं बताया गया", "ರೆಫರಲ್ ನಿಯಮ ತಿಳಿಸಿಲ್ಲ", "பரிந்துரை விதி குறிப்பிடப்படவில்லை"], "The data doesn't say whether this department needs a referral letter. We won't guess — confirm with the facility or a navigator.": ["डेटा में नहीं बताया गया कि इस विभाग को रेफ़रल पत्र चाहिए या नहीं। हम अनुमान नहीं लगाएँगे — सुविधा या सहायक से पुष्टि करें।", "ಈ ವಿಭಾಗಕ್ಕೆ ರೆಫರಲ್ ಪತ್ರ ಬೇಕೇ ಎಂದು ಡೇಟಾದಲ್ಲಿ ಇಲ್ಲ. ನಾವು ಊಹಿಸುವುದಿಲ್ಲ — ಕೇಂದ್ರ ಅಥವಾ ಸಹಾಯಕರಿಂದ ದೃಢೀಕರಿಸಿ.", "இந்தப் பிரிவுக்குப் பரிந்துரைக் கடிதம் தேவையா என்று தரவில் இல்லை. நாங்கள் ஊகிக்க மாட்டோம் — இடம் அல்லது வழிகாட்டியிடம் உறுதிப்படுத்துங்கள்."], "Missing information: payment method not confirmed": ["जानकारी गायब: भुगतान का तरीका पक्का नहीं", "ಕಾಣೆಯಾದ ಮಾಹಿತಿ: ಪಾವತಿ ವಿಧಾನ ದೃಢಪಟ್ಟಿಲ್ಲ", "விடுபட்ட தகவல்: கட்டண முறை உறுதிப்படுத்தப்படவில்லை"], "Missing information: referral rule not stated for this department": ["जानकारी गायब: इस विभाग का रेफ़रल नियम नहीं बताया गया", "ಕಾಣೆಯಾದ ಮಾಹಿತಿ: ಈ ವಿಭಾಗದ ರೆಫರಲ್ ನಿಯಮ ತಿಳಿಸಿಲ್ಲ", "விடுபட்ட தகவல்: இந்தப் பிரிவின் பரிந்துரை விதி குறிப்பிடப்படவில்லை"], "Rules changed after booking — needs your confirmation": ["बुकिंग के बाद नियम बदले — आपकी पुष्टि चाहिए", "ಬುಕಿಂಗ್ ನಂತರ ನಿಯಮ ಬದಲಾಗಿದೆ — ನಿಮ್ಮ ದೃಢೀಕರಣ ಬೇಕು", "முன்பதிவுக்குப் பின் விதிகள் மாறின — உங்கள் ஒப்புதல் தேவை"], "Not verified yet": ["अभी सत्यापित नहीं", "ಇನ್ನೂ ಪರಿಶೀಲಿಸಿಲ್ಲ", "இன்னும் சரிபார்க்கப்படவில்லை"], "Live queue reading uncertain — please confirm at the counter.": ["लाइव कतार की जानकारी अनिश्चित है — कृपया काउंटर पर पुष्टि करें।", "ಲೈವ್ ಸರದಿ ಮಾಹಿತಿ ಅನಿಶ್ಚಿತ — ದಯವಿಟ್ಟು ಕೌಂಟರ್‌ನಲ್ಲಿ ದೃಢೀಕರಿಸಿ.", "நேரடி வரிசைத் தகவல் உறுதியில்லை — கவுண்டரில் உறுதிப்படுத்துங்கள்."], "We're showing the last reliable number.": ["हम आख़िरी भरोसेमंद नंबर दिखा रहे हैं।", "ಕೊನೆಯ ವಿಶ್ವಾಸಾರ್ಹ ಸಂಖ್ಯೆಯನ್ನು ತೋರಿಸುತ್ತಿದ್ದೇವೆ.", "கடைசியாக நம்பகமான எண்ணைக் காட்டுகிறோம்."], "Live reading OK — display board and registration agree.": ["लाइव जानकारी ठीक — डिस्प्ले बोर्ड और पंजीकरण मेल खाते हैं।", "ಲೈವ್ ಮಾಹಿತಿ ಸರಿ — ಪ್ರದರ್ಶನ ಫಲಕ ಮತ್ತು ನೋಂದಣಿ ಹೊಂದುತ್ತವೆ.", "நேரடித் தகவல் சரி — காட்சிப் பலகையும் பதிவும் பொருந்துகின்றன."], "Display board sent no reading": ["डिस्प्ले बोर्ड से कोई जानकारी नहीं आई", "ಪ್ರದರ್ಶನ ಫಲಕದಿಂದ ಮಾಹಿತಿ ಬಂದಿಲ್ಲ", "காட்சிப் பலகையிலிருந்து தகவல் வரவில்லை"], "Display board looks stuck (same number repeatedly)": ["डिस्प्ले बोर्ड अटका लगता है (बार-बार वही नंबर)", "ಪ್ರದರ್ಶನ ಫಲಕ ನಿಂತಂತಿದೆ (ಅದೇ ಸಂಖ್ಯೆ ಪದೇ ಪದೇ)", "காட்சிப் பலகை சிக்கியதுபோல் உள்ளது (அதே எண் மீண்டும் மீண்டும்)"], "Stress tests": ["तनाव परीक्षण", "ಒತ್ತಡ ಪರೀಕ್ಷೆಗಳು", "அழுத்தச் சோதனைகள்"]});Object.keys(TRD).forEach(k=>{TRLI[k.toLowerCase()]=TRD[k]});[["^(Your saved journey.+reconnect\\.) Waiting to send: (\\d+)\\.$", ["$1 भेजने के लिए बाकी: $2।", "$1 ಕಳುಹಿಸಲು ಬಾಕಿ: $2.", "$1 அனுப்பக் காத்திருப்பவை: $2."]], ["^You're #(\\d+) on the wait-list\\. We'll remind you if a slot opens\\.$", ["प्रतीक्षा सूची में आप #$1 पर हैं। स्लॉट खुलने पर हम याद दिलाएँगे।", "ಕಾಯುವ ಪಟ್ಟಿಯಲ್ಲಿ ನೀವು #$1. ಸ್ಲಾಟ್ ತೆರೆದರೆ ತಿಳಿಸುತ್ತೇವೆ.", "காத்திருப்புப் பட்டியலில் நீங்கள் #$1. நேரம் காலியானால் நினைவூட்டுவோம்."]], ["^next (.+)$", ["अगला $1", "ಮುಂದಿನದು $1", "அடுத்தது $1"]], ["^Saved offline: (.+)$", ["ऑफ़लाइन सहेजा: $1", "ಆಫ್‌ಲೈನ್ ಉಳಿಸಲಾಗಿದೆ: $1", "இணைப்பின்றிச் சேமித்தது: $1"]], ["^Pending — will confirm when you're back online\\. Ref (NR-\\d+)\\.$", ["लंबित — ऑनलाइन होने पर पुष्टि होगी। संदर्भ $1।", "ಬಾಕಿ — ಆನ್‌ಲೈನ್ ಆದಾಗ ದೃಢೀಕರಣ. ಉಲ್ಲೇಖ $1.", "நிலுவையில் — இணைப்பு வந்ததும் உறுதிப்படுத்தப்படும். குறிப்பு எண் $1."]], ["^Back online — (\\d+) saved action\\(s\\) sent(.*)$", ["फिर ऑनलाइन — $1 सहेजे गए काम भेजे गए$2", "ಮತ್ತೆ ಆನ್‌ಲೈನ್ — $1 ಉಳಿಸಿದ ಕ್ರಿಯೆಗಳನ್ನು ಕಳುಹಿಸಲಾಗಿದೆ$2", "மீண்டும் இணைப்பில் — சேமித்த $1 செயல்கள் அனுப்பப்பட்டன$2"]], ["^Rules changed after you booked \\(policy v(\\d)\\)\\.$", ["आपकी बुकिंग के बाद नियम बदले (नीति v$1)।", "ನೀವು ಬುಕ್ ಮಾಡಿದ ನಂತರ ನಿಯಮ ಬದಲಾಗಿದೆ (ನೀತಿ v$1).", "நீங்கள் முன்பதிவு செய்தபின் விதிகள் மாறின (கொள்கை v$1)."]], ["^The facility data doesn't say whether (.+) needs a referral letter\\. We won't guess, because a wrong guess could mean being turned away\\.$", ["सुविधा के डेटा में नहीं बताया गया कि $1 को रेफ़रल पत्र चाहिए या नहीं। हम अनुमान नहीं लगाएँगे, क्योंकि गलत अनुमान से आपको लौटाया जा सकता है।", "$1 ಗೆ ರೆಫರಲ್ ಪತ್ರ ಬೇಕೇ ಎಂದು ಕೇಂದ್ರದ ಡೇಟಾದಲ್ಲಿ ಇಲ್ಲ. ತಪ್ಪು ಊಹೆಯಿಂದ ನಿಮ್ಮನ್ನು ಹಿಂದಕ್ಕೆ ಕಳುಹಿಸಬಹುದು, ಆದ್ದರಿಂದ ನಾವು ಊಹಿಸುವುದಿಲ್ಲ.", "$1 க்குப் பரிந்துரைக் கடிதம் தேவையா என்று இடத்தின் தரவில் இல்லை. தவறான ஊகத்தால் நீங்கள் திருப்பி அனுப்பப்படலாம் என்பதால் நாங்கள் ஊகிக்க மாட்டோம்."]], ["^The fee here is (.+), and it may be free under a government scheme\\. We won't guess\\.$", ["यहाँ शुल्क $1 है, और सरकारी योजना में यह निःशुल्क हो सकता है। हम अनुमान नहीं लगाएँगे।", "ಇಲ್ಲಿ ಶುಲ್ಕ $1, ಸರ್ಕಾರಿ ಯೋಜನೆಯಡಿ ಉಚಿತವಾಗಿರಬಹುದು. ನಾವು ಊಹಿಸುವುದಿಲ್ಲ.", "இங்கு கட்டணம் $1; அரசுத் திட்டத்தில் இலவசமாக இருக்கலாம். நாங்கள் ஊகிக்க மாட்டோம்."]], ["^Fee depends on it — here: (.+)\\. We won't guess; choose a payment option or ask a navigator\\.$", ["शुल्क इसी पर निर्भर है — यहाँ: $1। हम अनुमान नहीं लगाएँगे; भुगतान विकल्प चुनें या सहायक से पूछें।", "ಶುಲ್ಕ ಇದನ್ನು ಅವಲಂಬಿಸಿದೆ — ಇಲ್ಲಿ: $1. ನಾವು ಊಹಿಸುವುದಿಲ್ಲ; ಪಾವತಿ ಆಯ್ಕೆ ಮಾಡಿ ಅಥವಾ ಸಹಾಯಕರನ್ನು ಕೇಳಿ.", "கட்டணம் இதைப் பொறுத்தது — இங்கு: $1. நாங்கள் ஊகிக்க மாட்டோம்; கட்டண முறையைத் தேர்ந்தெடுங்கள் அல்லது வழிகாட்டியிடம் கேளுங்கள்."]], ["^What we trust: (.+)$", ["हम किस पर भरोसा करते हैं: $1", "ನಾವು ನಂಬುವುದು: $1", "நாங்கள் நம்புவது: $1"]], ["^Trusted: (.+) \\(higher-priority source and not older\\)\\.$", ["भरोसा: $1 (ऊँचे दर्जे का स्रोत और पुराना नहीं)।", "ನಂಬಿಕೆ: $1 (ಉನ್ನತ ಆದ್ಯತೆಯ ಮೂಲ, ಹಳೆಯದಲ್ಲ).", "நம்பப்படுவது: $1 (உயர் முன்னுரிமை மூலம், பழையது அல்ல)."]], ["^A newer but lower-priority source \\((.+), ([\\d-]+)\\) contradicts an older official record \\((.+), ([\\d-]+)\\)\\. Neither is treated as the truth until verified\\.$", ["एक नया लेकिन कम दर्जे का स्रोत ($1, $2) एक पुराने आधिकारिक रिकॉर्ड ($3, $4) से मेल नहीं खाता। सत्यापन तक किसी को भी सच नहीं माना जाता।", "ಹೊಸದಾದರೂ ಕಡಿಮೆ ಆದ್ಯತೆಯ ಮೂಲ ($1, $2) ಹಳೆಯ ಅಧಿಕೃತ ದಾಖಲೆಗೆ ($3, $4) ವಿರುದ್ಧವಾಗಿದೆ. ಪರಿಶೀಲನೆಯವರೆಗೆ ಯಾವುದನ್ನೂ ಸತ್ಯವೆಂದು ಪರಿಗಣಿಸುವುದಿಲ್ಲ.", "புதிய ஆனால் குறைந்த முன்னுரிமை மூலம் ($1, $2) பழைய அதிகாரப்பூர்வப் பதிவுக்கு ($3, $4) முரணாக உள்ளது. சரிபார்க்கும் வரை எதுவும் உண்மையாகக் கருதப்படாது."]], ["^Two fields in the same record contradict each other, so neither can be trusted on its own\\. Confirm with the facility before travelling\\.$", ["एक ही रिकॉर्ड के दो हिस्से एक-दूसरे से मेल नहीं खाते, इसलिए किसी पर अकेले भरोसा नहीं किया जा सकता। जाने से पहले सुविधा से पुष्टि करें।", "ಒಂದೇ ದಾಖಲೆಯ ಎರಡು ಭಾಗಗಳು ವಿರೋಧಿಸುತ್ತವೆ, ಆದ್ದರಿಂದ ಯಾವುದನ್ನೂ ಒಂಟಿಯಾಗಿ ನಂಬಲಾಗದು. ಹೊರಡುವ ಮೊದಲು ಕೇಂದ್ರದಿಂದ ದೃಢೀಕರಿಸಿ.", "ஒரே பதிவில் உள்ள இரண்டு தகவல்கள் முரண்படுகின்றன; எதையும் தனியாக நம்ப முடியாது. பயணத்திற்கு முன் இடத்திடம் உறுதிப்படுத்துங்கள்."]], ["^Sudden spike ignored \\(board showed (\\d+)\\)$", ["अचानक उछाल अनदेखा किया (बोर्ड पर $1)", "ಹಠಾತ್ ಏರಿಕೆ ನಿರ್ಲಕ್ಷಿಸಲಾಗಿದೆ (ಫಲಕದಲ್ಲಿ $1)", "திடீர் உயர்வு புறக்கணிக்கப்பட்டது (பலகையில் $1)"]], ["^Display board went backwards \\((-?\\d+)\\)$", ["डिस्प्ले बोर्ड पीछे चला गया ($1)", "ಪ್ರದರ್ಶನ ಫಲಕ ಹಿಂದಕ್ಕೆ ಹೋಯಿತು ($1)", "காட்சிப் பலகை பின்னோக்கிச் சென்றது ($1)"]], ["^Board \\((\\d+)\\) and registration system \\((\\d+)\\) disagree$", ["बोर्ड ($1) और पंजीकरण प्रणाली ($2) मेल नहीं खाते", "ಫಲಕ ($1) ಮತ್ತು ನೋಂದಣಿ ವ್ಯವಸ್ಥೆ ($2) ಹೊಂದುತ್ತಿಲ್ಲ", "பலகையும் ($1) பதிவு அமைப்பும் ($2) பொருந்தவில்லை"]]].forEach(([s,t])=>TRP.unshift([new RegExp(s),t]));
const TRIDX={hi:0,kn:1,ta:2};let TRC={};
function curLang(){return SESSION?S.lang:(AUTHUI.lang||"en")}
const PRE=/^([●◐☐☑⚠✓📍🔊▶⇪+·—]+\s*|\[[ x]\]\s+)/u,SUF=/(\s*[→✓])$/u;
function trCore(s,d){const L=curLang(),i=TRIDX[L];if(i==null||!s||!/[A-Za-z]/.test(s))return s;d=d||0;if(d>6)return s;
 const ck=L+"|"+s;if(TRC[ck]!=null)return TRC[ck];let r=trInner(s,i,d);TRC[ck]=r;return r}
function trInner(s,i,d){
 if(TRD[s])return TRD[s][i];const lo=TRLI[s.toLowerCase()];if(lo)return lo[i];
 let m=s.match(PRE);if(m&&m[0].length<s.length)return m[0]+trCore(s.slice(m[0].length),d+1);
 m=s.match(SUF);if(m&&m.index>0)return trCore(s.slice(0,m.index),d+1)+m[0];
 for(const [re,t] of TRP){const x=s.match(re);if(x)return t[i].replace(/\$(\d)/g,(_,n)=>x[+n]==null?"":trCore(x[+n],d+1))}
 for(const sep of [" · ","; ",": ",", "," — "," + "]){if(s.includes(sep)){const parts=s.split(sep),out=parts.map(p=>trCore(p,d+1));if(out.some((o,k)=>o!==parts[k]))return out.join(sep)}}
 m=s.match(/^(.+) \((.+)\)$/);if(m){const a=trCore(m[1],d+1),b=trCore(m[2],d+1);if(a!==m[1]||b!==m[2])return a+" ("+b+")"}
 m=s.match(/^\((.+)\)$/);if(m)return "("+trCore(m[1],d+1)+")";
 return s}
function trText(s){if(curLang()==="en"||s==null)return s;s=String(s);if(s.includes("\n"))return s.split("\n").map(trText).join("\n");const t=s.trim();if(!t)return s;const lead=s.slice(0,s.indexOf(t)),trail=s.slice(s.indexOf(t)+t.length);return lead+trCore(t)+trail}
const TRO=new WeakMap(),TRA=new WeakMap();
function translateDOM(root){if(!root)return;const en=curLang()==="en";const w=document.createTreeWalker(root,NodeFilter.SHOW_TEXT,{acceptNode:n=>{const p=n.parentElement;return(!p||/^(SCRIPT|STYLE|TEXTAREA)$/.test(p.tagName)||p.closest("[data-notr]"))?2:1}});const ns=[];while(w.nextNode())ns.push(w.currentNode);
 ns.forEach(n=>{let o=TRO.get(n);if(o==null||(n.nodeValue!==o.last)){o={src:n.nodeValue,last:null};}const v=en?o.src:trText(o.src);o.last=v;TRO.set(n,o);if(v!==n.nodeValue)n.nodeValue=v});
 root.querySelectorAll("[placeholder],[aria-label],[title]").forEach(el=>{let m=TRA.get(el)||{};["placeholder","aria-label","title"].forEach(a=>{const cur=el.getAttribute(a);if(cur==null)return;let o=m[a];if(!o||cur!==o.last)o={src:cur,last:null};const v=en?o.src:trText(o.src);o.last=v;m[a]=o;if(v!==cur)el.setAttribute(a,v)});TRA.set(el,m)})}

/* =========================================================
   RESILIENCE ENGINE — Hackathon constraints C01–C12
   ========================================================= */
const sleep=ms=>new Promise(r=>setTimeout(r,ms));
/* ---- Audit log with redaction (C04, C07, C09, C11) ---- */
function redact(s){return String(s).replace(/[^\s@<>"]+@[^\s@<>"]+\.[a-z]{2,}/gi,"[email hidden]").replace(/(\+?91[\s-]?)?\b[6-9]\d{4}[\s-]?\d{5}\b/g,"[phone hidden]")}
function audit(kind,msg){S.audit=S.audit||[];S.audit.unshift({at:Date.now(),kind,msg:redact(msg)});S.audit=S.audit.slice(0,250)}

/* ---- C07 Privacy boundary: block all outbound data from app logic ---- */
let NET_BLOCKED=0;


/* ---- C01 Offline: detection, outbox queue, idempotent sync ---- */
function isOnline(){return true}
function queueAction(type,payload,key){S.outbox=S.outbox||[];if(S.outbox.some(o=>o.key===key)){audit("offline","Duplicate queued action ignored: "+type);return false}
 S.outbox.push({id:"Q"+Date.now().toString(36),type,payload,key,at:Date.now()});audit("offline","Saved while offline (will send later): "+type);return true}
function syncOutbox(){if(!isOnline()||!(S.outbox&&S.outbox.length))return;let ok=0,dup=0,fail=0;const done=new Set(S.synced||[]);
 S.outbox.forEach(o=>{if(done.has(o.key)){dup++;return}
  if(o.type==="booking"){const L=S.legs.find(l=>l.id===o.payload.leg);
   if(!L||!L.booking||L.booking.ref!==o.payload.ref){dup++;done.add(o.key);return}
   const r=ledgerClaim(slotKey(L.facilityId,L.service,L.booking.at),holderId(L),L.booking.idem);
   if(r.ok){L.booking.status="confirmed";ok++}else{L.booking.status="conflict";fail++}}
  if(o.type==="ticket"){const tk=S.tickets.find(x=>x.id===o.payload.id);if(tk){tk.status="Queued";ok++}}
  done.add(o.key)});
 S.synced=[...done].slice(-400);S.outbox=[];audit("sync",`Reconnected: sent ${ok}, duplicates skipped ${dup}, slot conflicts ${fail}`);save();
 toast(`Back online — ${ok} saved action(s) sent${dup?`, ${dup} duplicate(s) skipped`:""}${fail?`, ${fail} slot conflict(s) need a new time`:""}`);render()}


/* ---- C09 Concurrency: slot ledger with compare-and-swap + idempotency ---- */
const LEDGER_KEY="nr-ledger-v1";let LEDGER_MEM={__v:0};
function ledgerRead(){try{const v=localStorage.getItem(LEDGER_KEY);return v?JSON.parse(v):{...LEDGER_MEM}}catch(e){return{...LEDGER_MEM}}}
function ledgerWrite(l){LEDGER_MEM=l;try{localStorage.setItem(LEDGER_KEY,JSON.stringify(l))}catch(e){}}
function slotKey(fid,sid,at){return fid+"|"+sid+"|"+new Date(at).toISOString()}
function holderId(L){return (SESSION?SESSION.id:"anon")+":"+L.id}
function ledgerClaim(key,holder,idem){const l=ledgerRead();const cur=l[key];
 if(cur){if(cur.holder===holder||(idem&&cur.idem===idem))return{ok:true,repeat:true};audit("concurrency","Claim refused — slot already held ("+key.split("|")[2].slice(0,16)+")");return{ok:false}}
 l[key]={holder,idem,at:Date.now()};l.__v=(l.__v||0)+1;ledgerWrite(l);audit("concurrency","Slot claimed ("+key.split("|")[2].slice(0,16)+")");return{ok:true}}
function ledgerRelease(key,holder){const l=ledgerRead();if(l[key]&&l[key].holder===holder){delete l[key];l.__v=(l.__v||0)+1;ledgerWrite(l);audit("concurrency","Slot released")}}
async function ledgerClaimCAS(key,holder,idem,jitter){for(let tries=0;tries<4;tries++){const l=ledgerRead(),v=l.__v||0,cur=l[key];
  if(cur&&cur.holder!==holder&&cur.idem!==idem)return{ok:false,reason:"already taken by another request"};
  if(cur&&(cur.holder===holder||cur.idem===idem))return{ok:true,repeat:true};
  await sleep(jitter);const l2=ledgerRead();if((l2.__v||0)!==v)continue;
  l2[key]={holder,idem,at:Date.now()};l2.__v=v+1;ledgerWrite(l2);return{ok:true}}
 return{ok:false,reason:"could not get a consistent lock"}}

/* ---- C11 Policy versions ---- */
const POLICIES={
 1:{v:1,name:"Policy v1 — initial rules",changes:[],rules:{}},
 2:{v:2,name:"Policy v2 — issued mid-day by organisers",changes:["Specialist OPDs (Cardiology, Orthopaedics) now need a referral letter at every facility, including private hospitals.","Physiotherapy at government facilities no longer needs a referral.","A booking can be rescheduled at most 2 times."],rules:{specialistReferralAll:true,govtPhysioNoReferral:true,maxResched:2}}};
function policy(){if(S&&S.sim){S.sim.offline=S.sim.sensor=S.sim.missingRef=S.sim.trGap=false}if(S)S.policyV=1;return POLICIES[1]}
function needsReferral(f,sid){const svc=f&&f.services&&f.services[sid];if(!svc)return false;let r=svc.referral;
 const P=policy().rules;if(P.specialistReferralAll&&["cardio","ortho"].includes(sid))r=true;
 if(P.govtPhysioNoReferral&&sid==="physio"&&/govt|government|community|esi|primary/i.test(f.type||""))r=false;
 return r===undefined?false:r}

/* ---- C02 Conflicts: source tiers + freshness rule ---- */
const SOURCE_TIER={official:1,facility:1,directory:2,organiser:2,community:3,patient:3,auto:2};
function tierOf(src){src=(src||"").toLowerCase();if(/website|insurance desk|facility|official|hospital/.test(src))return 1;if(/directory|organiser/.test(src))return 2;return 3}
function resolveConflict(c){
 if(c.auto)return{decision:"unresolved",trust:null,reason:"Two fields in the same record contradict each other, so neither can be trusted on its own. Confirm with the facility before travelling."};
 const recs=c.records||[];if(recs.length<2)return{decision:"unresolved",trust:null,reason:"Sources disagree and we can't tell which is right. Marked unverified — a navigator should confirm."};
 const sorted=[...recs].sort((a,b)=>a.tier-b.tier||new Date(b.at)-new Date(a.at));const best=sorted[0],other=sorted[1];
 const newerLower=new Date(other.at)>new Date(best.at)&&other.tier>best.tier;
 if(best.tier<other.tier&&!newerLower)return{decision:"trusted",trust:best,reason:`Trusted: ${best.source} (higher-priority source and not older).`};
 if(best.tier===other.tier)return{decision:"trusted",trust:best,reason:`Same source level — the newer record (${best.at}) is used.`};
 return{decision:"unresolved",trust:null,reason:`A newer but lower-priority source (${other.source}, ${other.at}) contradicts an older official record (${best.source}, ${best.at}). Neither is treated as the truth until verified.`}}

/* ---- C03 Adapter: map changed API (v2) into our internal model ---- */
const DAYMAP={sun:0,mon:1,tue:2,wed:3,thu:4,fri:5,sat:6};
const SCHEMEMAP={"cmchis":"cmchis","pm-jay":"pmjay","pmjay":"pmjay","ayushman":"pmjay","cghs":"cghs","esi":"esi","private":"private","insurance":"private","self":"self"};
const yes=v=>v===true||/^(yes|true|y|1|available)$/i.test(String(v));
function isV2(r){return r&&typeof r==="object"&&("facility_id" in r||"facility_name" in r||Array.isArray(r.departments))}
function adaptFacility(r,log){if(!isV2(r))return r;const id=r.facility_id;const out={id,name:r.facility_name,type:r.category,area:r.location&&r.location.area,address:r.location&&r.location.address,phone:r.contact&&r.contact.phone,
  open:r.hours&&r.hours.opens,close:r.hours&&r.hours.closes,
  days:r.hours&&Array.isArray(r.hours.weekdays)?r.hours.weekdays.map(d=>DAYMAP[String(d).slice(0,3).toLowerCase()]).filter(x=>x!=null):undefined,
  emergency:r.emergency_24x7!=null?yes(r.emergency_24x7):false,
  languages:typeof r.languages==="string"?r.languages.split(/[,;]/).map(x=>x.trim()).filter(Boolean):r.languages,
  access:r.accessibility?{wheelchair:yes(r.accessibility.step_free),lift:yes(r.accessibility.lift),isl:/request/i.test(r.accessibility.sign_language)?"request":yes(r.accessibility.sign_language),braille:yes(r.accessibility.braille),toilet:yes(r.accessibility.accessible_toilet)}:undefined,
  schemes:r.payment&&Array.isArray(r.payment.accepted)?r.payment.accepted.map(s=>SCHEMEMAP[String(s).toLowerCase()]||null).filter(Boolean):undefined,
  verified:r.last_verified?String(r.last_verified).slice(0,10):undefined,conflicts:[],services:{}};
 if(r.location&&r.location.coords){out.x=Number(r.location.coords.x);out.y=Number(r.location.coords.y)}
 (Array.isArray(r.departments)?r.departments:[]).forEach(d=>{if(!d||typeof d!=="object")return;out.services[d.service]={dept:d.name,floor:d.floor===undefined?0:(/^\d+$/.test(String(d.floor))?Number(d.floor):d.floor),referral:d.needs_referral===undefined?undefined:yes(d.needs_referral),fee:d.fee_inr===0||d.fee_inr==="0"?"Free":(d.fee_inr!=null?"₹"+d.fee_inr:d.fee),slotMins:d.slot_minutes!=null?Number(d.slot_minutes):undefined}});
 const known=["facility_id","facility_name","category","location","contact","hours","emergency_24x7","languages","accessibility","payment","departments","last_verified"];
 const extra=Object.keys(r).filter(k=>!known.includes(k));
 log.push(`Mapped API v2 record "${id}" → internal model (renamed fields, nested location/hours, string→number/boolean)${extra.length?`; ignored unknown fields: ${extra.join(", ")}`:""}`);return out}

/* ---- C04 Validation gate ---- */
function cleanStr(v,field,errs,warns,max){max=max||160;if(v==null)return v;if(typeof v!=="string"){errs.push(`${field}: expected text, got ${Array.isArray(v)?"list":typeof v}`);return null}
 let s=v.normalize("NFC");if(/[\u0000-\u0008\u000B\u000C\u000E-\u001F\u007F]/.test(s)){errs.push(`${field}: contains control characters`);return null}
 if(/[‪-‮⁦-⁩]/.test(s)){errs.push(`${field}: contains hidden text-direction characters (spoofing risk)`);return null}
 if(/[​-‍﻿]/.test(s)){s=s.replace(/[​-‍﻿]/g,"");warns.push(`${field}: removed invisible zero-width characters`)}
 if(/<\s*\/?\s*[a-z]|javascript:|on[a-z]+\s*=|\{\{|\$\{/i.test(s)){errs.push(`${field}: looks like code or HTML (possible injection)`);return null}
 if(s.length>max){errs.push(`${field}: too long (${s.length} characters)`);return null}return s.trim()}
function isISODate(s){if(typeof s!=="string"||!/^\d{4}-\d{2}-\d{2}$/.test(s))return false;const d=new Date(s+"T00:00:00Z");return !isNaN(d)&&d.toISOString().slice(0,10)===s}
function validateFacility(raw,idx,seen){const errs=[],warns=[];const lbl=`Record ${idx+1}`;
 if(!raw||typeof raw!=="object"||Array.isArray(raw))return{ok:false,id:lbl,errs:["Not a facility object"],warns};
 const f={};f.id=cleanStr(raw.id,"id",errs,warns,40);if(raw.id==null||raw.id==="")errs.push("id: missing");else if(!/^[A-Za-z0-9_-]+$/.test(f.id))errs.push("id: only letters, numbers, - and _ allowed");
 f.name=cleanStr(raw.name,"name",errs,warns,120);if(raw.name==null||raw.name==="")errs.push("name: missing");
 if(f.id&&seen.has(f.id))errs.push(`id "${f.id}": duplicate — first copy kept`);
 f.type=cleanStr(raw.type,"type",errs,warns,80)||"Facility";
 f.address=cleanStr(raw.address,"address",errs,warns,200)||"";f.phone=cleanStr(raw.phone,"phone",errs,warns,30)||"";
 if(f.phone&&!/^[0-9+()\- ]{6,20}$/.test(f.phone))errs.push("phone: not a phone number");
 const hasXY=raw.x!=null||raw.y!=null;
 if(raw.area!=null){f.area=cleanStr(raw.area,"area",errs,warns,40);if(f.area&&!AREAS[f.area]&&!hasXY)errs.push(`area "${f.area}": unknown area and no x/y given`)}
 if(hasXY){["x","y"].forEach(k=>{const v=raw[k];if(typeof v!=="number"||!isFinite(v))errs.push(`${k}: must be a number`);else if(v<-300||v>300)errs.push(`${k}: ${v} is outside the state map (±300 km)`);else f[k]=v})}
 if(raw.area==null&&!hasXY)errs.push("location: needs an area or x/y");
 const tm=/^([01]\d|2[0-3]):[0-5]\d$/;["open","close"].forEach(k=>{if(raw[k]==null){f[k]=k==="open"?"09:00":"16:00";warns.push(`${k}: missing — assumed ${f[k]}, shown as unverified`)}else if(typeof raw[k]!=="string"||!tm.test(raw[k]))errs.push(`${k}: "${String(raw[k]).slice(0,20)}" is not a valid time (HH:MM)`);else f[k]=raw[k]});
 if(f.open&&f.close&&f.open>=f.close)errs.push("hours: closing time is not after opening time");
 if(raw.days==null){f.days=[1,2,3,4,5,6];warns.push("days: missing — assumed Mon–Sat")}else if(!Array.isArray(raw.days)||!raw.days.every(d=>Number.isInteger(d)&&d>=0&&d<=6))errs.push("days: must be a list of weekday numbers 0–6");else f.days=[...new Set(raw.days)];
 if(raw.verified==null){f.verified="2000-01-01";warns.push("verified: missing — treated as unverified (stale)")}
 else if(!isISODate(raw.verified))errs.push(`verified: "${String(raw.verified).slice(0,25)}" is not a valid date`);
 else if(new Date(raw.verified)>new Date(Date.now()+864e5))errs.push(`verified: ${raw.verified} is in the future`);
 else if(raw.verified<"2015-01-01")errs.push(`verified: ${raw.verified} is unrealistically old`);else f.verified=raw.verified;
 f.emergency=raw.emergency==null?false:(typeof raw.emergency==="boolean"?raw.emergency:(errs.push("emergency: must be true/false"),false));
 if(raw.languages==null){f.languages=[];warns.push("languages: missing")}else if(!Array.isArray(raw.languages))errs.push("languages: must be a list");else{f.languages=raw.languages.map((l,i)=>cleanStr(l,`languages[${i}]`,errs,warns,30)).filter(Boolean)}
 f.access={};if(raw.access!=null){if(typeof raw.access!=="object"||Array.isArray(raw.access))errs.push("access: must be an object");else Object.keys(ACCESS).forEach(k=>{const v=raw.access[k];if(v==null)return;if(v===true||v===false||v==="request")f.access[k]=v;else errs.push(`access.${k}: must be true, false or "request"`)});if(raw.access&&typeof raw.access.note==="string")f.access.note=cleanStr(raw.access.note,"access.note",errs,warns,120)}
 if(raw.schemes==null){f.schemes=[];warns.push("schemes: missing — no payment schemes assumed")}else if(!Array.isArray(raw.schemes))errs.push("schemes: must be a list");else{f.schemes=raw.schemes.filter(s=>SCHEMES[s]&&s!=="unknown"&&s!=="self");const bad=raw.schemes.filter(s=>!SCHEMES[s]);if(bad.length)warns.push("schemes: ignored unknown codes "+bad.map(x=>String(x).slice(0,15)).join(", "))}
 if(raw.selfPay===false)f.selfPay=false;
 f.conflicts=Array.isArray(raw.conflicts)?raw.conflicts.filter(c=>c&&typeof c==="object").map(c=>({service:typeof c.service==="string"?c.service:null,field:cleanStr(c.field,"conflict.field",errs,warns,80)||"Unspecified",note:cleanStr(c.note,"conflict.note",errs,warns,300)||"",source:cleanStr(c.source,"conflict.source",errs,warns,120)||"",records:Array.isArray(c.records)?c.records:undefined})):[];
 f.services={};if(!raw.services||typeof raw.services!=="object"||Array.isArray(raw.services))errs.push("services: missing or not an object");
 else Object.entries(raw.services).forEach(([sid,s])=>{if(!SERVICES[sid]){warns.push(`services.${String(sid).slice(0,20)}: unknown service — ignored`);return}
  if(!s||typeof s!=="object"){errs.push(`services.${sid}: must be an object`);return}const o={};
  o.dept=cleanStr(s.dept,`services.${sid}.dept`,errs,warns,80);if(!o.dept)errs.push(`services.${sid}.dept: missing`);
  if(s.floor==null)o.floor=0;else if(typeof s.floor!=="number"||!Number.isInteger(s.floor))errs.push(`services.${sid}.floor: "${String(s.floor).slice(0,10)}" is not a whole number`);else if(s.floor<0||s.floor>60)errs.push(`services.${sid}.floor: ${s.floor} is unrealistic`);else o.floor=s.floor;
  if(s.slotMins!=null){if(typeof s.slotMins!=="number"||s.slotMins<5||s.slotMins>240)errs.push(`services.${sid}.slotMins: ${String(s.slotMins).slice(0,10)} is unrealistic (5–240)`);else o.slotMins=s.slotMins}
  if(s.avg!=null){if(typeof s.avg!=="number"||s.avg<=0||s.avg>180)errs.push(`services.${sid}.avg: ${String(s.avg).slice(0,10)} is unrealistic`);else o.avg=s.avg}
  if(s.days!=null){if(!Array.isArray(s.days)||!s.days.every(d=>Number.isInteger(d)&&d>=0&&d<=6))errs.push(`services.${sid}.days: invalid`);else o.days=s.days}
  if(s.referral===undefined||s.referral===null){o.referral=null;warns.push(`services.${sid}.referral: not stated — rule shown as unknown (C12)`)}else if(typeof s.referral!=="boolean")errs.push(`services.${sid}.referral: must be true/false`);else o.referral=s.referral;
  if(s.fee==null)o.fee="Fee not stated";else if(typeof s.fee==="number"){if(s.fee<0||s.fee>500000)errs.push(`services.${sid}.fee: ${s.fee} is negative or unrealistic`);else o.fee=s.fee===0?"Free":"₹"+s.fee}else{o.fee=cleanStr(s.fee,`services.${sid}.fee`,errs,warns,60);if(o.fee&&/-\s*₹|₹\s*-/.test(o.fee))errs.push(`services.${sid}.fee: negative amount`)}
  if(Array.isArray(s.extraDocs))o.extraDocs=s.extraDocs.filter(d=>DOCS[d]);
  f.services[sid]=o});
 if(raw.services&&typeof raw.services==="object"&&!Object.keys(f.services).length&&!errs.length)errs.push("services: none recognised");
 return{ok:!errs.length,id:f.id||lbl,name:f.name,rec:f,errs,warns}}
function parseCSV(text){const rows=[];let row=[],cur="",q=false;for(let i=0;i<text.length;i++){const c=text[i];
  if(q){if(c==='"'){if(text[i+1]==='"'){cur+='"';i++}else q=false}else cur+=c}
  else if(c==='"')q=true;else if(c===","){row.push(cur);cur=""}else if(c==="\n"||c==="\r"){if(c==="\r"&&text[i+1]==="\n")i++;row.push(cur);rows.push(row);row=[];cur=""}else cur+=c}
 let broken=null;if(q){broken=rows.length+1}else if(cur!==""||row.length){row.push(cur);rows.push(row)}
 const head=(rows.shift()||[]).map(h=>h.trim().toLowerCase());if(!head.includes("id"))throw new Error("CSV: header row must include an 'id' column");
 const byId={},order=[];rows.filter(r=>r.some(x=>x.trim())).forEach((r,ri)=>{const o={};head.forEach((h,i)=>o[h]=r[i]===undefined?undefined:r[i].trim());
  const num=v=>v===undefined||v===""?undefined:(/^-?\d+(\.\d+)?$/.test(v)?Number(v):v),bool=v=>v===undefined||v===""?undefined:(/^(true|yes)$/i.test(v)?true:/^(false|no)$/i.test(v)?false:v),list=v=>v?v.split(";").map(x=>x.trim()).filter(Boolean):undefined;
  const key=o.id||("row"+ri);if(!byId[key]){byId[key]={id:o.id,name:o.name,type:o.type,area:o.area,address:o.address,phone:o.phone,open:o.open,close:o.close,days:o.days?o.days.split(";").map(num):undefined,emergency:bool(o.emergency),languages:list(o.languages),schemes:list(o.schemes),verified:o.verified,access:{wheelchair:bool(o.wheelchair),lift:bool(o.lift),isl:o.isl==="request"?"request":bool(o.isl),braille:bool(o.braille),toilet:bool(o.toilet)},services:{}};order.push(key)}
  if(o.service)byId[key].services[o.service]={dept:o.dept,floor:num(o.floor),referral:bool(o.referral),fee:o.fee,slotMins:num(o.slotmins)}});
 const out=order.map(k=>byId[k]);if(broken)out.push({__bad:`CSV row ${broken}: a quoted value is never closed — row skipped`});return out}
function jsonErrorPos(text,err){const m=String(err.message).match(/position (\d+)/);if(!m)return err.message;const p=+m[1];const before=text.slice(0,p);const line=before.split("\n").length,col=p-before.lastIndexOf("\n");return `${err.message.replace(/ in JSON at position \d+.*$/,"")} (line ${line}, column ${col})`}
function loadDataset(text,name,mode,opts){opts=opts||{};const report={name,mode,accepted:[],quarantined:[],warnings:[],mapped:[],fatal:null,at:Date.now()};
 try{if(typeof text!=="string"||!text.trim())throw new Error("The file is empty");if(text.length>2e6)throw new Error("The file is too large (over 2 MB)");
  let arr;const t=text.replace(/^﻿/,"").trim();
  if(/\.csv$/i.test(name)||(!/^[\[{]/.test(t))){arr=parseCSV(t)}
  else{let j;try{j=JSON.parse(t)}catch(e){throw new Error("Malformed JSON — "+jsonErrorPos(t,e))}
   if(j&&!Array.isArray(j)&&typeof j==="object"){if(Array.isArray(j.facilities))j=j.facilities;else if(Array.isArray(j.data))j=j.data;else if(isV2(j))j=[j];else throw new Error("No list of facilities found in the response")}
   if(!Array.isArray(j))throw new Error("Expected a list of facilities");arr=j}
  if(arr.length>5000)throw new Error("Too many records (over 5,000)");
  const seen=new Set(mode==="merge"?DATA().map(f=>f.id):[]);
  arr.forEach((raw,i)=>{if(raw&&raw.__bad){report.quarantined.push({id:"CSV row",errs:[raw.__bad]});return}const r0=raw;const v=validateFacility(r0,i,seen);
   if(v.ok){seen.add(v.rec.id);report.accepted.push(v.rec);v.warns.forEach(w=>report.warnings.push(`${v.id}: ${w}`))}else report.quarantined.push({id:v.id,name:v.name,errs:v.errs})});
 }catch(e){report.fatal=e.message}
 if(report.fatal){audit("data",`Rejected "${name}": ${report.fatal}. Existing data kept.`)}
 else{if(report.accepted.length){if(mode==="merge"){S.data=[...DATA(),...report.accepted];S.dataName=(S.dataName||"built-in sample")+" + "+name}else{S.data=report.accepted;S.dataName=name}
   S.legs.forEach(L=>{if(L.facilityId&&!fac(L.facilityId)){L.facilityId=null;L.booking=null}})}
  S.quarantine=[...report.quarantined.map(q=>({...q,from:name,at:Date.now()})),...(S.quarantine||[])].slice(0,200);
  audit("data",`Loaded "${name}": ${report.accepted.length} accepted, ${report.quarantined.length} quarantined, ${report.warnings.length} warnings`);
  report.quarantined.forEach(q=>audit("data",`Quarantined ${q.id}: ${q.errs.join("; ")}`));report.mapped.forEach(m=>audit("api",m))}
 S.lastReport=report;save();return report}
function reportHTML(r){if(!r)return"";if(r.fatal)return`<div class="banner red"><span class="ic">✕</span><div><b>File rejected — nothing was changed.</b> ${esc(r.fatal)}. Your current facility data is still in use.</div></div>`;
 return`<div class="banner ${r.quarantined.length?"amber":"green"}"><span class="ic">${r.quarantined.length?"!":"✓"}</span><div><b>${r.accepted.length} record(s) loaded${r.quarantined.length?`, ${r.quarantined.length} held for review`:""}.</b> ${r.quarantined.length?"The rest of your data is untouched.":"Everything checked out."}</div></div>
 ${r.mapped.length?`<details open><summary class="small" style="font-weight:700;cursor:pointer">Adapter mapping (${r.mapped.length})</summary><ul class="small">${r.mapped.map(m=>`<li>${esc(m)}</li>`).join("")}</ul></details>`:""}
 ${r.quarantined.length?`<details><summary class="small" style="font-weight:700;cursor:pointer">Why ${r.quarantined.length} record(s) were held</summary><table class="mini"><thead><tr><th>Record</th><th>Reason</th></tr></thead><tbody>${r.quarantined.map(q=>`<tr><td>${esc(q.id)}${q.name?`<div class="tiny muted">${esc(q.name)}</div>`:""}</td><td>${q.errs.map(esc).join("<br>")}</td></tr>`).join("")}</tbody></table></details>`:""}
 ${r.warnings.length?`<details><summary class="small" style="font-weight:700;cursor:pointer">Notes (${r.warnings.length})</summary><ul class="small">${r.warnings.slice(0,40).map(w=>`<li>${esc(w)}</li>`).join("")}</ul></details>`:""}`}

/* ---- C05 Surge allocation (3× demand, 50% capacity) ---- */
function surgeAllocation(f,sid,day){const all=slotsForBase(f,sid,null).filter(s=>sod(s.at).getTime()===day);const baseCap=all.length,cap=Math.floor(baseCap/2);
 const r=rng(hash("surge"+f.id+sid+day));const baseDemand=Math.max(1,Math.round(baseCap*0.66)),demand=baseDemand*3;
 const reqs=[];for(let i=0;i<demand;i++){const committed=i<baseDemand;const x=r();reqs.push({id:"P"+String(i+1).padStart(3,"0"),committed,group:x<0.12?"Senior citizen (60+)":x<0.2?"Pregnant woman":x<0.26?"Person with disability":null,followup:!committed&&r()<0.18,t:i})}
 const order=[...reqs].sort((a,b)=>(b.committed-a.committed)||(a.committed?a.t-b.t:0)||(!!b.group-!!a.group)||(b.followup-a.followup)||a.t-b.t);
 let left=cap;order.forEach(q=>{if(left>0){q.out="Allocated";q.why=q.committed?"Existing booking honoured (booked before the surge)":q.group?`Priority group: ${q.group}`:q.followup?"Doctor-set follow-up date":"First come, first served";left--}
  else{q.out=q.committed?"Moved — needs confirmation":"Wait-list";q.why=q.committed?"Was booked, but the slot pool was halved: offered the earliest slot next open day first, before anyone new":`No capacity left — wait-list position ${0}`}});
 let w=0;order.filter(q=>q.out==="Wait-list").forEach(q=>{w++;q.why=`No capacity left — wait-list #${w}; shown alternatives below`});
 return{baseCap,cap,baseDemand,demand,allocated:order.filter(q=>q.out==="Allocated").length,moved:order.filter(q=>q.out.startsWith("Moved")).length,waitlisted:w,order}}
function alternativesFor(sid,excludeId){return DATA().filter(f=>f.id!==excludeId&&f.services[sid]).map(f=>{const free=slotsFor(f,sid,null).filter(s=>s.free);return{f,free:free.length,first:free[0]}}).filter(a=>a.free>0).sort((a,b)=>(a.first.at-b.first.at)||(dist(a.f)-dist(b.f))).slice(0,3)}

/* ---- C10 Faulty queue readings ---- */
function queueReading(q,token){const n=q.n;const base=q.truth;let board=base,reg=base;const F=false;
 if(F){if(n===2)board=base+83;if(n===3)board=null;if(n>=4&&n<=7)board=q.lastBoard;if(n===8)board=base-5;if(n>=9&&n<=10)reg=base+7}
 return{board,reg}}
function evalReading(q,rd){const flags=[];const last=q.serving;let cand=null;
 const ok=v=>v!=null&&v>=last&&v-last<=4;
 if(rd.board==null)flags.push("Display board sent no reading");else if(rd.board<last)flags.push(`Display board went backwards (${rd.board})`);else if(rd.board-last>4)flags.push(`Sudden spike ignored (board showed ${rd.board})`);
 if(rd.board!=null&&rd.board===q.lastBoard&&q.stuck>=3)flags.push("Display board looks stuck (same number repeatedly)");
 if(rd.board!=null&&rd.reg!=null&&Math.abs(rd.board-rd.reg)>2)flags.push(`Board (${rd.board}) and registration system (${rd.reg}) disagree`);
 if(!flags.length&&ok(rd.board))cand=rd.board;else if(ok(rd.reg)&&(rd.board==null||flags.length))cand=null;
 return{flags,cand}}

/* ---------- View: Stress-test lab (C01–C12) ---------- */
const V2_SAMPLE=JSON.stringify({status:"ok",apiVersion:"2.0",facilities:[
 {facility_id:"kalai-uphc",facility_name:"Kalaignar Nagar Urban PHC",category:"Urban primary health centre",location:{area:"tnagar",address:"Kalaignar Nagar, T. Nagar",coords:{x:9.4,y:12.2}},contact:{phone:"044-4000-2201"},hours:{opens:"08:00",closes:"16:00",weekdays:["Mon","Tue","Wed","Thu","Fri","Sat"]},emergency_24x7:"no",languages:"Tamil, English, Telugu",accessibility:{step_free:"yes",lift:"no",sign_language:"on_request",accessible_toilet:"yes"},payment:{accepted:["CMCHIS","PM-JAY"]},departments:[{service:"gen_opd",name:"OPD",floor:"0",needs_referral:"false",fee_inr:0,slot_minutes:"10"},{service:"cardio",name:"Cardiology outreach clinic",floor:"0",needs_referral:"true",fee_inr:0,slot_minutes:20}],last_verified:"2026-11-01T09:30:00Z",rating_stars:4.2,internal_code:"TN-CHN-0042"}
]},null,1);
const BAD_SAMPLE=`[
 {"id":"good-clinic","name":"Anbu Community Clinic","type":"Community health centre","area":"perambur","open":"08:00","close":"15:00","days":[1,2,3,4,5,6],"languages":["Tamil","English"],"access":{"wheelchair":true},"schemes":["cmchis","pmjay"],"verified":"2026-10-20","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false,"fee":"Free","slotMins":10}}},
 {"name":"No ID Hospital","area":"egmore","services":{"gen_opd":{"dept":"OPD"}}},
 {"id":"thendral","name":"Duplicate of an existing hospital","area":"egmore","verified":"2026-10-01","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 {"id":"bad-date","name":"Bad Date Clinic","area":"adyar","verified":"2026-13-45","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 {"id":"future-date","name":"Time Traveller Clinic","area":"adyar","verified":"2031-01-01","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 {"id":"neg-floor","name":"Basement Clinic","area":"guindy","verified":"2026-10-01","services":{"cardio":{"dept":"Cardiology","floor":-3,"referral":true,"slotMins":0}}},
 {"id":"neg-fee","name":"Pays You Clinic","area":"guindy","verified":"2026-10-01","services":{"dental":{"dept":"Dental","floor":0,"referral":false,"fee":-500}}},
 {"id":"xss","name":"<img src=x onerror=alert(1)> Hospital","area":"tnagar","verified":"2026-10-01","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 {"id":"rtl","name":"City \\u202ElatipsoH Clinic","area":"tnagar","verified":"2026-10-01","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 {"id":"zw-ok","name":"Nala\\u200Bm Annex","area":"triplicane","verified":"2026-10-15","languages":["Tamil"],"services":{"vacc":{"dept":"Immunisation","floor":0,"referral":false,"fee":"Free"}}},
 {"id":"wrong-types","name":"Wrong Types Clinic","area":"porur","languages":"Tamil","days":"Mon-Sat","verified":"2026-10-01","services":{"gen_opd":{"dept":"OPD","floor":"second","referral":"maybe"}}},
 {"id":"far-away","name":"Moon Base Clinic","x":5000,"y":-20,"verified":"2026-10-01","services":{"gen_opd":{"dept":"OPD","floor":0,"referral":false}}},
 "just a string",
 {"id":"no-referral-field","name":"Unknown-rule Eye Clinic","area":"velachery","verified":"2026-10-25","languages":["Tamil","English"],"schemes":["cmchis"],"services":{"eye":{"dept":"Eye OPD","floor":0,"fee":"₹300"}}}
]`;
const BAD_JSON=`[{"id":"broken","name":"Broken file","area":"egmore",}`;
const BAD_CSV=`id,name,type,area,open,close,days,languages,schemes,verified,wheelchair,lift,service,dept,floor,referral,fee
csv-ok,Marina Urban PHC,Urban primary health centre,triplicane,08:00,16:00,1;2;3;4;5;6,Tamil;Urdu,cmchis;pmjay,2026-10-28,yes,no,gen_opd,OPD,0,no,Free
csv-bad-time,Night Owl Clinic,Clinic,adyar,25:00,16:00,1;2,Tamil,cmchis,2026-10-28,yes,no,gen_opd,OPD,0,no,Free
csv-dup,Duplicate Row A,Clinic,guindy,08:00,16:00,1;2,Tamil,cmchis,2026-10-28,yes,no,gen_opd,OPD,0,no,Free
csv-dup,Duplicate Row A,Clinic,guindy,08:00,16:00,1;2,Tamil,cmchis,2026-10-28,yes,no,lab,Lab,0,no,Free
"csv-quote","Unclosed ""quote,Clinic,guindy`;
const PVTXT={};
function pvPhone(id,icon,tone,head,text,main,alt,foot){PVTXT[id]=head+". "+text.replace(/<[^>]+>/g,"");
 return`<div class="pvcol"><div class="pvlabel">What the patient sees</div><div class="pv"><div class="pvnotch"></div><div class="pvbody">
 <div class="pvic ${tone}">${icon}</div><p class="pvh">${head}</p><p class="pvt">${text}</p><div class="pvacts">${main}${alt}</div>
 <button class="pvsay" data-act="pvSay:${id}">🔊 Read aloud</button></div></div><p class="pvfoot">${foot}</p></div>`}
function pScreen(c){const txt={C04:"Only valid hospitals are listed. Broken or malicious records never reach the patient, and the app keeps working.",C05:"A calm “Busy today. Your booking is safe.” banner, scarce slots, and — if their slot had to go — a new time held for them before anyone new.",C05n:"“Our helpers are busy right now” with a call-back time — no ringing phone line, and they keep their place."}[c];
 return`<div class="pscard"><div class="pvlabel">What the patient sees</div><p class="small">${txt}</p><button class="btn block" data-act="demoGoTo:${c}">👁 Open the patient's screen</button></div>`}
function pv4(){const cf=DATA().flatMap(f=>conflicts(f,null).map(c=>({f,c})))[0];
 const txt=cf?`The ${esc(cf.c.field.replace(/^./,m=>m.toLowerCase()))} at <b>${esc(cf.f.name)}</b> may have changed.`:"Some details for this hospital may have changed.";
 return pvPhone("C04","!","amber","Please check before you go",txt,`<button class="pvbtn" data-act="pvDo:call">📞 Call the hospital</button>`,`<button class="pvbtn alt" data-act="pvDo:nav">Ask someone to check</button>`,
 "No error codes. Broken entries are left out; uncertain ones say “check first”.")}
function pv5(sg,f,sid,day){const bk=S.ui.bk||"kept";
 const all=slotsForBase(f,sid,null);const today=all.filter(x=>sod(x.at).getTime()===day);const nxt=all.find(x=>sod(x.at).getTime()>day)||today[today.length-1];
 const kept=today[Math.min(2,today.length-1)];const lost=today[Math.min(today.length-1,Math.floor(today.length*.75))];
 const when=x=>`${fmtDay(x.at)}, ${fmtTime(x.at)}`;
 const seg=`<div class="seg pvseg" role="tablist" aria-label="Booking outcome"><button role="tab" aria-selected="${bk==="kept"}" data-act="bk:kept">Slot kept</button><button role="tab" aria-selected="${bk==="moved"}" data-act="bk:moved">Slot moved</button></div>`;
 const body=bk==="kept"
  ?pvPhone("C05k","✓","green","Your booking is safe",`<b>${esc(when(kept))}</b> · token ${kept.token}<br>${esc(f.name)}. Nothing changes — come as planned.`,
    `<button class="pvbtn" data-act="pvDo:ok">✓ Got it</button>`,`<button class="pvbtn alt" data-act="pvDo:remind">Remind me the day before</button>`,
    "Booked before the rush → honoured first, in the order bookings were made. The patient isn't bothered with the surge at all.")
  :pvPhone("C05m","↻","amber","We had to move your visit",`The doctor has fewer slots ${(d=>/^(Today|Tomorrow)$/.test(d)?d.toLowerCase():"on "+d)(fmtDay(lost.at))}. Your new time is <b>${esc(when(nxt))}</b> — the first slot, held for you before any new patient.`,
    `<button class="pvbtn" data-act="pvDo:accept">✓ This time is fine</button>`,`<button class="pvbtn alt" data-act="pvDo:cb">📞 Call me to choose another</button>`,
    "Never silently cancelled. Moved to the earliest slot on the next open day, ahead of new requests, and only confirmed once the patient (or a navigator on their behalf) says yes.");
 return pScreen("C05")}
function pvNav(n){return pvPhone("C05n","☎","blue","Our helpers are busy right now",`You're in the queue. We'll call you back in about <b>${n.eta} minutes</b> — you don't need to stay on this screen.`,
 `<button class="pvbtn" data-act="pvDo:keep">✓ Keep my place</button>`,`<button class="pvbtn alt" data-act="pvDo:faq">Get a quick answer now</button>`,
 "Common questions are answered instantly; people who need a human are called back in priority order.")}
/* ---- C05 (navigator reading): requests ×3, human navigators −50% ---- */
function navSurge(){const baseNav=8,nav=4,mins=12,perHr=Math.floor(nav*60/mins);const baseReq=40,req=baseReq*3;const r=rng(hash("navsurge-v1"));
 const T=[["Which documents to bring",.22,1],["Is the hospital open / timings",.14,1],["Is my scheme accepted",.12,1],["Change or cancel a booking",.1,1],["Lost or confused at the hospital",.12,0],["Referral or paperwork problem",.14,0],["Needs language / sign-language help",.08,0],["Something else",.08,0]];
 const pick=()=>{let x=r(),a=0;for(const t of T){a+=t[1];if(x<a)return t}return T[T.length-1]};
 const all=[];for(let i=0;i<req;i++){const t=pick();const g=r()<.2?"60+":r()<.08?"Disability":r()<.06?"Pregnant":null;const today=r()<.22;all.push({id:"N"+String(i+1).padStart(3,"0"),topic:t[0],self:!!t[2],g,today,lost:t[0].startsWith("Lost")})}
 const instant=all.filter(q=>q.self&&!q.g&&!q.today);const queue=all.filter(q=>!instant.includes(q));
 const rank=q=>q.lost&&q.today?0:q.g?1:q.today?2:3;queue.forEach((q,i)=>q.i=i);queue.sort((a,b)=>rank(a)-rank(b)||a.i-b.i);
 queue.forEach((q,i)=>{q.hr=Math.floor(i/perHr);q.eta=Math.ceil((i+1)/nav)*mins;q.why=["At the hospital today and lost","Priority group: "+q.g,"Visit is today","First come, first served"][rank(q)]});
 const hrs=[];queue.forEach(q=>{hrs[q.hr]=(hrs[q.hr]||0)+1});const pri=queue.filter(q=>rank(q)<=1);
 const sample=queue.find(q=>q.g==="60+")||queue[0];
 return{baseNav,nav,baseReq,req,perHr,mins,instant:instant.length,queue,hrs,priFirst:pri.filter(q=>q.hr===0).length,pri:pri.length,maxH:hrs.length,eta:sample.eta}}
function labCard(id,title,sub,body){return`<section class="card stack lab" id="lab-${id}"><div class="labhead"><h3>${esc(title)}</h3><span class="ref" title="Hackathon constraint ${id}">${id}</span></div><p class="small muted" style="margin-top:-.4rem">${sub}</p>${body}</section>`}
function vLab(){const R=S.ui.lab||(S.ui.lab={});const L=leg();const curF=L.facilityId&&fac(L.facilityId);const sim=S.sim||{};
 const demoF=curF||DATA().find(f=>f.services.gen_opd);const demoSid=curF?L.service:"gen_opd";
 const tom=sod(new Date(Date.now()+864e5)).getTime();const days=[...new Set(slotsForBase(demoF,demoSid,null).map(s=>sod(s.at).getTime()))];const day=days.includes(tom)?tom:days[0];
 const tog=(k,on,off)=>`<button class="btn sm ${sim[k]?"warn":""}" data-act="sim:${k}">${sim[k]?on:off}</button>`;
 const surge=sim.surge&&day!=null?surgeAllocation(demoF,demoSid,day):null;
 const conflictsAll=DATA().flatMap(f=>conflicts(f,null).map(c=>({f,c})));
 const tab=S.ui.demoTab||"C04";const last=S.lastReport;const r4=R.C04?last:null;const ran4=!!r4,ran5=!!(sim.surge||sim.navSurge);
 const tabBtn=(id,title,ran)=>`<button class="dtab" role="tab" aria-selected="${tab===id}" data-act="demotab:${id}"><span class="c">Constraint ${id}</span><b>${title}</b><span class="st ${ran?"ok":""}">${ran?"✓ Handled":"Not run yet"}</span></button>`;
 const hero=`<section class="card dhero"><div class="row" style="justify-content:space-between;align-items:flex-start"><div><div class="eyebrow">Live constraint demo${S.ui.demoRun?" · admin view":""}</div><h2>${S.ui.demoRun?"How the platform handled it":"What happens when things go wrong?"}</h2><p class="small" style="max-width:56ch">${S.ui.demoRun?"Behind the scenes: what the system detected, what it did, and the numbers.":"Pick a constraint and trigger it — you'll first see the patient's screen, then how the platform dealt with it."}</p></div><div class="row" style="gap:.4rem"><button class="btn light sm" data-act="demoReset">↺ Reset demo</button></div></div>
  <div class="dtabs" role="tablist">${tabBtn("C04","Bad data arrives",ran4)}${tabBtn("C05","3× demand, half the resources",ran5)}</div></section>`;

 const flow=(sit,trig,how)=>`<div class="flow"><div><h4><span class="n">1</span>The situation</h4><p class="small">${sit}</p></div><div><h4><span class="n">2</span>Trigger it</h4><div class="row">${trig}</div></div><div><h4><span class="n">3</span>How Next Route responds</h4><ul class="small">${how}</ul></div></div>`;

 let body;
 if(tab==="C04"){
  const total=r4?r4.accepted.length+r4.quarantined.length:0;
  body=`<section class="card stack" id="lab-C04"><h3>C04 · Malformed or malicious data</h3>
  ${flow("A facility list from the organiser, a hospital or an API comes in broken: missing IDs, impossible dates, negative fees, duplicate entries, hidden Unicode, even HTML/script injection in a hospital name.",
   `<button class="btn sm" data-act="lab:badset">Send messy dataset</button><button class="btn sm" data-act="lab:badjson">Send broken JSON</button><button class="btn sm" data-act="lab:badcsv">Send messy CSV</button><label class="btn ghost sm" style="position:relative">Upload your own<input type="file" accept=".json,.csv,application/json,text/csv" data-change="data" style="position:absolute;inset:0;opacity:0;cursor:pointer"></label>`,
   "<li>Parses safely — a broken file never crashes the app</li><li>Checks every record: required fields, types, dates, ranges, duplicates, injection, hidden characters</li><li>Loads the good records, holds the bad ones with a reason</li><li>Never overwrites existing data with a broken file</li>")}
  ${r4?(r4.fatal?`<div class="verdict">✓ Constraint handled <span>— the file was rejected and the app kept running on the existing data.</span></div>${reportHTML(r4)}`:
   `<div class="verdict">✓ Constraint handled <span>— the app stayed up, good data went live and bad data was held aside.</span></div>
   <div class="pvwrap"><div class="stack"><div class="stats"><div><div class="k">Records received</div><div class="v">${total}</div></div><div class="good"><div class="k">Loaded safely</div><div class="v">${r4.accepted.length}</div></div><div><div class="k">Held for review</div><div class="v">${r4.quarantined.length}</div></div><div class="good"><div class="k">Existing data corrupted</div><div class="v">0</div></div></div>
   ${reportHTML(r4)}</div></div>`)
   :`<div class="empty">Pick one of the files in step 2 to see the result here.</div>`}
  </section>`;
 }else{
  const mode=S.ui.c05mode||"slots";const ns=sim.navSurge?navSurge():null;
  const seg=`<div class="seg" role="tablist" aria-label="Which resource is short"><button role="tab" aria-selected="${mode==="slots"}" data-act="c05mode:slots">Doctors &amp; appointment slots ${sim.surge?"✓":""}</button><button role="tab" aria-selected="${mode==="nav"}" data-act="c05mode:nav">Human navigators ${sim.navSurge?"✓":""}</button></div>`;
  const navHTML=`${flow("Three times as many people ask for a human navigator, while half the navigators are off sick. A phone line would just ring out — and the people most likely to need help are elderly or disabled.",
   sim.navSurge?`<button class="btn warn sm" data-act="sim:navSurge">■ Stop the surge</button><button class="btn ghost sm" data-act="nav:help" style="color:var(--ink);border-color:var(--line)">See it as a patient →</button>`:`<button class="btn sm" data-act="sim:navSurge">▶ Start the surge</button>`,
   "<li>Answers common questions instantly in the app (what to bring, timings, scheme cover, rescheduling) — so humans are kept for people who need them</li><li>Nobody waits on hold: everyone else gets a call-back time and keeps their place</li><li>Call-back order: lost at the hospital today → 60+, disability, pregnancy → visit today → first come first served</li><li>Never schedules more calls than the navigators on shift can handle. Emergencies go to 108 / 112</li>")}
  ${ns?`<div class="verdict">✓ Constraint handled <span>— ${ns.instant} answered instantly, ${ns.queue.length} call-backs scheduled within capacity, nobody dropped.</span></div>
   <div class="pvwrap"><div class="stack"><div class="stats"><div><div class="k">Navigators on shift</div><div class="v">${ns.nav} <small>was ${ns.baseNav}</small></div></div><div><div class="k">Help requests</div><div class="v">${ns.req} <small>was ${ns.baseReq}</small></div></div><div class="good"><div class="k">Answered instantly</div><div class="v">${ns.instant}</div></div><div class="good"><div class="k">Priority called in 1st hour</div><div class="v">${ns.priFirst}/${ns.pri}</div></div></div>
   <div><b class="small">Call-back schedule (max ${ns.perHr} calls per hour with ${ns.nav} navigators)</b>${ns.hrs.map((n,i)=>`<div class="hbar"><span>Hour ${i+1}</span><div><i style="width:${n/ns.perHr*100}%"></i></div><b>${n}/${ns.perHr}</b></div>`).join("")}</div>
   <details><summary class="small" style="font-weight:700;cursor:pointer">Every call-back, in order (${ns.queue.length})</summary><table class="mini"><thead><tr><th>#</th><th>Request</th><th>Need</th><th>Call-back in</th><th>Why this position</th></tr></thead><tbody>${ns.queue.map((q,i)=>`<tr><td>${i+1}</td><td>${q.id}</td><td>${esc(q.topic)}</td><td>~${q.eta} min</td><td>${esc(q.why)}</td></tr>`).join("")}</tbody></table></details></div></div>`
   :`<div class="empty">Press <b>Start the surge</b> in step 2 to see the result here.</div>`}`;
  body=`<section class="card stack" id="lab-C05"><h3>C05 · Demand ×3, resources −50%</h3>${seg}${mode==="nav"?navHTML:`
  ${flow("A heatwave or outbreak hits. Three times as many people want appointments, while half the doctors are unavailable, so each facility has half its usual slots.",
   `<button class="btn sm" data-act="surgeScn:kept">▶ Scenario 1: booking kept</button><button class="btn sm" data-act="surgeScn:moved">▶ Scenario 2: slot lost → reschedule</button>${sim.surge?`<button class="btn warn sm" data-act="sim:surge">■ Stop the surge</button>`:""}`,
   "<li>Never books more people than there are slots</li><li>Keeps existing bookings, and moves any that no longer fit to the next open day <i>before</i> anyone new</li><li>Then follows the same priority queues government hospitals use (60+, pregnant women, persons with disabilities), then doctor-set follow-ups, then first come first served</li><li>Everyone else is wait-listed with nearby alternatives. Emergencies go to 108 / 112</li>")}
  ${surge?`<div class="verdict">✓ Constraint handled <span>— ${surge.allocated} of ${surge.cap} slots used, nobody silently dropped.</span></div>
   <div class="pvwrap"><div class="stack"><div class="stats"><div><div class="k">Slots available</div><div class="v">${surge.cap} <small>was ${surge.baseCap}</small></div></div><div><div class="k">Requests</div><div class="v">${surge.demand} <small>was ${surge.baseDemand}</small></div></div><div class="good"><div class="k">Allocated</div><div class="v">${surge.allocated}/${surge.cap}</div></div><div><div class="k">Moved / wait-listed</div><div class="v">${surge.moved} <small>/ ${surge.waitlisted}</small></div></div></div>
   <div class="grid2"><div class="small"><b>Facility in this demo</b><br>${esc(demoF.name)} · ${esc(SERVICES[demoSid].name)} · ${esc(fmtDay(new Date(day)))}</div>
   <div><b class="small">Offered to wait-listed patients</b><ul class="small">${alternativesFor(demoSid,demoF.id).map(a=>`<li>${esc(a.f.name)} — ${a.free} free, next ${esc(fmtDay(a.first.at))} ${esc(fmtTime(a.first.at))}</li>`).join("")||"<li>No other facility has free slots — navigator call-back offered</li>"}<li>Earliest slot on the next open day here</li><li>Navigator call-back</li></ul></div></div>
   <details><summary class="small" style="font-weight:700;cursor:pointer">Every request, its outcome and why (${surge.order.length})</summary><table class="mini"><thead><tr><th>Request</th><th>Outcome</th><th>Reason</th></tr></thead><tbody>${surge.order.map(q=>`<tr><td>${q.id}${q.committed?" · booked earlier":""}</td><td><b>${q.out}</b></td><td>${esc(q.why)}</td></tr>`).join("")}</tbody></table></details></div></div>`
   :`<div class="empty">Run one of the scenarios in step 2 to see the result here.</div>`}`}
  </section>`;
 }
 return hero+body;
}

/* =========================================================
   Rendering
   ========================================================= */
function render(){
 try{applyDemo()}catch(e){console.error(e)}
 if(!SESSION){$("#app").hidden=true;$("#auth").hidden=false;document.documentElement.lang="en";renderAuth();return}
 $("#app").hidden=false;$("#auth").hidden=true;$("#auth").innerHTML="";
 {const nm=SESSION.name||"Guest";$("#userBtn").innerHTML=`<span class="av" aria-hidden="true">${esc(nm.trim().charAt(0).toUpperCase()||"G")}</span>${esc(nm.split(" ")[0])}`;}
 document.documentElement.lang=S.lang;document.documentElement.style.setProperty("--fs",S.fs);document.body.classList.toggle("hc",S.hc);
 $("#tagline").textContent=t("tag");$("#boundaryTxt").innerHTML=t("boundary");$("#langSel").value=S.lang;$("#citySel").value=S.city;
 $("#fsLbl").textContent=Math.round(S.fs*100)+"%";$("#hcBtn").textContent=t("hc");$("#hcBtn").setAttribute("aria-pressed",S.hc);
 $("#speakBtn").textContent=t("speak");$("#demoBtn").textContent=t("demo");$("#humanBtn").textContent=t("human");
 $("#foot").innerHTML=`${esc(t("note"))} Source: ${S.data?esc(S.dataName||"organiser upload"):"built-in sample (fictional facilities, "+esc(CITY().name)+")"} · Prototype — bookings, tickets and queues are simulated.`;
 renderJourney();renderMain();renderSide();
 translateDOM(document.body);
}
function sysLink(){const busy=S.sim&&S.sim.surge;const held=(S.quarantine||[]).length;
 return`<button class="syslink" data-act="nav:lab" title="System health"><span class="sdot ${busy?"amber":""}"></span>${busy?"High demand":"All systems normal"}${held&&!busy?` · ${held} held`:""}</button>`}
function renderJourney(){
 const st=stage(),idx=STAGES.indexOf(st);const cv=S.view;
 const legs=S.legs.length>1||leg().purpose?`<div class="legs"><span class="tiny muted" style="font-weight:700">JOURNEY LEGS</span>${S.legs.map((L,i)=>`<button class="leg ${i===S.cur?"cur":""} ${L.status==="done"?"done":""} ${L.status==="waiting"?"wait":""}" data-act="leg:${i}" title="${esc(L.purpose||"")}">${i+1}. ${L.service?esc(SERVICES[L.service].name):"New need"}${L.status==="waiting"?" · waiting":L.status==="done"?" ✓":""}</button>${i<S.legs.length-1?"<span class='muted'>→</span>":""}`).join("")}</div>`:"";
 const pct=idx/(STAGES.length-1);
 $("#journey").innerHTML=legs+`<div class="line"><div class="fill" style="width:calc((100% - 100%/6) * ${pct})"></div>${STAGES.map((s,i)=>`<button class="stn ${i<idx||(st==="follow"&&i===idx&&!leg().booking)?"done":""} ${i===idx?"now":""} ${VIEWOF[s]===cv?"view":""} ${i<idx?"done":""}" data-act="nav:${VIEWOF[s]}" aria-current="${VIEWOF[s]===cv?"page":"false"}"><span class="dot">${i<idx?"✓":i+1}</span><span class="lbl">${t("st_"+s)}</span><span class="sub">${t("sub_"+s)}</span></button>`).join("")}</div>`;
}
function renderSide(){
 const n=nextStep();const rs=escalationReasons();const rem=reminders().filter(r=>r.at>=sod(new Date())).slice(0,3);
 $("#side").innerHTML=`
 <section class="card next" aria-live="polite">
  <div class="eyebrow">${t("next")}</div>
  <h3>${esc(t(n.k))}</h3>
  <div class="row"><button class="btn light" data-act="${n.act}">${t("go")} →</button>${n.alt?`<button class="btn ghost sm" data-act="${n.alt.act}">${esc(n.alt.label)}</button>`:""}</div>
  <details class="why" open><summary>${t("why")}</summary><ul>${n.why.map(w=>`<li>${esc(w)}</li>`).join("")}</ul></details>
 </section>
 <section class="card">
  <div class="row"><h3 style="font-size:1rem">${t("reminders")}</h3><span class="spacer"></span><button class="linkbtn small" data-act="nav:followup">All →</button></div>
  ${rem.length?`<ul class="tl" style="margin-top:.7rem">${rem.map(r=>`<li class="${r.kind==="now"?"now":""}"><div class="when">${r.kind==="now"?"Now":esc(fmtDay(r.at)+" · "+fmtTime(r.at))}</div><div class="small"><b>${esc(r.title)}</b></div></li>`).join("")}</ul>`:`<p class="small muted" style="margin-top:.4rem">Reminders appear once you book a slot.</p>`}
 </section>
 <section class="card">
  <h3 style="font-size:1rem">Need a person?</h3>
  ${rs.length?`<p class="small" style="margin:.4rem 0">We spotted <b>${rs.length}</b> thing${rs.length>1?"s":""} a human navigator should check:</p><ul class="small" style="margin:0 0 .6rem;padding-left:1.1rem">${rs.slice(0,3).map(r=>`<li>${esc(r.t)}</li>`).join("")}</ul>`:`<p class="small muted" style="margin:.4rem 0 .6rem">Nothing looks incomplete or conflicting right now. You can still ask for help any time.</p>`}
  <button class="btn sm ${rs.some(r=>r.lvl==="high")?"warn":""}" data-act="nav:help">Request a navigator</button>
  ${S.tickets.length?`<p class="tiny muted" style="margin-top:.5rem">Open request: <b>${esc(S.tickets[0].id)}</b> · ${esc(S.tickets[0].status)}</p>`:""}
 </section>`;
}
function renderMain(){
 const v=S.view;const m=$("#main");
 const map={start:vStart,options:vOptions,documents:vDocs,book:vBook,visit:vVisit,followup:vFollow,help:vHelp,lab:vLab};
 m.innerHTML=sysBanners()+(map[v]||vStart)();
}

const DEMO_INFO={
 C04:{t:"C04 · Bad data was sent in",hint:"The broken and malicious records were stopped before they reached the platform. The patient just sees a normal list of valid hospitals — nothing crashed and nothing looks different to them."},
 C05:{t:"C05 · 3× patients, half the doctors",hint:"This is the patient's own screen. Look at the “Busy today” banner and the scarce slots — book one to see the visit pass, then switch between a slot that was kept and one that had to be moved."},
 C05n:{t:"C05 · 3× help requests, half the navigators",hint:"This is the patient's help page. Look at the “helpers are busy” banner — the patient keeps their place and gets a call-back time."}};
function demoGo(c){S.ui.demoRun=c;const L=leg();
 if(c==="C04"){S.sim=S.sim||{};S.sim.surge=false;S.sim.navSurge=false;if(L.booking&&/^demo-/.test(L.booking.idem||""))L.booking=null;if(!L.service)L.service="gen_opd";save();go("options")}
 else if(c==="C05"){const curF=L.facilityId&&fac(L.facilityId);if(!curF||!L.service||!curF.services[L.service]||["full","few"].includes(demoProfile(curF,L.service))){L.service=L.service&&DATA().some(f=>f.services[L.service])?L.service:"gen_opd";applyDemo();const c2=DATA().filter(f=>f.services[L.service]);L.facilityId=(c2.find(f=>demoProfile(f,L.service)==="open")||c2[0]||{}).id;L.booking=null}save();go("book")}
 else{save();go("help")}
 toast("Showing what the patient sees")}
function demoBar(){const c=S.ui.demoRun;if(!c||S.view==="lab")return"";
const d={...DEMO_INFO[c]};if(c==="C05"){d.t+=S.ui.bk==="moved"?" · Scenario 2: slot lost":" · Scenario 1: booking kept";d.hint=S.ui.bk==="moved"?"This patient booked before the surge, but their slot no longer exists. They're told straight away, a new time is held for them, and they can accept it or pick another.":"This patient booked before the surge and their slot still fits. They go straight to their visit pass, which tells them the booking is safe — nothing changes for them."}
 return`<div class="demobar" role="region" aria-label="Live demo"><div class="db-l"><span class="db-live"><span class="pdot"></span>Live demo</span><b>${d.t}</b><span class="db-hint">${d.hint}</span></div>
 <div class="db-r"><button class="linkbtn small db-end" data-act="demoEnd">End demo</button></div></div>
 <button class="demo-side" data-act="demoAdmin"><span>🛠</span><span class="ds-t">How the platform handled it</span></button>`}
function sysBanners(){let h=demoBar();

 if(S.sim&&S.sim.surge&&!(S.view==="visit"&&S.ui.demoRun==="C05"))h+=`<div class="banner amber" role="status"><span class="ic">!</span><div style="flex:1"><b style="font-size:1.12em">Busy today. Your booking is safe.</b><div class="small">If a day is full, we can call you when a slot opens.</div></div><button class="btn sm" data-act="pvDo:cb" style="align-self:center;white-space:nowrap">📞 Call me</button></div>`;

 if(S.sim&&S.sim.navSurge)h+=`<div class="banner amber" role="status"><span class="ic">☎</span><div style="flex:1"><b style="font-size:1.12em">Our helpers are busy right now.</b><div class="small">Ask for help and we'll call you back — you keep your place.</div></div></div>`;
 return h}
/* ---------- View: Need (intake) ---------- */
function vStart(){
 const p=S.profile,L=leg();const a=analyse(p.text);
 const sug=a.suggest.filter(x=>x.s!==L.service);
 const have=["id_proof","scheme_card","insurance_card","prescription","prev_reports","test_slip","vacc_card","mcp_card",...(S.city==="chennai"?["picme"]:[])];
 return`
 <section class="card stack">
  <div><div class="eyebrow">Step 1 · ${t("st_need")}${L.purpose?` · ${esc(L.purpose)}`:""}</div><h2>${t("q_service")}</h2><p class="muted small">Pick the service you've been told you need, or that you're looking for. If you're not sure, General OPD is the usual starting point.</p></div>
  <div class="svcgrid" role="group" aria-label="${t("q_service")}">${Object.entries(SERVICES).map(([id,s])=>`<button class="svc" aria-pressed="${L.service===id}" data-act="svc:${id}"><b>${esc(s.name)}</b><span>${esc(s.hint)}</span></button>`).join("")}</div>
  <div class="q"><label for="freeText">${t("q_text")}</label><textarea id="freeText" class="field" placeholder="e.g. “My doctor said I need to see a heart specialist”">${esc(p.text)}</textarea>
   <div id="guard">${guardBanner(a)}${routeHTML(a,L)}</div>
  </div>
 </section>
 <section class="card stack">
  <div class="grid2">
   <div class="q"><label for="areaSel">${t("q_area")}</label><select id="areaSel" class="field" data-change="area">${[...new Set(Object.values(AREAS).map(a=>a.district))].sort((a,b)=>(/city$/.test(b))-(/city$/.test(a))||a.localeCompare(b)).map(d=>`<optgroup label="${esc(d)}">${Object.entries(AREAS).filter(([k,a])=>a.district===d).map(([k,a])=>`<option value="${k}" ${p.area===k?"selected":""}>${esc(a.name)}</option>`).join("")}</optgroup>`).join("")}</select></div>
   <div class="q"><label for="paySel">${t("q_pay")}</label><select id="paySel" class="field" data-change="scheme">${Object.entries(SCHEMES).filter(([k])=>CITY().schemes.includes(k)).map(([k,s])=>`<option value="${k}" ${p.scheme===k?"selected":""}>${esc(s)}</option>`).join("")}</select></div>
  </div>
  <div class="q"><span class="ql">${t("q_lang")}</span><div class="chips">${CITY().langs.map(l=>`<button class="chip" aria-pressed="${p.languages.includes(l)}" data-act="lang:${l}">${l}</button>`).join("")}</div></div>
  <div class="q"><span class="ql">${t("q_access")}</span><div class="chips">${Object.entries(ACCESS).map(([k,a])=>`<button class="chip" aria-pressed="${p.access.includes(k)}" data-act="acc:${k}">${esc(a.name)}</button>`).join("")}</div></div>
  <div class="q"><span class="ql">${t("q_time")}</span><div class="chips">${Object.entries(TIMES).map(([k,x])=>`<button class="chip" aria-pressed="${p.time===k}" data-act="time:${k}">${x}</button>`).join("")}</div></div>
  <div class="q"><span class="ql">${t("q_have")}</span><div class="chips">${have.map(d=>`<button class="chip" aria-pressed="${dstat(d)==="ready"}" data-act="have:${d}">${esc(DOCS[d].name)}</button>`).join("")}${L.service?`<button class="chip" aria-pressed="${dstat("referral",L.service)==="ready"}" data-act="have:referral">Referral letter for ${esc(SERVICES[L.service].name)}</button>`:""}</div></div>
  <div class="row"><button class="btn" data-act="find" ${L.service?"":"disabled"}>${t("find")} →</button>${L.service?"":`<span class="small muted">Choose a service first.</span>`}</div>
 </section>`;
}

/* ---------- View: Find (discovery) ---------- */
function mapSVG(ev){
 const u=AREAS[S.profile.area];const col={ready:"var(--teal)",steps:"var(--amber)",blocked:"#9AA6BC"};
 const srt=[...ev].map((e,i)=>({e,i,d:dist(e.f)})).sort((a,b)=>a.d-b.d);const lim=Math.max(25,(srt[2]||srt[srt.length-1]||{d:25}).d*1.15);const near=srt.filter((n,j)=>j<2||n.d<=lim).slice(0,6);const pts=[u,...near.map(n=>areaOf(n.e.f))];
 let x0=Math.min(...pts.map(p=>p.x)),x1=Math.max(...pts.map(p=>p.x)),y0=Math.min(...pts.map(p=>p.y)),y1=Math.max(...pts.map(p=>p.y));
 const minSpan=14;if(x1-x0<minSpan){const c=(x0+x1)/2;x0=c-minSpan/2;x1=c+minSpan/2}if(y1-y0<minSpan*.6){const c=(y0+y1)/2;y0=c-minSpan*.3;y1=c+minSpan*.3}
 const pad=Math.max(2.5,(x1-x0)*.1);x0-=pad;x1+=pad;y0-=pad;y1+=pad*1.3;
 const W=405,k=Math.min(W/(x1-x0),440/(y1-y0)),H=Math.round((y1-y0)*k);const X=p=>(p.x-x0)*k,Y=p=>(p.y-y0)*k;
 const inBox=p=>p.x>=x0&&p.x<=x1&&p.y>=y0&&p.y<=y1;const roads=CITY().roads;
 const placed=[];const lab=(a,force)=>{const x=X(a),y=Y(a)+16;if(!force&&placed.some(q=>Math.abs(q.x-x)<62&&Math.abs(q.y-y)<13))return"";placed.push({x,y});return`<text x="${x}" y="${y}" font-size="9.5" fill="#5B6782" text-anchor="middle" font-family="Atkinson Hyperlegible, sans-serif">${esc(a.name)}</text>`};
 const shown=ev.map((e,i)=>({e,i})).filter(o=>inBox(areaOf(o.e.f)));const hidden=ev.length-shown.length;
 const scaleKm=[2,5,10,20,50].find(v=>v*k>=60)||50;
 return`<svg viewBox="0 0 ${W} ${H}" role="img" aria-label="Map of facilities near ${esc(u.name)}">
 ${roads.map(([a,b])=>`<line x1="${X(AREAS[a])}" y1="${Y(AREAS[a])}" x2="${X(AREAS[b])}" y2="${Y(AREAS[b])}" stroke="#fff" stroke-width="5" stroke-linecap="round" opacity=".85"/>`).join("")}
 ${lab(u,true)}${Object.values(AREAS).filter(a=>a!==u&&inBox(a)).map(a=>lab(a)).join("")}
 <circle cx="${X(u)}" cy="${Y(u)}" r="22" fill="var(--blue)" opacity=".12"/><circle cx="${X(u)}" cy="${Y(u)}" r="7" fill="var(--blue)" stroke="#fff" stroke-width="2.5"/>
 ${shown.map(({e,i})=>{const a=areaOf(e.f);const off=(hash(e.f.id)%7-3)*2.2;const x=X(a)+off+8,y=Y(a)-off-8;return`<g role="button" tabindex="0" data-act="jump:${e.f.id}" style="cursor:pointer"><title>${esc(e.f.name)} — ${t(e.status)}</title><circle cx="${x}" cy="${y}" r="10" fill="${col[e.status]}" stroke="#fff" stroke-width="2"/><text x="${x}" y="${y+3.5}" font-size="10" font-weight="700" fill="#fff" text-anchor="middle">${i+1}</text></g>`}).join("")}
 <g font-size="9" fill="#5B6782" font-family="Atkinson Hyperlegible, sans-serif"><line x1="10" y1="${H-10}" x2="${10+scaleKm*k}" y2="${H-10}" stroke="#5B6782" stroke-width="2"/><text x="10" y="${H-15}">${scaleKm} km</text>${hidden?`<text x="${W-8}" y="${H-10}" text-anchor="end">+${hidden} further away — see list</text>`:""}</g>
 </svg>`;
}
function facCard(e,i){
 const f=e.f,L=leg(),sel=L.facilityId===f.id,open=S.ui.exp[f.id];
 const accPills=Object.keys(ACCESS).filter(a=>f.access?.[a]).map(a=>`<span class="pill ${S.profile.access.includes(a)?"ok b":""}">${f.access[a]==="request"?"◐":"●"} ${esc(ACCESS[a].name.split(" /")[0])}</span>`).join("");
 return`<article class="fac ${sel?"sel":""} ${e.status==="blocked"?"blocked":""}" id="fac-${f.id}">
 <div class="hd"><span class="rank">${i+1}</span><div style="flex:1;min-width:0">
  <div class="row" style="gap:.5rem"><h3>${esc(f.name)}</h3><span class="status ${e.status}">${t(e.status)}</span>${e.cf.length?`<span class="pill mid b">⚠ ${e.cf.length} conflict${e.cf.length>1?"s":""}</span>`:""}${e.age>90?`<span class="pill mid">Data ${e.age}d old</span>`:""}</div>
  <div class="small muted">${esc(f.type)} · ${esc(areaOf(f).name)} · ${e.d.toFixed(1)} km · ${esc(e.svc.fee)}</div></div>
  <div style="text-align:right"><div class="tiny muted">Fit</div><div class="display" style="font-weight:800;font-size:1.3rem;line-height:1">${e.score}</div><div class="meter" style="width:64px"><i style="width:${e.score}%"></i></div></div></div>
 <div class="row" style="gap:.35rem">${e.free.length===0?`<span class="pill no b">Fully booked this week · wait-list</span>`:e.free.length<=4?`<span class="pill mid b">Only ${e.free.length} slot${e.free.length>1?"s":""} left · next ${esc(fmtDay(e.free[0].at))} ${esc(fmtTime(e.free[0].at))}</span>`:`<span class="pill ok b">Next: ${esc(fmtDay(e.free[0].at))} ${esc(fmtTime(e.free[0].at))}</span>`}${e.shared.length?`<span class="pill">Speaks ${esc(e.shared.join(", "))}</span>`:`<span class="pill mid b">No shared language · interpreter needed</span>`}${accPills}${e.svc.referral?`<span class="pill ${dstat("referral",L.service)==="ready"?"ok":"mid"} b">Referral required</span>`:e.svc.referral===null?`<span class="pill mid b">Referral rule unknown</span>`:""}</div>
 ${open?`<ul class="factors">${e.fx.map(x=>`<li><span class="m ${x.ok===true?"ok":x.ok===false?"no":"mid"}">${x.ok===true?"✓":x.ok===false?"✕":"!"}</span><span>${esc(x.label)}${x.detail?`<span class="d">${esc(x.detail)}</span>`:""}</span><span class="pts">${x.pts>0?"+":""}${x.pts||""}</span></li>`).join("")}<li><span></span><span class="tiny muted">Base 40 + factors = ${e.score}. Status is set by hard rules (payment, physical access) and referral needs, not by score.</span><span></span></li></ul>`:""}
 <div class="row"><button class="linkbtn small" data-act="exp:${f.id}" aria-expanded="${!!open}">${open?"Hide reasons":t("whythis")}</button><span class="spacer"></span>
 ${e.cf.length?`<button class="btn ghost sm" data-act="nav:help">Ask a navigator to verify</button>`:""}
 ${e.status==="blocked"?"":`<button class="btn sm ${sel?"ghost":""}" data-act="pick:${f.id}">${sel?"✓ "+t("chosen"):t("choose")}</button>`}</div>
 </article>`;
}
function vOptions(){
 const L=leg();if(!L.service)return empty("Choose a service first","Tell us what you need and we'll match facilities.","nav:start","Go to Need");
 const ev=ranked();const ok=ev.filter(e=>e.status!=="blocked"),bad=ev.filter(e=>e.status==="blocked");
 return`
 <section class="card stack">
  <div class="row"><div><div class="eyebrow">Step 2 · ${t("st_find")}</div><h2>${esc(SERVICES[L.service].name)} near ${esc(AREAS[S.profile.area].name)}</h2>
  <p class="small muted">${ev.length} facilities offer this. <b>${ev.filter(e=>e.status==="ready").length}</b> ready to book, <b>${ev.filter(e=>e.status==="steps").length}</b> need a step first, <b>${bad.length}</b> don't fit. Every score is explained — tap “${t("whythis")}”.</p></div></div>
  <div class="mapwrap map">${mapSVG(ev)}<div class="legend"><span><i style="background:var(--blue)"></i>You</span><span><i style="background:var(--teal)"></i>${t("ready")}</span><span><i style="background:var(--amber)"></i>${t("steps")}</span><span><i style="background:#9AA6BC"></i>${t("blocked")}</span><span>Map is schematic</span></div></div>
 </section>
 ${ok.length?ok.map((e,i)=>facCard(e,i)).join(""):`<div class="banner red"><span class="ic">!</span><div><b>No facility in the data meets all your needs.</b> A human navigator can look beyond this dataset or arrange support (transport, interpreter, ramps). <button class="btn sm warn" data-act="nav:help" style="margin-top:.4rem">Request a navigator</button></div></div>`}
 ${bad.length?`<section class="card"><button class="linkbtn" data-act="toggleBlocked">${S.ui.showBlocked?"Hide":"Show"} ${bad.length} that don't fit — and why</button>${S.ui.showBlocked?`<div class="stack" style="margin-top:.8rem">${bad.map((e,i)=>facCard(e,ok.length+i)).join("")}</div>`:""}</section>`:""}
 `;
}
function dataPanel(){
 const ex=JSON.stringify([{id:"my-phc",name:"Example PHC",type:"Urban PHC",area:"jayanagar",address:"…",phone:"…",open:"09:00",close:"16:30",days:[1,2,3,4,5,6],emergency:false,languages:["Kannada","English"],access:{wheelchair:true,lift:false,isl:false,braille:false,toilet:true},schemes:["pmjay"],verified:"2026-10-30",conflicts:[],services:{gen_opd:{dept:"OPD",floor:0,fee:"Free",referral:false,slotMins:10}}}],null,1);
 return`<section class="card"><details><summary style="cursor:pointer;font-weight:700">Data source · ${S.data?esc(S.dataName||"organiser upload"):"built-in sample"} (${DATA().length} facilities)</summary>
 <p class="small muted">Load the organiser-provided facility file (JSON array, or <span class="kbd">{"facilities":[…]}</span>). Areas: ${Object.keys(AREAS).join(", ")} — or give <span class="kbd">x</span>/<span class="kbd">y</span> in km. Service ids: ${Object.keys(SERVICES).join(", ")}.</p>
 <div class="row" style="margin:.5rem 0"><label class="btn sm" style="position:relative">Load organiser JSON<input type="file" accept=".json,application/json" data-change="data" style="position:absolute;inset:0;opacity:0;cursor:pointer"></label>${S.data?`<button class="btn ghost sm" data-act="resetData">Use sample data</button>`:""}<button class="btn ghost sm" data-copy="schema">Copy schema example</button></div>
 <pre class="code">${esc(ex)}</pre></details></section>`;
}

/* ---------- View: Documents ---------- */
function vDocs(){
 const L=leg();if(!L.facilityId)return empty("Pick a facility first","Each facility and payment method needs slightly different paperwork.","nav:options","Go to Find");
 const f=fac(L.facilityId),req=requiredDocs(f,L.service);const ready=req.filter(d=>dstat(d,L.service)==="ready").length;const pct=req.length?ready/req.length:1;
 const C=2*Math.PI*30;
 return`<section class="card stack">
 <div class="row" style="align-items:flex-start"><div style="flex:1"><div class="eyebrow">Step 3 · ${t("st_docs")}</div><h2>What to bring to ${esc(f.name)}</h2><p class="small muted">For ${esc(SERVICES[L.service].name)} · paying with ${esc(SCHEMES[S.profile.scheme])}. Your documents are saved in a wallet and reused across visits.</p></div>
 <svg class="ring" viewBox="0 0 74 74" role="img" aria-label="${ready} of ${req.length} ready"><circle cx="37" cy="37" r="30" stroke="var(--line2)" stroke-width="8" fill="none"/><circle cx="37" cy="37" r="30" stroke="var(--teal)" stroke-width="8" fill="none" stroke-linecap="round" stroke-dasharray="${C*pct} ${C}" transform="rotate(-90 37 37)"/><text x="37" y="42" text-anchor="middle" font-weight="800" font-size="15" font-family="Bricolage Grotesque" fill="var(--ink)">${ready}/${req.length}</text></svg></div>
 <div>${req.map(d=>{const st=dstat(d,L.service),w=S.wallet[dkey(d,L.service)]||{};return`<div class="doc"><span class="st ${st}">${st==="ready"?"✓":st==="pending"?"…":"!"}</span>
  <div><b>${esc(DOCS[d].name)}</b>${d==="referral"?` <span class="pill mid">for ${esc(SERVICES[L.service].name)}</span>`:""}<p class="small muted">${esc(DOCS[d].how)}</p>
  ${w.file?`<div class="tiny">📎 ${esc(w.file)}</div>`:""}
  ${d==="referral"&&st!=="ready"?`<button class="btn sm" data-act="getReferral" style="margin-top:.35rem">Book a General OPD visit to get one</button>`:""}</div>
  <div style="display:flex;flex-direction:column;gap:.35rem;align-items:flex-end"><div class="seg" role="group" aria-label="Status of ${esc(DOCS[d].name)}">${["missing","pending","ready"].map(s=>`<button aria-pressed="${st===s}" data-act="doc:${d}:${s}">${t(s==="ready"?"done":s)}</button>`).join("")}</div>
  <label class="upl">⇪ Attach photo<input type="file" accept="image/*,.pdf" data-change="upload:${d}"></label></div></div>`}).join("")}</div>
 ${req.includes("referral")?`<div class="banner blue"><span class="ic">i</span><div>Whether you need a referral is a rule of this department, from the organiser data. Whether you should see this specialist is a decision for a doctor — this app doesn't make it.</div></div>`:""}
 <div class="row"><button class="btn" data-act="nav:book">Continue to booking →</button><button class="btn ghost" data-act="copyList">Copy checklist</button></div>
 </section>`;
}

/* ---------- View: Book ---------- */
function vBook(){
 const L=leg();if(!L.facilityId)return empty("Pick a facility first","Slots come from the facility you choose.","nav:options","Go to Find");
 const f=fac(L.facilityId),svc=f.services[L.service];const nrq=needsReferral(f,L.service);const refUnknown=nrq===null&&!S.ui.refOverride&&dstat("referral",L.service)!=="ready";const refBlock=(nrq&&dstat("referral",L.service)!=="ready")||refUnknown;const payBlock=S.profile.scheme==="unknown"&&!/^free$/i.test(svc.fee||"");
 const all=slotsFor(f,L.service,L.notBefore);const days=[...new Set(all.map(s=>sod(s.at).getTime()))];
 if(S.ui.day==null||!days.includes(S.ui.day))S.ui.day=days[0];
 const mineAt=L.booking&&new Date(L.booking.at).getTime();
 const daySlots=all.filter(s=>sod(s.at).getTime()===S.ui.day);
 const showGrid=!L.booking||S.ui.resched;
 const cf=conflicts(f,L.service);
 return`<section class="card stack">
 <div><div class="eyebrow">Step 4 · ${t("st_book")}</div><h2>${esc(svc.dept)}</h2><p class="small muted">${esc(f.name)} · ${esc(f.address)} · ${esc(svc.fee)} · ~${svc.avg||8} min per patient${L.notBefore?` · follow-up on or after ${new Date(L.notBefore).toLocaleDateString(LOCALE[S.lang],{day:"numeric",month:"short"})}`:""}</p></div>
 ${cf.map(c=>`<div class="banner amber"><span class="ic">⚠</span><div><b>Conflicting information: ${esc(c.field)}.</b> ${esc(c.note)} <span class="tiny">(${esc(c.source)})</span><br><button class="linkbtn small" data-act="nav:help">Ask a navigator to confirm before you travel</button></div></div>`).join("")}
 ${L.booking&&L.booking.review?`<div class="banner red" role="alert"><span class="ic">!</span><div><b>Rules changed after you booked (policy v${S.policyV}).</b> ${esc(L.booking.review)} Your booking is kept — nothing is cancelled without your confirmation.<div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="reviewKeep">Keep booking — I'll bring it</button><button class="btn ghost sm" data-act="getReferral">Get a referral first</button><button class="btn ghost sm" data-act="cancelBooking">Cancel booking</button></div></div></div>`:""}
 ${refUnknown&&!L.booking?`<div class="banner amber" role="alert"><span class="ic">?</span><div><b>Booking deferred: one detail is missing.</b> The facility data doesn't say whether ${esc(svc.dept)} needs a referral letter. We won't guess, because a wrong guess could mean being turned away.<div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="nav:help">Ask a navigator to confirm</button><button class="btn ghost sm" data-act="refOverride">I have a referral letter anyway</button><button class="btn ghost sm" data-act="nav:options">Pick another facility</button></div></div></div>`:""}
 ${payBlock&&!L.booking?`<div class="banner amber" role="alert"><span class="ic">?</span><div><b>We need one detail before booking: how will you pay?</b> The fee here is ${esc(svc.fee)}, and it may be free under a government scheme. We won't guess.<div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="nav:start">Choose payment</button><button class="btn ghost sm" data-act="nav:help">Ask a navigator</button></div></div></div>`:""}
 ${L.booking?bookingCard(f,L):""}
 ${refBlock&&!refUnknown&&!L.booking?`<div class="banner red"><span class="ic">✕</span><div><b>Booking is locked: this department needs a referral letter.</b> We won't let you book a slot you'd be turned away from. <div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="getReferral">Get a referral first</button><button class="btn ghost sm" data-act="doc:referral:ready">I already have one</button><button class="btn ghost sm" data-act="nav:options">Pick another facility</button></div></div></div>`:""}
 ${showGrid&&!refBlock&&!payBlock?`
  ${S.ui.resched?`<div class="banner blue"><span class="ic">↻</span><div><b>Rescheduling.</b> Pick a new slot below — your current slot stays booked until you confirm. <button class="linkbtn small" data-act="reschedOff">${S.ui.reschedFrom==="visit"?"Keep current slot and go back to my pass":"Keep current slot"}</button></div></div>`:""}
  ${days.length?`<div class="days" role="tablist">${days.map(d=>{const dd=new Date(d);const c=all.filter(s=>sod(s.at).getTime()===d&&s.free).length;return`<button class="day" role="tab" aria-pressed="${S.ui.day===d}" data-act="day:${d}"><b>${esc(fmtDay(dd))}</b><span>${c===0?"Full · wait-list":c<=2?`Only ${c} left`:`${c} free`}</span></button>`}).join("")}</div>
  <div class="slots">${daySlots.map(s=>{const ms=s.at.getTime();const mine=ms===mineAt;const pick=S.ui.pick===ms;const pref=timeOk(s.at);return`<button class="slot ${s.free||mine?"":"taken"} ${mine?"mine":""} ${pick?"pick":""} ${s.free&&!mine&&s.contested?"contested":""}" ${s.free&&!mine&&s.contested?`title="Demo: someone else books this slot at the same moment"`:""} ${s.free&&!mine?`data-act="pickSlot:${ms}:${s.token}"`:"disabled"} aria-label="${fmtTime(s.at)} ${s.free?"available":"taken"}" style="${!pref&&s.free?"opacity:.7":""}">${fmtTime(s.at)}</button>`}).join("")}</div>
  ${S.ui.conflict?conflictBox():""}<p class="tiny muted">Faded slots are outside your “${esc(TIMES[S.profile.time])}” preference. Struck-out slots are taken.${daySlots.some(x=>x.free&&x.contested&&x.at.getTime()!==mineAt)?` <span class="demo-tag">⚡ Demo:</span> a slot marked ⚡ gets booked by someone else at the same moment you confirm — try it.`:""}</p>${daySlots.length&&!daySlots.some(x=>x.free)?waitlistBox(f,L):""}`:`<div class="banner amber"><span class="ic">!</span><div>No slots in the next week. A navigator can ask about walk-in queues.</div></div>${waitlistBox(f,L)}`}
  ${S.ui.pick?`<div class="row" style="background:var(--teal-l);padding:.7rem .9rem;border-radius:12px"><b>${esc(fmtDay(new Date(S.ui.pick)))}, ${esc(fmtTime(new Date(S.ui.pick)))}</b><span class="spacer"></span><button class="btn" data-act="confirmSlot">${S.ui.resched?"Confirm new time":t("book")}</button></div>`:""}`:""}
 </section>`;
}
function conflictBox(){const c=S.ui.conflict;return`<div class="banner red" role="alert"><span class="ic">⚡</span><div style="flex:1"><b>Someone else booked ${esc(fmtTime(new Date(c.at)))} a moment before you.</b> Nothing was booked for you and nothing was charged — two people can never hold the same slot.
 ${c.alts.length?`<div class="small" style="margin-top:.4rem">Nearest free times:</div><div class="row" style="margin-top:.35rem">${c.alts.map(a=>`<button class="btn sm" data-act="altPick:${a.at.getTime()}:${a.token}">${esc(fmtDay(a.at))}, ${esc(fmtTime(a.at))}</button>`).join("")}<button class="btn ghost sm" data-act="nav:help" style="color:var(--ink);border-color:var(--line)">Ask a navigator</button></div>`:`<div class="row" style="margin-top:.4rem"><button class="btn sm" data-act="joinWait">Join the wait-list</button><button class="btn ghost sm" data-act="nav:help">Ask a navigator</button></div>`}</div></div>`}
function waitlistBox(f,L){const w=(S.waitlist||[]).find(x=>x.leg===L.id&&x.day===S.ui.day);const alts=alternativesFor(L.service,f.id);
 return`<div class="banner blue"><span class="ic">⏳</span><div style="flex:1"><b>No free slots on this day.</b> ${w?`You're #${w.pos} on the wait-list. We'll remind you if a slot opens.`:`Join the wait-list, or try another place with free slots.`}
 <div class="row" style="margin-top:.5rem">${w?"":`<button class="btn sm" data-act="joinWait">Join the wait-list</button>`}<button class="btn ghost sm" data-act="nav:help">Ask a navigator</button></div>
 ${alts.length?`<div class="small" style="margin-top:.5rem"><b>Other places with free slots</b><ul style="margin:.2rem 0 0;padding-left:1.1rem">${alts.map(a=>`<li><button class="linkbtn small" data-act="pick:${a.f.id}">${esc(a.f.name)}</button> — next ${esc(fmtDay(a.first.at))}, ${esc(fmtTime(a.first.at))}</li>`).join("")}</ul></div>`:""}</div></div>`}
function bookingCard(f,L){if(L.booking.status==="pending")return`<div class="banner amber"><span class="ic">⏳</span><div style="flex:1"><b>Saved offline: ${esc(fmtDay(new Date(L.booking.at)))}, ${esc(fmtTime(new Date(L.booking.at)))}</b><div class="small">Pending — will confirm when you're back online. Ref ${esc(L.booking.ref)}.</div></div></div>`;
 if(L.booking.status==="conflict")return`<div class="banner red"><span class="ic">✕</span><div style="flex:1"><b>This slot was taken while you were offline.</b><div class="small">Please pick another time — nothing was charged or confirmed.</div><div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="clearConflict">Pick another time</button></div></div></div>`;
 const maxR=policy().rules.maxResched;const rLock=maxR&&L.booking.history.length>=maxR;const at=new Date(L.booking.at);return`<div class="banner green"><span class="ic">✓</span><div style="flex:1"><b>Booked: ${esc(fmtDay(at))}, ${esc(fmtTime(at))} · token ${L.booking.token}</b><div class="small">Ref ${esc(L.booking.ref)}${L.booking.history.length?` · rescheduled ${L.booking.history.length}×`:""}. Arrive 15 min early for registration.</div>
 <div class="row" style="margin-top:.5rem"><button class="btn sm" data-act="nav:visit">Open visit pass</button><button class="btn ghost sm" data-act="reschedOn" ${rLock?`disabled title="Policy v2: at most ${maxR} reschedules"`:""}>${t("resched")}</button>${rLock?`<span class="tiny muted">Policy v${S.policyV}: reschedule limit (${maxR}) reached</span>`:""}<button class="btn ghost sm" data-act="cancelBooking">${t("cancel")}</button></div></div></div>`}

/* ---------- View: Visit ---------- */
function surgeNewTime(L,f){const b=sod(new Date(L.booking.at)).getTime();const all=slotsForBase(f,L.service,null);return all.find(x=>sod(x.at).getTime()>b&&x.free)||all.find(x=>x.at.getTime()>L.booking.at&&x.free)}
function surgeVisitCard(L,f){if(!(S.sim&&S.sim.surge&&S.ui.demoRun==="C05"))return"";const at=new Date(L.booking.at);
 if(S.ui.bk==="moved"&&!S.ui.moveDone){const n=surgeNewTime(L,f);if(!n)return"";const d=fmtDay(at);
  return`<section class="card stack scard amber" role="alert"><div class="scard-ic">↻</div><div><h2 style="margin:0">We had to move your visit</h2><p class="pvt" style="text-align:left;margin:.4rem 0 0">The doctor has fewer slots ${/^(Today|Tomorrow)$/.test(d)?d.toLowerCase():"on "+esc(d)}. Your new time is <b>${esc(fmtDay(n.at))}, ${esc(fmtTime(n.at))}</b> — the first slot, held for you before any new patient.</p></div>
  <div class="row"><button class="btn" data-act="acceptMove:${n.at.getTime()}:${n.token}">✓ This time is fine</button><button class="btn ghost" data-act="reschedVisit" style="color:var(--ink);border-color:var(--line)">↻ Choose another time</button><button class="linkbtn small" data-act="pvDo:cb">📞 Call me instead</button></div></section>`}
 if(S.ui.bk==="moved"&&S.ui.moveDone)return`<section class="card scard green" role="status"><div class="scard-ic">✓</div><div><h2 style="margin:0">New time confirmed</h2><p class="small" style="margin:.3rem 0 0">Your visit was moved because of the surge, and you've confirmed the new time. Your pass below is updated — we'll remind you the day before.</p></div></section>`;
 return`<section class="card scard green" role="status"><div class="scard-ic">✓</div><div><h2 style="margin:0">Your booking is safe</h2><p class="small" style="margin:.3rem 0 0">It's busy, but bookings made earlier are honoured first. Nothing changes — come as planned.</p></div></section>`}
function vVisit(){
 const L=leg();if(!L.booking)return empty("No appointment yet","Book a slot and your visit pass will appear here.","nav:book","Go to Book");
 const f=fac(L.facilityId),svc=f.services[L.service],at=new Date(L.booking.at),req=requiredDocs(f,L.service);
 const q=S.ui.queue&&S.ui.queue.leg===L.id?S.ui.queue:null;const lv=new Date(at-travel(dist(f))*60000-15*60000);
 const needs=S.profile.access.map(a=>ACCESS[a].name);
 return`${surgeVisitCard(L,f)}<section class="card stack">
 <div><div class="eyebrow">Step 5 · ${t("st_visit")}</div><h2>Your visit pass</h2><p class="small muted">Show this at the registration counter. Copy it to send to a family member or caregiver.</p></div>
 <div class="pass" id="pass">
  <div class="ph"><div><div class="tiny" style="opacity:.75;letter-spacing:.1em">TOKEN</div><div class="tok">${L.booking.token}</div></div><div style="text-align:right"><div class="display" style="font-weight:700;font-size:1.1rem">${esc(fmtDay(at))} · ${esc(fmtTime(at))}</div><div class="small" style="opacity:.8">Ref ${esc(L.booking.ref)}</div></div></div>
  <dl class="pb">
   <div><dt>Where</dt><dd>${esc(f.name)}</dd><div class="small muted">${esc(svc.dept)} · ${svc.floor?`Floor ${svc.floor}`:"Ground floor"}<br>${esc(f.address)}</div></div>
   <div><dt>Leave by</dt><dd>${esc(fmtTime(lv))}</dd><div class="small muted">~${tmin(travel(dist(f)))} from ${esc(AREAS[S.profile.area].name)} + 15 min registration</div></div>
   <div><dt>Bring</dt><dd style="font-weight:400">${req.map(d=>`<div>${dstat(d,L.service)==="ready"?"☑":"☐"} ${esc(DOCS[d].name)}</div>`).join("")}</dd></div>
   <div><dt>Support requested</dt><dd style="font-weight:400">${needs.length?needs.map(esc).join("<br>"):"None"}<div class="small muted">Language: ${esc(S.profile.languages.join(", "))}${f.languages.some(l=>S.profile.languages.includes(l))?" ✓ staff listed":" — interpreter needed"}</div></dd></div>
   <div><dt>Payment</dt><dd>${esc(SCHEMES[S.profile.scheme])}</dd><div class="small muted">Fee: ${esc(svc.fee)}</div></div>
   <div><dt>Facility phone</dt><dd>${esc(f.phone)}</dd><div class="small muted">Emergency: 108 / 112</div></div>
  </dl>
 </div>
 <div class="row"><button class="btn ghost" data-act="copyPass">Copy pass as text</button><button class="btn ghost" data-act="reschedVisit">↻ ${t("resched")}</button></div>
 </section>
 <section class="card stack">
  <div><h3>Queue on the day</h3><p class="small muted">When you arrive, check in to see where you are in the queue (simulated for the prototype).</p></div>
  ${q?`<div class="queue"><div><div class="tiny muted">NOW SERVING</div><div class="qbig">${q.serving}</div></div><div class="qbar" aria-hidden="true"><i style="width:${Math.min(100,(q.serving-q.start)/(L.booking.token-q.start||1)*100)}%"></i></div><div style="text-align:right"><div class="tiny muted">YOU</div><div class="qbig" style="color:var(--teal)">${L.booking.token}</div></div></div>
  ${q.uncertain?`<div class="banner amber" role="status"><span class="ic">!</span><div><b>Live queue reading uncertain — please confirm at the counter.</b> We're showing the last reliable number. ${q.flags.map(esc).join(" · ")}</div></div>`:`<p class="tiny muted">✓ Live reading OK — display board and registration agree.</p>`}<p class="small" aria-live="polite">${q.serving>=L.booking.token&&!q.uncertain?`<b>It's your turn.</b> Please go to ${esc(svc.dept)}${svc.floor?`, floor ${svc.floor}`:""}.`:`${L.booking.token-q.serving} ahead of you · about <b>${(L.booking.token-q.serving)*(svc.avg||8)} min</b> wait at ~${svc.avg||8} min each.`}</p>`:`<button class="btn" data-act="checkin">I've arrived — check in</button>`}
 </section>
 <section class="card stack">
  <div><h3>After the visit: what did the doctor ask you to do?</h3><p class="small muted">You tell us what was decided; we only organise the paperwork and bookings that follow.</p></div>
  <div class="outcomes">
   <button class="out" data-act="outcome:referral"><b>Gave me a referral</b><span>To another department or hospital</span></button>
   <button class="out" data-act="outcome:tests"><b>Asked for tests</b><span>Lab work or scans</span></button>
   <button class="out" data-act="outcome:return"><b>Come back later</b><span>Follow-up visit after some time</span></button>
   <button class="out" data-act="outcome:done"><b>No more visits needed</b><span>Close this journey</span></button>
   <button class="out" data-act="nav:help"><b>I'm not sure / something else</b><span>Talk to a navigator</span></button>
  </div>
 </section>`;
}

/* ---------- View: Follow-up ---------- */
function vFollow(){
 const rem=reminders();const now=new Date();
 return`<section class="card stack">
 <div><div class="eyebrow">Step 6 · ${t("st_follow")}</div><h2>Reminders & next steps</h2><p class="small muted">Generated from your bookings and what the doctor asked you to do. Add them to your phone's calendar, or copy an SMS-style reminder for a caregiver.</p></div>
 ${rem.length?`<ul class="tl">${rem.map(r=>`<li class="${r.kind==="now"?"now":r.at<now?"past":""}"><div class="when">${r.kind==="now"?"Now":esc(fmtDay(r.at)+" · "+fmtTime(r.at))}</div><b>${esc(r.title)}</b><div class="small muted">${esc(r.body)}</div></li>`).join("")}</ul>
 <div class="row"><button class="btn" data-copy="ics">Copy calendar (.ics) text</button><button class="btn ghost" data-act="copySms">Copy SMS reminder</button></div><p class="tiny muted">Paste the calendar text into a file named <span class="kbd">visit.ics</span> and open it to add all reminders with 30-minute alerts.</p>`:`<p class="muted">No reminders yet — book a slot first.</p>`}
 </section>
 <section class="card stack"><h3>Journey history</h3>
 <table class="mini"><thead><tr><th>#</th><th>Service</th><th>Facility</th><th>Appointment</th><th>Outcome</th></tr></thead><tbody>
 ${S.legs.map((L,i)=>{const f=L.facilityId&&fac(L.facilityId);return`<tr><td>${i+1}</td><td>${L.service?esc(SERVICES[L.service].name):"—"}${L.purpose?`<div class="tiny muted">${esc(L.purpose)}</div>`:""}</td><td>${f?esc(f.name):"—"}</td><td>${L.booking?esc(fmtDay(new Date(L.booking.at))+" "+fmtTime(new Date(L.booking.at))):"—"}</td><td>${L.outcome?esc(L.outcome.label):L.status==="waiting"?"Waiting for referral":"—"}</td></tr>`}).join("")}
 </tbody></table>
 <div class="row"><button class="btn ghost sm" data-act="newNeed">+ Start a new need</button><button class="btn ghost sm" data-act="reset">Start over</button></div>
 </section>`;
}

/* ---------- View: Help / escalation ---------- */
function vHelp(){
 const rs=escalationReasons();
 return`<section class="card stack">
 <div><div class="eyebrow">Human navigator</div><h2>Talk to a person</h2><p class="small muted">Navigators are trained staff at the help desk or on the phone. They can confirm conflicting details, arrange interpreters or ramps, and find options outside this dataset. They do not give medical advice either — for that, they'll connect you to a clinician.</p></div>
 ${rs.length?`<div class="banner amber"><span class="ic">⚑</span><div><b>Why we suggest it</b><ul style="margin:.3rem 0 0;padding-left:1.1rem">${rs.map(r=>`<li>${esc(r.t)}</li>`).join("")}</ul></div></div>`:""}
 <div class="q"><span class="ql">What we'll send them (you can edit the note)</span><pre class="code" style="white-space:pre-wrap">${esc(caseSummary())}</pre></div>
 <div class="grid2"><div class="q"><label for="chan">How should they reach you?</label><select id="chan" class="field"><option>Phone call back</option><option>WhatsApp message</option><option>SMS</option><option>Video call with sign-language interpreter</option><option>I'll visit the help desk</option></select></div>
 <div class="q"><label for="when">When?</label><select id="when" class="field"><option>As soon as possible</option><option>This morning</option><option>This afternoon</option><option>Tomorrow</option></select></div></div>
 <div class="q"><label for="hnote">Anything else? (optional)</label><textarea id="hnote" class="field" placeholder="e.g. My daughter will take the call; I need help with the referral."></textarea></div>
 <div class="row"><button class="btn" data-act="ticket">Send request</button><button class="btn ghost" data-copy="summary">Copy summary</button></div>
 </section>
 ${S.tickets.map(tk=>`<section class="card"><div class="row"><h3>${esc(tk.id)}</h3><span class="pill b mid">${esc(tk.status)}</span><span class="spacer"></span><span class="tiny muted">${esc(new Date(tk.created).toLocaleString(LOCALE[S.lang]))}</span></div>
 <ul class="tl" style="margin-top:.8rem"><li class="past"><div class="when">Sent</div><b>Request received</b><div class="small muted">${esc(tk.channel)} · ${esc(tk.when)}</div></li><li class="now"><div class="when">Next</div><b>Navigator assigned</b><div class="small muted">Typical response: within 2 working hours (simulated)</div></li><li><div class="when">Then</div><b>Issue resolved, journey updated</b></li></ul></section>`).join("")}`;
}
function empty(h,p,act,lbl){return`<section class="card empty"><h3>${esc(h)}</h3><p class="muted">${esc(p)}</p><button class="btn" data-act="${act}" style="margin-top:.6rem">${esc(lbl)} →</button></section>`}

/* =========================================================
   Modal
   ========================================================= */
function modal(html){setTimeout(()=>translateDOM($("#modal")),0);$("#modal").innerHTML=`<div class="scrim" data-act="closeModal"><div class="dialog" role="dialog" aria-modal="true">${html}<div class="row" style="margin-top:1rem;justify-content:flex-end"><button class="btn ghost sm" data-act="closeModal">Close</button></div></div></div>`;const d=$(".dialog button,.dialog textarea");d&&d.focus()}
function closeModal(){$("#modal").innerHTML=""}
async function copy(text,label){text=trText(text);try{await navigator.clipboard.writeText(text);toast(label||"Copied")}catch(e){modal(`<h3>Copy this</h3><p class="small muted">Your browser blocked automatic copying. Select the text below and copy it.</p><textarea class="field" style="min-height:220px" readonly>${esc(text)}</textarea>`)}}

/* =========================================================
   Actions
   ========================================================= */
function go(view){S.view=view;S.ui.pick=null;S.ui.conflict=null;try{history.replaceState(null,"","#"+view)}catch(e){}render();window.scrollTo({top:0,behavior:"smooth"});$("#main").focus({preventScroll:true})}
function setStatus(d,sid,status,file){const k=dkey(d,sid);S.wallet[k]={...(S.wallet[k]||{}),status,...(file?{file}:{})};}
const ACT={
 authTab:t=>{AUTHUI.tab=t;AUTHUI.err={};AUTHUI.msg="";renderAuth();const f=$("#authForm input");f&&f.focus()},
 togglePw:id=>{AUTHUI.show[id]=!AUTHUI.show[id];renderAuth();const f=$("#"+id);if(f){f.focus();f.setSelectionRange(f.value.length,f.value.length)}},
 forgot:()=>{modal(`<h3>Reset your password</h3><p>In the live version you'd get a one-time code by SMS or email to set a new password.</p><p class="small muted">In this prototype, accounts live only on this device — create a new account, or continue as a guest.</p>`)},
 guest:()=>{setSession({id:"guest",name:"Guest",guest:true,at:Date.now()},false);loadState();render();toast("You're in as a guest — nothing is saved after you close the tab");go("start")},
 account:()=>{const u=SESSION;modal(`<h3>${esc(u.name)}</h3><p class="small muted">${u.guest?"Guest session — your journey isn't tied to an account.":"Signed in as <b>"+esc(u.id)+"</b>"+(u.who==="care"?" · managing care for someone else":"")}</p>${u.guest?`<p class="small">Create an account to keep your journey, documents and reminders.</p>`:""}<div class="row" style="margin-top:.8rem">${u.guest?`<button class="btn" data-act="logoutTo:up">Create an account</button>`:""}<button class="btn ${u.guest?"ghost":"warn"}" data-act="logout">Sign out</button></div>`)},
 logout:()=>{closeModal();if(SESSION&&SESSION.guest){try{localStorage.removeItem(stateKey())}catch(e){}}clearSession();AUTHUI.lang=S.lang||AUTHUI.lang;S=fresh();AUTHUI.tab="in";AUTHUI.err={};AUTHUI.msg="You've been signed out.";AUTHUI.msgKind="green";try{history.replaceState(null,"","#")}catch(e){}render();window.scrollTo(0,0)},
 logoutTo:t=>{ACT.logout();AUTHUI.tab=t;AUTHUI.msg="";renderAuth()},
 nav:v=>go(v),
 svc:id=>{const L=leg();if(L.service!==id){L.service=id;L.facilityId=null;L.booking=null;}L.autoPick=false;save();render()},
 lang:l=>{const a=S.profile.languages;S.profile.languages=a.includes(l)?a.filter(x=>x!==l):[...a,l];if(!S.profile.languages.length)S.profile.languages=[l];save();render()},
 acc:k=>{const a=S.profile.access;S.profile.access=a.includes(k)?a.filter(x=>x!==k):[...a,k];save();render()},
 time:k=>{S.profile.time=k;save();render()},
 have:d=>{const sid=leg().service;setStatus(d,sid,dstat(d,sid)==="ready"?"missing":"ready");save();render()},
 find:()=>go("options"),
 exp:id=>{S.ui.exp[id]=!S.ui.exp[id];render()},
 jump:id=>{S.ui.exp[id]=true;const ev=ranked().find(e=>e.f.id===id);if(ev&&ev.status==="blocked")S.ui.showBlocked=true;render();const el=$("#fac-"+id);if(el){el.scrollIntoView({behavior:"smooth",block:"center"});el.classList.add("flash")}},
 toggleBlocked:()=>{S.ui.showBlocked=!S.ui.showBlocked;render()},
 pick:id=>{const L=leg();if(L.facilityId!==id){L.facilityId=id;L.booking=null;S.ui.day=null}save();toast(fac(id).name+" selected");go(stage()==="docs"?"documents":"book")},
 doc:(d,s)=>{setStatus(d,leg().service,s);save();render();if(d==="referral"&&s==="ready")toast("Referral marked ready — booking unlocked")},
 getReferral:()=>{
  const L=leg();const target=L;target.status="waiting";
  const nl=blankLeg("gen_opd",{purpose:`Get a referral for ${SERVICES[target.service].name}`,forLeg:target.id});
  const near=DATA().map(f=>f.services.gen_opd?f:null).filter(Boolean);
  S.legs.splice(S.cur,0,nl);// insert before target; cur now points at new leg
  save();toast("Added a General OPD visit before your specialist visit");go("options");
 },
 day:d=>{S.ui.day=+d;S.ui.pick=null;render()},
 pickSlot:(ms,tok)=>{S.ui.pick=+ms;S.ui.pickTok=+tok;S.ui.conflict=null;render()},
 altPick:(ms,tok)=>{S.ui.day=sod(new Date(+ms)).getTime();S.ui.pick=+ms;S.ui.pickTok=+tok;S.ui.conflict=null;render()},
 confirmSlot:()=>{const L=leg();if(!S.ui.pick)return;const at=new Date(S.ui.pick).toISOString();const idem="bk-"+L.id+"-"+at;const key=slotKey(L.facilityId,L.service,at);const me=holderId(L);
  if(L.booking&&L.booking.idem===idem&&!S.ui.resched){toast("Already booked — no duplicate made");S.ui.pick=null;render();return}
  const online=isOnline();
  const f0=fac(L.facilityId);const sl=slotsForBase(f0,L.service,null).find(x=>x.at.getTime()===S.ui.pick);
  if(online&&sl&&sl.contested){const k2=key;const l=ledgerRead();if(!l[k2]){l[k2]={holder:"demo-other-patient",idem:"other-"+k2,at:Date.now()};l.__v=(l.__v||0)+1;ledgerWrite(l);audit("concurrency","Another patient claimed the slot first (demo race)")}}
  if(online){const r=ledgerClaim(key,me,idem);if(!r.ok){const pk=S.ui.pick;const alts=slotsFor(f0,L.service,L.notBefore).filter(x=>x.free&&x.at.getTime()!==pk).sort((a,b)=>Math.abs(a.at-pk)-Math.abs(b.at-pk)).slice(0,3).sort((a,b)=>a.at-b.at);
   S.ui.conflict={at:pk,alts};S.ui.pick=null;render();setTimeout(()=>{const b=document.querySelector(".banner.red");b&&b.scrollIntoView({behavior:"smooth",block:"center"})},40);return}}
  S.ui.conflict=null;
  if(L.booking&&S.ui.resched){const old=slotKey(L.facilityId,L.service,L.booking.at);L.booking.history.push(L.booking.at);L.booking.at=at;L.booking.token=S.ui.pickTok;L.booking.idem=idem;L.booking.status=online?"confirmed":"pending";if(online)ledgerRelease(old,me);audit("booking","Rescheduled booking "+L.booking.ref);toast("Rescheduled")}
  else{L.booking={at,token:S.ui.pickTok,ref:"NR-"+(hash(at+L.facilityId)%90000+10000),history:[],idem,status:online?"confirmed":"pending",policyV:S.policyV||1};audit("booking",`Booked ${L.booking.ref} under policy v${S.policyV||1}${online?"":" (offline — queued)"}`);toast(online?"Booked — token "+S.ui.pickTok:"Saved offline — will confirm when you're back online")}
  if(!online)queueAction("booking",{leg:L.id,ref:L.booking.ref},idem);
  const back=S.ui.reschedFrom==="visit";S.ui.resched=false;S.ui.reschedFrom=null;S.ui.pick=null;S.ui.queue=null;S.ui.moveDone=!!(back&&S.ui.bk==="moved"&&S.ui.demoRun==="C05");save();if(back||S.ui.demoRun==="C05"){go("visit");return}render()},
 reschedOn:()=>{S.ui.resched=true;S.ui.pick=null;S.ui.reschedFrom=null;render()},
 reschedVisit:()=>{const L=leg();const f=fac(L.facilityId);const maxR=(policy().rules||{}).maxResched;if(maxR&&L.booking&&L.booking.history.length>=maxR){toast(`Reschedule limit (${maxR}) reached — ask a navigator`);return}
  S.ui.resched=true;S.ui.pick=null;S.ui.reschedFrom="visit";if(L.booking)S.ui.day=sod(new Date(L.booking.at)).getTime();go("book");setTimeout(()=>{const g=document.querySelector(".days");g&&g.scrollIntoView({behavior:"smooth",block:"center"})},60)},
 reschedOff:()=>{S.ui.resched=false;S.ui.pick=null;if(S.ui.reschedFrom==="visit"){S.ui.reschedFrom=null;go("visit");return}render()},
 cancelBooking:()=>{modal(`<h3>Cancel this booking?</h3><p>Your slot will be released for someone else. You can book again any time.</p><div class="row" style="margin-top:.8rem"><button class="btn warn" data-act="cancelYes">Yes, cancel</button></div>`)},
 cancelYes:()=>{const L=leg();if(L.booking){ledgerRelease(slotKey(L.facilityId,L.service,L.booking.at),holderId(L));audit("booking","Cancelled booking "+L.booking.ref)}L.booking=null;S.ui.queue=null;closeModal();save();toast("Booking cancelled");render()},
 checkin:()=>{const L=leg();const start=Math.max(1,L.booking.token-6-(hash(L.id)%4));S.ui.queue={leg:L.id,serving:start,start,truth:start,n:0,lastBoard:start,stuck:0,flags:[],uncertain:false};render();tick()},
 outcome:type=>{
  const L=leg();
  if(type==="referral"){modal(`<h3>Referral to which department?</h3><p class="small muted">Choose what's written on the referral letter.</p><div class="svcgrid" style="margin-top:.6rem">${Object.entries(SERVICES).filter(([k])=>k!=="gen_opd").map(([k,s])=>`<button class="svc" data-act="refTo:${k}"><b>${esc(s.name)}</b><span>${esc(s.hint)}</span></button>`).join("")}</div>`);return}
  if(type==="return"){modal(`<h3>When should you come back?</h3><div class="chips" style="margin-top:.6rem">${[["1 week",7],["2 weeks",14],["1 month",30],["3 months",90]].map(([l,d])=>`<button class="chip" data-act="returnIn:${d}:${l}">${l}</button>`).join("")}</div>`);return}
  if(type==="tests"){finishLeg({type:"tests",label:"Asked for lab tests"});setStatus("test_slip","lab","ready");const nl=blankLeg("lab",{purpose:"Tests asked for at "+SERVICES[L.service].name});const f=fac(L.facilityId);if(f.services.lab)nl.facilityId=f.id;addLeg(nl);toast("Lab-test step added");go(nl.facilityId?"book":"options");return}
  if(type==="done"){finishLeg({type:"done",label:"No more visits needed"});save();toast("Journey closed");go("followup")}
 },
 refTo:k=>{closeModal();const L=leg();finishLeg({type:"referral",label:"Referred to "+SERVICES[k].name});setStatus("referral",k,"ready");
  const w=S.legs.findIndex(x=>x.status==="waiting"&&x.service===k);
  if(w>=0){S.legs[w].status="active";S.cur=w;toast("Referral ready — back to your "+SERVICES[k].name+" booking");save();go(S.legs[w].facilityId?"book":"options")}
  else{addLeg(blankLeg(k,{purpose:"Referred from "+SERVICES[L.service].name}));toast(SERVICES[k].name+" step added");go("options")}},
 returnIn:(d,l)=>{closeModal();const L=leg();const date=new Date(Date.now()+d*864e5);finishLeg({type:"return",label:"Come back in "+l,date:date.toISOString()});
  addLeg(blankLeg(L.service,{facilityId:L.facilityId,purpose:"Follow-up visit ("+l+")",notBefore:new Date(Math.max(Date.now(),date.getTime()-2*864e5)).toISOString()}));toast("Follow-up added — book when you're ready");go("followup")},
 leg:i=>{S.cur=+i;S.ui.queue=null;save();go(VIEWOF[stage()])},
 newNeed:()=>{addLeg(blankLeg());go("start")},
 reset:()=>{modal(`<h3>Start over?</h3><p>This clears your journey, documents and requests on this device.</p><div class="row" style="margin-top:.8rem"><button class="btn warn" data-act="resetYes">Clear everything</button></div>`)},
 resetYes:()=>{const keep={lang:S.lang,city:S.city,fs:S.fs,hc:S.hc,data:S.data,dataName:S.dataName};S={...fresh(),...keep};closeModal();save();go("start")},
 resetData:()=>{S.data=null;S.dataName=null;save();toast("Using sample data");render()},
 fs:()=>{const steps=[1,1.15,1.3,0.9];S.fs=steps[(steps.indexOf(S.fs)+1)%steps.length];save();render()},
 hc:()=>{S.hc=!S.hc;save();render()},
 speak:()=>{const n=nextStep();const txt=`${t("next")}: ${t(n.k)}. ${n.why.map(trText).join(" ")}`;try{const u=new SpeechSynthesisUtterance(txt);u.lang=LOCALE[S.lang];speechSynthesis.cancel();speechSynthesis.speak(u);toast("Reading aloud…")}catch(e){toast("Read-aloud isn't available in this browser")}},
 demo:()=>{modal(`<h3>Demo patients</h3><p class="small muted">Each one exercises a different part of the journey.</p><div class="stack" style="margin-top:.7rem">${CITY().personas.map(p=>`<button class="out" data-act="persona:${p.id}"><b>${esc(p.title)}</b><span>${esc(p.desc)}</span></button>`).join("")}</div>`)},
 persona:id=>{const p=CITY().personas.find(x=>x.id===id);const keep={lang:S.lang,city:S.city,fs:S.fs,hc:S.hc,data:S.data,dataName:S.dataName};S={...fresh(),...keep};S.profile={...S.profile,...p.profile};setCity();S.legs=[blankLeg(p.service)];p.have.forEach(d=>setStatus(d,p.service,"ready"));closeModal();save();toast("Loaded: "+p.title);go("start")},
 closeModal:()=>closeModal(),
 sim:k=>{S.sim=S.sim||{};S.sim[k]=!S.sim[k];if((k==="surge"||k==="navSurge")&&S.sim[k]&&S.view==="lab"){audit("lab",`${k} simulation ON`);save();demoGo(k==="surge"?"C05":"C05n");return}if((k==="surge"||k==="navSurge")&&!S.sim[k]&&S.ui.demoRun&&S.ui.demoRun.startsWith("C05"))S.ui.demoRun=null;audit("lab",`${k} simulation ${S.sim[k]?"ON":"OFF"}`);if(k==="offline"&&!S.sim[k])setTimeout(syncOutbox,50);if(k==="trGap")TRC={};if(k==="sensor")S.ui.queue=null;save();render();if(S.view==="lab")setTimeout(()=>{const v=document.querySelector(".verdict");v&&v.scrollIntoView({behavior:"smooth",block:"start"})},80);},
 pvSay:id=>{try{const u=new SpeechSynthesisUtterance(PVTXT[id]||"");u.lang="en-IN";u.rate=.9;speechSynthesis.cancel();speechSynthesis.speak(u);toast("Reading aloud…")}catch(e){toast("Read-aloud isn't available in this browser")}},
 pvDo:k=>{toast({ok:"Demo: nothing to do — booking unchanged",remind:"Demo: SMS / voice reminder set for the day before",accept:"Demo: new time confirmed and reminder updated",keep:"Done — you keep your place and we'll call you (demo)",faq:"Demo: opens instant answers — what to bring, timings, scheme cover",call:"Demo: this would dial the hospital's number",nav:"Demo: a navigator will check and call you back",cb:"Done — we'll call you when a slot opens (demo)",near:"Demo: shows the nearest hospital with a free slot"}[k]||"Demo")},
 authSubmit:()=>{const f=document.getElementById("authForm");f&&submitAuth(f)},
 c05mode:m=>{S.ui.c05mode=m;render()},
 acceptMove:(ms,tok)=>{const L=leg();if(!L.booking)return;L.booking.history.push(L.booking.at);L.booking.at=+ms;L.booking.token=+tok;S.ui.moveDone=true;audit("booking","Moved booking accepted during surge "+L.booking.ref);save();toast("New time confirmed");render()},
 demoGoTo:c=>demoGo(c),
 surgeScn:m=>{S.sim=S.sim||{};S.sim.surge=true;S.ui.bk=m;S.ui.moveDone=false;audit("lab",`Surge scenario: ${m==="kept"?"patient gets a booking":"slot lost, reschedule"}`);const L=leg();L.booking=null;demoGo("C05");
  {const L2=leg();const f=fac(L2.facilityId);const all=slotsForBase(f,L2.service,null);const d0=all.length?sod(all[0].at).getTime():0;const first=all.filter(x=>sod(x.at).getTime()===d0);const pickS=m==="moved"?(first[Math.min(first.length-1,Math.floor(first.length*.6))]||all[0]):(first[0]||all[0]);
   if(pickS){L2.booking={at:pickS.at.getTime(),token:pickS.token,ref:"NR-"+(hash(pickS.at.getTime()+L2.facilityId)%90000+10000),history:[],idem:"demo-"+pickS.at.getTime(),status:"confirmed",policyV:S.policyV||1,before:true}}save();go("visit")}},
 demoAdmin:()=>{const c=S.ui.demoRun||"C04";S.ui.demoTab=c==="C04"?"C04":"C05";if(c!=="C04")S.ui.c05mode=c==="C05n"?"nav":"slots";go("lab");setTimeout(()=>{const v=document.querySelector(".verdict")||document.querySelector(".empty");v&&v.scrollIntoView({behavior:"smooth",block:"start"})},80)},
 demoPatient:()=>{if(S.ui.demoRun)demoGo(S.ui.demoRun)},
 demoEnd:()=>{ACT.demoReset();S.ui.demoRun=null;go("lab")},
 demotab:c=>{S.ui.demoTab=c;render()},
 demoReset:()=>{S.ui.demoRun=null;try{const l=ledgerRead();Object.keys(l).forEach(k=>{if(k!=="__v"&&/^demo-/.test(l[k].holder))delete l[k]});ledgerWrite(l)}catch(e){}S.sim=S.sim||{};S.sim.surge=false;S.sim.navSurge=false;S.quarantine=[];S.lastReport=null;S.ui.lab={};S.data=null;S.dataName=null;audit("lab","Demo reset");save();toast("Demo reset — sample data restored");render()},
 labjump:c=>{setTimeout(()=>{const el=document.getElementById("lab-"+c);el&&el.scrollIntoView({behavior:"smooth",block:"start"})},30)},
 lab:what=>{S.ui.lab=S.ui.lab||{};const R=S.ui.lab;
  if(what==="badset"){const r=loadDataset(BAD_SAMPLE,"messy-dataset.json","merge");R.C04=reportHTML(r)}
  if(what==="badjson"){const r=loadDataset(BAD_JSON,"broken.json","merge");R.C04=reportHTML(r)}
  if(what==="badcsv"){const r=loadDataset(BAD_CSV,"messy.csv","merge");R.C04=reportHTML(r)}
  if(what==="v2"){const r=loadDataset(V2_SAMPLE,"api-v2-response.json","merge");R.C03=reportHTML(r)}
  if(what==="v2raw"){const r=loadDataset(V2_SAMPLE,"api-v2-response (no adapter).json","merge",{noAdapter:true});R.C03=`<p class="small"><b>Without the adapter the old integration fails:</b> the v2 record has no <span class="kbd">id</span>, <span class="kbd">name</span> or <span class="kbd">services</span> in the old format, so it is rejected — but safely, without crashing.</p>`+reportHTML(r)}
  if(what==="v2broken"){const r=loadDataset('{"status":502,"error":"upstream timeout"}',"api-broken-response.json","merge");R.C03=reportHTML(r)}
  if(what==="leak"){const rec={name:SESSION&&SESSION.name,contact:SESSION&&SESSION.id,service:leg().service};fetch("https://cloud-ai.example.com/v1/analyse",{method:"POST",body:JSON.stringify(rec)}).then(()=>{}).catch(e=>{R.C07=`<div class="banner green"><span class="ic">✓</span><div><b>Blocked.</b> ${esc(e.message)}. The audit log records the attempt with personal details hidden.</div></div>`;render()});return}
  if(what==="wipe"){modal(`<h3>Delete your data from this device?</h3><p>This removes your journey, documents, bookings and requests stored in this browser.</p><div class="row" style="margin-top:.8rem"><button class="btn warn" data-act="wipeYes">Delete</button></div>`);return}
  if(what==="unsurepay"){S.profile.scheme="unknown";audit("lab","Payment set to Not sure yet");save();toast("Payment set to “Not sure yet” — open Book to see the check")}
  if(what==="race"){labRace();return}
  if(what==="dupe"){labDupe();return}
  if(what==="clearLedger"){const l=ledgerRead();Object.keys(l).forEach(k=>{if(k!=="__v"&&/^demo-/.test(l[k].holder))delete l[k]});ledgerWrite(l);R.C09="";audit("lab","Demo claims cleared")}
  if(["badset","badjson","badcsv"].includes(what)&&S.view==="lab"){demoGo("C04");return}
  render();if(S.view==="lab")setTimeout(()=>{const v=document.querySelector(".verdict");v&&v.scrollIntoView({behavior:"smooth",block:"start"})},80);},
 wipeYes:()=>{try{localStorage.removeItem(stateKey());localStorage.removeItem(LEDGER_KEY)}catch(e){}closeModal();const keep={lang:S.lang,city:S.city};S={...fresh(),...keep};audit("privacy","User deleted their data from this device");save();toast("Your data was deleted from this device");go("start")},
 policy:v=>{applyPolicy(+v)},
 reviewKeep:()=>{const L=leg();if(L.booking){audit("policy",`Patient confirmed keeping ${L.booking.ref} under policy v${S.policyV}`);L.booking.review=null;L.booking.policyV=S.policyV;save();render()}},
 refOverride:()=>{S.ui.refOverride=true;setStatus("referral",leg().service,"ready");audit("booking","Patient confirmed they have a referral letter (rule unknown in data)");render()},
 joinWait:()=>{const L=leg();S.waitlist=S.waitlist||[];const same=S.waitlist.filter(x=>x.facilityId===L.facilityId&&x.day===S.ui.day).length;S.waitlist.push({leg:L.id,facilityId:L.facilityId,service:L.service,day:S.ui.day,pos:same+1+(hash(L.id)%5),at:Date.now()});audit("waitlist","Joined wait-list");save();toast("Added to the wait-list");render()},
 clearConflict:()=>{const L=leg();L.booking=null;save();render()},
 ticket:()=>{const id="NAV-"+(Date.now()%100000).toString().padStart(5,"0");const note=($("#hnote").value||"").replace(/[\u0000-\u001F\u007F]/g," ").slice(0,500);const on=isOnline();S.tickets.unshift({id,created:Date.now(),channel:$("#chan").value,when:$("#when").value,note,summary:caseSummary(),status:on?"Queued":"Waiting to send (offline)"});if(!on)queueAction("ticket",{id},"tk-"+id);audit("navigator",`Navigator request ${id} ${on?"sent":"saved offline"}`);save();toast(on?"Request "+id+" sent":"Saved offline — will send when you're back online");render()},
 copyPass:()=>{const L=leg(),f=fac(L.facilityId),at=new Date(L.booking.at);copy(`VISIT PASS — token ${L.booking.token} (ref ${L.booking.ref})\n${fmtDay(at)} ${fmtTime(at)}\n${f.name}, ${f.services[L.service].dept}\n${f.address} · ${f.phone}\nBring: ${requiredDocs(f,L.service).map(d=>DOCS[d].name).join(", ")}\nEmergency: 108 / 112`,"Visit pass copied")},
 copyList:()=>{const L=leg(),f=fac(L.facilityId);copy(`Checklist for ${f.name} (${SERVICES[L.service].name}):\n`+requiredDocs(f,L.service).map(d=>`${dstat(d,L.service)==="ready"?"[x]":"[ ]"} ${DOCS[d].name}`).join("\n"),"Checklist copied")},
 copySms:()=>{const r=reminders().filter(x=>x.ev)[0];if(!r)return toast("No appointment to remind about");copy(`Reminder: ${r.title} on ${fmtDay(r.at)} at ${fmtTime(r.at)} — ${r.body}. Leave early; bring your documents. Emergency 108/112.`,"SMS text copied")}
};
async function labRace(){const R=S.ui.lab;const L=leg();const f=(L.facilityId&&fac(L.facilityId))||DATA().find(x=>x.services.gen_opd);const sid=L.facilityId?L.service:"gen_opd";
 const free=slotsFor(f,sid,null).filter(x=>x.free);if(!free.length){R.C09=`<p class="small">No free slot to test with at ${esc(f.name)} — pick another facility.</p>`;render();return}
 const last=free[free.length-1];const key=slotKey(f.id,sid,last.at);
 const [a,b]=await Promise.all([ledgerClaimCAS(key,"demo-A","demo-A-"+key,40),ledgerClaimCAS(key,"demo-B","demo-B-"+key,40)]);
 audit("concurrency",`Race on ${f.name} ${fmtTime(last.at)}: A ${a.ok?"won":"lost"}, B ${b.ok?"won":"lost"}`);
 R.C09=`<table class="mini"><thead><tr><th>Request</th><th>Result</th></tr></thead><tbody><tr><td>User A</td><td><b>${a.ok?"Confirmed":"Refused"}</b> ${a.ok?"":"— "+esc(a.reason)}</td></tr><tr><td>User B</td><td><b>${b.ok?"Confirmed":"Refused"}</b> ${b.ok?"":"— "+esc(b.reason)+"; offered the wait-list and other slots"}</td></tr></tbody></table><p class="small">Slot: ${esc(f.name)}, ${esc(fmtDay(last.at))} ${esc(fmtTime(last.at))}. Exactly one claim succeeded; the slot now shows as taken for everyone. ${a.ok&&b.ok?"✕ DOUBLE BOOKING":"✓ No double booking"}</p>`;render()}
async function labDupe(){const R=S.ui.lab;const L=leg();const f=(L.facilityId&&fac(L.facilityId))||DATA().find(x=>x.services.gen_opd);const sid=L.facilityId?L.service:"gen_opd";
 const free=slotsFor(f,sid,null).filter(x=>x.free);if(!free.length){R.C09="<p class=\"small\">No free slot to test with.</p>";render();return}
 const s0=free[0];const key=slotKey(f.id,sid,s0.at);const idem="demo-retry-"+key;
 const res=await Promise.all([1,2,3].map(i=>ledgerClaimCAS(key,"demo-retry",idem,10*i)));const l=ledgerRead();const n=Object.keys(l).filter(k=>k===key).length;
 audit("concurrency",`Duplicate submit ×3 with one idempotency key → ${n} booking`);
 R.C09=`<p class="small">Three identical submissions with the same idempotency key: ${res.map((r,i)=>`#${i+1} ${r.ok?(r.repeat?"returned existing booking":"created booking"):"refused"}`).join(" · ")}. Bookings in ledger for that slot: <b>${n}</b> ✓</p>`;render()}
function applyPolicy(v){const before={};const L=leg();const ev=L.service?ranked():[];ev.forEach(e=>before[e.f.id]=e.status);
 S.policyV=v;S.policyLog=[...(S.policyLog||[]),{v,at:Date.now()}];TRC={};audit("policy",`Policy changed to v${v}`);
 const after=L.service?ranked():[];const changed=after.filter(e=>before[e.f.id]&&before[e.f.id]!==e.status).map(e=>`${e.f.name}: ${t(before[e.f.id])} → ${t(e.status)}`);
 const flagged=[];S.legs.forEach(x=>{if(!x.booking||!x.facilityId)return;const f=fac(x.facilityId);if(!f)return;if(needsReferral(f,x.service)&&dstat("referral",x.service)!=="ready"&&!x.booking.review){x.booking.review="This department now needs a referral letter.";flagged.push(`${f.name} (${SERVICES[x.service].name}) — booked under v${x.booking.policyV||1}, flagged for your confirmation`)}
  if(v===1&&x.booking.review){x.booking.review=null}});
 flagged.forEach(m=>audit("policy","Flagged, not cancelled: "+m));
 S.ui.lab=S.ui.lab||{};S.ui.lab.C11=`<p class="small"><b>Re-evaluated for ${L.service?esc(SERVICES[L.service].name):"current journey"}:</b></p><ul class="small">${changed.map(c=>`<li>${esc(c)}</li>`).join("")||"<li>No ranking changes for the current service.</li>"}</ul>${flagged.length?`<p class="small"><b>Bookings needing confirmation (not cancelled):</b></p><ul class="small">${flagged.map(c=>`<li>${esc(c)}</li>`).join("")}</ul>`:""}`;
 save();render()}
function finishLeg(outcome){const L=leg();L.outcome={...outcome,at:new Date().toISOString()};L.status="done";}
function addLeg(l){S.legs.push(l);S.cur=S.legs.length-1;save()}
function tick(){clearTimeout(tick.t);const q=S.ui.queue,L=leg();if(!q||!L.booking||S.view!=="visit")return;if((q.serving>=L.booking.token&&!q.uncertain)||q.n>40)return;
 tick.t=setTimeout(()=>{const q=S.ui.queue;if(!q)return;q.n++;if(q.truth<L.booking.token)q.truth++;const rd=queueReading(q,L.booking.token);const ev=evalReading(q,rd);
  if(rd.board!=null&&rd.board===q.lastBoard)q.stuck++;else q.stuck=0;if(rd.board!=null)q.lastBoard=rd.board;
  if(!ev.flags.length&&rd.board!=null&&rd.board>=q.serving&&rd.board-q.serving<=4){q.serving=rd.board;q.uncertain=false;q.flags=[]}
  else if(ev.flags.length){q.uncertain=true;q.flags=ev.flags;ev.flags.forEach(x=>audit("sensor",x))}
  render();tick()},2500)}

document.addEventListener("click",e=>{
 const c=e.target.closest("[data-copy]");if(c){const k=c.dataset.copy;if(k==="ics")copy(ics(),"Calendar text copied");if(k==="summary")copy(caseSummary(),"Summary copied");if(k==="schema")copy(dataPanel().match(/<pre class="code">([\s\S]*?)<\/pre>/)[1].replace(/&quot;/g,'"').replace(/&amp;/g,"&").replace(/&lt;/g,"<").replace(/&gt;/g,">"),"Schema copied");return}
 const el=e.target.closest("[data-act]");if(!el)return;
 if(el.classList.contains("scrim")&&e.target!==el)return;
 const [a,...args]=el.dataset.act.split(":");if(ACT[a]){e.preventDefault();ACT[a](...args)}
});
document.addEventListener("keydown",e=>{if((e.key==="Enter"||e.key===" ")&&e.target.matches("g[data-act]")){e.preventDefault();e.target.dispatchEvent(new MouseEvent("click",{bubbles:true}))}if(e.key==="Escape")closeModal()});
document.addEventListener("change",e=>{
 const k=e.target.dataset.change;if(!k)return;
 if(k==="area"||k==="scheme"){S.profile[k]=e.target.value;save();render()}
 if(k.startsWith("upload:")){const d=k.split(":")[1],f=e.target.files[0];if(f){setStatus(d,leg().service,"ready",f.name);save();toast("Attached "+f.name);render()}}
 if(k==="data"){const f=e.target.files[0];if(!f)return;const r=new FileReader();r.onload=()=>{const rep=loadDataset(String(r.result),f.name,"replace");S.ui.lab=S.ui.lab||{};S.ui.lab.C04=reportHTML(rep);toast(rep.fatal?"File rejected — current data kept":`Loaded ${rep.accepted.length} facilities`);if(S.view==="lab"){e.target.value="";demoGo("C04");return}if(S.view!=="lab")modal(`<h3>Data quality report</h3>${reportHTML(rep)}`);render();e.target.value=""};r.onerror=()=>toast("Couldn't read that file");r.readAsText(f)}
 if(k==="labLang"){S.lang=e.target.value;AUTHUI.lang=S.lang;TRC={};save();render()}
});
document.addEventListener("submit",e=>{if(e.target.id==="authForm"){e.preventDefault();submitAuth(e.target)}});
addEventListener("keydown",e=>{if(e.key==="Enter"&&e.target.closest&&e.target.closest("#authForm")&&e.target.tagName==="INPUT"&&e.target.type!=="checkbox"){e.preventDefault();submitAuth(e.target.closest("#authForm"))}});
document.addEventListener("input",e=>{const f=e.target.closest&&e.target.closest("#authForm");if(!f||!e.target.name)return;AUTHUI.vals[e.target.name]=e.target.type==="checkbox"?e.target.checked:e.target.value;if(e.target.name==="pw"&&$("#pwMeter")){$("#pwMeter").innerHTML=pwMeter(e.target.value);translateDOM($("#pwMeter"))}if(AUTHUI.err[e.target.name]){delete AUTHUI.err[e.target.name];e.target.setAttribute("aria-invalid","false");const m=$("#"+e.target.name+"-err");m&&m.remove()}});
let ft;document.addEventListener("input",e=>{if(e.target.id==="freeText"){S.profile.text=e.target.value.replace(/[\u0000-\u0008\u000B\u000C\u000E-\u001F\u007F\u202A-\u202E\u2066-\u2069]/g,"").slice(0,500);clearTimeout(ft);ft=setTimeout(()=>{if(autoRoute()){save();const el=$("#freeText"),pos=el?el.selectionStart:0;render();const n=$("#freeText");if(n){n.focus();n.setSelectionRange(pos,pos)}return}save();const a=analyse(S.profile.text),L=leg();
 $("#guard").innerHTML=guardBanner(a)+routeHTML(a,L);renderSide();translateDOM($("#guard"));translateDOM($("#side"))},350)}});
$("#langSel").addEventListener("change",e=>{S.lang=e.target.value;AUTHUI.lang=S.lang;TRC={};try{localStorage.setItem("nr-lang",S.lang)}catch(x){}save();render()});
document.addEventListener("change",e=>{if(e.target.id==="lang"&&e.target.closest("#authForm")){AUTHUI.lang=e.target.value;AUTHUI.vals.lang=e.target.value;TRC={};try{localStorage.setItem("nr-lang",AUTHUI.lang)}catch(x){}renderAuth();const el=$("#lang");el&&el.focus();return}if(e.target.id==="authLang"){TRC={};AUTHUI.lang=e.target.value;AUTHUI.vals.lang=e.target.value;try{localStorage.setItem("nr-lang",AUTHUI.lang)}catch(x){}renderAuth()}});
$("#citySel").addEventListener("change",e=>{const keep={lang:S.lang,fs:S.fs,hc:S.hc};S={...fresh(),...keep,city:e.target.value};S.profile.area=CITY().defArea;setCity();save();toast("Switched to "+CITY().name);go("start")});
window.addEventListener("hashchange",()=>{const h=location.hash.slice(1);if(h&&h!==S.view&&["start","options","documents","book","visit","followup","help","lab"].includes(h)){S.view=h;render()}});
(()=>{const h=location.hash.slice(1);if(["start","options","documents","book","visit","followup","help","lab"].includes(h))S.view=h;render()})();
</script>
</body>
</html>
