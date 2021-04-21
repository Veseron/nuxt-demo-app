<template>
    <div class="container">
        <MyItem
            v-for="rental in myRental"
            :key="rental.id"
            :item="rental"
        />
    </div>
</template>

<script>
import { mapState } from 'vuex';
export default {
    layout: 'no-nav',
    computed: {
        ...mapState([
            'myRental'
        ])
    }
}
</script>

<style scoped>

</style>