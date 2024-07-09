<script>
export default {
    data() {      //原型長 => data:function()
        return {
            test: "This is Text Code!!!",
            modelTxt: "",  //要給空值
            modelRadio:"",
            modelCheck:[],
            modelSelect:"",

        }
    }

    
}

</script>


<template>
    <!-- v-test -->
    <p v-text="this.test"></p> <!-- 功能一樣 -->
    <p>{{ this.test }}</p>

    <p v-text="'使用單引號表示字串'"></p>

    <!-- v-model -->
    <!-- 標籤的值與變數雙向綁定 -->
    <input type="text" v-model="this.modelTxt">
    <h3>與 v-model綁定的變數:{{ this.modelTxt }}</h3>

    <!-- 單選 -->
     <label for="cool1">酷1</label>
     <input type="radio" id="cool1" v-model="this.modelRadio" value="這是酷酷1" name="coolGr">
     <label for="cool2">酷2</label>
     <input type="radio" id="cool2" v-model="this.modelRadio" value="這是酷酷2" name="coolGr">
     <label for="cool3">酷3</label>
     <input type="radio" id="cool3" v-model="this.modelRadio" value="這是酷酷3" name="coolGr">
     <h3>您選擇：{{ this.modelRadio }}</h3>

     <!-- 複選 -->
      <label for="meat1">肉1</label>
      <input type="checkbox" name="meat" id="meat1" v-model="this.modelCheck" value="魚肉">
      <label for="meat2">肉2</label>
      <input type="checkbox" name="meat" id="meat2" v-model="this.modelCheck" value="雞肉">
      <label for="meat3">肉3</label>
      <input type="checkbox" name="meat" id="meat3" v-model="this.modelCheck" value="豬肉">
      <h3>您選擇：{{ this.modelCheck }}</h3>

      <!-- 下拉式選單 -->
       <select name="" id="" v-model="this.modelSelect">
        <option value="">請選擇</option>
        <option value="Tea">茶克拉</option>
        <option value="Coffee">嘎裡還式咖啡</option>
        <option value="Milk">牛奶</option>
       </select>
       <h3>您選擇：{{ this.modelSelect }}</h3>

</template>



<style></style>
