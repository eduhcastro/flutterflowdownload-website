<template>
  <main class="min-h-screen relative">


    <template>
      <header class="py-12 px-4 sm:px-6 lg:px-8">
        <div class="relative mx-auto max-w-[37.5rem] pt-20 text-center" style="
    display: flex;
    flex-direction: column;
    place-items: center;
">
          <div class="flex items-center justify-center space-x-3">
            <img loading="lazy" src="/logoFF.png" alt="FF" class="h-20 w-20" />
            <h1 class="text-4xl font-extrabold tracking-tight text-slate-700 sm:text-5xl"
              style="color: #14181b;font-style: normal;font-weight: 700;font-family: Productsans, sans-serif;">
              FF Download
            </h1>
          </div>
          <p class="mt-4 text-base leading-8 text-slate-800" style="
    width: max-content;
">
            On 03/22/2024, FlutterFlow launched its first official version of FlutterFlow Desktop, for Windows and
            MacOS. From
            then on, this project of mine becomes unnecessary.
            <br />
            When I did this project, FlutterFlow was not yet distributed for these platforms, and that's where the idea
            came from.
            <br />
            I thank everyone who used my tool, who put stars on GitHub, who followed me, and who accessed this site.
            <br />
            By the end of the year this site will be deactivated, as I will no longer renew the domain.
            <br />
            Thank you all.
          </p>

          <div style="display: flex; justify-content: center; margin-top: 6px;">
            <button
              onclick="window.open('https://flutterflow.io/desktop','_blank')"
              style="min-width: 120px;background-color: #4b39ef;margin-left: 0;margin-right: 0;box-shadow: 1px 1px 3px rgba(20, 24, 27, .69);color: #fff;border-radius: 8px;padding: 15px 24px;font-family: Productsans, sans-serif;font-size: 16px;transition: all .3s, opacity .2s;max-width: 250px;font-weight: 500;">
              Download from the official website</button>
            <button
            onclick="window.open('/download','_blank')"
              style="min-width: 120px;background-color: #fff;margin-left: 0;margin-right: 0;box-shadow: 1px 1px 3px rgba(20, 24, 27, .69);color: #0b0a0a;border-radius: 8px;padding: 15px 24px;font-family: Productsans, sans-serif;font-size: 16px;transition: all .3s, opacity .2s;max-width: 250px;font-weight: 500;">See old website</button>
          </div>


          <img style="margin-top: 3px;" src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExbDUycm14d3NycHh0OGVrMzl6OWR4OHE5OXp4ZXZrbzNodWkwOHdlNSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o6Mb4iDo3ne2U3M0o/giphy.gif" width="150px"/>




        </div>
      </header>
    </template>




  </main>
</template>

<script setup>
import seoConfig from "../seoConfig/index";
useHead({
  title: seoConfig.title,
  meta: [
    {
      name: "description",
      content: seoConfig.description,
      meta: [
        { name: "og:title", content: seoConfig.og.title },
        { name: "og:description", content: seoConfig.og.description },
        { name: "og:url", content: seoConfig.og.url },
        { name: "twitter:title", content: seoConfig.og.title },
        { name: "twitter:description", content: seoConfig.og.description },
      ],
    },
  ],
});
</script>
