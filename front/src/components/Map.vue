<template>
  <div class="map">
    <div class="map__content">
      <iframe
        style="border: 0; border-radius: 14px; width: 100%; height: 500px"
        frameborder="0"
        scrolling="no"
        marginheight="0"
        marginwidth="0"
        :src=linkX()
      ></iframe
      ><br /><small
        ><a
          href="https://www.openstreetmap.org/?mlat=52.09376&amp;mlon=15.72320#map=18/52.09376/15.72319"
          >Wyświetl większą mapę</a
        ></small
      >
    </div>
    <div class="map__nav">
      <!-- <div class="edit">
        <img
          style="width: 100%; height: 100%"
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Edit_icon_%28the_Noun_Project_30184%29.svg/1024px-Edit_icon_%28the_Noun_Project_30184%29.svg.png"
        />
      </div> -->
      <div class="gps-name">{{ gpsName }}</div>
      <hr />
      <div class="cords-list">
        <ol>
          <li v-for="cord in cordsList" @click="changeChords(cord)">
            {{ cord }}
          </li>
        </ol>
      </div>
    </div>
  </div>
</template>

<style scoped>
.map {
  font-family: "Nunito", sans-serif;
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 600px;
}
.map__content {
  border-radius: 14px;
  height: 100%;
  width: 70vw;
  margin-left: 32px;
  margin-right: 8px;
}
.map__nav {
  border: 1px solid black;
  /* height: 100%; */
  width: 20%;
  margin-right: 32px;
  height: 300px;
  border-radius: 14px;
  padding: 16px 32px 16px 8px;
  position: relative;
}
.edit {
  position: absolute;
  top: 16px;
  right: 16px;
  cursor: pointer;
  width: 30px;
  height: 30px;
}
.gps-name {
  font-weight: 700;
  font-size: 1.5rem;
  padding-left: 8px;
  color: #495f7a;
}
li {
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 16px;
  cursor: pointer;
}
@media (max-width: 992px) {
  .map {
    flex-direction: column-reverse;
    margin: 32px;
  }
  .map__nav {
    width: 90%;
    margin: 0px;
    margin-bottom: 32px;
  }
  .map__content {
    width: 100%;
    padding: 0px;
  }
}
</style>

<script>
export default {
  data() {
    return {
      gpsName: "Psota",
      cordsList: [195916, 329268, 895079, 479932],
      markerX: '15.72319507598877',
      markerY: '52.09367337611854',
      link: "https://www.openstreetmap.org/export/embed.html?bbox=3.718823075294496%2C52.0923128122943%2C30.727561712265016%2C52.095205883526475&layer=mapnik&marker=",
      // link: "https://www.openstreetmap.org/export/embed.html?bbox=${mapY}.718823075294496%2C52.0923128122943%2C${mapX}.727561712265016%2C52.095205883526475&layer=mapnik&marker=",
    };
  },
  methods: {
    changeChords(cord) {
      console.log(cord);
    },
    linkX() {
      var mapLink=this.link+this.markerY+'%2C'+this.markerX
      return mapLink
    },
  },
};
</script>
