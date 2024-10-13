<template>
    <div id="title">
        <div id="title-container">
            <div id="title-information">
                <p style="--i: 0s">欢迎来到</p>
                <h1 style="--i: 0.1s">杨柳 Willow Tree 的个人网站</h1>
                <p style="--i: 0.2s">Welcome to Willow Tree's own space.</p>
            </div>
        </div>
    </div>
</template>
    
<style scoped>
    #title {
        display: flex;
        align-items: center;
        justify-content: center;
        min-height: 100vh;
        color: rgb(230, 230, 230);
        background: rgb(25, 25, 25);
    }

    #title-container {
        display: flex;
        align-items: center;
        gap: 24px;
    }

    #title-information * {
        animation: title-information-tag-animation 1s ease var(--i) both;
    }

    @keyframes title-information-tag-animation {
        0% {
            opacity: 0;
            transform: translateX(50px);
            filter: blur(50px);
        }

        25% {
            transform: translateX(50px);
        }

        100% {
            transform: translateX(0);
        }
    }
</style>