<template>
  <div>
    <div id='intro'>
      <img class="profilepic" src="@/assets/profilepic.png" alt="Profile Pic">
      <br>Hi, my name is Adam.
        <div id='introduction'>
          <br>I'm a ... 
          <br><div id="thingsIam"></div>
      </div>
    </div>
    <a target="_blank" href="https://www.linkedin.com/in/aleonard9/">
      <img class="logo" src="@/assets/linkedin_logo.svg" title="Linkedin">
    </a>
    <a target="_blank" href="https://github.com/ALeonard9">
      <img class="logo" src="@/assets/github_logo.svg" title="Github">
    </a>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
var thingsIam = ['full stack developer', 'cloud enthusiast', 'dog lover',
                   'board gamer', 'clevelander'
                  ];
var thingsString = thingsIam.join(' | ');
var placeHolder = 0;
var textAdder = setInterval(function(){
  document.getElementById("thingsIam").innerHTML += thingsString.charAt(placeHolder);
    if (++placeHolder == thingsString.length){
      clearInterval(textAdder);
    }
}, 100);
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.logo{
  height:12%;
  width:12%;
  margin: 2%;
  margin-top: 5%;
}
.profilepic {
  height: 200px;
  width: 200px;
  border-radius: 50%;
  padding: 10px;
  border-color: black;
  margin-top: 4%;
}
#intro {
  font-size:39;
  font-family: 'Podkova';
  font-weight: bold;
  margin-top: 2%;
}
</style>
