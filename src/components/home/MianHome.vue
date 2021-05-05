<template>
  <div class="conte-home">
    <div class="row">
      <div class="col-12 col-sm-12 col-md-6 col-lg-5">
        <div class="box-home">
          <h2 class="title-h2">Calculadora de fletes e impuestos de aduana</h2>
          <h1 class="title-h1">Importaciones grupales</h1>
          <div class="sectionPeoples d-flex-align">
            <ul class="listPeople d-flex-align">
              <li><a href=""><img src="https://www.calculadoradefletes.com/assets/img/flags/venezuelaRound.svg" alt=""> </a></li>
              <li><a href=""><img src="https://www.calculadoradefletes.com/assets/img/flags/peruRound.svg" alt=""></a></li>
              <li><a href=""><img src="https://www.calculadoradefletes.com/assets/img/flags/panamaRound.svg" alt=""></a></li>
            </ul>
            <div class="secTxtRec d-flex-align">
              <span class="txtCantidadR">Más de <span style="color: #e0ff00">10.000 personas</span> nos recomiendan</span>
            </div>
          </div>
          <div class="sectionChecks">
            <ul>
              <li><i class="uil uil-check-circle"></i> &nbsp; Aranceles de Importación</li>
              <li><i class="uil uil-check-circle"></i> &nbsp; Evitar costos extras</li>
              <li><i class="uil uil-check-circle"></i> &nbsp; Disminuir costos de importación</li>
            </ul>
          </div>
          <div class="btnInfo d-flex-align">
            <button class="btnTgi tgi"> <i class="uil uil-user-arrows"></i> Taller gratuito </button>
            <button class="wspBtn"><i class="uil uil-whatsapp"></i>¿Tienes dudas? Escríbenos!</button>
          </div>
          <div class="calidad d-flex-align">
           <i> Calidad 100% asegurada</i> &nbsp;<i class="uil uil-info-circle"></i>
          </div>
        </div>
      </div>
      <div class="col-12 col-sm-12 col-md-6 col-lg-7">
        hola
      </div>
    </div>
  </div>
  <BtnWsp></BtnWsp>
</template>
<script>
import MainNav from "@/components/nav/MainNav";
import BtnWsp from "@/components/btnWhatsaap/btnWsp";
export default {
  components: {BtnWsp, MainNav}
}
</script>

<style lang="scss">
@import "src/components/style";
.conte-home {
  padding: 32px 32px 250px 32px;
}
.title-h2 {
  color: white;
  font-size: 36px;
  margin: 15px 0 4px 0 ;
}
.title-h1 {
  color: $colorLight;
  font-size: 60px;
  margin: 4px 0 0 0 ;
}
.sectionPeoples {
  margin-top: 35px;
}
.listPeople {
  list-style: none;
  margin: 0;
  padding: 0;
  li {
    margin-right: -5px;
  }
  li a img {
    width: 25px;
  }
}
.secTxtRec {
  margin-left: 20px;
}
.txtCantidadR {
  color: #FFFFFF;
  font-size: 16px;
}
.sectionChecks {
  ul {
    list-style: none;
    margin: 30px 0 0 0 ;
    padding: 0;
  }
  ul li {
    color: #FFFFFF;
    margin-top: 8px;
    font-size: 16px;
    display: flex;
    align-items: center;
    i {
      color: $colorLight;
      font-size: 24px;
    }
  }

}
.btnInfo {
  margin-top: 20px;
}
.wspBtn, .btnTgi {
  display: flex;
  align-items: center;
  margin-left: 15px;
  border: 2px solid #7ad06d;
  color: #7ad06d;
  background: transparent;
  padding: 4px 22px;
  outline: none;
  font-weight: 700;
  font-size: 16px;
  cursor: pointer;
  i {
    font-size: 30px;
    margin-right: 10px;
  }
  &:hover {
    background: #7ad06d;
    color: #121212;
  }
}
.calidad {
  margin-top: 10px;
  color: #FFFFFF;
  font-size: 13px;
  opacity: .5;
}
.btnTgi {
  border: 2px solid $colorLight !important;
  color: $colorLight !important;
  margin-left: 0 !important;
  justify-content: center;
  &:hover {
    background: $colorLight;
    color: #121212 !important;
  }
}
.tgi {
  i {
    font-size: 30px;
  }
}
@media (max-width: 768px) {
  .listPeople li {
    margin-right: 10px;
    margin-bottom: 15px;
  }
  .listPeople {
    justify-content: center;
  }
  .sectionPeoples {
    display: grid !important;
  }
  .title-h1 {
    font-size: 40px;
  }
  .title-h2 {
    font-size: 25px;
  }
}
</style>
