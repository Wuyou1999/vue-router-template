<template>
	<div>
		<div class="container">
			<div class="side-bar">
				<router-link to="/lib_fz">库分组</router-link>
			</div>
			<div class="kong"></div>
			<div class="content">
				<router-link to="/lib_tk">题库</router-link>
				<router-link to="/lib_zyk">资源库</router-link>
				<router-link to="/lib_hdk">活动库</router-link>
				<router-view/>
           </div>
			
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Lib',
		data() {
			return {

			};
		}
	};
</script>

<style>
	.container {
		display: flex;
		width: 90%;
		margin: 0 auto;

	}

	.side-bar {
		flex: 1 1 20%;
		display: flex;
		flex-direction: column;
		background-color: #fff;
		margin-top: 20px;
	}

	a {
		margin-bottom: 30px;
	}

	.kong {
		flex: 1 1 2%;
		display: flex;
		flex-direction: column;
		background-color: #AAAAAA;
	}

	.content {
		flex: 1 1 78%;
		text-align: left;
		background-color: #fff;
		margin-left: 150px;
		padding-bottom: 20px;
	}
</style>
