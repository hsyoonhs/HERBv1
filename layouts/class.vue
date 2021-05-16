<template>
  <div>
    <header class="class-header">
      <div class="container is-max-desktop">
        <img src="~assets/images/logo.png" />
        <hr style="width: 9rem; margin: 1.5rem auto;">
        <h1 class="title has-text-weight-bold is-size-1">2학년 예반</h1>
        <h2 class="subtitle has-text-weight-bold">청원고교</h2>
      </div>
    </header>
    <nav class="navigation">
      <ul>
        <li>
          <a href="https://school.cbe.go.kr/cw-h"> 청원고등학교 </a>
        </li>
        <li>
          <a href="https://hcs.eduro.go.kr/"> 자가진단 </a>
        </li>
        <li>
          <a href="https://ebsoc.co.kr/"> EBS 온라인클래스 </a>
        </li>
        <li>
          <a href="https://www.instagram.com/2021_cwhs_/"> 학생회 인스타 </a>
        </li>
        <li>
          <a href="https://www.youtube.com/channel/UC79aL3O7o-mCNQtbl_C4M0g">
            학생회 유튜브
          </a>
        </li>
      </ul>
    </nav>

    <section class="main-content container is-max-desktop">
      <div class="container column is-10">
        <section class="section">
          <nuxt />
          <div class="columns is-multiline">
            <div class="column is-full">
              <div class="card" id="realtime">
                <div class="card-content"></div>
              </div>
            </div>
            <div class="column">
              <div class="card" id="timetable">
                <header class="card-header">
                  <p class="card-header-title">시간표</p>
                </header>
                <div class="card-content"></div>
              </div>
            </div>
            <div class="column">
              <div class="card" id="meals">
                <header class="card-header">
                  <p class="card-header-title">급식 식단</p>
                </header>
                <div class="card-content"></div>
              </div>
            </div>
          </div>
        </section>
      </div>
    </section>

    <footer class="footer">
      <div class="content container is-max-desktop">
        <h3>HERB<sup>v1</sup></h3>
        <li><NuxtLink to="/information">정보</NuxtLink></li>
        <li>개발 및 디자인 ⓒ 2021 Hs Yoon</li>
        <li>
          저작권이 명시되지 않은 모든 자료는 청원고등학교에 귀속되어 있습니다.
        </li>
      </div>
    </footer>
  </div>
</template>
<style scoped>
.class-header {
  background: #ee9ca7;
  background: -webkit-linear-gradient(to top, #ffdde1, #ee9ca7);
  background: linear-gradient(to bottom, #ffdde1, #ee9ca7);
}

.class-header .container {
  padding: 4rem 0;
  text-align: center;
}

.class-header .container img {
  width: 5rem;
  height: 5rem;
  top: 50%;
  left: 50%;
  filter: invert(1) grayscale(1) brightness(1.9);
}

.class-header .container h1,
.class-header .container h2 {
  color: rgba(255, 255, 255, .6);
}

.navigation {
  padding: 0.5rem;
  background-color: #fff;
  border-bottom: 1px solid gainsboro;
  text-align: center;
  white-space: nowrap;
  overflow: auto;
  user-select: none;
  z-index: 1;
}

.navigation li {
  display: inline-block;
}

.navigation a {
  padding: 1rem;
  display: inline-block;
  border-radius: 4px;
  color: darkgray;
  transition: 0.2s;
}

.navigation a:hover {
  background-color: rgba(0, 0, 0, 0.04);
  color: #000;
  filter: none;
}

@media screen and (min-width: 769px) {
  .navigation {
    margin: 0;
    position: sticky;
    top: 0;
  }
}

.navigation::-webkit-scrollbar {
  display: none;
}

.navigation {
  -ms-overflow-style: none;
}
</style>

<script scoped>
let classCodeInRaw = "/11";
if (typeof window !== "undefined") {
   classCodeInRaw = window.location.pathname;
}
const classCode = classCodeInRaw.replace(/[/]/g, '');
const classCodeSplitted = classCode.split("");
const classGrade = classCodeSplitted[0];
const classNameInNum = classCodeSplitted[1];

if (classNameInNum == 1)
   className = '인'
else if (classNameInNum == 2)
   className = '의'
else if (classNameInNum == 3)
   className = '예'
else if (classNameInNum == 4)
   className = '지'
else if (classNameInNum == 5)
   className = '매'
else if (classNameInNum == 6)
   className = '난'
else if (classNameInNum == 7)
   className = '국'
else
   className = '죽'
   
if (typeof document !== "undefined") {
   document.querySelector('.class-header .title').innerHTML = `${classGrade}학년 ${className}반`;
}

window.onload = realtimeDate();
function realtimeDate(){
  const now = new Date();
  const nowDate = now.toLocaleDateString();
  const week = new Array('(일)', '(월)', '(화)', '(수)', '(목)', '(금)', '(토)');
  const nowWeek = week[now.getDay()];
  const nowTime = now.toLocaleTimeString();
  if (typeof document !== "undefined") {
     document.querySelector('#realtime .card-content').innerHTML = `${nowDate} ${nowWeek} ${nowTime}`;
  }
  setTimeout(realtimeDate, 1000);
}

let date = new Date();
let year = date.getFullYear();
let month = new String(date.getMonth() + 1);
let day = new String(date.getDate());

if(month.length == 1) {
  month = "0" + month;
}
if(day.length == 1) {
  day = "0" + day;
}

const todayDate = year + month + day;

if (typeof document !== "undefined") {
   const section = document.querySelector('#meals .card-content');
}

const requestURL = 'https://open.neis.go.kr/hub/mealServiceDietInfo?Type=json&ATPT_OFCDC_SC_CODE=M10&SD_SCHUL_CODE=8000214&MLSV_YMD=' + todayDate;

const request = new XMLHttpRequest();
request.open('GET', requestURL);
request.responseType = 'json';
request.send();
request.onload = function() {
    const mealDiet = request.response;
    showDiet(mealDiet);
}

function showDiet(jsonObj) {
  const diet = jsonObj['mealServiceDietInfo'][1]['row'];

  for (var i = 0; i < diet.length; i++) {
    if (typeof document !== "undefined") {
       const myArticle = document.createElement('article');
       const myH3 = document.createElement('h3');
       const myList = document.createElement('ul');
       const myPara = document.createElement('p');
    }
  
    const DDISH_NM_TEMP = diet[i].DDISH_NM.replace(/(<([^>]+)>)/ig,", ");
    const DDISH_NM = DDISH_NM_TEMP.replace(/([\d.])/ig,"");
    const words = DDISH_NM.split(',');

    myH3.textContent = diet[i].MMEAL_SC_NM;

    const mealList = words;
    for (let j = 0; j < mealList.length; j++) {
      if (typeof document !== "undefined") {
        const listItem = document.createElement('li');
      }
      listItem.textContent = mealList[j];
      myList.appendChild(listItem);
    }

    myPara.textContent = `칼로리: ${diet[i].CAL_INFO}`;

    myArticle.appendChild(myH3);
    myArticle.appendChild(myList);
    myArticle.appendChild(myPara);
    section.appendChild(myArticle);
  }
}
</script>
