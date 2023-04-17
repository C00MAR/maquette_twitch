<template>
    <div class="profil_box">
        <div class="profil_icon">
            <img src="@/public/asset\icon\account_avatar.png" alt="" class="pp">
            <img src="@/public/asset\icon\icon_coment.png" alt="" class="icon">
            <img src="@/public/asset\icon\icon_inbox.png" alt="" class="icon">
            <img src="@/public/asset\icon\icon_cast.png" alt="" class="icon">
        </div>
        <div class="profil_create">
            <button class="secondary">
                <img src="@/public/asset\icon\icon_diffusion.png" alt="">
                Créer
            </button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.profil_box{
    width: 100vw;
    height: 15vh;
    position: absolute;
    top: 0;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 0 5vw;
    align-items: center;
    .profil_icon{
        display: flex;
        gap: 10px;
        align-items: center;
        .pp{
            width: 40px;
            height: 40px;
        }
        .icon{
            width: 32px;
            height: 32px;
        }

    }
    .profil_create{
        .secondary{
            border-radius: 50px;
            display: flex;
            align-items: center;
            gap: 5px;
            img{
                width: 32px;
                height: 32px;
            }
        }
    }
}
</style>