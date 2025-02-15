<template>
    <div class='main'>
        <img src='./assets/image-qr-code.png' alt="lightblue background qr code image" class='qr'>
        <div class='cite'>
            <h4 class='outfit-700'>Improve your front-end skills by building projects</h4>
            <p class='outfit-400'>Scan the QR code to visit Frontend Mentor and take your coding skills to the next
                level</p>
        </div>

    </div>
</template>

<script>
export default {
    name: "App"
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@100..900&display=swap');

:root {
    --Slate300: hsl(212, 45%, 89%);
    --Slate500: hsl(216, 15%, 48%);
    --Slate900: hsl(218, 44%, 22%);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: black;
    display: flex;
    flex-direction: column;
    align-items: center;

}

#app {
    background-color: var(--Slate300);
    width: 1390px;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.main {
    background-color: white;
    width: 310px;
    height: 480px;
    border-radius: 20px;
    padding: 15px;
}

.qr {
    width: 280px;
    height: 280px;
    border-radius: 10px;
}

.cite {
    h4 {
        font-size: 20px;
        padding: 10px;
        text-align: center;
        margin-top: 10px;
        letter-spacing: 0.9px;
    }

    p {
        font-size: 15px;
        padding: 10px;
        text-align: center;
        margin-bottom: 10px;
    }
}

.outfit-400 {
    font-family: "Outfit", serif;
    font-optical-sizing: auto;
    font-weight: 400;
    font-style: normal;
    color: var(--Slate500);
}

.outfit-700 {
    font-family: "Outfit", serif;
    font-optical-sizing: auto;
    font-weight: 700;
    font-style: normal;
    color: var(--Slate900);
}

@media only screen and (max-width: 520px) {
    #app {
        width:380px;
        height:810px;
    }
}
</style>