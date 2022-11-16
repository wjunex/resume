<template>
    <div class="nav-box">
        <div class="nav">
            <div class="nav-item" v-for="(item, index) in navList" :key="index" @click="goToPage(index)">{{ item }}
            </div>
        </div>

    </div>
    <div class="content">
        <div class="page">Smiley Sans
            Type design  

            AD: Nagisa Chen
            D: oooooohmygosh, Nagisa Chen, Janine Sui, Heda Shi, Jian Li
            得意黑是一款在人文观感和几何特征中寻找视觉平衡的现代窄斜体。

            A condensed and oblique Chinese typeface seeking a visual balance between the humanist and the geometric.

            ➡ 下载 / Download</div>
        <div class="page" style="background-color: teal;">2</div>
        <div class="page">3</div>
        <div class="page" style="background-color: teal;">4</div>
    </div>
</template>

<script setup lang="ts">

import { ref, onMounted } from 'vue'

const navList = ref(['测试1', '测试2', '测试3', '测试4'])


const goToPage = (e) => {
    let top = window.innerHeight * e
    window.scrollTo({
        top: top,
        behavior: "smooth"
    });

}
onMounted(() => {

})

</script>

<style scoped lang="scss">
.nav-box {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 999;
}

.nav {
    width: 80%;
    height: 60px;
    background-color: bisque;
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin: 0 auto;
}

.content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;



    .page {
        width: 100%;
        height: 100vh;
        color: black;
        font-weight: 100;
        font-size: 14px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}
</style>