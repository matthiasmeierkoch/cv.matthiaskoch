<template>
<p>Happy {{weekdayName}}!</p>

</template>

<script>
    let arrayOfWeekdays = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];
    let dateObj = new Date();
    let weekdayNumber = dateObj.getDay();
    let weekdayName = arrayOfWeekdays[weekdayNumber];

    export default {
       async asyncData({$axios}) {
           let response = await $axios.get("weekdayName");
           let weekdayName = response.weekdayName;

            return {
                weekdayName
            }
        },
    }

</script>


<style>

</style>