<template>
    <div class="slider-jour">
        <H1 style="font-weight: bolder;">les articles en<br> solde</H1>
        <div class="slider">
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <span style="font-size: 0.8rem; text-decoration:line-through ;">500.000 </span> CFA
                    <h5 style="font-size: 1rem; color: red;">302.000 CFA</h5>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <span style="font-size: 0.8rem; text-decoration:line-through ;">500.000 </span>CFA
                    <h5 style="font-size: 1rem; color: red;">302.000 CFA</h5>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <span style="font-size: 0.8rem; text-decoration:line-through ;">500.000 </span>CFA
                    <h5 style="font-size: 1rem; color: red;">302.000 CFA</h5>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <span style="font-size: 0.8rem; text-decoration:line-through ;">500.000 </span>CFA
                    <h5 style="font-size: 1rem; color: red;">302.000 CFA</h5>
                </div>
            </div>
            <div class="card">
                <img src="/iphone15.jpg" alt="iphone 15">
                <div class="info">
                    <p>nom du prduit</p>
                    <span style="font-size: 0.8rem; text-decoration:line-through ;">500.000 </span>CFA
                    <h5 style="font-size: 1rem; color: red;">302.000 CFA</h5>
                </div>
            </div>

        </div>
    </div>
</template>

<style scoped>
.slider-jour {
    box-sizing: border-box;
}

.slider {
    padding: 20px;
    width: 90%;
    display: flex;
    overflow-x: auto;

}

.slider .card {
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
}</style>