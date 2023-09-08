<template>
  <div>
    <header class="shadow-sm bg-gray">
      <nav class="container mx-auto p-4 flex justiy-between">
        <ul class="container flex gap-3">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/blogs" class="btn">Blogs</NuxtLink></li>
          <li><NuxtLink to="/contact">Contact us</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <div>
      <h1>parant layout</h1>
    </div>
    <!-- output the page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>
