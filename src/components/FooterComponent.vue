<template>
  <el-row class="footer-row">
    <el-col :span="12">
      <p>
        Made with ❤️ by
        <a href="https://github.com/jwenjian" target="_blank">jwenjian</a>
      </p>
      <span class="copyright">
        Version: v{{ version }}
      </span>
      <span class="copyright">
        Icons made by
        <i>Freepik</i> from
        <u>www.flaticon.com</u>
      </span>
      <span class="copyright">
        Sound made by
        <i>pierrecartoons1979</i> from
        <u>freesound.org</u>
      </span>
    </el-col>
  </el-row>
</template>

<script>
const VERSION = require('../../package.json').version

export default {
  name: 'footer-component',
  data() {
    return {
      version: VERSION
    }
  },
  mounted() {
    console.log(VERSION)
  }
};
</script>

<style>
.footer-row {
  font-size: smaller;
  text-align: left;
  padding-left: 1em;
  margin-top: 2em;
}
.copyright {
  display: block;
  font-size: smaller;
}
</style>