<template>
  <div class="l-breadCrumb">
    <div class="container">
      <div class="row">
        <ul class="l-breadCrumb-list">
          <li class="l-breadCrumb-item">
            <a href="/zh-tw/" title="前往首頁">首頁</a>
          </li>
          <li class="l-breadCrumb-item">
            <a href="/zh-tw/personal" title="前往個人金融">個人金融</a>
          </li>
          <li class="l-breadCrumb-item">
            <a href="/zh-tw/personal/loan" title="前往貸款">貸款</a>
          </li>
          <li class="l-breadCrumb-item">
            <a href="/zh-tw/personal/loan/personal" title="前往信貸">信貸</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.l-breadCrumb {
  position: position;
  z-index: 5;
  font-size: 0.875rem;
  margin: 20px 12px;
  display: block;
  top: 110px;
}
.l-breadCrumb-list {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  margin: 0;
  padding: 0;
  list-style: none;
}
.l-breadCrumb-item a {
  color: inherit;
  text-decoration: none;
}
.l-breadCrumb-item + .l-breadCrumb-item {
  position: relative;
  padding-left: 16px;
  margin: 0;
}
.l-breadCrumb-item + .l-breadCrumb-item::before {
  content: "";
  position: absolute;
  left: 0;
  top: 50%;
  width: 8px;
  height: 14px;
  transform: translateY(-50%);
  background-repeat: no-repeat;
  background-size: 8px 14px;
  -webkit-mask: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8.6 14.4'%3E%3Cpath d='M1,1l6.1,6.1L1,13.3' fill='none' stroke='rgb(74, 74, 74)' stroke-linecap='round' stroke-linejoin='round' stroke-width='2'/%3E%3C/svg%3E")
    no-repeat center/8px 14px;
  mask: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8.6 14.4'%3E%3Cpath d='M1,1l6.1,6.1L1,13.3' fill='none' stroke='rgb(74, 74, 74)' stroke-linecap='round' stroke-linejoin='round' stroke-width='2'/%3E%3C/svg%3E")
    no-repeat center/8px 14px;
  background-color: currentColor;
}
.l-breadCrumb .l-breadCrumb-item a {
  -webkit-transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}
.l-breadCrumb .l-breadCrumb-item a:hover {
  color: #00a19b;
}
@media (min-width: 992px) {
  .l-breadCrumb {
    display: block;
  }
}
</style>
