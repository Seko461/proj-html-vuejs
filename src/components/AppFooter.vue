<script>
export default {
    name: 'AppFooter',

}
</script>
<template>
    <footer class="footer">
        <div class="row">
            <div class="left col-2">
                <div class="container">
                    <div class="find-us">
                        <div class="find-title">
                            <h4>FIND OUR RESTAURANTS</h4>
                        </div>
                        <div class="restaurant">
                            <p>1614 E. Bell Rd #104. <br>
                                Salerno, AZ 85022 <br>
                                (602) 867-1010</p>
                        </div>
                        <div class="restaurant">
                            <p>204 E. Piazzetta Tommaso <br>
                                Sorrento, AZ 85022 <br>
                                (358) 867-1010</p>
                        </div>
                        <div class="restaurant">
                            <p>Vale Puglia 54 <br>
                                Torre Del Greco AZ 85022 <br>
                                (359) 867-1010</p>
                        </div>
                        <div class="restaurant">
                            <p>Corso Itali AA <br>
                                Naples, AZ 85022 <br>
                                (989) 867-1010</p>
                        </div>
                    </div>
                    <div class="working-hours">
                        <h4>WORKING HOURS</h4>
                        <div class="day">
                            <h5>MONDAY</h5>
                            <span class="red">Kitchen Closed</span>
                        </div>
                        <div class="day">
                            <h5>TUESDAY UNTIL FRIDAY</h5>
                            <p>9:00 - 22:00</p>
                        </div>
                        <div class="day">
                            <h5>SATURDAY <span class="red signal">*</span></h5>
                            <p>Saturday 11 am to midnightd</p>
                        </div>
                        <div class="day">
                            <h5>SUNDAY</h5>
                            <p>9:00 - 22:00</p>
                        </div>
                        <div class="follow-us">
                            <span>FOLLOW US:</span>
                            <div class="social-icons">
                                <i class="fa-brands fa-twitter"></i>
                                <i class="fa-brands fa-facebook-f"></i>
                                <i class="fa-brands fa-square-instagram"></i>
                                <i class="fa-brands fa-linkedin-in"></i>

                            </div>
                        </div>
                    </div>
                    <div class="final-quote">
                        <h3>THE DON PEPPE CREW <br>
                            FIRST AND FOREMOST <br>
                            VALUES AN AUTHENTIC,<br>
                            WELL BAKED SLICE OF <br>
                            PIZZA.</h3>
                    </div>
                </div>
                <img width="80" class="bottom-image"
                    src="/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/footer-bottom-img.png"
                    alt="">
            </div>
            <div class="right col-2">
                <img src="/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/footer-img-1.jpg" alt="">
            </div>
        </div>
    </footer>
    <!-- /.footer -->
</template>
<style>
.footer {
    height: 470px;
    /* border: 1px solid red; */
    overflow: hidden;
}

.footer .left {
    background-image: url(/progetto front end finale pizza/drive-download-20240408T091339Z-001/img/cielostellato.PNG);

    display: flex;

    justify-content: center;


    .container {
        height: 50%;
        width: 80%;
        /* border: 1px solid red; */
        transform: translateY(5rem);
        display: flex;
        justify-content: space-between;
    }

}

.find-title>h4,
.working-hours>h4 {
    color: #B7903C;
    font-size: .75rem;
}

.restaurant,
.day {
    margin-top: 1rem;
}

.restaurant>p,
.day>p {
    color: #adadad;
    font-size: .6rem;
    line-height: 1.2rem;
}



.day>h5 {
    color: #B7903C;
}

.red {
    color: #d2401e;
    font-size: .75rem;
}

.follow-us {
    margin-top: 1.5rem;
    display: flex;
    align-items: center;
    gap: .5rem;

    >span {
        font-size: .8rem;
        color: #B7903C;
    }
}

.social-icons>i {
    margin-right: .5rem;
    color: white;
    font-size: .6rem;
}

.final-quote>h3 {
    color: white;
    font-size: 1rem;
    line-height: 1.8rem;
}

.left {
    position: relative;
}

.bottom-image {
    position: absolute;
    z-index: 22;
    bottom: 140px;
    right: 40px;
}

.footer .right {
    >img {
        width: 100%;

    }
}
</style>