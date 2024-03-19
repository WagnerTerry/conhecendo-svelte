<script>

  import Logo from "./Logo.svelte";

  const items = [
    { href: '/', label: 'Início'},
    { href: '/sobre', label: 'Sobre'},
    { href: '/portfolio', label: 'Portfólio'},
    { href: '/contato', label: 'Contato'},
    { href: '/faq', label: 'Perguntas Frequentes'},

  ]

</script>
<a href="/">
    <Logo />
</a>

{#each items as {href, label}}

<a {href} class="text-gray-800 transition-colors duration-300 transform dark:text-gray-200 border-b-2 hover:border-blue-500 mx-1.5 sm:mx-6">{label}</a>

{/each}
<!-- <a href="/" class="text-gray-800 transition-colors duration-300 transform dark:text-gray-200 border-b-2 border-blue-500 mx-1.5 sm:mx-6">Home</a> -->

