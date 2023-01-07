### Hi there 👋

<!--
**Yanoe7014/Yanoe7014** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<style>
  *,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 16px;

  --bg-peach: #f7dbc6;
  --bg-body: #9d7667;
  --bg-red: #ad3939;
  --bg-light: #fff;

  --bg-forum: #844949;
  --bg-forum-dark: #723c3c;
  --bg-guidebook: #611b1b;
  --bg-guidebook-lighter: #8f3d3d;
  /* bg-guidebook-rgb: rgb(95, 27, 27); */

  --svg-dark: #77270e;
  --svg-light: #d3901d;

  --text-light: #fff;
  --text-dark: #999;

  --font-display: "Bebas Neue", cursive;
}

body {
  background-color: var(--bg-body);
  line-height: 150%;
  font-family: "Gudea", Arial, Helvetica, sans-serif;
  color: var(--text-light);
}

main {
  background-color: var(--bg-light);
  max-width: 1300px;
  margin: 5vw auto;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  flex-direction: column;
}

.maintitle {
  background-color: var(--bg-red);
  width: 100%;
  padding: 3rem;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  position: relative;
  overflow: hidden;
}

.maintitle__name {
  width: 100%;
  color: var(--text-light);
  font-family: var(--font-display);
  font-size: 2.25rem;
  letter-spacing: 2px;
  position: relative;
}

.maintitle__name::after {
  content: "ワンパンマン";
  width: 100%;
  top: 0;
  left: 1.5rem;
  color: var(--text-light);
  font-family: var(--font-display);
  opacity: 0.15;
  font-size: 4rem;
  position: absolute;
  z-index: 2;
}

.maintitle__svg {
  opacity: 0.75;
  position: absolute;
  top: 0;
  right: 0;
  display: block;
}

.maintitle__svg-gradient {
  background: linear-gradient(to right, var(--bg-red), transparent);
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  z-index: 1;
}

.maintitle__svg,
.maintitle__svg-gradient {
  width: 60%;
}

.maintitle__svg-1,
.forum-row__guidebook__image-svg-1 {
  fill: var(--svg-dark);
}

.maintitle__svg-2,
.forum-row__guidebook__image-svg-2 {
  fill: var(--svg-light);
}

.forum-row {
  width: 100%;
  height: 740px;
  display: grid;
  grid-template-columns: 0.75fr 1fr;
  grid-template-rows: 1fr 1fr;
  padding: 8px;
  gap: 8px 8px;
  grid-template-areas:
    "guidebook announcements"
    "guidebook moderation";
}

.forum-row__guidebook {
  background-color: var(--bg-guidebook);
  position: relative;
  grid-area: guidebook;
}

.forum-row__guidebook-grid {
  width: 100%;
  height: 100%;
  display: grid;
  grid-template-columns: 3.5fr 1fr;
  grid-template-rows: 0.45fr 1fr;
  gap: 0px 0px;
  grid-template-areas:
    "guidebook-name guidebook-name"
    "guidebook-img guidebook-links";
  overflow: hidden;
}

.forum-row__guidebook-name {
  width: 100%;
  height: 90%;
  padding: 1.5rem;
  display: flex;
  align-items: center;
  font-family: var(--font-display);
  letter-spacing: 13px;
  font-size: 6rem;
  grid-area: guidebook-name;
}

.forum-row__guidebook-name a {
  width: 100%;
  height: 100%;
  line-height: 100%;
  color: var(--bg-light);
  text-decoration: none;
  transition: 0.5s color ease-out;
}

.forum-row__guidebook a:hover,
.forum-row__guidebook a:focus {
  color: var(--text-dark);
  transition: 0.3s color ease-in;
}

.forum-row__guidebook-name-guide,
.forum-row__guidebook-name-book {
  width: 100%;
  position: relative;
  z-index: 4;
  text-align: right;
}

.forum-row__guidebook-name-guide {
  padding-right: 5rem;
}

.forum-row__guidebook-name-guide::after {
  content: "";
  background-color: var(--svg-light);
  width: 60%;
  height: 5rem;
  position: absolute;
  z-index: -1;
  bottom: -50%;
  left: 10%;
  opacity: 0.25;
}

.forum-row__guidebook__image {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  grid-area: guidebook-img;
}

.forum-row__guidebook__image-svg {
  position: absolute;
  bottom: 0;
  left: 0;
  z-index: 2;
}

.forum-row__guidebook__image-svg,
.forum-row__guidebook__image__svg-gradient {
  width: 100%;
  bottom: -10%;
}

.forum-row__guidebook__image__svg-gradient {
  background: linear-gradient(to bottom, var(--bg-guidebook), transparent);
  height: 100%;
  position: absolute;
  right: 0;
  z-index: 3;
}

.forum-row__guidebook__image img {
  position: absolute;
  bottom: 0;
  left: -5%;
  height: 74%;
  z-index: 5;
}

.forum-row__guidebook__links {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  position: relative;
  z-index: 4;
  grid-area: guidebook-links;
}

.forum-row__guidebook__links a {
  width: 4rem;
  height: 4rem;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 1.5rem 0;
  text-decoration: none;
  color: var(--bg-peach);
}

.forum-row__guidebook__links div {
  border: 1px solid var(--bg-peach);
  width: 3.5rem;
  height: 3.5rem;
  font-size: 1.75rem;
  display: flex;
  align-items: center;
  justify-content: center;
  transform: rotate(45deg);
}

.forum-row__guidebook__links div i {
  transform: rotate(-45deg);
}

.forum-row__guidebook__links a:hover > div,
.forum-row__guidebook__links a:focus > div {
  animation-name: guidebook-link;
  animation-duration: 0.25s;
}

.forum-row__flex {
  width: 100%;
  height: 100%;
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.forum-row__announcements {
  grid-area: announcements;
}

.forum-row__moderation {
  grid-area: moderation;
}

.forum-row__announcements,
.forum-row__moderation {
  background: linear-gradient(
    to right,
    var(--bg-forum),
    var(--bg-guidebook-lighter)
  );
}

.forum-row__announcements,
.forum-row__moderation {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 0.8fr 0.65fr 0.65fr;
  gap: 0px 0px;
  grid-template-areas:
    "forumtitle"
    "forumdesc"
    "forumlast";
  position: relative;
  overflow: hidden;
}

.forum-row_title {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 0 0 0 2rem;
  position: relative;
  z-index: 2;
  grid-area: forumtitle;
}

.forum-row_title-name {
  font-family: var(--font-display);
  font-size: 4.5rem;
  letter-spacing: 2px;
  position: relative;
  z-index: 2;
}

.forum-row_title-name::after {
  content: "";
  background-color: var(--svg-light);
  width: 45%;
  height: 1rem;
  position: absolute;
  top: 0;
  right: -20%;
  opacity: 0.25;
  z-index: -1;
}

.forum-row_title-name a {
  color: var(--text-light);
  text-decoration: none;
}

.forum-row_title-stats {
  text-transform: lowercase;
  font-size: 1rem;
  letter-spacing: 1px;
  font-weight: 100;
  margin-bottom: 1.25rem;
  padding-left: 0.5rem;
}

.forum-row__desc {
  display: flex;
  align-items: center;
  justify-content: center;
  grid-area: forumdesc;
}

.forum-row_desc-box {
  width: 100%;
  max-height: 100%;
  padding: 0 3rem 0 4rem;
  display: flex;
  align-items: flex-start;
  overflow: auto;
  position: relative;
  text-align: justify;
  font-size: 1.1rem;
}

.forum-row_desc-box::before {
  content: "";
  background-color: var(--svg-light);
  width: 1rem;
  height: 100%;
  position: absolute;
  top: 0;
  left: 1.5rem;
  opacity: 0.25;
}

.forum-row_last {
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0 3rem;
  grid-area: forumlast;
}

.forum-row_last-date-topic {
  margin-bottom: 0.5rem;
  font-size: 2.25rem;
}

.forum-row_last-date-topic a,
.forum-row_last-date-name a:hover,
.forum-row_last-date-name a:focus {
  color: var(--text-light);
  text-decoration: none;
}

.forum-row_last-date {
  height: 100%;
  display: flex;
  align-items: flex-end;
  justify-content: center;
  flex-direction: column;
}

.forum-row_last-date-name a,
.forum-row_last-date-topic a:hover,
.forum-row_title-name a:hover,
.forum-row_last-date-topic a:focus,
.forum-row_title-name a:focus {
  color: var(--bg-peach);
  text-decoration: none;
}

.forum-row_last-avatar {
  height: 100%;
  display: flex;
  align-items: center;
}

.forum-row_last-avatar-diamond {
  outline: 1px solid var(--bg-peach);
  outline-offset: 0.25rem;
  width: 45px;
  height: 45px;
  transform: rotate(45deg);
  position: relative;
  left: 0.25rem;
  overflow: hidden;
}

.forum-row_last-avatar-diamond img {
  width: 150%;
  height: 150%;
  position: relative;
  top: -30%;
  left: -25%;
  transform: rotate(-45deg);
}

.forum-row_title,
.forum-row__desc,
.forum-row_last-date,
.forum-row_last-avatar {
  position: relative;
  z-index: 2;
}

.forum-row_svg {
  position: absolute;
  bottom: -20%;
  left: 0;
  width: 100%;
  opacity: 0.25;
}

.forum-row_svg-1 {
  fill: var(--svg-dark);
}

.forum-row_svg-2 {
  fill: var(--svg-light);
}

.forum-row__img-1,
.forum-row__img-2 {
  position: absolute;
  height: 100%;
  bottom: 0;
  right: 0;
  opacity: 0.03;
}

@keyframes guidebook-link {
  0% {
    transform: rotate(45deg);
  }
  25% {
    transform: rotate(60deg);
  }
  75% {
    transform: rotate(30deg);
  }
  90% {
    transform: rotate(55deg);
  }
  100% {
    transform: rotate(45deg);
  }
}

@media (max-width: 1280px) {
  main {
    width: 90vw;
    height: auto;
  }

  .forum-row__guidebook__image img {
    position: absolute;
    bottom: 0;
    height: 95%;
    left: 0;
  }
  .maintitle__svg,
  .maintitle__svg-gradient,
  .forum-row__guidebook__image-svg,
  .forum-row__guidebook__image__svg-gradient {
    display: none;
  }
  .forum-row {
    height: auto;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-template-areas:
      "guidebook"
      "announcements"
      "moderation";
    gap: 8px;
  }
  .forum-row__guidebook-name {
    font-size: 7rem;
    letter-spacing: 8px;
    justify-content: center;
  }
  .forum-row__guidebook-name a {
    display: flex;
    justify-content: center;
  }
  .forum-row__guidebook-name-guide {
    padding: 0;
  }
  .forum-row__guidebook-name-book {
    text-align: left;
  }
  .forum-row__guidebook__links {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
  }
  .forum-row__guidebook__links a {
    margin: 0 1.5rem;
  }
  .forum-row__guidebook-name-guide::after {
    left: 50%;
    bottom: -100%;
  }
  .forum-row__announcements,
  .forum-row__moderation {
    grid-template-rows: 0.45fr 0.65fr 0.5fr;
    overflow: hidden;
    margin: 0;
  }
  .forum-row_title-name {
    font-size: 3.25rem;
  }
  .forum-row__img-1,
  .forum-row__img-2 {
    display: none;
  }
  .forum-row_last-date-topic {
    font-size: 2rem;
  }
}

@media (max-width: 900px) {
  .forum-row__guidebook__image img {
    height: 90%;
    left: -5%;
  }

  main {
    width: 98vw;
  }
}

@media (max-width: 680px) {
  main {
    width: 100%;
    margin: auto;
  }
  .maintitle__name {
    text-align: center;
    font-size: 1.75rem;
  }
  .maintitle__name::after {
    font-size: 3rem;
    left: 0;
  }
  .forum-row {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .forum-row__guidebook-name {
    font-size: 4rem;
    letter-spacing: 3px;
  }
  .forum-row__guidebook__image img {
    height: 80%;
  }
  .forum-row__guidebook__links {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    margin-bottom: 2rem;
  }
  .forum-row__guidebook__links a {
    margin: 1.5rem 0;
  }
  .forum-row__guidebook-name-guide::after {
    display: none;
  }
  .forum-row__announcements,
  .forum-row__moderation {
    padding: 2rem 0;
    display: flex;
    flex-direction: column;
    gap: 3rem;
  }
  .forum-row_last-avatar {
    margin-bottom: 2rem;
  }
  .forum-row_last {
    width: 100%;
    padding: 0;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .forum-row_last-date {
    align-items: center;
  }
  .forum-row__guidebook__links {
    z-index: 6;
  }
}

@media (max-width: 550px) {
  .forum-row__guidebook__image img {
    height: 75%;
  }
  .maintitle__name::after {
    font-size: 2.5rem;
    left: 0;
  }
}
  </style>
  <meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Gudea:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/remixicon@2.5.0/fonts/remixicon.css" rel="stylesheet">
<main>
  <div class="maintitle">
    <div class="maintitle__name">
      001. category name
    </div>
    <svg class="maintitle__svg" version="1.1" viewBox="167 0 733 600" xmlns="http://www.w3.org/2000/svg">
      <path class="maintitle__svg-1" d="m434 600h-173v-33h237v-34h-263v-33h169v-33h-120v-34h-50v-33h184v-33h-184v-34h284v-33h-6v-33h32v-34h-365v-33h48v-33h-60v-34h370v-33h-254v-33h-51v-34h205v-33h463v33 34 33 33 34 33 33 34 33 33 34 33 33 34 33 33 34 33z" />
      <path class="maintitle__svg-2" d="m451 600h196v-33h11v-34h4v-33h-59v-33h2v-34h-141v-33h138v-33h160v-34h-223v-33h-45v-33h-73v-34h212v-33h-17v-33h-3v-34h-2v-33h-91v-33h210v-34h-300v-33h470v33 34 33 33 34 33 33 34 33 33 34 33 33 34 33 33 34 33z" />
    </svg>
    <div class="maintitle__svg-gradient"></div>
  </div>

  <div class="forum-row">
    <div class="forum-row__guidebook">
      <div class="forum-row__guidebook-grid">
        <div class="forum-row__guidebook-name">
          <a href="#" title="guidebook">
            <div class="forum-row__guidebook-name-guide">guide</div>
            <div class="forum-row__guidebook-name-book">book</div>
          </a>
        </div>
        <div class="forum-row__guidebook__image">
          <img src="https://img.nickpic.host/qePAVD.png" alt="saitama">
          <svg version="1.1" class="forum-row__guidebook__image-svg" viewBox="0 166 675 735" xmlns="http://www.w3.org/2000/svg">
            <path d="m0 166h52v241h52v2h52v117h52v-51h52v-220h52v192h51v-180h52v7h52v36h52v65h52v163h52v-46h52v69 340h-52-52-52-52-52-52-51-52-52-52-52-52-52z" class="forum-row__guidebook__image-svg-1" />
            <path d="m0 535h52v155h52v66h52v-71h52v-143h52v18h52v107h51v-243h52v265h52v-235h52v135h52v11h52v72h52v-244 473h-52-52-52-52-52-52-51-52-52-52-52-52-52z" class="forum-row__guidebook__image-svg-2" />
          </svg>
          <div class="forum-row__guidebook__image__svg-gradient"></div>
        </div>
        <div class="forum-row__guidebook__links">
          <a href="#" title="smth-important">
            <div>
              <i class="ri-pencil-line"></i>
            </div>
          </a>
          <a href="#" title="smth-important">
            <div>
              <i class="ri-pencil-line"></i>
            </div>
          </a>
          <a href="#" title="smth-important">
            <div>
              <i class="ri-pencil-line"></i>
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="forum-row__announcements">
      <div class="forum-row_title">
        <span class="forum-row_title-stats">
          0 topics. 0 replies.
        </span>
        <span class="forum-row_title-name">
          <a href="#" title="announcements">
            announcements
          </a>
        </span>
      </div>
      <div class="forum-row__desc">
        <div class="forum-row_desc-box">
          <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, voluptates rem. Quibusdam fugiat officiis nihil voluptate, vero, perferendis porro iure deleniti fugit architecto, at tempora maiores et quam dolore distinctio?</P>
        </div>
      </div>
      <div class="forum-row_last">
        <div class="forum-row_last-avatar">
          <div class="forum-row_last-avatar-diamond">
            <img src="https://icon-library.com/images/saitama-icon/saitama-icon-6.jpg" alt="saitama">
          </div>
        </div>
        <div class="forum-row_last-date">
          <span class="forum-row_last-date-topic">
            <a href="#" title="topic title">
              topic title here
            </a>
          </span>
          <span class="forum-row_last-date-name">
            by <a href="#" title="name">name</a> on january 9th, 2021
          </span>
        </div>
      </div>
      <img class="forum-row__img-1" src="https://img.nickpic.host/qLEoUx.png" title="saitama">
    </div>
    <div class="forum-row__moderation">
      <div class="forum-row_title">
        <span class="forum-row_title-stats">
          0 topics. 0 replies.
        </span>
        <span class="forum-row_title-name">
          <a href="#" title="moderation">
            moderation
          </a>
        </span>
      </div>
      <div class="forum-row__desc">
        <div class="forum-row_desc-box">
          <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, voluptates rem. Quibusdam fugiat officiis nihil voluptate, vero, perferendis porro iure deleniti fugit architecto, at tempora maiores et quam dolore distinctio?</P>
        </div>
      </div>
      <div class="forum-row_last">
        <div class="forum-row_last-avatar">
          <div class="forum-row_last-avatar-diamond">
            <img src="https://icon-library.com/images/saitama-icon/saitama-icon-6.jpg" alt="saitama">
          </div>
        </div>
        <div class="forum-row_last-date">
          <span class="forum-row_last-date-topic">
            <a href="#" title="topic title">
              topic title here
            </a>
          </span>
          <span class="forum-row_last-date-name">
            by <a href="#" title="name">name</a> on january 9th, 2021
          </span>
        </div>
      </div>
      <img class="forum-row__img-2" src="https://img.nickpic.host/qLEJF5.png" title="saitama">
    </div>
  </div>
</main>
