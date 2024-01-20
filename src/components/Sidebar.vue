<template>
     <!-- component -->
     <div x-data="setup()"  class="flex h-screen antialiased text-gray-900 bg-gray-100 dark:bg-dark dark:text-light">
           <!-- Sidebar -->
           <div  class="fixed inset-y-0 z-10 flex w-80">
               <!-- Curvy shape -->
               <svg class="absolute inset-0 w-full h-full text-white" style="filter: drop-shadow(10px 0 10px #00000030)"
                   preserveAspectRatio="none" viewBox="0 0 309 800" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                   <path
                       d="M268.487 0H0V800H247.32C207.957 725 207.975 492.294 268.487 367.647C329 243 314.906 53.4314 268.487 0Z" />
               </svg>
               <!-- Sidebar content -->
               <div class="z-10 flex flex-col flex-1">
                   <div class="flex items-center justify-between flex-shrink-0 w-64 p-4">
                       <!-- Logo -->
                       <a href="#">
                           <span class="sr-only">K-UI</span>
                           <img src="../assets/logo/ლოგო.svg" alt="">
                       </a>
                       <!-- Close btn -->
                       <button @click="isSidebarOpen = false" class="p-1 rounded-lg focus:outline-none focus:ring">
                           <svg class="w-6 h-6" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
                               viewBox="0 0 24 24" stroke="currentColor">
                               <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                   d="M6 18L18 6M6 6l12 12" />
                           </svg>
                           <span class="sr-only">Close sidebar</span>
                       </button>
                   </div>
                   <div class="flex flex-col flex-1 w-64 p-4 mt-4 space-y-4 text-[#697BFF]">
                       <button class="flex items-center space-x-2">

                           <img src="../assets/logo/დეშბორდი.svg" alt="">
                           <h3>დეშბორდი</h3>
                       </button>
                       <button class="flex items-center space-x-2">
                           <img src="../assets/logo/განცხადებები.svg" alt="">
                           <h3>განცხადებები</h3>
                       </button>
                       <button class="flex items-center space-x-2 ">
                           <img class="w-6 h-6" src="../assets/logo/Setyobinebebi.svg" alt="">
                           <h3>შეტყობინებები</h3>
                       </button>
                       <button class="flex items-center space-x-2">
                           <img src="../assets/logo/Vector.svg" alt="">
                           <h3>ლიდერბორდი</h3>
                       </button>
                       <button class="flex items-center space-x-2">
                           <img src="../assets/logo/profile_round.svg" alt="">
                           <h3>ჩემი პროფილი</h3>
                       </button>
                       <button class="flex items-center space-x-2 text-[#FF0000]">
                           <img src="../assets/logo/logout.svg" alt="">
                           <h3>გასვლა</h3>
                       </button>
                    </div>
                   
                   <div class="flex-shrink-0 p-4">
                       <button class="flex items-center space-x-2">
                           <img src="../assets/logo/Vectorkitx.svg" alt="">
                           <span>დახმარება</span>
                       </button>
                   </div>
               </div>
           </div>
           <div class="flex flex-col items-center justify-center flex-1">
               <!-- Page content -->
               <button @click="isSidebarOpen = true" class="fixed p-2 text-white bg-black rounded-lg top-5 left-5">
                   <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                       stroke="currentColor">
                       <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                   </svg>
                   <span class="sr-only">Open menu</span>
               </button>  
           </div>
       </div>
       
      
</template>
<script>
        const setup = () => {
        return {
                isSidebarOpen: false,
            }
        }
    </script>