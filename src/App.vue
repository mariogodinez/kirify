<template>
  <div id="app" class="relative">
	<HeaderComponent></HeaderComponent>
	<nav class="" style="position: absolute; right: 300px; bottom:130px; z-index:1000000;">
		<ul class="color-gray">
			<li class="">
				<router-link to="/login">programando kirify . . .</router-link>
			</li>
		</ul>
	</nav>
     <router-view></router-view>
     <div class="square40 rounded back-pinkred font20 flex flex-middle flex-center" style="border:2px solid white;position: fixed; bottom:10vh; right:3vw; z-index:10">
		<span class="fa fa-cart-plus color-white" style="margin-right:1px"></span>
		<span class="flex color-white flex-center rounded flex-middle" style="position:absolute; top:-1px; left:-7px; font-size:12px; background:#222; width:18px;height:18px;">3</span>
	</div>
     <MenuFooter></MenuFooter>
  </div>
</template>

<script>
	import HeaderComponent from './components/HeaderComponent.vue'
	import MenuFooter from './components/MenuFooter.vue'


	export default {
	  name: 'app',
	  components: {
	    HeaderComponent,
	    MenuFooter
	  }
	}
</script>
