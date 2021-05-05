<template>
  <div class="stock__control">
    <h4 class="title_stock">Mercacia en Stock</h4>
    <div class="row">
      <div class="col-12 col-sm-12 col-md-6 col-lg-3" v-for="stock in stocksOne">
        <div class="box-stock one">
          <img class="logo__product" v-bind:src="stock.logoProduct" alt="">
          <h3 class="titleStock_Produc one__title">{{ stock.title }}</h3>
          <ul class="like__logoPais one__like">
            <li class="likeli"><i class="uil uil-heart"></i> &nbsp;{{ stock.like }}</li>
            <li><img class="logo_pais" v-bind:src="stock.logoPais" alt=""> Perú</li>
          </ul>
          <br>
          <div class="section__btn__view">
            <button class="btnView one__btn">Ver inportadores</button>
          </div>
        </div>
      </div>
      <div class="col-12 col-sm-12 col-md-6 col-lg-3" v-for="stock in stocks">
        <div class="box-stock">
          <img class="logo__product" v-bind:src="stock.logoProduct" alt="">
          <h3 class="titleStock_Produc">{{ stock.title }}</h3>
          <ul class="like__logoPais">
            <li class="likeli"><i class="uil uil-heart"></i> &nbsp;{{ stock.like }}</li>
            <li><img class="logo_pais" v-bind:src="stock.logoPais" alt=""> Perú</li>
          </ul>
          <br>
          <div class="section__btn__view">
            <button class="btnView">Ver inportadores</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">

@import "src/components/style";

.stock__control {
  padding: 32px;
  background: #121212;
}
.title_stock {
  font-size: 30px;
  color: #FFFFFF;
  text-align: center;
}
.box-stock {
  display: block;
  margin: auto;
  width: 272px;
  min-height: 447px;
  padding: 15px;
  background: #333333;
  cursor: pointer;
}
.logo__product {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 2px;
}
.logo_pais {
  width: 20px;
  margin-right: 7px;
}
.like__logoPais {
  list-style: none;
  margin: 0;
  padding: 0;
  li {
    font-size: 12px;
    display: flex;
    align-items: center;
    color: #FFFFFF;
    i {
      font-size: 18px;
    }
  }
}
.titleStock_Produc{
  color: #FFFFFF;
  font-weight: 500;
  line-height: 1.7;
}

.likeli {
  margin-bottom: 5px;
  i {
    //color: #F42B1B;
  }
}
.section__btn__view {
  display: flex;
  justify-content: center;
}
.btnView {
  border: 1px solid $colorLight;
  background: transparent;
  height: 40px;
  padding: 0 20px;
  border-radius: 5px;
  color: #FFFFFF;
  font-family: 'DM Sans', sans-serif;
  font-size: 14px;
}
.one {
  background: $colorLight !important;
}
.one__title {
  color: #121212 !important;
}
.one__like {
  li, .likeli, i {
    color: #121212 !important;
  }
}
.one__btn {
  border: 1px solid #121212 !important;
  color: #121212 !important;
}
@media (max-width: 768px) {
  .box-stock {
    width: 100% !important;
    margin-bottom: 15px !important;
  }

}
</style>

<script>
export default  {
  data() {
    return {
      stocksOne: [
        {
          title:'Carrera de Marketing Digital',
          like: 21,
          logoPais: 'https://www.flaticon.com/svg/vstatic/svg/555/555605.svg?token=exp=1620174336~hmac=f42e3ba7fb15a8c6f65eea95ef251027',
          pais: 'Peru',
          logoProduct:'https://globalpromoitems.com/tienda/peru/20832-thickbox_default/mochila-antirrobo-ranley.jpg'
        }
      ],
      stocks: [
        {
          title:'Lavadora/Secadora Eléctrica',
          like: 15,
          logoPais: 'https://www.flaticon.com/svg/vstatic/svg/555/555605.svg?token=exp=1620174336~hmac=f42e3ba7fb15a8c6f65eea95ef251027',
          pais: 'Peru',
          logoProduct:'https://www.milar.es/blog/wp-content/uploads/2021/01/Centrifugado-min.jpg'
        },
        {
          title:'STOCKHOLM TV bench, walnut veneer, 160x40x50',
          like: 30,
          logoPais: 'https://www.flaticon.com/svg/vstatic/svg/555/555605.svg?token=exp=1620174336~hmac=f42e3ba7fb15a8c6f65eea95ef251027',
          pais: 'Peru',
          logoProduct:'https://www.ikea.com/pt/en/images/products/stockholm-tv-bench-walnut-veneer__0851074_pe655467_s5.jpg?f=s'
        },
        {
          title:'Cama Moderna Tapizada Blanco Bremen',
          like: 21,
          logoPais: 'https://www.flaticon.com/svg/vstatic/svg/555/555605.svg?token=exp=1620174336~hmac=f42e3ba7fb15a8c6f65eea95ef251027',
          pais: 'Peru',
          logoProduct:'https://i.pinimg.com/originals/62/2a/be/622abe9ea6fcf673c547f02afa6874b1.jpg'
        },
      ]
    }
  }
}
</script>
