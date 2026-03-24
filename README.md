<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="theme-color" content="#020c04">
<title>FleetGuard Pro — Women's Choice Quality Waters</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
html{height:100%;font-size:18px}
body{font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;background:var(--bg);color:var(--fg);height:100%;overflow:hidden;display:flex;flex-direction:column;-webkit-font-smoothing:antialiased}

:root{
  --acc:#4AFF1F;--acc2:#2bcc00;
  --acc-glow:rgba(74,255,31,.32);--acc-faint:rgba(74,255,31,.08);--acc-border:rgba(74,255,31,.22);
  --bg:#020c04;--s1:#071209;--s2:#0c1a0e;--s3:#112014;--s4:#172819;
  --b1:#1f361f;--b2:#264226;
  --fg:#edfae8;--fg2:#8eb88a;--fg3:#4a7048;
  --red:#FF3355;--red-faint:rgba(255,51,85,.09);--red-border:rgba(255,51,85,.38);--red-g:rgba(255,51,85,.28);
  --yel:#FFD600;
  --wa:#25D366;--wa2:#128C7E;
  --nav-h:66px;
  --safe-b:env(safe-area-inset-bottom,0px);
  --safe-t:env(safe-area-inset-top,0px);
  --r:10px;--rl:16px;--rxl:22px;
}

/* ── TOP BAR ── */
#topbar{flex-shrink:0;display:flex;align-items:center;justify-content:space-between;padding:11px clamp(14px,4vw,22px);padding-top:calc(11px + var(--safe-t));background:var(--s1);border-bottom:2px solid var(--b1);position:relative;z-index:200}
#topbar::after{content:'';position:absolute;bottom:-2px;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,var(--acc),transparent)}
.tb-logo{font-weight:900;font-size:clamp(17px,4.5vw,21px);letter-spacing:2px;text-transform:uppercase;color:var(--acc);text-shadow:0 0 18px var(--acc-glow);line-height:1}
.tb-logo em{color:var(--fg);font-style:normal;font-weight:300}
.tb-client{font-size:clamp(9px,2vw,10px);font-weight:700;letter-spacing:1.5px;text-transform:uppercase;color:var(--fg3);margin-top:2px}
.tb-dot{width:9px;height:9px;border-radius:50%;background:var(--acc);box-shadow:0 0 10px var(--acc-glow);animation:pulse 2s ease-in-out infinite;flex-shrink:0}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.55;transform:scale(.82)}}

/* ── PAGES ── */
#pages{flex:1;overflow:hidden;position:relative}
.page{position:absolute;inset:0;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch;padding:clamp(14px,3.8vw,24px);padding-bottom:calc(var(--nav-h) + var(--safe-b) + 18px);opacity:0;transform:translateY(12px);pointer-events:none;transition:opacity .25s,transform .25s;scrollbar-width:thin;scrollbar-color:var(--b2) transparent}
.page::-webkit-scrollbar{width:3px}
.page::-webkit-scrollbar-thumb{background:var(--b2);border-radius:2px}
.page.active{opacity:1;transform:none;pointer-events:all}

/* ── NAV ── */
#bnav{flex-shrink:0;position:fixed;bottom:0;left:0;right:0;height:calc(var(--nav-h) + var(--safe-b));padding-bottom:var(--safe-b);background:var(--s1);border-top:1px solid var(--b1);display:flex;z-index:300}
.nb{flex:1;background:none;border:none;cursor:pointer;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:4px;color:var(--fg3);font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;font-size:clamp(8px,1.9vw,10px);font-weight:800;letter-spacing:.7px;text-transform:uppercase;transition:color .2s;position:relative;padding:0 2px}
.nb svg{width:clamp(19px,5vw,23px);height:clamp(19px,5vw,23px);transition:transform .28s cubic-bezier(.34,1.56,.64,1),filter .2s}
.nb.active{color:var(--acc)}
.nb.active svg{transform:scale(1.22) translateY(-1px);filter:drop-shadow(0 0 5px var(--acc-glow))}
.nb.active::before{content:'';position:absolute;top:0;left:50%;transform:translateX(-50%);width:36px;height:3px;background:var(--acc);border-radius:0 0 3px 3px;box-shadow:0 0 8px var(--acc-glow)}

/* ── TYPOGRAPHY ── */
.pg-title{font-size:clamp(22px,5.5vw,30px);font-weight:900;letter-spacing:-.5px;line-height:1.1}
.pg-sub{font-size:clamp(13px,3vw,15px);color:var(--fg2);margin-top:4px;margin-bottom:clamp(16px,4vw,24px);line-height:1.5}
.sec-lbl{font-size:11px;font-weight:900;letter-spacing:2.5px;text-transform:uppercase;color:var(--acc);margin-bottom:12px;display:flex;align-items:center;gap:8px}
.sec-lbl::after{content:'';flex:1;height:1px;background:linear-gradient(90deg,var(--acc-border),transparent)}

/* ── CARDS ── */
.card{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(14px,3.8vw,20px);margin-bottom:clamp(12px,3vw,16px);position:relative;overflow:hidden}
.card::before{content:'';position:absolute;top:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent 5%,var(--acc-border) 50%,transparent 95%)}
.ch{font-size:clamp(11px,2.5vw,12px);font-weight:900;letter-spacing:2px;text-transform:uppercase;color:var(--acc);margin-bottom:15px;display:flex;align-items:center;gap:8px}
.ch svg{width:14px;height:14px;flex-shrink:0}

/* ══════════════════════════════════
   FORM FIELDS — live-miss highlight
══════════════════════════════════ */
.field{margin-bottom:14px;position:relative;transition:all .2s}
.field:last-child{margin-bottom:0}
.field>label{display:block;font-size:clamp(11px,2.4vw,13px);font-weight:800;letter-spacing:1.5px;text-transform:uppercase;color:var(--fg2);margin-bottom:7px;transition:color .18s}
.req{color:var(--acc);margin-left:2px;font-weight:900}
.field input,.field select,.field textarea{width:100%;background:var(--s3);border:2px solid var(--b2);border-radius:var(--r);color:var(--fg);font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;font-size:clamp(15px,3.5vw,17px);padding:clamp(11px,2.8vw,14px) clamp(12px,3vw,16px);outline:none;transition:border-color .18s,box-shadow .18s,background .18s;-webkit-appearance:none;appearance:none}
.field select{background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8'%3E%3Cpath d='M.5.5l5.5 6 5.5-6' stroke='%234a7048' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");background-repeat:no-repeat;background-position:right 14px center;padding-right:40px;cursor:pointer}
.field textarea{resize:vertical;min-height:66px;line-height:1.6}

/* FOCUS */
.field input:focus,.field select:focus,.field textarea:focus{border-color:var(--acc);box-shadow:0 0 0 3px var(--acc-faint);background:var(--s4)}

/* MISSED — applied live on blur / validate */
.field.err input,.field.err select,.field.err textarea{border-color:var(--red)!important;box-shadow:0 0 0 3px var(--red-faint)!important;background:rgba(255,51,85,.04)!important;animation:fldShake .32s ease}
.field.err label{color:var(--red)!important}
.field-err-msg{display:none;font-size:11px;font-weight:800;color:var(--red);letter-spacing:.8px;margin-top:5px;text-transform:uppercase}
.field.err .field-err-msg{display:block}
@keyframes fldShake{0%,100%{transform:translateX(0)}25%{transform:translateX(-5px)}75%{transform:translateX(5px)}}

.g2{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.field-meta{display:flex;justify-content:flex-end;margin-top:4px}
.char-c{font-family:'Courier New',monospace;font-size:11px;color:var(--fg3)}

/* ── VEHICLE PREVIEW ── */
.veh-prev{background:var(--s3);border:1px solid var(--acc-border);border-radius:var(--r);padding:13px 16px;margin-top:4px;margin-bottom:14px;display:none;grid-template-columns:1fr 1fr;gap:8px 18px;animation:fadeUp .22s ease}
@keyframes fadeUp{from{opacity:0;transform:translateY(-4px)}to{opacity:1;transform:none}}
.vp-k{font-size:10px;font-weight:800;letter-spacing:1.5px;text-transform:uppercase;color:var(--fg3);margin-bottom:2px}
.vp-v{font-size:clamp(12px,2.8vw,14px);font-weight:700;color:var(--acc);font-family:'Courier New',monospace}

/* ── STATS ── */
.stat-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:clamp(8px,2vw,12px);margin-bottom:clamp(14px,3.5vw,22px)}
@media(min-width:480px){.stat-grid{grid-template-columns:repeat(4,1fr)}}
.stat{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(14px,3.5vw,20px) 10px;text-align:center}
.stat-n{font-size:clamp(30px,8vw,46px);font-weight:900;letter-spacing:-1px;line-height:1;color:var(--acc);text-shadow:0 0 24px var(--acc-glow)}
.stat-l{font-size:clamp(10px,2.1vw,11px);font-weight:800;letter-spacing:1.5px;text-transform:uppercase;color:var(--fg2);margin-top:5px}

/* ── QUICK ACTIONS ── */
.qa{display:flex;align-items:center;gap:clamp(12px,3vw,17px);background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(13px,3.3vw,17px);cursor:pointer;transition:border-color .2s,box-shadow .2s;margin-bottom:11px}
.qa:hover{border-color:var(--acc);box-shadow:0 0 16px var(--acc-faint)}
.qa-ico{width:clamp(40px,9.5vw,48px);height:clamp(40px,9.5vw,48px);background:var(--acc-faint);border:1px solid var(--acc-border);border-radius:11px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.qa-ico svg{width:clamp(19px,4.7vw,23px);height:clamp(19px,4.7vw,23px);color:var(--acc)}
.qa-text{flex:1;min-width:0}
.qa-t{font-size:clamp(14px,3.3vw,16px);font-weight:800}
.qa-s{font-size:clamp(12px,2.7vw,14px);color:var(--fg2);margin-top:3px}
.qa-arr svg{width:17px;height:17px;color:var(--fg3)}

/* ── REPORT BADGE ── */
.rpt-badge{display:inline-flex;align-items:center;gap:8px;background:var(--acc-faint);border:1px solid var(--acc-border);border-radius:7px;padding:7px 13px;font-family:'Courier New',monospace;font-size:clamp(11px,2.5vw,13px);color:var(--acc);letter-spacing:1px;margin-bottom:clamp(14px,3.5vw,18px)}
.rpt-badge svg{width:12px;height:12px;flex-shrink:0}

/* ── MISSED SUMMARY BANNER ── */
.miss-banner{display:none;background:var(--red-faint);border:2px solid var(--red-border);border-radius:var(--rl);padding:clamp(13px,3.3vw,17px);margin-bottom:clamp(12px,3vw,16px)}
.miss-banner.show{display:block;animation:fldShake .36s ease}
.miss-ttl{font-size:clamp(13px,3vw,15px);font-weight:900;color:var(--red);margin-bottom:10px;display:flex;align-items:center;gap:7px}
.miss-list{display:flex;flex-direction:column;gap:6px;list-style:none}
.miss-list li{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);padding:6px 11px;background:rgba(255,51,85,.06);border-radius:7px;border-left:3px solid var(--red)}

/* ── PROGRESS ── */
.prog-wrap{background:var(--s3);border-radius:8px;height:9px;overflow:hidden;margin-bottom:8px}
.prog-bar{height:100%;background:linear-gradient(90deg,var(--acc2),var(--acc));border-radius:8px;transition:width .35s ease;box-shadow:0 0 10px var(--acc-glow)}
.prog-lbl{font-family:'Courier New',monospace;font-size:clamp(12px,2.7vw,13px);color:var(--fg2);text-align:right;margin-bottom:14px}

/* ── INSPECT SECTIONS ── */
.isec{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);margin-bottom:clamp(9px,2.3vw,13px);overflow:hidden;transition:border-color .2s,box-shadow .2s}
.isec.iscrit{border-color:rgba(255,51,85,.4)}
.isec.isdone{border-color:var(--acc-border)}
.isec.sec-missed{border-color:var(--red)!important;box-shadow:0 0 0 2px rgba(255,51,85,.15)!important}
.isec-hdr{display:flex;align-items:center;gap:11px;padding:clamp(12px,3vw,16px);cursor:pointer;user-select:none;transition:background .15s}
.isec-hdr:hover{background:rgba(74,255,31,.025)}
.isec-ico{width:clamp(35px,8.5vw,43px);height:clamp(35px,8.5vw,43px);background:var(--acc-faint);border:1px solid var(--acc-border);border-radius:9px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.isec-ico svg{width:clamp(17px,4.2vw,21px);height:clamp(17px,4.2vw,21px);color:var(--acc)}
.isec-title{flex:1;font-size:clamp(13px,3.1vw,15px);font-weight:900;letter-spacing:1px;text-transform:uppercase}
.isec-badge{font-size:11px;font-weight:800;padding:3px 10px;border-radius:20px;background:var(--s3);color:var(--fg2);border:1px solid var(--b2);white-space:nowrap}
.isec-chev{width:16px;height:16px;color:var(--fg3);transition:transform .25s;flex-shrink:0}
.isec.open .isec-chev{transform:rotate(180deg)}
.isec-body{max-height:0;overflow:hidden;transition:max-height .38s cubic-bezier(.4,0,.2,1);border-top:0 solid var(--b1)}
.isec.open .isec-body{max-height:9999px;border-top-width:1px}
.isec-inner{padding:clamp(11px,2.8vw,16px)}

/* ── INSPECT ITEM ── */
.iitem{background:var(--s3);border:2px solid var(--b2);border-radius:var(--r);padding:clamp(11px,2.8vw,15px);margin-bottom:11px;border-left:4px solid transparent;transition:border-color .2s,box-shadow .2s}
.iitem:last-child{margin-bottom:0}
.iitem.st-good{border-left-color:var(--acc)}
.iitem.st-minor{border-left-color:var(--yel)}
.iitem.st-critical{border-left-color:var(--red)}
.iitem.item-missed{border-color:var(--red)!important;box-shadow:0 0 0 2px var(--red-faint)!important;animation:fldShake .32s ease}
.iitem-name{font-size:clamp(14px,3.2vw,16px);font-weight:800;margin-bottom:11px;line-height:1.3}
.iitem.item-missed .iitem-name{color:var(--red)}
.srow{display:flex;gap:7px;margin-bottom:11px}
.sbtn{flex:1;padding:clamp(8px,2vw,11px) 3px;border-radius:8px;border:2px solid var(--b2);background:var(--s2);color:var(--fg2);font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;font-size:clamp(11px,2.5vw,13px);font-weight:900;letter-spacing:.5px;text-transform:uppercase;cursor:pointer;transition:all .16s;text-align:center}
.sbtn[data-v="good"].on{background:rgba(74,255,31,.14);border-color:var(--acc);color:var(--acc);box-shadow:0 0 8px rgba(74,255,31,.18)}
.sbtn[data-v="minor"].on{background:rgba(255,214,0,.14);border-color:var(--yel);color:var(--yel)}
.sbtn[data-v="critical"].on{background:rgba(255,51,85,.14);border-color:var(--red);color:var(--red);box-shadow:0 0 8px var(--red-g)}

/* ── IMAGE UPLOAD ── */
.img-drop{border:2px dashed var(--b2);border-radius:var(--r);padding:clamp(9px,2.3vw,13px);text-align:center;position:relative;cursor:pointer;transition:border-color .2s,background .18s;margin-bottom:9px}
.img-drop:hover{border-color:var(--acc);background:var(--acc-faint)}
.img-drop input[type="file"]{position:absolute;inset:0;opacity:0;cursor:pointer;width:100%;height:100%;font-size:0}
.img-drop-l{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);pointer-events:none;display:flex;align-items:center;justify-content:center;gap:7px}
.img-drop-l svg{width:15px;height:15px;flex-shrink:0}
.img-thumbs{display:grid;grid-template-columns:repeat(4,1fr);gap:7px;margin-top:9px}
.img-tw{position:relative;aspect-ratio:1;border-radius:7px;overflow:hidden;border:1.5px solid var(--b2)}
.img-tw img{width:100%;height:100%;object-fit:cover;display:block}
.img-del{position:absolute;top:3px;right:3px;width:20px;height:20px;background:rgba(255,51,85,.9);border:none;border-radius:50%;cursor:pointer;color:#fff;font-size:11px;font-weight:900;display:flex;align-items:center;justify-content:center;padding:0}

/* ── RESULT BANNER ── */
.res-banner{border-radius:var(--rl);padding:clamp(15px,3.8vw,20px);text-align:center;margin-bottom:clamp(13px,3.2vw,18px);display:none}
.res-banner.complete{background:var(--acc-faint);border:2px solid var(--acc);box-shadow:0 0 26px var(--acc-glow)}
.res-banner.critical{background:rgba(255,51,85,.07);border:2px solid var(--red);box-shadow:0 0 26px var(--red-g);animation:fldShake .4s ease}
.res-ico{font-size:clamp(28px,7vw,40px);margin-bottom:8px}
.res-title{font-size:clamp(16px,4vw,20px);font-weight:900;letter-spacing:2px;text-transform:uppercase}
.res-sub{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);margin-top:5px;line-height:1.5}
.res-banner.complete .res-title{color:var(--acc)}
.res-banner.critical .res-title{color:var(--red)}

/* ═══════════════════════════════════════
   ELECTRONIC CERTIFICATION (no signature)
═══════════════════════════════════════ */
.ecert{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(15px,3.8vw,22px);margin-bottom:clamp(12px,3vw,16px);position:relative;overflow:hidden}
.ecert::before{content:'';position:absolute;top:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent 5%,var(--acc-border) 50%,transparent 95%)}
.ecert-body{font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.65;margin-bottom:16px}
.ecert-body strong{color:var(--fg)}

/* Custom big checkbox row */
.cert-row{display:flex;align-items:flex-start;gap:14px;cursor:pointer;padding:13px 14px;background:var(--s3);border:2px solid var(--b2);border-radius:var(--r);transition:border-color .18s,background .18s;user-select:none}
.cert-row:hover{border-color:var(--acc-border);background:var(--s4)}
.cert-row.cert-err{border-color:var(--red)!important;background:var(--red-faint)!important;animation:fldShake .32s ease}
.cert-row.cert-done{border-color:var(--acc)!important;background:var(--acc-faint)!important;box-shadow:0 0 14px var(--acc-glow)}
.cert-row input[type=checkbox]{display:none}
.cert-box{width:30px;height:30px;border:2px solid var(--b2);border-radius:7px;background:var(--s2);display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:1px;transition:all .18s}
.cert-box svg{width:17px;height:17px;opacity:0;transition:opacity .15s}
.cert-row.cert-done .cert-box{background:var(--acc);border-color:var(--acc);box-shadow:0 0 10px var(--acc-glow)}
.cert-row.cert-done .cert-box svg{opacity:1;stroke:#000}
.cert-text{flex:1;font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.6}
.cert-text strong{color:var(--fg);font-weight:800}
.cert-text .cert-name{color:var(--acc);font-weight:900;font-family:'Courier New',monospace}
.cert-info{display:none;margin-top:14px;background:rgba(74,255,31,.06);border:1px solid var(--acc-border);border-radius:var(--r);padding:12px 14px;align-items:center;gap:12px}
.cert-info.show{display:flex}
.cert-info-ico{width:36px;height:36px;background:var(--acc);border-radius:8px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.cert-info-ico svg{width:18px;height:18px;stroke:#000}
.cert-info-text .lbl{font-size:10px;font-weight:800;letter-spacing:1.5px;text-transform:uppercase;color:var(--fg3)}
.cert-info-text .val{font-family:'Courier New',monospace;font-size:clamp(13px,3vw,14px);font-weight:800;color:var(--acc);margin-top:2px}
.cert-err-msg{display:none;font-size:clamp(12px,2.8vw,14px);color:var(--red);font-weight:700;margin-top:10px;padding:9px 13px;background:var(--red-faint);border-radius:7px;border-left:3px solid var(--red)}
.cert-err-msg.show{display:block}

/* ── WA SECTION ── */
.wa-section{background:linear-gradient(135deg,rgba(37,211,102,.1),rgba(18,140,126,.06));border:1.5px solid rgba(37,211,102,.3);border-radius:var(--rl);padding:clamp(15px,3.8vw,22px);margin-bottom:clamp(12px,3vw,16px);position:relative;overflow:hidden}
.wa-section::before{content:'';position:absolute;top:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent,rgba(37,211,102,.5),transparent)}
.wa-head{display:flex;align-items:center;gap:13px;margin-bottom:13px}
.wa-ico-w{width:48px;height:48px;background:var(--wa);border-radius:13px;display:flex;align-items:center;justify-content:center;flex-shrink:0;box-shadow:0 0 16px rgba(37,211,102,.32)}
.wa-ico-w svg{width:25px;height:25px;fill:#fff}
.wa-head h3{font-size:clamp(15px,3.5vw,17px);font-weight:900;color:var(--fg)}
.wa-head p{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);margin-top:2px}
.wa-num{font-family:'Courier New',monospace;font-size:clamp(14px,3.2vw,16px);color:var(--wa);font-weight:800;background:rgba(37,211,102,.1);border:1px solid rgba(37,211,102,.28);border-radius:7px;padding:6px 13px;display:inline-block;margin-bottom:13px}
.wa-note{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);line-height:1.7;margin-bottom:15px;padding:11px 14px;background:rgba(0,0,0,.18);border-radius:9px;border-left:3px solid var(--wa)}

/* ── DOWNLOAD SECTION ── */
.dl-section{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(14px,3.5vw,20px);margin-bottom:clamp(12px,3vw,16px);position:relative;overflow:hidden}
.dl-section::before{content:'';position:absolute;top:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent 5%,var(--acc-border) 50%,transparent 95%)}
.dl-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:9px;margin-top:13px}

/* ── BUTTONS ── */
.btn{display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:clamp(13px,3.2vw,16px);border-radius:var(--r);border:none;font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;font-size:clamp(14px,3.2vw,16px);font-weight:900;letter-spacing:1.5px;text-transform:uppercase;cursor:pointer;transition:all .2s}
.btn svg{width:17px;height:17px;flex-shrink:0}
.btn-acc{background:var(--acc);color:#000;box-shadow:0 0 18px var(--acc-glow)}
.btn-acc:hover:not(:disabled){box-shadow:0 0 30px var(--acc-glow);transform:translateY(-1px)}
.btn-acc:disabled{background:var(--s3);color:var(--fg3);box-shadow:none;cursor:not-allowed}
.btn-out{background:transparent;border:2px solid var(--b2);color:var(--fg2)}
.btn-out:hover{border-color:var(--acc);color:var(--acc)}
.btn-red{background:var(--red-faint);border:2px solid var(--red-border);color:var(--red)}
.btn-red:hover{background:rgba(255,51,85,.16);border-color:var(--red)}
.btn-wa{background:var(--wa);color:#fff;box-shadow:0 0 18px rgba(37,211,102,.3)}
.btn-wa:hover:not(:disabled){background:var(--wa2);box-shadow:0 0 30px rgba(37,211,102,.42);transform:translateY(-1px)}
.btn-wa:disabled{background:var(--s3);color:var(--fg3);box-shadow:none;cursor:not-allowed}
.btn-dl{background:var(--s3);color:var(--fg2);border:2px solid var(--b2);font-size:clamp(11px,2.5vw,13px);padding:10px 7px;letter-spacing:.7px;flex-direction:column;gap:4px}
.btn-dl svg{width:15px;height:15px}
.btn-dl:hover:not(:disabled){border-color:var(--acc);color:var(--acc);background:var(--acc-faint)}
.btn-dl:disabled{opacity:.38;cursor:not-allowed}
.btn-stk{display:flex;flex-direction:column;gap:11px;margin-top:16px}
.spin{width:17px;height:17px;border:2.5px solid rgba(0,0,0,.2);border-top-color:#000;border-radius:50%;animation:rot .65s linear infinite;display:inline-block}
@keyframes rot{to{transform:rotate(360deg)}}

/* ── HISTORY ── */
.hcard{background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(13px,3.2vw,17px);margin-bottom:11px;transition:border-color .2s}
.hcard:hover{border-color:var(--acc-border)}
.hrow{display:flex;align-items:flex-start;gap:11px}
.hico{width:clamp(34px,8vw,42px);height:clamp(34px,8vw,42px);border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:19px;flex-shrink:0;background:var(--s3)}
.hinfo{flex:1;min-width:0}
.hveh{font-size:clamp(14px,3.2vw,16px);font-weight:800;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.hreg{font-family:'Courier New',monospace;font-size:clamp(11px,2.5vw,12px);color:var(--acc);margin-top:3px}
.hmeta{font-size:clamp(11px,2.5vw,13px);color:var(--fg2);margin-top:2px}
.hrid{font-family:'Courier New',monospace;font-size:clamp(9px,2vw,11px);color:var(--fg3);margin-top:3px}
.hstat{font-size:11px;font-weight:900;letter-spacing:1px;padding:4px 10px;border-radius:20px;white-space:nowrap;flex-shrink:0}
.hstat.complete{background:var(--acc-faint);color:var(--acc);border:1px solid var(--acc-border)}
.hstat.critical{background:rgba(255,51,85,.12);color:var(--red);border:1px solid rgba(255,51,85,.3)}

/* ── HELP ── */
.help-hero{background:linear-gradient(135deg,var(--s2),var(--s3));border:1px solid var(--b1);border-radius:var(--rxl);padding:clamp(20px,5vw,28px);margin-bottom:18px;text-align:center;position:relative;overflow:hidden}
.help-hero::before{content:'';position:absolute;top:-40px;left:50%;transform:translateX(-50%);width:180px;height:180px;background:radial-gradient(circle,var(--acc-faint) 0%,transparent 70%);pointer-events:none}
.help-hero-ico{font-size:42px;margin-bottom:11px}
.help-hero h2{font-size:clamp(18px,4.5vw,24px);font-weight:900;color:var(--acc);text-shadow:0 0 14px var(--acc-glow);margin-bottom:5px}
.help-hero p{font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.6}
.help-step{display:flex;gap:13px;background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(13px,3.3vw,17px);margin-bottom:11px}
.step-num{width:clamp(34px,8vw,40px);height:clamp(34px,8vw,40px);background:var(--acc);color:#000;border-radius:50%;display:flex;align-items:center;justify-content:center;font-weight:900;font-size:clamp(14px,3.5vw,17px);flex-shrink:0;box-shadow:0 0 12px var(--acc-glow)}
.step-body{flex:1}
.step-title{font-size:clamp(14px,3.2vw,16px);font-weight:900;margin-bottom:5px}
.step-desc{font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.6}
.help-tip{background:var(--acc-faint);border:1px solid var(--acc-border);border-radius:var(--r);padding:clamp(11px,2.8vw,15px);margin-bottom:9px;display:flex;gap:11px}
.tip-ico{font-size:19px;flex-shrink:0}
.tip-text{font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.6}
.tip-text strong{color:var(--acc);font-weight:800}
.help-warn{background:var(--red-faint);border:1px solid var(--red-border);border-radius:var(--r);padding:clamp(11px,2.8vw,15px);margin-bottom:9px;display:flex;gap:11px}
.warn-text{font-size:clamp(13px,3vw,15px);color:var(--fg2);line-height:1.6}
.hsg-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:9px;margin-bottom:14px}
.hsg{border-radius:var(--r);padding:13px 9px;text-align:center;border:1px solid}
.hsg-ico{font-size:21px;margin-bottom:5px}
.hsg-lbl{font-size:clamp(12px,2.8vw,14px);font-weight:900;letter-spacing:.8px}
.hsg-sub{font-size:clamp(10px,2.2vw,12px);color:var(--fg2);margin-top:3px;line-height:1.4}
.hsg.good{background:rgba(74,255,31,.07);border-color:rgba(74,255,31,.3);color:var(--acc)}
.hsg.minor{background:rgba(255,214,0,.07);border-color:rgba(255,214,0,.3);color:var(--yel)}
.hsg.crit{background:rgba(255,51,85,.07);border-color:rgba(255,51,85,.3);color:var(--red)}

/* ── SETTINGS ── */
.sgrp{margin-bottom:22px}
.sitem{display:flex;align-items:center;gap:13px;background:var(--s2);border:1px solid var(--b1);border-radius:var(--rl);padding:clamp(12px,3vw,16px);margin-bottom:9px}
.sico{width:clamp(36px,8.5vw,44px);height:clamp(36px,8.5vw,44px);background:var(--acc-faint);border:1px solid var(--acc-border);border-radius:9px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.sico svg{width:clamp(16px,4vw,20px);height:clamp(16px,4vw,20px);color:var(--acc)}
.stxt{flex:1;min-width:0}
.slbl{font-size:clamp(14px,3.2vw,16px);font-weight:800}
.ssub{font-size:clamp(12px,2.7vw,14px);color:var(--fg2);margin-top:2px}
.tog{width:46px;height:25px;background:var(--s3);border:2px solid var(--b2);border-radius:13px;position:relative;cursor:pointer;transition:background .22s,border-color .22s;flex-shrink:0}
.tog.on{background:var(--acc);border-color:var(--acc)}
.tog::after{content:'';position:absolute;width:19px;height:19px;background:#fff;border-radius:50%;top:1px;left:1px;transition:left .22s;box-shadow:0 1px 4px rgba(0,0,0,.4)}
.tog.on::after{left:22px}
.arow{display:flex;justify-content:space-between;align-items:center;padding:10px 0;border-bottom:1px solid var(--b1);font-size:clamp(13px,3vw,15px)}
.arow:last-child{border-bottom:none}
.akey{color:var(--fg2);font-weight:700}
.aval{font-family:'Courier New',monospace;font-size:clamp(11px,2.5vw,12px);color:var(--acc)}
.copy-band{background:var(--s3);border:1px solid var(--b2);border-radius:var(--r);padding:14px 15px;text-align:center;margin-top:8px}
.copy-band p{font-size:clamp(12px,2.8vw,14px);color:var(--fg2);line-height:1.7}
.copy-band strong{color:var(--acc)}

/* ── EMPTY ── */
.empty{text-align:center;padding:clamp(44px,11vw,68px) 20px;color:var(--fg2)}
.empty svg{width:48px;height:48px;opacity:.2;margin-bottom:15px}
.empty h3{font-size:clamp(16px,3.8vw,19px);font-weight:900;margin-bottom:6px;color:var(--fg)}
.empty p{font-size:clamp(13px,3vw,15px)}

/* ── MODAL ── */
.moverlay{position:fixed;inset:0;background:rgba(0,0,0,.8);z-index:500;display:flex;align-items:flex-end;opacity:0;pointer-events:none;transition:opacity .24s}
.moverlay.open{opacity:1;pointer-events:all}
.mbox{background:var(--s2);border:1px solid var(--b2);border-radius:var(--rxl) var(--rxl) 0 0;padding:clamp(19px,4.8vw,27px);padding-bottom:calc(clamp(19px,4.8vw,27px) + var(--safe-b));width:100%;transform:translateY(100%);transition:transform .28s cubic-bezier(.4,0,.2,1)}
.moverlay.open .mbox{transform:none}
.mhandle{width:38px;height:4px;background:var(--b2);border-radius:2px;margin:0 auto 17px}
.mtitle{font-size:clamp(16px,4vw,21px);font-weight:900;margin-bottom:9px}
.mbody{font-size:clamp(13px,3vw,15px);color:var(--fg2);margin-bottom:20px;line-height:1.7}
.mbtns{display:flex;gap:11px}
.mbtns .btn{margin:0}
@media(min-width:540px){.moverlay{align-items:center;justify-content:center}.mbox{border-radius:var(--rxl);max-width:450px;width:90%;padding-bottom:clamp(19px,4.8vw,27px)}}

/* ── TOAST ── */
#toast{position:fixed;top:clamp(62px,12vw,78px);left:50%;transform:translateX(-50%) translateY(-16px);background:var(--s2);border:2px solid var(--acc);border-radius:var(--r);padding:9px 18px;font-size:clamp(13px,3vw,15px);font-weight:800;color:var(--acc);box-shadow:0 0 22px var(--acc-glow);z-index:9998;opacity:0;transition:all .26s;white-space:nowrap;pointer-events:none;max-width:90vw}
#toast.show{opacity:1;transform:translateX(-50%) translateY(0)}
#toast.err{border-color:var(--red);color:var(--red);box-shadow:0 0 22px var(--red-g)}

#report-render{position:fixed;left:-9999px;top:0;width:860px;display:none;z-index:-999}
</style>
</head>
<body>

<!-- TOP BAR -->
<header id="topbar">
  <div>
    <div class="tb-logo">Fleet<em>Guard</em> Pro</div>
    <div class="tb-client">Women's Choice Quality Waters</div>
  </div>
  <div class="tb-dot"></div>
</header>

<div id="pages">

<!-- ══════════ HOME ══════════ -->
<div class="page active" id="page-home">
  <div class="pg-title" id="greeting">Good morning</div>
  <div class="pg-sub">Fleet inspection overview</div>
  <div class="stat-grid">
    <div class="stat"><div class="stat-n" id="s-total">0</div><div class="stat-l">Total</div></div>
    <div class="stat"><div class="stat-n" id="s-comp" style="color:var(--acc)">0</div><div class="stat-l">Complete</div></div>
    <div class="stat"><div class="stat-n" id="s-crit" style="color:var(--red)">0</div><div class="stat-l">Critical</div></div>
    <div class="stat"><div class="stat-n" id="s-today">0</div><div class="stat-l">Today</div></div>
  </div>
  <div class="card">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>Recent Activity</div>
    <div id="home-recent"></div>
  </div>
  <div class="qa" onclick="switchTab('new')">
    <div class="qa-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 5H7a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V7a2 2 0 0 0-2-2h-2"/><rect x="9" y="3" width="6" height="4" rx="1"/><path d="m9 12 2 2 4-4"/></svg></div>
    <div class="qa-text"><div class="qa-t">Start New Inspection</div><div class="qa-s">Full vehicle assessment form</div></div>
    <div class="qa-arr"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="9 18 15 12 9 6"/></svg></div>
  </div>
  <div class="qa" onclick="switchTab('history')">
    <div class="qa-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg></div>
    <div class="qa-text"><div class="qa-t">Inspection History</div><div class="qa-s">Last 7 days — auto-cleared</div></div>
    <div class="qa-arr"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="9 18 15 12 9 6"/></svg></div>
  </div>
  <div class="qa" onclick="switchTab('help')">
    <div class="qa-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg></div>
    <div class="qa-text"><div class="qa-t">How to Use This App</div><div class="qa-s">Step-by-step guide &amp; tips</div></div>
    <div class="qa-arr"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="9 18 15 12 9 6"/></svg></div>
  </div>
</div>

<!-- ══════════ NEW INSPECTION ══════════ -->
<div class="page" id="page-new">
  <div class="pg-title">New Inspection</div>
  <div class="pg-sub">Fields marked <span style="color:var(--acc);font-weight:900">✱</span> are required</div>
  <div class="rpt-badge"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg><span id="rpt-id">RPT-···</span></div>

  <!-- MISSED SUMMARY BANNER -->
  <div class="miss-banner" id="miss-banner">
    <div class="miss-ttl">⚠️ Please complete these before submitting:</div>
    <ul class="miss-list" id="miss-list"></ul>
  </div>

  <!-- VEHICLE -->
  <div class="card">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="1" y="3" width="15" height="13" rx="2"/><path d="m16 8 5 3v5h-5"/><circle cx="5.5" cy="18.5" r="2.5"/><circle cx="18.5" cy="18.5" r="2.5"/></svg>Vehicle Information</div>
    <div class="g2">
      <div class="field" id="f-v-reg">
        <label>Registration <span class="req">✱</span></label>
        <input type="text" id="v-reg" placeholder="CA 123-456" maxlength="15"
          oninput="onVehChange();cc(this,'v-reg-c')"
          onblur="liveValidate('v-reg','f-v-reg','Enter registration plate')"
          autocapitalize="characters">
        <div class="field-meta"><span class="field-err-msg">Required</span><span class="char-c" id="v-reg-c">0/15</span></div>
      </div>
      <div class="field" id="f-v-year">
        <label>Year <span class="req">✱</span></label>
        <input type="text" id="v-year" placeholder="e.g. 2022" maxlength="4"
          oninput="onVehChange()"
          onblur="liveValidate('v-year','f-v-year','Enter vehicle year')"
          inputmode="numeric">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
    </div>
    <div class="g2">
      <div class="field" id="f-v-make">
        <label>Make <span class="req">✱</span></label>
        <input type="text" id="v-make" placeholder="e.g. Toyota" maxlength="30"
          oninput="onVehChange()"
          onblur="liveValidate('v-make','f-v-make','Enter vehicle make')"
          autocapitalize="words">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
      <div class="field" id="f-v-model">
        <label>Model <span class="req">✱</span></label>
        <input type="text" id="v-model" placeholder="e.g. Hilux" maxlength="30"
          oninput="onVehChange()"
          onblur="liveValidate('v-model','f-v-model','Enter vehicle model')"
          autocapitalize="words">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
    </div>
    <div class="g2">
      <div class="field">
        <label>Vehicle Type</label>
        <select id="v-type" onchange="onVehChange()">
          <option value="">— Select —</option>
          <option>Sedan</option><option>SUV / 4x4</option><option>Pickup Truck</option>
          <option>Panel Van</option><option>Cargo Van</option><option>Minibus</option>
          <option>Bus</option><option>Truck</option><option>Motorcycle</option><option>Other</option>
        </select>
      </div>
      <div class="field">
        <label>Mileage</label>
        <input type="text" id="v-mileage" placeholder="e.g. 87 450 km" maxlength="20" oninput="onVehChange()" inputmode="decimal">
      </div>
    </div>
    <div class="field">
      <label>Colour</label>
      <input type="text" id="v-color" placeholder="e.g. White Pearl" maxlength="30" oninput="onVehChange()" autocapitalize="words">
    </div>
    <div class="veh-prev" id="veh-prev">
      <div><div class="vp-k">Reg</div><div class="vp-v" id="pv-reg">—</div></div>
      <div><div class="vp-k">Year / Make</div><div class="vp-v" id="pv-make">—</div></div>
      <div><div class="vp-k">Model</div><div class="vp-v" id="pv-model">—</div></div>
      <div><div class="vp-k">Type</div><div class="vp-v" id="pv-type">—</div></div>
      <div><div class="vp-k">Mileage</div><div class="vp-v" id="pv-mileage">—</div></div>
      <div><div class="vp-k">Colour</div><div class="vp-v" id="pv-color">—</div></div>
    </div>
  </div>

  <!-- DRIVER -->
  <div class="card">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M20 21a8 8 0 1 0-16 0"/></svg>Driver Information</div>
    <div class="field" id="f-d-name">
      <label>Driver Full Name <span class="req">✱</span></label>
      <input type="text" id="d-name" placeholder="Driver's full name…" maxlength="60"
        oninput="checkReady()"
        onblur="liveValidate('d-name','f-d-name','Enter driver full name')"
        autocapitalize="words">
      <div class="field-meta"><span class="field-err-msg">Required</span></div>
    </div>
    <div class="g2">
      <div class="field">
        <label>Licence No.</label>
        <input type="text" id="d-license" placeholder="Licence number" maxlength="20" autocapitalize="characters">
      </div>
      <div class="field">
        <label>Contact</label>
        <input type="text" id="d-contact" placeholder="+27 82 000 0000" maxlength="20" inputmode="tel">
      </div>
    </div>
  </div>

  <!-- INSPECTOR -->
  <div class="card">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"/></svg>Inspector Details</div>
    <div class="field" id="f-i-name">
      <label>Inspector Full Name <span class="req">✱</span></label>
      <input type="text" id="i-name" placeholder="Your full name…" maxlength="60"
        oninput="checkReady();updateCertName()"
        onblur="liveValidate('i-name','f-i-name','Enter inspector full name')"
        autocapitalize="words">
      <div class="field-meta"><span class="field-err-msg">Required</span></div>
    </div>
    <div class="g2">
      <div class="field" id="f-i-badge">
        <label>Badge / ID <span class="req">✱</span></label>
        <input type="text" id="i-badge" placeholder="e.g. EMP-0042" maxlength="20"
          oninput="checkReady()"
          onblur="liveValidate('i-badge','f-i-badge','Enter badge / employee ID')"
          autocapitalize="characters">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
      <div class="field">
        <label>Location</label>
        <input type="text" id="i-location" placeholder="Depot / site name" maxlength="40" autocapitalize="words">
      </div>
    </div>
    <!-- MANUAL DATE & TIME — inspector types these themselves -->
    <div class="g2">
      <div class="field" id="f-i-date">
        <label>Inspection Date <span class="req">✱</span></label>
        <input type="date" id="i-date"
          onchange="checkReady()"
          onblur="liveValidate('i-date','f-i-date','Select inspection date')">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
      <div class="field" id="f-i-time">
        <label>Inspection Time <span class="req">✱</span></label>
        <input type="time" id="i-time"
          onchange="checkReady()"
          onblur="liveValidate('i-time','f-i-time','Enter inspection time')">
        <div class="field-meta"><span class="field-err-msg">Required</span></div>
      </div>
    </div>
    <p style="font-size:clamp(11px,2.4vw,13px);color:var(--fg3);margin-top:-4px">Enter the actual date and time of this inspection.</p>
  </div>

  <!-- PROGRESS -->
  <div class="card">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>Checklist Progress</div>
    <div class="prog-wrap"><div class="prog-bar" id="prog-bar" style="width:0%"></div></div>
    <div class="prog-lbl" id="prog-lbl">0 / 0 items assessed</div>
  </div>

  <!-- CHECKLIST SECTIONS -->
  <div id="isections"></div>

  <!-- RESULT BANNER -->
  <div class="res-banner" id="res-banner">
    <div class="res-ico" id="res-ico"></div>
    <div class="res-title" id="res-title"></div>
    <div class="res-sub" id="res-sub"></div>
  </div>

  <!-- ELECTRONIC CERTIFICATION -->
  <div class="ecert">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>Electronic Certification</div>
    <p class="ecert-body">By ticking below you confirm that this inspection was carried out by you personally, all information is accurate, and you take full responsibility for this report.</p>
    <label class="cert-row" id="cert-row" onclick="onCertClick(event)">
      <input type="checkbox" id="cert-chk">
      <div class="cert-box"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg></div>
      <span class="cert-text">I, <span class="cert-name" id="cert-name-disp">the inspector</span>, certify that this vehicle inspection report is complete, accurate and true to the best of my knowledge.</span>
    </label>
    <div class="cert-err-msg" id="cert-err-msg">⚠️ Enter your Inspector Name &amp; Badge/ID above before certifying.</div>
    <div class="cert-info" id="cert-info">
      <div class="cert-info-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><polyline points="20 6 9 17 4 12"/></svg></div>
      <div class="cert-info-text">
        <div class="lbl">Electronically Certified By</div>
        <div class="val" id="cert-info-val">—</div>
      </div>
    </div>
  </div>

  <!-- WHATSAPP -->
  <div class="wa-section">
    <div class="wa-head">
      <div class="wa-ico-w"><svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 0 1-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 0 1-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 0 1 2.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0 0 12.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 0 0 5.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 0 0-3.48-8.413z"/></svg></div>
      <div><h3>Send via WhatsApp</h3><p>Fleet manager · +27 78 020 5539</p></div>
    </div>
    <div class="wa-num">+27 78 020 5539</div>
    <div class="wa-note">ℹ️ Tapping <strong>Send to WhatsApp</strong> opens WhatsApp with the full formatted inspection report ready to send. Complete all required fields <span style="color:var(--acc);font-weight:900">✱</span> and certify electronically first.</div>
    <button class="btn btn-wa" id="wa-btn" disabled onclick="sendWhatsApp()">
      <svg viewBox="0 0 24 24" style="fill:currentColor;width:19px;height:19px"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 0 1-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 0 1-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 0 1 2.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0 0 12.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 0 0 5.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 0 0-3.48-8.413z"/></svg>
      Send to WhatsApp
    </button>
  </div>

  <!-- DOWNLOAD -->
  <div class="dl-section">
    <div class="ch"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>Download Report</div>
    <p style="font-size:clamp(13px,3vw,15px);color:var(--fg2)">Export your inspection. Requires all required fields completed and certified.</p>
    <div class="dl-grid">
      <button class="btn btn-dl" id="dl-png-btn" disabled onclick="downloadImage('png')">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><circle cx="8.5" cy="8.5" r="1.5"/><polyline points="21 15 16 10 5 21"/></svg>PNG
      </button>
      <button class="btn btn-dl" id="dl-jpg-btn" disabled onclick="downloadImage('jpg')">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><circle cx="8.5" cy="8.5" r="1.5"/><polyline points="21 15 16 10 5 21"/></svg>JPG
      </button>
      <button class="btn btn-dl" id="dl-txt-btn" disabled onclick="downloadTXT()">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>TXT Log
      </button>
    </div>
  </div>

  <div class="btn-stk">
    <button class="btn btn-red" onclick="checkMissed()">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>
      Check for Missed Fields
    </button>
    <button class="btn btn-out" onclick="confirmReset()">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="1 4 1 10 7 10"/><path d="M3.51 15a9 9 0 1 0 .49-3.99"/></svg>
      Reset Form
    </button>
  </div>
  <div style="height:12px"></div>
</div>

<!-- ══════════ HISTORY ══════════ -->
<div class="page" id="page-history">
  <div class="pg-title">History</div>
  <div class="pg-sub">Inspections from the last 7 days</div>
  <div id="hist-list"></div>
</div>

<!-- ══════════ HELP ══════════ -->
<div class="page" id="page-help">
  <div class="pg-title">Help &amp; Guide</div>
  <div class="pg-sub">How to use FleetGuard Pro</div>
  <div class="help-hero">
    <div class="help-hero-ico">🚗</div>
    <h2>FleetGuard Pro</h2>
    <p>Digital vehicle inspection for <strong style="color:var(--acc)">Women's Choice Quality Waters</strong>.</p>
  </div>
  <div class="sec-lbl">How It Works</div>
  <div class="help-step"><div class="step-num">1</div><div class="step-body"><div class="step-title">Fill in Vehicle Details</div><div class="step-desc">Enter the registration, year, make, model, type and mileage. Fields with <strong style="color:var(--acc)">✱</strong> are required. Fields go red if you skip past them without filling in.</div></div></div>
  <div class="help-step"><div class="step-num">2</div><div class="step-body"><div class="step-title">Driver &amp; Inspector Info</div><div class="step-desc">Enter driver's full name and licence. Enter your inspector name and badge. Then manually set the inspection <strong style="color:var(--acc)">date and time</strong>.</div></div></div>
  <div class="help-step"><div class="step-num">3</div><div class="step-body"><div class="step-title">Complete All Checklist Items</div><div class="step-desc">Tap a section to expand it. Select <strong style="color:var(--acc)">Good</strong>, <strong style="color:var(--yel)">Minor</strong>, or <strong style="color:var(--red)">Critical</strong> for every item. You can add notes and up to 4 photos per item.</div></div></div>
  <div class="help-step"><div class="step-num">4</div><div class="step-body"><div class="step-title">Check for Missed Fields</div><div class="step-desc">Tap <strong style="color:var(--red)">Check for Missed Fields</strong> at any time. All empty required fields and unanswered items will glow red and scroll into view.</div></div></div>
  <div class="help-step"><div class="step-num">5</div><div class="step-body"><div class="step-title">Electronic Certification</div><div class="step-desc">Tick the certification checkbox. This replaces a paper signature and certifies the report under your name and badge. Your name must be entered first.</div></div></div>
  <div class="help-step"><div class="step-num">6</div><div class="step-body"><div class="step-title">Send or Download</div><div class="step-desc">Tap <strong style="color:var(--wa)">Send to WhatsApp</strong> to send the full report to the fleet manager at +27 78 020 5539. Or download as PNG, JPG, or TXT log.</div></div></div>
  <div class="sec-lbl" style="margin-top:20px">Status Guide</div>
  <div class="hsg-grid">
    <div class="hsg good"><div class="hsg-ico">✅</div><div class="hsg-lbl">Good</div><div class="hsg-sub">No issues found</div></div>
    <div class="hsg minor"><div class="hsg-ico">⚠️</div><div class="hsg-lbl">Minor</div><div class="hsg-sub">Needs attention soon</div></div>
    <div class="hsg crit"><div class="hsg-ico">🔴</div><div class="hsg-lbl">Critical</div><div class="hsg-sub">Immediate action required</div></div>
  </div>
  <div class="sec-lbl">Tips</div>
  <div class="help-tip"><div class="tip-ico">📸</div><div class="tip-text"><strong>Photos:</strong> Upload up to 4 photos per checklist item for evidence. Clear photos help the fleet manager assess the issue without visiting the vehicle.</div></div>
  <div class="help-tip"><div class="tip-ico">🪪</div><div class="tip-text"><strong>Licence Disc:</strong> Always inspect the disc — missing or expired discs are a legal issue and must be marked <strong style="color:var(--red)">Critical</strong>.</div></div>
  <div class="help-tip"><div class="tip-ico">🔴</div><div class="tip-text"><strong>Red Highlights:</strong> Any field you skip will turn red when you leave it. Use <em>Check for Missed Fields</em> to find everything at once.</div></div>
  <div class="help-warn"><div class="tip-ico">⚠️</div><div class="warn-text">WhatsApp must be installed on your device to use the send feature. Reports go to fleet manager <strong>+27 78 020 5539</strong>.</div></div>
  <div class="card" style="margin-top:14px">
    <div class="arow"><span class="akey">Fleet Manager</span><span class="aval" style="color:var(--wa)">+27 78 020 5539</span></div>
    <div class="arow"><span class="akey">Version</span><span class="aval">6.0.0</span></div>
    <div class="arow"><span class="akey">Developer</span><span class="aval">Graphiccafe PTY LTD</span></div>
    <div class="arow"><span class="akey">Client</span><span class="aval" style="font-size:10px">Women's Choice Quality Waters</span></div>
  </div>
</div>

<!-- ══════════ SETTINGS ══════════ -->
<div class="page" id="page-settings">
  <div class="pg-title">Settings</div>
  <div class="pg-sub">App configuration &amp; information</div>
  <div class="sgrp">
    <div class="sec-lbl">Display</div>
    <div class="sitem">
      <div class="sico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg></div>
      <div class="stxt"><div class="slbl">Dark / Light Mode</div><div class="ssub">Toggle interface brightness</div></div>
      <div class="tog on" id="dark-tog" onclick="toggleMode(this)"></div>
    </div>
  </div>
  <div class="sgrp">
    <div class="sec-lbl">Data</div>
    <div class="sitem">
      <div class="sico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="3 6 5 6 21 6"/><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a1 1 0 0 1 1-1h4a1 1 0 0 1 1 1v2"/></svg></div>
      <div class="stxt"><div class="slbl">Clear All Records</div><div class="ssub">Remove all stored inspection history</div></div>
      <button class="btn btn-out" style="width:auto;padding:8px 15px;font-size:13px;letter-spacing:1px" onclick="clearAll()">Clear</button>
    </div>
  </div>
  <div class="sgrp">
    <div class="sec-lbl">About</div>
    <div class="card">
      <div class="arow"><span class="akey">Application</span><span class="aval">FleetGuard Pro</span></div>
      <div class="arow"><span class="akey">Version</span><span class="aval">6.0.0</span></div>
      <div class="arow"><span class="akey">Certification</span><span class="aval">Electronic checkbox</span></div>
      <div class="arow"><span class="akey">Date / Time</span><span class="aval">Manual entry</span></div>
      <div class="arow"><span class="akey">Photos per item</span><span class="aval">Up to 4</span></div>
      <div class="arow"><span class="akey">Send method</span><span class="aval">WhatsApp</span></div>
      <div class="arow"><span class="akey">Fleet manager</span><span class="aval" style="color:var(--wa)">+27 78 020 5539</span></div>
      <div class="arow"><span class="akey">Storage</span><span class="aval">localStorage · 7 days</span></div>
    </div>
    <div class="copy-band">
      <p>© 2025 <strong>Melato Tatu</strong> / <strong>Graphiccafe PTY LTD</strong><br>
      Developed exclusively for<br><strong>Women's Choice Quality Waters</strong><br>
      All rights reserved.</p>
    </div>
  </div>
</div>

</div><!-- /pages -->

<nav id="bnav">
  <button class="nb active" data-t="home" onclick="switchTab('home')">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>Home
  </button>
  <button class="nb" data-t="new" onclick="switchTab('new')">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 5H7a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V7a2 2 0 0 0-2-2h-2"/><rect x="9" y="3" width="6" height="4" rx="1"/><path d="m9 12 2 2 4-4"/></svg>Inspect
  </button>
  <button class="nb" data-t="history" onclick="switchTab('history')">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>History
  </button>
  <button class="nb" data-t="help" onclick="switchTab('help')">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg>Help
  </button>
  <button class="nb" data-t="settings" onclick="switchTab('settings')">
    <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1-2.83 2.83l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-4 0v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83-2.83l.06-.06A1.65 1.65 0 0 0 4.68 15a1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1 0-4h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 2.83-2.83l.06.06A1.65 1.65 0 0 0 9 4.68a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 4 0v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 2.83l-.06.06A1.65 1.65 0 0 0 19.4 9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 0 4h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>Settings
  </button>
</nav>

<div class="moverlay" id="reset-modal" onclick="if(event.target===this)closeModal('reset-modal')">
  <div class="mbox">
    <div class="mhandle"></div>
    <div class="mtitle">Reset Form?</div>
    <div class="mbody">All entered data and checklist responses will be cleared. History records are not affected.</div>
    <div class="mbtns">
      <button class="btn btn-out" onclick="closeModal('reset-modal')" style="flex:1">Cancel</button>
      <button class="btn" onclick="resetForm();closeModal('reset-modal')" style="flex:2;background:var(--red);color:#fff">Reset</button>
    </div>
  </div>
</div>

<div id="report-render"></div>
<div id="toast"></div>

<script>
/* ═════════════════════════════════════
   SCHEMA
═════════════════════════════════════ */
const SCHEMA = [
  { id:'exterior', label:'Exterior', ico:'car', items:[
    {id:'body_panels',  lbl:'Body Panels & Paint'},
    {id:'windscreen',   lbl:'Windscreen & Windows'},
    {id:'mirrors',      lbl:'Mirrors'},
    {id:'tyres',        lbl:'Tyres & Rims'},
    {id:'wipers',       lbl:'Wipers & Washers'},
  ]},
  { id:'interior', label:'Interior', ico:'int', items:[
    {id:'dashboard',    lbl:'Dashboard & Warning Lights'},
    {id:'seatbelts',    lbl:'Seatbelts'},
    {id:'seats',        lbl:'Seats & Headrests'},
    {id:'horn',         lbl:'Horn'},
    {id:'ac',           lbl:'Air Conditioning'},
  ]},
  { id:'engine', label:'Engine', ico:'eng', items:[
    {id:'oil',          lbl:'Engine Oil Level'},
    {id:'coolant',      lbl:'Coolant Level'},
    {id:'battery',      lbl:'Battery Condition'},
    {id:'belts',        lbl:'Belts & Hoses'},
    {id:'brakefld',     lbl:'Brake Fluid Level'},
  ]},
  { id:'lights', label:'Lights & Electrics', ico:'lit', items:[
    {id:'headlights',   lbl:'Headlights (High & Low Beam)'},
    {id:'taillights',   lbl:'Tail & Brake Lights'},
    {id:'indicators',   lbl:'Indicators & Hazards'},
    {id:'reverselit',   lbl:'Reverse Light'},
    {id:'intlights',    lbl:'Interior Lights'},
  ]},
  { id:'licdisc', label:'Licence Disc', ico:'disc', items:[
    {id:'disc_present', lbl:'Licence Disc is Present'},
    {id:'disc_legible', lbl:'Licence Disc is Legible'},
    {id:'disc_expiry',  lbl:'Licence Disc Not Expired'},
    {id:'disc_correct', lbl:'Disc Matches Vehicle Registration'},
    {id:'disc_pos',     lbl:'Disc Displayed on Windscreen'},
  ]},
];

const ICOS = {
  car: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="1" y="3" width="15" height="13" rx="2"/><path d="m16 8 5 3v5h-5"/><circle cx="5.5" cy="18.5" r="2.5"/><circle cx="18.5" cy="18.5" r="2.5"/></svg>`,
  int: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/></svg>`,
  eng: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 7V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v2"/><line x1="12" y1="12" x2="12" y2="16"/><line x1="10" y1="14" x2="14" y2="14"/></svg>`,
  lit: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="5"/><line x1="12" y1="1" x2="12" y2="3"/><line x1="12" y1="21" x2="12" y2="23"/><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"/><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"/><line x1="1" y1="12" x2="3" y2="12"/><line x1="21" y1="12" x2="23" y2="12"/></svg>`,
  disc:`<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="3"/><line x1="12" y1="2" x2="12" y2="9"/><line x1="12" y1="15" x2="12" y2="22"/></svg>`,
};

const WA_NUM = '27780205539';

/* ═════════════════════════════════════
   STATE
═════════════════════════════════════ */
let S = { reportId:'', certified:false, data:{} };

/* ═════════════════════════════════════
   INIT
═════════════════════════════════════ */
document.addEventListener('DOMContentLoaded', () => {
  loadTheme();
  initData();
  buildSections();
  newReportId();
  cleanOld();
  updateDash();
  setGreeting();
});

const g  = id => document.getElementById(id);
const gv = id => { const e = g(id); return e ? e.value.trim() : ''; };
const cc = (input, cid) => { const e = g(cid); if (e) e.textContent = `${input.value.length}/${input.maxLength}`; };

function initData() {
  SCHEMA.forEach(sec => sec.items.forEach(item => {
    S.data[item.id] = { status:null, comment:'', images:[] };
  }));
}

function setGreeting() {
  const h = new Date().getHours();
  const gr = h < 12 ? 'Good morning' : h < 17 ? 'Good afternoon' : 'Good evening';
  const el = g('greeting'); if (el) el.textContent = gr;
}

function newReportId() {
  const ts = Date.now().toString(36).toUpperCase();
  const rn = Math.random().toString(36).slice(2,5).toUpperCase();
  S.reportId = `RPT-${ts}-${rn}`;
  const el = g('rpt-id'); if (el) el.textContent = S.reportId;
}

/* ═════════════════════════════════════
   LIVE VALIDATION — turns field red on blur
═════════════════════════════════════ */
function liveValidate(inputId, fieldId) {
  const val = gv(inputId);
  const fEl = g(fieldId);
  if (!fEl) return;
  if (!val) {
    fEl.classList.add('err');
  } else {
    fEl.classList.remove('err');
  }
  checkReady();
}

function clearErr(fieldId) {
  const fEl = g(fieldId);
  if (fEl) fEl.classList.remove('err');
}

/* ═════════════════════════════════════
   VEHICLE PREVIEW
═════════════════════════════════════ */
function onVehChange() {
  const reg = gv('v-reg'), yr = gv('v-year'), mk = gv('v-make'),
        mdl = gv('v-model'), type = gv('v-type'), mil = gv('v-mileage'), col = gv('v-color');
  const prev = g('veh-prev');
  const has = reg || mk || mdl;
  if (prev) prev.style.display = has ? 'grid' : 'none';
  if (has) {
    const s = (id,val) => { const e=g(id); if(e) e.textContent = val||'—'; };
    s('pv-reg',reg); s('pv-make',`${yr||'—'} / ${mk||'—'}`);
    s('pv-model',mdl); s('pv-type',type); s('pv-mileage',mil); s('pv-color',col);
  }
  // clear err on those fields if now filled
  if (reg)  clearErr('f-v-reg');
  if (yr)   clearErr('f-v-year');
  if (mk)   clearErr('f-v-make');
  if (mdl)  clearErr('f-v-model');
  checkReady();
}

/* ═════════════════════════════════════
   ELECTRONIC CERT
═════════════════════════════════════ */
function updateCertName() {
  const nm = gv('i-name');
  const el = g('cert-name-disp');
  if (el) el.textContent = nm || 'the inspector';
}

function onCertClick(e) {
  e.preventDefault();
  const iName  = gv('i-name');
  const iBadge = gv('i-badge');
  const chk    = g('cert-chk');
  const row    = g('cert-row');
  const errMsg = g('cert-err-msg');
  const info   = g('cert-info');
  const infoVal= g('cert-info-val');

  if (!iName || !iBadge) {
    // flash error, highlight missing inspector fields
    row.classList.add('cert-err');
    setTimeout(() => row.classList.remove('cert-err'), 800);
    if (errMsg) errMsg.classList.add('show');
    if (!iName)  { const f = g('f-i-name');  if(f) f.classList.add('err'); }
    if (!iBadge) { const f = g('f-i-badge'); if(f) f.classList.add('err'); }
    return;
  }

  // toggle
  chk.checked = !chk.checked;
  S.certified = chk.checked;
  row.classList.toggle('cert-done', chk.checked);
  if (errMsg) errMsg.classList.remove('show');

  if (chk.checked) {
    if (infoVal) infoVal.textContent = `${iName}  ·  ${iBadge}`;
    if (info)    info.classList.add('show');
  } else {
    if (info) info.classList.remove('show');
  }
  checkReady();
}

/* ═════════════════════════════════════
   BUILD CHECKLIST
═════════════════════════════════════ */
function buildSections() {
  const wrap = g('isections'); if (!wrap) return;
  wrap.innerHTML = '';
  SCHEMA.forEach(sec => {
    const div = document.createElement('div');
    div.className = 'isec'; div.id = `sec-${sec.id}`;
    div.innerHTML = `
      <div class="isec-hdr" onclick="toggleSec('${sec.id}')">
        <div class="isec-ico">${ICOS[sec.ico]}</div>
        <div class="isec-title">${sec.label}</div>
        <div class="isec-badge" id="bdg-${sec.id}">0/${sec.items.length}</div>
        <svg class="isec-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
      </div>
      <div class="isec-body"><div class="isec-inner" id="inn-${sec.id}"></div></div>`;
    wrap.appendChild(div);
    sec.items.forEach(item => g(`inn-${sec.id}`).appendChild(buildItem(item)));
  });
}

function toggleSec(id) { const el = g(`sec-${id}`); if (el) el.classList.toggle('open'); }

function buildItem(item) {
  const el = document.createElement('div');
  el.className = 'iitem'; el.id = `itm-${item.id}`;
  el.innerHTML = `
    <div class="iitem-name">${item.lbl}</div>
    <div class="srow">
      <button class="sbtn" data-v="good"     data-it="${item.id}" onclick="setStatus('${item.id}','good')">✓ Good</button>
      <button class="sbtn" data-v="minor"    data-it="${item.id}" onclick="setStatus('${item.id}','minor')">⚠ Minor</button>
      <button class="sbtn" data-v="critical" data-it="${item.id}" onclick="setStatus('${item.id}','critical')">✕ Critical</button>
    </div>
    <textarea placeholder="Notes / comments (optional)…" id="cmt-${item.id}" oninput="S.data['${item.id}'].comment=this.value"></textarea>
    <div class="img-drop">
      <input type="file" accept="image/*" multiple onchange="handleImgs('${item.id}',this)">
      <div class="img-drop-l"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>Upload photos (max 4 per item)</div>
    </div>
    <div class="img-thumbs" id="prv-${item.id}"></div>`;
  return el;
}

function setStatus(itemId, val) {
  S.data[itemId].status = val;
  document.querySelectorAll(`.sbtn[data-it="${itemId}"]`).forEach(b => b.classList.toggle('on', b.dataset.v === val));
  const el = g(`itm-${itemId}`);
  if (el) { el.className = `iitem st-${val}`; } // clears item-missed too
  updateProgress(); updateBadge(itemId); renderResult(); checkReady();
}

function updateBadge(itemId) {
  SCHEMA.forEach(sec => {
    if (!sec.items.find(i => i.id === itemId)) return;
    const done = sec.items.filter(i => S.data[i.id]?.status).length;
    const bdg = g(`bdg-${sec.id}`); if (bdg) bdg.textContent = `${done}/${sec.items.length}`;
    const el  = g(`sec-${sec.id}`); if (!el) return;
    const hasCrit = sec.items.some(i => S.data[i.id]?.status === 'critical');
    const allDone = sec.items.every(i => S.data[i.id]?.status);
    el.classList.toggle('iscrit', hasCrit);
    el.classList.toggle('isdone', allDone && !hasCrit);
    if (allDone) el.classList.remove('sec-missed');
  });
}

function updateProgress() {
  const all  = SCHEMA.flatMap(s => s.items);
  const done = all.filter(i => S.data[i.id]?.status).length;
  const pct  = all.length ? Math.round(done / all.length * 100) : 0;
  const pb = g('prog-bar'); if (pb) pb.style.width = pct + '%';
  const pl = g('prog-lbl'); if (pl) pl.textContent = `${done} / ${all.length} items assessed`;
}

function renderResult() {
  const banner = g('res-banner'); if (!banner) return;
  const assessed = SCHEMA.flatMap(s => s.items).filter(i => S.data[i.id]?.status);
  if (!assessed.length) { banner.style.display = 'none'; return; }
  const hasCrit = assessed.some(i => S.data[i.id]?.status === 'critical');
  banner.style.display = 'block';
  banner.className = 'res-banner ' + (hasCrit ? 'critical' : 'complete');
  g('res-ico').textContent  = hasCrit ? '⛔' : '✅';
  g('res-title').textContent = hasCrit ? 'CRITICAL ISSUES FOUND' : 'INSPECTION COMPLETE';
  g('res-sub').textContent   = hasCrit
    ? 'One or more critical items found. Vehicle requires immediate attention.'
    : 'All assessed items recorded. Vehicle meets inspection standards.';
}

/* ═════════════════════════════════════
   CHECK MISSED — highlights everything red
═════════════════════════════════════ */
function checkMissed() {
  const missed = [];

  const reqFields = [
    {vid:'v-reg',   fid:'f-v-reg',   label:'Vehicle Registration'},
    {vid:'v-year',  fid:'f-v-year',  label:'Vehicle Year'},
    {vid:'v-make',  fid:'f-v-make',  label:'Vehicle Make'},
    {vid:'v-model', fid:'f-v-model', label:'Vehicle Model'},
    {vid:'d-name',  fid:'f-d-name',  label:'Driver Full Name'},
    {vid:'i-name',  fid:'f-i-name',  label:'Inspector Full Name'},
    {vid:'i-badge', fid:'f-i-badge', label:'Inspector Badge / ID'},
    {vid:'i-date',  fid:'f-i-date',  label:'Inspection Date'},
    {vid:'i-time',  fid:'f-i-time',  label:'Inspection Time'},
  ];

  reqFields.forEach(({vid, fid, label}) => {
    const fEl = g(fid);
    if (!gv(vid)) {
      if (fEl) fEl.classList.add('err');
      missed.push(label);
    }
  });

  if (!S.certified) missed.push('Electronic Certification — tick the checkbox');

  SCHEMA.forEach(sec => {
    const unassessed = sec.items.filter(i => !S.data[i.id]?.status);
    if (unassessed.length) {
      const secEl = g(`sec-${sec.id}`);
      if (secEl) { secEl.classList.add('sec-missed'); secEl.classList.add('open'); }
      unassessed.forEach(item => {
        const el = g(`itm-${item.id}`);
        if (el) el.classList.add('item-missed');
        missed.push(`${sec.label} → ${item.lbl}`);
      });
    }
  });

  const banner = g('miss-banner');
  const list   = g('miss-list');

  if (!missed.length) {
    if (banner) banner.classList.remove('show');
    toast('✓ All fields complete — ready to send!');
    return;
  }

  if (list)   list.innerHTML = missed.map(m => `<li>${m}</li>`).join('');
  if (banner) banner.classList.add('show');

  const page = g('page-new');
  if (page)   page.scrollTo({ top: 0, behavior: 'smooth' });

  toast(`⚠️ ${missed.length} item${missed.length > 1 ? 's' : ''} need attention`, true);
}

/* ═════════════════════════════════════
   VALIDATION — enables buttons
═════════════════════════════════════ */
function checkReady() {
  updateCertName();
  const ok = gv('v-reg') && gv('v-year') && gv('v-make') && gv('v-model') &&
             gv('d-name') && gv('i-name') && gv('i-badge') &&
             gv('i-date') && gv('i-time') &&
             SCHEMA.flatMap(s => s.items).every(i => S.data[i.id]?.status) &&
             S.certified;
  ['wa-btn','dl-png-btn','dl-jpg-btn','dl-txt-btn'].forEach(id => {
    const el = g(id); if (el) el.disabled = !ok;
  });
  if (ok) { const mb = g('miss-banner'); if (mb) mb.classList.remove('show'); }
}

/* ═════════════════════════════════════
   IMAGES — max 4
═════════════════════════════════════ */
async function handleImgs(itemId, input) {
  const files = Array.from(input.files);
  const cur   = S.data[itemId].images;
  const space = 4 - cur.length;
  if (space <= 0) { toast('Maximum 4 photos per item', true); input.value = ''; return; }
  for (let i = 0; i < Math.min(files.length, space); i++) cur.push(await compressImg(files[i]));
  renderPreviews(itemId); input.value = '';
}

function compressImg(file) {
  return new Promise(res => {
    const fr = new FileReader();
    fr.onload = e => {
      const img = new Image();
      img.onload = () => {
        const MAX = 900; let {width:w, height:h} = img;
        if (w > MAX) { h = Math.round(h * MAX / w); w = MAX; }
        const c = document.createElement('canvas'); c.width = w; c.height = h;
        c.getContext('2d').drawImage(img, 0, 0, w, h);
        res(c.toDataURL('image/jpeg', 0.78));
      };
      img.src = e.target.result;
    };
    fr.readAsDataURL(file);
  });
}

function renderPreviews(itemId) {
  const wrap = g(`prv-${itemId}`); if (!wrap) return;
  wrap.innerHTML = '';
  S.data[itemId].images.forEach((src, i) => {
    const w = document.createElement('div'); w.className = 'img-tw';
    w.innerHTML = `<img src="${src}" alt=""><button class="img-del" onclick="delImg('${itemId}',${i})">✕</button>`;
    wrap.appendChild(w);
  });
}
function delImg(itemId, i) { S.data[itemId].images.splice(i, 1); renderPreviews(itemId); }

/* ═════════════════════════════════════
   REPORT DATA
═════════════════════════════════════ */
function buildRD() {
  const hasCrit = SCHEMA.flatMap(s => s.items).some(i => S.data[i.id]?.status === 'critical');
  return {
    reportId: S.reportId,
    date: gv('i-date'), time: gv('i-time'),
    vReg: gv('v-reg'), vYear: gv('v-year')||'—', vMake: gv('v-make'),
    vModel: gv('v-model'), vType: gv('v-type')||'—',
    vMileage: gv('v-mileage')||'—', vColor: gv('v-color')||'—',
    dName: gv('d-name'), dLicense: gv('d-license')||'—', dContact: gv('d-contact')||'—',
    iName: gv('i-name'), iBadge: gv('i-badge'), iLocation: gv('i-location')||'—',
    hasCrit, verdict: hasCrit ? 'CRITICAL ISSUES FOUND' : 'INSPECTION COMPLETE',
  };
}

/* ═════════════════════════════════════
   WHATSAPP
═════════════════════════════════════ */
function sendWhatsApp() {
  const d = buildRD();
  const lines = [
    `🚗 *FLEETGUARD PRO — VEHICLE INSPECTION REPORT*`,
    `━━━━━━━━━━━━━━━━━━━━━━━━`,
    `📋 Report ID: \`${d.reportId}\``,
    `📅 Date: ${d.date}   🕒 Time: ${d.time}`,
    `${d.hasCrit?'⛔':'✅'} *${d.verdict}*`,'',
    `🚙 *VEHICLE*`,
    `• Reg: *${d.vReg}*   Year: ${d.vYear}`,
    `• ${d.vMake} ${d.vModel} — ${d.vType}`,
    `• Mileage: ${d.vMileage}   Colour: ${d.vColor}`,'',
    `👤 *DRIVER*`,
    `• Name: *${d.dName}*`,
    `• Licence: ${d.dLicense}   Contact: ${d.dContact}`,'',
    `🔍 *INSPECTOR*`,
    `• Name: *${d.iName}*   Badge: ${d.iBadge}`,
    `• Location: ${d.iLocation}`,'',
    `📝 *CHECKLIST*`,
  ];

  SCHEMA.forEach(sec => {
    lines.push(`\n*— ${sec.label.toUpperCase()} —*`);
    sec.items.forEach(item => {
      const st  = S.data[item.id]?.status || 'N/A';
      const ico = st==='good'?'✅':st==='minor'?'⚠️':'🔴';
      const lbl = st==='good'?'GOOD':st==='minor'?'MINOR ISSUE':'CRITICAL';
      const cmt = S.data[item.id]?.comment ? ` _${S.data[item.id].comment}_` : '';
      lines.push(`${ico} ${item.lbl}: *${lbl}*${cmt}`);
    });
  });

  lines.push('',`━━━━━━━━━━━━━━━━━━━━━━━━`,
    `✅ *Electronically certified by: ${d.iName} (${d.iBadge})*`,
    `_Sent via FleetGuard Pro v6.0_`,
    `_Women's Choice Quality Waters_`,
    `_© Melato Tatu / Graphiccafe PTY LTD_`,
    `_${new Date().toISOString()}_`);

  window.open(`https://wa.me/${WA_NUM}?text=${encodeURIComponent(lines.join('\n'))}`, '_blank');

  saveHist({id:d.reportId,date:d.date,time:d.time,vehicle:`${d.vMake} ${d.vModel}`,reg:d.vReg,year:d.vYear,driver:d.dName,inspector:d.iName,badge:d.iBadge,hasCritical:d.hasCrit,timestamp:Date.now()});
  updateDash(); renderHistory();
  toast('✓ WhatsApp opened with full report');
}

/* ═════════════════════════════════════
   HTML REPORT (image export)
═════════════════════════════════════ */
function buildReportHTML() {
  const d  = buildRD();
  const sc = s => s==='good'?'#4AFF1F':s==='minor'?'#FFD600':s==='critical'?'#FF3355':'#555';
  const sl = s => s==='good'?'GOOD':s==='minor'?'MINOR':s==='critical'?'CRITICAL':'N/A';
  const ir = (k,val) => `<div style="margin-bottom:9px"><div style="font-size:10px;font-weight:800;letter-spacing:1px;text-transform:uppercase;color:#3a5e38">${k}</div><div style="font-size:13px;font-weight:800;color:#d4ead0;font-family:Courier New,monospace;margin-top:1px">${val||'—'}</div></div>`;

  let cl = '';
  SCHEMA.forEach(sec => {
    cl += `<tr style="background:#0c1a0e"><td colspan="3" style="padding:8px 14px;font-weight:900;font-size:12px;letter-spacing:2px;color:#4AFF1F;text-transform:uppercase;border-bottom:1px solid #1e3020">${sec.label}</td></tr>`;
    sec.items.forEach((item,idx) => {
      const dt = S.data[item.id]; const st = dt?.status||'N/A';
      cl += `<tr style="background:${idx%2===0?'#07100a':'#0b1710'}">
        <td style="padding:8px 14px;font-size:13px;color:#d4ead0;border-bottom:1px solid #1a2e1c;width:50%">${item.lbl}</td>
        <td style="padding:8px 14px;border-bottom:1px solid #1a2e1c;width:20%"><span style="background:${sc(st)}20;color:${sc(st)};border:1px solid ${sc(st)}55;padding:3px 10px;border-radius:12px;font-size:11px;font-weight:900;letter-spacing:1px">${sl(st)}</span></td>
        <td style="padding:8px 14px;font-size:12px;color:#6a9e68;border-bottom:1px solid #1a2e1c">${dt?.comment||''}</td>
      </tr>`;
    });
  });

  return `<div style="background:#020c04;color:#edfae8;font-family:'Helvetica Neue',Helvetica,Arial,sans-serif;width:860px">
    <div style="background:#071209;padding:26px 34px;border-bottom:3px solid #4AFF1F">
      <div style="display:flex;justify-content:space-between;align-items:flex-start">
        <div>
          <div style="font-size:26px;font-weight:900;letter-spacing:3px;color:#4AFF1F;text-shadow:0 0 18px rgba(74,255,31,.4);text-transform:uppercase">FLEET<span style="color:#edfae8;font-weight:300">Guard</span> PRO</div>
          <div style="font-size:11px;letter-spacing:2px;color:#3a5e38;text-transform:uppercase;margin-top:4px">Women's Choice Quality Waters</div>
          <div style="font-size:13px;font-weight:800;color:#8eb88a;margin-top:6px">VEHICLE INSPECTION REPORT</div>
        </div>
        <div style="text-align:right">
          <div style="background:${d.hasCrit?'#FF3355':'#4AFF1F'};color:${d.hasCrit?'#fff':'#000'};padding:10px 20px;border-radius:10px;font-weight:900;font-size:13px;letter-spacing:1px">${d.hasCrit?'⛔ CRITICAL':'✅ COMPLETE'}</div>
          <div style="font-family:Courier New,monospace;font-size:11px;color:#4AFF1F;margin-top:9px;background:rgba(74,255,31,.07);border:1px solid rgba(74,255,31,.2);padding:5px 10px;border-radius:5px">${d.reportId}</div>
          <div style="font-size:11px;color:#3a5e38;margin-top:5px">${d.date} · ${d.time}</div>
        </div>
      </div>
    </div>
    <div style="display:grid;grid-template-columns:1fr 1fr 1fr;border-bottom:1px solid #1f361f">
      <div style="padding:18px 22px;background:#071209;border-right:1px solid #1f361f"><div style="font-size:10px;font-weight:900;letter-spacing:2px;text-transform:uppercase;color:#4AFF1F;margin-bottom:11px">🚗 Vehicle</div>${ir('Reg',d.vReg)}${ir('Make',d.vMake)}${ir('Model',d.vModel)}${ir('Year',d.vYear)}${ir('Type',d.vType)}${ir('Mileage',d.vMileage)}${ir('Colour',d.vColor)}</div>
      <div style="padding:18px 22px;background:#071209;border-right:1px solid #1f361f"><div style="font-size:10px;font-weight:900;letter-spacing:2px;text-transform:uppercase;color:#4AFF1F;margin-bottom:11px">👤 Driver</div>${ir('Name',d.dName)}${ir('Licence',d.dLicense)}${ir('Contact',d.dContact)}</div>
      <div style="padding:18px 22px;background:#071209"><div style="font-size:10px;font-weight:900;letter-spacing:2px;text-transform:uppercase;color:#4AFF1F;margin-bottom:11px">🔍 Inspector</div>${ir('Name',d.iName)}${ir('Badge',d.iBadge)}${ir('Location',d.iLocation)}${ir('Date',d.date)}${ir('Time',d.time)}</div>
    </div>
    <div><div style="padding:11px 22px;background:#0c1a0e;border-bottom:1px solid #1f361f"><span style="font-size:11px;font-weight:900;letter-spacing:2px;text-transform:uppercase;color:#4AFF1F">📝 Inspection Checklist</span></div>
    <table style="width:100%;border-collapse:collapse"><thead><tr style="background:#071209"><th style="padding:8px 14px;text-align:left;font-size:10px;font-weight:900;letter-spacing:1px;text-transform:uppercase;color:#3a5e38;border-bottom:1px solid #1f361f">Item</th><th style="padding:8px 14px;text-align:left;font-size:10px;font-weight:900;letter-spacing:1px;text-transform:uppercase;color:#3a5e38;border-bottom:1px solid #1f361f">Status</th><th style="padding:8px 14px;text-align:left;font-size:10px;font-weight:900;letter-spacing:1px;text-transform:uppercase;color:#3a5e38;border-bottom:1px solid #1f361f">Notes</th></tr></thead><tbody>${cl}</tbody></table></div>
    <div style="margin:20px;border-radius:11px;padding:17px 22px;text-align:center;background:${d.hasCrit?'rgba(255,51,85,.08)':'rgba(74,255,31,.06)'};border:2px solid ${d.hasCrit?'#FF3355':'#4AFF1F'}">
      <div style="font-size:18px;font-weight:900;letter-spacing:3px;color:${d.hasCrit?'#FF3355':'#4AFF1F'}">${d.hasCrit?'⛔ CRITICAL ISSUES IDENTIFIED':'✅ INSPECTION COMPLETE'}</div>
    </div>
    <div style="margin:0 20px 20px;background:rgba(74,255,31,.06);border:1px solid rgba(74,255,31,.18);border-radius:10px;padding:14px 18px;display:flex;align-items:center;gap:13px">
      <div style="width:36px;height:36px;background:#4AFF1F;border-radius:8px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg viewBox="0 0 24 24" fill="none" stroke="#000" stroke-width="3" width="19" height="19"><polyline points="20 6 9 17 4 12"/></svg></div>
      <div><div style="font-size:10px;font-weight:900;letter-spacing:1.5px;text-transform:uppercase;color:#3a5e38">Electronically Certified</div><div style="font-size:14px;font-weight:800;color:#4AFF1F;margin-top:2px">${d.iName} · ${d.iBadge}</div><div style="font-size:11px;color:#3a5e38;margin-top:2px">Date: ${d.date}  ·  Time: ${d.time}</div></div>
    </div>
    <div style="background:#071209;border-top:1px solid #1f361f;padding:11px 22px;display:flex;justify-content:space-between">
      <span style="font-family:Courier New,monospace;font-size:10px;color:#3a5e38">© Melato Tatu / Graphiccafe PTY LTD — Women's Choice Quality Waters</span>
      <span style="font-family:Courier New,monospace;font-size:10px;color:#3a5e38">${d.reportId}</span>
    </div>
  </div>`;
}

/* ═════════════════════════════════════
   DOWNLOAD IMAGE
═════════════════════════════════════ */
async function downloadImage(fmt) {
  const btn  = g(`dl-${fmt}-btn`);
  const orig = btn.innerHTML;
  btn.innerHTML = '<span class="spin"></span>'; btn.disabled = true;
  const container = g('report-render');
  container.innerHTML = buildReportHTML();
  container.style.cssText = 'position:fixed;left:-9999px;top:0;width:860px;display:block;background:#020c04;z-index:-999';
  try {
    await new Promise(r => setTimeout(r, 150));
    const canvas = await html2canvas(container, {scale:2,useCORS:true,allowTaint:true,backgroundColor:'#020c04',logging:false,width:860});
    const d = buildRD();
    const fname = `${d.vReg.replace(/\s/g,'_')}_${d.date}_${d.iName.replace(/\s+/g,'_')}.${fmt}`;
    const mime  = fmt==='png'?'image/png':'image/jpeg';
    const url   = fmt==='png'?canvas.toDataURL(mime):canvas.toDataURL(mime,0.93);
    const a = document.createElement('a'); a.href = url; a.download = fname;
    document.body.appendChild(a); a.click(); document.body.removeChild(a);
    toast(`✓ ${fmt.toUpperCase()} saved`);
  } catch(err) {
    toast('Export failed — try again', true); console.error(err);
  } finally {
    container.innerHTML = ''; container.style.display = 'none';
    btn.innerHTML = orig; btn.disabled = false;
  }
}

/* ═════════════════════════════════════
   DOWNLOAD TXT
═════════════════════════════════════ */
function downloadTXT() {
  const d = buildRD(), now = new Date().toISOString();
  const H = '═'.repeat(64), h2 = '─'.repeat(64);
  const lines = [
    H,'  FLEETGUARD PRO — VEHICLE INSPECTION LOG',
    "  Women's Choice Quality Waters",H,'',
    `  Report ID    : ${d.reportId}`,
    `  Generated    : ${now}`,
    `  Date         : ${d.date}`,
    `  Time         : ${d.time}`,
    `  Result       : ${d.verdict}`,'',
    h2,'  VEHICLE INFORMATION',h2,
    `  Registration : ${d.vReg}`,`  Make         : ${d.vMake}`,
    `  Model        : ${d.vModel}`,`  Year         : ${d.vYear}`,
    `  Type         : ${d.vType}`,`  Mileage      : ${d.vMileage}`,
    `  Colour       : ${d.vColor}`,'',
    h2,'  DRIVER INFORMATION',h2,
    `  Full Name    : ${d.dName}`,`  Licence No.  : ${d.dLicense}`,
    `  Contact      : ${d.dContact}`,'',
    h2,'  INSPECTOR INFORMATION',h2,
    `  Full Name    : ${d.iName}`,`  Badge / ID   : ${d.iBadge}`,
    `  Location     : ${d.iLocation}`,`  Date         : ${d.date}`,
    `  Time         : ${d.time}`,'',
    h2,'  INSPECTION CHECKLIST',h2,
  ];
  SCHEMA.forEach(sec => {
    lines.push('',`  [ ${sec.label.toUpperCase()} ]`,'');
    sec.items.forEach(item => {
      const dt = S.data[item.id];
      const st = dt?.status ? dt.status.toUpperCase() : 'NOT ASSESSED';
      const pad = ' '.repeat(Math.max(0, 40 - item.lbl.length));
      lines.push(`    ${item.lbl}${pad}: ${st}`);
      if (dt?.comment) lines.push(`    ${' '.repeat(42)}Note: ${dt.comment}`);
    });
  });
  lines.push('',H,`  VERDICT: ${d.verdict}`,H,'',
    `  ELECTRONICALLY CERTIFIED BY: ${d.iName} (${d.iBadge})`,
    `  Certification Date / Time  : ${d.date} at ${d.time}`,'',
    h2,'  © 2025 Melato Tatu / Graphiccafe PTY LTD',
    "  Developed exclusively for Women's Choice Quality Waters",
    `  FleetGuard Pro v6.0 — All Rights Reserved`,
    `  Log generated: ${now}`,h2);

  const blob = new Blob([lines.join('\r\n')], {type:'text/plain;charset=utf-8'});
  const url  = URL.createObjectURL(blob);
  const fname = `${d.vReg.replace(/\s/g,'_')}_${d.date}_${d.iName.replace(/\s+/g,'_')}.txt`;
  const a = document.createElement('a'); a.href = url; a.download = fname;
  document.body.appendChild(a); a.click(); document.body.removeChild(a);
  URL.revokeObjectURL(url);
  saveHist({id:d.reportId,date:d.date,time:d.time,vehicle:`${d.vMake} ${d.vModel}`,reg:d.vReg,year:d.vYear,driver:d.dName,inspector:d.iName,badge:d.iBadge,hasCritical:d.hasCrit,timestamp:Date.now()});
  updateDash(); renderHistory();
  toast('✓ TXT log downloaded');
}

/* ═════════════════════════════════════
   RESET
═════════════════════════════════════ */
function confirmReset() { const el = g('reset-modal'); if (el) el.classList.add('open'); }
function closeModal(id) { const el = g(id); if (el) el.classList.remove('open'); }

function resetForm() {
  ['v-reg','v-year','v-make','v-model','v-mileage','v-color','d-name','d-license','d-contact','i-name','i-badge','i-location','i-date','i-time'].forEach(id => { const e=g(id); if(e) e.value=''; });
  const vt = g('v-type'); if (vt) vt.value = '';
  const vp = g('veh-prev'); if (vp) vp.style.display = 'none';
  S.certified = false;
  const chk = g('cert-chk'); if (chk) chk.checked = false;
  const row = g('cert-row'); if (row) { row.classList.remove('cert-done','cert-err'); }
  const info = g('cert-info'); if (info) info.classList.remove('show');
  const cerr = g('cert-err-msg'); if (cerr) cerr.classList.remove('show');
  const cnd = g('cert-name-disp'); if (cnd) cnd.textContent = 'the inspector';

  SCHEMA.flatMap(s => s.items).forEach(item => {
    S.data[item.id] = {status:null, comment:'', images:[]};
    document.querySelectorAll(`.sbtn[data-it="${item.id}"]`).forEach(b => b.classList.remove('on'));
    const ta = g(`cmt-${item.id}`); if (ta) ta.value = '';
    const pv = g(`prv-${item.id}`); if (pv) pv.innerHTML = '';
    const it = g(`itm-${item.id}`); if (it) it.className = 'iitem';
  });
  SCHEMA.forEach(sec => {
    const b  = g(`bdg-${sec.id}`); if (b) b.textContent = `0/${sec.items.length}`;
    const el = g(`sec-${sec.id}`); if (el) el.className = 'isec';
  });
  document.querySelectorAll('.field.err').forEach(el => el.classList.remove('err'));
  const mb = g('miss-banner'); if (mb) mb.classList.remove('show');
  const rb = g('res-banner');  if (rb) rb.style.display = 'none';
  const rc = g('v-reg-c');     if (rc) rc.textContent = '0/15';
  newReportId(); updateProgress(); checkReady();
}

/* ═════════════════════════════════════
   THEME
═════════════════════════════════════ */
function toggleMode(el) {
  el.classList.toggle('on');
  if (el.classList.contains('on')) { document.body.removeAttribute('data-mode'); localStorage.setItem('fg_mode','dark'); }
  else { document.body.setAttribute('data-mode','light'); localStorage.setItem('fg_mode','light'); }
}
function loadTheme() {
  if (localStorage.getItem('fg_mode') === 'light') {
    document.body.setAttribute('data-mode','light');
    const tog = g('dark-tog'); if (tog) tog.classList.remove('on');
  }
}

/* ═════════════════════════════════════
   STORAGE
═════════════════════════════════════ */
function saveHist(e){ const h=getHist(); h.push(e); try{localStorage.setItem('fg_hist',JSON.stringify(h));}catch(x){} }
function getHist(){ try{return JSON.parse(localStorage.getItem('fg_hist')||'[]');}catch{return [];} }
function cleanOld(){ const cut=Date.now()-7*24*60*60*1000; try{localStorage.setItem('fg_hist',JSON.stringify(getHist().filter(h=>h.timestamp>cut)));}catch(e){} }
function clearAll(){ if(!confirm('Delete ALL stored inspection records?'))return; localStorage.removeItem('fg_hist'); updateDash(); renderHistory(); toast('All records cleared'); }

/* ═════════════════════════════════════
   DASHBOARD
═════════════════════════════════════ */
function updateDash() {
  const hist = getHist(), today = new Date().toISOString().split('T')[0];
  g('s-total').textContent = hist.length;
  g('s-comp').textContent  = hist.filter(h => !h.hasCritical).length;
  g('s-crit').textContent  = hist.filter(h => h.hasCritical).length;
  g('s-today').textContent = hist.filter(h => h.date === today).length;
  const el = g('home-recent'), last = [...hist].reverse().slice(0,4);
  if (!last.length) { el.innerHTML = '<div style="font-size:15px;color:var(--fg2);padding:12px 0;text-align:center">No inspections yet — tap Inspect to begin</div>'; return; }
  el.innerHTML = last.map(h => `
    <div style="display:flex;align-items:center;gap:11px;padding:10px 0;border-bottom:1px solid var(--b1)">
      <div style="width:9px;height:9px;border-radius:50%;background:${h.hasCritical?'var(--red)':'var(--acc)'};box-shadow:0 0 7px ${h.hasCritical?'rgba(255,51,85,.4)':'var(--acc-glow)'};flex-shrink:0"></div>
      <div style="flex:1;min-width:0">
        <div style="font-size:clamp(13px,3vw,15px);font-weight:800;overflow:hidden;text-overflow:ellipsis;white-space:nowrap">${h.vehicle} · ${h.reg}</div>
        <div style="font-size:clamp(11px,2.5vw,13px);color:var(--fg2);margin-top:2px">${h.date} ${h.time} · ${h.driver||'—'} → ${h.inspector}</div>
      </div>
      <div style="font-size:10px;font-weight:900;padding:3px 9px;border-radius:20px;flex-shrink:0;background:${h.hasCritical?'rgba(255,51,85,.12)':'var(--acc-faint)'};color:${h.hasCritical?'var(--red)':'var(--acc)'}">
        ${h.hasCritical?'CRITICAL':'COMPLETE'}
      </div>
    </div>`).join('');
}

/* ═════════════════════════════════════
   HISTORY
═════════════════════════════════════ */
function renderHistory() {
  const list = g('hist-list'); if (!list) return;
  const hist = [...getHist()].reverse();
  if (!hist.length) {
    list.innerHTML = `<div class="empty"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg><h3>No Inspections Yet</h3><p>Completed inspections appear here for 7 days.</p></div>`;
    return;
  }
  list.innerHTML = hist.map(h => `
    <div class="hcard"><div class="hrow">
      <div class="hico">${h.hasCritical?'⛔':'✅'}</div>
      <div class="hinfo">
        <div class="hveh">${h.vehicle}</div>
        <div class="hreg">${h.reg}${h.year?' · '+h.year:''}</div>
        <div class="hmeta">${h.date} ${h.time}${h.driver?' · Driver: '+h.driver:''}</div>
        <div class="hmeta">Inspector: ${h.inspector} · ${h.badge}</div>
        <div class="hrid">${h.id}</div>
      </div>
      <div class="hstat ${h.hasCritical?'critical':'complete'}">${h.hasCritical?'CRITICAL':'COMPLETE'}</div>
    </div></div>`).join('');
}

/* ═════════════════════════════════════
   NAVIGATION
═════════════════════════════════════ */
function switchTab(tab) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nb').forEach(b => b.classList.remove('active'));
  const pg = g(`page-${tab}`); if (pg) pg.classList.add('active');
  const nb = document.querySelector(`.nb[data-t="${tab}"]`); if (nb) nb.classList.add('active');
  if (tab === 'history') renderHistory();
  if (tab === 'home') { updateDash(); setGreeting(); }
}

/* ═════════════════════════════════════
   TOAST
═════════════════════════════════════ */
let _tt = null;
function toast(msg, isErr = false) {
  const el = g('toast');
  el.textContent = msg;
  el.classList.toggle('err', isErr);
  el.classList.add('show');
  clearTimeout(_tt);
  _tt = setTimeout(() => el.classList.remove('show'), 3200);
}
</script>
</body>
</html>
