<template>
  <div class="container mx-auto px-6 main-container-desktop">
    <div class="grid grid-cols-2 gap-3 mt-8">
      <div>
        <div class="bg-transparent p-8 mt-4 text-left">
          <p class="text-7xl brand-tedara mb-2 pl-0 p-2">Tedara</p>
          <p class="text-3xl font-black mb-2">Order from restaurants near you.</p>
          <p class="text-md mb-3 font-thin">
            <span class="font-semibold">Tedara</span>  is the easy way to get the food you love delivered. 
            We bring food from the best restaurants and desserts to your doorstep. 
            We have hundreds of restaurants to choose from.
          </p>
          <button class="btn-unblur">Use App Now</button>
        </div>
      </div>
      <div class="px-6 mt-8 bg-transparent text-center">
        <div class="phone phone-use">
          <div class="notch"></div>
            <div class="iframe-wrapper">
              <iframe title="appIframe" src="https://demo.foodomaa.com/" 
              frameborder="0" id="appIframe"></iframe>
            </div>
          </div>
      </div>
    </div>
  </div>

  <div class="container mx-auto px-6 desktop-footer">
    <div class="grid grid-cols-2 gap-3 mt-8">
      <div class="bg-transparent p-8 mt-4">
        <p class="text-4xl brand-tedara mb-2 pl-0 p-2">Tedara</p>
        <div class="font-size-sm mb-30">
          <p>#1201, Someplace, Near Somewhere</p>
          <p>
            <a href="/pages/faq" target="_blank">Cookie Policy</a><br>
          </p>
        </div>
      </div>
      <div class="bg-transparent p-8 mt-4">
        <h3 class="h5 font-w700">We Are Social</h3>
        <a href="https://www.facebook.com" class="btn btn-sm btn-rounded btn-alt-secondary mr-10" target="_blank" rel="noopener noreferrer">
          <i class="fa fa-fw fa-facebook"></i>
        </a>
        <a href="https://www.google.com" class="btn btn-sm btn-rounded btn-alt-secondary mr-10" target="_blank" rel="noopener noreferrer">
          <i class="fa fa-fw fa-google-plus"></i>
        </a>
        <a href="https://www.instagram.com" class="btn btn-sm btn-rounded btn-alt-secondary mr-10" target="_blank" rel="noopener noreferrer">
          <i class="fa fa-fw fa-instagram"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
  export default {};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Train+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@200&display=swap');
* {
  font-family: 'Montserrat Alternates', sans-serif;
}

.main-container-desktop {
    min-height: 100vh;
    background: -o-linear-gradient
    (135deg,
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9)
    );
    background: linear-gradient(
    -45deg,
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9)
    );
    background-size: 500% 500%;
    -webkit-animation: Gradient 50s ease infinite;
    animation: Gradient 50s ease infinite;
    position: relative;
    z-index: 1;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    overflow: hidden;
}

.main-container-desktop::before {
    content: "";
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    position: absolute;
    background: url(/images/bg-design.png) no-repeat scroll center bottom/cover;
    z-index: -1;
}

.brand-tedara {
  font-family: 'Train One', cursive;
}
.phone {
    -ms-flex-negative: 0;
    flex-shrink: 0;
    -webkit-box-shadow: 0 0 20px 10px rgba(0, 0, 0, 0.2);
    box-shadow: 0 0 20px 10px rgba(0, 0, 0, 0.2);
    width: 380px;
    height: 665px;
    padding: 10px 7px;
    border-radius: 20px;
    background: #d9dee3;
    -ms-grid-row-align: center;
    -ms-flex-item-align: center;
    align-self: center;
    margin: -3.5rem 0 0 12rem;
    position: relative;
    -webkit-transform: rotate(-15deg);
    -ms-transform: rotate(-15deg);
    transform: rotate(-15deg);
    -webkit-transition: 0.3s linear all;
    -o-transition: 0.3s linear all;
    transition: 0.3s linear all;
}
.phone-use {
    width: 380px;
    height: 665px;
    margin: -3rem 0 0 8rem;
    -webkit-transition: 0.3s linear all;
    -o-transition: 0.3s linear all;
    transition: 0.3s linear all;
    -webkit-transform: rotate(0deg);
    -ms-transform: rotate(0deg);
    transform: rotate(0deg);
}
.phone .notch {
    position: absolute;
    height: 1rem;
    width: 28%;
    background-color: #d9dee3;
    z-index: 9;
    right: 50%;
    -webkit-transform: translate(50%, -5%);
    -ms-transform: translate(50%, -5%);
    transform: translate(50%, -5%);
    border-bottom-left-radius: 2rem;
    border-bottom-right-radius: 2rem;
}
.phone .iframe-wrapper {
    position: relative;
    border-radius: 12px;
    overflow: hidden;
    height: 100%;
}
.phone iframe {
    height: 100%;
    display: block;
    width: 100%;
    border-radius: 12px;
}
.blured {
    -webkit-filter: grayscale(0.8);
    filter: grayscale(0.8);
}
.btn-unblur {
    height: 4rem;
    width: 200px;
    background-color: rgba(0, 0, 0, 0.9);
    text-align: center;
    font-size: 1.2rem;
    font-weight: 500;
    color: #fff;
    border-radius: 0.275rem;
    line-height: 4rem;
    -webkit-transition: 0.2s linear all;
    -o-transition: 0.2s linear all;
    transition: 0.2s linear all;
}
.btn-unblur:hover {
    background-color: #f1593a;
    -webkit-box-shadow: 0 12px 32px rgba(0, 0, 0, 0.4);
    box-shadow: 0 12px 32px rgba(0, 0, 0, 0.4);
    cursor: pointer;
    -webkit-transition: 0.2s linear all;
    -o-transition: 0.2s linear all;
    transition: 0.2s linear all;
}
#appIframe {
    pointer-events: none;
}
.phone-use #appIframe {
    pointer-events: auto !important;
}

/* Footer style */
.desktop-footer {
    min-height: 70vh;
    background: -o-linear-gradient
    (135deg,
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9)
    );
    background: linear-gradient(
    -45deg,
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9),
    rgba(0,0,0,0.9)
    );
    background-size: 500% 500%;
    -webkit-animation: Gradient 50s ease infinite;
    animation: Gradient 50s ease infinite;
    position: relative;
    z-index: 1;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    overflow: hidden;
}

.desktop-footer::before {
    content: "";
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    position: absolute;
    background: url(/images/bg-design.png) no-repeat scroll center bottom/cover;
    z-index: -1;
    -webkit-transform: rotate(
-180deg
);
    -ms-transform: rotate(-180deg);
    transform: rotate(
-180deg
);
}
</style>