<template>
    <div>
        <!-- 子组件 -->
        <span>{{name}}</span>
    </div>
</template>
<script>
export default {
    props:{
        name:String,
        required:true
    }
}
</script>

