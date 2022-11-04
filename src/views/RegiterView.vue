<script setup>
import registerFormVue from '../components/authentication/registerForm.vue';
import IconBadgeVue from '../components/icons/IconBadge.vue';
import iconBookVue from '../components/icons/iconBook.vue';
import IconsLayerVue from '../components/icons/IconsLayer.vue';
import Customizable  from '../components/authentication/features/Customizable.vue';
import Documentation from '../components/authentication/features/Documentation.vue';
import Fortune from '../components/authentication/features/Fortune.vue';

</script>
      
<template>
  <main>
    <div class="relative overflow-hidden bg-white">
      <div class="mx-auto">
        <div class="flex flex-col items-center w-full min-h-screen pt-6 sm:justify-center sm:pt-0">
          <div class="w-full p-5 mx-auto md:max-w-4xl">
            <h2 class="mb-10 text-5xl font-bold text-center">
              <span class="block lg:mb-2">Join & Get Our</span>
              <span class="block">Pro Benefits</span>
            </h2>
          </div>
          <div class="w-full p-5 mx-auto md:max-w-4xl">
            <div class="grid grid-cols-1 gap-4 md:grid-cols-2">
              <div class="mx-auto md:mx-0">
                <div class="mb-12">
                  <div class="block mb-2">
                   <!-- icons layer -->
                   <IconsLayerVue/>
                    <h3 class="inline-block ml-2 text-lg font-semibold">
                      Customizable
                    </h3>
                  </div>
                  <Customizable />
                </div>
                <div class="mb-12">
                  <div class="block mb-2">
                    <!-- icons fortune  -->
                    <iconLayerVue />
                    <h3 class="inline-block ml-2 text-lg font-semibold">
                      500 Fortune
                    </h3>
                  </div>
               <fortune />
                </div>
                <div class="mb-12">
                  <div class="block mb-2">
                    <!-- icons books -->
                    <iconBookVue />
                    <h3 class="inline-block ml-2 text-lg font-semibold">
                      Documentation
                    </h3>
                  </div>
                  <Documentation />
                </div>
              </div>
              <div>
                <!-- Register -->
                <registerFormVue />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
