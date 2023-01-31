<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
    <nav
    class="bg-white px-2 sm:px-4 py-2.5 dark:bg-gray-900 sticky w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600"
  >
    <div
      class="container max-w-7xl flex flex-wrap items-center justify-between mx-auto pl-10 pr-10"
    >
      <a href="#" class="flex items-center">
        <img
          src="../assets/Images/logo.svg"
          class="h-6 mr-3 sm:h-9"
          alt="Flowbite Logo"
        />
      </a>
      <div class="flex md:order-2">
        <a
          href="#"
          class="text-white bg-blue-500 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-500 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-500 dark:hover:bg-blue-500 dark:focus:ring-blue-900"
        >
          Contactez-nous
      </a>
        <button
          data-collapse-toggle="navbar-sticky"
          type="button"
          class="inline-flex items-center p-2 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
          aria-controls="navbar-sticky"
          aria-expanded="false"
        >
          <span class="sr-only">Ouvrire le menu</span>
          <svg
            class="w-6 h-6"
            aria-hidden="true"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </button>
      </div>
      <div
        class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1"
        id="navbar-sticky"
      >
        <ul
          class="flex flex-col p-4 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700"
        >
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:p-0 dark:text-white"
              aria-current="page"
              >Acceuil</a
            >
          </li>
          <li>
            <a
              href="#"
              class="flex items-center justify-between w-full py-2 pl-3 pr-4 font-medium text-gray-700 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent"
              aria-current="page"
              >A propos</a
            >
          </li>
          <li>
            <button
              id="dropdownNavbarLink"
              data-dropdown-toggle="dropdownNavbar"
              class="flex items-center justify-between w-full py-2 pl-3 pr-4 font-medium text-gray-700 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent"
            >
              Produits<svg
                class="pt-1 w-5 h-5 ml-0"
                aria-hidden="true"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                  clip-rule="evenodd"
                ></path>
              </svg>
            </button>
            <div
              id="dropdownNavbar"
              class="z-10 hidden font-normal bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700 dark:divide-gray-600"
            >
              <ul
                class="py-2 text-sm text-gray-700 dark:text-gray-400"
                aria-labelledby="dropdownLargeButton"
              >
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Logico</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Jdoc</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >OmegaPointage</a
                  >
                </li>
              </ul>
            </div>
          </li>
          <li>
            <button
              id="dropdownNavbarLink"
              data-dropdown-toggle="dropdownNavbar"
              class="flex items-center justify-between w-full py-2 pl-3 pr-4 font-medium text-gray-700 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent"
            >
              Services<svg
                class="pt-1 w-5 h-5 ml-0"
                aria-hidden="true"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                  clip-rule="evenodd"
                ></path>
              </svg>
            </button>
            <div
              id="dropdownNavbar"
              class="z-10 hidden font-normal bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700 dark:divide-gray-600"
            >
              <ul
                class="py-2 text-sm text-gray-700 dark:text-gray-400"
                aria-labelledby="dropdownLargeButton"
              >
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Logico</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Jdoc</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >OmegaPointage</a
                  >
                </li>
              </ul>
            </div>
          </li>
          <li>
            <button
              id="dropdownNavbarLink"
              data-dropdown-toggle="dropdownNavbar"
              class="flex items-center justify-between w-full py-2 pl-3 pr-4 font-medium text-gray-700 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent"
            >
              Partenaires<svg
                class="pt-1 w-5 h-5 ml-0"
                aria-hidden="true"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                  clip-rule="evenodd"
                ></path>
              </svg>
            </button>
            <div
              id="dropdownNavbar"
              class="z-10 hidden font-normal bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700 dark:divide-gray-600"
            >
              <ul
                class="py-2 text-sm text-gray-700 dark:text-gray-400"
                aria-labelledby="dropdownLargeButton"
              >
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Logico</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >Jdoc</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white"
                    >OmegaPointage</a
                  >
                </li>
              </ul>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <section class="hero__background px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
    <div class="grid max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
        <div class="mr-auto place-self-center lg:col-span-7">
            <h1 class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl text-blue-50">Services et Ingénierie <span class="text__gradient">Informatique</span></h1>
            <p class="max-w-2xl mb-6 font-semibold text-blue-50 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">Crée en 1999, c’est une SSII (Société de Services et d’Ingénierie Informatique) dont les fondateurs capitalisent <span class="text__span-color">plus de 20 ans d’expérience dans le domaine</span> des systèmes d’information.</p>
            <a href="#" class="inline-flex items-center justify-center px-5 py-3 mr-3 text-base font-medium text-center text-white rounded-lg bg-blue-500 hover:bg-blue-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
                Nos Services
                <svg class="w-5 h-5 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
            </a>
            <br>
            <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
              <span class="text-blue-50  font-bold text-base">Nos valeurs :</span> 
            </a>
            <br>
            <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
              <div class="bg-purple-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="text-blue-50 font-normal text-base font-medium">Confiance, engagement, transparence</span> 
            </a>
            <br>
            <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
              <div class="bg-purple-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="text-blue-50 font-normal text-base font-medium">Adaptabilité, sérieux et compétence technique</span> 
            </a>
            <br>
            <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
              <div class="bg-purple-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="text-blue-50 font-normal text-base font-medium">Accompagnement, conseil, disponibilité</span> 
            </a>
        </div>
        
        <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
            <img src="../assets/Images/Mask group.svg" alt="mockup">
        </div>
      </div>
      <a href="#" class="py-1 px-1 block max-w-screen-xl ml-auto mr-auto">
          <img class="flex center ml-auto mr-auto" src="../assets/Images/mouse_line.svg" alt="mockup">
      </a>
</section>
</template>

<style scoped>
/* span{
    font-size: smaller;
}
.contactbar__container {
    position: relative;
    width: 100vw;
    height: 4vh;
    left: 0px;
    top: 0px;
    display: flex;
    flex-direction: row;
    font-size: medium;
    letter-spacing: 0.05rem;
    align-items: center;
    justify-content: space-between;

    background: #436BB2;
    border-radius: 0px;
    color: white;
}

.contactbar__element{
    display: flex;
    flex-direction: row;
    margin-right: 10rem;
    margin-left: 10rem;
}

.contactbar__element i{
    margin: 0.5rem;
} */
</style>
