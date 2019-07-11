<template>
<div>
<h1>{{title}}</h1>
<h2>Hi All</h2>
<button @click="reversemessage">Click</button>
</div>
</template>
<script>
export default{
	data(){
	return{
	name:"sai chandan",
	title:"vuejs project"
	}
	},
	methods:{
	reversemessage:function(){
	console.log(this.name=this.name.split('').reverse().join(''))
	}
	}
}
</script>
