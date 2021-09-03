<template>
    <div :class="`alert ${bgColor}`" v-if="showAlert">
        <div class="alert-content">
            <div class="w-8">
                <Icon :icon="icon" class="pt-1" :iconColor="iconColor" />
            </div>
            <div class="w-full">
                <div class="pb-1 flex justify-between">
                    <h1 :class="`font-semibold ${titleColor}`">{{ title }}</h1>
                    <button @click="showAlert = false">
                        <Icon icon="close" :iconColor="closeIconColor" />
                    </button>
                </div>
                <div>
                    <p :class="`text-sm ${descColor}`">{{ desc }}</p>    
                </div>
                <div class="alert-links">
                    <a :href="link.href" v-for="(link, index) in links" :key="index" :class="`text-sm pr-2 ${linkColor}`">{{ link.label }}</a>
                </div>            
            </div>
        </div>
    </div>
</template>

<script>

export default ({
    props: {
        title: {
            type: String,
            default: "Title"
        },
        desc: {
            type: String,
            default: "Title"
        },
        titleColor: {
            type: String,
            default: "text-gray-900"
        },
        descColor: {
            type: String,
            default: "text-gray-700"
        },
        linkColor: {
            type: String,
            default: "text-gray-700"
        },
        icon: {
            type: String,
            default: "error"
        },
        bgColor: {
            type: String,
            default: "bg-blue-300"
        },
        links: {
            type: Array,
            default: []
        },
        iconColor: {
            type: String,
            default: "text-blue-500"
        },
        closeIconColor: {
            type: String,
            default: "text-blue-500"
        },
    },

    data() {
        return {
            showAlert: true
        }
    },
})
</script>
