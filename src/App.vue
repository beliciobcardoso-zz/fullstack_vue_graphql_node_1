<template>
  <div>
    <div id="slogan" class="text-center">
      <h1>Pagina Principal</h1>
      <br />
      <h6 class="text-secondary">Gerador de nomes ultilizando Vue.Js, GraphQl e Node</h6>
    </div>
    <div id="main">
      <div class="container">
        <div class="row">
          <div class="col-md">
            <h5>
              Prefixos
              <span class="badge badge-info">0</span>
            </h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item"></li>
                </ul>
                <br />
                <input class="form-control" type="text" placeholder="Digite o Sufixo" />
              </div>
            </div>
          </div>
          <div class="col-md">
            <h5>
              Sufixos
              <span class="badge badge-info">0</span>
            </h5>
            <div class="card">
              <div class="card-body">
                <ul class="list-group">
                  <li class="list-group-item"></li>
                </ul>
                <br />
                <input class="form-control" type="text" placeholder="Digite o Sufixo" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "font-awesome/css/font-awesome.css";

export default {
  name: "app"
};
</script>

<style>
#slogan {
  margin-top: 30px;
  margin-bottom: 30px;
}

#main {
  background-color: #c2bbbb;
  padding-top: 30px;
  padding-bottom: 30px;
}
</style>
