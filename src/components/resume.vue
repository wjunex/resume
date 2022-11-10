<script setup lang="ts">
import { ref } from 'vue'

let title = ref('web前端开发工程师')
let photo = ref('https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fc-ssl.duitang.com%2Fuploads%2Fblog%2F202105%2F04%2F20210504062111_d8dc3.thumb.1000_0.jpg&refer=http%3A%2F%2Fc-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1670679478&t=fe058430d2f167aed16d91ea76323c71')
let name = ref('王俊');
let info = ref(['贵州大学', '25岁', '两年经验'])


</script>

<template>
    <div class="content-box">
        <div class="title">{{ title }}</div>
        <img class="photo" :src="photo" alt="">
        <div class="name">{{ name }}</div>
        <div class="info">
            <div class="info-item" v-for="(item, index) in info" :key="index">{{ item }}</div>
        </div>
        <div class="main">
            <p>You came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.</p>
            <p>You came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.You came to me Like the dawn through the night Just shining
                like the sun.You came to me Like the dawn through the night Just shining like the sun.You came to me
                Like the dawn through the night Just shining like the sun.You came to me Like the dawn through the night
                Just shining like the sun.You came to me Like the dawn through the night Just shining like the sun.You
                came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.</p>
            <p>You came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.You came to me Like the dawn through the night Just shining
                like the sun.You came to me Like the dawn through the night Just shining like the sun.You came to me
                Like the dawn through the night Just shining like the sun.You came to me Like the dawn through the night
                Just shining like the sun.You came to me Like the dawn through the night Just shining like the sun.You
                came to me Like the dawn through the night Just shining like the sun.</p>
            <p>You came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.You came to me Like the dawn through the night Just shining
                like the sun.You came to me Like the dawn through the night Just shining like the sun.You came to me
                Like the dawn through the night Just shining like the sun.You came to me Like the dawn through the night
                Just shining like the sun.You came to me Like the dawn through the night Just shining like the sun.You
                came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.</p>
            <p>You came to me Like the dawn through the night Just shining like the sun.You came to me Like the dawn
                through the night Just shining like the sun.You came to me Like the dawn through the night Just shining
                like the sun.You came to me Like the dawn through the night Just shining like the sun.You came to me
                Like the dawn through the night Just shining like the sun.You came to me Like the dawn through the night
                Just shining like the sun.You came to me Like the dawn through the night Just shining like the sun.You
                came to me Like the dawn through the night Just shining like the sun.</p>

        </div>
    </div>
</template>



<style lang="scss" scoped>
.content-box {
    width: 60%;
    background-color: #FFF;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    padding: 60px;
    box-sizing: border-box;

    .title {
        font-size: 24px;
    }

    .photo {
        width: 66px;
        height: 66px;
        border-radius: 50%;
        margin-top: 60px;
    }

    .name {
        font-size: 18px;
        margin-top: 10px;
    }

    .info {
        display: flex;
        margin-top: 60px;
        border-top: 1px solid #000;
        padding: 6px;

        .info-item {
            font-size: 16px;
            margin-left: 6px;
        }
    }

    .main {
        margin-top: 60px;
        width: 100%;

    }




}
</style>