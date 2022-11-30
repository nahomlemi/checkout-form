<template>
  <div class = "container">
    <h1 class = "header"> Checkout Form </h1>

    <div class = "info">

      <div class = "name">
        <div class = "firstName">
          <label>First Name:</label><br>
          <input type = "text" required/>
        </div>
        <div class = "lastName">
          <label>Last Name</label>
          <input type = "text" required/>
        </div>
      </div>
      
      <div>
        <label>e-mail:</label>
        <input type = "email" required v-model = "email"/>
      </div>
      <div>
        <label>Password:</label><br>
        <input type = "password" requred v-model = "password"/>
      </div>

    </div>

    <div>
      <select v-model = "option">
        <option>Regular </option>
        <option>Pro </option>
      </select>
    </div>
  
    <label>Review</label><br>
    <textarea type = "text" class = "review">enter your review.
    </textarea>

    <div class = "buttons">
      <button class = "confirm">Confirm</button>
      <button class = "cancel">Cancel</button>
    </div>
    
  </div>
</template>

<script>
export default {
  data(){
    return {
      email:"",
      password:"",
      option:""
    }
  }
}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@500&display=swap');

.container{
width:450px;
padding: 20px 10px 50px 10px;
background: white;
border-radius: 60px;
margin: 30px auto;
}
label {
color:#aaa;
}
.header{
  color: #808080;
  font-family: 'IBM Plex Mono', monospace;
}
.name{
display:flex;
justify-content:space-around;
}
label {
margin-bottom: 10px;
}

input, select{
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  border-radius: 10px;
  color: #555;
  margin-bottom: 20px;
}

.buttons{
padding:10px;
}
.buttons button{
border :0;
padding:15px 25px;
margin:10px;
border-radius:10px;
}
.confirm{
color:white;
background:#0b6dff;
}
.review{

background: #eee;
border: 0;
border-radius: 15px;
width: 300px;
height: 100px;
}

</style>
