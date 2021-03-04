<template>
	<!--
  <div id="app" class="container">
    <h1>Vue JS</h1>
    <PostsLista :posts="posts" />
  </div>
  -->

	<div>
		<Neve v-if="isSnowing" />
		<Folhas v-else />
	</div>
</template>

<script>
import Neve from './components/Neve';
import Folhas from './components/Folhas';

export default {
	components: { Neve, Folhas },
	data() {
		return {
			isSnowing: true,
			posts: [
				{
					id: 1,
					titulo: 'Components Vue',
					conteudo: 'Conteudo id 1',
					autor: 'Gabriel'
				},
				{
					id: 2,
					titulo: 'Components Vue',
					conteudo: 'Conteudo id 2',
					autor: 'Gabriel Fredo'
				},
				{
					id: 3,
					titulo: 'Components Vue',
					conteudo: 'Conteudo id 3',
					autor: 'Mr'
				}
			]
		};
	}
};
</script>

<style>
.container {
	width: 960px;
	margin: auto;
}
body {
	margin: 0;
}
</style>
