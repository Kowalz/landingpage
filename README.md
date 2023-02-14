<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nnanenene</title>
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link
    href="https://fonts.googleapis.com/css2?family=Montserrat:wght@900&family=Open+Sans:ital,wght@0,400;0,700;1,400&display=swap"
    rel="stylesheet">
  <link rel="stylesheet" href="css/styles.css">
  <style>
  :root{
    --primary-color: #0A1128;
    --white-color: #FFFFFF;
    --light-gray-color:#eeee;
    --secondary-color:lightgreen;
    --gap: 3rem;
  }
  
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  html {
    font-size: 62.5%;
    scroll-behavior: smooth;
  }
  
  body {
    font-family: 'Open Sans', sans-serif;
    font-size: 2rem;
    color: var(--primary-color);
    line-height: 1.5;
  }
  
  h1, h2, h3, h4, h5, h6 {
    font-family: 'Montserrat', sans-serif;
  }
  

  h1 {
    font-size: 6rem;
    text-transform: uppercase;
  }
  
  h2 {
    font-size: 5.5rem;
  }
  
  h3 {
    font-size: 5rem;
  }
  
  h4 {
    font-size: 4.5rem;
  }
  
  h5 {
    font-size: 4rem;
  }
  
  h6 {
    font-size: 3.5rem;
  }
  
  .main-bg {
    background-image: url('../Image/scattered-forcefields.svg');
    background-size: cover;
    background-position: center center;
    color: var(--white-color);
  }
  
  .white-bg {
    background: var(--white-color);
    color:var(--primary-color)
  }
  
  .main-content {
    max-width: 120rem;
    margin: 0 auto;
    padding: 10rem var(--gap);
  }
  
  a {
    text-decoration: none;
  }
  .section {
    min-height: 100vh;
  }
  .menu {
    
    position: fixed;
    top:0;
    right:0;
    left:0;
    width:100%;
    border-bottom: 0.1rem solid var(--light-gray-color);
    z-index: 1; 
  }
  .menu-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 0;
    padding-bottom: 0;
  }

  .menu ul  {
    list-style:none;
    display: flex;
    
  }

  

    .menu ul li a {
        display: block;
        padding: 2rem;
        font-size: 1.8rem;
        color: var(--primary-color);
        position: relative;
      }
  
   h1 {
    font-size: 2.3rem;
    color:var(--primary-color)
   }

   .menu h1 a {
    color: inherit;
    text-decoration:none;
   }

   .menu ul li a::after {
    content: '';
    bottom: 1rem;
    position: absolute;
    left:50%;
    width: 0;
    height:0.2rem ;
    
    background-color:var(--secondary-color);
    transition: all 300ms ease-in-out;

    
  }
  .menu ul li a:hover:after {
    width: 50%;
    left:25%;
  }
  .menu-spacing {
    height: 6.4rem;
  }

  .intro-content {
    position:relative;
    /*top:-8rem; */
    display: grid;
    grid-template-columns: 1fr 1.5fr;
    gap:var(--gap);
    min-height: 100vh;
  }
  .intro-text-content , .intro-img {
    display:flex ;
    flex-flow: column wrap;
    justify-content: center;

  }
  .intro-text-content h2 {
    font-size: 6rem;
    margin-bottom: 5rem;
    text-transform: uppercase;
    line-height: 1.2;
  }
  .intro-img img {
    max-width: 100%;
    height: auto;
  }

  .top3-content {
    max-width: 64rem;
    height: 100vh;
    display:flex;
    min-height: 100vh;
    flex-direction: column;
    flex-wrap: nowrap;
    justify-content: center;
    text-align: center;

  }
  
  p{
    margin-bottom: 3rem;
  }

  .grid-one-content {
    display: flex;
    flex-flow: column wrap;
    justify-content: center;
    min-height: 100vh;
  }

  .grid-main-heading {
    margin-bottom: 1rem;
  }

  .grid-description {
    padding-bottom: 5rem
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: var(--gap);
    counter-reset: grid-counter;
  }
  .grid h3 {
    font-size: 3rem;
    position: relative;
    padding-left: 5rem;
    padding-bottom: 3rem;
  }

  .grid h3::before {
    counter-increment: grid-counter;
    content: counter(grid-counter);
    position: absolute;
    font-size: 8rem;
    font-style: italic;
    top: -4rem;
    left: -2rem;
    transform: rotate(5deg);
  }

  .gallery-img {
    width: 100%;
    max-width: 36rem;
    max-height: 36rem;
    overflow: hidden;
  }

  .gallery-img img {
    transition:  all 300ms ease-in-out;
  }

  .gallery-img img:hover {
    transform: translate(-3%,3%) scale(1.2) rotate(5deg);
  }

  .responsive-table{
    overflow: hidden;
    overflow-x: auto;
    

  }

  table {
    min-width: 360px;
    width: 100%;
    border-collapse: collapse ;
  }

  table caption {
    font-style: italic;
    font-size: 1.6rem;
    text-align: left;
    margin-bottom: 1rem;
  }


  table td , table th {
    white-space: nowrap;
    padding: 1rem;
    text-align: left;
    border: 0.1rem solid var(--light-gray-color);
  }

  tfoot td ,  table th{
    background-color: var(--light-gray-color);

  }
  .contact-form {
    grid-column: span 2;

  }
  .contact-form .form-grid {
    border:none;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap:var(--gap);
  }
  .form-group {
    
  flex: 1 1 320px;
  }
  .form-grid legend {
    font-style: italic;
    font-size: 1.6rem;
    margin-bottom: 3rem;
  }

   .form-group input:focus , .form-group textarea:focus
   {
   box-shadow: 0 0 10px 2px var(--secondary-color);
  }



  .form-group label {
    display: block;
    margin-bottom: 1rem;
  }
  .form-group input , .form-group textarea {
    border: none;
    background-color: var(--white-color);
    padding: 1.5rem 2rem;
    width: 100%;
    font-size: 3rem;
    outline: none;
  }
  
  .full-width {
    width: 100%;
    flex: 1 1 100%;
  }
  .form-group  button {
    border: 0.5rem solid  var(--white-color);
    background: none;
    color: var(--white-color);
    padding: 1.5rem 2rem;
    font-size:3rem;
    cursor: pointer;
    transition: all 300ms ease-in-out;
  }
  .form-group button:hover {
    background-color: var(--white-color);
    color: var(--primary-color ); 
}

.form-group ::placeholder{
    color: var(--light-gray-color);
}
.footer a {
    color: var(--primary-color) ;
}
.footer {
    text-align: center;
    font-size: 1.6rem;
}
footer p {
    margin: 0;
padding: 3rem;}

.close-menu {
  display: none;
  
}



.back-to-top {
  position: fixed;
  bottom: 2rem;
  right: 2rem;
  background: var(--white-color);
  width: 5rem;
  height: 5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  color: var(--primary-color);
  transform: rotate(-90deg);
  border: 0.1rem solid var(--primary-color);
}


@media (max-width:800px) {
  .intro-content ,.grid {
    grid-template-columns: 1fr;
  }

  .gallery-img{
    width: 100%;
    max-width: auto;
    max-height: auto ;
  
  }
 .gallery-img img {
  width: 100%;
 }
 .grid-one-content {
  display: block;
 }
 .menu {
  bottom: 0;

  display: none;
 }
 .menu-content , .menu-content ul{
  flex-direction: column;
  justify-content: center;
}

  .menu-content {
    height: 100vh;
  }

  .close-menu {
    display: none;
  }
  
  .close-menu-label::after {
    content: '≡';
    position: fixed;
    z-index:2;
    top: 2rem;
    right: 2rem;
    background-color: var(--primary-color);
    color: var(--white-color);
    font-size: 3rem;
    line-height:3rem;
    width: 3rem;
    height: 3rem;
    text-align:center;
    padding: 0.5rem;
    cursor: pointer;}

    .close-menu:checked~.menu {
      display: block;
    }

    .close-menu:checked~.close-menu-label::after{
      content: '×';
    } 

    .menu-spacing {
      display: none;
    }
 



}

  </style>
</head>

<body >
    <input id="close-menu" class="close-menu" type="checkbox" aria-label="Close menu" role="button">
  <label class="close-menu-label" for="close-menu" title="close menu"></label>
    

    <aside class="menu white-bg">
        <div class="main-content menu-content">
          <h1 onclick="getElementById('close-menu').checked = false;">
            <A href="#home" >Kowalskii</A>
        </h1>
        <NAV>
            <ul onclick="getElementById('close-menu').checked = false;">
                <li><a href="#intro">Intro</a></li>
                <li><a href="#grid-one">GridOne</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#grid-two">GridTwo</a></li>
                <li><a href="#Pricing">Pricing</a></li>
                <li><a href="#Contato"> Contato</a></li>
            </ul>
        </NAV>
    </div>
</aside>
<div class="menu-spacing"></div>

<section id="home" class =" intro main-bg section ">
    <div class="main-content intro-content">
    <div class="intro-text-content">
    <h2>Lorem Bitcoin Jobs UP or DOWN?</h2>
    <p>Um produto personalizado será composto de escolhas do cliente:
         cores, modelos, detalhes, dizeres, medidas, estampas, materi
         al. O produto comum será idêntico para todos que optarem po
         r sua compra</p>
    </div>
    <div class="intro-img">
        <img src="Image/fotos.svg" alt="Logo de HTML,css , e js">
    </div>
</div>
</section>

<section id="intro" class ="white-bg section">
    <div class="main-content top3-content">
        <h2> Apple Silicon-based
            Macs</h2>
        <p>The release of Apple Silicon-based
             Macs at the end of last year gene
             rated a flurry of news coverage an
             d some surprises at the machine’s pe
             rformance. This post details some back
             ground information on the experience of po
             rting Firefox to run natively on these CPUs.</p>
             <p>
             We’ll start with some background on the Mac tra
             nsition and give an overview of Firefox internals 
             that needed to know about the new architecture, 
             before moving on to the concept of Universal Binaries.
            </p>
            <p>We’ll then explain how DRM/EME works on the new platform,
                 t
                alk about our experience with macOS Big Sur, and discuss
                 various updater problems we had to deal with. We’ll con
                 clude with the release and an overview of various other im
                 provements that are in the pipeline.</p>
        
    </div>

</section>

<section id="grid-one" class="grid-one main-bg section">
    <div class="main-content grid-one-content">
      <h2 class="grid-main-heading">My Grid</h2>
      <p class="grid-description">Here are some recent work.</p>

    <div class="grid"> 

        <article>
            <H3>First</H3>
    <p>Lorem ipsum dolor sit amet cons
        ectetur, adipisicing elit. Incidunt 
        placeat voluptas nostrum recusandae
         a amet corporis quae cum illum nobis
          assumenda ea, magnam deleniti odio aspe
          riores praesentium, nam eos molestias!</p>
          </article>
          <article>
            <H3>Another site</H3>
          <p>Lorem ipsum dolor sit amet cons
            ectetur, adipisicing elit. Incidunt 
            placeat voluptas nostrum recusandae
             a amet corporis quae cum illum nobis
              assumenda ea, magnam deleniti odio aspe
              riores praesentium, nam eos molestias!</p>
            </article>

            <article>
                <H3>Another site </H3>
              <p>Lorem3 ipsum dolor sit amet cons
                ectetur, adipisicing elit. Incidunt 
                placeat voluptas nostrum recusandae
                 a amet corporis quae cum illum nobis
                  assumenda ea, magnam deleniti odio aspe
                  riores praesentium, nam eos molestias!</p>
                </article>
       
            </div>

</div>
</section>

<section id="gallery" class="grid-one white-bg section">
    <div class="main-content grid-one-content">
      <h2 class="grid-main-heading">Gallery</h2>
      <p class="grid-description">Here are some of my pics.</p>

    <div class="grid"> 

        <div class="gallery-img">
       <img src="https://source.unsplash.com/random/360x360?=r1"
             alt="random image from unsplash">
        </div>
        <div class="gallery-img">
            <img src="https://source.unsplash.com/random/360x360?=r2"
             alt="random image from unsplash">
             </div>
         <div class="gallery-img">
                <img src="https://source.unsplash.com/random/360x360?=r3"
             alt="random image from unsplash">
         </div>
         <div class="gallery-img">
            <img src="https://source.unsplash.com/random/360x360?=r4"
         alt="random image from unsplash">
     </div>
     <div class="gallery-img">
        <img src="https://source.unsplash.com/random/360x360?=r5"
     alt="random image from unsplash">
 </div>
 <div class="gallery-img">
    <img src="https://source.unsplash.com/random/360x360?=r6"
 alt="random image from unsplash">
</div>
</div>
</div>
</section>

<section id="grid-two" class="grid-one main-bg section">
    <div class="main-content grid-one-content">
      <h2 class="grid-main-heading">JOBS</h2>
      <p class="grid-description">Here are some recent work.</p>

    <div class="grid"> 

        <article>
            <H3>A good one</H3>
    <p>Lorem ipsum dolor sit amet cons
        ectetur, adipisicing elit. Incidunt 
        placeat voluptas nostrum recusandae
         a amet corporis quae cum illum nobis
          assumenda ea, magnam deleniti odio aspe
          riores praesentium, nam eos molestias!</p>
          </article>
          <article>
            <H3>The goat</H3>
          <p>Lorem ipsum dolor sit amet cons
            ectetur, adipisicing elit. Incidunt 
            placeat voluptas nostrum recusandae
             a amet corporis quae cum illum nobis
              assumenda ea, magnam deleniti odio aspe
              riores praesentium, nam eos molestias!</p>
            </article>

            <article>
                <H3>The best </H3>
              <p>Lorem ipsum dolor sit amet consectetu
                r, adipisicing elit. Quibusdam perferen
                dis nisi omnis culpa eius optio eos invent
                ore rerum? Harum velit consectetur tempora e
                t numquam distinctio vero exercitationem moll
                itia laborum inventore?</p>
                </article>
       
            </div>

</div>
</section>

<section id="Pricing" class ="white-bg section">
    <div class="main-content top3-content">
        <h2>Pricing
        </h2>
        <p>The release of Apple Silicon-based
             Macs at the end of last year gene
             rated a flurry of news coverage an
             d some surprises at the machine’s pe
             rformance. This post details some back
             ground information on the experience of po
             rting Firefox to run natively on these CPUs.</p>
             <p>The release of Apple Silicon-based
                ground information on the experience of po
                rting Firefox to run natively on these CPUs.</p>

             <div class="responsive-table">
             
             <table>
                <caption>Pricing Table</caption>
                <thead>
                    <tr>
                        <th> Titulo 1</th> 
                        <th> Titulo 2</th>
                        <th> Titulo 3</th>
                        <th> Titulo 4</th>         
                        <th> Titulo 5</th>            
                    </tr>              
                </thead>
                <tbody>
                    <tr>
                    <td> Content 1</td> 
                   <td> Content 2</td> 
                    <td> Content 3</td>
                    <td> Content 3</td>
                    <td> Content 3</td>        
  </tr>
     <tr>
          <td> Content 1</td> 
         <td> Content 2</td> 
        <td> Content 3</td>
        <td> Content 3</td>
        <td> Content 3</td>
                           
    </tr>
    <tr>
        <td> Content 1</td> 
       <td> Content 2</td> 
      <td> Content 3</td>
      <td> Content 3</td>
      <td> Content 3</td>                        
  </tr>                      
                </tbody>
                <tfoot>
                    <tr>
                        
                     <td> </td>
                     <td> </td>
                     <td> </td>
                     <td> </td>
                     <td> Testando</td>
                    </tr>
                </tfoot>
            </table>
        </div>
    </div>
</section>

<section id="Contato" class =" intro main-bg section ">
    <div class="main-content intro-content">
    <div class="intro-text-content">
    <h2>CONTACT US</h2>
    <p>To wrap up January, we are proud to
         bring you the release of Firefox 85.
          In this version we are bringing you s
          upport for the :focus-visible pseudo-c
          lass in CSS and associated devtools, an
          d the complete removal of Flash support 
          from Firefox.</p>
    </div>
    <div class="intro-img">
        <img src="Image/gato.svg" alt="Logo de HTML,css , e js">
    </div>
    <div class="contact-form">
    <fieldset class="form-grid">
        <legend> Contact me</legend>
        <div class="form-group">
            <label for="First-name">Primeiro Nome:</label>
            <input type="text" name="first-name" id="first-name"
             placeholder="Seu Nome">
        </div>
        <div class="form-group">
            <label for="last-name">Sobrenome:</label>
            <input type="text" name="last-name" id="last-name"
            placeholder="Seu Sobrenome">
        </div>
        <div class="form-group Arruma-one">
            <label for="email">Email:</label>
            <input type="email" name="email" id="email"
            placeholder="Ex: unknown@gmail.com">
        </div>
        <div class="form-group full-width">
            <label for="message">Descrição:</label>
            <textarea name="message" id="message" cols="30" rows="10" placeholder="Seu Desejo Magestade"></textarea>
            
        </div>
        <div class="form-group full-width">
            <button type="submit">Enviar</button>
        </div>


            

    
    </fieldset>
</div>

</section>

 <footer  id="footer" class="footer white-bg">
    <P><A  rel="nofolllow " target="_blank" href="https://www.instagram.com/pedroks.pks/">Make By Kowalz </A></P>
 </footer>
 
 <a class="back-to-top" href="#">➤</a>

</body>


</html>
