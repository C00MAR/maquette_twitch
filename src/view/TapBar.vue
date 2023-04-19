<script>
</script>

<template>
    <div class="tapbar_box">
        <div class="tapbar_category active">
            <img src="@/public/asset\icon\icon_like_active.png" alt="">
            <p>Suivis</p>
        </div>
        <div class="tapbar_category">
            <img src="@/public/asset\icon\icon_decouvrir.png" alt="">
            <p>Découvrir</p>
        </div>
        <div class="tapbar_category">
            <img src="@/public/asset\icon\icon_parcourir.png" alt="">
            <p>Parcourir</p>
        </div>
        <div class="tapbar_category">
            <img src="@/public/asset\icon\icon_loupe.png" alt="">
            <p>Rechercher</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .tapbar_box{
        border-top: 2px solid rgb(37, 37, 37);
        background-color: var(--color-black);
        position: sticky;
        bottom: 0;
        font-size: 17px;
        width: 100vw;
        height: 10vh;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-around;
        padding: 0 5vw;
        .tapbar_category{
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 5px;
            font-size: 12px;
            
            img{
                width: 32px;
                height: 32px;
            }
        }
    }
    
    .tapbar_box .active{
        color: var(--color-light-purple);
    }
</style>