<script lang="ts">
   /*
   Projects
ML
   - prerna boutique
   - suno

   */



</script>

<div id="showcase">
   <div class="section">
      <h2 class="title">WORK</h2>
      <p>I've worked at
         <a target="_blank" href="https://www.linkedin.com/company/giden">Giden</a>,
         <a target="_blank" href="https://www.linkedin.com/company/giden">Acrylic Robotics</a>,
         <a target="_blank" href="https://www.loftorbital.com/">Loft Orbital</a>,
         <a target="_blank" href="https://www.walmart.ca/">Walmart</a>, and
         <a target="_blank" href="https://www.wealthsimple.com/en-ca/">Wealthsimple</a>
       </p>
      <p>Currently, you can find me at <a target="_blank" href="https://www.glossgenius.com/">GlossGenius</a>.</p>
   </div>

   <div class="section">
      <h2 class="title">PLAY</h2>
      <div class="container">
         <div class="item" >
            <img src="/Screen Shot 2023-06-14 at 8.55.49 PM.png" alt="" />
            <p><b>Spaceshots:</b> A space platformer based around the concept of gravity assists inspired by a tech demo made to teach elementary students science concepts. Made with Python with a custom physics engine. </p>
         </div>
         <div class="item" >
            <img src="/Screen Shot 2023-06-14 at 9.28.13 PM.png" alt="" />
            <p><b>Aaja: </b>An app made during COVID to help you and your friends find movies to watch and places to eat, together.</p>
         </div>
         <div class="item" >
            <a href="https://drive.google.com/file/d/1iG9m5AOaalxmbYr9JIcqRNYNVHWAuSyK/view" target="_blank" ><img src="https://lh3.googleusercontent.com/u/0/drive-viewer/AFGJ81ryPXAdGx5xenksGEDHGB1NIR82lwX7vdE9eNlFd8bsmCG1oDXqKaMZ724xrIVNUcLpUNBgD2xJDZLITzLOvXRjKq6o=w1920-h1080-k-pd" alt=""/></a>
            <p><b>Autonomous Robot: </b>A maze-solving robot made with Arduino and couple servo motors. Controlled with a custom Python algorithms over Bluetooth. Used multiple ultrasonic sensors to localize instantly.</p>
         </div>
         <!-- <div class="item" >
            <a href="https://drive.google.com/drive/u/0/folders/1Vsq7JVfx6SJh3gYwWaH1i021K_GzKL9q" target="_blank" ><img src="/Screen Shot 2023-06-14 at 9.51.44 PM.png" alt="" /></a>
            <p><b>Table Tennis Bot</b>A robotic arm trainined with custom simulaton using Blender for physics engine. Used OpenAI Gym with Policy gradients to train a neural net with reinforcement learning.</p>
         </div> -->
      </div>
   </div>

   <div class="section">
      <h2 class="title">ML</h2>
      <div class="container">
         <div class="item" >
            <img src="/Screen Shot 2023-06-14 at 9.59.48 PM.png" alt="" />
            <p><b>Vibify:</b> Web app to let you feed in your entire Spotify library and output pre-made playlists by segmenting songs in similar clusters using hierarchical clustering on a custom FastAPI backend.</p>
         </div>
         <div class="item" >
            <a href="https://suno.chat/" target="_blank" ><img src="/Screen Shot 2023-06-14 at 10.04.01 PM.png" alt="" /></a>
            <p><b>Suno: </b>An app currently being developed using the advancements of LLM's to create a smart journal with an integrated chatbot to explore your feelings.</p>
         </div>
         <div class="item" >
            <a href="https://medium.com/@baetia/creating-a-birthday-present-as-an-engineer-f2a7affe8484" target="_blank" ><img src="https://miro.medium.com/v2/resize:fit:3792/format:webp/1*O9ROQ7OXNyX318s4kSjNdw.png" alt="" /></a>
            <p><b>Prerna's Boutique: </b>A web app created for my partner to help her shop multiple online retailers at once by presenting all items in one place. A recommender system was built using cosine similarity where each product was vectorized based on skin coverage of the dress, price, and description keywords.</p>
         </div>
         <div class="item" >
            <a href="https://drive.google.com/drive/u/0/folders/1Vsq7JVfx6SJh3gYwWaH1i021K_GzKL9q" target="_blank" ><img src="/Screen Shot 2023-06-14 at 9.51.44 PM.png" alt=""/></a>
            <p><b>Table Tennis Bot: </b>A robotic arm trained with a custom simulator using Blender for the physics engine. Used OpenAI Gym with Policy gradients to train a neural net with reinforcement learning.</p>
         </div>
      </div>
   </div>
</div>

<style>
   @import url("https://fonts.googleapis.com/css2?family=Damion&display=swap");
   #showcase {
      /* min-height: 100vh; */
      display: flex;
      padding: 30px 10vw;
      background: #ffd516;
      flex-direction: column;
   }

   /* .section {
      /* display: flex; */
      /* flex-direction: column; */
   /* }  */

   .section p {
      /* font-family: "Helvetica"; */
      font-size: 2rem;
      padding-left: 2%;
   }

   .title {
      font-family: "Damion", cursive;
      color: #000;
      font-size: 8rem;
      font-weight: bold;
      rotate: -8deg;
      margin-top: 0;
      margin-bottom: clamp(60px, 10vw, 100px);
   }


   img {
      border-radius: 30%;
      /* min-width: 300px; */
      width: clamp(300px, 50vw, 500px);
      aspect-ratio: 16/9;
      object-fit: cover;
   }

   .container {
      display: flex;
      align-items: stretch;
      flex-direction: column;
      flex-wrap: wrap;
      justify-content: space-between; /* or any other value that suits your layout needs */
   }

   .item {
      display: flex;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      flex-basis: calc(100% / 2); /* adjust this to the desired width per item */
   }
   .item img {
      margin-bottom: 10px;
   }

   @media (min-width: 600px) {
      .container {
      flex-direction: row;
   }
   
   }

</style>