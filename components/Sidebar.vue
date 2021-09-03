<template>
    <div :class="`${showMenu ? '2xl:w-1/5 xl:w-1/4 lg:w-1/3 md:w-2/5 w-4/5 p-6' : 'w-20 p-3'} transition-all delay-100 min-h-screen border-r-2 border-gray-200 relative`">
      <div class="w-full">
        <div class="w-full flex flex-row justify-between items-center">
          <div :class="`rounded-md p-3 ${showMenu ? 'inline-block' : 'hidden'}`">
            <svg :class="`${showMenu ? 'w-8 h-8' : 'w-6 h-6'} transition-all delay-100`" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M5.10526 14.3158C4.38158 14.3158 3.78947 14.9079 3.78947 15.6316C3.78947 16.3553 4.38158 16.9474 5.10526 16.9474C5.82895 16.9474 6.42105 16.3553 6.42105 15.6316C6.42105 14.9079 5.82895 14.3158 5.10526 14.3158ZM5.10526 19.5789C4.38158 19.5789 3.78947 20.1711 3.78947 20.8947C3.78947 21.6184 4.38158 22.2105 5.10526 22.2105C5.82895 22.2105 6.42105 21.6184 6.42105 20.8947C6.42105 20.1711 5.82895 19.5789 5.10526 19.5789ZM5.10526 9.05263C4.38158 9.05263 3.78947 9.64474 3.78947 10.3684C3.78947 11.0921 4.38158 11.6842 5.10526 11.6842C5.82895 11.6842 6.42105 11.0921 6.42105 10.3684C6.42105 9.64474 5.82895 9.05263 5.10526 9.05263ZM1.15789 9.71053C0.789474 9.71053 0.5 10 0.5 10.3684C0.5 10.7368 0.789474 11.0263 1.15789 11.0263C1.52632 11.0263 1.81579 10.7368 1.81579 10.3684C1.81579 10 1.52632 9.71053 1.15789 9.71053ZM5.10526 3.78947C4.38158 3.78947 3.78947 4.38158 3.78947 5.10526C3.78947 5.82895 4.38158 6.42105 5.10526 6.42105C5.82895 6.42105 6.42105 5.82895 6.42105 5.10526C6.42105 4.38158 5.82895 3.78947 5.10526 3.78947ZM24.8421 11.0263C25.2105 11.0263 25.5 10.7368 25.5 10.3684C25.5 10 25.2105 9.71053 24.8421 9.71053C24.4737 9.71053 24.1842 10 24.1842 10.3684C24.1842 10.7368 24.4737 11.0263 24.8421 11.0263ZM15.6316 6.42105C16.3553 6.42105 16.9474 5.82895 16.9474 5.10526C16.9474 4.38158 16.3553 3.78947 15.6316 3.78947C14.9079 3.78947 14.3158 4.38158 14.3158 5.10526C14.3158 5.82895 14.9079 6.42105 15.6316 6.42105ZM15.6316 1.81579C16 1.81579 16.2895 1.52632 16.2895 1.15789C16.2895 0.789474 16 0.5 15.6316 0.5C15.2632 0.5 14.9737 0.789474 14.9737 1.15789C14.9737 1.52632 15.2632 1.81579 15.6316 1.81579ZM1.15789 14.9737C0.789474 14.9737 0.5 15.2632 0.5 15.6316C0.5 16 0.789474 16.2895 1.15789 16.2895C1.52632 16.2895 1.81579 16 1.81579 15.6316C1.81579 15.2632 1.52632 14.9737 1.15789 14.9737ZM10.3684 24.1842C10 24.1842 9.71053 24.4737 9.71053 24.8421C9.71053 25.2105 10 25.5 10.3684 25.5C10.7368 25.5 11.0263 25.2105 11.0263 24.8421C11.0263 24.4737 10.7368 24.1842 10.3684 24.1842ZM10.3684 1.81579C10.7368 1.81579 11.0263 1.52632 11.0263 1.15789C11.0263 0.789474 10.7368 0.5 10.3684 0.5C10 0.5 9.71053 0.789474 9.71053 1.15789C9.71053 1.52632 10 1.81579 10.3684 1.81579ZM10.3684 6.42105C11.0921 6.42105 11.6842 5.82895 11.6842 5.10526C11.6842 4.38158 11.0921 3.78947 10.3684 3.78947C9.64474 3.78947 9.05263 4.38158 9.05263 5.10526C9.05263 5.82895 9.64474 6.42105 10.3684 6.42105ZM10.3684 13.6579C9.27632 13.6579 8.39474 14.5395 8.39474 15.6316C8.39474 16.7237 9.27632 17.6053 10.3684 17.6053C11.4605 17.6053 12.3421 16.7237 12.3421 15.6316C12.3421 14.5395 11.4605 13.6579 10.3684 13.6579ZM20.8947 14.3158C20.1711 14.3158 19.5789 14.9079 19.5789 15.6316C19.5789 16.3553 20.1711 16.9474 20.8947 16.9474C21.6184 16.9474 22.2105 16.3553 22.2105 15.6316C22.2105 14.9079 21.6184 14.3158 20.8947 14.3158ZM20.8947 19.5789C20.1711 19.5789 19.5789 20.1711 19.5789 20.8947C19.5789 21.6184 20.1711 22.2105 20.8947 22.2105C21.6184 22.2105 22.2105 21.6184 22.2105 20.8947C22.2105 20.1711 21.6184 19.5789 20.8947 19.5789ZM20.8947 9.05263C20.1711 9.05263 19.5789 9.64474 19.5789 10.3684C19.5789 11.0921 20.1711 11.6842 20.8947 11.6842C21.6184 11.6842 22.2105 11.0921 22.2105 10.3684C22.2105 9.64474 21.6184 9.05263 20.8947 9.05263ZM20.8947 3.78947C20.1711 3.78947 19.5789 4.38158 19.5789 5.10526C19.5789 5.82895 20.1711 6.42105 20.8947 6.42105C21.6184 6.42105 22.2105 5.82895 22.2105 5.10526C22.2105 4.38158 21.6184 3.78947 20.8947 3.78947ZM24.8421 14.9737C24.4737 14.9737 24.1842 15.2632 24.1842 15.6316C24.1842 16 24.4737 16.2895 24.8421 16.2895C25.2105 16.2895 25.5 16 25.5 15.6316C25.5 15.2632 25.2105 14.9737 24.8421 14.9737ZM15.6316 19.5789C14.9079 19.5789 14.3158 20.1711 14.3158 20.8947C14.3158 21.6184 14.9079 22.2105 15.6316 22.2105C16.3553 22.2105 16.9474 21.6184 16.9474 20.8947C16.9474 20.1711 16.3553 19.5789 15.6316 19.5789ZM15.6316 24.1842C15.2632 24.1842 14.9737 24.4737 14.9737 24.8421C14.9737 25.2105 15.2632 25.5 15.6316 25.5C16 25.5 16.2895 25.2105 16.2895 24.8421C16.2895 24.4737 16 24.1842 15.6316 24.1842ZM10.3684 8.39474C9.27632 8.39474 8.39474 9.27632 8.39474 10.3684C8.39474 11.4605 9.27632 12.3421 10.3684 12.3421C11.4605 12.3421 12.3421 11.4605 12.3421 10.3684C12.3421 9.27632 11.4605 8.39474 10.3684 8.39474ZM10.3684 19.5789C9.64474 19.5789 9.05263 20.1711 9.05263 20.8947C9.05263 21.6184 9.64474 22.2105 10.3684 22.2105C11.0921 22.2105 11.6842 21.6184 11.6842 20.8947C11.6842 20.1711 11.0921 19.5789 10.3684 19.5789ZM15.6316 13.6579C14.5395 13.6579 13.6579 14.5395 13.6579 15.6316C13.6579 16.7237 14.5395 17.6053 15.6316 17.6053C16.7237 17.6053 17.6053 16.7237 17.6053 15.6316C17.6053 14.5395 16.7237 13.6579 15.6316 13.6579ZM15.6316 8.39474C14.5395 8.39474 13.6579 9.27632 13.6579 10.3684C13.6579 11.4605 14.5395 12.3421 15.6316 12.3421C16.7237 12.3421 17.6053 11.4605 17.6053 10.3684C17.6053 9.27632 16.7237 8.39474 15.6316 8.39474Z" fill="#6B7280"/>
            </svg>
          </div>
          <div :class="`${showMenu ? 'inline-block' : 'hidden'} w-full px-3`">
            <h5 class="text-gray-700 font-semibold text-xl">Acme Inc.</h5>
            <p class="text-gray-400 text-sm">San Francisco, CA</p>
          </div>
          <div class="p-2">
            <button
                @click="showMenu = !showMenu"
                :class="`inline-block transition-all delay-100 rounded-md p-2`"
                type="button">
                <Icon :icon="showMenu ? 'menu-close' : 'menu-show'" size="xl" iconColor="hover:text-blue-500 text-gray-500" />
            </button>
          </div>
        </div>
      </div>

      <div class="w-full mt-6">
        <ul class="">
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="dashboard" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-blue-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-blue-500 font-semibold transition-all delay-100">Dashboard</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="cart" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Store</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="analytic" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Analytics</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="report" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Reports</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="inbox" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Inbox</span>
              <Badge 
                label="32"
                labelColor="text-blue-800"
                v-if="showMenu"
              />
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="users" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Users</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="payouts" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Payouts</span>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="settings" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Settings</span>
            </nuxt-link>
          </li>
          <li class="relative">
            <a href="#" @click="s = !s" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 my-1 rounded-md group hover:bg-blue-200`">
              <Icon icon="comment" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Commments</span>
              <Icon icon="chevron-down" v-if="showMenu" size="md" :class="`inline-block transform ${s ? 'rotate-180' : ''} transition-all delay-100`" iconColor="group-hover:text-blue-500 text-gray-500" />
            </a>
            <ul v-show="s && showMenu" :class="`ml-6 border-l-2 border-gray-200 transition-all delay-100`">
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 mx-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">All comments</span>
                    </a>
                </li>
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 mx-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">Span</span>
                    </a>
                </li>
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 mx-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">Trashes</span>
                    </a>
                </li>
            </ul>
            <ul v-show="s && !showMenu" :class="`absolute top-12 left-12 z-50 bg-white rounded-md shadow-md w-36`">
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">All comments</span>
                    </a>
                </li>
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">Span</span>
                    </a>
                </li>
                <li>
                    <a href="#" :class="`flex items-center ${showMenu ? 'justify-between' : 'justify-center'} p-3 rounded-md group hover:bg-blue-200`">
                        <span class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100 text-sm">Trashes</span>
                    </a>
                </li>
            </ul>
          </li>
        </ul>
<!-- 
        <div class="absolute left-0 right-0 bottom-3 bg-white px-3">
            <a href="#" :class="`flex items-center ${showMenu ? 'justify-between px-6 py-3' : 'justify-center p-3'} shadow-md rounded-md group hover:bg-blue-200`">
              <Icon icon="add" size="2xl" class="inline-block" iconColor="group-hover:text-blue-500 text-gray-500" />
              <span v-if="showMenu" class="w-full pl-3 group-hover:text-blue-500 text-gray-500 font-semibold transition-all delay-100">Logout</span>
            </a>
        </div> -->
      </div>
    </div>
</template>

<script>
export default({
    data() {
        return {
            showMenu: true,
            s: true
        }
    },
})
</script>
