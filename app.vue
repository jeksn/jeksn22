<script setup>
import DarkmodeToggle from "/components/DarkModeToggle.vue";
</script>
<script>
export default {
  methods: {
    changeMode() {
      this.$colorMode.preference =
        this.$colorMode.preference === "light" ? "dark" : "light";
    },
  },
};
</script>
<template>
  <main>
    <header class="fixed w-full bg-opacity-90 px-4 md:px-0">
      <div class="max-w-screen-xl mx-auto py-8">
        <a href="/" class="logo text-lg bg-black py-4 px-8 text-white"
          >jeksn.me</a
        >
      </div>
    </header>
    <div class="h-screen flex flex-col justify-center px-4 md:px-0">
      <div class="max-w-screen-lg mx-auto">
        <h2 class="text-4xl md:text-6xl font-semibold mt-4">
          Front-end
          <span class="underline underline-offset-2">developer</span> based in
          <span class="underline underline-offset-2">Stockholm</span>
        </h2>
        <p class="mt-6 text-lg md:text-2xl max-w-screen-lg">
          I'm a design minded developer currently working at
          <a
            href="https://wtmg.se"
            class="underline underline-offset-2 hover:underline-offset-4"
            >WTMG</a
          ><br />
          Don't hesitate to get in touch.
        </p>
        <div class="mt-8">
          <h2 class="text-lg md:text-2xl">Where to find me:</h2>
          <ul class="text-base md:text-lg">
            <li>
              <a
                href="https://twitter.com/jeksn_"
                target="_blank"
                class="underline underline-offset-2 hover:underline-offset-4"
                >Twitter</a
              >
            </li>
            <li>
              <a
                href="https://www.linkedin.com/in/jeksn/"
                target="_blank"
                class="underline underline-offset-2 hover:underline-offset-4"
                >LinkedIn</a
              >
            </li>
            <li>
              <a
                href="https://oku.club/user/jek5n"
                target="_blank"
                class="underline underline-offset-2 hover:underline-offset-4"
                >Oku.club</a
              >
            </li>
            <li>
              <a
                href="mailto:johan@jeksn.me"
                target="_blank"
                class="underline underline-offset-2 hover:underline-offset-4"
                >E-mail me</a
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
    <DarkmodeToggle />
  </main>
</template>
<style>
.dark-mode {
  @apply text-white bg-black;
}
.dark-mode > .logo {
  @apply text-black bg-white;
}
.light-mode {
  @apply text-black bg-white;
}
</style>
