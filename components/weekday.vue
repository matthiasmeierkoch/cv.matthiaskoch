<template>
    <p class="weekday" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">Happy {{ weekday }} !</p>

</template>

<script>
    import sal from 'sal.js';

    const dayName = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
    let day = new Date().getDay();
    let weekdayName = dayName[day];

    export default {
        data() {
         return { weekday: weekdayName}
        },

        mounted() {
            this.$nextTick(() => sal());
        }
    }

</script>


<style>
.weekday{
    margin-top: 2rem;
}
</style>