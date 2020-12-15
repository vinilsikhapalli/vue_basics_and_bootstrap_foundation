<template>
<div>
    <h2 v-text="message"></h2>
    <h3>{{message}}</h3><br/>
    <p v-html="link"></p>
    <p v-show="checkValueOne"> I am There Here ( v - show )</p>

    <p v-if="checkValTwo"> I am If condition ( v - if ) </p>
    <p v-else-if="checkValueOne"> ha ha ha ( v - else if ) </p>
    <p v-else> Finally ( v - else )</p>
        <p>{{test}}</p>
    <p v-pre>{{ something wan a show u in flower braces }}</p>
    <h1 v-cloak><strong> I am cloak  </strong></h1>
    <b-icon-volume-mute>list items</b-icon-volume-mute>
    <ul>
        <li v-for="v in listVal" :key="v.id"> 
            {{v.data}}
        </li>
    </ul>
    <div class="text-center">
    <input type="text" v-model="TwoWayBind" placeholder=" for two way binding">
    <p id="twoWay">{{TwoWayBind}}</p>
    </div>
    </div>
</template>

<script>
export default {

data(){
    return{
        message:'I am The One',
        link:'Hai..... <a target="block" href="www.vue.org">click here</a>',
        checkValueOne:true,
        checkValTwo:true,
        test:' THIS IS FOR  one time rendaring the content  ( v-once ) ',
        listVal:[
            {id:1,data:'Item one'},
            {id:2,data:'Item two'},
            {id:3,data:'Item three'},
            {id:4,data:'Item four'},
            {id:5,data:'Item five'},
            {id:6,data:'Item six'},
            {id:7,data:'Item seven'}
        ],
        TwoWayBind:''
    }
}

}
</script>

<style scoped>

[v-cloak]{
    background-color: red;
}

li{
    list-style-type: none;
}

#twoWay{
    background-color:red;
}
</style>