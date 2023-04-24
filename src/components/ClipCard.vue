<template>
    <div class="card_clip">
        <div class="preview_box">
            <div class="mute_statue">
                <img src="@/public/asset\icon/preview_card_sound_icon.png" alt="" class="sound_icon">
            </div>
            <div class="total_view">
                <div class="red_dot"></div>
                <p class="number_view">5.2k</p>
            </div>
        </div>
        <div class="detail_box">
            <img src="@/public/asset/db_temp/db_pp_temp-0.png" alt="">
            <div>
                <h1>Qui sera le Maître Des Fleurs ?</h1>
                <p class="account">Ponce</p>
                <p>Maître Des Fleurs</p>
                <div>
                    <p class="tag">Français</p>
                    <p class="tag">Quiz</p>
                    <p class="tag">Ponce</p>
                    <p class="tag">Fleur</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card_clip{
    width: 100vw;
    height: 35vh;
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 0 2vw;
    .preview_box{
        width: 100%;
        height: 60%;
        background-color: var(--color-purple);
        border-radius: 10px;
        position: relative;
        .mute_statue{
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: flex-end;
            align-items: flex-start;
            .sound_icon{
                background-color: rgba(0, 0, 0, 0.8);
                padding: 3px 3px;
                border-radius: 5px;
                width: 37px;
                height: 37px;
                margin: 10px;
            }
        }
        .total_view{
            position: absolute;
            bottom: 10px;
            left: 15px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
            background-color: rgba(0, 0, 0, 0.8);
            border-radius: 5px;
            padding: 0px 5px;
            .red_dot{
                width: 15px;
                height: 15px;
                background-color: red;
                border-radius: 50%;
                border: 2px black solid;
            }
            .number_view{
                font-size: 12px;
                font-weight: 700;
                color: var(--color-white);
                margin: 10px;
            }
        }
    }
    .detail_box{
        width: 100%;
        height: 10vh;
        border-radius: 10px;
        display: flex;
        gap: 10px;
        flex-direction: row;
        img{
            width: 7vh;
            height: 7vh;
            border-radius: 10px;
        }
        div{
            display: flex;
            flex-direction: column;
            gap: 5px;
            h1{
                font-size: 21px;
                font-weight: 700;
                color: var(--color-light-grey);
            }
            p{
                font-size: 15px;
                font-weight: 200;
                color: rgb(175, 175, 175);
            }
            p.account{
                display: flex;
            }
            p.account::after{
                    content: "";
                    width: 15px;
                    height: 15px;
                    display: flex;
                    flex-direction: row;
                    background: url("../public/asset/icon/icon_verif.png") no-repeat 2px 5px; 
                }
            div{
                display: flex;
                flex-direction: row;
                gap: 5px;
                p.tag{
                    font-size: 14px;
                    font-weight: 500;
                    font-family: 'Roobert', sans-serif;
                    color: var(--color-purple);
                    background-color: rgba(255, 255, 255, 0.2);
                    width: fit-content;
                    padding: 3px 1vh;
                    border-radius: 15px;
                    font-weight: 700;
                    }
            }
        }
    }
}
</style>