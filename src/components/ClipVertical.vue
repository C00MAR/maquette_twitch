<template>
    <div>
        <p class="view_counter">1.2k vues</p>
        <h2>My bad là d'sus !</h2>
        <p class="account">AntoineDaniel</p>
    </div>
</template>

<style lang="scss" scoped>
div{
    height: 25vh;
    width: 40vw;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    padding: 10px 7px;
    background: var(--color-purple) url("");
    h2{
        font-size: 18px;
    }
    p.view_counter{
        width: fit-content;
        padding: 4px 6px;
        font-size: 15px;
        font-weight: 200;
        color: rgb(247, 247, 247); 
        background-color: rgba(0, 0, 0, 0.8);
        border-radius: 3px;
    }
    p.account{
        display: flex;
        font-size: 15px;
        font-weight: 200;
        color: rgb(175, 175, 175);
    }
    p.account::after{
        content: "";
        width: 15px;
        height: 15px;
        display: flex;
        flex-direction: row;
        background: url("../public/asset/icon/icon_verif.png") no-repeat 2px 5px; 
    }
}
</style>