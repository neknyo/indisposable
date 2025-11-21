---
layout: default
title: App Login
---

<h2>Restricted Area</h2>
<p>Please enter your password to access the tool.</p>

<input type="password" id="pwd" placeholder="Password">
<button onclick="check()">Login</button>
<p id="msg" style="color:red;display:none">Wrong Password</p>

<script>
function check() {
    var p = document.getElementById("pwd").value;
    // CHANGE '1234' TO YOUR PASSWORD
    if (p === "1234") {
        window.location.href = "/app/dashboard.html";
    } else {
        document.getElementById("msg").style.display = "block";
    }
}
</script>
