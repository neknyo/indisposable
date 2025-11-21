---
title: "App Login"
---

<div id="login-box" style="text-align:center; margin-top:50px;">
    <h2>Restricted Access</h2>
    <input type="password" id="passInput" placeholder="Password..." style="padding:10px;">
    <button onclick="checkPass()" style="padding:10px;">Unlock</button>
    <p id="errorMsg" style="color:red; display:none;">Access Denied</p>
</div>

<script>
    function checkPass() {
        var pass = document.getElementById('passInput').value;
        // ⚠️ REPLACE 'mypass123' WITH YOUR PASSWORD
        if (pass === 'mypass123') {
            // This redirects to the hidden file below
            window.location.href = "/app/secret-tool/"; 
        } else {
            document.getElementById('errorMsg').style.display = 'block';
        }
    }
</script>
