<template>
<div>
<table v-if="isvisible">
<tr>
<th>name</th>
<th>age></th>
<th>course</th>
</tr>
<tr v-for="event in person">
<td>{{event.name}}</td>
<td>{{event.age}}</td>
<td>{{event.course}}</td>
</tr>
</table>
<button @click:"tap">submit</button>
<input type="text" v-on:model="modall">
<p :style="{color:'red'}">chandan</p>
<p 
<p>{{modal}}</p>
</div>
</template>
<script>
export default{
	data(){
	return{
   person:[{name:"chandan",age:"23",course:software},
   {name:"ram",age:"23",course:BCA},
   {name:"ravana",age:"23",course:B.COM}],
   isvisible:true,
   modall:"sai"
	}
	},
	methods:{
	tap:function(){
    this.isvisible=!this.isvisible
	}
	}
}
</script>