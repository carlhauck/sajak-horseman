<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
*,
::before,
::after {
  box-sizing: border-box;
}

*:focus {
  outline: none !important;
}

@font-face {
  font-family: "basier_square_monobold";
  src: url("./fonts/basiersquaremono-bold-webfont.eot");
  src: url("./fonts/basiersquaremono-bold-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-bold-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-bold-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-bold-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monobold_italic";
  src: url("./fonts/basiersquaremono-bolditalic-webfont.eot");
  src: url("./fonts/basiersquaremono-bolditalic-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-bolditalic-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-bolditalic-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-bolditalic-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monomedium";
  src: url("./fonts/basiersquaremono-medium-webfont.eot");
  src: url("./fonts/basiersquaremono-medium-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-medium-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-medium-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-medium-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monoMdIt";
  src: url("./fonts/basiersquaremono-mediumitalic-webfont.eot");
  src: url("./fonts/basiersquaremono-mediumitalic-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-mediumitalic-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-mediumitalic-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-mediumitalic-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monoregular";
  src: url("./fonts/basiersquaremono-regular-webfont.eot");
  src: url("./fonts/basiersquaremono-regular-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-regular-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-regular-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-regular-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monoRgIt";
  src: url("./fonts/basiersquaremono-regularitalic-webfont.eot");
  src: url("./fonts/basiersquaremono-regularitalic-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-regularitalic-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-regularitalic-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-regularitalic-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monosemibold";
  src: url("./fonts/basiersquaremono-semibold-webfont.eot");
  src: url("./fonts/basiersquaremono-semibold-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-semibold-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-semibold-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-semibold-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "basier_square_monoSBdIt";
  src: url("./fonts/basiersquaremono-semibolditalic-webfont.eot");
  src: url("./fonts/basiersquaremono-semibolditalic-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/basiersquaremono-semibolditalic-webfont.woff2") format("woff2"),
    url("./fonts/basiersquaremono-semibolditalic-webfont.woff") format("woff"),
    url("./fonts/basiersquaremono-semibolditalic-webfont.ttf")
      format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "archialight";
  src: url("./fonts/archia-light-webfont.eot");
  src: url("./fonts/archia-light-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/archia-light-webfont.woff2") format("woff2"),
    url("./fonts/archia-light-webfont.woff") format("woff"),
    url("./fonts/archia-light-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "archiaregular";
  src: url("./fonts/archia-regular-webfont.eot");
  src: url("./fonts/archia-regular-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/archia-regular-webfont.woff2") format("woff2"),
    url("./fonts/archia-regular-webfont.woff") format("woff"),
    url("./fonts/archia-regular-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "archiamedium";
  src: url("./fonts/archia-medium-webfont.eot");
  src: url("./fonts/archia-medium-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/archia-medium-webfont.woff2") format("woff2"),
    url("./fonts/archia-medium-webfont.woff") format("woff"),
    url("./fonts/archia-medium-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "archiasemibold";
  src: url("./fonts/archia-semibold-webfont.eot");
  src: url("./fonts/archia-semibold-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./fonts/archia-semibold-webfont.woff2") format("woff2"),
    url("./fonts/archia-semibold-webfont.woff") format("woff"),
    url("./fonts/archia-semibold-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "archiabold";
  src: url("./fonts/archia-bold-webfont.eot");
  src: url("./fonts/archia-bold-webfont.eot?#iefix") format("embedded-opentype"),
    url("./fonts/archia-bold-webfont.woff2") format("woff2"),
    url("./fonts/archia-bold-webfont.woff") format("woff"),
    url("./fonts/archia-bold-webfont.ttf") format("truetype");
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: "fingerpaint";
  src: url("./fonts/FingerPaint-Regular.ttf");
  font-weight: normal;
  font-style: normal;
}

body {
  font-family: "archialight";
  height: 100vh;
  overflow: hidden;
  color: #464646;
  user-select: none; /* supported by Chrome and Opera */
  -webkit-user-select: none; /* Safari */
  -khtml-user-select: none; /* Konqueror HTML */
  -moz-user-select: none; /* Firefox */
  -ms-user-select: none; /* Internet Explorer/Edge */
}

body.game {
  background-color: #f3f6f7;
}

body.menu {
  background-color: black;
}

.text-center {
  text-align: center !important;
}

.disable-dbl-tap-zoom {
  touch-action: manipulation;
}

.container {
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
}

h1 {
  margin-block-start: 0;
  margin-block-end: 0;
}

.modal {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1050;
  display: none;
  overflow: hidden;
  outline: 0;
}
.modal.fade .modal-dialog {
  transition: -webkit-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
  transition: transform 0.3s ease-out, -webkit-transform 0.3s ease-out;
  -webkit-transform: translate(0, -50px);
  transform: translate(0, -50px);
}

.modal-backdrop {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1040;
  width: 100vw;
  height: 100vh;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
}
.modal-backdrop.show {
  opacity: 0.5;
}

@media (min-width: 576px) {
  .container {
    max-width: 540px;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 960px;
  }
}

@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}
</style>
