<script>
  import { Heading } from "flowbite-svelte";
  import Youtube from "$lib/components/YouTube.svelte";

  let player;

  const toggle = () => {
    console.log('changing video id')
    player.loadVideoById("dQw4w9WgXcQ");
  }
</script>

<section class="bg-white dark:bg-gray-900">
    <div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
        <div class="mr-auto place-self-center lg:col-span-7">
            <h1 class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white">Join Us</h1>
            <p class="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
            tempor incididunt ut labore et dolore magna aliqua. Senectus et netus
            et malesuada fames ac turpis egestas sed. Arcu non sodales neque
            sodales ut. Etiam non quam lacus suspendisse. Tortor id aliquet lectus
            proin nibh nisl.
            </p>
            <a href="/" class="bg-red-200 inline-flex items-center justify-center px-5 py-3 text-base font-medium text-center text-gray-900 border border-gray-300 rounded-lg hover:bg-red-300 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800">
                Contact Us
            </a> 
        </div>
        <div class="hidden lg:mt-0 lg:col-span-5 lg:flex bg-white-800 bg-cover bg-center bg-[url('https://placehold.co/600x400?text=Image+of+church')] bg-blend-lighten h-600 w-400 rounded-md" >
        </div>
    </div>
</section>
<section class="bg-red-50 rounded-md dark:bg-gray-900 py-4">
    <!-- events container -->
    <div class="grid max-w-screen-xl mx-auto px-4 lg:gap-4 lg:py-8 lg:grid-cols-12 bg-white rounded">
        <div class="place-self-start h-full w-full lg:col-span-6 bg-white px-8 py-8 rounded">
            <h3 class="max-w-2xl mb-4 text-4xl font-extrabold text-gray-800 tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white">
              Worship
            </h3>
            <p class="max-w-2xl mb-6 font-light text-gray-700 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
           
            <p class="text-xl">In person worship at 11:00 AM</p>
            <p class="text-xl">Youth and Adult Sunday school start at 9:45 AM</p>
           

        </div>
        <div class="place-self-center h-full w-full lg:col-span-6 bg-white px-8 py-8 rounded">
            <div><p class="text-2xl font-black text-center">Recent Sermon</p></div>
        <div>
        <Youtube id="nmcXGW-d8Fw" />
        </div>
        </div>
    </div>
</section>
<section class="bg-white rounded-md dark:bg-gray-900">
    <div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
        <div class="place-self-start lg:col-span-7">
            <h3 class="font-serif max-w-2xl mb-4 text-4xl font-extrabold text-gray-800 tracking-tight leading-none md:text-5xl xl:text-6xl dark:text-white">
              Events
            </h3>
            <p class="max-w-2xl mb-6 font-light text-gray-700 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
        </div>
    </div>
</section>
