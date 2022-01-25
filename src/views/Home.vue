<template>
  <div class="home">

    <Section id="welcome" cols="7" >
      <div class="welcome">
        <div class="welcome-title">
          <h2 class="title">ENCUENTRA EL EMPLEO <span class="text-primary">PERFECTO PARA TI</span></h2>
          <p class="subtitle">Con tan solo un click.</p>
        </div>
        <div class="welcome-body">
          <p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nesciunt pariatur tempore eaque veritatis perferendis in ipsam labore enim. 
            Eius beatae delectus quidem ipsum rerum voluptate labore molestiae accusamus adipisci voluptatum? </p>
          <p class="subtitle text-primary text-end">Dinos que buscas?</p>
          <div class="d-flex end">
            <router-link to="#jobs" class="btn btn-primary">Empleos</router-link>
            <router-link to="#recruit" class="btn btn-ligth">Reclutar</router-link>
          </div>
        </div>
      </div>
      <img class="welcome-img" src="@/assets/img/welcome.svg" alt="">
    </Section>

    <Section id="about" cols="7" rows="3">
      <div class="about-title">
        <h2 class="title text-white">LOS MEJORES EMPLEOS Y <span class="text-primary d-block">EL MEJOR TALENTO</span></h2>
        <p class="subtitle text-white">en un solo lugar.</p>
      </div>
      <img class="about-img" src="@/assets/img/about.svg" alt="">
      <div class="about text-start">
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iusto facilis porro quia repellendus error, 
          ratione tempore non adipisci, ipsam aliquid sit. 
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iusto facilis porro quia repellendus error, 
          ratione tempore non adipisci, ipsam aliquid sit. 
          Ducimus quidem obcaecati exercitationem iusto libero alias blanditiis quibusdam?
        </p>
      </div>
    </Section>

    <Section id="jobs" cols="4">
      <div class="jobs-title"><h2 class="title text-white">EMPLEOS QUE <span class="text-primary">SE AJUSTAN A TUS NECECIDADES</span> .</h2></div>
      <img class="jobs-img" src="@/assets/img/jobs.svg" alt="">
      <div class="card">
        <h4 class="card-title">Cuáles son tus intereses?</h4>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut fugiat modi at, veritatis ea consequatur dolor beatae, 
          repellendus vero alias sed in molestias pariatur facere laudantium, doloremque tempora eligendi dolorem?</p>
        <router-link to="#contact" class="btn btn-primary">Aplica</router-link>
      </div>
    </Section>

    <Section id="recruit" cols="4">
      <h2 class="title">
        ENCUENTRA <span class="text-white">EL PERFIL PERFECTO</span> PARA TU EMPRESA
      </h2>
      <img class="recruit-img" src="@/assets/img/recruit.svg" alt="">
      <div class="card">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut fugiat modi at, veritatis ea consequatur dolor beatae, 
          repellendus vero alias sed in molestias pariatur facere laudantium, doloremque tempora eligendi dolorem?</p>
        <router-link to="#contact" class="btn btn-primary">Encuentra</router-link>
      </div>
    </Section>

    <Section id="contact" cols="2">
      <div class="contact-logo">
        <img src="@/assets/logo/logo-2.svg">
        <SocialLinks />
      </div>
      <div class="contact">
        <div class="contact-title">
          <h2 class="title">CONTACTANOS</h2>
          <p class="subtitle"> No te arrepentiras! </p>
        </div>
        <form class="contact-form">
          <div class="form-row">
            <label for="name">Nombre : </label>
            <input type="text" name="name">
          </div>
          <div class="form-row">
            <label for="mail">Correo : </label>
            <input type="email" name="mail">
          </div>
          <label class="textarea">Cuentos sobre ti!</label>
          <textarea name="" rows="10"></textarea>
        </form>
      </div>
    </Section>

  </div>
</template>

<script>
import Section from "../components/section/Section.vue";
import SocialLinks from "../components/nav/SocialLinks.vue";
export default {
  name: 'Home',
  components: {
    Section,
    SocialLinks
}
}
</script>

<style lang="scss">

#welcome, #about, #jobs, #recruit, #contact {
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

// --- Welcome ---

#welcome {
  // background-color: aqua;
  background-image: 
    url('../assets/img/fondo-1.svg');
  // clip-path: url('#curve-bot');
  // height: 300px;
  color: #fff;
  margin-top: 72px;

  .welcome {
    grid-row: unset;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    height: min(90%, 600px);

    &-title {
      max-width: 80%;
      justify-self: start;
    }

    &-body {
      max-width: 80%;
      text-align: left;
    }
  }

  .title, .subtitle {
    text-align: center;
  }
  .title {
    margin-bottom: 0;
  }
  .title + .subtitle {
    display: none;
    font-size: 1.2rem;
    margin-top: 0;
  }

  .welcome-img {
    grid-row: unset;
    width: min(100%, 500px);
    justify-self: center;
  }

  @media (min-width: 820px) {
    margin-top: 0;

    .welcome {
      grid-column: 2 / 5;
      grid-row: 1;
      width: 80%;
      justify-self: start;

      &-title {
        align-self: flex-end; 

        .title, .subtitle {
          display: block;
          text-align: right;
        }
      }

      &-img {
        grid-column: 4 / -1;
        grid-row: 1;
      }
    }
  }
}

// --- End Welcome ---

// --- About ---

#about {
  background-image: 
    url('../assets/img/fondo-2.svg');

  .about {
    padding: 1em 1.5em;
    background-color: #fff;
    color: var(--dark);
    width: 80%;
    border: 3px solid var(--secondary);
    border-radius: .3em;
    box-shadow: 4px 10px 10px rgba(0,0,0, .4);

    &-img {
      width: 80%;
    }

    &-title {
      width: 80%;

      .title {
        text-align: center;
        margin-bottom: 0;
        
        & + .subtitle {
          margin-top: 0;
          font-size: 1.2em;
        }
      }
      .subtitle {
        display: none;
      }
    }
  }

  
  @media (min-width: 820px) {
    .about {
      grid-column: 5 / -2;
      grid-row: 2;
      
      &-img {
        grid-column: 1 / 5;
        grid-row: 2;
      }

      &-title {
        grid-column: 2 / -3;
        grid-row: 1;

        .title {
          text-align: right;
        }

        .subtitle {
          text-align: right;
          display: block;
        }
      }
    }  
  }

}

//  --- End About ---

// --- Jobs ---

#jobs {
  // background-color: var(--secondary);
  background-image: 
    url('../assets/img/fondo-3.svg'),
    linear-gradient( 0deg, var(--primary), var(--secondary));

  .jobs {

    &-title {
      max-width: 80%;
      
    }
  }

  .card {
    background-color: #fff;
    padding: 10px;
    border: 3px solid var(--secondary);
    border-radius: .3em;
    width: min(80%, 400px);
    min-height: 200px;
    box-shadow: 4px 10px 10px rgba(0,0,0, .4);
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    &-title {
      font-size: 1.5em;
    }

  }
  
  @media (min-width: 820px) {
    .jobs {

      &-title {
        grid-column: 2 / -1;
        grid-row: 1 / 3;
      }

      &-img {
        grid-row: 2 / 7;
        grid-column: 1 / 3;
      }
    }

    
    .card {
      grid-row: 3/ 7;
      grid-column: 3 / 5;
    }
  }
}

// --- End Jobs ---

// --- Recruit ---

#recruit {
  // background-color: var(--secondary);
  
  background-image: 
    url('../assets/img/fondo-4.svg'),
    linear-gradient(  var(--primary), var(--secondary));

  .card {
    background-color: #fff;
    padding: 10px;
    border: 3px solid var(--secondary);
    border-radius: .3em;
    width: min(80%, 400px);
    min-height: 200px;
    box-shadow: 4px 10px 10px rgba(0,0,0, .4);
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    max-width: 80%;
  }

  .title {
    max-width: 80%;

  }

  @media (min-width: 820px) {
    .recruit {
      &-img {
        grid-column: 3 / 5;
        grid-row: 2 / 7;
      }
    }

    .card {
      max-width: 80%;
      grid-column: 1 / 3;
      grid-row: 3 / 7;
    }
    
    .title {
      grid-column: 1 / 4;
      grid-row: 1 / 3;
    }
  }
}

// --- End Recruit ---

// --- Contact ---

#contact {
  min-height: calc(100vh - 52px);
  background-color: #23272fcc;
  color: #fff;

  .contact {
    width: min(80%, 500px);

    &-logo {
      width: min(80%, 400px);
      display: none;
      flex-direction: column;
      align-items: center;
      gap: 60px;

      @media (min-width: 820px) {
        display: flex;
      }
    }
  
    &-form {
      margin-top: 4em;
      display: flex;
      flex-direction: column;
      gap: 20px;

      .form-row {
        display: flex;
        align-items: center;
      }
  
      label {
        text-align: start;
        display: inline-block;
        min-width: 100px;
        color: var(--secondary);
      }
  
      input {
        width: 100%;
        display: inline-block;
      }
  
      textarea {
        display: block;
      }
  
      .textarea {
        text-align: center;
        display: flex;
        flex-direction: column;
      }
    }
  }

  .title {
    margin-bottom: 0;
    
    & + .subtitle {
      margin-top: 0;
      font-size: 1.2em;
      color: var(--secondary);

    }
  }

}

// --- End Contact ---


</style>
