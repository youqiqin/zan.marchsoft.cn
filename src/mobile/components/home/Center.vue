<template>
    <div>
        <mt-header fixed title="个人中心"></mt-header>
        <div id="test">
            <div class="bg_user">
                <div class="user_picture"></div>
                <div>
                    <p>{{name}}</p>
                    <p>{{number}}</p>
                </div>
            </div>
        </div>
        <NavBottom selected="4"></NavBottom>
    </div>
</template>

<script>
import NavBottom from '../NavBottom.vue'
export default {
    components:{
        NavBottom
    },
    data () {
        return {
            a:1,
            name:'桑金超',
            number:'2016010226'
        }
    },
    methods:{
        
    },
    beforeCreate(){
        console.log(this.a)
        console.log('beforeCreate')
    },
    created(){
        console.log('created')
        console.log(this.a)
    },
    mounted(){
        // axios.get('baidu.com').then(function (response) {
        //     console.log(response.data);
        // }).catch(function (error) {
        //     console.log(error);
        // });
        
    }
}
</script>
<style>
    html,body{
        margin: 0;
        padding: 0;
    }
</style>
<style scoped>
    #test{
        /*background: yellow!important;*/
    }
    .bg_user{
        margin:12% 0 0 0;
        background: url(../../assets/img/bg_user.jpg) no-repeat center center;
        background-size: 100% 100%;
    }
</style>

