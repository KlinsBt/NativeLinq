<script>
// import img1 from "../images/bgs/img1.jpg";
// import img2 from "../images/bgs/img2.jpg";
// import img3 from "../images/bgs/img3.jpg";
import img4 from "../images/bgs/kid-widescreen.png";
import c1 from "../images/carousel/i1.png";
import c2 from "../images/carousel/i2.png";
import c3 from "../images/carousel/i3.png";
import c4 from "../images/carousel/i4.png";
import c5 from "../images/carousel/i5.png";
import c6 from "../images/carousel/i6.png";
import c7 from "../images/carousel/i7.png";
import c8 from "../images/carousel/i8.png";
import c9 from "../images/carousel/i9.png";
import c10 from "../images/carousel/i10.png";
import c11 from "../images/carousel/i11.png";
</script>




<div class="content">
    <div class="img-container">
        <h1>APRENDE INGLÉS</h1>
        <img id="c1" src={c1} alt="Icon 1">
        <img id="c2" src={c2} alt="Icon 2">
        <img id="c3" src={c3} alt="Icon 3">
        <img id="c4" src={c4} alt="Icon 4">
        <img id="c5" src={c5} alt="Icon 5">
        <img id="c6" src={c6} alt="Icon 6">
        <img id="c7" src={c7} alt="Icon 7">
        <img id="c8" src={c8} alt="Icon 8">
        <img id="c9" src={c9} alt="Icon 9">
        <img id="c10" src={c10} alt="Icon 10">
        <img id="c11" src={c11} alt="Icon 11">
        <img id="kid" src={img4} alt="1">
    </div>
</div>





<style>

.content {
    position: relative;
    display: grid;
    justify-items: center;
    padding: 0px 25px;
    background: rgb(83,192,212);
    background: linear-gradient(42deg, rgba(83,192,212,1) 15%, rgba(132,208,224,1) 47%, rgba(164,223,241,1) 83%);
    width: 100%;
    min-height: 900px;
    overflow: hidden;
}

.img-container {
    display: grid;
    gap: 1rem;
    width: 100%;
    height: 400px;
    z-index: 3;
}

.img-container > h1 {
    font-family: KristenITC, "Segoe UI", "Helvetica Neue", sans-serif !important;
    font-size: 50px;
    color: black;
    position: absolute;
    top: 320px;
    left: 300px;
}

#kid {
    position: absolute;
    width: 1500px;
    height: auto;
    bottom: 0px;
    right: 0px;
}

#c1 {
    width: 150px;
    height: auto;
    position: absolute;
    top: 430px;
    left: 25px;
    animation: tilt1 10s infinite linear;
}

#c2 {
    width: 130px;
    height: auto;
    position: absolute;
    top: 550px;
    left: 100px;
    animation: tilt2 11s infinite linear;
}

#c3 {
    width: 140px;
    height: auto;
    position: absolute;
    top: 650px;
    left: 190px;
    animation: tilt1 11s infinite linear;
}

#c4 {
    width: 140px;
    height: auto;
    position: absolute;
    top: 220px;
    left: 110px;
    animation: tilt2 12s infinite linear;
}

#c5 {
    width: 140px;
    height: auto;
    position: absolute;
    top: 740px;
    left: 370px;
    animation: tilt1 8s infinite linear;
}

#c6 {
    width: 150px;
    height: auto;
    position: absolute;
    top: 150px;
    left: 280px;
    animation: tilt2 12s infinite linear;
}

#c7 {
    width: 120px;
    height: auto;
    position: absolute;
    top: 20px;
    left: 430px;
    animation: tilt1 9s infinite linear;
}

#c8 {
    width: 150px;
    height: auto;
    position: absolute;
    top: 450px;
    left: 350px;
    animation: tilt2 10s infinite linear;
}

#c9 {
    width: 120px;
    height: auto;
    position: absolute;
    top: 600px;
    left: 540px;
    animation: tilt1 9s infinite linear;
}

#c10 {
    width: 150px;
    height: auto;
    position: absolute;
    top: 100px;
    left: 800px;
    animation: tilt2 11s infinite linear;
}

#c11 {
    width: 120px;
    height: auto;
    position: absolute;
    top: 220px;
    left: 600px;
    animation: tilt1 9s infinite linear;
}

@keyframes tilt1 {
  0% {transform: translate(0px, 0%);}
  50% {transform: translate(20px, 10px) rotate(15deg);}
  100% {transform: translate(0px, 0px);}
}

@keyframes tilt2 {
  0% {transform: translate(0px, 0%);}
  50% {transform: translate(-20px, 15px) rotate(-15deg);}
  100% {transform: translate(0px, 0px);}
}

@media (min-width: 935px) and (max-width: 1265px) {
    #kid {
        display: none;
    }
}

@media (min-width: 580px) and (max-width: 934px) {
    #kid {
        display: none;
    }

    .img-container > h1 {
        font-size: 50px;
        top: 270px;
        left: 70px;
    }

    #c4 {
        width: 140px;
        top: 20px;
        left: 80px;
    }
}

@media (min-width: 545px) and (max-width: 579px) {
    #kid {
        display: none;
    }

    .img-container > h1 {
        font-size: 50px;
        top: 270px;
        left: 40px;
    }

    #c4 {
        width: 140px;
        top: 20px;
        left: 80px;
    }
}

@media (min-width: 0px) and (max-width: 545px) {
    #kid {
        display: none;
    }

    .img-container > h1 {
        font-size: 45px;
        top: 270px;
        left: 10px;
        max-width: 450px;
    }

    #c4 {
        width: 140px;
        top: 20px;
        left: 80px;
    }
}

</style>