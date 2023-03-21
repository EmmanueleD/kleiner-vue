<script setup>
import { useLayout } from '@/layout/composables/layout';
import { computed } from 'vue';

const { layoutConfig, contextPath } = useLayout();

const logoUrl = computed(() => {
    return `${contextPath}layout/images/logo-white.svg`;
});
</script>

<template>
    <div class="layout-footer">
        by

        <img src="../assets/img/emmd-logo.png" alt="Logo" height="15" class="mx-2" />
        with
        <img :src="logoUrl" alt="Logo" height="15" class="mx-2" />
    </div>
</template>
<style lang="scss" scoped></style>
