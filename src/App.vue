<template>
  <div class="secBackground">
    <MainNav></MainNav>
    <MianHome></MianHome>
  </div>
  <BannerWhatsaap></BannerWhatsaap>
  <br>
  <ListImportProce></ListImportProce>
  <Presentacion></Presentacion>
  <Servicios></Servicios>
  <DeseasImportar></DeseasImportar>
  <StockMercancia></StockMercancia>
  <sumate></sumate>
  <br>
  <MainFooter></MainFooter>

  <router-view/>
</template>

<style lang="scss">
@import "components/style";
#app {
  //font-family: 'DM Sans', sans-serif;
}
body {
  font-family: 'DM Sans', sans-serif;
  margin: 0;
  padding: 0;
}
button, p {
  font-family: 'DM Sans', sans-serif;
}

.secBackground {
  background: #121212;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
<script>
import MianHome from "@/components/home/MianHome";
import MainNav from "@/components/nav/MainNav";
import BannerWhatsaap from "@/components/WhatsappBanner/bannerWhatsaap";
import ListImportProce from "@/components/list/ListImportProce";
import Presentacion from "@/components/infoExtra/Presentacion";
import DeseasImportar from "@/components/infoExtra/DeseasImportar";
import Servicios from "@/components/servicios/Servicios";
import StockMercancia from "@/components/stock/StockMercancia";
import Sumate from "@/components/infoExtra/Sumate";
import MainFooter from "@/components/footer/MainFooter";
export default {
  components: {
    MainFooter,
    Sumate,
    StockMercancia,
    Servicios, DeseasImportar, Presentacion, ListImportProce, BannerWhatsaap, MainNav, MianHome}
}
</script>
