<template>
  <div class="container d-flex mr-6">
    <div class="region my-auto mr-2">
        <p class="city">leeds</p>
        <p class="time">00:32</p>
    </div>
    <div class="suntimes my-auto">
       <p class="sunrise"><i class="wi wi-sunrise"></i>05:08</p>
       <p class="sunrise"><i class="wi wi-sunset"></i>21:18</p>
    </div>
    <div class="forecast d-flex">
        <div class="forecast--icon t0 d-flex flex-column align-center">
            <p class="forecast--time">00:00</p>
            <i class="icon wi wi-day-sunny"></i>
            <p class="temperature">temp</p>
        </div>
        <div class="forecast--icon t1 d-flex flex-column align-center">
            <p class="forecast--time">01:00</p>
            <i class="icon wi wi-day-cloudy"></i>
            <p class="temperature">temp</p>
        </div>
        <div class="forecast--icon t2 d-flex flex-column align-center">
            <p class="forecast--time">02:00</p>
            <i class="icon wi wi-day-rain"></i>
            <p class="temperature">temp</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .region {
        text-align: center;
        .city {
            font-weight: bold;
            font-size: 1.5rem;
            text-transform: uppercase;
            margin-top: -0.3rem;
        }
        .time {
            margin-top: -0.7rem;
        }
    }

    .suntimes {
        font-size: 0.9rem;
    }

    .forecast {
        gap: 1rem;
        .forecast--icon {
            .icon {
                margin: 0.3rem 0 0.1rem 0;
                font-weight: 100;
                font-size: 1.75rem;
            }
        }

        .temperature {
            font-size: 0.8rem;
        }

        .temperature::after {
            position: relative;
            content: '\00B0'+ 'C';
        }
    }

    .forecast::before {
        position: relative;
        content: '';
        background-color: black;
        width: 1px;
        height: 90%;
        top: 10%;
        left: 0.5rem;
    }
</style>