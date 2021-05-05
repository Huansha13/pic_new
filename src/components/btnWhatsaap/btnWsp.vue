<template>
  <div class="sectionBtnWsp">
    <input type="checkbox" id="wsp" style="display: none">
    <div class="wspPaises">
      <ul>
        <li><a href=""><span class="namePais">Venezuela</span> &nbsp; <img src="https://www.calculadoradefletes.com/assets/img/flags/venezuelaRound.svg" alt=""> </a></li>
        <li><a href=""><span class="namePais">Peru</span> &nbsp; <img src="https://www.calculadoradefletes.com/assets/img/flags/peruRound.svg" alt=""></a></li>
        <li><a href=""><span class="namePais">Panamá</span> &nbsp; <img src="https://www.calculadoradefletes.com/assets/img/flags/panamaRound.svg" alt=""></a></li>
      </ul>
    </div>
    <div class="sect-btn">
      <label for="wsp">
        <div class="btnWsp">
          <div class="icon">
            <i class="uil uil-whatsapp"></i>
          </div>
          <div class="txtBtnWsp">
            ¿Preguntas? !Escribenos!
          </div>
        </div>
      </label>
    </div>
  </div>


</template>

<style lang="scss">
.sectionBtnWsp {
  position: fixed;
  right: 0;
  bottom: 0;
  padding: 30px 30px;
  z-index: 1;
}
.btnWsp {
  background: #25d366;
  box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.25);
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  padding: 11px 22px;
}
.icon {
  display: flex;
  align-items: center;
  i {
    font-size: 35px;
    color: white !important;
  }
}

.wspPaises {
  display: none;
}
#wsp:checked + .wspPaises {
  display: flex !important;
  flex-direction: column;
}
.wspPaises {

  ul {
    list-style: none;
    margin: 0;
    padding-right: 10px;
    li {
      margin-bottom: 15px;
      display: flex;
      justify-content: flex-end;
    }
    li a {
      display: flex;
      align-items: center;
      color: #0c1924;
      text-decoration: none;
      img {
        width: 40px;
      }
    }
  }
}
.sect-btn {
  display: flex;
  justify-content: flex-end;
}
.namePais {
  background: #FFFFFF;
  box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.25);
  border-radius: 5px;
  padding: 7px 20px;
  margin-right: 10px;
  color: #121212;
  font-weight: 500;

}
.txtBtnWsp {
  color: #FFFFFF;
  font-size: 16px;
  font-weight: 500;
}

@media (max-width: 768px) {
  .sectionBtnWsp {
    padding: 30px 30px !important;
  }
  .sectionBtnWsp {
    display: none;
  }
}

</style>
