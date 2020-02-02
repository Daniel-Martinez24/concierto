<template>
  <div
    class="map"
  >
    <div class="arriba">
      <h2>LUGAR DEL EVENTO</h2>
      <h1>Lienzo Charro “Los Tamaulipecos”</h1>
      <svg width="30" height="40" viewBox="0 0 30 40" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M13.4584 39.193C2.10703 22.7368 0 21.0479 0 15C0 6.7157 6.7157 0 15 0C23.2843 0 30 6.7157 30 15C30 21.0479 27.893 22.7368 16.5416 39.193C15.7966 40.2691 14.2033 40.269 13.4584 39.193ZM15 21.25C18.4518 21.25 21.25 18.4518 21.25 15C21.25 11.5482 18.4518 8.75 15 8.75C11.5482 8.75 8.75 11.5482 8.75 15C8.75 18.4518 11.5482 21.25 15 21.25Z" fill="white"/>
      </svg>
      <p>Las Fuentes Coloniales, #88703 Reynosa, Tamps.</p>
    </div>
    <no-ssr>
      <MglMap
        :access-token="Token"
        :map-style="mapStyle"
        :center="center"
        :zoom="zoom"
        @load="onMapLoaded"
      >
        <MglGeolocateControl ref="geolocateControl" />
      </MglMap>
      </no-ssr>
  </div>
</template>

<script>
export default {
  data () {
    return {
      Token: 'pk.eyJ1IjoiZGFuaWVsbWFydGluZXoyNCIsImEiOiJjazYzdG1mZnEwZHV4M21wOTU4dmpjY25jIn0.5xxPgyy2muUHlgrhHXZQ4A',
      mapStyle:  'mapbox://styles/mapbox/dark-v10',
      center: [-98.3121804, 26.0523096],  
      zoom: 15
    }
  }
}
</script>

<style scoped>
.map {
  position: relative;
  color: #fff;
  width: 100vh;
}
.map h2 {
  position: absolute;
  z-index: 10;
  left: 40%;
  top: 5%;
}
.map h1 {
  position: absolute;
  z-index: 10;
  left: 39%;
  top: 10%;

  font-weight: normal;
  font-size: 18px;
  line-height: 21px;
}
.map p {
  position: absolute;
  z-index: 10;
  left: 37%;
  top: 90%;

  font-weight: normal;
  font-size: 18px;
  line-height: 21px;
}
.map svg {
  position: absolute;
  z-index: 10;
  left: 45%;
  top: 47%;

}
</style>
