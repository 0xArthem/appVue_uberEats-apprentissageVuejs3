<template>

<div class="restaurant--card">
    <div class="restaurant--image">

    </div>

    <div class="restaurant--information">
        <div class="top">
            <p class="name">
                {{ info_restaurant.name }}
            </p>
            <p class="evaluation">
                <span>{{ info_restaurant.note }}</span>
            </p>
        </div>
        <p class="time">
            {{ info_restaurant.drive_time}}
        </p>
    </div>
</div>
  
</template>

<script>
export default {
    name: 'RestaurantCard',
    props: {
        info_restaurant: Object
    }

}
</script>

<style lang="scss">
.restaurant--card{
    width: 32%;
    height:30vh;
    .restaurant--image{
        background-image: url('https://cn-geo1.uber.com/image-proc/resize/eats/format=webp/width=550/height=440/quality=70/srcb64=aHR0cHM6Ly9kMXJhbHNvZ25qbmczNy5jbG91ZGZyb250Lm5ldC8zNzg4MDJiMC1jNTI4LTQ4MjktYjBiNS0wY2M2NDBkZjYzY2QuanBlZw==');
        height:70%;
        background-size:cover;
        background-position: center;
    }
    .restaurant--information{
        color:black;
        .top{
            margin: 10px 0px;
            display:flex;
            align-items:center;
            justify-content: space-between;
            .evaluation{
                background-color: #eeeeee;
                display:flex;
                justify-content:center;
                align-items:center;
                height:30px;
                width:30px;
                font-size:0.9rem;
                border-radius: 50%;
            }
        }
        .time{
            font-size:0.9rem;
        }
    }
}
</style>