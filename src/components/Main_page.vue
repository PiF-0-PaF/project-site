<template>
   <div class="header">
        <div class="levaya_chast">
            <router-link to="menu.vue">
                <svg class="icons" width="80" height="80" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<rect width="80" height="80" fill="url(#pattern0)"/>
<defs>
<pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
<use xlink:href="#image0_16_2" transform="scale(0.00195312)"/>
</pattern>
<image id="image0_16_2" width="512" height="512" xlink:href="data:image/png;base64,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"/>
</defs>
                </svg>
            </router-link>  

            <svg class="icons" width="60" height="60" viewBox="0 0 80 69" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 68.8172V57.3477H80V68.8172H0ZM0 40.1434V28.6738H80V40.1434H0ZM0 11.4695V0H80V11.4695H0Z" fill="black"/>
            </svg>
        </div>
        
        <div class="pravaya_chast">
            <svg class="icons" width="80" height="80" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M40 64C31.6667 64 24.3 59.7333 20 53.3333C20.1 46.6667 33.3334 43 40 43C46.6667 43 59.9 46.6667 60 53.3333C57.7963 56.6147 54.8195 59.3038 51.3319 61.1639C47.8442 63.024 43.9527 63.998 40 64ZM40 16.6667C42.6522 16.6667 45.1957 17.7202 47.0711 19.5956C48.9465 21.471 50 24.0145 50 26.6667C50 29.3188 48.9465 31.8624 47.0711 33.7377C45.1957 35.6131 42.6522 36.6667 40 36.6667C37.3479 36.6667 34.8043 35.6131 32.929 33.7377C31.0536 31.8624 30 29.3188 30 26.6667C30 24.0145 31.0536 21.471 32.929 19.5956C34.8043 17.7202 37.3479 16.6667 40 16.6667ZM40 6.66666C35.6226 6.66666 31.2881 7.52885 27.2439 9.20401C23.1997 10.8792 19.5251 13.3345 16.4298 16.4298C10.1786 22.681 6.66669 31.1594 6.66669 40C6.66669 48.8405 10.1786 57.319 16.4298 63.5702C19.5251 66.6655 23.1997 69.1208 27.2439 70.796C31.2881 72.4711 35.6226 73.3333 40 73.3333C48.8406 73.3333 57.319 69.8214 63.5702 63.5702C69.8215 57.319 73.3334 48.8405 73.3334 40C73.3334 21.5667 58.3334 6.66666 40 6.66666Z" fill="black"/>
            </svg>
        </div>
   </div>

   <div class="content">
        <div class="item">
            <img src="@/assets/tovar1.png" alt="">
            <div class="text">AMD Ryzen 5</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar2.png" alt="">
            <div class="text">Intel Core i5</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar3.png" alt="">
            <div class="text">DELL h27s</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar4.png" alt="">
            <div class="text">DELL h21</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar5.png" alt="">
            <div class="text">Samsung G15RT43</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar6.png" alt="">
            <div class="text">KINGSTON FURY</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar7.png" alt="">
            <div class="text">SEAGATE SkyHawk</div>
        </div>
        <div class="item">
            <img src="@/assets/tovar8.png" alt="">
            <div class="text">Western Digital</div>
        </div>
        
   </div>
</template>
<script>
export default{}

</script>
<style scoped>

.header{

    width: 100%;
    height: 100px;
    display: flex;
    background: linear-gradient(85deg, #fb63f9, #c2e534);
}

.levaya_chast{
    width: 100%;
    display: flex;
    flex-direction: row-reverse;
    flex-wrap: wrap;
    align-content: center;
    justify-content: space-between;
    align-items: center;
}

.pravaya_chast{
    width: 100px;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    align-content: stretch;
    justify-content: flex-end;
    align-items: center;
}

.icons{
    cursor: pointer;
}

.content{
    width: 100%;
    height: 100vh;
    display: flex;
    flex-wrap: wrap;
    align-content: space-around;
    justify-content: space-around;
    flex-direction: column;
    background: linear-gradient(85deg, white, whitesmoke);
}

.text{
    font-size: 24px;
    font-weight: 400;
    color: white;
    background-color: grey;
}

.item{
    margin-top: 50px;
    cursor: pointer;
}

</style>
