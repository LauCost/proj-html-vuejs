<template>
  <div>
    <div class="search">
      <i class="fas fa-search"></i>
      <input type="text" placeholder="Search..." />
    </div>
  </div>
</template>


<style lang="scss">
.search {
  display: flex;
  align-items: center;
  background-color: #f3f4f3;
  border: none;
  padding: 5px;
  border-radius: 50px;

  i {
    margin-left: 10px;
  }
  input {
    width: 300px;
    padding: 10px;
    border: none;
    border-radius: 50px;
    margin-left: 10px;
    background-color: #f3f4f3;
    font-size: 18px;
    color: #9ca7ab;
  }
}
</style>