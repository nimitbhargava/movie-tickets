<template>
    <b-container class="bv-example-row">
        <b-row>
            <b-col>1 of 3</b-col>
            <b-col>2 of {{ this.count }} 3</b-col>
            <b-col>1 of 3</b-col>
        </b-row>
    </b-container>
</template>

<script>
import { mapState } from 'vuex';

export default {
    name: 'Main',
    props: {},
    computed: {
        ...mapState({
            count: state => state.count
        })
    }
}
</script>

<style scoped>

</style>