# i
 
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>A Little Surprise For You 💐💗</title>

<style>
* {
    box-sizing: border-box;
}

html {
    width: 100%;
    min-height: 100%;
    overflow-x: hidden;
    overflow-y: auto;
}

body {
    width: 100%;
    min-width: 0;
    min-height: 100vh;
    min-height: 100dvh;
    margin: 0;
    padding: 20px;

    display: grid;
    place-items: center;

    overflow-x: hidden;
    overflow-y: auto;

    font-family: "Trebuchet MS", Arial, sans-serif;
    background:
        radial-gradient(circle at top left, #ffd9e7, transparent 35%),
        radial-gradient(circle at bottom right, #ffc4d9, transparent 35%),
        linear-gradient(135deg, #fff0f5, #ffe0eb);

    color: #6b2945;
}

/* =========================
   MAIN CARD
========================= */

.card {
    width: 100%;
    max-width: 450px;
    min-width: 0;

    max-height: 94vh;
    max-height: 94dvh;

    margin: 0 auto;
    padding: 30px 24px;

    position: relative;
    z-index: 10;

    text-align: center;

    overflow-y: auto;
    overflow-x: hidden;

    scrollbar-width: none;

    background: rgba(255, 255, 255, 0.94);

    border: 2px solid rgba(255, 182, 208, 0.75);
    border-radius: 32px;

    box-shadow:
        0 20px 50px rgba(214, 83, 122, 0.25),
        0 5px 15px rgba(214, 83, 122, 0.1);

    backdrop-filter: blur(12px);
}

.card::-webkit-scrollbar {
    display: none;
}

/* =========================
   PAGES
========================= */

.page {
    width: 100%;
    min-width: 0;

    display: none;

    animation: pageIn 0.6s ease forwards;
}

.page.active {
    display: block;
}

@keyframes pageIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* =========================
   TEXT
========================= */

h1 {
    margin: 10px 0;
    color: #d94d7a;
    font-size: clamp(28px, 8vw, 42px);
}

h2 {
    margin: 10px 0;
    color: #d94d7a;
    font-size: clamp(24px, 7vw, 34px);
}

p {
    line-height: 1.7;
    font-size: 16px;
}

/* =========================
   BUTTON
========================= */

button {
    border: none;
    cursor: pointer;

    font-family: inherit;
    font-weight: bold;

    transition:
        transform 0.25s ease,
        box-shadow 0.25s ease,
        background 0.25s ease;
}

.main-btn {
    margin-top: 20px;

    padding: 14px 25px;

    border-radius: 30px;

    background: linear-gradient(
        135deg,
        #ff72a5,
        #e94d7d
    );

    color: white;

    font-size: 16px;

    box-shadow:
        0 8px 20px rgba(221, 74, 119, 0.3);
}

.main-btn:hover {
    transform: translateY(-3px) scale(1.03);

    box-shadow:
        0 12px 25px rgba(221, 74, 119, 0.4);
}

.main-btn:active {
    transform: scale(0.97);
}

/* =========================
   BOUQUET
========================= */

.big-bouquet {
    font-size: clamp(70px, 22vw, 110px);

    margin: 10px auto 5px;

    line-height: 1;

    animation: bouquetFloat 3s ease-in-out infinite;
}

@keyframes bouquetFloat {
    0%,
    100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-10px);
    }
}

.subtitle {
    font-size: 15px;
    color: #a4516d;
}

/* =========================
   ENVELOPE
========================= */

.envelope-area {
    padding: 25px 0;
}

.envelope {
    position: relative;

    width: min(260px, 75vw);
    height: 170px;

    margin: 30px auto;

    background: #ffc3d7;

    border-radius: 10px;

    cursor: pointer;

    box-shadow:
        0 15px 30px rgba(210, 76, 120, 0.2);

    transition:
        transform 0.3s ease,
        box-shadow 0.3s ease;
}

.envelope:hover {
    transform: translateY(-5px);

    box-shadow:
        0 20px 35px rgba(210, 76, 120, 0.3);
}

.envelope::before {
    content: "";

    position: absolute;

    left: 0;
    top: 0;

    width: 0;
    height: 0;

    border-left: 130px solid transparent;
    border-right: 130px solid transparent;
    border-top: 95px solid #ff9fbd;
}

.envelope::after {
    content: "";

    position: absolute;

    left: 0;
    bottom: 0;

    width: 0;
    height: 0;

    border-left: 130px solid transparent;
    border-right: 130px solid transparent;
    border-bottom: 90px solid #ffabc6;
}

.heart-seal {
    position: absolute;

    left: 50%;
    top: 50%;

    transform: translate(-50%, -50%);

    z-index: 3;

    font-size: 40px;
}

/* =========================
   LETTER
========================= */

.letter {
    margin-top: 15px;

    padding: 22px;

    border-radius: 20px;

    background: #fff7fa;

    border: 1px solid #ffd0df;

    text-align: left;

    box-shadow:
        inset 0 0 20px rgba(255, 175, 200, 0.1);
}

.letter h2 {
    text-align: center;
}

.letter p {
    margin: 10px 0;
}

.signature {
    margin-top: 20px;

    text-align: right;

    font-style: italic;

    color: #d94d7a;
}

/* =========================
   TEDDY
========================= */

.teddy {
    font-size: clamp(75px, 22vw, 110px);

    margin: 10px 0;

    animation:
        teddyBounce 2s ease-in-out infinite;
}

@keyframes teddyBounce {
    0%,
    100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-8px);
    }
}

/* =========================
   DATE QUESTION
========================= */

.date-question {
    margin-top: 10px;
}

.date-question h1 {
    margin-bottom: 5px;
}

.date-question p {
    color: #92506a;
}

/* =========================
   YES / NO BUTTONS
========================= */

.buttons {
    width: 100%;

    display: flex;

    justify-content: center;
    align-items: center;

    gap: 15px;

    margin-top: 25px;

    min-height: 80px;

    position: relative;
}

.yes-btn,
.no-btn {
    padding: 13px 25px;

    border-radius: 30px;

    font-size: 16px;
}

.yes-btn {
    background: #ff6f9f;
    color: white;

    box-shadow:
        0 7px 18px rgba(220, 70, 115, 0.25);
}

.no-btn {
    background: #f5d9e2;
    color: #8c5268;
}

.yes-btn:hover,
.no-btn:hover {
    transform: scale(1.05);
}

/* =========================
   SUCCESS
========================= */

.success-heart {
    font-size: clamp(70px, 20vw, 100px);

    animation:
        heartBeat 1s infinite;
}

@keyframes heartBeat {
    0%,
    100% {
        transform: scale(1);
    }

    25% {
        transform: scale(1.12);
    }

    50% {
        transform: scale(1);
    }

    75% {
        transform: scale(1.12);
    }
}

.success-message {
    font-size: 18px;

    color: #d94d7a;

    font-weight: bold;
}

/* =========================
   FLOATING HEARTS / FLOWERS
========================= */

.floating {
    position: fixed;

    pointer-events: none;

    z-index: 1;

    animation:
        floatUp linear forwards;
}

@keyframes floatUp {
    from {
        transform: translateY(110vh) rotate(0deg);
        opacity: 0;
    }

    10% {
        opacity: 1;
    }

    90% {
        opacity: 1;
    }

    to {
        transform: translateY(-120px) rotate(360deg);
        opacity: 0;
    }
}

/* =========================
   MOVING CAT
========================= */

.moving-cat {
    position: fixed;

    bottom: 15px;
    left: 0;

    font-size: 55px;

    z-index: 20;

    pointer-events: none;

    animation:
        catWalk 14s linear infinite,
        catBounce 0.6s ease-in-out infinite;
}

@keyframes catWalk {
    0% {
        transform: translate3d(-120px, 0, 0);
    }

    48% {
        transform: translate3d(calc(100vw - 80px), 0, 0);
    }

    50% {
        transform: translate3d(calc(100vw - 80px), 0, 0);
    }

    98% {
        transform: translate3d(-120px, 0, 0);
    }

    100% {
        transform: translate3d(-120px, 0, 0);
    }
}

@keyframes catBounce {
    0%,
    100% {
        margin-bottom: 0;
    }

    50% {
        margin-bottom: 8px;
    }
}

/* =========================
   CAT TEXT
========================= */

.cat-text {
    position: fixed;

    bottom: 70px;
    left: 50%;

    transform: translateX(-50%);

    z-index: 19;

    font-size: 13px;

    color: #c84d76;

    pointer-events: none;

    white-space: nowrap;

    animation: catTextFade 2s ease-in-out infinite;
}

@keyframes catTextFade {
    0%,
    100% {
        opacity: 0.5;
    }

    50% {
        opacity: 1;
    }
}

/* =========================
   MOBILE
========================= */

@media (max-width: 600px) {

    body {
        padding: 12px;

        box-sizing: border-box;
    }

    .card {
        max-width: 450px;

        max-height: 96vh;
        max-height: 96dvh;

        padding: 25px 18px;

        border-radius: 26px;
    }

    .letter {
        padding: 18px;
    }

    .buttons {
        gap: 10px;
    }

    .yes-btn,
    .no-btn {
        padding: 12px 20px;

        font-size: 15px;
    }

    .moving-cat {
        font-size: 45px;
    }
}

/* =========================
   VERY SMALL PHONES
========================= */

@media (max-width: 360px) {

    body {
        padding: 8px;
    }

    .card {
        padding: 20px 14px;
    }

    .buttons {
        gap: 7px;
    }

    .yes-btn,
    .no-btn {
        padding: 11px 17px;

        font-size: 14px;
    }

    .letter {
        padding: 15px;
    }
}
</style>
</head>

<body>

<!-- =========================
     FLOATING DECORATIONS
========================= -->

<div class="moving-cat">
    🐈🎀
</div>

<div class="cat-text">
    Meowww~ 💗
</div>

<!-- =========================
     MAIN CARD
========================= -->

<div class="card">

    <!-- INTRO PAGE -->
    <section class="page active" id="introPage">

        <div class="big-bouquet">
            💐
        </div>

        <h1>
            For Nicolaiii 💗
        </h1>

        <p class="subtitle">
            I made a little something for you...
        </p>

        <button
            class="main-btn"
            onclick="showPage('envelopePage')"
        >
            Open my little surprise 💌
        </button>

    </section>


    <!-- ENVELOPE PAGE -->
    <section class="page" id="envelopePage">

        <h2>
            A little letter for you 💗
        </h2>

        <p>
            Click the envelope to open it.
        </p>

        <div
            class="envelope-area"
            onclick="showPage('letterPage')"
        >

            <div class="envelope">

                <div class="heart-seal">
                    💗
                </div>

            </div>

        </div>

    </section>


    <!-- LETTER PAGE -->
    <section class="page" id="letterPage">

        <div class="letter">

            <h2>
                Hiii Nicolaiii 💗
            </h2>

            <p>
                I just wanted to make something a little special for you.
            </p>

            <p>
                Sometimes, the simplest moments can become
                the sweetest memories.
            </p>

            <p>
                So I thought...
                why not ask you properly? 🥺
            </p>

            <p>
                I would really love to spend some time with you,
                have coffee, talk about random things,
                laugh together, and simply enjoy the moment.
            </p>

            <p>
                So here's my little question for you...
            </p>

            <div class="signature">
                — From Christian 💗
            </div>

        </div>

        <button
            class="main-btn"
            onclick="showPage('questionPage')"
        >
            Continue 💌
        </button>

    </section>


    <!-- QUESTION PAGE -->
    <section class="page" id="questionPage">

        <div class="teddy">
            🧸
        </div>

        <div class="date-question">

            <h1>
                Coffee Date? ☕💗
            </h1>

            <p>
                Would you like to go on a coffee date with me?
            </p>

        </div>

        <div class="buttons">

            <button
                class="yes-btn"
                id="yesBtn"
                onclick="sayYes()"
            >
                YES 💗
            </button>

            <button
                class="no-btn"
                id="noBtn"
                onclick="sayNo()"
            >
                NO 😭
            </button>

        </div>

    </section>


    <!-- SUCCESS PAGE -->
    <section class="page" id="successPage">

        <div class="success-heart">
            💗
        </div>

        <h1>
            YEEHEYYY!! 🥳💗
        </h1>

        <p class="success-message">
            It's a date! ☕🌸
        </p>

        <p>
            I can't wait to spend some time with you.
        </p>

        <p>
            Thank you for saying yes! 🥺💗
        </p>

        <div style="
            font-size: 45px;
            margin-top: 15px;
        ">
            ☕🌷💐🧸
        </div>

    </section>

</div>


<script>

/* =========================
   PAGE NAVIGATION
========================= */

function showPage(pageId) {

    const pages = document.querySelectorAll(".page");

    pages.forEach(function(page) {

        page.classList.remove("active");

    });

    const target = document.getElementById(pageId);

    if (target) {

        target.classList.add("active");

    }

    /*
     * Always return the card to the top.
     * This prevents the content from appearing
     * shifted after clicking another page.
     */

    const card = document.querySelector(".card");

    if (card) {
        card.scrollTop = 0;
    }

    /*
     * Prevent horizontal movement caused by
     * transformed/scaled elements.
     */

    window.scrollTo({
        top: 0,
        left: 0,
        behavior: "instant"
    });
}


/* =========================
   NO BUTTON
========================= */

let noCount = 0;

function sayNo() {

    noCount++;

    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");

    /*
     * Make YES gradually bigger.
     * Maximum size is limited so it cannot
     * create a huge horizontal overflow.
     */

    const yesScale = Math.min(
        1 + noCount * 0.2,
        2.2
    );

    yesBtn.style.transform =
        "scale(" + yesScale + ")";

    /*
     * Make NO smaller.
     */

    const noScale = Math.max(
        1 - noCount * 0.12,
        0.35
    );

    noBtn.style.transform =
        "scale(" + noScale + ")";

    /*
     * Change the text as they keep clicking NO.
     */

    const messages = [
        "NO 😭",
        "Are you sure? 🥺",
        "Really? 😭",
        "Pleaseee 🥺",
        "Think again 💗",
        "One coffee? ☕🥺",
        "Pleaaaseee 😭💗"
    ];

    noBtn.innerText =
        messages[Math.min(noCount, messages.length - 1)];

    /*
     * Eventually hide the NO button.
     */

    if (noCount >= 7) {

        noBtn.style.opacity = "0";
        noBtn.style.pointerEvents = "none";

    }
}


/* =========================
   YES BUTTON
========================= */

function sayYes() {

    showPage("successPage");

    /*
     * Create celebration hearts.
     */

    for (let i = 0; i < 18; i++) {

        setTimeout(function() {

            createFloating(
                ["💗", "💖", "💕", "🌸", "✨", "🌷"][
                    Math.floor(
                        Math.random() * 6
                    )
                ]
            );

        }, i * 120);

    }
}


/* =========================
   FLOATING ELEMENTS
========================= */

function createFloating(symbol) {

    const element = document.createElement("div");

    element.className = "floating";

    element.innerText = symbol;

    /*
     * Keep elements away from the extreme
     * right edge to prevent horizontal overflow.
     */

    const randomLeft =
        Math.min(
            Math.random() * 96,
            96
        );

    element.style.left =
        randomLeft + "vw";

    element.style.fontSize =
        (16 + Math.random() * 20) + "px";

    element.style.animationDuration =
        (4 + Math.random() * 4) + "s";

    document.body.appendChild(element);

    setTimeout(function() {

        element.remove();

    }, 8500);
}


/* =========================
   AUTOMATIC FLOATING HEARTS
========================= */

setInterval(function() {

    const symbols = [
        "💗",
        "💖",
        "💕",
        "🌸",
        "🌷",
        "✨"
    ];

    const symbol =
        symbols[
            Math.floor(
                Math.random() * symbols.length
            )
        ];

    createFloating(symbol);

}, 1000);


/* =========================
   EXTRA SAFETY
   Prevent accidental horizontal
   scrolling on resize.
========================= */

window.addEventListener("resize", function() {

    document.documentElement.style.overflowX = "hidden";

    document.body.style.overflowX = "hidden";

});


/* =========================
   INITIAL SETUP
========================= */

document.addEventListener("DOMContentLoaded", function() {

    const card = document.querySelector(".card");

    if (card) {
        card.scrollTop = 0;
    }

});

</script>

</body>
</html>
