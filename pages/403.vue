<template>
    <div class="container p-4 has-text-centered">
        <span class="icon is-large">
            <fa class="has-text-danger"
                icon="ban"
                size="2x"/>
        </span>
        <p class="subtitle is-3">
            {{ this.$i18n('You are not authorized here') }}
        </p>
    </div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core';
import { faBan } from '@fortawesome/free-solid-svg-icons';

library.add(faBan);

export default {
    name: 'unauthorized',
    head: {
        title: 'Unauthorized'
    }
};
</script>

