
<html>
  <head>

    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  
  <body>

<div>
  <h1>자주 들어가는 사이트 목록</h1>
<ul>
  <h>  
  가장 많이 사용하는 사이트
  <h>
    <li><a href="https://www.naver.com">NAVER </a></li><br>
    <li><a href="https://www.facebook.com">FACEBOOK</a></li><br>
    <li><a href="https://www.google.com">GOOGLE DRIVE</a></li><br>
    <li><a href="https://www.youtube.com">YOUTUBE</a></li><br>
    <li><a href="https://www.daum.com">Daum</a></li><br><br>
 
  <h>  
  인강 사이트
  <h>
     <li><a href="http://www.mimacstudy.com/main/main.ds">대성 마이맥</a></li><br>
     <li><a href="http://www.megastudy.net/">메가스터디</a></li><br>
     <li><a href="https://skyedu.conects.com/go3/main">스카이에듀</a></li><br>
     <li><a href="https://www.etoos.com/home/default.asp">이투스</a></li><br>


<style>#calendar { width: 380px; height: 300px; text-align: center; border: 1px solid black;}.week { display: flex;}.weekname { width: 50px; }.days { display: flex; flex-wrap: wrap; }.daynum { width: 50px; line-height: 30px; height: 30px; cursor: pointer;}.daynum .empty { pointer-events: none;}.today { background-color:hotpink; border : 2px solid darkviolet;}.daynum:hover { background: greenyellow; color: palevioletred; border : 2px solid darkviolet; font-size: 20px;}.prev-btn{ position: absolute; top : 20; left:30px;}.next-btn{ position: absolute; top : 20; left:30px;}//id는 # 클래스는 .으로 시작#goto{ position : absolute; left : 300px; top : 100px; margin-left:146px;} </style>
<link href="style.css" rel="stylesheet" ><div id="calendar"> <h2></h2> <div class="week"></div> <div class="days"></div> <button id = "goto" onClick = "today_init()" style="display:none">이번달로 가기</button> </div><button class="prev-btn"onClick="handlePrevCalendar()">이전></button><button class="next-btn"onClick="handleNextCalendar()">다음></button><script src="script.js"></script><script>const calendar = document.getElementById("calendar");const week = document.querySelector(".week");const days = document.querySelector(".days");let today = new Date();let count = 0;const firstDay = (count) => new Date(today.getFullYear(), today.getMonth() + count, 1);const lastDay = (count) => new Date(today.getFullYear(), today.getMonth() + count + 1, 0);const weekName = ["일", "월", "화", "수", "목", "금", "토"];week.innerHTML = weekName .map((week) => <div class="weekname"> ${week} </div>) .join("");1;function calendarBuilding(firstDate, lastDate) { const calendarHeader = calendar.querySelector("h2"); calendarHeader.innerHTML = `${lastDate.getFullYear()}년 ${ lastDate.getMonth() + 1 } 월`; let weekday_no = 0; days.innerHTML = ""; for (let i = 0; i < firstDate; i++) { days.innerHTML += <div class="daynum empty"></div>; weekday_no++; } for (let i = 1; i < lastDate.getDate() + 1; i++) { if ((weekday_no%7) == 0) { if (i == today.getDate() && count==0){ days.innerHTML += <div class="daynum today sunday"> ${i} </div>; } else{ days.innerHTML += <div class="daynum sunday"> ${i} </div>; } } else { if (i == today.getDate() && count==0){ days.innerHTML += <div class="daynum today"> ${i} </div>; } else{ days.innerHTML += <div class="daynum"> ${i} </div>; } } weekday_no++; } days.innerHTML += <span class = "WM"> made by Seohyeon </span> if (count != 0){ document.getElementById("goto").style.display="block"; } else{ document.getElementById("goto").style.display="none"; }}function handleNextCalendar() { count += 1; const firstDate = firstDay(count).getDay(); const lastDate = lastDay(count); calendarBuilding(firstDate, lastDate);}function handlePrevCalendar() { count -= 1; const firstDate = firstDay(count).getDay(); const lastDate = lastDay(count); calendarBuilding(firstDate, lastDate);}function init() { const firstDate = firstDay(0).getDay(); const lastDate = lastDay(0); calendarBuilding(firstDate, lastDate);}function today_init(){ count = 0; init()}init();</script><style>#calendar { width: 380px; height: 300px; text-align: center; border: 1px solid black;}.week { display: flex;}.weekname { width: 50px; }.days { display: flex; flex-wrap: wrap; }.daynum { width: 50px; line-height: 30px; height: 30px; cursor: pointer;}.daynum .empty { pointer-events: none;}.today { background-color:hotpink; border : 2px solid darkviolet;}.daynum:hover { background: greenyellow; color: palevioletred; border : 2px solid darkviolet; font-size: 20px;}.prev-btn{ position: absolute; top : 20; left:30px;}.next-btn{ position: absolute; top : 20; left:30px;}//id는 # 클래스는 .으로 시작#goto{ position : absolute; left : 300px; top : 100px; margin-left:146px;} </style>

<!-- #3CB371 - 연초 
    8B00FF - 보라
-->
