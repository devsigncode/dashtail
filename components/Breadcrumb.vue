<template>
    <div class="breadcrumb">
        <a class="pt-2" href="/">
            <Icon icon="home" size="2xl" class="inline-block" :iconColor="iconColor" />
        </a>
        <ul class="flex flex-wrap">
            <li v-for="(link, index) in links" :key="index">
                <a class="pl-3" :href="link.href">
                    <Icon :icon="divaider" size="lg" class="inline-block -m-1 pr-1" :iconColor="iconColor" />
                    <div :class="`${iconColor} inline-block`">{{ link.label }}</div>
                </a>
            </li>
        </ul>
    </div>
</template>

<script>

export default ({
    props: {
        links: {
            type: Array,
            default: []
        },
        iconColor: {
            type: String,
            default: "text-gray-500"
        },
        divaider: {
            type: String,
            default: "chevron-right"
        },
    },

    data() {
        return {
        }
    },
})
</script>
