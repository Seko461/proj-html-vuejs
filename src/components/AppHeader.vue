<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            leftVoices: ['HOME', 'PAGES', 'MENU'],
            rightVoices: ['EVENT', 'BLOG', 'LANDING'],


        }
    }

}
</script>
<template>
    <header class="header">

        <nav class="nav-bar">

            <div class="left">
                <button class="order"><a href="#">ORDER ONLINE</a></button>
                <ul>
                    <li style="cursor: pointer" v-for="voice in   leftVoices  ">{{ voice }}</li>
                </ul>
            </div>
            <!-- /.left -->
            <div class="center-logo">
                <img width='120'
                    src="/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/h5-logo-divided-header.png"
                    alt="">
            </div>
            <!-- /.center-logo -->
            <div class="right">
                <ul>
                    <li style="cursor: pointer" v-for="  voice   in   rightVoices  ">{{ voice }}</li>
                </ul>
                <button class="cart">
                    <div class="counter">
                        0
                    </div>
                    <img width="20"
                        src="../../public/progetto front end finale pizza/drive-download-20240408T091339Z-001/svg/svg-1.svg"
                        alt="">
                    <a href="#">CART</a>
                </button>
                <button>
                    <i class="fa-solid fa-magnifying-glass fa-flip-horizontal"></i>
                    <a href="#">SEARCH</a></button>
            </div>
            <!-- /.right -->

        </nav>
        <!-- /.nav-bar -->
        <jumbo class="jumbo">

            <div class="controls">
                <div class="prev">
                    <p>PREV</p>
                </div>
                <img width="240"
                    src="/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/h3-rev-img-6.png" alt="">
                <div class="next">
                    <p>NEXT</p>
                </div>
            </div>
            <div class="pizza-slice">
                <img src="/progetto front end finale pizza/drive-download-20240408T091339Z-001/svg/svg-4.svg" alt="">
            </div>
        </jumbo>
        <!-- /.jumbo -->
    </header>
    <!-- /.header -->
</template>
<style>
.header {
    /* border: 1px solid red; */
    height: 30rem;
    background-image: url(/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/cielostellato.PNG);
    background-position: center;





}



.nav-bar {
    /* border: 1px solid black; */
    padding-top: 1rem;
    display: flex;
    justify-content: center;
    gap: 2rem;
    align-items: center;





    .left,
    .right {
        display: flex;
        gap: 1rem;
    }


}

.left ul {
    margin-left: 4rem;
}

.right ul {
    margin-right: 3rem;
}


.nav-bar ul {
    display: flex;
    flex-direction: row;
    gap: 2rem;
    list-style: none;
    align-items: center;


}

.left>ul>li {
    color: white;
    font-size: .5rem;
}

.right>ul>li {
    color: white;
    font-size: .5rem;
}


.nav-bar>li>img {
    color: white;

}

a {
    text-decoration: none;
    font-size: .5rem;
    color: white;


}

.cart {

    display: flex;
    align-items: center;
    gap: .25rem;

}

.cart a {
    padding-top: .222rem;
}

.counter {
    background-color: white;
    width: .75rem;
    height: .75rem;
    border-radius: 50%;
    font-size: .5rem;
    color: red;
    transform: translateX(.75rem);
    margin-bottom: .5rem;
    text-align: center;

}

.nav-bar button {
    border: none;
    background-color: transparent;
    letter-spacing: .1rem;

}

.order a {
    background-color: #D2401E;
    padding: .5rem 1.5rem;
}


.mustache-icon {
    margin-right: .2rem;
}

.fa-magnifying-glass {
    color: white;
    font-size: .55rem;
    margin-right: .2rem;
}

.jumbo {
    background-image: url(/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/h3-rev-img-5.png);
    background-repeat: no-repeat;
    background-size: 38rem;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;

}


.prev,
.next {
    background-color: white;
    font-size: .5rem;
    text-align: center;
    height: 3rem;
    width: 3rem;
    border-radius: 50%;
    color: #D2401E;
    cursor: pointer;

}

.prev {

    transform: translateX(-1.75rem);
    display: flex;


}

.prev p {
    padding-bottom: 3.2rem;
    padding-right: .5rem;
    transform: rotatez(90deg);
    letter-spacing: .1rem;
}

.next {
    transform: translateX(1.75rem);
    display: flex;
}

.next p {
    transform: rotatez(-90deg);
    padding-top: 1.25rem;
    letter-spacing: .1rem;
}

.controls {
    justify-content: space-between;
    align-items: center;
    display: flex;
    width: 100%;
    /* border: 1px solid magenta; */
    /* transform: translateY(2rem); */
}

.controls img {
    transform: translateY(2rem);
}

.pizza-slice {
    /* border: 1px solid black; */
    z-index: 999;
    position: fixed;
    top: 800px;
    right: 20px;
    width: 3rem;
    height: 3rem;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    background-color: #fbf9f9;
    cursor: pointer;
}

.pizza-slice:hover {
    background-color: lightgray;

}
</style>