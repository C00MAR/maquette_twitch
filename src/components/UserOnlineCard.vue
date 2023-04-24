<template>
    <div class="card_online_user">
        <div class="picture">
            <img :src="`asset/db_temp/${imgurl.imgsrc}.png`" alt="">
            <div class="redDot"></div>
        </div>
        <p>Ponce</p>
    </div>
</template>

<script>
export default {
    props: {
        imgurl: {
            type: String,
            default: "db_pp_temp-0"
        }
    }
}

</script>

<style lang="scss" scoped>
    .card_online_user{
        display: flex;
        position: relative;
        flex-direction: column;
        align-items: center;
        height: fit-content;
        .picture{
            margin-bottom: -10px;
            .redDot{
            width: 15px;
            height: 15px;
            background-color: red;
            border-radius: 50%;
            position: relative;
            top: -20px;
            right: -43px;
            border: 2px black solid;
        }
        }
        
        p{
            font-size: 12px;
            font-weight: 700;
            color: var(--color-white);
        }
    }
</style>