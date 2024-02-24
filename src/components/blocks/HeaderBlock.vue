<template>
    <div class="Navigation">
        <div>
            <img src="@/assets/images/Logo.png" alt="">
        </div>
        <div class="telefon">+7 987 654 32-10</div>


    </div>
</template>
  
<script>
// @ is an alias to /src
// import logoIcon from '@/components/icons/logoIcon.vue'

export default {
    name: 'HeaderPage',
    components: {
        // logoIcon
    },
    props: {

    },
    setup() {

    }
}
</script>
<style lang="scss" scoped>
.Navigation {
    display: flex;
    height: 60px;
    padding: 13px 70px;
    justify-content: space-between;
    align-items: center;
    gap: 10%; //1485px;
    background-color: #3278FF;
    margin-bottom: 235px;
}

.telefon {
    color: #fff;
    font-family: Roboto;
    font-size: 22px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
</style>
  