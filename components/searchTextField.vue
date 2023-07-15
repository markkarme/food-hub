
<template>
  <div class="search">
    <input placeholder="Search..." type="text" />
    <button type="submit"><v-icon size="25">mdi-magnify</v-icon></button>
  </div>
</template>
<script>
export default {
    name:"SearchTextField"
}
</script>
<style scoped>
.search {
  display: inline-block;
  position: relative;
  background: #fff;
}

.search input[type="text"] {
  width: 600px;
  padding: 10px;
  border: 1px solid black;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.search button[type="submit"] {
  background-color: red;
  border: none;
  color: #fff;
  cursor: pointer;
  padding: 10px 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  position: absolute;
  top: 0;
  right: 0;
  transition: .9s ease;
}

.search button[type="submit"]:hover {
  transform: scale(1.1);
  color: rgb(255, 255, 255);
  background-color: red;
}

</style>