<template>
  <!-- <div v-if="loading">
    <div>
      <PageLoader />
    </div>
  </div> -->
  <div class="bg-header vh-100" style="direction: rtl">
    <!-- text and image -->
    <div class="container-fluid">
      <NavBarCom />
      <div class="row align-items-center vh-100 m-0 p-0">
        <div class="row d-flex justify-content-center">
          <div class="col-md-10">
            <div class="row align-items-center justify-content-between mb-2">
              <div
                class="col-lg-5 fw-bold align-middle text-center text-lg-end"
              >
                <h1 class="pb-3 lh-lg" style="color: #1f1e1e">
                  <strong>
                    سجل الأن واحصل علي
                    <span style="color: #3aa8f5">شريحتك</span>
                  </strong>
                </h1>
                <p class="pb-3" style="color: #1f1e1e">
                  هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة، لقد تم
                  توليد هذا النص من مولد النص العربى
                </p>
                <button
                  style="
                    background-color: #ffbe03;
                    width: 160px;
                    height: 50px;
                    border-radius: 12px;
                  "
                  class="btn fw-bold mb-4 text-dark"
                >
                  <!-- <FontAwesome icon="circle-arrow-left" class="ms-2" /> -->
                  تسجيل دخول
                </button>
              </div>
              <div class="col-lg-6 text-center mt-sm-4 text-lg-start">
                <!-- <img loading="lazy"
                  class="img-fluid rounded-3"
                  src="../../assets/adsl/img1.png"
                  alt="img"
                /> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="home" style="direction: rtl" id="home">
    <!-- section 2 -->
    <section class="py-5">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-md-10">
            <div class="row justify-content-center text-center">
              <div>
                <strong>
                  <h3 class="fw-900" style="color: #3aa8f5; font-size: 30px">
                    ما يميزنا
                  </h3>
                </strong>
                <!-- <h3 class="fw-bold fs-20">ما يميزنا</h3> -->
                <p class="fs-30 fw-bold">هذا النص هو مثال لنص يمكن أن يستبدل</p>
              </div>
            </div>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-md-10">
            <div class="row justify-content-around text-center">
              <div class="col-md-3" v-for="card in cards" :key="card.id">
                <div class="text-center position-relative">
                  <div
                    class="mx-auto rounded-4 d-flex align-items-center justify-content-center"
                    style="
                      width: 100px;
                      height: 100px;
                      border-radius: 16px;
                      background-color: #fde7d4;
                      color: #ffbe03;
                    "
                  >
                    <img loading="lazy" :src="card.image" alt="img" />
                  </div>
                  <p class="fs-18g my-3">
                    {{ card.title }}
                  </p>
                  <p class="fs-18g my-3">
                    {{ card.desc }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- section 3 الإشتراكات -->
    <section class="py-5">
      <div class="container-fluid">
        <div class="row justify-content-center">
          <div class="col-md-10">
            <div class="row justify-content-center text-center">
              <div>
                <strong>
                  <h3 class="fw-900" style="color: #ffbe03; font-size: 30px">
                    الإشتراكات
                  </h3>
                </strong>
                <p class="fs-30 fw-bold">هذا النص هو مثال لنص يمكن أن يستبدل</p>
              </div>
            </div>
          </div>
        </div>
        <div class="row justify-content-center mt-lg-4">
          <div class="col-md-10">
            <div class="row justify-content-around text-center">
              <div
                class="col-md-3 my-3"
                v-for="subscrip in subscriptions"
                :key="subscrip.id"
              >
                <div class="card border-0 text-center subscriptions">
                  <div
                    class="mx-auto d-flex align-items-center justify-content-center"
                  >
                    <img loading="lazy" :src="subscrip.image" alt="img" />
                  </div>
                  <p class="fs-18 my-3 fw-900" style="color: #1176c9">
                    {{ subscrip.title }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- text and image -->
    <div class="container-fluid py-5" style="position: relative">
      <div class="row d-flex justify-content-center">
        <div class="col-md-10">
          <div class="row align-items-center justify-content-between mb-2">
            <div class="col-lg-5 fw-bold align-middle text-center text-lg-end">
              <div class="circleshape"></div>
              <div class="circle"></div>

              <p class="pb-3" style="color: #1f1e1e">
                هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة
              </p>
              <p class="pb-3" style="color: #1f1e1e">
                هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة، لقد تم توليد
                هذا النص من مولد النص العربى، حيث يمكنك أن تولد مثل هذا النص
              </p>
            </div>
            <div class="col-lg-6 text-center mt-sm-4 text-lg-start">
              <img
                loading="lazy"
                class="img-fluid rounded-3"
                src="../../assets/adsl/card.png"
                alt="img"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- section 3 المضافة حديثاً -->
    <section class="py-5">
      <div class="container-fluid">
        <div class="row justify-content-center">
          <div class="col-md-10">
            <div class="row justify-content-center text-center my-4">
              <div>
                <strong>
                  <h3 class="fw-900" style="color: #3aa8f5; font-size: 30px">
                    المضافة حديثاً
                  </h3>
                </strong>
                <span
                  class="text-center float-lg-start fw-bold"
                  style="color: #3aa8f5"
                  >عرض الكل</span
                >
              </div>
            </div>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-md-11">
            <div class="row justify-content-lg-around text-center">
              <div
                class="col-md-3 my-3 my-lg-0 d-flex justify-content-center"
                v-for="news in News"
                :key="news.id"
              >
                <div class="card rounded-5 add-News">
                  <div
                    class="mx-auto rounded-4 mt-3 d-flex align-items-center justify-content-center"
                  >
                    <img loading="lazy" :src="news.image" alt="img" />
                  </div>
                  <div class="card-body">
                    <p class="fs-18 mb-0">
                      {{ news.title }}
                    </p>
                    <p class="fs-18">
                      {{ news.number }}
                    </p>
                    <p class="card-text d-inline ms-4">
                      المدة : {{ news.time }}
                    </p>
                    <button
                      style="
                        width: 125px;
                        height: 50px;
                        border-radius: 16px;
                        background-color: #ffbe0333;
                        color: #ff9d0a !important;
                      "
                      class="btn me-4"
                    >
                      أضف للعربة
                    </button>
                  </div>
                </div>
                <!-- <div class="text-center position-relative">
                  <div
                    class="mx-auto rounded-4 d-flex align-items-center justify-content-center"
                  >
                    <img loading="lazy" :src="news.image" alt="img" />
                  </div>
                  <p class="fs-18 mt-5">
                    {{ news.title }}
                  </p>
                </div> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- بانر -->
    <section class="pt-5">
      <div class="container-fluid bg-img">
        <div class="row d-flex justify-content-center">
          <div class="col-md-10">
            <div class="row align-items-center justify-content-between mb-2">
              <div
                class="col-lg-5 fw-bold align-middle text-center text-lg-end"
              >
                <h2
                  class="mb-4 font_h1 fw-bold btn-gradient-1"
                  style="font-weight: 900 !important"
                >
                  حمل التطبيق واحصل علي شريحتك
                </h2>
                <p class="pb-3" style="color: #1f1e1e">
                  هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة، لقد تم
                  توليد هذا النص من مولد
                </p>
                <div class="text-center text-lg-end">
                  <!-- Google Play button -->
                  <a class="market-btn google-btn" href="#" role="button">
                    <span class="market-button-subtitle fs-10">GET IT ON</span>
                    <span class="market-button-title">Google Play</span>
                  </a>
                  <!-- App Store button -->
                  <a
                    class="market-btn apple-btn"
                    href="#"
                    role="button"
                    style="width: 160.72px"
                  >
                    <span class="market-button-subtitle fs-10"
                      >Download on the</span
                    >
                    <span class="market-button-title">App Store</span>
                  </a>
                </div>
              </div>
              <div
                class="col-lg-5 fw-bold align-middle text-center text-lg-end"
              >
                <img
                  loading="lazy"
                  class="img-fluid"
                  src="@/assets/adsl/mobile.png"
                  alt="img"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- تواصل -->
    <section>
      <div
        class="container-fluid py-5"
        style="background-image: linear-gradient(to right, #1176c9, #3aa8f5)"
      >
        <div class="row d-flex justify-content-center">
          <div class="col-md-10">
            <div class="row align-items-center justify-content-between mb-2">
              <div class="text-center">
                <h3>كيف يمكننا مساعدتك ؟</h3>
                <button
                  class="btn my-3 whatsbtn text-dark"
                  style="
                    background-color: #e2e2e2;
                    border-radius: 12px;
                    font-size: 18px;
                  "
                >
                  <img
                    loading="lazy"
                    width="50"
                    height="50"
                    src="@/assets/adsl/whatsapp.png"
                    alt="whatsapp"
                  />
                  للطلب عبر الواتساب
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
  <FooterCom />
</template>

<script>
// import PageLoader from "@/components/pageloader/PageLoder.vue";
import NavBarCom from "@/components/navbar/NavBar.vue";
import FooterCom from "@/components/footer/FooterCom.vue";
export default {
  name: "HomeCom",
  components: {
    NavBarCom,
    FooterCom,
    // PageLoader,
  },
  data() {
    return {
      cards: [
        {
          id: 1,
          title: "موثوق و مضمون",
          desc: "هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة",
          image: require("@/assets/adsl/trusted.png"),
        },
        {
          id: 2,
          title: "سريع وموفر",
          desc: "هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة",
          image: require("@/assets/adsl/fast.png"),
        },
        {
          id: 3,
          title: "معك دائما",
          desc: "هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة",
          image: require("@/assets/adsl/withyou.png"),
        },
      ],
      subscriptions: [
        {
          id: 1,
          title: "شهرية",
          image: require("@/assets/adsl/Subscriptions.png"),
        },
        {
          id: 2,
          title: "3 شهور",
          image: require("@/assets/adsl/Subscriptions.png"),
        },
        {
          id: 3,
          title: "6 شهور",
          image: require("@/assets/adsl/Subscriptions.png"),
        },
        {
          id: 4,
          title: "سنة",
          image: require("@/assets/adsl/Subscriptions.png"),
        },
      ],
      News: [
        {
          id: 1,
          title: "رقم الشريحة",
          image: require("@/assets/adsl/almona.png"),
          number: "955664400225485",
          time: "شهر",
        },
        {
          id: 2,
          title: "رقم الشريحة",
          image: require("@/assets/adsl/almona.png"),
          number: "955664400225485",
          time: "شهر",
        },
        {
          id: 3,
          title: "رقم الشريحة",
          image: require("@/assets/adsl/almona.png"),
          number: "955664400225485",
          time: "شهر",
        },
        {
          id: 4,
          title: "رقم الشريحة",
          image: require("@/assets/adsl/almona.png"),
          number: "955664400225485",
          time: "شهر",
        },
      ],
    };
  },
};
</script>

<style scoped>
/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  .bg-header {
    background-image: url("@/assets/adsl/header.png");
    background-position: left; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: initial;
  }
  .circleshape {
    z-index: 1;
    position: absolute;
    left: 0px;
    right: 60px;
    top: 29%;
    transform: translate(-50%, -50%);
    border: 1px dashed #ffb4052e;
    width: 73px;
    height: 73px;
    border-radius: 50%;
    background: #ffb4052e;
  }
  .circle {
    z-index: 1;
    position: absolute;
    left: 0px;
    right: 40%;
    top: 75%;
    transform: translate(-50%, -50%);
    border: 1px dashed #ffb4052e;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background: #ffb505;
  }
  .bg-img {
    background-image: url("@/assets/adsl/bannar.png");
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: cover; /* Resize the background image to cover the entire container */
  }
  .whatsbtn {
    width: 30%;
  }
}

.home {
  direction: rtl;
  color: #1f1e1e !important;
}
a {
  color: #212a34 !important;
  font-weight: bold !important;
  text-decoration: none !important;
}

/* app store */
.market-btn {
  display: inline-block;
  padding: 0.3125rem 0.875rem;
  padding-left: 2.8125rem;
  -webkit-transition: border-color 0.25s ease-in-out,
    background-color 0.25s ease-in-out;
  -webkit-transition: border-color 0.25s ease-in-out,
    background-color 0.25s ease-in-out;
  -o-transition: border-color 0.25s ease-in-out,
    background-color 0.25s ease-in-out;
  transition: border-color 0.25s ease-in-out, background-color 0.25s ease-in-out;
  border: 1px solid #e7e7e7;
  background-position: center left 0.75rem;
  background-color: #ebebec;
  background-size: 1.5rem 1.5rem;
  background-repeat: no-repeat;
  text-decoration: none;
  margin: 2px 2px;
  -webkit-transition: all 0.5s ease-in-out;
  -o-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
  border-radius: 12px;
}
.market-btn .market-button-title {
  display: block;
  color: #222;
  font-size: 1.125rem;
}
/* .market-btn:hover .market-button-title {
  color: rgb(0, 0, 0);
} */
.market-btn .market-button-subtitle {
  display: block;
  margin-bottom: -0.25rem;
  color: #888;
  font-size: 0.75rem;
}
/* .market-btn:hover .market-button-subtitle {
  color: rgb(255, 255, 255);
} */
.apple-btn {
  background-image: url(data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pgo8IS0tIEdlbmVyYXRvcjogQWRvYmUgSWxsdXN0cmF0b3IgMTkuMC4wLCBTVkcgRXhwb3J0IFBsdWctSW4gLiBTVkcgVmVyc2lvbjogNi4wMCBCdWlsZCAwKSAgLS0+CjxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeD0iMHB4IiB5PSIwcHgiIHZpZXdCb3g9IjAgMCAzMDUgMzA1IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCAzMDUgMzA1OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIgd2lkdGg9IjI0cHgiIGhlaWdodD0iMjRweCI+CjxnIGlkPSJYTUxJRF8yMjhfIj4KCTxwYXRoIGlkPSJYTUxJRF8yMjlfIiBkPSJNNDAuNzM4LDExMi4xMTljLTI1Ljc4NSw0NC43NDUtOS4zOTMsMTEyLjY0OCwxOS4xMjEsMTUzLjgyQzc0LjA5MiwyODYuNTIzLDg4LjUwMiwzMDUsMTA4LjIzOSwzMDUgICBjMC4zNzIsMCwwLjc0NS0wLjAwNywxLjEyNy0wLjAyMmM5LjI3My0wLjM3LDE1Ljk3NC0zLjIyNSwyMi40NTMtNS45ODRjNy4yNzQtMy4xLDE0Ljc5Ny02LjMwNSwyNi41OTctNi4zMDUgICBjMTEuMjI2LDAsMTguMzksMy4xMDEsMjUuMzE4LDYuMDk5YzYuODI4LDIuOTU0LDEzLjg2MSw2LjAxLDI0LjI1Myw1LjgxNWMyMi4yMzItMC40MTQsMzUuODgyLTIwLjM1Miw0Ny45MjUtMzcuOTQxICAgYzEyLjU2Ny0xOC4zNjUsMTguODcxLTM2LjE5NiwyMC45OTgtNDMuMDFsMC4wODYtMC4yNzFjMC40MDUtMS4yMTEtMC4xNjctMi41MzMtMS4zMjgtMy4wNjZjLTAuMDMyLTAuMDE1LTAuMTUtMC4wNjQtMC4xODMtMC4wNzggICBjLTMuOTE1LTEuNjAxLTM4LjI1Ny0xNi44MzYtMzguNjE4LTU4LjM2Yy0wLjMzNS0zMy43MzYsMjUuNzYzLTUxLjYwMSwzMC45OTctNTQuODM5bDAuMjQ0LTAuMTUyICAgYzAuNTY3LTAuMzY1LDAuOTYyLTAuOTQ0LDEuMDk2LTEuNjA2YzAuMTM0LTAuNjYxLTAuMDA2LTEuMzQ5LTAuMzg2LTEuOTA1Yy0xOC4wMTQtMjYuMzYyLTQ1LjYyNC0zMC4zMzUtNTYuNzQtMzAuODEzICAgYy0xLjYxMy0wLjE2MS0zLjI3OC0wLjI0Mi00Ljk1LTAuMjQyYy0xMy4wNTYsMC0yNS41NjMsNC45MzEtMzUuNjExLDguODkzYy02LjkzNiwyLjczNS0xMi45MjcsNS4wOTctMTcuMDU5LDUuMDk3ICAgYy00LjY0MywwLTEwLjY2OC0yLjM5MS0xNy42NDUtNS4xNTljLTkuMzMtMy43MDMtMTkuOTA1LTcuODk5LTMxLjEtNy44OTljLTAuMjY3LDAtMC41MywwLjAwMy0wLjc4OSwwLjAwOCAgIEM3OC44OTQsNzMuNjQzLDU0LjI5OCw4OC41MzUsNDAuNzM4LDExMi4xMTl6IiBmaWxsPSIjMmUyZTJlIi8+Cgk8cGF0aCBpZD0iWE1MSURfMjMwXyIgZD0iTTIxMi4xMDEsMC4wMDJjLTE1Ljc2MywwLjY0Mi0zNC42NzIsMTAuMzQ1LTQ1Ljk3NCwyMy41ODNjLTkuNjA1LDExLjEyNy0xOC45ODgsMjkuNjc5LTE2LjUxNiw0OC4zNzkgICBjMC4xNTUsMS4xNywxLjEwNywyLjA3MywyLjI4NCwyLjE2NGMxLjA2NCwwLjA4MywyLjE1LDAuMTI1LDMuMjMyLDAuMTI2YzE1LjQxMywwLDMyLjA0LTguNTI3LDQzLjM5NS0yMi4yNTcgICBjMTEuOTUxLTE0LjQ5OCwxNy45OTQtMzMuMTA0LDE2LjE2Ni00OS43N0MyMTQuNTQ0LDAuOTIxLDIxMy4zOTUtMC4wNDksMjEyLjEwMSwwLjAwMnoiIGZpbGw9IiMyZTJlMmUiLz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8L3N2Zz4K);
}
.google-btn {
  background-image: url(data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pgo8IS0tIEdlbmVyYXRvcjogQWRvYmUgSWxsdXN0cmF0b3IgMTkuMC4wLCBTVkcgRXhwb3J0IFBsdWctSW4gLiBTVkcgVmVyc2lvbjogNi4wMCBCdWlsZCAwKSAgLS0+CjxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeD0iMHB4IiB5PSIwcHgiIHZpZXdCb3g9IjAgMCA1MTIgNTEyIiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA1MTIgNTEyOyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIgd2lkdGg9IjUxMnB4IiBoZWlnaHQ9IjUxMnB4Ij4KPHBvbHlnb24gc3R5bGU9ImZpbGw6IzVDREFERDsiIHBvaW50cz0iMjkuNTMsMCAyOS41MywyNTEuNTA5IDI5LjUzLDUxMiAyOTkuMDA0LDI1MS41MDkgIi8+Cjxwb2x5Z29uIHN0eWxlPSJmaWxsOiNCREVDQzQ7IiBwb2ludHM9IjM2OS4wNjcsMTgwLjU0NyAyNjIuMTc1LDExOS40NjcgMjkuNTMsMCAyOTkuMDA0LDI1MS41MDkgIi8+Cjxwb2x5Z29uIHN0eWxlPSJmaWxsOiNEQzY4QTE7IiBwb2ludHM9IjI5LjUzLDUxMiAyOS41Myw1MTIgMjYyLjE3NSwzODMuNTUxIDM2OS4wNjcsMzIyLjQ3IDI5OS4wMDQsMjUxLjUwOSAiLz4KPHBhdGggc3R5bGU9ImZpbGw6I0ZGQ0E5NjsiIGQ9Ik0zNjkuMDY3LDE4MC41NDdsLTcwLjA2Myw3MC45NjFsNzAuMDYzLDcwLjk2MWwxMDguNjg4LTYyLjg3N2M2LjI4OC0zLjU5Myw2LjI4OC0xMS42NzcsMC0xNS4yNyAgTDM2OS4wNjcsMTgwLjU0N3oiLz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPGc+CjwvZz4KPC9zdmc+Cg==);
}
.btn-gradient-1 {
  border-width: 4px;
  border-top: 0;
  border-left: 0;
  border-right: 0;
  border-style: solid;
  -o-border-image: -o-linear-gradient(left, darkblue, darkorchid) 1;
  border-image: -webkit-gradient(
      linear,
      left top,
      right top,
      from(#ffffff05),
      to(white)
    )
    1;
  border-image: linear-gradient(to right, #ffffff05, white) 1;
  padding-bottom: 10px; /* Add padding to create space below the text */
}
.subscriptions ::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  border-radius: 26px 0px 26px 26px !important;
  border: 1px solid transparent;
  background: linear-gradient(270deg, #1176c921, #1176c9cf) border-box;
  -webkit-mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
  -webkit-mask-composite: destination-out;
  mask-composite: exclude;
}
.add-News {
  transition: all 0.3s ease-in-out;
  border-radius: 26px;
}
.add-News:hover {
  width: 18rem;
  border: 1px #ffb505 solid;
  border-radius: 26px;
  box-shadow: 0px 0px 12px rgba(255, 190, 3, 0.2);
}
</style>
