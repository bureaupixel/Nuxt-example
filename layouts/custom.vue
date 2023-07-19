<template>
    <div>
      <header class="p-5">
        <nav class="flex flex-wrap items-center justify-between mx-auto">
            <span class="text-3xl">
                <NuxtLink to="/">Nuxt example</NuxtLink>
            </span>   
            <span>    
                <ul class="flex flex-row">
                    <li class="pl-5"><NuxtLink to="/about">About</NuxtLink></li>
                    <li class="pl-5"><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
                    <li class="pl-5"><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
                </ul>
            </span>   
        </nav>
        <slot name="header">   
        </slot>
      </header>
      <main class="p-5">
        <slot name="main">
        </slot>
      </main>
      <footer class="p-5 fixed bottom-0 bg-white">
        <slot name="footer">
        </slot>
      </footer>
    </div>
  </template>
  