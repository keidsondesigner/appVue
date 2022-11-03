<template>
  <div>
    <button>{{text}}</button>
  </div>
</template>

<script>
  export default {
    props: {
    text: String
  }
  }
</script>

<style  scoped>
button {
  font-weight: 500;
  border: 0;
  border-radius: 3em;
  font-size: 14px;


  color: white;
  background-color: #41b883;
  padding: 12px 18px;

  cursor: pointer;
  display: inline-block;
  line-height: 1;

  transition: background 0.8s;
}

button:hover {
  background-color: #209b64;
  background-image: radial-gradient(circle, transparent 1%, #209b64 1%);
  background-position: center;
  background-size: 15000%;
}

button:active {
  background-color: #41b883;
  background-size: 100%;
  transition: background 0s;
}
</style>
