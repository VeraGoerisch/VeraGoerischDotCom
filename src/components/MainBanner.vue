<template>
  <el-row>
    <el-col :span="24"
      ><div class="background">
        <el-avatar
          class="avatar"
          :size="250"
          src="/images/profile.jpg"
        ></el-avatar>
        <h2>Vera Goerisch</h2>
        <h3>Front-End Web Developer</h3>
        <el-row class="buttons">
          <a
            class="button"
            href="mailto:contact@veragoerisch.com"
            @click="$event.currentTarget.blur()"
            ><i class="far fa-envelope"></i
          ></a>
          <a
            class="button"
            href="https://www.linkedin.com/in/veragoerisch/"
            target="_blank"
            @click="$event.currentTarget.blur()"
            ><i class="fab fa-linkedin-in"></i
          ></a>

          <a
            class="button"
            href="https://github.com/VeraGoerisch"
            target="_blank"
            @click="$event.currentTarget.blur()"
            ><i class="fab fa-github"></i
          ></a>
          <el-tooltip
            content="Download Resume"
            placement="bottom"
            effect="light"
          >
            <a
              class="button"
              href="/files/resume_vera_goerisch.pdf"
              download
              @click="$event.currentTarget.blur()"
              ><i class="fas fa-file-download"></i
            ></a>
          </el-tooltip>
        </el-row>
      </div>
    </el-col>
  </el-row>
</template>
<script>
export default {};
</script>

<style scoped lang="scss">
.background {
  background: url('/images/background.jpg') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  height: 500px;
  position: relative;
  margin-bottom: 30px;
  h2,
  h3 {
    color: #fff;
    font-weight: 300;
    text-transform: uppercase;
    letter-spacing: 0.15em;
  }
  h2 {
    font-size: 48px;
    letter-spacing: 6px;
    margin: 0 0 30px;
  }
  h3 {
    font-size: 24px;
    letter-spacing: 3px;
  }
}
.avatar {
  margin: 30px auto 20px;
}
.buttons {
  position: absolute;
  top: 460px;
  width: 100%;
  margin: 0 auto;
}
.button {
  display: inline-block;
  margin: 7px;
  height: 60px;
  width: 60px;
  border-radius: 50%;
  color: #fff;
  background-color: #989898;
  font-size: 30px;
  line-height: 60px;
  &:hover,
  &:focus,
  &:active {
    background-color: #858585;
    color: #e7e7e7;
  }
}
</style>
