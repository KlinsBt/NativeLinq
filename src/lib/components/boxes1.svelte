<script>
    import icon1 from "$lib/images/libro-abierto2.png";
    import icon2 from "$lib/images/chat.png";
    import icon3 from "$lib/images/usuarios.png";
</script>





<div class="boxes-container">
    <div class="box">
        <div class="box-img-container">
            <img src={icon1} alt="Box Icon">
        </div>
        <h2>Aprendizaje divertido</h2>
        <p>
            En NativeLinq creemos que aprender Ingles debe ser 
            divertido. Nuestros profesores tienen mucha energia y 
            hacen juegos divertidos en Ingles para reforzar las habilidades 
            de hablar de tu hijo.
        </p>
    </div>
    <div class="box">
        <div class="box-img-container">
            <img src={icon2} alt="Box Icon">
        </div>
        <h2>Preparacion de examenes</h2>
        <p>
            Preparacion experta para cualquier examen: de A1 hasta 
            C2. Aprende con los mejores profesores y asegure tu futuro.
        </p>
    </div>
    <div class="box">
        <div class="box-img-container">
            <img src={icon3} alt="Box Icon">
        </div>
        <h2>Metodo nativo</h2>
        <p>
            Aprender como aprenden los nativos: sin libros de texto ni 
            ejercicios de gramática. Aprender Ingles util y practico, hacia 
            clases de conversacion con hablantes nativos.
        </p>
    </div>
</div>





<style>

.boxes-container {
    display: flex;
    justify-content: center;
    align-items: start;
    flex-wrap: wrap;
    gap: 1rem;
    height: auto;
}

.box {
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: center;
    gap: 1rem;
    padding: 1rem;
    border: 1px solid rgba(0, 0, 0, 0);
    border-radius: 10px;
    max-width: 220px;
    height: 350px;
    transition: all 0.1s linear;
    /* cursor: pointer; */
}

.box:hover {
    border: 1px solid var(--brand-color-3);
}

.box:nth-child(1) > .box-img-container {
    background-color: rgba(252, 130, 89);
}

.box:nth-child(2) > .box-img-container {
    background-color: rgb(255 238 156);
}

.box:nth-child(3) > .box-img-container {
    background-color: rgb(98 93 238);
}

.box-img-container {
    width: 100px;
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 25px;
}

.box-img-container > img {
    width: 70%;
    height: auto;
    object-fit: contain;
}

.box > h2 {
    text-align: center;
    max-width: 155px;
    margin: 5px 0px 0px 0px;
}

.box > p {
    text-align: center;
    margin: 5px 0px 0px 0px;
}

</style>