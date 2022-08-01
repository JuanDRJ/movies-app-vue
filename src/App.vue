<template>

  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <h1>{{msg}}</h1> -->
  <link rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />

  <body>

   <div class=".body">
     <div class="grid-container">
       <header class="header">
         <a>
           <img class="logo-header"
             src="https://static.platzi.com/media/user_upload/logo-d871d30b-ac23-4240-93f3-13e49084d80b.jpg" alt="">
         </a>
         <div class="search">
           <span class="material-symbols-outlined">search</span>
           <input type="text" placeholder="Busca las mejores películas...">
         </div>
         <div class="right-profile">
           <span>Bambi Rodriguez</span>
           <img src="https://cdn-icons-png.flaticon.com/512/80/80889.png" alt="">
           <select>
             <option value="" disabled selected></option>
             <option value=""> Acción</option>
             <option value=""> Terror </option>
             <option value=""> Aventura</option>
           </select>
         </div>
       </header>
       <div class="sidebar">
         <div class="sidebar-icons">
           <a href="">
             <img class="home-img" src="./assets/pinpng.com-home-images-png-118886.png" alt="">
             <p>Home</p>
           </a>
    
           <a href="">
             <img class="home-img" src="./assets/toppng.com-transparent-fire-white-flame-icon-white-350x447.png" alt="">
             <p>Trending</p>
           </a>
    
           <a href="">
             <img class="home-img" src="./assets/heart-5-64.png" alt="">
             <p>Mas likes</p>
           </a>
    
           <div class="settings">
             <a href="">
               <img class="home-img-end"
                 src="https://icon-library.com/images/white-settings-icon/white-settings-icon-0.jpg" alt="">
               <p>Ajustes</p>
             </a>
           </div>
    
         </div>
       </div>
       <div class="main">
         <h3>Ahora en Cines</h3>
         <div class="movies">
    
           <div class="container">
            <img class="movie-img" src="https://images.thedirect.com/media/article_full/star-wars-next-movie_1.jpg"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://www.filmsnewsfeed.com/images/article/12-best-movies-about-magic-ever-made-article-image6.webp"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://assets.mubicdn.net/images/film/89619/image-w448.jpg?1445906907"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
         </div>
    
         <h3>Aclamadas por la crítica</h3>
         <div class="movies">
    
           <div class="container">
            <img class="movie-img" src="https://www.themoviedb.org/t/p/w250_and_h141_face/6U2B92g8Zp6iVQljD8PP27iBMAH.jpg"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://www.filmcompanion.in/wp-content/uploads/2021/05/FC_-Koi-Jaane-Na.jpg"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://img.buzzfeed.com/buzzfeed-static/static/2018-09/13/10/enhanced/buzzfeed-prod-web-03/enhanced-11213-1536850713-2.jpg?output-format=jpg&output-quality=auto"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
         </div>
         <h3>No te debes perder</h3>
         <div class="movies">
    
           <div class="container">
            <img class="movie-img" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQquLzVerHLR1XxaKXWpH8dcEAds9pb_q8vYg&usqp=CAU"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://www.worldoffemale.com/wp-content/uploads/2011/04/image-0071.jpg"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
           <div class="container">
            <img class="movie-img" src="https://www.indiewire.com/wp-content/uploads/2020/09/Screen-Shot-2020-09-22-at-8.42.54-AM.png"
              alt=""><div class="overlay"><div class="text">STAR WARS <br> La aventura del Jedi</div> </div>
           </div>
         </div>
       </div>
     </div>
   </div>
  </body>

</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      msg: "Helou World¿d",
    }
  },
  components: {
    
  }
}

</script>

<style>
*{
  font-family: 'roboto';
  color: rgb(51, 51, 51);
  margin:0px;
  padding: 0px;
  box-sizing: border-box;
  max-width: 100vw;
  
}

html{
  height: 100%;
}
.body{
  min-height: 100%;
  display: flex;
  justify-content: center;
}
.grid-container > * {
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px;
  text-align: center;
  padding: 10px;
}
.grid-container{
  display: grid;
  grid-template-columns:100%;
  gap: 5px;
  width: 98vw;
  height: 100vh;
  grid-template-columns: 110px auto;
  grid-template-rows: 60px auto;
  grid-template-areas:
        "header   header"
        "sidebar  main"
      ;
  
}
.header{
  background: rgb(255, 255, 255);
  grid-area: header;
  display:flex;
  flex-direction: row;
  justify-content: space-between;
  
}
.header input{
  width: 320px;
  border: none;
  padding: 10px;
  border-radius: 20px;
  color: gray;
  font-size: 15px;
  
}
.header input:focus{
  width: 450px;
  outline:none;
  transition: 500ms ease;
  
}

.search{
  display: flex;
  align-items: center;
  border: gray 1px solid;
  border-radius: 20px;
}

span{
  padding: 8px;
}
.logo-header{
  padding: 0px;
  margin-left: 30px;
}
.sidebar{
  background-image: linear-gradient(#FF535B, #fd7466);
  grid-area: sidebar;
}
.main{
  grid-area: main;
  background: rgb(255, 255, 255);
  display: flex;
  flex-direction: column;
 
}

.right-profile{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.right-profile img{
  width: 50px;
  padding: 2px;
  margin: 3px;
}

.right-profile span{
  padding: 5px;
}

select{
  width: 20px;
  border:none;
}

.sidebar-icons{
  display: flex;
  flex-direction: column;

}
.home-img{
  width: 50px;
  margin-top: 30px;
}

.home-img-end{
  width: 50px;
  margin-top: 200px;
}

a{
  text-decoration: none;
  color: white;
}
.sidebar p {
 color: white;
}
.settings{
  align-content:flex-end;
}

.sidebar img:hover{
  transition: 500ms ease;
  transform: rotate(20deg);
  transition-duration: 800ms;
}

.sidebar a:hover{
  color: rgb(235, 102, 102)
}

.main h3{
  text-align: left;
  margin-top: 10px;
  margin-left: 60px;
}
.movies{
  display: flex;
  justify-content: space-evenly ;
  margin-top: 10px;
}
.movie-img{
  margin-top: 10px;
  width: 280px;
  height: 158px;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: #070707;
}
.text {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
.container {
  position: relative;
  width:relative;
}

.container:hover .overlay {
  opacity: 0.8;
}
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

@media (max-width: 800px) {
  .grid-container{
  display: grid;
  grid-template-columns:100%;
  gap: 5px;
  width: 100vw;
  height: 100vh;
  grid-template-columns: 200px auto;
  grid-template-rows: 60px  80px auto;
  grid-template-areas:
        "header header"
        "sidebar sidebar"
        "main main"
      ;
  
}

.sidebar-icons{
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
}

.sidebar-icons img{
 margin: 0;
 width: 30px ;
 

}

.movies{
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-top: 10px;
}

.main h3{
  text-align: center;
  font-size: 30px;
  margin-top: 20px;
}
.movies img{
  width: 400px;
  height: 250px;
  margin: 0 auto;
}
.right-profile span{
  display: none;
}

.header input{
  width: 200px;
  border: none;
  padding: 10px;
  border-radius: 20px;
  color: gray;
  font-size: 15px;
  
}
}

.logo-header{
  margin:10px;
  width: 50px;
}

.header input:focus{
  width: 200px;
  outline:none;

  
}

</style>
