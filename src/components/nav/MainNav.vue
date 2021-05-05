<template>
  <nav class="d-flex-align">
    <div class="logo">
     <span class="pic-logo">PIC</span>
      <span class="pic-slider">Tu experto en logistica</span>
    </div>
    <div class="login">
      <button class="btn web" type="submit"> Iniciar sesión </button>
      <button class="movil" type="submit"> <i class="uil uil-user"></i> </button>
    </div>
  </nav>
</template>

<style lang="scss">
@import "src/components/style";
.movil {
  display: none;
}
nav {
  justify-content: space-between;
  padding: 32px;
}
.logo {
  display: grid;
  .pic-logo {
    font-size: 25px;
    color: white;
    font-weight: 700;
    letter-spacing: 5px;
  }
  .pic-slider {
    color: white;
    text-transform: uppercase;
    font-size: 12px;
    letter-spacing: 2px;
  }
}
.btn {
  background: $colorLight;
  border: none;
  outline: none;
  padding: 14px 22px;
  font-size: 16px;
  font-weight: 700;
  color: #121212;
  transition: all .5s;
  cursor: pointer;
  &:hover {
    background: $colorDrak;
  }
}

@media (max-width: 768px) {
  .web {
    display: none;
  }
  .movil {
    display: inline-flex;
    background:  transparent;
    border: none;
    outline: none;
    i {
      color: $colorLight;
      font-size: 30px;
    }
  }
}

</style>
