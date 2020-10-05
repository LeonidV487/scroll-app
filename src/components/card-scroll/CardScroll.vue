<template>
    <v-card
            outlined
            class="border-transparent mt-3 ml-12 py-1"
            width="180"
    >

        <v-row v-for="item in content"
               :key="item.id"
               class="justify-center flex-column border-1 ma-2">
            <v-img
                    :src="item.image"
                    contain
                    class="mt-5"
                    height="20"
            ></v-img>
            <p class="caption text-center font-weight-medium pt-2">{{item.text}}</p>
        </v-row>
    </v-card>
</template>

<script>
    export default {
        name: "CardScroll",

        data: () => ({
            content: [
                {id: 1, text: "Аналитика", image: require("../../images/Group.png")},
                {id: 2, text: "Продукт", image: require("../../images/Product.png")},
                {id: 3, text: "Пользователи", image: require("../../images/Group.png")},
                {id: 4, text: "Конструктор сайта", image: require("../../images/Builder.png")},
                {id: 5, text: "Трансляции", image: require("../../images/Stream.png")},
                {id: 6, text: "Рассылка", image: require("../../images/Mail.png")},
                {id: 7, text: "Маркетинг", image: require("../../images/Marketing.png")},
                {id: 8, text: "Платежи", image: require("../../images/Payments.png")},
                {id: 9, text: "Настройки", image: require("../../images/Settings.png")},
            ]
        }),
    }
</script>

<style scoped>

</style>