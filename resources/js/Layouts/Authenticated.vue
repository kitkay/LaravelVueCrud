<script setup>
import { ref } from 'vue';
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import Dropdown from '@/Components/Dropdown.vue';
import DropdownLink from '@/Components/DropdownLink.vue';
import BreezeNavLink from '@/Components/NavLink.vue';
import ResponsiveNavLink from '@/Components/ResponsiveNavLink.vue';
import { Link } from '@inertiajs/inertia-vue3';

const showingNavigationDropdown = ref(false);
</script>
<!-- Navigation Links -->
<div class="hidden space-x-8 sm:-my-px sm:ml-10 sm:flex">

    <BreezeNavLink
        :href="route('dashboard')"
        :active="route().current('dashboard')"
    >
        Dashboard
    </BreezeNavLink>

    <BreezeNavLink :href="route('posts.index')" :active="route().current('posts.index')">
        Posts
    </BreezeNavLink>

  </div>