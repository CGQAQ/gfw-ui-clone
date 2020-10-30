<template>
  <div class="sidebar__root">
    <div class="speed">
      <div class="speed__upload">
        <span>↑</span><span>0</span><span>B/s</span>
      </div>
      <div class="speed__download">
        <span>↓</span><span>0</span><span>B/s</span>
      </div>
    </div>
    <div class="nav">
      <div class="nav__selected">General</div>
      <div class="nav__selected_next">Proxies</div>
      <div>Profiles</div>
      <div>Logs</div>
      <div>Connections</div>
      <div>Settings</div>
      <div>Feedback</div>
    </div>
    <div class="status">
      <div class="status__top">00:25:59</div>
      <div class="status__bottom"><font-awesome-icon class="status__icon" icon="circle"/> Connected</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideBar",
  components: ['font-awesome-icon']
}
</script>

<style scoped>
.sidebar__root {
  width: 170px;
  height: 95vh;
  background: #F5F5F5;
  display: flex;
  flex-direction: column;
}

.speed {
  width: 100%;
  height: 80px;
  font-weight: lighter;
  font-size: 100%;
  color: #34373b;
  border-bottom: #DCDCDC 1px solid;
}

.speed__upload span:nth-child(odd){
  font-size: 65%;
}

.speed__download span:nth-child(odd){
  font-size: 65%;
}

.speed div {
  display: flex;
  justify-content: space-evenly;
  height: 50%;
}

.speed div span {
  height: 100%;
  line-height: 50px;
}

.nav {
  min-height: 404px;
  background: white;
}

.nav div {
  color: #747D88;
  background: #F5F5F5;
  height: 60px;
  min-height: 60px;
  text-align: center;
  line-height: 70px;
}

.nav__selected {
  color: black !important;
  background: white !important;
}

.nav__selected_next{
  border-top-right-radius: 10px;
}

.status {
  display: flex;
  flex: 1 1 auto;
  flex-direction: column;
  justify-content: flex-end;
  border-top: #DCDCDC 1px solid;
}

.status__icon {
  color: #41B883;
  margin-right: 5px;
  font-size: 85%;
}

.status__top {
  flex: 10 0 auto;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  padding-bottom: 15px;
}

.status__bottom{
  flex: 1 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 85%;
  padding: 5px;
  font-weight: lighter;
  color: #34373b;
  font-family: sans-serif;
}
</style>