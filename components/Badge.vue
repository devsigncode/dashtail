<template>
    <div :class="`badge ${bgColor}`" v-if="showBadge">
        <Icon icon="dot" size="sm" class="inline-block" :iconColor="dotIconColor" v-if="dotIcon" />
        <span :class="`text-sm font-semibold ${closeIcon ? 'pr-1' : '' } ${dotIcon ? 'pl-1' : '' } ${labelColor}`">{{ label }}</span>
        <button @click="showBadge = false" v-if="closeIcon">
            <Icon icon="close" size="sm" class="inline-block" :iconColor="closeIconColor" />
        </button>
    </div>
</template>

<script>

export default ({
    props: {
        label: {
            type: String,
            default: "Badge"
        },
        labelColor: {
            type: String,
            default: "text-gray-900"
        },
        bgColor: {
            type: String,
            default: "bg-gray-300"
        },
        dotIconColor: {
            type: String,
            default: "text-gray-300"
        },
        closeIconColor: {
            type: String,
            default: "text-gray-300"
        },
        closeIcon: {
            type: Boolean,
            default: false
        },
        dotIcon: {
            type: Boolean,
            default: false
        },
    },

    data() {
        return {
            showBadge: true
        }
    },
})
</script>
