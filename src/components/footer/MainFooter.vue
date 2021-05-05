<template>
  <div class="content-footer">
    <div class="row">
      <div class="col-12 col-sm-12 col-mg-12 col-lg-4">
        <div class="box__left">
          <h3>Suscríbete a nuestro Taller</h3>
          <br>
          <div class="input__btn">
            <input class="input_txt" type="email" placeholder="Email">
            <button class="btn__send"><i class="uil uil-message"></i></button>
          </div>
          <br>
          <div class="liner"></div>
          <br>
          <div class="section__copy_list d-flex-align">
            <span>
              ©2021
              <span>PIC Cargo, todo los derechos reservados</span>
            </span>
            <ul class="list__redes__sociales">
              <li><a href="#"><i class="uil uil-facebook-f"></i></a></li>
              <li><a href="#"><i class="uil uil-twitter"></i></a></li>
              <li><a href="#"><i class="uil uil-instagram"></i></a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-12 col-sm-12 col-mg-12 col-lg-8">
        <div class="box__right">
          <div class="enlaces d-flex">
            <ul>
              <div class="title_heading">Taller</div>
              <li class="subTitle" v-for="tall in taller">{{tall}}</li>
            </ul>
            <ul class="sec__pic">
              <div class="title_heading">PIC</div>
              <li class="subTitle" v-for="pic in pics">{{pic}}</li>
            </ul>
            <div class="">
              <div class="title_heading">Nosotros</div>
              <ul class="ul__nosotros">
                <li class="subTitle" v-for="nst in nosotros">{{nst}}</li>
              </ul>
            </div>

          </div>
          <div class="box_address__btns d-flex-align">
            <div class="address">
              <div class="sec_address" v-for="add in address">
                <span>{{add.name}}</span>
                <p>{{add.des}}</p>
                <br>
              </div>
            </div>
            <div class="btns">
              <button> <i class="uil uil-whatsapp"></i> &nbsp; WhatsApp </button>
              <button><img src="https://www.flaticon.com/svg/vstatic/svg/555/555605.svg?token=exp=1620174336~hmac=f42e3ba7fb15a8c6f65eea95ef251027" alt=""> &nbsp; Perú </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.box__left {
  padding-right: 55px;
  margin-right: 25px;
  border-right: 2px solid #262626;
  padding-bottom: 100px;
  h3 {
    color: #FFFFFF;
    font-size: 24px;
  }
}
.content-footer {
  background: #121212;
  height: 100vh;
  padding: 72px;
}
.input__btn {
  display: flex;
  align-items: center;
}
.input_txt{
  background: #262626;
  width: 100%;
  color: #FFFFFF;
  height: 48px;
  outline: none;
  border: none;
  margin-right: 5px;
  padding-left: 5px;
  font-size: 16px;
}
.btn__send {
  background: #e0ff00;
  width: 48px;
  height: 48px;
  border: none;
  outline: none;
  cursor: pointer;
  i {
    color: #121212;
    font-size: 24px;
  }
}
.liner {
  margin-top: 50px;
  margin-bottom: 25px;
  padding-bottom: 5px;
  border-bottom: 2px solid #262626;
}
.section__copy_list{
  span {
    color: #FFFFFF;
    opacity: .7;
    font-size: 13px;
    display: flex;
    flex-direction: column;
    line-height: 25px;
  }
}
.list__redes__sociales {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  li {
    margin-left: 11px;
  }
  li a {
    color: #FFFFFF;
    font-size: 24px;
  }
}
.enlaces {
  justify-content: space-between;
  margin-bottom: 10px;
  padding-bottom: 20px;
  border-bottom: 2px solid #262626;
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }
}
.ul__nosotros {
  columns: 2;
  -webkit-columns: 2;
  -moz-columns: 2;
}
.title_heading {
  margin-bottom: 25px;
  padding-top: 25px;
  color: #e0ff00;
  font-weight: 700;
  font-size: 16px;
}
.subTitle {
  color: #676767;
  font-size: 13px;
  margin-bottom: 23px;
  cursor: pointer;
  &:hover {
    color: #e0ff00;
  }
}
.btns {
  display: flex;
  align-items: center;
  button {
    width: 150px;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #262626;
    color: #A8A8A8;
    font-size: 16px;
    border: none;
    outline: none;
    margin-left: 15px;

    I {
      font-size: 24px;
    }
    img {
      width: 24px;
    }
  }
}
.box_address__btns {
  margin-top: 30px;
}
.sec_address {
  span {
    color: #FFFFFF;
    font-size: 16px;
    font-weight: 700;
  }
  p {
    margin: 0;
    padding-top: 10px;
    color: #535353;
  }
}
@media (max-width: 768px) {
  .sec__pic {
    padding-left: 40px !important;
  }
  .subTitle {
    margin-bottom: 15px;
  }
  .box_address__btns {
    flex-wrap: wrap;
    .btns {
      justify-content: space-between;
      display: flex;
      width: 100%;
      button {
        margin-left: 0 !important;
      }
    }
  }
}
</style>

<script>
export default {
  data() {
    return {
      address: [
        {
          name: 'HQ Buenos Aires',
          des: 'El Salvador 5218, Piso 3 Oficina 308, Palermo Soho, CP 1414, Buenos Aires, Argentina'
        },
        {
          name: 'HQ Miami',
          des: '3000 NE 2nd Avenue, Miami, FL 33137'
        }
      ],
      taller: [
          'cursos',
          'Prodcuto',
          'Data',
          'Herramientas'
      ],
      pics: [
          'Plataforma',
          'Preguntas',
          'Frecuencia'
      ],
      nosotros: [
          'Equipo',
          'Referidos',
          'empresas',
          'Nueva historia',
          'Prensa',
          'ONGs',
          'Testimonios',
          'Alianzas',
          'Trabaja con nosotros',
          'Terminos de uso'
      ]
    }
  }
}
</script>
