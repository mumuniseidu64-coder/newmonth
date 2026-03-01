# newmonth
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>New Month Flow</title>
<style>
body { font-family: Arial; text-align: center; margin-top: 80px; background: #f4f4f4; }
.box { background: white; padding: 25px; border-radius: 10px; width: 90%; max-width: 400px; margin: auto; box-shadow: 0 0 10px rgba(0,0,0,0.2); }
button { padding: 10px 15px; margin: 8px; border-radius: 5px; border: none; cursor: pointer; font-size: 16px; }
.yes { background: #00b894; color: white; }
.no { background: #d63031; color: white; }
.option { background: #0984e3; color: white; }
</style>
</head>
<body>

<div class="box">
<h3>🌸 Happy New Month 🌸</h3>
<p>Wishing you peace, happiness and success this month 😊</p>

<p>Are you still in a relationship with the person you told me about?</p>
<button class="yes" onclick="stillRelationship()">Yes</button>
<button class="no" onclick="notRelationship()">No</button>

<p id="content"></p>
</div>

<script>
function stillRelationship() {
    document.getElementById("content").innerHTML =
        "I understand 😊 I respect that. May you always be happy.";
}

function notRelationship() {
    document.getElementById("content").innerHTML =
        "Oh, I see 😄<br><br>Now that the way is clear, I’m ready… will you accept me?<br><br>" +
        "<button class='yes' onclick='acceptMe()'>Yes</button>" +
        "<button class='no' onclick='noAccept()'>No</button>";
}

function acceptMe() {
    document.getElementById("content").innerHTML =
        "Yay! 😄 I’m so happy!<br><br>Now, a bigger question… will you marry me in the future?<br><br>" +
        "<button class='yes' onclick='marryYes()'>Yes</button>" +
        "<button class='no' onclick='marryNo()'>No</button>";
}

function noAccept() {
    document.getElementById("content").innerHTML =
        "I respect your decision 😊<br><br>Thank you for your honesty.";
}

function marryYes() {
    document.getElementById("content").innerHTML =
        "Wow 😄! Congratulations to us!<br><br>Looking forward to a beautiful future together 💕";
}

function marryNo() {
    document.getElementById("content").innerHTML =
        "I understand 😊 No pressure. I appreciate your honesty.";
}
</script>

</body>
</html>
