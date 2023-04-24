<template>
    <div class="scroll_online_user">
        <OnlineCard v-for="imgsrc in srcList" :imgurl='{ imgsrc }'/>
    </div>
</template>

<script>
import OnlineCard from '../components/UserOnlineCard.vue'

export default {
    name: "OnlineUser",
    components: {
        OnlineCard
    },
    data () {
        return {
            srcList: ["db_pp_temp-0","db_pp_temp-1","db_pp_temp-2","db_pp_temp-3","db_pp_temp-4","db_pp_temp-5","db_pp_temp-6","db_pp_temp-7","db_pp_temp-8"]
        }
    }
}
</script>

<style lang="scss" scoped>
.scroll_online_user{
    width: 100vw;
    height: 13vh;
    display: flex;
    flex-direction: row;
    gap: 25px;
    padding: 0 5vw;
    overflow-x: scroll;
    overflow-y: hidden;
}

.scroll_online_user::-webkit-scrollbar {
    display: none;
}
</style>