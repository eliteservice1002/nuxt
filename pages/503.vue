<template>
    <div class="container p-4 has-text-centered">
        <span class="icon is-large">
            <fa class="has-text-info"
                icon="tools"
                size="2x"/>
        </span>
        <p class="subtitle is-3 mx-6">
            {{ this.$i18n('The application is briefly unavailable for scheduled maintenance. Please check back in a few minutes') }}
        </p>
    </div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core';
import { faTools } from '@fortawesome/free-solid-svg-icons';

library.add(faTools);

export default {
    name: 'maintenanceMode',
    head: {
        title: 'Maintenance Mode'
    }
};
</script>