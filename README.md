<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>शासकीय उच्चतर माध्यमिक विद्यालय खवासा - परिणाम</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.9.2/html2pdf.bundle.min.js"></script>

<style>
:root {
    --primary-color: #6366f1;
    --secondary-color: #a855f7;
    --success-color: #22c55e;
    --fail-color: #ef4444;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;
    min-height: 100vh;
    margin: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
}

@keyframes gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

.container {
    max-width: 600px;
    width: 100%;
    background: rgba(255, 255, 255, 0.95);
    padding: 30px;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px);
}

h2 {
    text-align: center;
    color: #333;
    margin-bottom: 25px;
    border-bottom: 3px solid var(--primary-color);
    padding-bottom: 10px;
}

select, input {
    width: 100%;
    padding: 12px;
    margin-bottom: 15px;
    border: 2px solid #ddd;
    border-radius: 10px;
    box-sizing: border-box;
    font-size: 16px;
    transition: 0.3s;
}

select:focus, input:focus {
    border-color: var(--primary-color);
    outline: none;
    box-shadow: 0 0 8px rgba(99, 102, 241, 0.3);
}

button {
    width: 100%;
    padding: 14px;
    background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
    color: white;
    border: none;
    border-radius: 10px;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.2s, box-shadow 0.2s;
    margin-bottom: 15px;
}

button:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

button:active { transform: translateY(0); }

.result-box {
    display: none;
    margin-top: 20px;
    padding: 20px;
    border-radius: 15px;
    background: #f8fafc;
    border: 1px solid #e2e8f0;
}

table {
    width: 100%;
    border-collapse: collapse;
    margin: 15px 0;
}

th, td {
    border: 1px solid #e2e8f0;
    padding: 12px;
    text-align: center;
}

th { background: #f1f5f9; color: #475569; }

.status-pass { color: var(--success-color); font-weight: bold; }
.status-fail { color: var(--fail-color); font-weight: bold; }

/* Styles for the Marquee */
.custom-marquee {
    width: 100%;
    background: rgba(0, 0, 0, 0.8);
    color: white;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    left: 0;
    font-weight: bold;
    letter-spacing: 1px;
    border-top: 2px solid var(--secondary-color);
}

.marquee-text {
    background: linear-gradient(to right, #ff8a00, #da1b60, #89fffd, #ef32d9);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 18px;
}
</style>
</head>

<body>

<div class="container">
    <h2>शासकीय उच्चतर माध्यमिक विद्यालय खवासा 🏫<br><span style="font-size: 0.7em; color: #666;">प्री बोर्ड परीक्षा परिणाम</span></h2>

    <select id="classSelect">
        <option value="">कक्षा चुनें</option>
        <option value="10_A">10th A</option>
        <option value="10_B">10th B</option>
        <option value="12_arts">12th Arts</option>
        <option value="12_science">12th Science</option>
    </select>

    <input type="number" id="rollInput" placeholder="Roll Number दर्ज करें">
    <button onclick="getResult()">परिणाम देखें</button>

    <div id="resultBox" class="result-box"></div>

    <button id="downloadBtn" onclick="downloadPDF()" style="display:none; background: var(--success-color);">
        📄 PDF डाउनलोड करें
    </button>
</div>

<div class="custom-marquee">
    <marquee behavior="scroll" direction="left">
        <span class="marquee-text">✨ Designed and Developed by Dheeraj Shrivas | शासकीय उच्चतर माध्यमिक विद्यालय खवासा - आपका उज्जवल भविष्य हमारी प्राथमिकता ✨</span>
    </marquee>
</div>

<script>
// Data remains the same as provided
const results = {
"10_A":{
10001:{name:"",subjects:{IT:{theory:8,practical:13}}},
10004:{name:"",subjects:{IT:{theory:9,practical:9}}},
10005:{name:"",subjects:{IT:{theory:11,practical:13}}},
10006:{name:"",subjects:{IT:{theory:2,practical:13}}},
10007:{name:"",subjects:{IT:{theory:11,practical:13}}},
10009:{name:"",subjects:{IT:{theory:5,practical:13}}},
10010:{name:"",subjects:{IT:{theory:8,practical:13}}},
10011:{name:"",subjects:{IT:{theory:7,practical:13}}},
10015:{name:"",subjects:{IT:{theory:14,practical:13}}},
10016:{name:"",subjects:{IT:{theory:20,practical:13}}},
10017:{name:"",subjects:{IT:{theory:7,practical:13}}},
10018:{name:"",subjects:{IT:{theory:6,practical:13}}},
10019:{name:"",subjects:{IT:{theory:16,practical:30}}},
10020:{name:"",subjects:{IT:{theory:15,practical:13}}},
10021:{name:"",subjects:{IT:{theory:12,practical:14}}},
10022:{name:"",subjects:{IT:{theory:21,practical:13}}},
10023:{name:"",subjects:{IT:{theory:15,practical:13}}},
10025:{name:"",subjects:{IT:{theory:7,practical:13}}},
10032:{name:"",subjects:{IT:{theory:14,practical:13}}},
10033:{name:"",subjects:{IT:{theory:7,practical:13}}},
10034:{name:"7",subjects:{IT:{theory:15,practical:13}}},
10035:{name:"",subjects:{IT:{theory:7,practical:13}}},
10038:{name:"",subjects:{IT:{theory:33,practical:15}}},
10039:{name:"",subjects:{IT:{theory:20,practical:13}}},
10040:{name:"",subjects:{IT:{theory:31,practical:16}}},
10041:{name:"",subjects:{IT:{theory:50,practical:21}}},
10042:{name:"",subjects:{IT:{theory:17,practical:13}}},
10044:{name:"",subjects:{IT:{theory:35,practical:15}}},
10045:{name:"",subjects:{IT:{theory:18,practical:13}}},
10046:{name:"",subjects:{IT:{theory:91,practical:60}}},
10051:{name:"",subjects:{IT:{theory:22,practical:20}}},
10052:{name:"",subjects:{IT:{theory:18,practical:13}}},
10053:{name:"",subjects:{IT:{theory:19,practical:13}}},
10055:{name:"",subjects:{IT:{theory:98,practical:60}}},
10056:{name:"",subjects:{IT:{theory:30,practical:25}}},
10057:{name:"",subjects:{IT:{theory:14,practical:13}}},
10058:{name:"",subjects:{IT:{theory:23,practical:15}}},
10059:{name:"",subjects:{IT:{theory:24,practical:16}}},
10026:{name:"",subjects:{IT:{theory:5,practical:13}}},
10029:{name:"",subjects:{IT:{theory:8,practical:13}}},
10030:{name:"",subjects:{IT:{theory:12,practical:13}}},
10031:{name:"",subjects:{IT:{theory:6,practical:13}}}
},
"10_B":{
202:{name:"Gaurav Singh",subjects:{Physics:{theory:70,practical:10},Chemistry:{theory:68,practical:12},Biology:{theory:72,practical:10},Maths:{theory:65,practical:15},Hindi:{theory:80,practical:10},English:{theory:75,practical:10}}}
},
"12_arts":{
226771058051:{name:"Abhay Singh Awathar",subjects:{Hindi:{theory:95,practical:0},English:{theory:99,practical:0},IT:{theory:98,practical:0},Geography:{theory:92,practical:0},Political:{theory:90,practical:0},Economics:{theory:97,practical:0}}}
},
"12_science":{
12035:{name:"",subjects:{Physics:{theory:28,practical:26},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12036:{name:"",subjects:{Physics:{theory:14,practical:22},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12037:{name:"",subjects:{Physics:{theory:43,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12038:{name:"",subjects:{Physics:{theory:44,practical:29},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12039:{name:"",subjects:{Physics:{theory:23,practical:25},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12040:{name:"",subjects:{Physics:{theory:30,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12041:{name:"",subjects:{Physics:{theory:35,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12042:{name:"",subjects:{Physics:{theory:23,practical:22},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12043:{name:"",subjects:{Physics:{theory:13,practical:22},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12044:{name:"",subjects:{Physics:{theory:33,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12045:{name:"",subjects:{Physics:{theory:34,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12046:{name:"",subjects:{Physics:{theory:23,practical:26},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12047:{name:"",subjects:{Physics:{theory:29,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12048:{name:"",subjects:{Physics:{theory:28,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12049:{name:"",subjects:{Physics:{theory:25,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12050:{name:"",subjects:{Physics:{theory:23,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12051:{name:"",subjects:{Physics:{theory:30,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12052:{name:"",subjects:{Physics:{theory:36,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12053:{name:"",subjects:{Physics:{theory:42,practical:29},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12054:{name:"",subjects:{Physics:{theory:34,practical:28},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12055:{name:"",subjects:{Physics:{theory:23,practical:25},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12056:{name:"",subjects:{Physics:{theory:20,practical:23},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12057:{name:"",subjects:{Physics:{theory:13,practical:22},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12058:{name:"",subjects:{Physics:{theory:25,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}},
12059:{name:"",subjects:{Physics:{theory:25,practical:27},Chemistry:{theory:82,practical:20},Biology:{theory:75,practical:20},Maths:{theory:80,practical:20},Hindi:{theory:70,practical:20},English:{theory:74,practical:20}}}
}
};

function getGrade(t){
if(t>=90)return"A1";
if(t>=80)return"A2";
if(t>=70)return"B1";
if(t>=60)return"B2";
if(t>=50)return"C";
if(t>=33)return"D";
return"F";
}

function getResult(){
const c=document.getElementById('classSelect').value;
const r=document.getElementById('rollInput').value;
const box=document.getElementById('resultBox');
const btn=document.getElementById('downloadBtn');

if(!c||!r){alert("कृपया Class और Roll Number दर्ज करें");return;}
const d=results[c]?.[r];

if(!d){
    box.style.display="block";
    box.innerHTML="<h3 style='color:red; text-align:center;'>❌ रिकॉर्ड नहीं मिला</h3>";
    btn.style.display="none";
    return;
}

let pass=true, html=`<div id="printArea">
    <h3 style="color:#333; margin-top:0;">नाम: ${d.name||"—"}</h3>
    <table>
        <tr><th>विषय</th><th>Theory</th><th>Prac.</th><th>Total</th><th>Grade</th></tr>`;

for(let s in d.subjects){
    let t=d.subjects[s].theory, p=d.subjects[s].practical, total=t+p;
    if(total<33) pass=false;
    html+=`<tr><td>${s}</td><td>${t}</td><td>${p}</td><td>${total}</td><td>${getGrade(total)}</td></tr>`;
}

html+=`</table>
    <h3 style="text-align:center;">Result: <span class="${pass?'status-pass':'status-fail'}">${pass?"✅ उत्तीर्ण (PASS)":"❌ अनुत्तीर्ण (FAIL)"}</span></h3>
    </div>`;

box.innerHTML=html;
box.style.display="block";
btn.style.display="block";
}

function downloadPDF(){
const element = document.getElementById('printArea');
const opt = {
  margin: 10,
  filename: 'Pre_Board_Result.pdf',
  image: { type: 'jpeg', quality: 0.98 },
  html2canvas: { scale: 2 },
  jsPDF: { unit: 'mm', format: 'a4', orientation: 'portrait' }
};
html2pdf().set(opt).from(element).save();
}
</script>

</body>
</html> 

 
