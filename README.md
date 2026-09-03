# i
 <html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>A Little Surprise For You 💐💗</title>

<style>

/* =========================
   BASIC RESET
========================= */

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html,
body {
    width: 100%;
    min-height: 100%;
    max-width: 100%;
    overflow-x: hidden;
}

body {
    min-height: 100vh;
    min-height: 100dvh;

    display: flex;
    justify-content: center;
    align-items: center;

    padding: 20px;

    font-family:
        "Trebuchet MS",
        Arial,
        sans-serif;

    color: #8a4560;

    background:
        radial-gradient(
            circle at 10% 10%,
            #ffffff 0%,
            transparent 25%
        ),
        radial-gradient(
            circle at 90% 90%,
            #ffb6d0 0%,
            transparent 30%
        ),
        radial-gradient(
            circle at 50% 0%,
            #ffd1e2 0%,
            transparent 40%
        ),
        linear-gradient(
            135deg,
            #ffc9dd,
            #fff0f6,
            #ffc4da
        );

    overflow-x: hidden;
}


/* =========================
   BACKGROUND HEARTS
========================= */

.hearts {
    position: fixed;
    inset: 0;
    overflow: hidden;
    pointer-events: none;
    z-index: 1;
}

.heart {
    position: absolute;
    bottom: -50px;
    opacity: 0;

    animation:
        floatUp
        6s
        linear
        forwards;
}

@keyframes floatUp {

    0% {
        transform:
            translate3d(0, 0, 0)
            rotate(0deg);
        opacity: 0;
    }

    15% {
        opacity: 1;
    }

    100% {
        transform:
            translate3d(0, -115vh, 0)
            rotate(360deg);
        opacity: 0;
    }
}


/* =========================
   FLOATING FLOWERS
========================= */

.flower {
    position: fixed;
    bottom: -60px;
    pointer-events: none;
    z-index: 2;
    opacity: 0;
    max-width: 100vw;

    animation:
        flowerUp
        8s
        linear
        forwards;
}

@keyframes flowerUp {

    0% {
        transform:
            translate3d(0, 0, 0)
            rotate(0deg);
        opacity: 0;
    }

    15% {
        opacity: .9;
    }

    100% {
        transform:
            translate3d(0, -115vh, 0)
            rotate(300deg);
        opacity: 0;
    }
}


/* =========================
   SPARKLES
========================= */

.sparkle {
    position: fixed;
    color: #f08aaa;
    font-size: 24px;
    pointer-events: none;
    z-index: 3;

    animation:
        sparkle
        2.5s
        ease-in-out
        infinite;
}

@keyframes sparkle {

    0%,
    100% {
        opacity: .3;
        transform: scale(.8);
    }

    50% {
        opacity: 1;
        transform: scale(1.3);
    }
}


/* =========================
   MAIN CARD
========================= */

.card {
    width: min(450px, 100%);
    max-width: 100%;

    max-height: 94vh;
    max-height: 94dvh;

    padding: 30px 24px;

    position: relative;
    z-index: 10;

    text-align: center;

    overflow-y: auto;
    overflow-x: hidden;

    scrollbar-width: none;

    background:
        rgba(255, 255, 255, .94);

    border:
        2px solid
        rgba(255, 182, 208, .75);

    border-radius: 32px;

    box-shadow:
        0 20px 50px
        rgba(214, 83, 122, .25),

        0 5px 15px
        rgba(214, 83, 122, .1);

    backdrop-filter:
        blur(12px);
}

.card::-webkit-scrollbar {
    display: none;
}


/* =========================
   BOWS
========================= */

.corner-bow {
    position: absolute;
    font-size: 30px;

    animation:
        bowWiggle
        2s
        ease-in-out
        infinite;
}

.bow-left {
    top: 12px;
    left: 15px;
}

.bow-right {
    top: 12px;
    right: 15px;
    animation-delay: .5s;
}

@keyframes bowWiggle {

    0%,
    100% {
        transform: rotate(-8deg);
    }

    50% {
        transform:
            rotate(8deg)
            scale(1.1);
    }
}


/* =========================
   PAGE TRANSITIONS
========================= */

.page {
    width: 100%;
    max-width: 100%;

    animation:
        pageIn
        .7s
        ease;
}

@keyframes pageIn {

    0% {
        opacity: 0;
        transform:
            translate3d(0, 15px, 0);
    }

    100% {
        opacity: 1;
        transform:
            translate3d(0, 0, 0);
    }
}

.hidden {
    display: none !important;
}


/* =========================
   INTRODUCTION
========================= */

.intro {
    padding:
        20px
        5px
        10px;

    max-width: 100%;
}

.intro-small {
    margin-top: 5px;
    font-size: 15px;
    color: #c27a94;
}

.intro-title {
    margin-top: 15px;
    font-size: 28px;
    color: #df507d;
}

.intro-text {
    margin-top: 12px;
    font-size: 16px;
    line-height: 1.6;
    color: #98506a;
}


/* =========================
   BOUQUET
========================= */

.bouquet {
    width: 100%;
    min-height: 300px;

    margin:
        5px
        auto
        5px;

    display: flex;

    justify-content: center;
    align-items: center;

    position: relative;

    overflow: visible;

    animation:
        bouquetFloat
        3s
        ease-in-out
        infinite;
}

@keyframes bouquetFloat {

    0%,
    100% {
        transform:
            translate3d(0, 0, 0);
    }

    50% {
        transform:
            translate3d(0, -8px, 0);
    }
}

.big-bouquet {
    display: block;

    font-size: 190px;

    line-height: 1;

    white-space: nowrap;

    filter:
        drop-shadow(
            0 12px 10px
            rgba(214, 83, 122, .20)
        );

    transform-origin: center center;

    user-select: none;
}


/* =========================
   OPEN BUTTON
========================= */

.open-button {
    margin-top: 15px;

    padding:
        14px
        27px;

    border: none;

    border-radius: 50px;

    background:
        linear-gradient(
            135deg,
            #f06f9a,
            #df4f7d
        );

    color: white;

    font-family: inherit;

    font-size: 17px;

    font-weight: bold;

    cursor: pointer;

    box-shadow:
        0 8px 20px
        rgba(214, 83, 122, .25);

    transition:
        transform .25s ease,
        box-shadow .25s ease;
}

.open-button:hover {
    transform:
        translate3d(0, -3px, 0)
        scale(1.03);

    box-shadow:
        0 10px 25px
        rgba(214, 83, 122, .35);
}

.open-button:active {
    transform: scale(.96);
}


/* =========================
   ENVELOPE
========================= */

.envelope-area {
    padding:
        15px
        5px
        10px;

    max-width: 100%;
}

.envelope-title {
    margin-top: 10px;
    font-size: 25px;
    color: #df507d;
}

.envelope-subtitle {
    margin-top: 8px;
    font-size: 14px;
    color: #b86e88;
}

.envelope {
    width: 290px;
    height: 190px;

    max-width: 100%;

    margin:
        35px
        auto
        25px;

    position: relative;

    cursor: pointer;

    perspective: 700px;
}

.envelope-body {
    position: absolute;
    inset: 0;

    background:
        linear-gradient(
            135deg,
            #fff4f8,
            #ffd5e3
        );

    border:
        2px solid
        #f2b5ca;

    border-radius: 10px;

    box-shadow:
        0 12px 25px
        rgba(214, 83, 122, .18);

    overflow: hidden;
}

.envelope-body::before {
    content: "";

    position: absolute;

    bottom: 0;
    left: 0;

    width: 0;
    height: 0;

    border-left:
        143px solid transparent;

    border-right:
        143px solid transparent;

    border-bottom:
        105px solid
        #ffc5d8;
}

.envelope-body::after {
    content: "";

    position: absolute;

    top: 0;
    left: 0;

    width: 0;
    height: 0;

    border-left:
        143px solid transparent;

    border-right:
        143px solid transparent;

    border-top:
        100px solid
        #ffe6ef;
}

.seal {
    position: absolute;

    left: 50%;
    top: 47%;

    transform:
        translate(-50%, -50%);

    z-index: 10;

    font-size: 40px;

    filter:
        drop-shadow(
            0 4px 4px
            rgba(214, 83, 122, .15)
        );

    animation:
        sealBeat
        1.5s
        ease-in-out
        infinite;
}

@keyframes sealBeat {

    0%,
    100% {
        transform:
            translate(-50%, -50%)
            scale(1);
    }

    50% {
        transform:
            translate(-50%, -50%)
            scale(1.12);
    }
}

.click-envelope {
    font-size: 14px;
    color: #c06f8a;

    animation:
        blink
        2s
        ease-in-out
        infinite;
}

@keyframes blink {

    0%,
    100% {
        opacity: .6;
    }

    50% {
        opacity: 1;
    }
}


/* =========================
   LETTER
========================= */

.letter {
    margin:
        15px
        5px
        5px;

    padding:
        25px
        20px;

    max-width: 100%;

    background:
        linear-gradient(
            135deg,
            #fffafa,
            #fff0f6
        );

    border:
        2px solid
        #f4bfd1;

    border-radius: 22px;

    box-shadow:
        0 10px 25px
        rgba(214, 83, 122, .12);
}

.letter-top {
    font-size: 35px;
}

.letter h1 {
    margin:
        12px
        0;

    font-size: 27px;
    color: #df507d;
}

.letter p {
    font-size: 16px;
    line-height: 1.7;
    color: #98506a;
}

.letter-name {
    margin-top: 15px;
    color: #df507d;
    font-weight: bold;
}


/* =========================
   DATE QUESTION
========================= */

.character {
    position: relative;

    display: inline-block;

    margin-top: 5px;

    font-size: 72px;

    line-height: 1;

    animation:
        characterBounce
        2s
        ease-in-out
        infinite;

    filter:
        drop-shadow(
            0 7px 8px
            rgba(214, 83, 122, .15)
        );
}

.character-bow {
    position: absolute;

    top: -18px;
    right: -15px;

    font-size: 34px;

    animation:
        bowFloat
        1.8s
        ease-in-out
        infinite;
}

@keyframes characterBounce {

    0%,
    100% {
        transform:
            translate3d(0, 0, 0);
    }

    50% {
        transform:
            translate3d(0, -9px, 0);
    }
}

@keyframes bowFloat {

    0%,
    100% {
        transform: rotate(-10deg);
    }

    50% {
        transform:
            rotate(10deg)
            scale(1.1);
    }
}

.decorations {
    margin:
        8px
        0
        15px;

    font-size: 21px;

    letter-spacing: 5px;

    animation:
        sparkleText
        2s
        ease-in-out
        infinite;
}

@keyframes sparkleText {

    0%,
    100% {
        opacity: .7;
    }

    50% {
        opacity: 1;
    }
}

.question-title {
    margin:
        15px
        0
        10px;

    font-size: 30px;
    color: #e05280;
}

.question {
    margin-bottom: 25px;
    font-size: 18px;
    line-height: 1.6;
}


/* =========================
   BUTTONS
========================= */

.buttons {
    min-height: 120px;

    width: 100%;

    display: flex;

    justify-content: center;
    align-items: center;

    gap: 15px;

    position: relative;

    overflow: visible;
}

.date-button {
    border: none;

    border-radius: 50px;

    padding:
        14px
        28px;

    font-family: inherit;

    font-size: 17px;

    font-weight: bold;

    cursor: pointer;

    transition:
        transform .35s ease,
        background .25s ease,
        box-shadow .25s ease;
}

#yesBtn {
    position: relative;

    z-index: 3;

    background:
        linear-gradient(
            135deg,
            #f06f9a,
            #df4f7d
        );

    color: white;

    box-shadow:
        0 7px 18px
        rgba(214, 83, 122, .3);
}

#yesBtn:hover {
    box-shadow:
        0 9px 23px
        rgba(214, 83, 122, .38);
}

#noBtn {
    position: relative;

    z-index: 2;

    background: #ffe3ed;

    color: #9a7180;

    border:
        1px solid
        #f8bfd2;
}

#noBtn:hover {
    background: #ffd5e4;
}

#message {
    min-height: 28px;
    margin-top: 10px;

    font-weight: bold;
    color: #dc507d;
}

.tiny {
    margin-top: 18px;
    font-size: 13px;
    color: #c27a94;
}


/* =========================
   SUCCESS PAGE
========================= */

.success h1 {
    margin:
        15px
        0
        10px;

    font-size: 35px;
    color: #e05280;
}

.thank-you {
    margin-top: 20px;

    padding:
        23px
        18px;

    background:
        linear-gradient(
            135deg,
            #fff0f6,
            #ffdce9
        );

    border:
        2px solid
        #f6bfd2;

    border-radius: 25px;

    box-shadow:
        inset 0 0 20px
        rgba(255,255,255,.7),

        0 8px 20px
        rgba(214,83,122,.12);
}

.thank-you p {
    font-size: 17px;
    line-height: 1.7;
}

.important {
    color: #df4f7d;
    font-weight: bold;
}

.chat-bubble {
    position: relative;

    margin:
        22px
        auto
        5px;

    max-width: 330px;

    padding:
        15px
        18px;

    background: white;

    border:
        2px solid
        #f5bfd2;

    border-radius: 20px;

    color: #98506a;

    font-size: 15px;
    line-height: 1.5;

    box-shadow:
        0 5px 15px
        rgba(214,83,122,.1);
}

.chat-bubble::after {
    content: "";

    position: absolute;

    bottom: -10px;
    left: 50%;

    width: 18px;
    height: 18px;

    background: white;

    border-right:
        2px solid
        #f5bfd2;

    border-bottom:
        2px solid
        #f5bfd2;

    transform:
        translateX(-50%)
        rotate(45deg);
}

.final-note {
    margin-top: 25px;

    color: #bd718b;

    font-size: 14px;

    line-height: 1.6;
}


/* =========================
   MOVING CAT
   IMPORTANT FIX:
   Uses transform instead of left:100vw
   so it cannot create horizontal scrolling.
========================= */

.moving-cat {
    position: fixed;

    bottom: 15px;
    left: 0;

    font-size: 55px;

    z-index: 20;

    pointer-events: none;

    animation:
        catWalk
        14s
        linear
        infinite,

        catBounce
        .6s
        ease-in-out
        infinite;
}

.cat-bow {
    position: absolute;

    top: -8px;
    right: -5px;

    font-size: 23px;

    animation:
        catBow
        .8s
        ease-in-out
        infinite;
}

@keyframes catWalk {

    0% {
        transform:
            translate3d(-120px, 0, 0);
    }

    48% {
        transform:
            translate3d(calc(100vw - 10px), 0, 0);
    }

    50% {
        transform:
            translate3d(calc(100vw - 10px), 0, 0);
    }

    98% {
        transform:
            translate3d(-120px, 0, 0);
    }

    100% {
        transform:
            translate3d(-120px, 0, 0);
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

@keyframes catBow {

    0%,
    100% {
        transform: rotate(-10deg);
    }

    50% {
        transform:
            rotate(10deg)
            scale(1.1);
    }
}


/* =========================
   CAT MESSAGE
========================= */

.cat-message {
    position: fixed;

    bottom: 78px;
    left: 20px;

    padding:
        9px
        14px;

    background: white;

    border:
        2px solid
        #f5bfd2;

    border-radius: 18px;

    color: #d95780;

    font-size: 13px;
    font-weight: bold;

    z-index: 21;

    animation:
        messageFloat
        2s
        ease-in-out
        infinite;
}

@keyframes messageFloat {

    0%,
    100% {
        transform:
            translate3d(0, 0, 0);
    }

    50% {
        transform:
            translate3d(0, -5px, 0);
    }
}


/* =========================
   MOBILE
========================= */

@media (max-width: 500px) {

    body {
        padding: 12px;
        overflow-x: hidden;
    }

    .card {
        width: 100%;
        max-width: 450px;

        padding:
            28px
            18px;
    }

    .bouquet {
        width: 100%;
        min-height: 270px;

        margin:
            0
            auto
            5px;

        display: flex;

        justify-content: center;
        align-items: center;
    }

    .big-bouquet {
        font-size: 145px;
        line-height: 1;

        transform:
            translate3d(0, 0, 0);
    }

    .intro-title {
        font-size: 25px;
    }

    .envelope {
        width: 270px;
        height: 175px;
        max-width: 100%;
    }

    .character {
        font-size: 63px;
    }

    .question-title {
        font-size: 27px;
    }

    .success h1 {
        font-size: 31px;
    }

    .moving-cat {
        font-size: 45px;
    }

    .cat-message {
        left: 8px;
        bottom: 65px;
    }

    .buttons {
        width: 100%;
        gap: 10px;
    }

    .date-button {
        padding:
            13px
            22px;

        font-size: 16px;
    }
}


/* =========================
   VERY SMALL PHONES
========================= */

@media (max-width: 360px) {

    .big-bouquet {
        font-size: 120px;
    }

    .bouquet {
        min-height: 235px;
    }

    .date-button {
        padding:
            12px
            18px;

        font-size: 15px;
    }
}


/* =========================
   EXTRA HORIZONTAL SAFETY
========================= */

html {
    overflow-x: hidden;
    width: 100%;
}

body {
    overflow-x: hidden;
    width: 100%;
    max-width: 100vw;
}

.card,
.page,
.intro,
.envelope-area,
.letter,
.success {
    max-width: 100%;
}


/* =========================
   REDUCED MOTION
========================= */

@media (prefers-reduced-motion: reduce) {

    *,
    *::before,
    *::after {
        animation-duration: .01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: .01ms !important;
    }
}

</style>
</head>

<body>


<!-- =========================
     FLOATING BACKGROUND
========================= -->

<div
    class="hearts"
    id="hearts">
</div>


<span
    class="sparkle"
    style="top:8%;left:8%;">
    ✦
</span>

<span
    class="sparkle"
    style="top:20%;right:8%;animation-delay:.7s;">
    ✧
</span>

<span
    class="sparkle"
    style="bottom:18%;left:9%;animation-delay:1s;">
    ♡
</span>

<span
    class="sparkle"
    style="bottom:25%;right:10%;animation-delay:.4s;">
    ✦
</span>


<!-- =========================
     MOVING CAT
========================= -->

<div class="moving-cat">

    🐱

    <span class="cat-bow">
        🎀
    </span>

</div>

<div class="cat-message">
    Meowww~ 💗
</div>


<!-- =========================
     MAIN CARD
========================= -->

<main class="card">


<!-- =========================
     CORNER BOWS
========================= -->

<div class="corner-bow bow-left">
    🎀
</div>

<div class="corner-bow bow-right">
    🎀
</div>


<!-- =========================
     INTRODUCTION
========================= -->

<section
    id="introPage"
    class="page">

    <div class="intro">

        <div class="intro-small">
            ✨ A little surprise for you ✨
        </div>


        <div class="bouquet">

            <span class="big-bouquet">
                💐
            </span>

        </div>


        <h1 class="intro-title">
            For Nicolaiii 💗
        </h1>


        <p class="intro-text">

            I prepared a little something
            for you hehe... 🌷🫶🏻🌷

            <br><br>

            It's nothing too serious,
            just something cute from me. 🎀

        </p>


        <button
            class="open-button"
            id="seeBouquetBtn"
            type="button">

            Open my little surprise 💌

        </button>

    </div>

</section>


<!-- =========================
     ENVELOPE
========================= -->

<section
    id="envelopePage"
    class="page hidden">

    <div class="envelope-area">

        <div class="decorations">
            🌷 🎀 💗 🎀 🌷
        </div>


        <h1 class="envelope-title">
            There's a little letter for you 💌
        </h1>


        <p class="envelope-subtitle">
            Tap the envelope to open it
        </p>


        <div
            class="envelope"
            id="envelope"
            role="button"
            tabindex="0"
            aria-label="Open the letter">

            <div class="envelope-body">
            </div>

            <div class="seal">
                💗
            </div>

        </div>


        <p class="click-envelope">
            💌 click meee 🎀
        </p>

    </div>

</section>


<!-- =========================
     LETTER
========================= -->

<section
    id="letterPage"
    class="page hidden">

    <div class="letter">

        <div class="letter-top">
            💌
        </div>


        <h1>
            Hiii Nicolaiii 💗
        </h1>


        <p>

            Before you continue...

            <br><br>

            I just wanted to give you
            this little virtual bouquet. 💐

            <br><br>

            I hope it makes you smile
            even just a little bit. 🥹💗

            <br><br>

            And there's one tiny question
            I wanted to ask you...

        </p>


        <div class="letter-name">

            — From someone who wants
            to take you out for coffee 🎀

        </div>


        <button
            class="open-button"
            id="questionBtn"
            type="button">

            There's one more thing... 💗

        </button>

    </div>

</section>


<!-- =========================
     DATE QUESTION
========================= -->

<section
    id="questionPage"
    class="page hidden">


    <div class="character">

        🧸

        <span class="character-bow">
            🎀
        </span>

    </div>


    <div class="decorations">
        🌷 💗 ✨ 🎀 ✨ 💗 🌷
    </div>


    <h1 class="question-title">
        Coffee Date?
    </h1>


    <p class="question">

        Hi Nicolaiii heheee 💗

        <br>

        Would you like to go on a

        <br>

        <strong>
            Coffee date
        </strong>

        with me? 🌷✨

    </p>


    <div class="buttons">

        <button
            id="yesBtn"
            class="date-button"
            type="button">

            YES 💗

        </button>


        <button
            id="noBtn"
            class="date-button"
            type="button">

            NO 😭

        </button>

    </div>


    <div
        id="message"
        aria-live="polite">
    </div>


    <p class="tiny">
        Choose wisely... 👀🎀
    </p>

</section>


<!-- =========================
     SUCCESS
========================= -->

<section
    id="successPage"
    class="page hidden">

    <div class="success">

        <div class="character">

            🧸

            <span class="character-bow">
                🎀
            </span>

        </div>


        <div class="decorations">
            💗 🎀 🌷 ✨ 🎀 🌷 💗
        </div>


        <h1>
            YEEHEYYY!! 🥳💗
        </h1>


        <p class="question">
            Thank youuu for saying yes hehehe🎀
        </p>


        <div class="thank-you">

            <p>
                I’m really happyyy
                you said yes! 💐💐
            </p>

            <br>

            <p>

                No pressure on the date haaa.

                <span class="important">
                    Chat me whenever you're freeee
                </span>

                because I respect your time
                and I want us to enjoy it when
                we're both available. 🌷

            </p>

        </div>


        <div class="chat-bubble">

            💌 Just chat me when you're free,
            okayyy?

            <br>

            I'll be waiting hehe 🎀

        </div>


        <div class="final-note">

            Take your timeee 🤍

            <br>

            No rush, no pressure —
            just a cute little coffee date
            when the time is right.!!!

        </div>


        <div
            class="decorations"
            style="margin-top:22px;">

            🎀 💕 🌷 💕 🎀

        </div>

    </div>

</section>


</main>


<!-- =========================
     JAVASCRIPT
========================= -->

<script>


/* =========================
   PAGE ELEMENTS
========================= */

const introPage =
    document.getElementById("introPage");

const envelopePage =
    document.getElementById("envelopePage");

const letterPage =
    document.getElementById("letterPage");

const questionPage =
    document.getElementById("questionPage");

const successPage =
    document.getElementById("successPage");


const seeBouquetBtn =
    document.getElementById("seeBouquetBtn");

const envelope =
    document.getElementById("envelope");

const questionBtn =
    document.getElementById("questionBtn");

const yesBtn =
    document.getElementById("yesBtn");

const noBtn =
    document.getElementById("noBtn");

const message =
    document.getElementById("message");

const heartsContainer =
    document.getElementById("hearts");


/* =========================
   CHANGE PAGE
========================= */

function showPage(page) {

    const pages = [
        introPage,
        envelopePage,
        letterPage,
        questionPage,
        successPage
    ];

    pages.forEach(currentPage => {
        currentPage.classList.add("hidden");
    });

    page.classList.remove("hidden");


    /* Restart animation */

    page.classList.remove("page");

    void page.offsetWidth;

    page.classList.add("page");


    /* Always reset card scroll */

    const card =
        document.querySelector(".card");

    card.scrollTop = 0;

}


/* =========================
   INTRO → ENVELOPE
========================= */

seeBouquetBtn.addEventListener(
    "click",
    () => {

        createHearts(15);

        createFlowers(12);

        showPage(envelopePage);

    }
);


/* =========================
   ENVELOPE → LETTER
========================= */

envelope.addEventListener(
    "click",
    openEnvelope
);


envelope.addEventListener(
    "keydown",
    event => {

        if (
            event.key === "Enter" ||
            event.key === " "
        ) {

            event.preventDefault();

            openEnvelope();

        }

    }
);


function openEnvelope() {

    createHearts(12);

    createFlowers(8);

    showPage(letterPage);

}


/* =========================
   LETTER → QUESTION
========================= */

questionBtn.addEventListener(
    "click",
    () => {

        createHearts(10);

        showPage(questionPage);

    }
);


/* =========================
   NO BUTTON
========================= */

const noMessages = [

    "Try again 😭💗",

    "Are you sure? 🥺🎀",

    "Think again hehe 👀",

    "Wrong button 😭",

    "The YES button is waiting... 💗",

    "Pleaseeee 🥹🌷",

    "You can't escape the coffee date 😌💗",

    "One more chance? 🥺💕"

];


let noCount = 0;


noBtn.addEventListener(
    "click",
    sayNo
);


function sayNo() {

    const currentMessage =
        noMessages[
            Math.min(
                noCount,
                noMessages.length - 1
            )
        ];

    message.textContent =
        currentMessage;

    noCount++;


    /* =====================
       YES GETS BIGGER
    ===================== */

    const yesSize =
        Math.min(
            3,
            1 + noCount * .25
        );

    yesBtn.style.transform =
        `scale(${yesSize})`;


    /* =====================
       NO GETS SMALLER
    ===================== */

    const noSize =
        Math.max(
            .55,
            1 - noCount * .08
        );

    noBtn.style.transform =
        `scale(${noSize})`;


    if (noCount >= 7) {

        yesBtn.style.transform =
            "scale(3)";

        message.textContent =
            "Okayyyy... YES na lang 😭💗🎀";

    }


    createHearts(5);

}


/* =========================
   YES BUTTON
========================= */

yesBtn.addEventListener(
    "click",
    sayYes
);


function sayYes() {

    yesBtn.style.transform = "";

    noBtn.style.transform = "";

    createHearts(40);

    createFlowers(25);

    showPage(successPage);


    setTimeout(() => {

        createHearts(25);

        createFlowers(15);

    }, 800);

}


/* =========================
   CREATE HEARTS
========================= */

function createHearts(count = 15) {

    const emojis = [

        "💗",
        "💕",
        "💖",
        "💘",
        "🤍",
        "♡",
        "🎀",
        "✨"

    ];


    for (
        let i = 0;
        i < count;
        i++
    ) {

        setTimeout(() => {

            const heart =
                document.createElement("div");

            heart.classList.add("heart");

            heart.textContent =
                emojis[
                    Math.floor(
                        Math.random() *
                        emojis.length
                    )
                ];


            heart.style.left =
                Math.random() * 100 +
                "vw";


            heart.style.fontSize =
                (
                    16 +
                    Math.random() * 20
                ) +
                "px";


            heart.style.animationDuration =
                (
                    4 +
                    Math.random() * 4
                ) +
                "s";


            heartsContainer.appendChild(
                heart
            );


            setTimeout(() => {

                heart.remove();

            }, 8500);

        }, i * 80);

    }

}


/* =========================
   CREATE FLOWERS
========================= */

function createFlowers(count = 8) {

    const flowers = [

        "🌸",
        "🌷",
        "🌺",
        "🌼",
        "🪻",
        "🌹",
        "💐"

    ];


    for (
        let i = 0;
        i < count;
        i++
    ) {

        setTimeout(() => {

            const flower =
                document.createElement("div");

            flower.classList.add("flower");

            flower.textContent =
                flowers[
                    Math.floor(
                        Math.random() *
                        flowers.length
                    )
                ];


            flower.style.left =
                Math.random() * 100 +
                "vw";


            flower.style.fontSize =
                (
                    18 +
                    Math.random() * 25
                ) +
                "px";


            flower.style.animationDuration =
                (
                    5 +
                    Math.random() * 5
                ) +
                "s";


            document.body.appendChild(
                flower
            );


            setTimeout(() => {

                flower.remove();

            }, 11000);

        }, i * 180);

    }

}


/* =========================
   INITIAL AMBIANCE
========================= */

setTimeout(() => {

    createHearts(8);

    createFlowers(6);

}, 800);


/* =========================
   CONTINUOUS FLOWERS
========================= */

setInterval(() => {

    createFlowers(2);

}, 6000);


</script>

</body>
</html>
