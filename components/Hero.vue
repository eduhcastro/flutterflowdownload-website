<style scoped>
.contri-list,
.step-3 {
  overflow: hidden;
  position: relative;
}

.step-3 {
  align-content: center;
  align-items: center;
  display: flex;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  gap: 24px;
  height: -moz-min-content;
  height: min-content;
  justify-content: flex-start;
  padding: 0;
  width: 100%;
}

.contri-list,
.contri-list-user {
  flex: none;
  transition: all .5s ease;
}

.contri-list {
  height: 40px;
}

.contri-list,
.step-3 {
  overflow: hidden;
  position: relative;
}

.contri-list-user {
  border-radius: 99px;
  bottom: 0;
  left: 0;
  overflow: hidden;
  top: 0;
  width: 40px;
  will-change: transform;
}
</style>
<template>
  <header class="py-12 px-4 sm:px-6 lg:px-8" style="background-image: url(background1.png);
  background-size: 30%;
  background-repeat: no-repeat;
  background-position: 88% 45%;">
    <div class="relative mx-auto max-w-[37.5rem] pt-20 text-center">
      <div class="flex items-center justify-center space-x-3">
        <img loading="lazy" src="/logoFF.png" alt="FF" class="h-20 w-20" />
        <h1 class="text-4xl font-extrabold tracking-tight text-slate-700 sm:text-5xl"
          style="color: #14181b;font-style: normal;font-weight: 700;font-family: Productsans, sans-serif;">
          FF Download
        </h1>
      </div>
      <p class="mt-4 text-base leading-7 text-slate-600">
        Welcome! Unofficial project dedicated to FlutterFlow. Using Node.js in conjunction with ElectronJS, I developed a
        portable application for Windows and MacOS. Download now and enjoy the different experience!
      </p>

      <div style="display: flex;justify-content: center;margin-top: 6px;">
        <button
          style="min-width: 120px;background-color: #4b39ef;margin-left: 0;margin-right: 0;box-shadow: 1px 1px 3px rgba(20, 24, 27, .69);color: #fff;border-radius: 8px;padding: 15px 24px;font-family: Productsans, sans-serif;font-size: 16px;transition: all .3s, opacity .2s;max-width: 250px;font-weight: 500;">
          Download on Windows</button>
        <button
          style="min-width: 120px;background-color: #fff;margin-left: 0;margin-right: 0;box-shadow: 1px 1px 3px rgba(20, 24, 27, .69);color: #0b0a0a;border-radius: 8px;padding: 15px 24px;font-family: Productsans, sans-serif;font-size: 16px;transition: all .3s, opacity .2s;max-width: 250px;font-weight: 500;">Download
          on MacOS</button>
      </div>


      <div class="step-3" style="margin-top: 35px;">
        <div class="contri-list" style="display:flex">

          <div v-for="contributor in contributors" :key="contributor.avatar_url" class="contri-list-user">
            <img :src="contributor.avatar_url" alt="Contributor Avatar"
              style="pointer-events:none;user-select:none;display:block;width:100%;height:100%;border-radius:inherit;object-position:center;object-fit:cover;image-rendering:auto">
          </div>

        </div>
      </div>

      <div
        style="display:flex;justify-content:center;margin-top:10px;flex-direction: column;align-content: center;text-align: center;place-items: center;">
        <h3 style="font-size: 12px;color: #484848;">Contribute to the project</h3><button id="login-with-github"
          type="submit" data-network="Github" class="button social-account-button button-fullwidth"
          style="font-family: var(--cp-font-family);-webkit-appearance: none;display: -webkit-inline-box;display: -webkit-inline-flex;display: -ms-inline-flexbox;display: flex;-webkit-box-align: center;-webkit-align-items: center;-ms-flex-align: center;align-items: center;vertical-align: middle;position: relative;font-family: inherit;font-size: 14px;text-shadow: none;line-height: 1.2;white-space: nowrap;text-overflow: ellipsis;text-decoration: none !important;font-weight: 400 !important;cursor: pointer;background: hsl(0deg 0% 0%);color: white;border-radius: 11px;padding: 10px;width: 210px;place-items: center;">
          <svg width="98" height="96" viewBox="0 0 100 100"
            style="width: 20px;height: 20px;fill: hsl(0deg 0% 100%);position: absolute;left: 14px;">
            <path fill-rule="evenodd" clip-rule="evenodd"
              d="M48.854 0C21.839 0 0 22 0 49.217c0 21.756 13.993 40.172 33.405 46.69 2.427.49 3.316-1.059 3.316-2.362 0-1.141-.08-5.052-.08-9.127-13.59 2.934-16.42-5.867-16.42-5.867-2.184-5.704-5.42-7.17-5.42-7.17-4.448-3.015.324-3.015.324-3.015 4.934.326 7.523 5.052 7.523 5.052 4.367 7.496 11.404 5.378 14.235 4.074.404-3.178 1.699-5.378 3.074-6.6-10.839-1.141-22.243-5.378-22.243-24.283 0-5.378 1.94-9.778 5.014-13.2-.485-1.222-2.184-6.275.486-13.038 0 0 4.125-1.304 13.426 5.052a46.97 46.97 0 0 1 12.214-1.63c4.125 0 8.33.571 12.213 1.63 9.302-6.356 13.427-5.052 13.427-5.052 2.67 6.763.97 11.816.485 13.038 3.155 3.422 5.015 7.822 5.015 13.2 0 18.905-11.404 23.06-22.324 24.283 1.78 1.548 3.316 4.481 3.316 9.126 0 6.6-.08 11.897-.08 13.526 0 1.304.89 2.853 3.316 2.364 19.412-6.52 33.405-24.935 33.405-46.691C97.707 22 75.788 0 48.854 0z"
              fill="#fff"></path>
          </svg>
          <span
            style="--cp-button-color: hsl(0deg 0% 100%);--cp-button-hover-bg: var(--cp-color-19);padding-left: 30px;text-align: left;">Github
            repository project</span>
        </button><button id="login-with-github" type="submit" data-network="Github"
          class="button social-account-button button-fullwidth"
          style="font-family: var(--cp-font-family);-webkit-appearance: none;display: -webkit-inline-box;display: -webkit-inline-flex;display: -ms-inline-flexbox;display: flex;-webkit-box-align: center;-webkit-align-items: center;-ms-flex-align: center;align-items: center;vertical-align: middle;position: relative;font-family: inherit;font-size: 14px;text-shadow: none;line-height: 1.2;white-space: nowrap;text-overflow: ellipsis;text-decoration: none !important;font-weight: 400 !important;cursor: pointer;background: hsl(0, 0%, 100%);color: black;border-radius: 11px;padding: 10px;width: 210px;margin-top: 5px;box-shadow: 10px;place-items: center;box-shadow: 1px 1px #b9b9b9;">
          <svg width="98" height="96" viewBox="0 0 100 100"
            style="width: 20px;height: 20px;fill: hsl(0deg 0% 100%);position: absolute;left: 14px;filter: invert(100%);">
            <path fill-rule="evenodd" clip-rule="evenodd"
              d="M48.854 0C21.839 0 0 22 0 49.217c0 21.756 13.993 40.172 33.405 46.69 2.427.49 3.316-1.059 3.316-2.362 0-1.141-.08-5.052-.08-9.127-13.59 2.934-16.42-5.867-16.42-5.867-2.184-5.704-5.42-7.17-5.42-7.17-4.448-3.015.324-3.015.324-3.015 4.934.326 7.523 5.052 7.523 5.052 4.367 7.496 11.404 5.378 14.235 4.074.404-3.178 1.699-5.378 3.074-6.6-10.839-1.141-22.243-5.378-22.243-24.283 0-5.378 1.94-9.778 5.014-13.2-.485-1.222-2.184-6.275.486-13.038 0 0 4.125-1.304 13.426 5.052a46.97 46.97 0 0 1 12.214-1.63c4.125 0 8.33.571 12.213 1.63 9.302-6.356 13.427-5.052 13.427-5.052 2.67 6.763.97 11.816.485 13.038 3.155 3.422 5.015 7.822 5.015 13.2 0 18.905-11.404 23.06-22.324 24.283 1.78 1.548 3.316 4.481 3.316 9.126 0 6.6-.08 11.897-.08 13.526 0 1.304.89 2.853 3.316 2.364 19.412-6.52 33.405-24.935 33.405-46.691C97.707 22 75.788 0 48.854 0z"
              fill="#fff"></path>
          </svg>
          <span
            style="--cp-button-color: hsl(0deg 0% 100%);--cp-button-hover-bg: var(--cp-color-19);padding-left: 30px;text-align: left;">Github
            repository website</span>
        </button>
      </div>



    </div>
  </header>

  <h1 style="text-align: center;font-size: medium;">Components</h1>

  <div style="height: 120px;margin-top: 15px;">
    <div style="display:flex;justify-content: center;align-items: center;">

      <div>
        <h3 style="font-size: 13px; color: #5e5d5d;">App</h3>
        <div style="display: flex; justify-content: center; align-items: center; height: 40px;">
          <div>
            <img style="width: 200px;"
              src="https://assets-global.website-files.com/635ff61792c1c6ebf4e1edad/6364138a12ac6843f1c23412_flutterflow_logo_black-p-500.png">
          </div>

          <div>
            <img src="https://cdn.icon-icons.com/icons2/2699/PNG/512/electronjs_logo_icon_169208.png"
              style="width: 200px;">
          </div>
        </div>
      </div>


      <div>
        <h3 style="font-size: 13px;
  color: #5e5d5d;">Website</h3>
        <div style="display: flex; justify-content: center; align-items: center;  height: 40px;">
          <div>
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/66/Nuxt_logo_%282021%29.svg" style="width: 170px;">
          </div>

          <div>
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/Vercel_logo_black.svg/2560px-Vercel_logo_black.svg.png"
              style="width: 150px;">
          </div>
        </div>
      </div>



    </div>
  </div>
</template>

<script setup>
const { data: contribuidores } = await useFetch('https://api.github.com/repos/eduhcastro/flutterflow-desktop/contributors')
var contributors = contribuidores.value
</script>

<style scoped>
.form-input {
  @apply block h-10 w-full rounded-md bg-white pr-3 pl-12 text-slate-900 shadow-md shadow-black/5 ring-1 ring-slate-900/5 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-primary sm:text-sm sm:leading-6;
}

.form-submit {
  @apply inline-flex justify-center rounded-lg text-sm font-semibold py-2.5 px-4 bg-slate-900 text-white hover:bg-slate-700 ml-4 flex-none;
}
</style>
