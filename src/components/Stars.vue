<template>
<div class="rating">
	<ul class="list">
		<li v-for="star in maxStars" class="star" v-bind:class="{'active':star <= stars}" >
			<icon v-bind:name="star <= stars ? 'star' : 'star-half'"></icon>
		</li>
	</ul>
</div>
</template>
<script>
import 'vue-awesome/icons/star'
import 'vue-awesome/icons/star-half'
import Icon from 'vue-awesome/components/Icon'
export default {
	components:{ Icon },
	data(){
		return {
			stars : 3,
			maxStars : 5
		}
	}
}
</script>
<style>
.rating{

}
.list{

}
.star{
	
}

</style>