<template>
  <div id="pcs-sold">
    <div className="pcs-sold__super-info">
      <div className="super-info__text">
        <span>456K Pcs</span>
      </div>
      <div className="super-info__dropdown">
        <div className="dropdown__title">
          <div className="title__drop">
            <span>Daily</span>
          </div>
          <div>
            <img
              className="title__icon"
              src="../assets/images/arrow-down.svg"
            />
          </div>
        </div>
        <div className="dropdown-content">
          <span>Hello World!</span>
        </div>
      </div>
    </div>
    <div className="pcs-sold__second-info">
      <span>Ticket Sold</span>
    </div>
    <div className="pcs-sold__progress-bar">
      <div className="progress-bar__value"></div>
    </div>
  </div>
</template>

<style scoped>
#pcs-sold {
  background-color: #2f363d;
  border-radius: 15px;
  margin: 0 5vw 5vw;
  padding-bottom: 5.6vw;
}
.pcs-sold__super-info {
  margin: 0 6.36vw;
  padding: 25px 0 0 0;
  display: flex;
  justify-content: space-between;
}
.super-info__dropdown {
  position: relative;
  display: inline-block;
}
.dropdown__title {
  display: flex;
}

.title__drop {
  font-size: 3.18vw;
  padding-right: 12px;
  color: #b7b7b7;
}
.super-info__text {
  font-weight: 600;
  font-style: normal;
  font-size: 4.07vw;
  line-height: 25px;
  letter-spacing: 1px;
}
.title__icon {
  width: 3.18vw;
  height: 3.18vw;
}
.pcs-sold__second-info {
  text-align: left;
  margin: 0 6.36vw;
  font-size: 3.18vw;
  font-weight: 300;
  color: #b7b7b7;
}
.pcs-sold__progress-bar {
  height: 2.17vw;
  background: rgba(255, 255, 255, 0.12);
  border-radius: 40.8407px;
  transform: matrix(1, 0, 0, -1, 0, 0);
  margin: 5.6vw 6.36vw 0;
}
.progress-bar__value {
  height: 100%;
  width: 80%;
  background: #13b497;
  box-shadow: 0px 0px 16.7552px rgba(19, 180, 151, 0.56);
  border-radius: 40.8407px;
  transform: matrix(1, 0, 0, -1, 0, 0);
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  padding: 12px 16px;
  z-index: 1;
}

.super-info__dropdown:hover .dropdown-content {
  display: block;
}
</style>
