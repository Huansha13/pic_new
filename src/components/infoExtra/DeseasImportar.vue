<template>
  <div class="wrapper">
    <div class="row">
      <div class="col-12 col-sm-12 col-md-6 col-lg-6">
        <h3><span>¿Deseas </span><span class="span2">Importar?</span></h3>
      </div>
      <div class="col-12 col-sm-12 col-md-6 col-lg-6">
        <a href=""> <img class="di-img" src="https://www.calculadoradefletes.com/assets/img/importar.png" alt=""></a>
      </div>
    </div>

  </div>
</template>

<style lang="scss">
@import "src/components/style";
.wrapper {
  padding: 32px;
  h3 {
    font-size: 70px;
    text-align: center;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0;
    color: #121212;
    .span2 {
      padding-bottom: 5px;
      margin-bottom: 5px;
      border-bottom: 5px solid $colorLight;
    }
  }
}
.di-img {
  border-radius: 5px;
  width: 100%;
}

.row {
  justify-content: space-evenly;
}

@media (max-width: 768px) {
  .di-img {
    width: 100%;
    margin-top: 30px;
  }
  .wrapper h3 {
    font-size: 35px;
  }
}

</style>
