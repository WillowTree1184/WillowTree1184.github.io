<template>
    <div id="introduce">
        <div id="introduce-card">
            <div>
                <h2 id="introduce-title">杨柳 WillowTree</h2>
                <p>#1184</p>
            </div>
            <div>
                <p>性别：男</p>
                <p>年龄: 14岁</p>
            </div>
            <div id="introduce-tag-list">
                <p>游戏开发者</p>
                <p>前后端工程师</p>
                <p>文字排版狂魔</p>
                <p>摄影爱好者</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
    #introduce {
        
    }

    #introduce-card {
        transition: 0.5s;
        display: flex;
        flex-direction: column;
        gap: 32px;
        border-radius: 16px;
        color: rgb(230, 230, 230);
        background: rgb(25, 25, 25);
        background-image: linear-gradient(90deg, rgba(25, 25, 25, 0) 0, rgb(25, 25, 25) 250px), url(/src/assets/headphoto.png);
        background-repeat: no-repeat;
        background-size: auto 100%;
        background-position-y: center;
        transform: rotate3d(1, -0.5, 0, 8deg);
        filter: blur(0.25px) brightness(1);
        margin: 25px;
        padding: 32px;
        padding-left: 200px;
    }

    #introduce-card:hover {
        transform: rotate3d(1, -0.5, 0, 0deg);
        filter: blur(0) brightness(1.1);
    }

    #introduce-tag-list {
        display: flex;
        gap: 16px;
    }
</style>