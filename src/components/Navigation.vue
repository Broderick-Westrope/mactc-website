<script setup>
const navItems = [
    { href: '#about', text: 'About' },
    { href: '#services', text: 'Services' },
    { href: '#fees', text: 'Fees' },
    { href: '#contact', text: 'Contact' }
];
</script>

<template>
    <nav class="navbar bg-base-200 top-0 z-50">
        <div class="container mx-auto px-4">
            <ul class="menu menu-horizontal px-1">
                <li v-for="item in navItems" :key="item.href">
                    <a :href="item.href" class="hover:bg-base-300">{{ item.text }}</a>
                </li>
            </ul>
        </div>
    </nav>
</template>
