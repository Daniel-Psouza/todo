<template>

    <header class="flex justify-between bg-blue-600 h-25 items-center px-5">
        <h1 class="text-white text-2xl font-bold">Gerenciamento de Tarefas</h1>
        <nav class="flex gap-4 text-white">
            <Link :href="route('register.index')">Cadastro de Usuário</Link>
            <Link :href="route('todos.create')">Cadastro de Tarefas</Link>
            <Link :href="route('todos.index')">Gerenciar Tarefas</Link>
        </nav>
    </header>

    <main class="w-11/12 mx-auto mt-4">
        <slot />
    </main>
</template>

<script setup lang='ts'>
    import { Link } from '@inertiajs/vue3'
</script>