<template>
  <div class="loaderoverlay" id="loadoverlay">
    <div class="full-height valign-wrapper">
      <div class="full-width center">
        <div class="row">
          <div class="col s6 offset-s3">
            <div class="progress">
              <!-- <div class="determinate" style="width: 70%;"></div> -->
              <div class="indeterminate"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  methods: {
    showLoad(event) {
      this.style.display = none;
    },

    hideLoad(event) {
      this.style.display = block;
    }
  }
};
</script>

<style>
  .loaderoverlay {
    position: fixed;
    /* display: none; */
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgba(255, 255, 255, 0.7);
    z-index: 10000;
    cursor: pointer;
  }
</style>
