<template>
  <!-- <div class="container mx-auto"> -->
    <!-- <Alert 
      title="Lorem, ipsum dolor." 
      desc="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque, optio? Lorem ipsum dolor sit, amet consectetur adipisicing elit. Praesentium dolore repellendus hic error atque ad exercitationem dolorem similique et, dolor autem quaerat eligendi asperiores, architecto accusantium, quibusdam neque at reprehenderit optio dicta tempore pariatur corrupti." 
      :links="alertLinks"
      icon="warning"
      bgColor="bg-yellow-200"
      iconColor="text-yellow-700"
      closeIconColor="text-yellow-700"
      linkColor="text-yellow-700"
      titleColor="text-yellow-700"
      descColor="text-yellow-700"
      />
    <Alert 
      title="Lorem, ipsum dolor." 
      desc="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque, optio? Lorem ipsum dolor sit, amet consectetur adipisicing elit. Praesentium dolore repellendus hic error atque ad exercitationem dolorem similique et, dolor autem quaerat eligendi asperiores, architecto accusantium, quibusdam neque at reprehenderit optio dicta tempore pariatur corrupti." 
      :links="alertLinks"
      icon="info"
      bgColor="bg-blue-200"
      iconColor="text-blue-700"
      closeIconColor="text-blue-700"
      linkColor="text-blue-700"
      titleColor="text-blue-700"
      descColor="text-blue-700"
      />
    <Alert 
      title="Lorem, ipsum dolor." 
      desc="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque, optio? Lorem ipsum dolor sit, amet consectetur adipisicing elit. Praesentium dolore repellendus hic error atque ad exercitationem dolorem similique et, dolor autem quaerat eligendi asperiores, architecto accusantium, quibusdam neque at reprehenderit optio dicta tempore pariatur corrupti." 
      :links="alertLinks"
      icon="success"
      bgColor="bg-green-200"
      iconColor="text-green-700"
      closeIconColor="text-green-700"
      linkColor="text-green-700"
      titleColor="text-green-700"
      descColor="text-green-700"
      />
    <Alert 
      title="Lorem, ipsum dolor." 
      desc="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eaque, optio? Lorem ipsum dolor sit, amet consectetur adipisicing elit. Praesentium dolore repellendus hic error atque ad exercitationem dolorem similique et, dolor autem quaerat eligendi asperiores, architecto accusantium, quibusdam neque at reprehenderit optio dicta tempore pariatur corrupti." 
      :links="alertLinks"
      icon="info"
      bgColor="bg-red-200"
      iconColor="text-red-700"
      closeIconColor="text-red-700"
      linkColor="text-red-700"
      titleColor="text-red-700"
      descColor="text-red-700"
      /> -->

      <!-- <Badge 
        label="Badge text"
        labelColor="text-green-500"
        :dotIcon="true"
        :closeIcon="true"
        dotIconColor="text-green-500"
        closeIconColor="text-green-500"
        bgColor="bg-green-100"
      />
      <Badge 
        label="Badge text"
        labelColor="text-yellow-500"
        :dotIcon="true"
        :closeIcon="true"
        dotIconColor="text-yellow-500"
        closeIconColor="text-yellow-500"
        bgColor="bg-yellow-100"
      />
      <Badge 
        label="Badge text"
        labelColor="text-red-500"
        :dotIcon="true"
        :closeIcon="true"
        dotIconColor="text-red-500"
        closeIconColor="text-red-500"
        bgColor="bg-red-100"
      />
      <Badge 
        label="Badge text"
        labelColor="text-gray-500"
        :dotIcon="true"
        :closeIcon="true"
        dotIconColor="text-gray-500"
        closeIconColor="text-gray-500"
      /> -->
      
      <!-- <Breadcrumb 
        :links="breadcrumbLinks"
        divaider="chevron-right"
      />
      <Breadcrumb 
        :links="breadcrumbLinks"
        divaider="dot"
      />
      <Breadcrumb 
        :links="breadcrumbLinks"
        divaider="drob"
      /> -->
      
      <!-- <button class="button">
        Button
      </button>
      <button class="button px-6 py-3">
        Button
      </button>
      <button class="button bg-green-500 hover:bg-green-600">
        Button
      </button>
      <button class="button-circle">
        <Icon icon="add" size="lg" class="inline-block pt-1" iconColor="text-white" />
      </button> -->


  <!-- </div> -->

  <div class="w-full">
    <Sidebar />
  </div>
</template>

<script>
export default {
  data() {
    return {
      alertLinks: [
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        }
      ],
      breadcrumbLinks: [
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        },
        {
          href: "https://google.com",
          label: "google.com"
        }
      ],
      showMenu: true
    }
  },


  methods: {
  }
}
</script>
