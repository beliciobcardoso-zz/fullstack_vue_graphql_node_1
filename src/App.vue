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
							<span class="badge badge-info">{{prefixes.length}}</span>
						</h5>
						<div class="card">
							<div class="card-body">
								<ul class="list-group">
									<li class="list-group-item" v-for="prefixe in prefixes" v-bind:key="prefixe">{{prefixe}}</li>
								</ul>
								<br />
								<div class="input-group">
									<input class="form-control" type="text" placeholder="Digite o Prefixo" />
									<div class="input-group-append">
										<button class="btn btn-info">
											<span class="fa fa-plus"></span>
										</button>
									</div>
								</div>
							</div>
						</div>
					</div>
					<div class="col-md">
						<h5>
							Sufixos
							<span class="badge badge-info">{{ sufixes.length}}</span>
						</h5>
						<div class="card">
							<div class="card-body">
								<ul class="list-group">
									<li class="list-group-item" v-for="sufixe in sufixes" v-bind:key="sufixe">{{ sufixe}}</li>
								</ul>
								<br />
								<div class="input-group">
									<input class="form-control" type="text" placeholder="Digite o Sufixo" />
									<div class="input-group-append">
										<button class="btn btn-info">
											<span class="fa fa-plus"></span>
										</button>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
				<br />
				<h5>
					Dominios
					<span class="badge badge-info">{{ domains.length}}</span>
				</h5>
				<div class="card">
					<div class="card-body">
						<ul class="list-group">
							<li class="list-group-item" v-for="domain in domains" v-bind:key="domain">{{ domain }}</li>
						</ul>
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
	name: "app",
	data() {
		return {
			prefixes: ["air"],
			sufixes: ["bar"],
			domains: ["teste", "teste2", "teste3", "teste4"]
		};
	}
};
</script>

<style>
#slogan {
	margin-top: 30px;
	margin-bottom: 30px;
}

#main {
	background-color: #c2bbbb;
  padding:40px;
}

</style>
