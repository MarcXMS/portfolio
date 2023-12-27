<script setup>

</script>

<template>
  <div style="line-height: 0;">&nbsp</div>
  <div class="flex flex-wrap justify-center items-center flex-col">
    <TransitionGroup name="fade" appear>

      <h1 class="text-7xl font-bold" key="1">
        Marc Lüdders
      </h1>

      <h2 class="text-2xl" key="2" style="transition-delay: 0.1s; margin-bottom: 50px;">Web Developer</h2>

      <div class="mainContainer" key="3" style="transition-delay: 0.2s; max-width: 600px;">
        <h2 class="text-2xl font-bold" key="3" style="transition-delay: 0.2s;">Experienced in</h2>

        <div class="flex justify-center" key="4" style="transition-delay: 0.3s; margin-top: 20px;">
          <div class="flex flex-wrap justify-center gap-5">

            <div class="tooltip w-16" data-tip="JavaScript">
              <img src="/src/assets/js.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Vue.js">
              <img src="/src/assets/vue.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Vite.js">
              <img src="/src/assets/vite.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Tailwind CSS">
              <img src="/src/assets/tailwind.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Websockets (Socket.io)">
              <img src="/src/assets/socketio.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Progressive Web Apps">
              <img src="/src/assets/pwa.png" style="margin-top: 15px;" />
            </div>


            <div class="tooltip w-16 " data-tip="Node.js">
              <img src="/src/assets/nodejs.svg" />
            </div>

            <div class="tooltip w-16" data-tip="Express.js">
              <img src="/src/assets/expressjs.png" style="margin-top: 5px;" />
            </div>

            <div class="tooltip w-16 flex justify-center" data-tip="PostgreSQL">
              <img src="/src/assets/postgresql.svg" />
            </div>

            <div class="tooltip w-16 h-16 flex justify-center" data-tip="Apache">
              <img src="/src/assets/apache.svg" class="h-16" />
            </div>

            <div class="tooltip w-16 flex justify-center" data-tip="NGINX">
              <img src="/src/assets/nginx.svg" />
            </div>

            <div class="tooltip w-16 flex justify-center" data-tip="PM2">
              <img src="/src/assets/pm2.svg" />
            </div>

          </div>
        </div>
      </div>
      <h1 class="text-5xl font-bold" key="6" style="transition-delay: 0.4s; margin-top: 50px;">
        Projects I've worked on
      </h1>

      <div class="flex flex-wrap justify-center gap-5" key="7" style="margin-top: 20px; transition-delay: 0.5s;">

        <div class="secondaryContainer" key="8">
          <h3 class="text-3xl font-bold text-left" style="margin-bottom: 10px; margin-top: -10px;">Public Booking</h3>
          <a href="https://luehe-aue.de/die-elli/#booking-embed" target="_blank" class="">
            <img src="/src/assets/elli.png" class="projectImg" />
          </a>

          <div class="text-left text-lg font-bold" style="margin-top: 10px;">Web App to book public and private boat trips
            with booking managment tools for staff</div>
          <div class="text-left text-lg"><span class="font-bold">Tech:</span> Vue 3, WebSockets, Express (Node.js), NocoDB
            (PostgreSQL)</div>
        </div>


        <div class="secondaryContainer" key="8">
          <h3 class="text-3xl font-bold text-left" style="margin-bottom: 10px; margin-top: -10px;">Fahrmit</h3>
          <a href="https://fahrmit.ole.land" target="_blank" class="">
            <img src="/src/assets/fahrmit.png" class="projectImg" />
          </a>

          <div class="text-left text-lg font-bold" style="margin-top: 10px;">Local carpooling platform powered by a
            Progressive Web App</div>
          <div class="text-left text-lg"><span class="font-bold">Tech:</span> Vue 3, WebSockets, Express (Node.js), PWA, Airtable
          </div>
        </div>

        <div class="secondaryContainer" key="8">
          <h3 class="text-3xl font-bold text-left" style="margin-bottom: 10px; margin-top: -10px;">Course Booking</h3>
          <a href="https://kurse-buchen.app.geht.digital" target="_blank" class="">
            <img src="/src/assets/booking.png" class="projectImg" />
          </a>

          <div class="text-left text-lg font-bold" style="margin-top: 10px;">Online platform designed for reserving courses, such as those offered by fitness centers</div>
          <div class="text-left text-lg"><span class="font-bold">Tech:</span> Vue 3, WebSockets, Express (Node.js), PWA, Airtable</div>
        </div>


        <div class="secondaryContainer" key="8">
          <h3 class="text-3xl font-bold text-left" style="margin-bottom: 10px; margin-top: -10px;">Password Reset for Alfresco</h3>
          <a href="/" class="">
            <img src="/src/assets/reset.png" class="projectImg" />
          </a>

          <div class="text-left text-lg font-bold" style="margin-top: 10px;">Password reset dialog plugin for the Open-Source ECM Alfresco</div>
          <div class="text-left text-lg"><span class="font-bold">Tech:</span> Vue 3 & Express (Node.js)
          </div>
        </div>




      </div>
    </TransitionGroup>
  </div>
</template>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: transform 0.5s ease, opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
  transform: translateY(15px);
}

.mainContainer {
  background-color: #004397;
  color: #d8e2ff;
  border-radius: 15px;
  padding: 20px;
}

.secondaryContainer {
  background-color: #3f4759;
  color: #dbe2f9;
  border-radius: 15px;
  padding: 20px;
  padding-bottom: 12px;
}

.projectImg {
  width: 770px;
  border-radius: 5px;
  transition: transform .2s;
}

.projectImg:hover {
  transform: scale(1.03);
}
/*
@media (prefers-color-scheme: light) {
  .mainContainer {
    background-color: #d8e2ff;
    color: #001a43;
  }

  .secondaryContainer {
    background-color: #dbe2f9;
    color: #141b2c;
  }
}*/
</style>
