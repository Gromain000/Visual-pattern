<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Which card comes next?</title>
<style>
    body {
        margin: 0;
        background: #000;
        font-family: Arial, Helvetica, sans-serif;
        color: #fff;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 40px;
    }

    h1 {
        font-size: 32px;
        font-weight: 600;
        margin-bottom: 25px;
    }

    .panel {
        width: 900px;
        background: #5b5b5b;
        border-radius: 35px;
        padding: 30px 40px;
        display: flex;
        gap: 50px;
    }

    .cards {
        display: flex;
        flex-direction: column;
        gap: 12px;
    }

    .card {
        width: 95px;
        height: 135px;
        border: 2px solid #fff;
        border-radius: 6px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 34px;
        position: relative;
    }

    .card.small {
        font-size: 26px;
    }

    .corner {
        position: absolute;
        font-size: 14px;
        line-height: 1.1;
    }

    .top-left {
        top: 6px;
        left: 6px;
        text-align: left;
    }

    .bottom-right {
        bottom: 6px;
        right: 6px;
        transform: rotate(180deg);
    }

    .labels {
        display: flex;
        flex-direction: column;
        gap: 36px;
        font-size: 30px;
        padding-top: 10px;
    }

    .answers {
        width: 900px;
        margin-top: 40px;
        font-size: 30px;
    }

    .answers div {
        margin: 12px 0;
    }
</style>
</head>
<body>

<h1>Which card comes next?</h1>

<div class="panel">
    <!-- Left card stack -->
    <div class="cards">
        <div class="card">
            <div class="corner top-left">A<br>♠</div>
            ♠
            <div class="corner bottom-right">A<br>♠</div>
        </div>

        <div class="card">
            <div class="corner top-left">2<br>♠</div>
            ♠
            <div class="corner bottom-right">2<br>♠</div>
        </div>

        <div class="card">
            <div class="corner top-left">3<br>♠</div>
            ♠
            <div class="corner bottom-right">3<br>♠</div>
        </div>

        <div class="card">
            <div class="corner top-left">4<br>♠</div>
            ♠ ♠
            <div class="corner bottom-right">4<br>♠</div>
        </div>

        <div class="card small">?</div>
    </div>

    <!-- Right labels -->
    <div class="labels">
        <div>A♠</div>
        <div>2♥</div>
        <div>3♠</div>
        <div>4♥</div>
        <div>?</div>
    </div>
</div>

<div class="answers">
    <div>A) 5♠</div>
    <div>B) 5♥</div>
    <div>C) 6♠</div>
</div>

</body>
</html>
