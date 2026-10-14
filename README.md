# STOCK-FALSOS-
Código base para control de stock falso".
<!DOCTYPE html>
<html lang="es"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>FAKE STOCK NOCTURNO</title>
<style>
:root{box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);--bg:#ffffff;--card:#fff;--tx:#1f2347;--mut:#667;--bd:#dde1f0;--yel:#ffe600;--blue:#3483fa;--navy:#2d3277;--r:#d93a4a;--g:#0a9a55;--sh:0 1px 3px rgba(31,35,71,.08),0 4px 14px rgba(31,35,71,.05)}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--tx);font-family:"Proxima Nova",system-ui,-apple-system,"Segoe UI",Roboto,sans-serif}
header{background:#fff;padding:10px 16px;display:flex;align-items:center;gap:14px;position:sticky;top:env(safe-area-inset-top,0px);z-index:5;border-bottom:3px solid var(--navy);box-shadow:0 5px 0 var(--yel)}
.lgo{display:flex}header img{height:40px;width:auto;display:block;border-radius:6px}
header .tt{line-height:1.2;min-width:0}header b{display:block;font-size:13px;color:var(--navy);font-weight:800;letter-spacing:.06em}header small{font-size:11px;color:#667;letter-spacing:.04em}
header .id{margin-left:auto;font-size:12px;font-weight:700;color:var(--navy);background:var(--yel);padding:6px 11px;border-radius:999px}
main{max-width:560px;margin:0 auto;padding:18px 16px 40px}
.hide{display:none!important}
.card{background:var(--card);border:1px solid var(--bd);border-radius:12px;box-shadow:var(--sh);padding:20px;margin-bottom:16px}
.hero{background:#fff;border:2px solid var(--navy);color:var(--navy);border-radius:12px;padding:22px 20px;margin-bottom:16px;position:relative;overflow:hidden;box-shadow:0 5px 0 var(--yel)}
.hero:after{content:"";position:absolute;right:-30px;top:-30px;width:120px;height:120px;border-radius:50%;background:var(--yel);opacity:.9}
.hero h1{color:var(--navy);margin:0 0 6px;font-size:23px;position:relative;z-index:1;max-width:80%}.hero p{margin:0;color:#556;font-size:14px;position:relative;z-index:1;max-width:80%}
h1{font-size:22px;font-weight:700;margin:2px 0 4px;color:var(--tx)}h2{font-size:17px;font-weight:700;margin:0 0 10px}
.ctx{color:var(--mut);font-size:14px;margin:0 0 16px;text-transform:capitalize}.ctx::first-letter{}
label{display:block;font-size:12px;font-weight:700;color:var(--navy);letter-spacing:.05em;margin:16px 0 6px}label:first-child{margin-top:0}label i{color:var(--r);font-style:normal}
.f{width:100%;padding:13px;font-size:16px;border-radius:8px;border:1px solid #c9cde0;background:var(--card);color:var(--tx);font-family:inherit}
.f:focus{outline:2px solid var(--navy);border-color:var(--navy)}
.btn{width:100%;padding:15px;border:0;border-radius:8px;background:var(--navy);color:#fff;font-size:15px;font-weight:700;letter-spacing:.03em;margin-top:18px;font-family:inherit;box-shadow:0 2px 0 var(--yel)}
.btn:disabled{background:#c5c8d8;box-shadow:none}
.back{background:none;border:0;color:var(--navy);font-size:14px;font-weight:600;padding:4px 0;margin-bottom:8px;font-family:inherit}
.cards3{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:16px}
.pc{background:var(--card);border:1px solid var(--bd);border-radius:12px;box-shadow:var(--sh);padding:16px 4px 12px;text-align:center;color:var(--tx);font-family:inherit;position:relative;overflow:hidden}
.pc span{font-size:11px;font-weight:700;letter-spacing:.05em;min-height:28px;display:flex;align-items:center;justify-content:center;color:var(--mut)}
.pc b{display:block;font-size:34px;font-weight:700;margin-top:6px;color:var(--r)}
.pc.zero b{color:var(--g)}
.pc.on{border-color:var(--navy);box-shadow:0 0 0 2px var(--navy)}.pc.on span{color:var(--navy)}
.pc.on:before{content:"";position:absolute;left:0;right:0;top:0;height:5px;background:var(--yel)}
.tbl{overflow:hidden;animation:sd .3s ease}
@keyframes sd{from{opacity:0;transform:translateY(-12px)}to{opacity:1;transform:none}}
.tbl .card{padding:0;overflow:hidden}
table{width:100%;border-collapse:collapse;font-size:14px}
th{background:var(--navy);color:#fff;text-align:left;padding:12px;font-size:11px;font-weight:700;letter-spacing:.06em}
td{padding:13px 12px;border-top:1px solid var(--bd)}tbody tr:nth-child(even){background:rgba(45,50,119,.04)}
td.u{font-weight:700;font-variant-numeric:tabular-nums}
.tg{font-size:11px;font-weight:700;padding:4px 9px;border-radius:999px;background:rgba(45,50,119,.1);color:var(--navy);white-space:nowrap}
.alert{display:flex;gap:12px;align-items:flex-start;border:1px solid var(--bd);border-left:5px solid var(--r);background:var(--card);border-radius:12px;box-shadow:var(--sh);padding:14px;margin-top:6px}
.alert.ok{border-left-color:var(--g)}
.alert p{margin:0;font-size:14px;line-height:1.45;color:var(--mut)}.alert b{display:block;font-size:15px;margin-bottom:2px;color:var(--tx)}
.ai{flex:none;width:28px;height:28px;border-radius:50%;background:var(--r);color:#fff;font-weight:800;display:flex;align-items:center;justify-content:center}.ok .ai{background:var(--g)}
.note{font-size:12px;color:var(--mut);text-align:center;margin-top:16px}
.bar{height:6px;background:var(--bd);border-radius:3px;overflow:hidden;margin-bottom:8px}.bar div{height:100%;background:var(--navy);transition:width .3s}
.stp{font-size:12px;font-weight:600;color:var(--mut);letter-spacing:.04em;margin-bottom:14px;text-transform:uppercase}
.ico{width:48px;height:48px;border-radius:50%;background:var(--navy);color:var(--yel);display:flex;align-items:center;justify-content:center;font-size:22px;font-weight:800;margin-bottom:14px}
.tc{border-top:5px solid var(--yel)}.tc p{font-size:15px;line-height:1.6;margin:0;color:var(--mut)}
.end{text-align:center;padding:38px 22px;border-top:5px solid var(--yel)}
.end .ico{margin:0 auto 20px;width:72px;height:72px;font-size:36px;background:var(--g);color:#fff}
.end p{font-size:16px;font-weight:700;line-height:1.6;letter-spacing:.03em;margin:0}
footer{text-align:center;font-size:11px;color:var(--mut);padding:0 16px 24px;letter-spacing:.05em}
.ctl{padding:14px}
.seg{display:flex;background:#eef0f8;border-radius:8px;padding:3px;margin-bottom:12px}
.seg button{flex:1;border:0;background:none;padding:10px;font-size:12px;font-weight:700;letter-spacing:.08em;color:var(--mut);border-radius:6px;font-family:inherit}
.seg button.on{background:var(--navy);color:#fff}
.nav{display:flex;align-items:center;justify-content:space-between;gap:8px}
.nav span{font-weight:700;font-size:15px;text-align:center}
.nav button{width:40px;height:40px;border-radius:8px;border:1px solid var(--bd);background:var(--card);color:var(--navy);font-size:22px;font-family:inherit}
.nav button:disabled{opacity:.3}
.cal{display:grid;grid-template-columns:repeat(7,1fr);gap:5px;margin-top:12px}
.cal button{border:1px solid var(--bd);background:var(--card);border-radius:8px;padding:7px 0 6px;color:var(--tx);font-family:inherit;display:flex;flex-direction:column;align-items:center;gap:3px}
.cal small{font-size:10px;font-weight:700;color:var(--mut);letter-spacing:.04em}
.cal em{font-style:normal;font-size:16px;font-weight:700}
.cal u{text-decoration:none;font-size:11px;font-weight:700;min-width:20px;height:20px;line-height:20px;border-radius:10px;background:var(--r);color:#fff}
.cal u.z{background:rgba(10,154,85,.15);color:var(--g)}
.cal button.tod{border-color:var(--navy)}
.cal button.on{background:var(--navy);border-color:var(--navy);color:#fff}.cal button.on small{color:#c9cdf0}
.cal button.fut{opacity:.35}
.hint{font-size:12px;color:var(--mut);text-align:center;margin:12px 0 0}
.deco{position:fixed;inset:0;z-index:0;pointer-events:none;overflow:hidden}
.deco svg{position:absolute;inset:0;width:100%;height:100%}
.deco img{position:absolute;left:50%;top:52%;width:min(80vw,460px);transform:translate(-50%,-50%);opacity:.07}
main,footer{position:relative;z-index:1}
#splash{position:fixed;inset:0;z-index:100;background:#fff;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:24px;overflow:hidden;transition:opacity .9s ease,visibility .9s}
#splash.out{opacity:0;visibility:hidden}
#splash svg{position:absolute;inset:0;width:100%;height:100%}
#splash .lg{position:relative;width:min(62vw,300px);opacity:0;transform:scale(.8);animation:lgin 1.1s .2s cubic-bezier(.2,.8,.2,1) forwards}
@keyframes lgin{to{opacity:1;transform:none}}
#splash h2{position:relative;margin:22px 0 0;font-size:clamp(26px,8vw,40px);font-weight:800;letter-spacing:.08em;color:var(--navy);display:flex;flex-wrap:wrap;justify-content:center}
#splash h2 span{opacity:0;transform:translateY(14px);animation:chin .5s forwards}
@keyframes chin{to{opacity:1;transform:none}}
#splash .ln{position:relative;height:6px;width:0;background:var(--yel);border-radius:3px;margin-top:12px;animation:lnin 1s 1.6s ease forwards}
@keyframes lnin{to{width:min(60vw,260px)}}
#splash small{position:relative;margin-top:16px;font-size:11px;letter-spacing:.2em;color:#889;opacity:0;animation:chin .6s 2.2s forwards}
</style></head><body>
<div id="splash"><svg viewBox="0 0 400 800" preserveAspectRatio="xMidYMid slice" fill="none"><circle cx="370" cy="110" r="95" stroke="#2d3277" stroke-width="2" opacity=".22"/><circle cx="370" cy="110" r="62" fill="#ffe600" opacity=".55"/><circle cx="25" cy="720" r="120" stroke="#2d3277" stroke-width="2" opacity=".2"/><circle cx="25" cy="720" r="70" stroke="#ffe600" stroke-width="10" opacity=".7"/><path d="M420 560 L270 720M420 600 L240 780" stroke="#ffe600" stroke-width="4" opacity=".8"/></svg>
<img class="lg" id="sl" alt="Mercado Libre"><h2 id="sh" aria-label="Bienvenidos"></h2><div class="ln"></div><small>FAKE STOCK NOCTURNO</small></div>
<header><div class="lgo"><img src="data:image/png;base64,LOGO_ENCABEZADO_BASE64" alt="Mercado Libre"></div><div class="tt"><b>FAKE STOCK NOCTURNO</b><small>MERCADO LIBRE · OPERACIONES</small></div><span class="id hide" id="idtag"></span></header>
<div class="deco" aria-hidden="true"><svg viewBox="0 0 400 800" preserveAspectRatio="xMidYMid slice" fill="none">
<circle cx="370" cy="110" r="95" stroke="#2d3277" stroke-width="2" opacity=".22"/><circle cx="370" cy="110" r="62" fill="#ffe600" opacity=".55"/>
<circle cx="25" cy="720" r="120" stroke="#2d3277" stroke-width="2" opacity=".2"/><circle cx="25" cy="720" r="70" stroke="#ffe600" stroke-width="10" opacity=".7"/><circle cx="95" cy="640" r="22" fill="#2d3277" opacity=".18"/>
<path d="M-20 300 L140 140M-20 340 L180 140" stroke="#2d3277" stroke-width="2" opacity=".14"/><path d="M420 560 L270 720M420 600 L240 780" stroke="#ffe600" stroke-width="4" opacity=".8"/><path d="M420 520 L300 640" stroke="#2d3277" stroke-width="2" opacity=".18"/>
</svg><img src="data:image/png;base64,LOGO_MARCA_DE_AGUA_BASE64" alt=""></div>
<main>

<section class="view" id="v0">
<div class="hero"><h1>Fake Stock Nocturno</h1><p>Consulta los fake stock levantados en tu operación.</p></div>
<div class="card">
<label for="gid">INGRESA TU ID GROOT <i>*</i></label>
<input class="f" id="gid" placeholder="Escribe o escanea tu ID" autocomplete="off" autocapitalize="characters">
<label for="proc">PROCESO <i>*</i></label>
<select class="f" id="proc"><option value="">Selecciona un proceso</option><option value="venta">Picking venta</option><option value="transfer">Picking Transfer</option></select>
<button class="btn" id="go" disabled>Continuar</button>
</div></section>

<section class="view hide" id="v1">
<button class="back" id="b1">‹ Cambiar proceso</button>
<h1>Picking venta</h1><div class="card ctl" id="ctl"></div>
<div class="cards3" id="cards"></div>
<div id="tw"></div>
<div id="al"></div>
<p class="note" id="upd"></p>
</section>

<section class="view hide" id="v2">
<button class="back" id="b2">‹ Cambiar proceso</button>
<h1>Picking Transfer</h1>
<div class="card" style="text-align:center;color:var(--mut)">Aún no hay data de fake stock para Picking Transfer.<br>Próximamente disponible.</div>
</section>

<section class="view hide" id="v3">
<button class="back" id="b3">‹ Volver a mis stock falsos</button>
<div class="bar"><div id="pb"></div></div><p class="stp" id="st"></p>
<div class="card tc" id="tc"></div>
<button class="btn" id="nx">Siguiente</button>
</section>

<section class="view hide" id="v4"><div class="card end"><div class="ico">✓</div><p>AGRADECEMOS TU PARTICIPACIÓN EN ESTA CAPACITACIÓN. TE DESEAMOS EL MAYOR DE LOS ÉXITOS EN TUS PRÓXIMOS TURNOS.</p></div>
<button class="btn" id="rv">Volver a ver mis stock falsos</button>
<p class="note">Si tienes dudas, revisa tus stock falsos junto con tu team.</p></section>
</main>
<footer>FAKE STOCK NOCTURNO</footer>
<script>
// ===== DATA (ejemplo). Reemplazar luego por la fuente en línea =====
var DATA_URL=""; // JSON con la misma estructura; se consulta cada minuto
function ago(n){var d=new Date();d.setDate(d.getDate()-n);return d.getFullYear()+'-'+('0'+(d.getMonth()+1)).slice(-2)+'-'+('0'+d.getDate()).slice(-2)}
var DATA=[
{fecha:ago(0),hora:"06:15",ubicacion:"MZ-P1-A04-R12",proceso:"Picking venta"},
{fecha:ago(0),hora:"07:40",ubicacion:"RS-P1-B07-R05",proceso:"Continuo"},
{fecha:ago(0),hora:"08:05",ubicacion:"MZ-P2-A11-R03",proceso:"Pick to ship"},
{fecha:ago(0),hora:"09:30",ubicacion:"RS-P2-B02-R08",proceso:"Picking venta"},
{fecha:ago(0),hora:"10:10",ubicacion:"RS-P0-A09-R14",proceso:"Continuo"},
{fecha:ago(1),hora:"07:05",ubicacion:"MZ-P3-C15-R01",proceso:"Picking venta"},
{fecha:ago(1),hora:"12:20",ubicacion:"RS-P1-B03-R10",proceso:"Pick to ship"},
{fecha:ago(2),hora:"09:45",ubicacion:"MZ-P2-A06-R02",proceso:"Continuo"},
{fecha:ago(3),hora:"14:30",ubicacion:"RS-P2-B12-R07",proceso:"Picking venta"},
{fecha:ago(3),hora:"15:10",ubicacion:"MZ-P1-A01-R09",proceso:"Picking venta"},
{fecha:ago(5),hora:"08:00",ubicacion:"MZ-P3-C04-R11",proceso:"Pick to ship"},
{fecha:ago(8),hora:"10:25",ubicacion:"RS-P0-A02-R03",proceso:"Continuo"}
];
var TRAIN=[
["1","Escanea primero la ubicación","Antes de tomar cualquier producto, escanea la etiqueta de la ubicación (MZ o RS) y confirma que coincide con la que indica tu RF."],
["2","Verifica el producto","Compara el SKU y la descripción con lo que muestra el RF. Si no coinciden, no confirmes el picking."],
["3","Cuenta la cantidad real","Confirma físicamente la cantidad que tomas. Nunca asumas ni ingreses una cantidad sin contarla."],
["4","Reporta diferencias de inmediato","Si la ubicación está vacía o hay diferencia de unidades, repórtalo en el RF y avisa a tu líder. No sustituyas por otra ubicación."],
["5","Cierra bien cada movimiento","Deja el producto en su posición correcta y escanea cada movimiento. Un buen proceso evita el fake stock."]
];
// ====================================================================
var ID="",sel=null,tstep=0,total=0;
var PROCS=["CONTINUO","PICKING VENTA","PICK TO SHIP"],NAMES={"CONTINUO":"Continuo","PICKING VENTA":"Picking venta","PICK TO SHIP":"Pick to ship"};
function $(i){return document.getElementById(i)}
function show(id){[].forEach.call(document.querySelectorAll('.view'),function(v){v.classList.add('hide')});$(id).classList.remove('hide');window.scrollTo(0,0)}
function chk(){var v=$('gid').value.trim()&&$('proc').value;$('go').disabled=!v}
$('gid').addEventListener('input',chk);$('proc').addEventListener('change',chk);
$('gid').addEventListener('keydown',function(e){if(e.key==='Enter'){e.preventDefault();$('proc').focus()}});
$('go').onclick=function(){ID=$('gid').value.trim().toUpperCase();$('idtag').textContent='ID '+ID;$('idtag').classList.remove('hide');
 if($('proc').value==='venta'){sel=null;MODE='dia';ANCH=ago(0);SELD=null;render();show('v1')}else show('v2')};
$('b1').onclick=$('b2').onclick=function(){show('v0')};
var MODE='dia',ANCH=ago(0),SELD=null;
var DN=['dom','lun','mar','mié','jue','vie','sáb'],MN=['ene','feb','mar','abr','may','jun','jul','ago','sep','oct','nov','dic'];
function pd(s){var p=s.split('-');return new Date(+p[0],+p[1]-1,+p[2])}
function fd(d){return d.getFullYear()+'-'+('0'+(d.getMonth()+1)).slice(-2)+'-'+('0'+d.getDate()).slice(-2)}
function addD(s,n){var d=pd(s);d.setDate(d.getDate()+n);return fd(d)}
function wk(s){var d=pd(s),k=(d.getDay()+6)%7;return addD(s,-k)}
function sh(s){var d=pd(s);return DN[d.getDay()]+' '+('0'+d.getDate()).slice(-2)+'/'+('0'+(d.getMonth()+1)).slice(-2)}
function range(){if(MODE==='dia')return[ANCH];if(SELD)return[SELD];var w=wk(ANCH),r=[];for(var i=0;i<7;i++)r.push(addD(w,i));return r}
function rows(){var r=range();return DATA.filter(function(x){return r.indexOf(x.fecha)>=0})}
function cnt(p){return rows().filter(function(r){return r.proceso===NAMES[p]}).length}
function ctl(){
 var T=ago(0),h='<div class="seg"><button data-m="dia" class="'+(MODE==='dia'?'on':'')+'">DÍA</button><button data-m="semana" class="'+(MODE==='semana'?'on':'')+'">SEMANA</button></div>';
 if(MODE==='dia'){var d=pd(ANCH);h+='<div class="nav"><button data-n="-1">‹</button><span>'+(ANCH===T?'Hoy · ':'')+DN[d.getDay()]+' '+d.getDate()+' '+MN[d.getMonth()]+' '+d.getFullYear()+'</span><button data-n="1" '+(ANCH>=T?'disabled':'')+'>›</button></div>'}
 else{var w=wk(ANCH),e=addD(w,6),a=pd(w),b=pd(e);
  h+='<div class="nav"><button data-n="-7">‹</button><span>'+a.getDate()+' '+MN[a.getMonth()]+' – '+b.getDate()+' '+MN[b.getMonth()]+' '+b.getFullYear()+'</span><button data-n="7" '+(wk(T)<=w?'disabled':'')+'>›</button></div><div class="cal">';
  for(var i=0;i<7;i++){var s=addD(w,i),n=DATA.filter(function(x){return x.fecha===s}).length,dd=pd(s);
   h+='<button data-d="'+s+'" class="'+(SELD===s?'on ':'')+(s>T?'fut ':'')+(s===T?'tod':'')+'" '+(s>T?'disabled':'')+'><small>'+DN[dd.getDay()].toUpperCase()+'</small><em>'+dd.getDate()+'</em><u class="'+(n?'':'z')+'">'+(s>T?'':n)+'</u></button>'}
  h+='</div><p class="hint">'+(SELD?'Mostrando '+sh(SELD)+' · toca de nuevo para ver toda la semana':'Mostrando toda la semana · toca un día para ver su detalle')+'</p>'}
 var c=$('ctl');c.innerHTML=h;
 [].forEach.call(c.querySelectorAll('[data-m]'),function(b){b.onclick=function(){MODE=b.dataset.m;SELD=null;if(MODE==='dia'&&ANCH>T)ANCH=T;render()}});
 [].forEach.call(c.querySelectorAll('[data-n]'),function(b){b.onclick=function(){ANCH=addD(ANCH,+b.dataset.n);SELD=null;render()}});
 [].forEach.call(c.querySelectorAll('[data-d]'),function(b){b.onclick=function(){SELD=SELD===b.dataset.d?null:b.dataset.d;render()}})}
function render(){
 ctl();var all=rows();total=all.length;
 $('cards').innerHTML='';
 PROCS.forEach(function(p){var n=cnt(p),b=document.createElement('button');b.className='pc'+(n?'':' zero')+(sel===p?' on':'');b.innerHTML='<span>'+p+'</span><b>'+n+'</b>';
  b.onclick=function(){sel=p;render();var t=$('tw');if(t.scrollIntoView)t.scrollIntoView({behavior:'smooth',block:'nearest'})};$('cards').appendChild(b)});
 var tw=$('tw'),multi=range().length>1;
 if(sel){var r=all.filter(function(x){return x.proceso===NAMES[sel]}).sort(function(a,b){return(b.fecha+b.hora).localeCompare(a.fecha+a.hora)});
  tw.innerHTML='<div class="tbl"><div class="card"><table><thead><tr><th>UBICACIÓN</th><th>'+(multi?'FECHA Y HORA':'HORA DEL LEVANTAMIENTO')+'</th><th>PROCESO</th></tr></thead><tbody>'+
  (r.length?r.map(function(x){return '<tr><td class="u">'+x.ubicacion+'</td><td>'+(multi?sh(x.fecha)+' · ':'')+x.hora+' h</td><td><span class="tg">'+x.proceso+'</span></td></tr>'}).join(''):'<tr><td colspan="3" style="text-align:center;color:var(--mut)">Sin fake stock en este proceso</td></tr>')+'</tbody></table></div></div>';
 }else tw.innerHTML='';
 var lab=MODE==='dia'?'en este día':(SELD?'en este día':'en esta semana');
 $('al').innerHTML=total>2?'<div class="alert"><span class="ai">!</span><p><b>Capacitación obligatoria</b>Tienes '+total+' fake stock levantados '+lab+'. Debes completar una breve capacitación.</p></div><button class="btn" id="tr">Ir a la capacitación</button>':
  '<div class="alert ok"><span class="ai">✓</span><p><b>Sin acción requerida</b>Tienes '+total+' fake stock '+lab+'. ¡Sigue así!</p></div>';
 if($('tr'))$('tr').onclick=function(){tstep=0;train();show('v3')};
 $('upd').textContent='Actualizado '+new Date().toTimeString().slice(0,5)+(DATA_URL?'':' · datos de ejemplo');
}
function train(){var t=TRAIN[tstep],last=tstep===TRAIN.length-1;
 $('pb').style.width=((tstep+1)/TRAIN.length*100)+'%';$('st').textContent='Capacitación · Paso '+(tstep+1)+' de '+TRAIN.length;
 $('tc').innerHTML='<div class="ico">'+t[0]+'</div><h2>'+t[1]+'</h2><p>'+t[2]+'</p>';
 $('nx').textContent=last?'ENTENDIDO':'Siguiente';window.scrollTo(0,0)}
$('rv').onclick=$('b3').onclick=function(){render();show('v1')};
$('nx').onclick=function(){if(tstep<TRAIN.length-1){tstep++;train()}else show('v4')};
function pull(){if(!DATA_URL)return;fetch(DATA_URL).then(function(r){return r.json()}).then(function(d){if(Array.isArray(d)){DATA=d;if(!$('v1').classList.contains('hide'))render()}}).catch(function(){})}
pull();setInterval(pull,60000);
(function(){var h=$('sh'),s='¡BIENVENIDOS!';for(var i=0;i<s.length;i++){var e=document.createElement('span');e.textContent=s[i];e.style.animationDelay=(1.0+i*.07)+'s';h.appendChild(e)}
$('sl').src=document.querySelector('.deco img').src;
var sp=$('splash'),d=false;function end(){if(d)return;d=true;sp.classList.add('out');setTimeout(function(){sp.remove()},1000)}
sp.onclick=end;setTimeout(end,3900)})();
</script></body></html>