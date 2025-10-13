<script setup>
//image
import logo1 from "@/assets/img/logo1.png";
import logo1_2 from "@/assets/img/logo1_2.png";
import logo2 from "@/assets/img/logo2.png";
//import structure from "@/assets/img/structure.jpg";
//import UTSA_LiuEncheng from "@/assets/img/UTSA_LiuEncheng.jpg";
//import UTSA_ChenYinhua from "@/assets/img/UTSA_ChenYinhua.jpg";
//import UTSA_LaiHuanjin from "@/assets/img/UTSA_LaiHuanjin.jpg";
// example components
import HorizontalTeamCard from "@/examples/cards/teamCards/HorizontalTeamCard.vue";
import DefaultInfoCard from "../../../../examples/cards/infoCards/DefaultInfoCard.vue";
//import CenteredBlogCard from "../../../../examples/cards/blogCards/CenteredBlogCard.vue";
//import RotatingCard from "../../../../examples/cards/rotatingCards/RotatingCard.vue";
//import RotatingCardFront from "../../../../examples/cards/rotatingCards/RotatingCardFront.vue";
//import RotatingCardBack from "../../../../examples/cards/rotatingCards/RotatingCardBack.vue";
</script>
<template>
  <section class="py-7">
    <div class="container">
      <div class="row align-items-center">
        <img src="@/assets/img/structure.jpg" />
      </div>
      <div class="row g-4 mt-6 mb-4">
        <h2 class="title-shift">學生會</h2>
        <div
          class="row mt-6 align-items-stretch justify-content-center text-center"
        >
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo1_2})` }"
            ></div>
            <p class="head-name">博愛校區副會長<br />陳胤華</p>
          </div>
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo1_2})` }"
            ></div>
            <p class="head-name">會長<br />劉恩誠</p>
          </div>
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo1_2})` }"
            ></div>
            <p class="head-name">天母校區副會長<br />賴桓津</p>
          </div>
        </div>
      </div>
      <div class="d-flex flex-column gap-4 mt-4 mb-4">
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '秘書部', link: 'javascript:;' }"
          description="負責文書、檔案、通知、紀錄等，例如法規修訂、會議記錄等等都由秘書部負責。如果你擅長統整資料，那秘書部會是一個非常適合你發揮的地方。"
        />
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '總務部', link: 'javascript:;' }"
          description="負責會費出納、會計、預算書與決算書編制、庶務、場地與器材管理。適合對數字敏感、擅長使用Excel，做事細心又謹慎的同學。"
          :reverse="true"
        />
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '公關部', link: 'javascript:;' }"
          description="負責學生會校內外聯絡、協調、宣傳等。也負責經營社群、撰寫文案與設計圖像。如果你文筆流暢，又樂於表達自己的想法，或對美感有一定敏銳度，想要看到自己的設計變成真正的實體周邊或海報。那公關部會非常適合你！"
        />
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '文化部', link: 'javascript:;' }"
          description="負責全校系活動籌畫，此部門的同學通常都很活潑，也很有創意和執行力。如果你想和他們一起舉辦能讓大家留下美好回憶的活動，文化部等你來加入！"
          :reverse="true"
        />
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '學權部', link: 'javascript:;' }"
          description="負責處理學生權益與義務事宜，他們關注社會議題，重視學生基本權益。適合有主見，願意分析議題進行論述，並為大眾站出來的同學加入。"
        />
        <HorizontalTeamCard
          class="mt-4"
          :image="logo1"
          :profile="{ name: '資訊部', link: 'javascript:;' }"
          description="負責個資控管、檔案管理以及網站與系統的開發維護。適合有基礎電腦使用能力，願意邊學邊做，且對資訊科技有熱忱的同學。"
          :reverse="true"
        />
      </div>
      <div class="row g-4 mt-6 mb-4">
        <h2 class="title-shift">學生議會</h2>
        <div
          class="row mt-6 align-items-stretch justify-content-center text-center"
        >
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo2})` }"
            ></div>
            <p class="head-name">博愛校區副議長<br />呂芷婕</p>
          </div>
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo2})` }"
            ></div>
            <p class="head-name">議長<br />簡廷宇</p>
          </div>
          <div class="col-auto head-card">
            <div
              class="head-frame"
              :style="{ backgroundImage: `url(${logo2})` }"
            ></div>
            <p class="head-name">天母校區副議長<br />李佳芸</p>
          </div>
        </div>
      </div>
      <div class="row g-4 mt-4 mb-4 d-flex justify-content-center">
        <h6 class="context-shift">
          臺北市立大學學生議會是本校最高的學生自治立法機關，<br />
          代表全體學生行使自治權，肩負監督、審議與推動政策的重要責任。<br />
          學生議會的設立，旨在保障同學權益、促進校園民主，<br />
          並作為學生與校方之間的溝通橋樑。
        </h6>
      </div>
      <div class="row g-4 mt-4 mb-4 justify-content-center">
        <div class="col-lg-10">
          <div class="row g-4 mt-4 mb-4">
            <DefaultInfoCard
              col="col-md-6"
              :title="{ text: '議會職權', class: 'text-dark' }"
              :description="{
                text: `
                  <ul class='list-unstyled m-0 p-0'>
                  <li> - <b>立法與審議</b>：討論並制定與學生相關之規章及自治事項。</li>
                  <li> - <b>預算與決算審查</b>：審核學生會及各自治組織之年度預算與決算。</li>
                  <li> - <b>監督與質詢</b>：監督學生會及其他自治組織之施政，並可提出質詢。</li>
                  <li class='no-wrap'> - <b>建議與聲明</b>：針對校園公共事務提出建議或代表全體學生發表立場聲明。</li>
                  </ul>
                `,
                class: 'text-muted',
              }"
            />
            <DefaultInfoCard
              col="col-md-6"
              :title="{ text: '議會組成', class: 'text-dark' }"
              :description="{
                text: '議會由當選議員與當然議員組成，確保不同學系之學生權益均衡展現。議員任期固定，並透過會議制度履行表決、審查及討論職責。 ',
                class: 'text-muted',
              }"
            />
            <DefaultInfoCard
              col="col-md-6"
              :title="{ text: '議會運作', class: 'text-dark' }"
              :description="{
                text: `
                <ul class='list-unstyled m-0 p-0'>
                  <span class='no-wrap'>
                    學生議會設有多個委員會及秘書處，以分工合作的方式確保議事效能：
                  </span>
                  <li> - <b>大會</b>：議會最高決策會議，由全體議員組成，處理重大決策與表決。</li>
                  <li> - <b>委員會</b>：依議題設置專責委員會，深入審查與研究各類提案。</li>
                  <li> - <b>秘書處</b>：作為議會行政支柱，負責議事支援、文書處理及人事培訓。</li>
                </ul>
              `,
                class: 'text-muted',
              }"
            />
            <DefaultInfoCard
              col="col-md-6"
              :title="{ text: '我們的使命', class: 'text-dark' }"
              :description="{
                text: '學生議會秉持民主、透明、專業之原則，持續為同學爭取權益，推動校園公共事務，並促進師生間的對話與合作。我們相信，每位學生的聲音都應被傾聽，而議會正是將這些聲音匯聚並付諸行動的地方。',
                class: 'text-muted',
              }"
            />
          </div>
          <div class="d-flex flex-column gap-4 mt-4 mb-4">
            <HorizontalTeamCard
              class="mt-4"
              :image="logo2"
              :profile="{ name: '秘書處', link: 'javascript:;' }"
              description="
                <ul class='list-unstyled m-0 p-0'>
                  學生議會的核心行政單位，肩負協助議會運作、確保議事順暢的任務。
                  <li> - <b>文書組</b>：文書處理、檔案歸檔、會議紀錄與議程草擬</li>
                  <li> - <b>議事組</b>：會議流程規劃、召集議員、維持秩序</li>
                  <li> - <b>公關組</b>：內外聯繫、資訊公告、社群宣傳</li>
                  <li> - <b>人事組</b>：招募培訓、考勤紀律、團隊凝聚</li>
                </ul>"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.head-card {
  text-align: center; /* 文字與圈圈置中 */
  margin: 0 50px; /* 卡片間距 */
}
.head-frame {
  width: 200px;
  height: 200px; /* 固定圈圈大小 */
  border-radius: 50%;
  background-size: cover;
  background-position: center;
  border: 3px solid #444;
  margin: 0 auto; /* 確保圈圈在中間 */
}
.head-name {
  margin-top: 8px;
  font-size: 24px;
  font-weight: 500;
}
.title-shift {
  margin-left: 10%; /* 可以改數值調整，20% 大概就是介於左邊跟中間 */
  /*text-shadow: 3px 3px 2px rgba(0, 0, 0, 0.3); /* X位移 Y位移 模糊程度 顏色 */
}
.context-shift {
  text-align: center;
  line-height: 2;
  margin: 0 auto;
  max-width: 450px;
}
.point-cards {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* 兩欄 */
  gap: 12px;
  margin-top: 10px;
}
.team-card ul {
  margin-top: 6px; /* 與前面文字的間距 */
  padding-left: 1.2rem; /* 左邊縮排 */
  line-height: 1.6; /* 每行高度（行距） */
}
.team-card li {
  margin-bottom: 4px; /* 每個項目之間的間距 */
}
.no-wrap {
  white-space: nowrap;
}
</style>
