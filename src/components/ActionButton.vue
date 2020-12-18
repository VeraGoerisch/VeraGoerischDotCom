<template
  ><a
    class="button"
    :href="href"
    :target="isNewTab ? '_blank' : '_self'"
    :download="isDownload ? this.fileName : false"
    @click="$event.currentTarget.blur()"
    ><slot></slot
  ></a>
</template>

<script>
export default {
  props: {
    isDownload: {
      type: Boolean,
      required: false,
      default: false,
    },
    fileName: {
      type: String,
      required: false,
      default: 'file',
    },
    href: {
      type: String,
      required: true,
    },
    isNewTab: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
};
</script>

<style scoped lang="scss">
.button {
  display: inline-block;
  margin: 7px;
  height: 60px;
  width: 60px;
  border-radius: 50%;
  background-color: #989898;
  .icon {
    padding: 15px;
    width: 30px;
    height: 30px;
    fill: #fff;
  }
  &:hover,
  &:focus,
  &:active {
    background-color: #858585;
    .icon {
      fill: #e7e7e7;
    }
  }
}
</style>
