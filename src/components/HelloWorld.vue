<template>
  <div class="container">
    <Particles
      id="tsparticles"
      width="100%"
      height="100%"
      :style="{
        position: 'fixed',
      }"
      :options="{
        background: {
          color: {
            value: '#000',
          },
        },
        fpsLimit: 75,
        interactivity: {
          detectsOn: 'canvas',
          events: {
            onClick: {
              enable: false,
              mode: 'push',
            },
            onHover: {
              enable: false,
              mode: 'repulse',
            },
            resize: true,
          },
          modes: {
            bubble: {
              distance: 400,
              duration: 2,
              opacity: 0.8,
              size: 40,
            },
            push: {
              quantity: 4,
            },
            repulse: {
              distance: 200,
              duration: 0.4,
            },
          },
        },
        particles: {
          color: {
            value: '#ffffff',
          },
          links: {
            color: '#ffffff',
            distance: 150,
            enable: true,
            opacity: 0.5,
            width: 1,
          },
          collisions: {
            enable: true,
          },
          move: {
            direction: 'none',
            enable: true,
            outMode: 'bounce',
            random: false,
            speed: 1.5,
            straight: false,
          },
          number: {
            density: {
              enable: true,
              value_area: 1000,
            },
            value: 70,
          },
          opacity: {
            value: 0.5,
          },
          shape: {
            type: 'circle',
          },
          size: {
            random: true,
            value: 5,
          },
        },
        detectRetina: true,
      }"
    />
    <div class="centerContent">
      <div class="title">JIGAR LODAYA</div>
      <hr class="border" />
      <div class="title">Frontend Developer</div>
      <div class="subTitle">
        Knowledge Base
        <div class="iconSet">
          <img
            src="https://img.shields.io/badge/html5%20-%23E34F26.svg?&style=for-the-badge&logo=html5&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/css3%20-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/bootstrap%20-%23563D7C.svg?&style=for-the-badge&logo=bootstrap&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/javascript%20-%23323330.svg?&style=for-the-badge&logo=javascript&logoColor=%23F7DF1E"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/jquery%20-%230769AD.svg?&style=for-the-badge&logo=jquery&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/php-%23777BB4.svg?&style=for-the-badge&logo=php&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/laravel%20-%23FF2D20.svg?&style=for-the-badge&logo=laravel&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/mysql-%2300f.svg?&style=for-the-badge&logo=mysql&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/react%20-%2320232a.svg?&style=for-the-badge&logo=react&logoColor=%2361DAFB"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/angular%20-%23DD0031.svg?&style=for-the-badge&logo=angular&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/node.js%20-%2343853D.svg?&style=for-the-badge&logo=node.js&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/typescript%20-%23007ACC.svg?&style=for-the-badge&logo=typescript&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/redux%20-%23593d88.svg?&style=for-the-badge&logo=redux&logoColor=white"
          />
          &nbsp;
          <img
            src="https://img.shields.io/badge/Amazon%20AWS-%23232F3E?logo=amazon-aws&logoColor=white&style=for-the-badge"
          />
        </div>
      </div>
      <hr class="borderThin" />
      <div class="subTitle">
        Contact Info
        <div class="iconSet">
          <a href="https://github.com/jigs1212" target="_blank">
            <img
              src="https://img.shields.io/badge/github-%23100000.svg?&style=for-the-badge&logo=github&logoColor=white"
            /> </a
          >&nbsp;
          <a
            href="https://stackoverflow.com/users/2336835/jigs1212"
            target="_blank"
          >
            <img
              src="https://img.shields.io/badge/stack%20overflow-FE7A16?logo=stack-overflow&logoColor=white&style=for-the-badge"
              alt="Stackoverflow"
            /> </a
          >&nbsp;
          <a
            href="https://www.linkedin.com/in/jigar-lodaya-aba3268b/"
            target="_blank"
          >
            <img
              src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white"
              alt="LinkedIn"
            /> </a
          >&nbsp;
          <a
            href="mailto:jigar.lodaya12@gmail.com?subject=Hola%Jigar"
            target="_blank"
          >
            <img
              src="https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white"
              alt="Gmail"
            /> </a
          >&nbsp;
        </div>
      </div>
      <hr class="border" />
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.logo {
  position: absolute;
  top: 10%;
  left: 5%;
}

.container {
  min-height: 100vh;
  max-height: 100vh;
  font-family: "Fira Code", monospace;
  position: relative;
}

.centerContent {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  max-height: 100vh;
  color: #fff;
  width: 70%;
  text-align: center;

  @for $i from 1 through 5 {
    .title {
      font-size: 3rem;
      padding: 0 50px 20px;

      &:nth-of-type(2) {
        font-size: 2rem;
      }

      &:nth-of-type(#{$i})::before {
        content: "<";
        padding-right: 10px;
        color: rgb(random(255), random(255), random(255));
      }

      &:nth-of-type(#{$i})::after {
        content: "/>";
        color: rgb(random(255), random(255), random(255));
      }
    }

    .subTitle {
      font-size: 1.5rem;
      padding: 10px 50px;

      &:nth-of-type(#{$i})::before {
        content: "<";
        padding-right: 10px;
        color: rgb(random(255), random(255), random(255));
      }

      &:nth-of-type(#{$i})::after {
        content: "/>";
        color: rgb(random(255), random(255), random(255));
      }
    }
  }

  .iconSet {
    padding: 10px 20px;
    .icon {
      height: 50px;
    }
  }
}
.borderThin {
  border-bottom: 0.001rem ridge #fff;
  width: 50%;
}
.border {
  border-bottom: 0.01rem ridge #fff;
  width: auto;
}

.badges {
  text-align: right;
  position: absolute;
  top: 10%;
  right: 5%;
}

@media (max-width: 767px) {
  .centerContent {
    width: 100%;

    .title {
      margin-top: 50px;
      font-size: 1.5rem;
      padding: 0 25px 10px;
    }

    .title:nth-of-type(2) {
      font-size: 1rem;
    }

    .subTitle {
      font-size: 1rem;
      padding: 5px 25px;
    }

    .iconSet {
      padding: 5px 15px;
    }
  }
}
</style>
