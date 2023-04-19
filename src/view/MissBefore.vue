<template>
    <div class="miss">
        <h2>Ce que tu as <span>manqué</span> hier...</h2>
        <div class="clip_scroll">
            <VerticalCard />
            <VerticalCard />
            <VerticalCard />
            <VerticalCard />
        </div>
    </div>
</template>

<script>
import VerticalCard from '../components/ClipVertical.vue'

export default {
    name: "MissBefore",
    components: {
        VerticalCard
    }
}
</script>

<style lang="scss" scoped>
.miss{
    h2{
        font-size: 1.5rem;
        font-weight: 600;
        margin: 0px 0 10px 0;
        padding: 1vh 3vw 0;
        span{
            color: var(--color-light-purple);
        }
    }
    .clip_scroll{
        display: flex;
        flex-direction: row;
        overflow-x: scroll;
        gap: 4vw;
        padding: 0 3vw;
        &::-webkit-scrollbar{
            display: none;
        }
    }
}
</style>