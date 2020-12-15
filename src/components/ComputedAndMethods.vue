<template>
    <div>
        <section>
            <div class="col-md-10">
                <h1> Hello World  I am {{ text }} </h1>
            </div>
        </section>
        <section>
            <ul>
                <li>First Name : {{ firstName }}  </li>
                 <li>First Name : {{ lastName }}  </li>
            </ul>
        </section>
        <section>
            <div class="col-md-10 ">
                <div class='col-md-5 ' >
                    <label class='col-md-6'>
                        First Name
                    </label>
                    <div class='col-md-6 form-control text-center'>
                          <input type='text' v-model='firstName' placeholder="Enter First Name">  
                    </div>
                    <label class='col-md-6'>
                        Last Name
                    </label>
                    <div class='col-md-6 form-control text-center '>
                          <input type='text' v-model='lastName' placeholder="Enter Last Name">  
                    </div>
                </div>
                
            </div>
        </section>
    </div>
</template>

<script>
export default {
    
    data(){
        return{
            firstName:'',
            lastName:''
        }
    },
    computed:{
        text:function(){
            return this.firstName + " "+ this.lastName;
        }
    }

}
</script>

<style scoped>

</style>