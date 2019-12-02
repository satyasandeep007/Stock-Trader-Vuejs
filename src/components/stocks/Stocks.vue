<template>
    <div>
       <app-stock v-for="stock in stocks" :key="stock"></app-stock>
    </div>
</template>

<script>
import Stock from './Stock';

export default {

    components: {
        appStock : Stock,
    },
data() {
    return {
        stocks : [
            {id:1, name: 'Google', price:700},
            {id:2, name: 'Tata', price:600},
            {id:3, name: 'Infosys', price:500},
            {id:4, name: 'Wipro', price:400},
            {id:5, name: 'Facebook', price:300},
            {id:6, name: 'Instagram', price:200},
        ]
    }
},
}
</script>