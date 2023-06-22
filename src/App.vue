<template>
  <div>
    <Header />
    <StepsGetCard />
    <Postpaid />
    <Prepaid />
    <Activity />
    <AksesPremium />
    <Banner />
    <QuestionAnswer />
    <Subscribe />
    <SocialMedia />
    <Footer />
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import StepsGetCard from "./components/organisms/StepsGetCard.vue";
import Postpaid from "./components/organisms/Postpaid.vue";
import Prepaid from "./components/organisms/Prepaid.vue";
import Activity from "./components/organisms/Activity.vue";
import AksesPremium from "./components/organisms/AksesPremium.vue";
import Banner from "./components/organisms/Banner.vue";
import QuestionAnswer from "./components/organisms/QuestionAnswer.vue";
import Subscribe from "./components/organisms/Subscribe.vue";
import SocialMedia from "./components/organisms/SocialMedia.vue";
import Footer from "./components/organisms/Footer.vue";
import Header from "./components/organisms/Header.vue";

export default {
  name: "App",
  components: {
    StepsGetCard,
    Postpaid,
    Prepaid,
    Activity,
    AksesPremium,
    Banner,
    QuestionAnswer,
    Subscribe,
    SocialMedia,
    Footer,
    Header,
  },
};
</script>

<style>
#app {
  background-color: #fff;
  overflow: hidden;
}
*:focus {
  outline: none;
}
body {
  font-size: 16px !important;
  line-height: 1.2;
  color: #000;
  background: #fff;
  font-weight: 400;
  font-family: "Roboto", sans-serif !important;
  min-width: 100% !important;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: "Roboto", sans-serif;
  font-weight: bold;
  margin: unset;
  line-height: 1.2;
}
h1,
.h1 {
  font-size: 3em;
}
h2,
.h2 {
  font-size: 2em;
}
h3,
.h3 {
  font-size: 1.875em;
}
h4,
.h4 {
  font-size: 1.3em;
}
h5,
.h5 {
  font-size: 1.1em;
}
h6,
.h6 {
  font-size: 1em;
}
p,
.p,
.psmall,
.pxsmall,
.pxxsmall {
  margin: 0;
}
p,
.p {
  font-size: 1em;
}
.psmall {
  font-size: 0.9em;
}
.pxsmall {
  font-size: 0.8em;
}
.pxxsmall {
  font-size: 0.7em;
}
.font-primary {
  color: #ed2324;
}
.font-dark {
  color: #212529;
}
.border-right {
  border-right: 1px solid #212529;
}

.btn-indosat {
  background-color: #ed2324;
  border-radius: 20px;
  width: fit-content;
  color: #fff;
  border: none;
  padding: 15px 25px;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 14px;
}

.card-indosat {
  padding: 20px 10px;
  border-radius: 16px;
  box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.1);
  border: none;
}
@media only screen and (max-width: 992px) {
  body {
    font-size: 15px !important;
  }
}
@media only screen and (max-width: 768px) {
  body {
    font-size: 14px !important;
  }
  .btn-indosat {
    width: 100%;
    text-align: center;
  }
}
@media only screen and (max-width: 576px) {
  body {
    font-size: 14px !important;
  }
  .border-right {
    border-right: none;
  }
}
</style>
