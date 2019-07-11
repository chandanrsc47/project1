<template>
<div>
<table v-if="isvisible">
<tr>
<th>name</th>
</tr>
<tr v-for="items in person">
<td>{{item.name}}</td>
<td>{{item.color}}</td>
</tr>
</table>
<button @click="pqr">submit</button>
<button @click="increase">submit</button>
<p>{{counter}}</p>
<p>{{ageinc()}}</p>
</div>
<template>
<script>
export default{
	data(){
	return{
	person:[{name:"dhoni",color:"yellow"},
	{name:"sachin",color:"blue"}],
	isvisible:true,
    created(){
    this.hello()
    },
    counter:0,
    age:20
    }
	}
	},
	methods:{
	abc:function(){
	this.isvisisble=!this.isvisibe
	},
	hello:function(){
	alert("this is a vuejs a page")
	},
	increase:function(){
	this.counter++;
	},
	ageinc:function(){
	return this.age+this.counter
	}
}
}