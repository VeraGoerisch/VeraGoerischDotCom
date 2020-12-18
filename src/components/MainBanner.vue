<template>
  <el-row>
    <el-col :span="24"
      ><div class="background">
        <el-avatar
          class="avatar"
          :size="250"
          :src="require('@/assets/images/profile.jpg')"
        ></el-avatar>
        <h2>Vera Goerisch</h2>
        <h3>Front-End Web Developer</h3>
        <el-row class="buttons">
          <ActionButton href="mailto:contact@veragoerisch.com"
            ><EmailIcon class="icon"
          /></ActionButton>
          <ActionButton
            href="https://www.linkedin.com/in/veragoerisch/"
            is-new-tab
            ><LinkedInIcon class="icon"
          /></ActionButton>
          <ActionButton href="https://github.com/VeraGoerisch" is-new-tab
            ><GitHubIcon class="icon"
          /></ActionButton>
          <el-tooltip
            content="Download Resume"
            placement="bottom"
            effect="light"
          >
            <ActionButton
              href="/files/resume.pdf"
              :is-download="true"
              file-name="resume_vera_goerisch"
              ><DownloadIcon class="icon"
            /></ActionButton>
          </el-tooltip>
        </el-row>
      </div>
    </el-col>
  </el-row>
</template>
<script>
import ActionButton from './ActionButton';
import EmailIcon from './icons/EmailIcon';
import GitHubIcon from './icons/GitHubIcon';
import LinkedInIcon from './icons/LinkedInIcon';
import DownloadIcon from './icons/DownloadIcon';
export default {
  components: {
    ActionButton,
    EmailIcon,
    GitHubIcon,
    LinkedInIcon,
    DownloadIcon,
  },
};
</script>

<style scoped lang="scss">
.background {
  background: url('../assets/images/background.jpg') no-repeat center center
    fixed;
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

@media only screen and (max-width: 400px) {
  .background h2 {
    font-size: 40px;
  }
  .background h3 {
    font-size: 20px;
  }
}
</style>
