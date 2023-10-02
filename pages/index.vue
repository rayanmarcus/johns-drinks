
<template>
  <div>
    <div>
      Aqui a mensagem: {{ msg }} ///
      <NuxtLink to="/about">Ir para about</NuxtLink>
    </div>
    <div>
      <button @click="onClick()">Click</button>
    </div>
    <div>
      My composable {{ foo2 }} \o/
    </div>
    <NuxtWelcome />
  </div>
</template>

<script setup lang="ts">

const msg = "1ª mensagem para exibir"
const foo2 = texto('2ª mensagem para exibir no meu composableee')
const onClick = (() => alert('My alert') )
</script>