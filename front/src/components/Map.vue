<template>
  <div class="map">
    <div class="map__content">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2451.219702490395!2d15.721748999999999!3d52.09393299999999!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xbe104b3b26fda304!2zNTLCsDA1JzM4LjIiTiAxNcKwNDMnMTguMyJF!5e0!3m2!1spl!2spl!4v1673198519814!5m2!1spl!2spl"
        style="border: 0; border-radius: 14px; width: 100%; height: 500px"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
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
li{
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom: 16px;
    cursor: pointer;
}
@media (max-width: 992px) {
  .map{
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
    };
  },
  methods: {
    changeChords(cord) {
      console.log(cord);
    },
  },
};
</script>
