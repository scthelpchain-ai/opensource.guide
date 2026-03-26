

# Open Source Guides
[![Build Status](https://github.com/github/opensource.guide/workflows/GitHub%20Actions%20CI/badge.svg)](https://github.com/github/opensource.guide/actions)

Open Source Guides (https://opensource.guide/) are a collection of resources for individuals, communities, and companies who want to learn how to run and contribute to an open-source project.

## Background
Open Source Guides were created and are curated by GitHub, along with input from outside community reviewers, but they are not exclusive to GitHub products. One reason we started this project is that we felt that there weren't enough resources for people creating open-source projects.

Our goal was to aggregate community best practices, *not* what GitHub (or any other individual or entity) thinks is best. Therefore, we used examples and quotations from others to illustrate our points.

## Contributing

This site is powered by [Jekyll](https://jekyllrb.com/). Check out our [contributing guidelines](/CONTRIBUTING.md) for ways to offer feedback and contribute.

## Licenses

Content is released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). See [notices](notices.md) for complete details, including attribution guidelines, contribution terms, and software and third-party licenses and permissions.

## Acknowledgments

The initial release of these guides was authored by **[@nayafia][1], [@bkeepers][2], [@stephbwills][3],** and **[@mlinksva][4]**.

Thanks to **[@aitchabee][5], [@benbalter][6], [@brettcannon][7], [@caabernathy][8], [@coralineada][9], [@dmleong][10], [@ericholscher][11], [@gr2m][12], [@janl][13], [@jessfraz][14], [@bluesomewhere][15], [@kfogel][16], [@kytrinyx][17], [@lee-dohm][18], [@mikeal][19], [@mikemcquaid][20], [@nathansobo][21], [@nruff][22], [@nsqe][23], [@orta][24], [@parkr][25], [@shazow][26], [@steveklabnik][27],** and **[@wooorm][28]** for lending their valuable input and expertise leading up to the initial release, and to **[@sophshep][29]** and **[@jeejkang][30]** for designing and illustrating the guides.

## Disclaimer
While we've got advice about running an open source project, we're not lawyers. Be sure to read our [disclaimer](notices.md#legal-disclaimer) before diving in.

[1]:https://github.com/nayafia
[2]:https://github.com/bkeepers
[3]:https://github.com/stephbwills
[4]:https://github.com/mlinksva
[5]:https://github.com/aitchabee
[6]:https://github.com/benbalter
[7]:https://github.com/brettcannon
[8]:https://github.com/caabernathy
[9]:https://github.com/CoralineAda
[10]:https://github.com/dmleong
[11]:https://github.com/ericholscher
[12]:https://github.com/gr2m
[13]:https://github.com/janl
[14]:https://github.com/jessfraz
[15]:https://github.com/bluesomewhere
[16]:https://github.com/kfogel
[17]:https://github.com/kytrinyx
[18]:https://github.com/lee-dohm
[19]:https://github.com/mikeal
[20]:https://github.com/MikeMcQuaid
[21]:https://github.com/nathansobo
[22]:https://github.com/nruff
[23]:https://github.com/nsqe
[24]:https://github.com/orta
[25]:https://github.com/parkr
[26]:https://github.com/shazow
[27]:https://github.com/steveklabnik
[28]:https://github.com/wooorm
[29]:https://github.com/sophshep
[30]:https://github.com/jeejkang<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scthelpchain | International Digital Exchange</title>
    <style>
        body { font-family: Arial, sans-serif; background: #000c18; color: #fff; text-align: center; margin: 0; padding: 20px; }
        .card { background: #001f3f; border: 1px solid #ffd700; border-radius: 15px; padding: 25px; max-width: 500px; margin: 20px auto; box-shadow: 0 0 20px rgba(255, 215, 0, 0.3); }
        .gold-text { color: #ffd700; font-size: 24px; font-weight: bold; }
        .btn { display: block; width: 100%; padding: 12px; margin: 10px 0; border-radius: 8px; border: none; font-weight: bold; cursor: pointer; text-decoration: none; }
        .btn-fb { background: #1877f2; color: white; }
        .btn-ex { background: #ffd700; color: #000; }
        input { width: 90%; padding: 10px; margin: 10px 0; border-radius: 5px; border: 1px solid #ffd700; background: #000; color: #00ff00; }
        .footer { font-size: 12px; color: #aaa; margin-top: 30px; }
    </style>
</head>
<body>

    <div class="header">
        <h1 class="gold-text">SCT HELPCHAIN</h1>
        <p>International Digital Exchange & Charity Platform</p>
    </div>

    <div class="card">
        <a href="https://www.facebook.com/share/1AtU1uz1nn/" target="_blank" class="btn btn-fb">Contact on Facebook</a>
        
        <div style="margin: 20px 0;">
            <label>Amount (USDT):</label><br>
            <input type="number" id="usdt" placeholder="Enter USDT" oninput="calc()">
        </div>

        <div style="background: rgba(0,0,0,0.5); padding: 10px; font-size: 12px; border: 1px dashed #ffd700;">
            Payment Address (BEP-20):<br>
            <strong>0x9fdb46c96240a185383e726b914c8d0437cc43cc</strong>
        </div>

        <button class="btn btn-ex" onclick="send()">Exchange Now</button>
    </div>

    <div class="footer">
        &copy; 2026 Scthelpchain | Developed for Global Assistance
    </div>

    <script>
        function calc() {
            let u = document.getElementById('usdt').value;
            if(u > 0) { console.log("Total: " + (u * 126.5) + " BDT"); }
        }
        function send() {
            let u = document.getElementById('usdt').value;
            window.open("https://wa.me/8801410522152?text=Exchange Request: " + u + " USDT", "_blank");
        }
    </script>

</body>
</html>

