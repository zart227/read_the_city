<template>
    <div class="info">
        <h2 class="title">
            {{ title }}
        </h2>
        <p class="description">
            {{ description }}
        </p>
    </div>
</template>

<script>
// import { ref } from 'vue'

export default {
    name: 'CardInfo',
    components: {
    },
    props: {
        title: {
            type: String,
            default: "Name"
        },
        description: {
            type: String,
            default: "Name"
        }
    },
    setup() {
    }
}
</script>

<style lang="scss" scoped>
.title {
    color: #000;
    text-align: center;
    font-family: Roboto;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.description {
    color: #000;
    text-align: center;
    font-family: Roboto;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.info {
    width: 268px;
}
</style>
