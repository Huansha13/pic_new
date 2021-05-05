<template>
  <div class="section__service">
    <div class="title__service">
      Servicios / Corredores
    </div>
    <div class="section__box">
      <div class="box__service" v-for="serv in service">
        <div class="icon__tarifa d-flex-align">
          <span class="icon"> <i :class="serv.icon"></i> </span>
          <span class="titleService">{{serv.title}}</span>
        </div>
        <p class="decrip__p">{{serv.descrp}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      service: [
        {
          icon: 'uil uil-dollar-alt',
          title: 'Tarifas',
          descrp: 'Consulta nuestras tarifas promocionales de fletes marítimos'
        },
        {
          icon: 'uil uil-package',
          title: 'Importar',
          descrp: 'IMPORTA o EXPORTA desde ASIA'
        },
        {
          icon: 'uil uil-lightbulb-alt',
          title: 'Asesoría',
          descrp: 'Asesoría gratuita y personalizada'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import "src/components/style";
.section__service {
  padding: 32px;
  margin-top: 30px;
}
.section__box {
  display: flex;
  justify-content: space-between;
}
.box__service {
  width: 350px;
  margin: 35px 0;
  padding: 15px;
  background: #FFFFFF;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  .titleService {
    text-align: center;
    margin: 0;
    padding: 0;
    letter-spacing: -.015em;
    font-size: 17px;
    color: #121212;
  }
}
.btn-click{
  border: 1px solid $colorLight;
  margin-top: 35px;
  padding: 7px 20px ;
  //background: $colorLight;
  color: $colorLight;
  background: #121212;
  font-size: 16px;
  font-weight: 500;
  font-family: 'DM Sans', sans-serif;
  cursor: pointer;
  &:hover {
    background: $colorLight;
    color: #121212;
  }
}
.title__service {
  font-size: 26px;
  font-weight: 700;
}
.icon {
  i {
    color: #121212;
  }
  display: flex;
  margin-right: 6px;
}
.titleService {
  font-size: 22px !important;
  font-weight: 700;
}
.decrip__p {
  color: #808080 !important;
  padding: 10px 0 0 0 ;
  margin: 0;
}
.icon__tarifa {
  justify-content: start !important;
}
.section__box {
  display: flex;
}
@media (max-width: 768px) {
  .section__box {
    display: block !important;
  }
}
</style>
