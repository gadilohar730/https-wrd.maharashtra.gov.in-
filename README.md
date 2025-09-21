<!DOCTYPE html>
<html lang="mr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>पाटबंधारे भरती</title>
<style>
body {font-family:"Segoe UI",Arial,sans-serif; margin:0; background:#f0f2f5;}
header {background:linear-gradient(90deg,#d32f2f,#ff5722); color:white; padding:20px 40px; display:flex; justify-content:space-between; align-items:center;}
header h1 {font-size:28px;}
header nav a {color:white; margin-left:20px; text-decoration:none; font-weight:600;}
header nav a:hover {text-decoration:underline;}

.hero {display:flex; flex-direction:column; align-items:center; justify-content:center; background:#ffe0b2; padding:80px 20px; text-align:center; border-bottom:5px solid #d32f2f; border-radius:0 0 50% 50% / 0 0 10% 10%;}
.hero h2 {font-size:36px; color:#d32f2f; margin-bottom:15px;}
.hero p {font-size:18px; margin-bottom:25px;}
.hero button {padding:15px 35px; background:#d32f2f; color:white; border:none; border-radius:50px; cursor:pointer; font-size:16px; font-weight:bold;}
.hero button:hover {background:#b71c1c;}

.notifications {max-width:900px; margin:30px auto; display:flex; gap:20px;}
.notifications .card {flex:1; background:white; padding:20px; border-radius:15px; box-shadow:0 4px 12px rgba(0,0,0,0.1);}
.notifications h3 {color:#d32f2f; margin-bottom:15px;}
.notifications ul {list-style:none; padding-left:0;}
.notifications ul li {padding:8px 0; border-bottom:1px dashed #ccc;}
.notifications ul li:last-child {border-bottom:none;}

.container {max-width:900px; margin:30px auto; background:white; padding:30px; border-radius:20px; box-shadow:0 6px 20px rgba(0,0,0,0.1);}
.container h2 {text-align:center; color:#d32f2f; margin-bottom:30px;}
.step {display:none;}
.step.active {display:block;}
label {display:block; margin-top:12px; font-weight:600;}
input, select {width:100%; padding:12px; margin-bottom:12px; border-radius:10px; border:1px solid #ccc;}
.buttons {text-align:right; margin-top:20px;}
button {padding:10px 20px; margin-left:10px; border:none; border-radius:10px; background:#d32f2f; color:white; cursor:pointer;}
button:hover {background:#b71c1c;}
.preview p {margin:6px 0;}

/* Progress bar */
.progress-container {width:100%; background:#eee; border-radius:10px; margin-bottom:20px;}
.progress-bar {width:0%; height:10px; background:#d32f2f; border-radius:10px;}
footer {background:#333; color:white; text-align:center; padding:20px; margin-top:40px;}
footer a {color:#ffeb3b; text-decoration:none;}
footer a:hover {text-decoration:underline;}
</style>
</head>
<body>

<header>
<h1>पाटबंधारे भरती</h1>
<nav><a href="#">मुख्य पृष्ठ</a><a href="#formSection">अर्ज करा</a><a href="#">सूचना</a><a href="#">संपर्क</a></nav>
</header>

<section class="hero">
<h2>पाटबंधारे भरती 2025</h2>
<p>संपूर्ण अर्ज प्रक्रिया ऑनलाइन भरा आणि PDF मध्ये डाउनलोड करा</p>
<button onclick="document.getElementById('formSection').scrollIntoView({behavior:'smooth'})">अर्ज करा</button>
</section>

<section class="notifications">
<div class="card">
<h3>ताज्या अधिसूचना</h3>
<ul>
<li>पाटबंधारे भरती अर्ज प्रक्रिया सुरु.</li>
<li>अर्ज भरण्याची अंतिम तारीख: 15 ऑक्टोबर 2025.</li>
<li>पात्रतेसाठी आवश्यक कागदपत्रांची यादी.</li>
<li>फॉर्म पूर्ण करण्यासाठी 7 स्टेप्स फॉलो करा.</li>
</ul>
</div>
<div class="card">
<h3>महत्त्वाचे सूचना</h3>
<ul>
<li>सर्व माहिती खरी भरा.</li>
<li>Required fields पूर्ण करा अन्यथा पुढे जाऊ शकत नाही.</li>
<li>Transaction नंतर Application ID मिळेल.</li>
<li>PDF मध्ये डाउनलोड / Print करू शकता.</li>
</ul>
</div>
</section>

<div class="container" id="formSection">
<h2>पाटबंधारे भरती अर्ज फॉर्म</h2>
<div class="progress-container"><div class="progress-bar" id="progressBar"></div></div>
<form id="bhartiForm">

<!-- Step 1 -->
<div class="step active">
<h3>Step 1: उमेदवार नोंदणी</h3>
<label>पूर्ण नाव</label><input type="text" name="fullName" required>
<label>वडिलांचे/आईचे नाव</label><input type="text" name="parentName" required>
<label>जन्मतारीख</label><input type="date" name="dob" required>
<label>मोबाईल नंबर</label><input type="tel" name="mobile" required>
<label>ई-मेल आयडी</label><input type="email" name="email" required>
<label>आधार क्रमांक</label><input type="text" name="aadhaar" required>
</div>

<!-- Step 2 -->
<div class="step">
<h3>Step 2: वैयक्तिक माहिती</h3>
<label>पत्ता</label><input type="text" name="address" required>
<label>लिंग</label><select name="gender" required>
<option value="">निवडा</option><option>पुरुष</option><option>महिला</option><option>इतर</option></select>
<label>जात</label><select name="category" required>
<option value="">निवडा</option><option>Open</option><option>SC</option><option>ST</option><option>OBC</option><option>EWS</option></select>
<label>राष्ट्रीयत्व</label><input type="text" name="nationality" required>
<label>वैवाहिक स्थिती</label><select name="maritalStatus" required>
<option value="">निवडा</option><option>एकल</option><option>विवाहित</option></select>
</div>

<!-- Step 3 -->
<div class="step">
<h3>Step 3: शैक्षणिक माहिती</h3>
<label>10 वी उत्तीर्ण वर्ष, बोर्ड, टक्केवारी</label><input type="text" name="tenth" required>
<label>12 वी उत्तीर्ण वर्ष, बोर्ड, टक्केवारी</label><input type="text" name="twelfth" required>
<label>पदवी / डिप्लोमा / ITI माहिती</label><input type="text" name="graduation">
<label>इतर प्रमाणपत्रे</label><input type="text" name="otherCertificates">
</div>

<!-- Step 4 -->
<div class="step">
<h3>Step 4: कागदपत्र Upload</h3>
<label>आधार कार्ड</label><input type="file" name="aadhaarFile" accept=".jpg,.png,.pdf" required>
<label>पॅन कार्ड</label><input type="file" name="panFile" accept=".jpg,.png,.pdf">
<label>नॉन क्रिमिनल</label><input type="file" name="nonCriminal" accept=".jpg,.png,.pdf">
<label>रहिवासी प्रमाण पत्र</label><input type="file" name="residence" accept=".jpg,.png,.pdf">
<label>पासपोर्ट साईज फोटो</label><input type="file" name="photo" accept=".jpg,.png" required>
<label>स्वाक्षरी</label><input type="file" name="signature" accept=".jpg,.png" required>
<label>शैक्षणिक प्रमाणपत्रे (PDF)</label><input type="file" name="educationFiles" accept=".pdf">
<label>जात प्रमाणपत्र (जर लागू असेल)</label><input type="file" name="casteFile" accept=".pdf">
<label>इतर आवश्यक कागदपत्र</label><input type="file" name="otherDocs" accept=".pdf">
</div>

<!-- Step 5 -->
<div class="step">
<h3>Step 5: फॉर्म Preview</h3>
<div class="preview" id="previewDiv"></div>
</div>

<!-- Step 6 -->
<div class="step">
<h3>Step 6: Payment</h3>
<p>Application Fee: ₹50/-</p>
<p>Account Number: 04023023963</p>
<p>IFSC CODE: JJSB0000005</p>
<p>UPI ID: jhalseva@ybl</p>
<button type="button" onclick="makePayment('PhonePe')">PhonePe</button>
<button type="button" onclick="makePayment('GPay')">GPay</button>
<button type="button" onclick="makePayment('Paytm')">Paytm</button>
<p>Transaction नंतर पुढे जा.</p>
</div>

<!-- Step 7 -->
<div class="step">
<h3>Step 7: Final Submit & Print</h3>
<p>Application ID: <strong id="appId"></strong></p>
<button type="button" onclick="window.print()">Download / Print PDF</button>
</div>

<div class="buttons">
<button type="button" id="prevBtn" onclick="nextPrev(-1)">Back</button>
<button type="button" id="nextBtn" onclick="nextPrev(1)">Next</button>
</div>

</form>
</div>

<footer>
<p>&copy; 2025 पाटबंधारे भरती. सर्व हक्क राखीव. | <a href="#">गोपनीयता धोरण</a></p>
</footer>

<script>
let currentStep = 0;
let paymentDone = false;

showStep(currentStep);

function showStep(n){
    const steps = document.getElementsByClassName("step");
    for(let i=0;i<steps.length;i++){ steps[i].classList.remove("active"); }
    steps[n].classList.add("active");
    document.getElementById("prevBtn").style.display = n==0 ? "none" : "inline";
    document.getElementById("nextBtn").innerHTML = n==(steps.length-1) ? "Submit" : "Next";
    document.getElementById("progressBar").style.width = ((n+1)/7*100) + '%';
    if(n==4) populatePreview();
}

function nextPrev(n){
    const steps = document.getElementsByClassName("step");
    // Payment check
    if(currentStep==5 && !paymentDone){
        alert("कृपया सर्वप्रथम Application Fee ₹50/- भरा.");
        return false;
    }
    if(n==1 && !validateForm()) return false;
    currentStep += n;
    if(currentStep >= steps.length){
        document.getElementById("appId").innerText = "PB" + Math.floor(Math.random()*1000000);
        alert("Arj यशस्वीरित्या सबमिट झाला!");
        return false;
    }
    showStep(currentStep);
}

function validateForm(){
    const step = document.getElementsByClassName("step")[currentStep];
    const inputs = step.getElementsByTagName("input");
    for(let input of inputs){
        if(input.hasAttribute("required") && input.value==""){
            alert("कृपया सर्व required fields भरा.");
            return false;
        }
    }
    return true;
}

function populatePreview(){
    const form = document.getElementById("bhartiForm");
    const preview = document.getElementById("previewDiv");
    preview.innerHTML = "";
    const data = new FormData(form);
    for(let [key,value] of data.entries()){
        preview.innerHTML += `<p><strong>${key}:</strong> ${value.name || value}</p>`;
    }
}

// Payment function
function makePayment(method){
    alert(method + " वर ₹50/- फी भरण्यासाठी redirect");
    paymentDone = true;
}
</script>

</body>
</html>
