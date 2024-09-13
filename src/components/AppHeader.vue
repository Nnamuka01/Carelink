<template>
   <header class="heading">
      <div class="header-content">
         <h2>The only healthcare service you need</h2>
         <p>We are committed to improving the health and well-being 
         from specialized treatments to advanced medical equipment to 
         serve every Individual.</p>
         <div id="header-button">
            <a class="open" href="">Open a free account</a>
            <a class="providers" href="">For Providers</a>
         </div>
      </div>
      <div class="header-images">
         <img class="doc" src="../assets/images/Image 1.png" alt="A doctor smiling">
         <img class="doc" src="../assets/images/Image 2.png" alt="A nurse and a friend laughing">
         <img class="doc" src="../assets/images/Image 3.png" alt="A nurse and a newborn">
      </div>
   </header>
</template>

<style>
 .header-content {
/* Auto layout */
display: flex;
flex-direction: column;
align-items: center;
padding: 72px 72px 40px;
gap: 24px;
background: linear-gradient(180deg, #F5F9FF 0%, #C2D9FF 50%, rgba(245, 249, 255, 0) 75%);
border-radius: 40px;
height: 40vh;
}

.header-content p {
   color: #023584;
}

a {
   text-decoration: none;
}

#header-button {
   display: flex;
   align-items: center;
   gap: 20px;
}

.open {
   color: white;
   border: 1px;
   background-color: #0461f0;
   border-radius: 20px;
   padding: 10px;
   padding-inline: 20px;
}

.open:hover {
   background-color: #0056b3;
}

.providers {
   color: #000;
   border: 1px;
   border-radius: 20px;
   background-color: white;
   padding-inline: 10px;
   padding: 10px;
}

.providers:hover {
   background-color: #0056b3;
   color: white;
}

.header-images {
   display: flex;
   height: 140px;
   flex-direction: row;
   align-items: flex-start;
   gap: 10px;
   padding: 0px;
   justify-content: center;
}

.doc {
   height: 340px;
   width: 300px;
}


</style>