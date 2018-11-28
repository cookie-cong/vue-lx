<template>
    <div>
        <!-- 子组件 -->
        <span>{{valueNmae}}</span>
        <button @click="childClick">点击触发</button>
    </div>
</template>
<script>
export default{
    data(){
        return{
            valueNmae:"我是子组件传的值"
        }
    },
    methods:{
        childClick(){
            this.$emit("child",this.valueNmae)
        }
    }
}
</script>
