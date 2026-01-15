<template>
  <nav class="l-subnav p-0">
    <div class="l-subnavContent p-0">
      <ul class="l-subnavMenu p-0">
        <div class="l-subnavList px-3">
          <li class="l-subnavItem">
            <a
              class="l-subnavItem-link active"
              href="#1"
              title="前往H2_輪播卡片"
              >H2_輪播卡片</a
            >
          </li>
          <li class="l-subnavItem">
            <a class="l-subnavItem-link" href="#2" title="前往H2_不輪播卡片"
              >H2_不輪播卡片</a
            >
          </li>
          <li class="l-subnavItem">
            <a class="l-subnavItem-link" href="#3" title="前往H2_文字卡片"
              >H2_文字卡片</a
            >
          </li>
          <li class="l-subnavItem">
            <a class="l-subnavItem-link" href="#3" title="前往H2_文字卡片"
              >H2_文字卡片</a
            >
          </li>
          <li class="l-subnavItem">
            <a class="l-subnavItem-link" href="#3" title="前往H2_文字卡片"
              >H2_文字卡片</a
            >
          </li>
          <li class="l-subnavItem">
            <a class="l-subnavItem-link" href="#3" title="前往H2_文字卡片"
              >H2_文字卡片</a
            >
          </li>
          <div class="activeLine"></div>
        </div>
        <div class="l-subnavMenu-button">
          <div class="btnWrapper">
            <a
              href="https://card.esunbank.com.tw/EsunCreditweb/txnservice/identify?PRJCD=CLAP01"
              rel="noopener noreferrer"
              class="btnLine color-primary mx-2 my-0"
              target="_blank"
              title="前往字數上限：7中字另開新視窗"
              >字數上限7字</a
            >
            <a
              class="btn bg-primary mx-2 my-0"
              href="https://card.esunbank.com.tw/EsunCreditweb/txnservice/identify?PRJCD=CLAP01"
              title="前往2中字"
              >2中字</a
            >
          </div>
        </div>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.l-subnav {
  position: sticky;
  top: 0px;
  width: 100%;
  background-color: white;
  -webkit-box-shadow: inset lightgrey 0 0px 0, rgba(0, 0, 0, 0.1) 0 1px 1px 0;
  box-shadow: inset lightgrey 0 0px 0, rgba(0, 0, 0, 0.1) 0 1px 1px 0;
  z-index: 100;
}
.l-subnav::before {
  content: "";
  width: 20px;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  z-index: 1;
  -webkit-transform: rotate(180deg);
  transform: rotate(180deg);
  background: -webkit-gradient(
    linear,
    left top,
    right top,
    from(rgba(255, 255, 255, 0)),
    color-stop(52%, rgb(255, 255, 255)),
    to(rgb(255, 255, 255))
  );
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0) 0%,
    rgb(255, 255, 255) 52%,
    rgb(255, 255, 255) 100%
  );
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#00ffffff", endColorstr="#ffffff", GradientType=1);
  background-size: 100% auto;
}

.l-subnavContent {
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
}

.l-subnavMenu {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
  display: -webkit-box !important;
  display: -ms-flexbox !important;
  display: flex !important;
  -webkit-box-align: center !important;
  -ms-flex-align: center !important;
  align-items: center !important;
  -webkit-box-pack: justify !important;
  -ms-flex-pack: justify !important;
  justify-content: space-between !important;
}

.l-subnavMenu::before {
  content: "";
  width: 20px;
  height: 100%;
  position: absolute;
  right: 0;
  top: 0;
  z-index: 100;
  background: -webkit-gradient(
    linear,
    left top,
    right top,
    from(rgba(255, 255, 255, 0)),
    color-stop(80%, white),
    to(white)
  );
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0) 0%,
    white 80%,
    white 100%
  );
  background-size: 100% auto;
}

.l-subnavList {
  width: 100%;
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: nowrap;
  flex-wrap: nowrap;
  overflow: scroll;
  -ms-scroll-chaining: none;
  overscroll-behavior: none;
  scrollbar-width: none;
  -ms-overflow-style: none;
  -webkit-transform: translateZ(0);
  transform: translateZ(0);
  -webkit-transition: -webkit-transform var(--ease) var(--duration);
  transition: -webkit-transform var(--ease) var(--duration);
  transition: transform var(--ease) var(--duration);
  transition: transform var(--ease) var(--duration),
    -webkit-transform var(--ease) var(--duration);
}
.l-subnavItem {
  margin-top: 0;
}
.l-subnavItem-link {
  display: block;
  padding: 16px;
  text-decoration: none;
  white-space: nowrap;
  color: var(--color-link);
  -webkit-transition: color var(--ease) var(--duration);
  transition: color var(--ease) var(--duration);
}

.l-subnavItem-link.active {
  color: var(--color-active);
  border-bottom: 4px solid #00a19b;
  color: #00a19b;
}

.activeLine {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 4px;
  background-color: var(--color-active);
  -webkit-transition: width var(--ease) var(--duration),
    -webkit-transform var(--ease) var(--duration);
  transition: width var(--ease) var(--duration),
    -webkit-transform var(--ease) var(--duration);
  transition: width var(--ease) var(--duration),
    transform var(--ease) var(--duration);
  transition: width var(--ease) var(--duration),
    transform var(--ease) var(--duration),
    -webkit-transform var(--ease) var(--duration);
}
.l-subnavMenu-button {
  width: 100%;
    -webkit-box-flex: 0;
    -ms-flex: 0 0 16.6666666667%;
    flex: 0 0 16.6666666667%;
    max-width: 16.6666666667%;
}
.l-subnavMenu-button .btnWrapper {
  display: -webkit-box !important;
  display: -ms-flexbox !important;
  display: flex !important;
  -ms-flex-wrap: wrap;
  /*flex-wrap: wrap;*/
  /* margin-right: -15px;*/
  /*margin-left: -15px;*/
  position: relative;
  z-index: 101;
  -webkit-box-pack: end !important;
  -ms-flex-pack: end !important;
  justify-content: flex-end !important;
}
.l-subnavMenu-button .btnWrapper::before {
  content: "";
  position: absolute;
  width: 20px;
  left: -15px;
  height: 100%;
  right: 0;
  top: 0;
  z-index: 100;
  background: -webkit-gradient(
    linear,
    left top,
    right top,
    from(rgba(255, 255, 255, 0)),
    color-stop(80%, white),
    to(white)
  );
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0) 0%,
    white 80%,
    white 100%
  );
  background-size: 100% auto;
}

.btnWrapper .btnLine {
  width: 100%;
  height: 50px;
  position: relative;
  display: none;
  z-index: 101;
}

.btnWrapper .btn {
    outline: none;
    width: 150px;
    height: auto;
    padding: 4px 0;
    position: relative;
    z-index: 101;
}
@media (min-width: 1400px) {
  .l-subnav {
    top: 0;
  }
  .l-subnavContent {
    max-width: 1360px;
  }
}
@media (min-width: 1200px) {
  .l-subnavContent {
    max-width: 1140px;
  }
  .l-subnavMenu-button {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 33.3333333333%;
    flex: 0 0 33.3333333333%;
    max-width: 33.3333333333%;
  }
  .btnWrapper .btnLine{
  display: block;
  }
}
@media (min-width: 992px) {
  .l-subnavList {
    margin: initial;
  }
}

@media (min-width: 768px) {
  .l-subnavMenu-button {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 16.6666666667%;
    flex: 0 0 16.6666666667%;
    max-width: 16.6666666667%;
  }
}

@media (min-width: 576px) {
  .l-subnavList {
    margin: 0 auto;
  }
  .btnWrapper .btn {
    height: 44px;
    padding: 10px 0;
  }
}

.p-0 {
  padding: 0 !important;
}
ol,
ul {
  list-style: none;
}
</style>
