<template>
  <div class="presentacion__section">
    <div class="row">
      <div class="col-12 col-sm-12 col-md-6 col-lg-6">
        <div class="presentation-txt__box">
          <h2>
            Importaciones para Pymes y Emprendedores
          </h2>
          <div class="liner-hor"></div>
          <br>
          <div class="txt-info">
            Las principales desafiantes al momento de empezar una IMPORTACIÓN son: La falta de capital y el desconocimiento de proveedores confiables.
            Por lo antes expuesto PIC CARGO ha creado una nueva linea de atención a nuestros importantes para que puedan realizar su importación facil y segura.
          </div>
        </div>
      </div>
      <div class="col-12 col-sm-12 col-md-6 col-lg-6">
        <div class="presentation-txt__box">
          <h2>
            ¿Por qué es importante contar con el respaldo de un buen corredor de aduanas?
          </h2>
          <ul class="list-impo">
            <li v-for="(imp, index) in importante"><i class="uil uil-check"></i> &nbsp; {{imp}}</li>
          </ul>
          <br>
<!--          <h2>-->
<!--            ¿Qué costos debo considerar para realizar una operación exitosa?-->
<!--          </h2>-->
<!--          <ul class="list-cost">-->
<!--            <li v-for="(cost, index) in costos" :key="cost"><i class="uil uil-check"></i> &nbsp; {{cost.name}}-->
<!--              <ol>-->
<!--                <li>{{cost.descrip}}</li>-->
<!--              </ol>-->
<!--            </li>-->
<!--          </ul>-->
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "src/components/style";
.presentacion__section {
  background: #121212;
  margin: 32px;
  padding: 30px;
}
.presentation-txt__box {
  padding: 40px 60px;
  h2 {
    font-size: 36px;
    color: #FFFFFF;
  }
}
.liner-hor {
  width: 60px;
  height: 16px;
  background: $colorLight;
}
.txt-info {
  text-align: justify !important;
  color: #FFFFFF;
  font-size: 16px;
  line-height: 2;
}
.presentation-txt__box {
  h2 {
    font-size: 20px;
  }
}
.list-impo {
  list-style: none;
  margin: 0;
  padding: 0;
  li {
    margin-bottom: 20px;
    color: #FFFFFF;
    i {
      color: $colorLight;
      font-size: 24px;
    }
  }
}
.list-cost {
  list-style: none;
  margin: 0;
  padding: 0;
  li {
    color: #FFFFFF;
    margin-bottom: 10px;
    i {
      font-size: 24px;
      color: $colorLight;
    }
    ol {
      margin-left: 15px;
      margin-top: 6px;
    }
  }
}


@media (max-width: 768px) {
  .presentacion__section {
    margin: 0;
  }
  .presentation-txt__box {
    padding: 0;
  }
}

</style>

<script>
export default {
  data() {
    return {
      importante: [
          'Aranceles de Importación',
          'Evitar costos extras',
          'Disminuir costos de importación',

      ],
      costos: [
        {
          name: 'Costos del país de origen',
          descrip:  'Honorarios Aduana de exportación'
        },
        {
          name: 'Costos de Destino',
          descrip: 'Honorarios Aduana de Importación'
        }
      ]
    }
  }
}
</script>
