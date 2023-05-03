<script setup lang="ts">
//endpoint de la pagina
const props = defineProps<{
  ENDPOINT_API: string;
}>();
const ENDPOINT = props.ENDPOINT_API;
</script>

<template>
  <div class="page-bg"><!-- No colocar contenido --></div>
  <div id="body-pd" class="container-fluid">
      <!-- cuestionario autoconocimiento 1-->
      <div class="row">
        <form @submit.prevent="">
          <div class="col-xl-12 col-sm-12 col-12 mb-3 mt-4">
            <div class="card shadow-sm border-0">
              <div class="card-content">
                <!-- card body -->
                <div class="card-body">
                  <h5 id="titulo2" class="card-title">Test de Autoconocimiento</h5>
                  <p id="intrucciones2" class="card-text">
                    Marque si o no a todos los adjetivos que describan tu
                    personalidad.Trate de definirse tal como es, no como le
                    gustaría ser.
                  </p>
                </div>
                <!-- cuestionario -->
                <!-- pregunta 1 -->

                <div class="card-body">
                  <div class="media-body text-left col mr1 shadow-sm p-1 rounded">
                    <div id="juntadotodo2">
                      <h6 id="pregunta2">
                        1 .- ¿Aceptarías trabajar escribiendo artículos en la
                        sección económica de un diario?
                      </h6>
                      <div id="juntado2" style="text-indent: 10px">
                        <input id="circulo2" type="radio" /><label id="opciones2">
                          Si</label
                        >
                      </div>
                      <div id="juntado2" style="text-indent: 10px">
                        <input id="circulo2" type="radio" /><label id="opciones2">
                          ¿?</label
                        >
                      </div>
                      <div id="juntado2" style="text-indent: 10px">
                        <input id="circulo2" type="radio" /><label id="opciones2"
                          >No</label
                        >
                      </div>
                    </div>
                  </div>
                </div>

                <!-- <script>for (i=1 ; i<=10 ; i++){
                  document.write("<div class='mt-4'>");
                }  </script> -->

                <!-- ----------------- -->
              </div>
            </div>
          </div>
          <div class="centrado"><input
              id="resolver2"
              type="submit"
              class="lform-submit"
              value="Resolver"
            /></div>
          
        </form>
      </div>
    </div>
</template>
<style>
.centrado {
  display: flex;
  justify-content: center;
  align-items: center;
}
@media screen and (max-width: 768px) {
        #body-pd {
          padding: 2% 4% 10% 4%;
        }

        #titulo2 {
          text-align: center;
          font-weight: bold;
          font-size: 23px;
          color: rgb(43, 150, 87);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #intrucciones2 {
          text-align: justify;
          padding: 2% 1% 0% 1%;
          font-size: 15px;
          color: rgb(107, 107, 107);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #pregunta2 {
          font-size: 15px;
          color: rgb(65, 65, 65);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #juntadotodo2 {
          background-color: rgb(236, 236, 236);
          /* top: 0;
	left: 0;
	right: 0;
	bottom: 0; */
          /* width: 100%; */
          /* display: block; */
          border-radius: 20px;
          justify-content: center;
          align-items: center;
          padding: 25px;
          /* text-align: center; */
        }
        #juntado2 {
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
          font-size: 15px;
          /* height: 135%; */
          width: 95%;
          font-weight: bold;
          padding: 1% 0% 1% 1.5%;
          border-radius: 15px;
          margin: 1% 0% 1% 3%;
          border: rgb(70, 192, 121) solid 1px;
        }

        #juntado2:hover {
          width: 95%;
          background-color: rgb(43, 150, 87);
          border: rgb(70, 192, 121) solid 1px;
          color: white;
        }
        #circulo2 {
          background-color: #ce2c2c;
          width: 1.5em;
          height: 1.5em;
          border-radius: 100%;
          border: #ce2c2c solid 1.125em;
          margin-right: 0.375em;
          transition: 0.25s ease;
          /* box-shadow: inset 0 0 0 0.125em #00005c; */
        }
        #opciones2 {
          padding-top: 10px;
        }
        #resolver2 {
          font-size: 20px;
          background-color: rgb(43, 150, 87);
          border: rgb(43, 150, 87) solid 1px;
          color: white;
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
          font-weight: bold;
          padding: 0.5% 4% 0.5% 4%;
          border-radius: 15px;
          align-items: center;
        }
      }
      @media screen and (min-width: 769px) {
        #body-pd {
          padding: 2% 12% 10% 12%;
        }

        #titulo2 {
          font-size: 20px;
          color: rgb(43, 150, 87);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #intrucciones2 {
          text-align: justify;
          padding: 2% 10% 0% 10%;
          font-size: 15px;
          color: rgb(107, 107, 107);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #pregunta2 {
          font-size: 15px;
          color: rgb(65, 65, 65);
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        }
        #juntadotodo2 {
          background-color: rgb(245, 245, 245);
          /* top: 0;
	left: 0;
	right: 0;
	bottom: 0; */
          /* width: 100%; */
          /* display: block; */
          border-radius: 20px;
          justify-content: center;
          align-items: center;
          padding: 25px;
          /* text-align: center; */
        }
        #juntado2 {
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
          font-size: 15px;
          /* height: 135%; */
          width: 20%;
          font-weight: bold;
          padding: 1% 0% 1% 1.5%;
          border-radius: 15px;
          margin: 1% 0% 1% 3%;
          border: rgb(70, 192, 121) solid 1px;
        }

        #juntado2:hover {
          width: 20%;
          background-color: rgb(43, 150, 87);
          border: rgb(70, 192, 121) solid 1px;
          color: white;
        }
        #circulo2 {
          background-color: #ce2c2c;
          width: 1.5em;
          height: 1.5em;
          border-radius: 100%;
          border: #ce2c2c solid 1.125em;
          margin-right: 0.375em;
          transition: 0.25s ease;
          /* box-shadow: inset 0 0 0 0.125em #00005c; */
        }
        #opciones2 {
          padding-top: 10px;
        }
        #resolver2 {
          font-size: 22px;
          background-color: rgb(43, 150, 87);
          border: rgb(43, 150, 87) solid 1px;
          color: white;
          font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
          font-weight: bold;
          padding: 0.5% 2% 0.5% 2%;
          border-radius: 15px;
          align-items: center;
        }
      }
</style>
