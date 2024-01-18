<template>
    <div class="slider-jour">
        <div class="slider">
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>Iphone 15 Black, 256 GIGA</p>
                        <h3>302.000 CFA</h3>
                    </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <h2>302.000 CFA</h2>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <h2>302.000 CFA</h2>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <h2>302.000 CFA</h2>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <h2>302.000 CFA</h2>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <h5 style="font-size: 1rem;">302.000 CFA</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.slider-jour{
    box-sizing: border-box;
}
.slider{
    padding: 20px;
    width: 90%;
    display: flex;
    overflow-x: auto;

}
.slider .card{
    padding: 10px;
    height: 350px;
    width: 200px;
    background-color: white;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0px 20px 0px 0px;
}
.card img {
    width: 150px;
}
</style>