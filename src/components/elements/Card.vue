<template>
    <div class="card">
        <img class="card__preview" :src="preview" alt="">
        <div class="card__info">
            <CardInfo :title="title" :description="description" />
        </div>
        <div class="card__button">
            <ButtonCard name="Купить" />
        </div>

    </div>
</template>
  
<script>
// import { stringifyQuery } from 'vue-router';

// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import ButtonCard from '@/components/ui/ButtonCard.vue'
import CardInfo from '@/components/elements/CardInfo.vue'

export default {
    name: 'CardElement',
    components: {
        ButtonCard, CardInfo
    },
    props: {
        title: {
            type: String,
            default: "Name"
        },
        description: {
            type: String,
            default: "description"
        },
        preview: {
            type: String,
            default: ''
        }
    },
    setup() {

    }
}
</script>
<style lang="scss" scoped>
.card {
    // width: 330px;
    // height: 490px;
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 1px;
    border-radius: 10px;
    // margin: 26px;
    background: #FFF;
    /* Тень серая */
    box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.30);
    justify-content: center;
    // margin-top: 19px;
    padding: 10px;
}

.card__button {
    margin-bottom: 24px;
    // margin-top: auto;
}

.card__info {
    display: inline-flex;
    flex-direction: column;
    align-items: center;
    gap: 14px;
    margin: 26px;
}
</style>