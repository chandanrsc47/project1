<template>
<div>
<p>{{name}}</p>
<button @click="reversemessage">Click</button>
</div>
</template>
<script>
export default{
	data(){
	return{
	name:"sai chandan"
	}
	},
	methods:{
	reversemessage:function(){
	console.log(this.name=this.name.split('').reverse().join(''))
	}
	}
}
</script>
