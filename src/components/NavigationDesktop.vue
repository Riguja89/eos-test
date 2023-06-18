<template>
  <div class="nav-container">
    <div class="navigation-desktop">
      <div class="navigation-desktop__group">
        <div class="group__burger-icon">
          <img src="../assets/burger.svg" alt="burger-icon" />
        </div>
        <div class="group__test-icon">
          <img src="../assets/test-logo.svg" alt="test-logo" />
        </div>
      </div>

      <div class="navigation-desktop__group">
        <div class="group__search-container">
          <input type="text" placeholder="  Search here" />
          <img src="../assets/images/search-icon.svg" alt="" />
        </div>
        <div class="group__seting-icon">
          <img src="../assets/images/setting-icon.svg" alt="" />
        </div>
      </div>

      <div class="navigation-desktop__group">
        <div class="group__news-container">
          <img src="../assets/nav-notification.svg" alt="" />
        </div>
        <div class="right-group__dot-counter"></div>
        <div class="group__news-container">
          <img src="../assets/images/nav-msg.svg" alt="" />
        </div>
        <div class="right-group__dot-counter"></div>
        <div class="group__news-container">
          <img src="../assets/images/nav-gift.svg" alt="" />
        </div>
        <div class="right-group__dot-counter disable"></div>
      </div>

      <div class="navigation-desktop__group">
        <div class="group__profile-image">
        </div>
        <div class="group__profile-name">
          <span>David</span>
        </div>
        <div class="group__dropdown-icon">
          <img src="../assets/images/arrow-down.svg" alt="" />
        </div>
      </div>
    </div>
    <div class="dashboard-bar">
      <span>Dashboard /</span>
    </div>
  </div>
</template>

<style scoped>
.nav-container {
  height: 9.53vw;
}
.navigation-desktop {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  height: 6.25vw;
}
.group__burger-icon img {
  height: 2.39vw;
  width: 2.39vw;
}
.group__test-icon img {
  height: 2.64vw;
  width: 4.42vw;
}
.group__test-icon {
    padding-right: 2.5vw;
}

.group__search-container {
  width: 39.16vw;
  height: 2.92vw;
  border-radius: 12px;
  background: #1c2126;
  border: 1px solid #2f363d;
  display: flex;
  align-items: center;
  justify-content: center;
}
.group__search-container input {
  width: 90%;
  height: 50%;
  background: #1c2126;
  border: none;
  box-shadow: 0px 11px 23px rgba(0, 0, 0, 0.02);
  font-size: 0.84vw;
  color: white;
  margin-left: 20px;
  border-left: #13b497 2px solid;
  outline: none;
}
.group__search-container img {
  width: 1.25vw;
  height: 1.25vw;
  margin-right:1.5vw ;
}
.group__seting-icon img {
  height: 2.92vw;
  width: 2.92vw;
  margin: 0 0.78vw;
  display: flex;
  align-items: center;
}
.group__seting-icon {
    padding-right: 7.5vw;
}
.group__news-container {
    height: 2.92vw;
    width: 2.92vw;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #2F363D;
    border-radius: 12px;
}
.group__news-container img {
    height: 1.5vw;
    width: 1.5vw;
}
.navigation-desktop__group {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin: 0 1.72vw;
}
.right-group__dot-counter {
  height: 0.9vw;
  width: 0.9vw;
  border-radius: 50%;
  background-color: #d9b75f;
  position: relative;
  margin-right: 0.4vw;
  left: -0.52vw;
  top: -1.2vw;
}
.disable {
    background-color: gray;
}
.group__profile-image {
    height: 2.92vw;
    width: 2.92vw;
    margin-right: 1.5vw;
    background-color: #C4C4C4;
    border-radius: 12px;
}
.group__profile-name {
    font-size: 0.84vw;
    margin-right: 1.5vw;
}
.group__dropdown-icon {
    height: 0.325vw;
    width:  0.625vw;
    display: flex;
    align-items: center;
    margin-right: 2vw;
}
.dashboard-bar {
  height: 3.28vw;
  background-color: #2d3339;
  text-align: start;
  color: #13b497;
  padding-left: 4.7vw;
  display: flex;
  align-items: center;
  font-size: 0.84vw;
}
</style>
