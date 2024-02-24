<template>
    <button class="button">
        <span class="button__name">{{ name }}</span>
    </button>
</template>
  
<script>

// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
    name: 'ButtonCard',
    components: {
        //HelloWorld
    },
    props: {
        name: {
            type: String,
            default: "Купить"
        }
    },
    setup() {

    }
}
</script>
<style lang="scss" scoped>
.button {
    display: inline-flex;
    padding: 6px 38px;
    justify-content: center;
    align-items: center;
    gap: 10px;
    border-radius: 7px;
    background: #3278FF;

    //     width: Hug (141px)
    // height: Hug (34px)
    // top: 20px
    // left: 37px
    // padding: 6px, 38px, 6px, 38px
    // border-radius: 7px
    // gap: 10px
    width: 65px;
    height: 22px
}

.button__name {
    color: #FFF;
    text-align: center;
    // font-feature-settings: 'calt' off;
    /* Btn */
    font-family: Roboto;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: 22px;
    /* 110% */
    // letter-spacing: -0.4px;
}
</style>