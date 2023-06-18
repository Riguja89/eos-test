<template>
  <div id="navigation-mobile">
    <div class= "navigation-mobile__left-group">
      <div class="left-group__burger-icon">
        <img src="../assets/burger.svg" alt="burger-icon" />
      </div>
      <div class="left-group__logo">
        <img src="../assets/test-logo.svg" alt="test-logo" />
      </div>
    </div>

    <div class= "navigation-mobile__right-group">
      <div class= "right-group__notification-container">
        <img src="../assets/nav-notification.svg" alt="" />
      </div>
      <div class= "right-group__dot-counter"></div>
      <div class= "right-group__profile-container">
        <img src="../assets/nav-profile.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<style scoped>
#navigation-mobile {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    height: 18.57vw;
    margin-top: 4.32vw;
}
.navigation-mobile__left-group {
    display: flex;
    align-items: center;
    padding-left: 3.81vw;
}
.left-group__burger-icon img {
    height: 11.7vw;
    width: 11.7vw;
}
.left-group__logo img {
  height: 8.9vw;
    width: 11.45vw;
}
.navigation-mobile__right-group {
    display: flex;
    align-items: center;
    padding-right: 3.81vw;
}
.right-group__notification-container {
    height: 9.8vw;
    width: 9.8vw;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #2F363D;
    border-radius: 3.05vw;
}
.right-group__notification-container img {
    height: 4.8vw;
    width: 4.8vw;
}
.right-group__profile-container {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 1.9vw;
    height: 9.28vw;
}

.right-group__profile-container img{
    height: 9.28vw;
}
.right-group__dot-counter {
    height: 2.65vw;
    width: 2.65vw;
    border-radius: 50%;
    background-color: #D9B75F;
    position: relative;
    left: -2.2vw;
    top: -3.5vw;
}
</style>
