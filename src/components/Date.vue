<template>
    <div class="container">
        <div class="current ml-6 d-flex align-center">
            <span class="date mr-2">23</span><span class="month ml-2">July</span>
        </div>
        <div class="current-display d-flex justify-center align-center">
             <v-btn class="today-btn mx-2">Today</v-btn>
            <v-btn icon="mdi-chevron-left" size="x-small"></v-btn>
            <span class="current-text px-2">July</span>
            <v-btn icon="mdi-chevron-right" size="x-small"></v-btn>
           <v-btn class="ml-2" icon="mdi-refresh" size="x-small"></v-btn>
        </div>
    </div>
  
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .current {
        font-size: 1.75rem;
        .date {
            font-weight: bold;
            font-size: 2.25rem;
        }
    }

    .current::before {
        content: '';
        position: relative;
        background-color: black;
        height: 43px;
        left: 3.1rem;
        width: 2px;
    }

</style>