# Digital-Well-Being-and-Responsible-Technology-Use-

<!DOCTYPE html>
<html lang="en">

<head>
<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

<title>Mindful Bytes | Digital Well-being</title>

<style>

/* =====================================================
   RESET
===================================================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    overflow-x: hidden;
}

body {
    width: 100%;
    min-width: 0;
    overflow-x: hidden;

    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.7;

    color: #30243d;
    background: #f7f2fc;
}

img {
    max-width: 100%;
}

a {
    -webkit-tap-highlight-color: transparent;
}

h1,
h2,
h3 {
    line-height: 1.2;
}

p {
    margin-bottom: 15px;
}


/* =====================================================
   NAVIGATION
===================================================== */

nav {
    position: sticky;
    top: 0;
    z-index: 1000;

    width: 100%;

    background: rgba(255, 255, 255, 0.97);

    border-bottom: 1px solid #e4d8f0;

    box-shadow:
        0 3px 15px rgba(75, 45, 100, 0.08);
}

.nav-container {
    width: 100%;
    max-width: 1100px;

    margin: 0 auto;

    padding: 14px 25px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: #7137a5;

    text-decoration: none;

    font-size: 1.2rem;
    font-weight: bold;

    white-space: nowrap;
}

nav ul {
    list-style: none;

    display: flex;
    gap: 25px;
}

nav ul li a {
    color: #51425e;

    text-decoration: none;

    font-size: 0.9rem;
    font-weight: bold;

    transition: color 0.2s ease;
}

nav ul li a:hover {
    color: #7137a5;
}


/* =====================================================
   HERO
===================================================== */

.hero {
    position: relative;

    width: 100%;
    min-height: 80vh;

    display: flex;
    align-items: center;

    color: white;

    /* IMPORTANT:
       Prevent the background from acting fixed */
    background-image:
        linear-gradient(
            rgba(91, 45, 135, 0.88),
            rgba(139, 78, 183, 0.82)
        ),
        url("https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1600&q=85");

    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: scroll;
}

.hero-content {
    width: 100%;
    max-width: 1100px;

    margin: 0 auto;

    padding: 80px 25px;
}

.tag {
    display: inline-block;

    padding: 7px 15px;

    border: 1px solid rgba(255, 255, 255, 0.6);

    border-radius: 50px;

    background: rgba(255, 255, 255, 0.13);

    font-size: 0.8rem;
    font-weight: bold;

    margin-bottom: 20px;
}

.hero h1 {
    width: 100%;
    max-width: 800px;

    font-size: clamp(2.5rem, 7vw, 5rem);

    margin-bottom: 25px;
}

.hero p {
    width: 100%;
    max-width: 700px;

    font-size: 1.15rem;

    margin-bottom: 30px;
}

.button {
    display: inline-block;

    padding: 12px 22px;

    background: white;
    color: #7137a5;

    border-radius: 50px;

    text-decoration: none;
    font-weight: bold;

    transition:
        transform 0.25s ease,
        box-shadow 0.25s ease;
}

.button:hover {
    transform: translateY(-3px);

    box-shadow:
        0 8px 20px rgba(0, 0, 0, 0.2);
}


/* =====================================================
   GENERAL CONTAINER
===================================================== */

.container {
    width: 100%;
    max-width: 1100px;

    margin: 0 auto;

    padding: 75px 25px;
}

.section-title {
    width: 100%;
    max-width: 750px;

    text-align: center;

    margin: 0 auto 45px;
}

.section-title span {
    color: #7137a5;

    font-size: 0.8rem;

    font-weight: bold;

    text-transform: uppercase;

    letter-spacing: 2px;
}

.section-title h2 {
    color: #43245c;

    font-size: 2.5rem;

    margin: 10px 0 15px;
}

.section-title p {
    color: #74677d;
}


/* =====================================================
   INTRODUCTION
===================================================== */

.intro-box {
    width: 100%;

    background: white;

    padding: 35px;

    border-radius: 22px;

    border: 1px solid #e5d8ef;

    box-shadow:
        0 10px 30px rgba(92, 52, 125, 0.08);
}

.highlight {
    color: #7137a5;
    font-weight: bold;
}


/* =====================================================
   TWO COLUMN FEATURES
===================================================== */

.feature {
    width: 100%;

    display: grid;

    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);

    gap: 45px;

    align-items: center;

    margin-top: 45px;
}

.feature > div {
    min-width: 0;
}

.feature.reverse .feature-image {
    order: 2;
}

.feature-image {
    width: 100%;
}

.feature-image img {
    width: 100%;
    height: 360px;

    object-fit: cover;

    display: block;

    border-radius: 22px;

    box-shadow:
        0 15px 35px rgba(92, 52, 125, 0.15);
}

.caption {
    width: 100%;

    text-align: center;

    color: #81758a;

    font-size: 0.85rem;

    margin-top: 10px;
}

.feature h3 {
    color: #7137a5;

    font-size: 1.5rem;

    margin-bottom: 15px;
}


/* =====================================================
   CARDS
===================================================== */

.cards {
    width: 100%;

    display: grid;

    grid-template-columns:
        repeat(3, minmax(0, 1fr));

    gap: 20px;

    margin-top: 30px;
}

.card {
    min-width: 0;

    background: white;

    padding: 27px;

    border-radius: 18px;

    border: 1px solid #e5d8ef;

    box-shadow:
        0 8px 24px rgba(92, 52, 125, 0.06);

    transition:
        transform 0.25s ease,
        box-shadow 0.25s ease;
}

.card:hover {
    transform: translateY(-6px);

    box-shadow:
        0 15px 30px rgba(92, 52, 125, 0.13);
}

.number {
    width: 45px;
    height: 45px;

    display: grid;
    place-items: center;

    border-radius: 50%;

    background: #eee2fa;

    color: #7137a5;

    font-weight: bold;

    margin-bottom: 17px;
}

.card h3 {
    color: #7137a5;

    margin-bottom: 10px;
}


/* =====================================================
   STRATEGIES
===================================================== */

.strategies {
    width: 100%;

    display: grid;

    gap: 15px;

    margin-top: 30px;
}

.strategy {
    width: 100%;

    background: white;

    padding: 22px;

    border-radius: 15px;

    border-left: 5px solid #9b59c6;

    box-shadow:
        0 5px 18px rgba(92, 52, 125, 0.06);

    transition: transform 0.2s ease;
}

.strategy:hover {
    transform: translateX(5px);
}

.strategy strong {
    display: block;

    color: #43245c;

    font-size: 1.05rem;

    margin-bottom: 5px;
}


/* =====================================================
   HABIT LIST
===================================================== */

.habit-list {
    padding-left: 25px;

    margin-top: 20px;
}

.habit-list li {
    margin-bottom: 10px;
}

.habit-list li::marker {
    color: #8e44ad;
}


/* =====================================================
   CALL TO ACTION
===================================================== */

.cta {
    width: 100%;

    margin-top: 50px;

    padding: 45px;

    border-radius: 25px;

    color: white;

    background:
        linear-gradient(
            135deg,
            #7137a5,
            #a05dcc
        );

    box-shadow:
        0 15px 35px rgba(113, 55, 165, 0.25);
}

.cta h2 {
    color: white;

    margin-bottom: 15px;
}

.cta p {
    max-width: 800px;
}

.cta .button {
    margin-top: 10px;
}


/* =====================================================
   REFERENCES
===================================================== */

.references {
    width: 100%;

    background: #321b43;

    color: #e9dff0;
}

.references .section-title h2 {
    color: white;
}

.references .section-title span {
    color: #d9b8ed;
}

.references .section-title p {
    color: #d3c3dc;
}

.references ul {
    width: 100%;

    padding-left: 25px;
}

.references li {
    margin-bottom: 13px;
}

.references a {
    color: #d9b8ed;

    font-weight: bold;
}

.references a:hover {
    color: white;
}


/* =====================================================
   GROUP INFORMATION
===================================================== */

.group-info {
    width: 100%;

    background: #f7f2fc;
}

.group-box {
    width: 100%;

    background: #ffffff;

    padding: 40px;

    border-radius: 24px;

    border: 1px solid #e5d8ef;

    box-shadow:
        0 12px 35px rgba(92, 52, 125, 0.10);
}


/* GROUP TITLE */

.group-heading {
    display: flex;

    align-items: center;

    gap: 18px;

    margin-bottom: 35px;
}

.group-heading h2 {
    color: #43245c;

    font-size: 2.3rem;
}

.group-icon {
    width: 14px;
    height: 38px;

    display: block;

    border-radius: 20px;

    background: linear-gradient(
        180deg,
        #7137a5,
        #a05dcc
    );
}


/* BASIC DETAILS */

.group-details {
    display: grid;

    grid-template-columns:
        repeat(3, minmax(0, 1fr));

    gap: 20px;

    margin-bottom: 45px;
}

.detail {
    padding: 20px;

    background: #f7f2fc;

    border-radius: 15px;

    border: 1px solid #e5d8ef;
}

.detail strong {
    display: block;

    color: #7137a5;

    font-size: 1rem;

    margin-bottom: 5px;
}

.detail span {
    color: #30243d;

    font-size: 1rem;
}


/* MEMBERS TITLE */

.members-title {
    color: #7137a5;

    font-size: 1.6rem;

    margin-bottom: 22px;
}


/* MEMBERS GRID */

.members-grid {
    display: grid;

    grid-template-columns:
        repeat(3, minmax(0, 1fr));

    gap: 15px;
}

.member-card {
    min-width: 0;

    padding: 18px 20px;

    background: #faf8f4;

    border: 1px solid #e5d8ef;

    border-radius: 15px;

    transition:
        transform 0.2s ease,
        box-shadow 0.2s ease;
}

.member-card:hover {
    transform: translateY(-4px);

    box-shadow:
        0 8px 20px rgba(92, 52, 125, 0.10);
}

.member-card strong {
    display: block;

    color: #43245c;

    font-size: 1.05rem;

    margin-bottom: 3px;
}

.member-card span {
    color: #74677d;

    font-size: 0.9rem;
}


/* =====================================================
   GROUP INFORMATION - TABLET
===================================================== */

@media (max-width: 800px) {

    .group-box {
        padding: 30px;
    }

    .group-details {
        grid-template-columns: 1fr 1fr;
    }

    .members-grid {
        grid-template-columns: 1fr 1fr;
    }

}


/* =====================================================
   GROUP INFORMATION - MOBILE
===================================================== */

@media (max-width: 600px) {

    .group-box {
        padding: 25px 20px;

        border-radius: 20px;
    }

    .group-heading {
        gap: 12px;

        margin-bottom: 25px;
    }

    .group-heading h2 {
        font-size: 1.8rem;
    }

    .group-icon {
        width: 10px;
        height: 32px;
    }

    .group-details {
        grid-template-columns: 1fr;

        gap: 12px;

        margin-bottom: 35px;
    }

    .detail {
        padding: 17px;
    }

    .members-title {
        font-size: 1.4rem;
    }

    .members-grid {
        grid-template-columns: 1fr 1fr;

        gap: 12px;
    }

    .member-card {
        padding: 16px 14px;
    }

    .member-card strong {
        font-size: 0.95rem;
    }

    .member-card span {
        font-size: 0.82rem;
    }

}


/* =====================================================
   VERY SMALL PHONES
===================================================== */

@media (max-width: 380px) {

    .members-grid {
        grid-template-columns: 1fr;
    }

}


/* =====================================================
   FOOTER
===================================================== */

footer {
    width: 100%;

    text-align: center;

    padding: 25px 20px;

    background: #241330;

    color: #cdbbd5;

    font-size: 0.85rem;
}

footer p {
    margin-bottom: 5px;
}


/* =====================================================
   TABLET
===================================================== */

@media (max-width: 800px) {

    .nav-container {
        padding: 14px 20px;
    }

    nav ul {
        display: none;
    }

    .hero {
        min-height: 75vh;
    }

    .hero-content {
        padding: 70px 20px;
    }

    .hero h1 {
        font-size: clamp(2.4rem, 9vw, 4rem);
    }

    .hero p {
        font-size: 1.05rem;
    }

    .container {
        padding: 65px 20px;
    }

    .feature,
    .feature.reverse {
        grid-template-columns: 1fr;

        gap: 30px;
    }

    .feature.reverse .feature-image {
        order: 0;
    }

    .feature-image img {
        height: 320px;
    }

    .cards {
        grid-template-columns: 1fr;
    }

    .intro-box,
    .cta {
        padding: 30px;
    }

    .section-title h2 {
        font-size: 2.1rem;
    }
}


/* =====================================================
   MOBILE
===================================================== */

@media (max-width: 600px) {

    body {
        font-size: 0.95rem;
    }

    .logo {
        font-size: 1.05rem;
    }

    .hero {
        min-height: auto;

        background-position: center;
    }

    .hero-content {
        padding: 70px 18px;
    }

    .tag {
        margin-bottom: 18px;
    }

    .hero h1 {
        font-size: 2.6rem;

        line-height: 1.12;

        margin-bottom: 20px;
    }

    .hero p {
        font-size: 1rem;

        line-height: 1.6;
    }

    .button {
        padding: 11px 19px;
    }

    .container {
        padding: 55px 18px;
    }

    .section-title {
        margin-bottom: 30px;
    }

    .section-title h2 {
        font-size: 1.9rem;
    }

    .section-title span {
        font-size: 0.72rem;
    }

    .intro-box {
        padding: 25px 20px;

        border-radius: 18px;
    }

    .feature {
        margin-top: 35px;
    }

    .feature-image img {
        height: 250px;

        border-radius: 18px;
    }

    .feature h3 {
        font-size: 1.35rem;
    }

    .card {
        padding: 23px;
    }

    .strategy {
        padding: 20px;

        border-left-width: 4px;
    }

    .cta {
        margin-top: 35px;

        padding: 27px 22px;

        border-radius: 20px;
    }

    .cta h2 {
        font-size: 1.45rem;
    }

    .references .container {
        padding: 55px 20px;
    }

    footer {
        padding: 22px 18px;

        font-size: 0.78rem;
    }
}


/* =====================================================
   VERY SMALL PHONES
===================================================== */

@media (max-width: 380px) {

    .hero-content {
        padding: 55px 16px;
    }

    .hero h1 {
        font-size: 2.25rem;
    }

    .hero p {
        font-size: 0.92rem;
    }

    .container {
        padding-left: 16px;
        padding-right: 16px;
    }

    .section-title h2 {
        font-size: 1.7rem;
    }

    .intro-box {
        padding: 22px 18px;
    }

    .feature-image img {
        height: 220px;
    }

    .cta {
        padding: 24px 18px;
    }
}

</style>
</head>


<body>


<!-- =====================================================
     NAVIGATION
===================================================== -->

<nav>

<div class="nav-container">

<a href="#home" class="logo">
Digital Well-Being
</a>

<ul>

<li>
<a href="#about">About</a>
</li>

<li>
<a href="#burnout">Burnout</a>
</li>

<li>
<a href="#strategies">Strategies</a>
</li>

<li>
<a href="#habits">Digital Habits</a>
</li>

<li>
<a href="#references">Sources</a>
</li>

</ul>

</div>

</nav>


<!-- =====================================================
     HERO
===================================================== -->

<header class="hero" id="home">

<div class="hero-content">

<span class="tag">
Digital Balance
</span>

<h1>
Mindful Scrolling &
<br>
Responsible Technology Use
</h1>

<p>
Technology connects us, helps us learn, and makes
everyday life easier. Learn how to use technology
responsibly while maintaining a healthy balance
between online and offline life.
</p>

<a href="#about" class="button">
Explore the Guide ↓
</a>

</div>

</header>


<!-- =====================================================
     MAIN
===================================================== -->

<main>


<!-- =====================================================
     INTRODUCTION
===================================================== -->

<section class="container" id="about">

<div class="section-title">

<span>
01 • Introduction
</span>

<h2>
What Is Digital Well-being?
</h2>

<p>
A healthy relationship with technology
starts with awareness.
</p>

</div>


<div class="intro-box">

<p>
In today's world, digital technology is part of
everyday life. Students use phones, computers,
and the internet for communication, schoolwork,
entertainment, and social connection.
</p>

<p>
While technology offers many benefits, spending
too much time online or using devices without
healthy boundaries can affect focus, rest,
and everyday routines.
</p>

<p>
<span class="highlight">
Digital well-being
</span>
means using technology in a way that supports
your goals, relationships, safety, and overall
quality of life.
</p>

</div>


<div class="feature">

<div class="feature-image">

<img
src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1000&q=85"
alt="Student using a laptop">

<p class="caption">
Technology works best when it supports—not controls—our daily lives.
</p>

</div>


<div>

<h3>
Why Does It Matter?
</h3>

<p>
Responsible technology use helps people become
more intentional about where their time and
attention go.
</p>

<p>
Small changes, such as taking breaks,
turning off unnecessary notifications,
and spending time offline, can make
digital activities more manageable.
</p>

<p>
Digital well-being also encourages
responsible digital citizenship:
communicating respectfully, protecting
personal information, and thinking carefully
before sharing information online.
</p>

</div>

</div>

</section>


<!-- =====================================================
     DIGITAL BURNOUT
===================================================== -->

<section class="container" id="burnout">

<div class="section-title">

<span>
02 • Awareness
</span>

<h2>
Understanding Digital Burnout
& Screen Fatigue
</h2>

<p>
Recognizing digital strain is the first step
toward healthier technology habits.
</p>

</div>


<div class="cards">

<article class="card">

<div class="number">
01
</div>

<h3>
Physical Discomfort
</h3>

<p>
Long periods of screen use may be associated
with tired eyes, headaches, neck discomfort,
or poor posture.
</p>

</article>


<article class="card">

<div class="number">
02
</div>

<h3>
Sleep Disruption
</h3>

<p>
Using devices late at night can make it
harder to wind down. Creating a calmer
screen-free routine before sleep may help.
</p>

</article>


<article class="card">

<div class="number">
03
</div>

<h3>
Mental Fatigue
</h3>

<p>
Constant notifications and multitasking
can make it difficult to focus and may
leave users feeling mentally tired.
</p>

</article>

</div>


<div class="feature reverse">

<div class="feature-image">

<img
src="https://images.unsplash.com/photo-1512428559087-560fa5ceab42?auto=format&fit=crop&w=1000&q=85"
alt="Person using a smartphone">

<p class="caption">
Being aware of screen habits can help us make better digital choices.
</p>

</div>


<div>

<h3>
Pause. Notice. Reset.
</h3>

<p>
Instead of automatically checking every
notification, pause and ask whether checking
it is actually necessary.
</p>

<p>
A simple reset can be as easy as standing
up, looking away from the screen, drinking
water, talking to someone, or spending
a few minutes doing an offline activity.
</p>

</div>

</div>

</section>


<!-- =====================================================
     STRATEGIES
===================================================== -->

<section class="container" id="strategies">

<div class="section-title">

<span>
03 • Practical Guide
</span>

<h2>
Strategies for Responsible
Technology Use
</h2>

<p>
Simple habits can help you take control
of your digital routine.
</p>

</div>


<div class="strategies">

<div class="strategy">

<strong>
1. Audit Your Screen Time
</strong>

<p>
Check your device's screen-time report.
Notice which apps take the most time and
decide whether that use matches your priorities.
</p>

</div>


<div class="strategy">

<strong>
2. Create Phone-Free Zones
</strong>

<p>
Choose specific moments—such as meals,
study sessions, or conversations—when
you keep your phone away.
</p>

</div>


<div class="strategy">

<strong>
3. Silence Non-Essential Notifications
</strong>

<p>
Turn off unnecessary alerts. Fewer
interruptions can make it easier to
concentrate.
</p>

</div>


<div class="strategy">

<strong>
4. Practice the 20-20-20 Rule
</strong>

<p>
During extended screen use, every 20 minutes,
look at something about 20 feet away for
at least 20 seconds.
</p>

</div>


<div class="strategy">

<strong>
5. Make Time for Offline Activities
</strong>

<p>
Balance online activities with hobbies,
reading, exercise, creative activities,
family time, and face-to-face conversations.
</p>

</div>

</div>

</section>


<!-- =====================================================
     DIGITAL HABITS
===================================================== -->

<section class="container" id="habits">

<div class="section-title">

<span>
04 • Digital Citizenship
</span>

<h2>
Cultivating Positive Digital Habits
</h2>

<p>
Digital well-being is also about the quality
of our online interactions.
</p>

</div>


<div class="feature">

<div>

<h3>
Make Your Digital Space Better
</h3>

<p>
Responsible technology use includes creating
a healthier online environment. Follow accounts
that provide useful or positive content and
think before posting or sharing.
</p>


<ul class="habit-list">

<li>
Protect your passwords and personal information.
</li>

<li>
Think critically before believing or sharing information.
</li>

<li>
Communicate respectfully online.
</li>

<li>
Use privacy and safety settings when available.
</li>

<li>
Take breaks when online activity becomes overwhelming.
</li>

</ul>

</div>


<div class="feature-image">

<img
src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=1000&q=85"
alt="Students communicating with each other">

<p class="caption">
Healthy digital habits leave room for meaningful
real-world connections.
</p>

</div>

</div>


<!-- =====================================================
     CALL TO ACTION
===================================================== -->

<div class="cta">

<h2>
Take the Digital Wellness Challenge
</h2>

<p>
For one day, choose one small digital habit
to improve. Try turning off unnecessary
notifications, taking regular screen breaks,
or keeping your phone away during a meal
or study session.
</p>

<p>

<strong>
Reflection:
</strong>

Does the way you use technology help you
reach your goals, or is it sometimes
distracting you from them?

</p>

<a href="#references" class="button">
View Reliable Sources
</a>

</div>

</section>

</main>


<!-- =====================================================
     REFERENCES
===================================================== -->

<section class="references" id="references">

<div class="container">

<div class="section-title">

<span>
05 • References
</span>

<h2>
Reliable Sources
</h2>

<p>
Explore these organizations for more information
about digital well-being and online safety.
</p>

</div>
 

<ul>

<li>
Center for Humane Technology
<a
href="https://www.humanetech.com/"
target="_blank"
rel="noopener noreferrer">
Humanetech.com
</a>
</li>


<li>
World Health Organization
<a
href="https://www.who.int/"
target="_blank"
rel="noopener noreferrer">
WHO Official Website
</a>
</li>


<li>
UNICEF
<a
href="https://wwww.unicef.org/"
target="_blank"
rel="noopener noreferrer">
UNICEF Official Website
</a>
</li>

</ul>

</div>

</section>


<!-- =====================================================
     GROUP INFORMATION
===================================================== -->

<section class="group-info">

<div class="container">

<div class="group-box">

<div class="group-heading">

<span class="group-icon"></span>

<h2>
Group Information
</h2>

</div>


<!-- BASIC INFORMATION -->

<div class="group-details">

<div class="detail">

<strong>Section:</strong>

<span>
12 STEM 3
</span>

</div>


<div class="detail">

<strong>Subject:</strong>

<span>
Empowerment Technology
</span>

</div>


<div class="detail">

<strong>Group Number:</strong>

<span>
Group No. 4
</span>

</div>

</div>


<!-- MEMBERS -->

<h3 class="members-title">
Group Members & Roles
</h3>


<div class="members-grid">


<div class="member-card">

<strong>Valle</strong>

<span>Group Leader</span>

</div>


<div class="member-card">

<strong>Jadjuri</strong>

<span>Content Writer</span>

</div>


<div class="member-card">

<strong>Basay</strong>

<span>HTML/CSS Developer</span>

</div>


<div class="member-card">

<strong>Añabieza</strong>

<span>Media Designer</span>

</div>


<div class="member-card">

<strong>Malinas</strong>

<span>Media Designer</span>

</div>


<div class="member-card">

<strong>Cagang</strong>

<span>Content Researcher</span>

</div>


<div class="member-card">

<strong>Reston</strong>

<span>Media Designer</span>

</div>


<div class="member-card">

<strong>Alcontin</strong>

<span>Media Designer</span>

</div>


<div class="member-card">

<strong>Sedra</strong>

<span>Publisher</span>

</div>


</div>

</div>

</div>

</section>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

<p>
Digital Well-being & Responsible Technology Use
• HTML webpage project.
</p>

<p>
Created by 12-Stem 3 Students for Emptech-Mr Dagatan.
</p>

</footer>


</body>
</html>
