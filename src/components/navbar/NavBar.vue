<template>
  <!-- Navbar & Hero Start -->
  <!-- <div class="style sticky-top"> -->

  <div class="style">
    <nav
      class="navbar navbar-expand-lg navbar-light p-0"
      style="position: relative; top: 40px"
    >
      <div class="container">
        <router-link class="navbar-brand" :to="{ name: 'home' }">
          <img
            loading="lazy"
            src="@/assets/adsl/logo.png"
            width="50"
            height="50"
            alt="img"
          />
        </router-link>
        <span
          style="background-color: #ffbe03; color: white"
          class="navbar-toggler p-2"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <!-- <span class="p-2"><FontAwesome icon="caret-down" /></span> -->
          <span class="navbar-toggler-icon"></span>
        </span>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <div class="navbar-nav nav mx-auto mb-2 mb-lg-0 p-0">
            <router-link
              class="m-2 ms-lg-4 me-lg-4"
              :to="{ name: 'home' }"
              exact
              ><span class="fw-bold">الرئيسة</span></router-link
            >

            <router-link class="m-2 ms-lg-4 me-lg-4" :to="{ name: 'ourwork' }"
              ><span class="fw-bold">اعمالنا</span></router-link
            >

            <router-link class="m-2 ms-lg-4 me-lg-4" to="/products"
              ><span class="fw-bold">منتجاتنا</span></router-link
            >
            <router-link class="m-2 ms-lg-4 me-lg-4" to="/articles"
              ><span class="fw-bold">المدونة</span></router-link
            >

            <router-link class="m-2 ms-lg-4 me-lg-4" to="/about"
              ><span class="fw-bold">من نحن</span></router-link
            >
          </div>

          <router-link class="border-0" :to="{ name: 'ordernow' }" exact>
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
          </router-link>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "NavBarCom",
  mounted() {
    window.scrollTo(0, 0);
  },
};
</script>

<style scoped>
.style {
  direction: rtl;
}

.nav a {
  text-decoration: none;
  color: #353536 !important;
  font-weight: 900 !important;
  transition: all 0.2s ease-in-out;
}
.nav a:hover {
  color: #ffbe03 !important;
}
.nav .router-link-exact-active {
  color: #ffbe03 !important;
}
.navbar-toggler {
  padding: var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);
  font-size: var(--bs-navbar-toggler-font-size);
  line-height: 1;
  color: rgb(203 21 21 / 55%);
  background-color: transparent;
  border: var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);
  border-radius: var(--bs-navbar-toggler-border-radius);
  transition: var(--bs-navbar-toggler-transition);
}
</style>
