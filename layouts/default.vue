<template>
  <div class="default-layout mx-auto container h-screen flex flex-col px-4">
    <Header class="" />
    <div class="grow">
      <slot />
    </div>
    <Footer class="" />
  </div>
</template>
