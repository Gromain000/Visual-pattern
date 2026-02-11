<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Visual Pattern</title>
<style>
    body {
        background-color: black;
        color: white;
        font-family: Arial, sans-serif;
        text-align: center;
        padding-top: 100px;
    }

    .container {
        max-width: 600px;
        margin: auto;
    }

    .question {
        font-size: 28px;
        margin-bottom: 40px;
    }

    .choices {
        text-align: left;
        display: inline-block;
        font-size: 22px;
    }

    .choices label {
        display: block;
        margin: 20px 0;
        cursor: pointer;
    }

    .proceed-btn {
        display: none;
        margin-top: 80px;
        padding: 18px 80px;
        font-size: 28px;
        background-color: #34C759; /* Same green style */
        color: black;
        border: none;
        border-radius: 12px;
        cursor: pointer;
        font-weight: 600;
    }

    .proceed-btn:hover {
        opacity: 0.9;
    }
</style>
</head>
<body>

<div class="container">
    <div class="question">Which card comes next?</div>

    <div class="choices">
        <label><input type="radio" name="answer"> A) 5♠</label>
        <label><input type="radio" name="answer"> B) 5♥</label>
        <label><input type="radio" name="answer"> C) 6♠</label>
    </div>

    <br>

    <button id="proceed" class="proceed-btn">Proceed</button>
</div>

<script>
    const radios = document.querySelectorAll('input[name="answer"]');
    const proceedBtn = document.getElementById('proceed');

    radios.forEach(radio => {
        radio.addEventListener('change', () => {
            proceedBtn.style.display = "inline-block";
        });
    });

    // Optional: redirect when clicked
    // proceedBtn.addEventListener('click', () => {
    //     window.location.href = "nextpage.html";
    // });
</script>

</body>
</html>
