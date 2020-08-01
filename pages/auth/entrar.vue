<template lang="pug">
  .login-wrapper
    .login-form
      h1.title Entrar
      .card
        label(for="email") Endereço de email
        input(type="email" id="email" placeholder="catioro@gatito.miau")
        .my-3
        label(for="senha") Senha
        input(type="password" id="senha" placeholder="********")
        .my-3
        button.orange(type="submit") Entrar na minha conta
</template>

<script>
export default {
  name: ''
}
</script>

<style lang="postcss" scoped>
.login-wrapper {
  @apply bg-indigo-400 w-screen h-screen flex flex-col;

  .login-form {
    @apply flex flex-col m-auto justify-center items-stretch w-full max-w-sm;

    .title {
      @apply text-white text-4xl font-bold uppercase tracking-wide pl-6;
    }

    .card {
      @apply bg-white w-full shadow-xl rounded-xl px-6 pt-6 pb-6 flex flex-col;
    }

    label {
      @apply mb-1;
    }
  }
}
</style>
