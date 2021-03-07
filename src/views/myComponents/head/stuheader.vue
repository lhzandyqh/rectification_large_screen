<template>
  <div class="header-bg">
    <!--    <img src="../../../assets/pic/header_bg.png" class="header-img">-->
    <div class="header_content">
      <div class="time_container">
        <span>2021-02-03</span>
      </div>
      <div class="layer_container" @click="gotoMajorLayer">
        <span>专业层面</span>
        <!--        <div class="layer_content">-->
        <!--          <span>专业层面</span>-->
        <!--        </div>-->
      </div>
      <div class="layer_container" @click="gotoCourseLayer">
        <span>课程层面</span>
        <!--        <div class="layer_content">-->
        <!--          <span>课程层面</span>-->
        <!--        </div>-->
      </div>
      <div class="main_head" @click="gotoSchoolLayer">
        <span>石家庄人民医专大屏监控平台</span>
      </div>
      <div class="goset">
        <img src="../../../assets/icon/goSet.png" @click="gotoManagementPlatform">
      </div>
      <div class="pro_layer_container_right" @click="gotoStudentLayer">
        <div class="layer_content_right">
          <span>学生层面</span>
        </div>
      </div>
      <div class="layer_container_right" @click="gotoTeacherLayer">
        <div class="layer_content_right">
          <span>教师层面</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  methods: {
    gotoManagementPlatform: function() {
      this.$router.push('/documentation/index')
    },
    gotoMajorLayer: function() {
      this.$router.push('/majorindex')
    },
    gotoSchoolLayer: function() {
      this.$router.push('/dashboard')
    },
    gotoCourseLayer: function() {
      this.$router.push('/courseindex')
    },
    gotoTeacherLayer: function() {
      this.$router.push('teacherIndex')
    },
    gotoStudentLayer: function() {
      this.$router.push('studentIndex')
    }
  }
}
</script>

<style scoped>
.header-bg {
  width: 100%;
  height: 5.5rem;
  position: relative;
  background: url("../../../assets/pic/header_bg.png") no-repeat;
  background-size: 100% 100%;
}
.header_content {
  width: 100%;
  /*position: absolute;*/
  /*top: 1rem;*/
}
.time_container {
  width: 6%;
  float: left;
  margin-top: 1.6rem;
  margin-left: 1.6rem;
  /*position: absolute;*/
  /*top: 1.6rem;*/
}
.time_container span {
  font-size: 1rem;
  font-weight: bold;
}
.layer_container {
  text-align: center;
  cursor: pointer;
  width: 8%;
  height: 3rem;
  float: left;
  border: 1px solid #44a5fc;
  transform: skewX(40deg);
  margin-left: 2rem;
  margin-top: 0.6rem;
}
.layer_container span {
  line-height: 3rem;
  display: block;
  width: 100%;
  height: 3rem;
  transform: skewX(-40deg);
  font-weight: bold;
  color:#44a5fc ;
}
.main_head {
  margin-top: 0.8rem;
  height: 3rem;
  width: 25%;
  float: left;
  text-align: center;
  margin-left: 11%;
  cursor: pointer;
}
.main_head span {
  line-height: 3rem;
  font-size: 1.5rem;
  color: #3b91b6;
  font-weight: bold;
}
.layer_container :hover {
  /*/*text-align: center;*/
  /*width: 100%;*/
  /*height: 3rem;*/
  box-shadow:0rem 0rem 0.2rem 0.2rem #b1dde8;
  transform: skewX(0deg);
  background-color: #44a5fc;
  color: white;
}
.layer_container_right {
  text-align: center;
  cursor: pointer;
  width: 8%;
  height: 3rem;
  float: right;
  border: 1px solid #44a5fc;
  transform: skewX(-40deg);
  margin-right: 2rem;
  margin-top: 0.6rem;
}
.layer_container_right :hover {
  /*/*text-align: center;*/
  /*width: 100%;*/
  /*height: 3rem;*/
  box-shadow:0rem 0rem 0.2rem 0.2rem #b1dde8;
  transform: skewX(0deg);
  background-color: #44a5fc;
  color: white;
}
.layer_content_right {
  text-align: center;
  transform: skewX(40deg);
}
.layer_content span {
  line-height: 3rem;
  color: #44a5fc;
  font-weight: bold;
}
.layer_content_right span {
  line-height: 3rem;
  display: block;
  width: 100%;
  height: 3rem;
  /*transform: skewX(-40deg);*/
  font-weight: bold;
  color:#44a5fc ;
}
.pro_layer_container_right {
  cursor: pointer;
  width: 8%;
  height: 3rem;
  float: right;
  border: 1px solid #44a5fc;
  transform: skewX(-40deg);
  margin-right: 2rem;
  margin-top: 0.6rem;
  background-color:#44a5fc;
}
.pro_layer_container_right span {
  line-height: 3rem;
  display: block;
  width: 100%;
  height: 3rem;
  /*transform: skewX(-40deg);*/
  font-weight: bold;
  color:white ;
}
.goset {
  width: 4%;
  margin-right: 2rem;
  height: 3rem;
  float: right;
  margin-top: 1rem;
  cursor: pointer;
}
.goset img {
  width: 2rem;
  height: 2rem;
}
/*.header-img {*/
/*  width: 100%;*/
/*  height: 5.5rem;*/
/*  position: relative;*/
/*}*/
</style>

