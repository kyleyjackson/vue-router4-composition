<template>
    <div>
        <h1>Invoices</h1>
    </div>
</template>

<script>
import { onBeforeRouteLeave } from 'vue-router'
export default{
    setup(){
        onBeforeRouteLeave((to, from)=>{
            const answer = window.confirm(
                "Do you wish to leave Invoices? They are quite radical in my opinion"
            )
            if(!answer) return false
        })
    }
}
</script>