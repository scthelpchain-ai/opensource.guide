
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scthelpchain | International Digital Exchange</title>
    <style>
        body { font-family: 'Segoe UI', Arial, sans-serif; background: radial-gradient(circle, #001f3f, #000c18); color: #fff; text-align: center; margin: 0; padding: 20px; }
        .card { background: rgba(0, 31, 63, 0.8); border: 1px solid #ffd700; border-radius: 15px; padding: 25px; max-width: 500px; margin: 20px auto; box-shadow: 0 0 30px rgba(255, 215, 0, 0.2); backdrop-filter: blur(10px); }
        .gold-text { color: #ffd700; font-size: 28px; font-weight: bold; text-transform: uppercase; letter-spacing: 2px; }
        .btn { display: block; width: 100%; padding: 14px; margin: 12px 0; border-radius: 10px; border: none; font-weight: bold; cursor: pointer; text-decoration: none; font-size: 16px; transition: 0.3s; }
        .btn-fb { background: #1877f2; color: white; }
        .btn-ex { background: #ffd700; color: #000; }
        .btn:hover { opacity: 0.8; transform: scale(1.02); }
        input { width: 90%; padding: 12px; margin: 10px 0; border-radius: 8px; border: 1px solid #ffd700; background: #000; color: #00ff00; font-size: 18px; text-align: center; }
        .address-box { background: rgba(0,0,0,0.6); padding: 15px; font-size: 13px; border: 1px dashed #ffd700; border-radius: 8px; margin: 20px 0; word-break: break-all; }
        .footer { font-size: 12px; color: #aaa; margin-top: 40px; border-top: 1px solid rgba(255,215,0,0.2); padding-top: 20px; }
    </style>
</head>
<body>

    <div class="header">
        <h1 class="gold-text">SCT HELPCHAIN</h1>
        <p style="color: #ffd700; opacity: 0.8;">International Digital Exchange & Charity Platform</p>
    </div>

    <div class="card">
        <a href="https://www.facebook.com/share/1bf8n82KKc/" target="_blank" class="btn btn-fb">Contact on Facebook</a>
        
        <div style="margin: 20px 0;">
            <label style="color: #ffd700;">Exchange Amount (USDT):</label><br>
            <input type="number" id="usdt" placeholder="0.00" oninput="calc()">
            <p id="result" style="color: #00ff00; font-weight: bold; margin-top: 10px;"></p>
        </div>

        <div class="address-box">
            <strong>Payment Address (BEP-20):</strong><br>
            <span style="color: #00ff00;">0x9fdb46c96240a185383e726b914c8d0437cc43cc</span>
        </div>

        <button class="btn btn-ex" onclick="send()">Exchange Request via WhatsApp</button>
    </div>

    <div class="footer">
        &copy; 2026 Scthelpchain International | Purana Paltan, Dhaka<br>
        Developed for Global Financial Assistance
    </div>

    <script>
        const rate = 126.5;
        function calc() {
            let u = document.getElementById('usdt').value;
            let res = document.getElementById('result');
            if(u > 0) { 
                res.innerHTML = "You will receive: " + (u * rate).toFixed(2) + " BDT";
            } else {
                res.innerHTML = "";
            }
        }
        function send() {
            let u = document.getElementById('usdt').value;
            if(u > 0) {
                window.open("https://wa.me/8801410522152?text=Scthelpchain Exchange Request: " + u + " USDT", "_blank");
            } else {
                alert("Please enter USDT amount!");
            }
        }
    </script>

</body>
</html>
