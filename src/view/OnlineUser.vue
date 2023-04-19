<template>
    <div class="scroll_online_user">
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
        <OnlineCard />
    </div>
</template>

<script>
import OnlineCard from '../components/UserOnlineCard.vue'

export default {
    name: "OnlineUser",
    components: {
        OnlineCard
    }
}
</script>

<style lang="scss" scoped>
.scroll_online_user{
    width: 100vw;
    height: 10vh;
    display: flex;
    flex-direction: row;
    gap: 25px;
    padding: 0 5vw;
    overflow-x: scroll;
}

.scroll_online_user::-webkit-scrollbar {
    display: none;
}
</style>