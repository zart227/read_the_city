<template>
    <main class="main">
        <Card :preview="require('@/assets/images/image_1.png')" title="Skyrim.История создания великой игры"
            description="Франк Экстанази" />
        <Card :preview="require('@/assets/images/image_2.png')" title="Поисковое продвижение сайтов"
            description="Сергей Анисимов" />

        <Card :preview="require('@/assets/images/image_3.png')" title="Английский для дизайнеров"
            description="Татьяна Магарина" />

        <Card :preview="require('@/assets/images/image_4.png')" title="Дизайн и цвет. Практикум" description="Шон Адамс" />
    </main>
</template>
  
<script>
// @ is an alias to /src
import Card from '@/components/elements/Card'

export default {
    name: 'MainBlock',
    components: {
        Card
    },
    props: {

    },
    setup() {

    }
}
</script>
<style lang="scss" scoped>
.main {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 26px;
}
</style>