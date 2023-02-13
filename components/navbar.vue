<template>
    <div class="navbar bg-base-300 fixed t-0 z-50 w-full">
        <div class="navbar-start">
            <div class="dropdown">
                <label tabindex="0" class="btn btn-ghost lg:hidden">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                        stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h8m-8 6h16" />
                    </svg>
                </label>
                <ul tabindex="0" class="menu menu-compact dropdown-content mt-3 p-2 shadow bg-base-100 rounded-box w-52">
                <li><NuxtLink to="/contact">Contact</NuxtLink></li>
                <li><NuxtLink to="/about">Despre</NuxtLink></li>
                <li><NuxtLink to="/showcase">Produse</NuxtLink></li>
                </ul>
            </div>
            <NuxtLink to="/" class="btn btn-ghost normal-case text-xl">Prodeprod</NuxtLink>
        </div>
        <div class="navbar-end hidden lg:flex">
            <ul class="menu menu-horizontal px-1">
                <li>
                    <NuxtLink to="/contact">Contact</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">Despre</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/showcase">Produse</NuxtLink>
                </li>
            </ul>
        </div>
     
    </div>
</template>
<script></script>