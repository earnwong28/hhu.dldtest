[index.html](https://github.com/user-attachments/files/34950073/index.html)
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>กลุ่มควบคุมป้องกันโรคโค</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Prompt:wght@400;500;600&family=Sarabun:wght@400;600&display=swap">
<style>
:root{--bg:#f6faf7;--surface:#fff;--ink:#17301f;--muted:#566b5d;--line:#d5e3d9;--accent:#1f7a4d;--tag:#e3f3ea;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0e1b14;--surface:#162a1f;--ink:#e8f3ec;--muted:#9fb8a8;--line:#28422f;--accent:#6fd0a0;--tag:#1f3b2b}}
:root[data-theme="dark"]{--bg:#0e1b14;--surface:#162a1f;--ink:#e8f3ec;--muted:#9fb8a8;--line:#28422f;--accent:#6fd0a0;--tag:#1f3b2b}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font-family:Sarabun,system-ui,sans-serif;font-size:17px;line-height:1.6}
h1,h2,h3,.bn b{font-family:Prompt,Sarabun,sans-serif}
.wrap{max-width:960px;margin:0 auto;padding:0 18px}
.hero{padding:36px 0 8px;display:flex;align-items:center;gap:20px}
.hero svg{flex:none;width:84px;height:84px;color:var(--accent)}
.hero p{margin:0;color:var(--muted)}
h1{font-size:clamp(1.6rem,5.5vw,2.4rem);line-height:1.25;margin:2px 0 6px;font-weight:600}
.search{margin:16px 0 4px}
.search input{width:100%;padding:14px 18px;font:inherit;border:2px solid var(--line);border-radius:999px;background:var(--surface);color:var(--ink)}
.search input:focus{outline:3px solid var(--accent);border-color:var(--accent)}
h2{font-size:1.25rem;margin:36px 0 14px;font-weight:600}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:14px}
.bn{position:relative;display:flex;flex-direction:column;justify-content:flex-end;min-height:150px;padding:18px;border-radius:22px;color:#fff;text-decoration:none;background:linear-gradient(135deg,var(--c),var(--c2));background-size:cover;background-position:center;overflow:hidden;transition:transform .15s,box-shadow .15s}
.bn:hover,.bn:focus-visible{transform:translateY(-3px);box-shadow:0 10px 22px rgba(0,0,0,.22);outline:none}
.bn:focus-visible{box-shadow:0 0 0 4px var(--surface),0 0 0 7px var(--accent)}
.bn.has-img::before{content:"";position:absolute;inset:0;background:linear-gradient(transparent 25%,rgba(0,0,0,.7))}
.bn>*{position:relative}
.bn .ic{position:absolute;top:14px;right:14px;width:54px;height:54px;border-radius:50%;background:rgba(255,255,255,.22);display:grid;place-items:center}
.bn .ic svg{width:30px;height:30px}
.bn b{font-size:1.15rem;font-weight:600;line-height:1.3}
.bn span{font-size:.92rem;opacity:.95}
.new{position:absolute;top:14px;left:14px;background:#ffd23f;color:#3a2c00;border-radius:999px;padding:1px 12px;font-size:.85rem;font-weight:600}
.item{background:var(--surface);border:1px solid var(--line);border-radius:18px;padding:16px;margin:0 0 12px}
.item h3{font-size:1.02rem;margin:0 0 8px;font-weight:500}
.code{display:inline-block;background:var(--tag);border-radius:999px;padding:0 12px;font-size:.85rem;margin-bottom:6px}
.links{display:flex;flex-wrap:wrap;gap:8px}
.links a{padding:6px 14px;border-radius:999px;border:1.5px solid var(--accent);color:var(--accent);text-decoration:none;font-size:.95rem}
.links a:first-child{background:var(--accent);color:var(--surface)}
.links a:hover,.links a:focus-visible{outline:3px solid var(--accent);outline-offset:2px}
.contact{background:var(--surface);border:1px solid var(--line);border-radius:18px;padding:18px}
.contact a{color:var(--accent)}
footer{margin:40px 0 40px;color:var(--muted);font-size:.9rem}
footer a{color:var(--accent)}
.none{color:var(--muted);display:none}
@media (prefers-reduced-motion:reduce){.bn{transition:none}}
</style>
</head>
<body>
<div class="wrap">
<div class="hero">
  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M4 6l3 3M20 6l-3 3"/><rect x="6" y="8" width="12" height="11" rx="5"/><circle cx="10" cy="12" r=".6"/><circle cx="14" cy="12" r=".6"/><ellipse cx="12" cy="16" rx="3" ry="2"/></svg>
  <div><p>สำนักควบคุม ป้องกันและบำบัดโรคสัตว์</p><h1>กลุ่มควบคุมป้องกันโรคโค</h1></div>
</div>
<div class="search"><input id="q" type="search" placeholder="ค้นหาโครงการ เช่น ลัมปี สกิน, บรูเซลลา, R2001" aria-label="ค้นหาโครงการ"></div>

<h2>เมนูหลัก</h2>
<div class="grid" id="banners"></div>

<div id="main"></div>
<p class="none" id="none">ไม่พบโครงการที่ตรงกับคำค้น</p>

<h2>ติดต่อเรา</h2>
<div class="contact">กลุ่มควบคุมป้องกันโรคโค<br>โทร <a href="tel:026534444">02-653-4444</a> ต่อ 4165<br><a href="mailto:dcontrol13@dld.go.th">dcontrol13@dld.go.th</a></div>
<footer>หน้านี้รวบรวมลิงก์จากไซต์หลักเพื่อเปิดได้สะดวก สิทธิ์เข้าถึงไฟล์เป็นไปตามต้นฉบับ · <a href="https://sites.google.com/view/bdcvs-dart/%E0%B8%AB%E0%B8%99%E0%B8%B2%E0%B9%81%E0%B8%A3%E0%B8%81">ไซต์ต้นฉบับ</a></footer>
</div>
<script>
var D="https://drive.google.com/drive/folders/";
var sections=[
{t:"โครงการปีงบประมาณ 2569",items:[
 {n:"โครงการสำรวจความชุกและเฝ้าระวังโรคปากและเท้าเปื่อยในพื้นที่เสี่ยง",c:"R2601",l:[["โฟลเดอร์โครงการ",D+"16WRGLHAZq4Ip3-Zsdn_9FeGdmSg-ohPv"],["บันทึกข้อมูล","https://shorturl.at/yLC3C"]]},
 {n:"โครงการเฝ้าระวังโรคลัมปี สกิน",c:"R1601",l:[["โฟลเดอร์โครงการ",D+"12X5K3h52rHj9wgnqgC48gYQBXbAd1CHy"],["ข้อมูล","https://gqr.sh/CRkg"]]},
 {n:"โครงการตรวจติดตามระดับภูมิคุ้มกันโรคปากและเท้าเปื่อยในโคนม",c:"R2001",l:[["โฟลเดอร์โครงการ",D+"10XJfzXLtjRDqh8JKJwpP_-ZlYkRakmKs"],["บันทึกข้อมูล","https://shorturl.at/GEqFk"]]},
 {n:"โครงการตรวจติดตามระดับภูมิคุ้มกันโรคปากและเท้าเปื่อยในโคเนื้อ",c:"R2701",l:[["โฟลเดอร์โครงการ",D+"1urkIjGaJlM8uV6PF2Q1g0d7h6ZUx_HuX"],["บันทึกข้อมูล","https://shorturl.at/KCuvi"]]},
 {n:"โครงการเฝ้าระวังโรคปากและเท้าเปื่อยซีโรไทป์ SAT1 และ SAT2 ในพื้นที่เสี่ยง",c:"R2201",l:[["โฟลเดอร์โครงการ",D+"1Ezi0qfnPooce2Ijx_baHjpZLDaYDmDum"],["บันทึกข้อมูล","https://docs.google.com/spreadsheets/d/1Ibti1toxm_AXmtyvPDQlTzeaw7Z_bRI-DTfeSkut5Ys/edit"]]}
]},
{t:"วัณโรคและบรูเซลลา ปี 2569",items:[
 {n:"การทดสอบวัณโรคในโค และสัตว์ในหน่วยราชการกรมปศุสัตว์",l:[["บันทึกข้อมูล กำหนดเป้าหมายและทดสอบวัณโรค",D+"1r-VJDXQNPea23m2zKklokrSf09HNs18K"]]},
 {n:"โครงการเฝ้าระวังและกำจัดโรคบรูเซลลาในโคนมโดยตรวจคัดกรองจากน้ำนมดิบ (BRU-Milk) เชียงใหม่–นครราชสีมา",c:"R0101",l:[["เชียงใหม่",D+"1MdNygpzxeWWuiWjfKiAGK97ezmo1HCjy"],["นครราชสีมา",D+"1N7S8aD9Knbap-eTP-GKAzubD7RB_lxS5"],["อัพโหลดสรุปโครงการ",D+"12JlP745C8Of0Mr6B5tRNifSGolbiNmIr"],["แบบสอบสวนโรคบรูเซลลา","https://drive.google.com/file/d/1uyjfieh204RVB6ofG34f2CIAWL4FLDfQ/view"]]},
 {n:"โครงการเฝ้าระวังและทดสอบโรคบรูเซลลาในฟาร์ม GFM (BRU-Serum)",c:"R2801",l:[["โครงการฯ และเป้าหมาย",D+"1Ub83iGnBgl9Mc_S_tpy-qfxedM0OqZf_"],["หนังสือ แบบสอบสวนโรค และแบบฟอร์ม",D+"1NMq9hZj1RKS8229jpxcI1YOChsbaFgoe"],["คำแนะนำการบันทึกข้อมูล","https://docs.google.com/document/d/1562mjb-LRK4cfDA8CrwCek9dEJqsMkR6GM-DQmCbHNE/edit"],["อัพโหลดสรุปโครงการ",D+"14BHda6MjMy2Gg0AG3OAvCEh2HXH9WNGS"]]}
]},
{t:"โครงการปีงบประมาณ 2568",items:[
 {n:"โครงการตรวจติดตามระดับภูมิคุ้มกันโรคปากและเท้าเปื่อยในโคนม",c:"R2001",l:[["โฟลเดอร์โครงการ",D+"1_Sl1YiFpoaXlmMkvwDI27_M24wQ0Wuxv"],["ส่วนบันทึกข้อมูล","https://docs.google.com/spreadsheets/d/1kYTTOzN7JZQ-jfi8GfvBwXT95VIB1jdVaVpqveME13Y/edit"]]},
 {n:"โครงการสำรวจความชุกและติดตามภูมิคุ้มกันโรคปากและเท้าเปื่อยหลังฉีดวัคซีนในลูกโคนม",c:"R1801",l:[["โฟลเดอร์โครงการ",D+"1qApQOMI3lrfgbVsL4qlLYunNnMIT4xDa"],["ส่วนบันทึกข้อมูล","https://docs.google.com/spreadsheets/d/1nyClpWZ6wvZybYrXzulx_01KeJCFhFaly1vljbmZBBI/edit"]]},
 {n:"โครงการสำรวจความชุกโรคพยาธิในเลือดและพยาธิทางเดินอาหารโค",c:"R1901",l:[["ส่วนบันทึกข้อมูล","https://docs.google.com/spreadsheets/d/1mRtJVrPbysM5FGCgBsjkt2nxhNYtpUIYiqfO1qM-kZA/edit"]]},
 {n:"โครงการเฝ้าระวังและกำจัดโรคบรูเซลลาในโคนม พื้นที่ปศุสัตว์เขต 1, 3 และ 7",l:[["หนังสือแจ้งหน่วยงาน",D+"1RPc4tEmIk8L5U7_UIKgAa4JUEnpSpQbV"],["โครงการฯ 2568",D+"1fmJDbGjyncMLUyo3cHpzgnDeuhQ_nzHG"],["ลพบุรี",D+"1zTnobRyDsfMR07FRAEBOn7ZB9U6p44_p"],["สระบุรี",D+"1Sgtf6cR3tPtbtaNDKuKIQe3JIuOducEL"],["นครราชสีมา",D+"1PuMnldn6Ymc5aZEmaZE-AUpYaXk-OIMo"],["ประจวบคีรีขันธ์",D+"1TmQ_JhLQu2ezP3C0pQH9LwBxfWYwx3kY"],["กาญจนบุรี",D+"1BRPd_BUJyi4qx2IkK1yV11ZcV-qCytlz"],["นครปฐม",D+"1_KcSFfwUD9yplMRJs9VWh4skHMw0eZAf"],["ราชบุรี",D+"1ZMGdRU0TbPnRASGDHjmqQhIahkyFWWEJ"],["เพชรบุรี",D+"1Yzc0pumtu1p46oC5zuoV4-XOIs6a68wB"]]}
]},
{t:"หน่วย DART (หน่วยควบคุมโรคและช่วยเหลือภัยพิบัติด้านสุขภาพสัตว์)",items:[
 {n:"เอกสารการปฏิบัติงาน ปี 2568",l:[["หนังสือแจ้งแผนการปฏิบัติงาน",D+"1dSIxk-azvJpmpCXAQIu3NlsmEJanmR5S"],["แบบฟอร์มรายงานผล (Excel)","https://docs.google.com/spreadsheets/d/15Tw-UBij0jbpuGbx6w_L7tx4IOT2X2Md/edit"],["สรุปรายงานประจำเดือน (Word)","https://docs.google.com/document/d/1qEJjcPOeXCxruiIRmRUjyRB3oZopL6y2/edit"]]}
]},
{t:"โรคลัมปี สกิน (LSD)",items:[
 {n:"ไซต์ข้อมูลโรคลัมปี สกิน",l:[["โรคลัมปี สกิน (LSD)","https://sites.google.com/view/lsddld/home"],["GFM","https://sites.google.com/view/gfmdld"]]},
 {n:"การทดสอบวัณโรคในโคนม ปี 2568",l:[["หนังสือต่าง ๆ",D+"1JtdNJ9y4KcnF8ino6k8InvKu8PQG9gBY"],["กำหนดเป้าหมาย",D+"1HLd0sB_9-ybZpvY_rhvS1vp4FDgUkGQD"],["สรุปเป้าหมายและแผนจัดสรร",D+"1q3mEEEmTE_m04Mo0818KZggptp_7kdbp"],["บันทึกผลการทดสอบ",D+"1Mz4KpnsbP2ZsQbwqKRy9Ye7mwaHLlHWN"]]}
]}
];

// แบนเนอร์เมนูหลัก: ใส่ลิงก์รูปในช่อง img (เช่น "images/vaccine.jpg") เพื่อใช้รูปจริงเป็นพื้นหลัง
var I={
 syringe:'<path d="M18 2l4 4M17 7l3-3M19 9l-8.7 8.7a2.8 2.8 0 01-4 0l-.3-.3a2.8 2.8 0 010-4L14.7 4.7M6 15l-3 3M9 12l3 3M11 10l3 3"/>',
 cow:'<path d="M4 6l3 3M20 6l-3 3"/><rect x="6" y="8" width="12" height="11" rx="5"/><circle cx="10" cy="12" r=".6"/><circle cx="14" cy="12" r=".6"/><ellipse cx="12" cy="16" rx="3" ry="2"/>',
 box:'<path d="M21 8l-9-5-9 5 9 5 9-5zM3 8v8l9 5 9-5V8M12 13v8"/>',
 chart:'<path d="M4 20V10M10 20V4M16 20v-8M22 20H2"/>',
 check:'<rect x="5" y="4" width="14" height="17" rx="2"/><path d="M9 12l2 2 4-4"/>',
 shield:'<path d="M12 3l8 3v6c0 5-3.5 8-8 9-4.5-1-8-4-8-9V6l8-3z"/><path d="M9 12l2 2 4-4"/>',
 virus:'<circle cx="12" cy="12" r="4"/><path d="M12 3v3M12 18v3M3 12h3M18 12h3M5.6 5.6l2.1 2.1M16.3 16.3l2.1 2.1M18.4 5.6l-2.1 2.1M7.7 16.3l-2.1 2.1"/>',
 home:'<path d="M3 11l9-7 9 7v9H3z"/><path d="M9 20v-6h6v6"/>'
};
var banners=[
 {t:"การรณรงค์ฉีดวัคซีน",s:"FMD และ LSD",u:D+"1u8-ql3TogKya_rkcevJnbjntnPjoRq8F",i:"syringe",c:"#1f7a4d",c2:"#34a56b",img:""},
 {t:"การสำรวจประชากรโคนม",s:"ข้อมูลฟาร์มและจำนวนโค",u:D+"1EY_JyGfeAadxycz74C2C4iCQV4Ss3ua1",i:"cow",c:"#1f6fb2",c2:"#3d93d8",img:""},
 {t:"การจัดสรรวัคซีนป้องกัน",s:"แผนและจำนวนที่จัดสรร",u:D+"1remB-I-rvG7IPvAMEmMa5SfXA16LakDE",i:"box",c:"#b4540f",c2:"#e07a2a",img:""},
 {t:"ตัวชี้วัดโคนม",s:"ดูผลงานและตัวชี้วัด",u:D+"1SVXrPmfWYw3AQrNCuGsoY-ECbciwLB0V",i:"chart",c:"#6a4fb3",c2:"#8f74d6",img:""},
 {t:"การติดตามการฉีดวัคซีน",s:"ติดตามผลล่าสุด",u:D+"1iYfbwGQ9-gxfmgXpi8cF5MUyaz568WYy",i:"check",c:"#0f766e",c2:"#2aa198",img:"",n:1},
 {t:"โรคลัมปี สกิน (LSD)",s:"สื่อประชาสัมพันธ์ ความรู้ และมาตรการ",u:"https://sites.google.com/view/lsddld/home",i:"virus",c:"#a63446",c2:"#d4566a",img:""},
 {t:"GFM",s:"ฟาร์มที่มีการจัดการที่ดี",u:"https://sites.google.com/view/gfmdld",i:"home",c:"#4d7a1f",c2:"#7ba83a",img:""},
 {t:"หน่วย DART",s:"แผนและรายงานการปฏิบัติงาน",u:D+"1dSIxk-azvJpmpCXAQIu3NlsmEJanmR5S",i:"shield",c:"#2c5282",c2:"#4a78b5",img:""}
];
document.getElementById("banners").innerHTML=banners.map(function(b){
 var st='--c:'+b.c+';--c2:'+b.c2+(b.img?';background-image:url('+b.img+')':'');
 return '<a class="bn'+(b.img?' has-img':'')+'" style="'+st+'" href="'+b.u+'" target="_blank" rel="noopener">'+(b.n?'<i class="new" style="font-style:normal">อัปเดตใหม่</i>':'')+'<div class="ic"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">'+I[b.i]+'</svg></div><b>'+b.t+'</b><span>'+b.s+'</span></a>';
}).join("");
function a(p){return '<a href="'+p[1]+'" target="_blank" rel="noopener">'+p[0]+'</a>'}
document.getElementById("main").innerHTML=sections.map(function(s){
 return '<section><h2>'+s.t+'</h2>'+s.items.map(function(i){
  return '<div class="item" data-k="'+(i.n+' '+(i.c||'')+' '+s.t).toLowerCase()+'">'+(i.c?'<span class="code">รหัส LIMS '+i.c+'</span>':'')+'<h3>'+i.n+'</h3><div class="links">'+i.l.map(a).join("")+'</div></div>';
 }).join("")+'</section>';
}).join("");
document.getElementById("q").addEventListener("input",function(e){
 var k=e.target.value.trim().toLowerCase(),shown=0;
 document.querySelectorAll("#main section").forEach(function(sec){
  var n=0;
  sec.querySelectorAll(".item").forEach(function(it){var ok=!k||it.dataset.k.indexOf(k)>-1;it.style.display=ok?"":"none";if(ok)n++});
  sec.style.display=n?"":"none";shown+=n;
 });
 document.getElementById("none").style.display=shown?"none":"block";
});
</script>
</body>
</html>
