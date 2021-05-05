<template>
  <div class="section__sumate">
    <div class="box_txt_btn d-flex-align">
      <h2>Súmate a PIC y lleva tu emprendimiento al siguiente nivel</h2>
      <button class="btn">¡Quiero unirme!</button>
    </div>
  </div>
</template>

<style lang="scss">
.section__sumate {
  padding: 32px;
}
.box_txt_btn {
  justify-content: space-evenly;
  h2 {
    font-size: 36px;
    width: 598px;
    text-align: end;
  }
}
@media (max-width: 767px) {
  .box_txt_btn {
    flex-direction: column !important;
  }
  .box_txt_btn h2 {
    font-size: 30px;
    width: 100%;
    text-align: inherit;
    line-height: 50px;
  }
  .box__left {
    padding-right: 0 !important;
    margin-right: 0 !important;
    border-right: none !important;
  }
  .content-footer {
    height: auto !important;
    padding: 32px !important;
  }
  .enlaces {
    flex-wrap: wrap;
    justify-content: flex-start !important;
    margin-bottom: 0;
    padding-bottom: 0;
    border-bottom: 2px solid #262626;
  }
}
</style>
