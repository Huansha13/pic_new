<template>
  <div class="section-banner-wsp">
   <div class="backgroundBanner">
     <div class="sect-title">
       <h2 class="d-flex-align"><i class="uil uil-whatsapp"></i>Únete al grupo de WhatsApp</h2>
       <div class="selecResidencia">Selecciona tú país de residencia:</div>
     </div>
     <div class="row">
       <div class="col-12 col-sm-12 col-md-6 col-lg-4">
         <div class="box-banner">
           <img src="https://www.calculadoradefletes.com/assets/img/flags/panama.svg" alt="">
           <h3>Panamá | +50762197664</h3>
         </div>
       </div>
       <div class="col-12 col-sm-12 col-md-6 col-lg-4">
         <div class="box-banner">
           <img src="https://www.calculadoradefletes.com/assets/img/flags/peru.svg" alt="">
           <h3>Perú | +51920301745</h3>
         </div>
       </div>
       <div class="col-12 col-sm-12 col-md-6 col-lg-4">
         <div class="box-banner">
           <img src="https://res.cloudinary.com/yfr/image/upload/v1620209403/portafolio/venezuela_kxu5j4.svg" alt="">
           <h3>Venezuela | +582127632240</h3>
         </div>
       </div>
     </div>
   </div>
  </div>
</template>

<style lang="scss">
@import "src/components/style";
.section-banner-wsp {
  margin: 0 105px;
  position: relative;
}
.backgroundBanner {
  background: $colorLight;
  position: absolute;
  left: 0;
  top: -125px;
  width: 100%;
}
.box-banner {
  cursor: pointer;
  &:hover {
    background: $colorDrak;
  }
  img {
    width: 50px;
  }
  h3 {
    margin: 5px 0;
  }
  p {
    font-size: 14px;
  }
}
.sect-title {
  padding: 10px 24px;
  h2 {
    font-size: 20px;
    font-weight: 500;
    letter-spacing: 2px;
    text-transform: uppercase;
    margin: 5px;
    i {
      font-size: 28px;
      margin-right: 5px;
    }
  }
}
.box-banner {
  padding: 10px 15px;
  margin: 10px 30px;
}
.selecResidencia {
  font-size: 13px;
  text-transform: uppercase;
  margin-left: 42px;
}

@media (max-width: 768px) {
  .conte-home {
    padding: 32px 32px 32px 32px !important;
  }
  .backgroundBanner {
    position: relative;
    left: auto;
    top: auto;
  }
  .section-banner-wsp {
    margin: auto;
    padding: 15px;
    background: $colorLight;
    position: relative;
  }
  .btnInfo {
    display: grid !important;
  }
  .wspBtn {
    margin-top: 10px;
    margin-left: 0 !important;
  }
}

</style>
