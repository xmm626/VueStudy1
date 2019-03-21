<template>
	<div id="app">
		<div class="header">
			<router-link to="/" class="nav-item">
			<img src="./assets/logo.png"/>
			</router-link>
			<div class="ni">
				<router-link to="/task" class="nav-item">任务中心</router-link>
			<router-link to="/lib" class="nav-item">库管理</router-link>
			<router-link to="/ucenter" class="nav-item">许某</router-link>
			</div>
			
		</div>
		<div class=" container "><router-view></router-view></div>
	</div>
</template>

<script>
export default {
	name: 'App'
};
</script>

<style>
#app {
	background-color: rgb(244, 244, 244);
}
.header {
	display: flex;
	height: 100px;
	background-color: white;
	font-size: 20px;
	padding-left: 120px;
	align-items: center;
}

.nav-item {
	width: 100px;

	margin-right: 20px;
}
img{
	widows: 100px;
	height: 40px;
	margin-right: 100px;
}

.ni{
	margin-left: 45%;
}
.container {
	width: 80%;
	margin: 0 auto;
	padding-bottom: 20px;
}
a {
	text-decoration: none;
	color: #aaa;
}
a:hover {
	color: rgb(2,165,218);
}
</style>
