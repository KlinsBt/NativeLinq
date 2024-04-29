<script>

export let name = "Cory Partridge";
export let description = "";
export let img_src = "";

</script>





<div class="container">
    <div class="svg-background"></div>
    <div class="svg-background2"></div>
    <!-- <div class="circle"></div> -->
    <div class="pfp-container">
      <img class="profile" src="{img_src}" alt="Profile">
    </div>
    <div class="text-container">
        <p class="name-text">{name}</p>
        <p class="desc-text">{description}</p>
    </div>
</div>
  




<style>
.container {
  position: relative;
  background-color: var(--brand-color-1);
  background-color: #f9f9fa;
  min-width: 280px;
  min-height: 500px;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0px 0px 15px 1px rgb(179, 179, 179);
  margin: 25px;
}

.svg-background {
  width: 350%;
  height: 100%;
  position: absolute;
  top: -300px;
  left: -50px;
  z-index: 1;
  background-color: var(--brand-color-2);
  -webkit-clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
  clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
  transform: rotate(20deg);
}

.svg-background2 {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0px;
  left: -70px;
  background-color: var(--brand-color-3);
  background-color: var(--brand-color-1);
  /* background-color: rgb(194, 194, 194); */
  z-index: 1;
  -webkit-clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
  clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
  transform: rotate(40deg);
}

.pfp-container {
  position: absolute;
  width: 150px;
  height: 150px;
  margin-top: -10px;
  margin-left: -10px;
  overflow: hidden;
  border-radius: 0px 50% 50% 0px;
  border: 7px solid #ECEFF1;
  z-index: 3;
}

.profile {
  width: 100%;
  height: auto;
  z-index: 3;
}

.text-container {
  position: absolute;
  right: 0;
  margin: 170px 0px 0px 0px;
  max-width: 245px;
  padding-right: 10px;
  text-align: left;
  z-index: 2;
}

.name-text {
  color: var(--brand-color-3);
  font-size: 28px;
  font-weight: 700;
  margin: 5px 0px 0px 0px;
  text-align: center;
}

.desc-text {
  font-size: 15px;
  margin: 15px 0px 0px 0px;
}
</style>