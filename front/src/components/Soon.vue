<template>
  <div class="soon">
    <h1>Przepraszamy, strona dopiero powstaje!</h1>
    <div class="working-dog">
      <img src="../assets/img/working-dome.png" />
    </div>
    <button type="button" @click="$emit('changePage', 0)">Strona główna</button>
  </div>
</template>

<style scoped>
.soon {
  font-family: "Nunito", sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 128px;
}
h1 {
  font-weight: 700;
  font-size: 2.6rem;
  color: #495f7a;
  text-align: center;
}

button {
  width: 30%;
  border-radius: 15px;
  padding: 20px 0px;
  border: 1px solid #b3bcc7;
  background: none;
  color: #495f7a;
  font-weight: 700;
  font-size: 1.4rem;
  cursor: pointer;
  transition: color 0.75s, background-color 0.75s;
  margin-bottom: 150px;
}
button:hover {
  color: white;
  background: #495f7a;
  transition: color 0.75s, background-color 0.75s;
}
@media (max-width: 768px) {
  button {
    width: 90%;
  }
}
@media (hover: none) {
  button {
    color: white;
    background: #495f7a;
    transition: color 0.75s, background-color 0.75s;
  }
}
</style>
<script>
export default {
  name: "Soon",
};
</script>
