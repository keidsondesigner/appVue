<template>
  <form>
    <div class="single-div__input">
        <input type="number" class="input" id="nome" required>
        <label for="nome">{{ text }}</label>
        <span>{{ message }}</span>
    </div>
  </form>
</template>

<script>
  export default {
    props: {
      text: String,
      message: String,
  }
  }
</script>

<style  scoped>
form{
    width: 100%;
    max-width: 350px;
    padding: 2%;
}

.single-div__input{
    position: relative;
    margin: 30px 0;
}
.single-div__input label{
    position: absolute;
    bottom: 22px;
    left: 0;
    color: rgb(150,150,150);
    cursor: text;
    transition: 0.5s ease-in-out;
}

.input{
    width: 100%;
    padding: 5px;
    border: 0;
    border-bottom: 2px solid rgb(200,200,200);
    outline: 0;
    font-size: 16px;
    color: rgb(80,80,80);
    transition: 0.5s ease-in-out;
}

.input:focus,
.input:valid{
    border-bottom: 2px solid cornflowerblue;
}
.input:focus ~ label,
.input:valid ~ label{
    transform: translateY(-24px);
    font-size: 12px;
    /* color: cornflowerblue; */
}

span {
  color: #ff5575;
  font-size: 12px;
  font-style: italic;
}
</style>
