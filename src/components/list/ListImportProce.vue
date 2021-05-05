<template>
  <div class="sectionProceso">
    <br>
    <div class="lisPeople">
      <ul class="d-flex-align" style="padding: 0;">
        <li v-for="n in imge"><img class="persona" v-bind:src="n"></li>
      </ul>
    </div>
    <div class="listImportaciones">
      <h1>Más de <span>15.000 Personas</span> nos recomiendan</h1>
      <h3>IMPORTACIONES EN PROCESO ...</h3>
    </div>
    <div class="section-box-list">
      <div class="btn__scroll">
        <button><i class="uil uil-angle-left-b"></i></button>
        <button><i class="uil uil-angle-right-b"></i></button>
      </div>
      <div class="sectionListProduct">
        <div class="boxList" v-for="n in 10">
          <img class="img-prod" src="https://res.cloudinary.com/yfr/image/upload/v1620078368/pic/descarga_4_l9kyd1.jpg" alt="">
          <div class="sub-box">
            <h4> Carteras, edredones, relojes, ferretería y repuestos de autos</h4>
            <div class="destino">
              <ul class="">
                <li><img class="bandera" src="https://www.calculadoradefletes.com/assets/img/flags/venezuelaRound.svg" alt=""> &nbsp;Desde Venezuela</li>
                <span>Cierra el <b>15 May.</b>  y Llega el <b> 15 Jun.</b></span>
              </ul>
            </div>
          </div>
          <div class="dates">
            <span class="via">Vía <i class="uil uil-ship"></i> &nbsp; Marítimo</span>
          </div>
        </div>
      </div>
    </div>
    <br>
    <div class="btn__todo">
      <button>Mirar todo las importaciones <i class="uil uil-arrow-right"></i></button>
    </div>
    <br> <br>
  </div>
</template>

<style lang="scss">
@import "src/components/style";
.sectionProceso {
  margin-top: 150px;
}
.lisPeople {
  ul {
    list-style: none;
    justify-content: center;
  }
  li {
    margin-right: -10px;
  }
  ul li .persona {
    width: 50px;
    height: 50px;
    object-fit: cover;
    border-radius: 50%;
  }
}
.listImportaciones {
  padding: 32px 32px 0 32px;
  h1 {
    text-align: center;
    span {
      margin-bottom: 2px;
      padding-bottom: 2px;
      border-bottom: 3px solid $colorLight;
    }
  }
  h3 {
    text-align: center;
    margin-top: 25px;
    padding-top: 25px;
    border-top: 1px solid #b0b0b0;
  }
}
.sectionListProduct {
  display: flex;
  overflow: auto;
  &::-webkit-scrollbar {
    display: none;
  }
}
.boxList {
  min-width: 400px;
  background: #FFFFFF;
  box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.25);
  margin: 0 5px 32px 32px;
  cursor: pointer;
  border-radius: 5px 5px 0 0;
  &:hover {
    //background: rgba(203, 203, 203, 0.1);
  }
  .img-prod {
    width: 100%;
    height: 150px;
    object-fit: cover;
    border-radius: 5px 5px 0 0;
  }
  h4 {
    margin: 0;
    font-weight: 500;
    padding: 20px 0 15px 0;
    font-size: 16px;
    text-transform: uppercase;
    opacity: .7;
  }
}
.section-box-list {
  position: relative;
}
.bandera {
  width: 30px;
}
.destino {
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    li {
      display: flex;
      align-items: center;
      b {
        margin-right: 10px;
      }
    }
  }
}
.sub-box {
  padding: 0 10px 10px 10px;
}
.dates {
  padding: 10px;
  font-size: 13px;
}
.destino {
  ul li {
    font-size: 16px;
    font-weight: 500;
    text-transform: uppercase;
    margin-bottom: 7px;
    i {
      font-size: 18px;
    }
  }
}

.via{
  opacity: .5;
  font-size: 15px;
  margin-left: 5px;
  i {
    margin-left: 5px;
    font-size: 18px;
  }
}
.btn__scroll {
  height: 100%;
  display: flex;
  align-items: center;
  padding: 0 32px;
  z-index: 1;
  margin-bottom: 10px;
  button {
    width: 40px;
    height: 40px;
    color: #FFFFFF;
    background: #121212;
    border: none;
    outline: none;
    margin-right: 10px;
    cursor: pointer;
    i {
      font-size: 24px;
    }
  }
}
@media (max-width: 768px) {
  .sectionProceso {
    margin-top: 10px;
  }
  .listImportaciones {
   padding: 0;
    text-align: center;
  }
  .boxList {
    min-width: 350px !important;
  }
}
.btn__todo {
  display: flex;
  justify-content: center;
  button {
    border: 1px solid #333;
    padding: 12px;
    font-size: 16px;
    background: #FFFFFF;
    font-weight: 500;
    cursor: pointer;
    display: flex;
    justify-content: center;
    align-items: center;
    i {
      margin-left: 5px;
      font-size: 24px;
    }
    &:hover {
      background: #121212;
      color: #FFFFFF;
    }
  }
}

</style>

<script>
export default  {
  data() {
    return {
      imge: [
          'https://t1.pb.ltmcdn.com/es/posts/4/8/4/que_significa_sonar_con_la_persona_que_te_gusta_5484_600.jpg',
          'https://definicion.de/wp-content/uploads/2015/03/Varon.jpg',
          'https://www.limaorganica.pe/wp-content/uploads/2020/05/killa-larga-hombre-700x460.jpg',
          'https://english.indiana.edu/images/profiles/profiles-768x768/connolly_joseph.jpg'
      ]
    }
  }
}
</script>
