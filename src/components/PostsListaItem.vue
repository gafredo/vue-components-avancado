<template>
	<div class="post">
		<slot>
			<div class="post-cabecalho">
				<h2>{{ post.titulo }}</h2>
			</div>
			<div class="post-conteudo">
				<!-- sem a propriedade name ele fica sendo default 
      <slot></slot>
      -->
				<p>{{ post.conteudo }}</p>
			</div>
			<div class="post-rodape">
				<small> {{ post.autor }}</small>
				<a href="#" class="link">Ler mais...</a>
			</div>
		</slot>
	</div>
</template>

<script>
export default {
	props: {
		post: {
			type: Object,
			required: true
		}
	}
};
</script>

<style scoped>
.post {
	margin: 15px auto;
}
.post-cabecalho {
	padding: 5px 12px;
	background-color: #eee;
}
.post-conteudo {
	font-size: 16px;
}
.post-rodape {
	font-style: italic;
}
.link {
	float: right;
	text-decoration: none;
	color: blue;
}
.post-paragrafo {
	color: green;
}
</style>
