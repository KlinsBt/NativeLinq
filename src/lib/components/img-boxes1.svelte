<script>
import img1 from "../images/bgs/img1.jpg";
import img2 from "../images/bgs/img2.jpg";
import img3 from "../images/bgs/img3.jpg";
</script>




<div class="info-box">
    <div>
        <div>
            <h1>Por Que Somos Distintos?</h1>
            <p>
                NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo 
                Nativo. Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar 
                el futuro de tu hijo/a en un mundo cada vez mas internacional, hace falta algo 
                mas. Con el metodo nativo, los ninos aprenden de la misma manera que los hablantes 
                nativos: hacia juegos, conversacion, y temas importantes para ellos.
            </p>
        </div>
        <img src={img1} alt="Kid">
    </div>
    <div>
        <img src={img2} alt="Kid">
        <div>
            <h1>Por Que Somos Distintos?</h1>
            <p>
                NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo 
                Nativo. Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar 
                el futuro de tu hijo/a en un mundo cada vez mas internacional, hace falta algo 
                mas. Con el metodo nativo, los ninos aprenden de la misma manera que los hablantes 
                nativos: hacia juegos, conversacion, y temas importantes para ellos.
            </p>
        </div>
    </div>
</div>





<style>

.info-box {
    display: grid;
    justify-items: center;
    background-color: white;
    width: 100%;
}

.info-box > div {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    width: 100%;
}

.info-box > div > div > h1 {
    max-width: 600px;
}

.info-box > div > div > p {
    max-width: 600px;
    padding: 0px 25px;
}

.info-box > div > img {
    width: 100%;
    height: auto;
}

@media (min-width: 1500px) {

    .info-box > div > img {
        max-width: 800px;
    }
}

@media (min-width: 1265px) and (max-width: 1499px) {

    .info-box > div > img {
        max-width: 600px;
    }
}

@media (min-width: 0px) and (max-width: 1264px) {

    .info-box > div {
        justify-content: center;
    }

    .info-box > div:nth-child(2) {
        flex-direction: column-reverse;
    }

    .info-box > div > div {
        align-self: center;
    }

    .info-box > div > img {
        max-width: 600px;
        align-self: center;
    }
}

</style>