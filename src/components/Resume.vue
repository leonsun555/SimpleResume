<template>
<div class="resume">
  <div class="left">
    <h1>孫以晨</h1>
    <h4>前端工程師</h4>
    <hr>
    <p>畢業於台灣科技大學,現任於台北藝術大學招生組,對於前端新技術擁有永無止境的熱情!</p>
    <div class="buttons">
      <a class="btn fill" href="https://github.com/leonsun555" target="_blank">Github</a>
    </div>
    <div class="block">
      <h4>Skills</h4>
      <h2>專業技能</h2>
      <ul class="listSkill">
        <li>
          <div class="circle">
            <div class="p90"></div>
            <div class="p180"></div>
            <div class="p270"></div>
            <div class="p360"></div>
          </div>
          前端技術(html/css/js)
        </li>
        <li>
          
          <div class="circle">
            <div class="p90"></div>
            <div class="p180"></div>
            <div class="p270"></div>
          </div>
          後端技術(API)
        </li>
        <li>
          
          <div class="circle">
            <div class="p90"></div>
            <div class="p180"></div>
            <div class="p270"></div>
          </div>
          資料分析與處理(Database)
        </li>
        <li>
          
          <div class="circle">
            <div class="p90"></div>
            <div class="p180"></div>
          </div>
          網路技術與理論(Routing)
        </li>
        <li>
          
          <div class="circle">
            <div class="p90"></div>
            <div class="p180"></div>
            <div class="p270"></div>
          </div>
          開發框架應用(Vue.js,ASP.NET)
        </li>
      </ul>
    </div>
    <div class="block">
      <h4>Programming Language</h4>
      <h2>程式語言</h2>
      <ul class="listProgram">
         <li>Html/Css
          <div class="bar">
            <div class="value p70"></div>
          </div>
        </li>
        <li>JavaScript
          <div class="bar">
            <div class="value p70"></div>
          </div>
        </li>
        <li>C#
          <div class="bar">
            <div class="value p50"></div>
          </div>
        </li>
        <li>SQL
          <div class="bar">
            <div class="value p50"></div>
          </div>
        </li>
        <li>VB.Net
          <div class="bar">
            <div class="value p30"></div>
          </div>
        </li>
        <li>Python
          <div class="bar">
            <div class="value p30"></div>
          </div>
        </li>
      </ul>
    </div>
  </div>
  <div class="right">
    <div class="decoration"></div>
    <div class="block-right">
      <h4>Experience</h4>
      <h2>職涯經歷</h2>
      <ul class="listExperience">
        <li class="year">2015
          <ul>
            <li>Cyber Power 碩天科技 軟體測試工程師</li>
          </ul>
        </li>
        <li class="year">2017
          <ul>
             <li>Asia Credit Management 亞洲信用管理 MIS工程師</li>
          </ul>
        </li>
        <li class="year">2019
          <ul>
            
            <li>國立台北藝術大學 招生專案計畫工程師</li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="block-right">
      <h4>Works</h4>
      <h2>相關作品</h2>
       <ul>
        <li>亞洲信用管理公司內部行政系統</li>
        <li>北藝大招生行政系統</li>
        <li>北藝大招生資料分析平台</li>
        <li>北藝大招生宣傳品訂購網站</li>
        <li>專題作品-路跑社群平台App</li>
      </ul>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* 複寫區 */
ul{
  padding: 0;
  list-style: none;
}
h2{
  margin: 0;
  margin-bottom: 25px;
  font-weight: 400;
}
h2::after{
  content: "";
  display: inline-block;
  width: 20px;
  height: 8px;
  background-color: #FF7168;
  margin-left: 10px;
}
h4{
  margin: 0;
  margin-top: 40px;
  opacity: 0.8;
  font-weight: 400;
}
a{
  color: white;
  text-decoration: none
}
hr{
  border: none;
  border-bottom: solid 4px #FF7168;
  width: 40%;
  margin-left: 0;
}
.block-right {
  margin-bottom: 10rem
}

.resume{
  display: flex;
  max-width: 950px;
  border: solid 6px MediumSlateBlue;
  padding: 50px;
  position: relative;
}
.left{
  flex: 5
}
.right{
  flex: 7
}
.left,.right{
  padding: 15px
}
.left{
  padding-right: 50px;
  border-right: solid 1px #FF7168;
}

.right{
  padding-left: 50px;
  padding-top: 150px;
}


.decoration{
  width: 300px;
  height: 140px;
  background: linear-gradient(135deg,#FF5F5F,#FFFFAE);
  border-radius: 70px 0px 0px 70px;
  position: absolute;
  right: 0;
  top: 50px;
}

.listExperience>li{
  display: flex;
  margin-bottom: 10px;
  
}

.listExperience>li:nth-child(1) ul{
  border-color: #FF7168
}
.listExperience>li:nth-child(2) ul{
  border-color: #FFA582
}
.listExperience>li:nth-child(3) ul{
  border-color: #FFB087
}
.listExperience>li:nth-child(4) ul{
  border-color: #FFDE9E
}
.listExperience li ul{
  padding-left: 10px;
  margin-left: 10px;
  margin-bottom: 15px;
  border-left: solid 4px white
}


/* list skill */
.listSkill{
  display: flex;
  flex-wrap: wrap;
  
}
.listSkill li{
  width: 25%;
  padding: 5px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.circle{
  width: 50px;
  height: 50px;
  background-color: #fff;
  border-radius: 50%;
  position: relative;
  overflow: hidden;
  background-color: rgba(255, 113, 104,0.4);
}
.circle::after{
  content: "";
  display: block;
  background-color: #fff;
  width: calc(100% - 20px);
  height: calc(100% - 20px);
  border-radius: 50%;
  position: relative;
  left: 50%;
  top: 50%;
  transform: translate(-50%,-50%)
}
.p90,.p180,.p270,.p360{
  width: 50%;
  height: 50%;
  position: absolute;
  left: 50%;
  top: 0;
  background-color: #FF7168;
}
.p180{
  top: 50%;
}
.p270{
  left: 0;
  top: 50%;
}
.p360{
  left: 0;
  top: 0;
}


/* list program */

.listProgram .bar{
  width: 150px;
  height: 10px;
  border: solid 2px #FF7168;
  border-radius: 5px
}
.listProgram li{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 10px;
}
.value{
  height: 100%;
  width: 60%;
  background-color: #FF7168;
}
.value.p10{
  width: 10%;
}
  
.value.p20{
  width: 20%;
}
.value.p30{
  width: 30%;
}
.value.p40{
  width: 40%;
}
.value.p50{
  width: 50%;
}
.value.p60{
  width: 60%;
}
.value.p70{
  width: 70%;
}
.value.p80{
  width: 80%;
}
.value.p90{
  width: 90%;
}

.value.p100{
  width: 100%;
}

.btn{
  border: solid 3px #FF7168;
  padding: 5px 20px;
  margin-right: 10px;
}
.fill{
  background-color: #FF7168;
}
</style>

