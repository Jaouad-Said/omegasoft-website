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
            <h1 class="max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl text-blue-50">Services et Ing??nierie <span class="text__gradient">Informatique</span></h1>
            <p class="max-w-2xl mb-6 font-semibold text-blue-50 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">Cr??e en 1999, c???est une SSII (Soci??t?? de Services et d???Ing??nierie Informatique) dont les fondateurs capitalisent <span class="text__span-color">plus de 20 ans d???exp??rience dans le domaine</span> des syst??mes d???information.</p>
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
              <div class="bg-purple-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="text-blue-50 font-normal text-base font-medium">Adaptabilit??, s??rieux et comp??tence technique</span> 
            </a>
            <br>
            <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
              <div class="bg-purple-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="text-blue-50 font-normal text-base font-medium">Accompagnement, conseil, disponibilit??</span> 
            </a>
        </div>
        
        <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
            <img src="../assets/Images/Mask group.svg" alt="mockup">
        </div>
      </div>
      <a href="#" class="py-1 px-1 block max-w-screen-xl ml-auto mr-auto">
        <img class="flex center ml-auto mr-auto cursor-pointer animate-bounce" src="../assets/Images/mouse_line.svg" alt="mockup">
      </a>
  </section>
  <section class="service__Background px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
        <!-- -----------------------------------------------------Services-------------------------------------------------------------- -->
    <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
      <div class="mr-auto ml-auto  place-self-center">
        <h1 class="section__Title justify-center max-w-2xl mt-4 text-xl font-bold md:text-5xl xl:text-2xl text-blue-50">Nos Services</h1>
        <h2 class="section__SubTitle max-w-2xl mt-2 text-xl font-bold md:text-5xl xl:text-2xl text-blue-50">Les services que nous fournissons sont les plus efficaces du march??</h2>
      </div>
    </div>
    <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
      <div class="flex flex-wrap justify-center mr-auto ml-auto place-self-center lg:col-span-7">
        
      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg ">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>

      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>

      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>

      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>

      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>

      <div class="service__Card max-w-xs p-6 bg-white border m-4 border-gray-100 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 hover:shadow-lg">
        <img class="flex mr-auto w-10 h-10 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Service Icon.svg" alt="mockup">
        <a href="#">
            <h5 class="service__Title mb-2 text-2xl font-semibold tracking-tight text-gray-900 dark:text-white">D??veloppement sp??cifique
              des applications</h5>
        </a>
        <p class="service__Description mb-3 font-normal text-gray-500 dark:text-gray-400">Coder une fonctionnalit??, un site web ou encore une application enti??re, r??pondant aux besoins sp??cifiques de votre entreprise.</p>
          <a href="#" class="sevice__Button inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Voir Plus
            <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
            </svg>
        </a>
      </div>
      </div>
    </div>

        <!-- -----------------------------------------------------Produits-------------------------------------------------------------- -->
    <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
      <div class="mr-auto ml-auto  place-self-center">
        <h1 class="section__Title justify-center max-w-2xl mt-4 text-xl font-bold md:text-5xl xl:text-2xl text-blue-50">Nos Produits</h1>
      </div>
    </div>
    <div class="px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
      <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 pr-10 pl-10 ">
          <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
            <img src="../assets/Images/Capture d?????cran 2023-01-25 124117 1.svg" alt="mockup">
          </div>
          <div class="mr-auto place-self-center lg:col-span-7 p-6">
              <span class="product__Badge-Logico">Solution logicielle</span>
              <h1 class="product__Title max-w-2xl mb-2 mt-6 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl text-blue-50">La solution ERP</h1>
              <h1 class="max-w-2xl mb-4 text-2xl tracking-tight"><span class="product__text-gradient" >Logico</span></h1>
              <p class="product__Description max-w-2xl mb-2 font-semibold md:text-lg lg:text-xl">La solution logicielle ERP pour la gestion de toute une cha??ne de valeur de la p??che. Du traitement ?? l???exportation et quel que soit votre activit??, de la cong??lation, de la conserverie ou de la farine et huile de poisson.</p>
              
              <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Confiance, engagement, transparence</span> 
              </a>
              <br>
              <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Adaptabilit??, s??rieux et comp??tence technique</span> 
              </a>
              <br>
              <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Accompagnement, conseil, disponibilit??</span> 
              </a>
              <br>
              <a href="#" class="product__Button-Logico mt-4 inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                Voir Plus
                <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
                </svg>
              </a>
          </div>
        </div>
     </div>
    <div class="px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
        <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 pr-10 pl-10 ">
            <div class="mr-auto place-self-center lg:col-span-7 p-6">
                <span class="product__Badge-Jdoc bg-indigo-100 text-indigo-800 text-sm font-medium mr-auto rounded dark:bg-indigo-900 dark:text-indigo-300">Solution logicielle</span>
                <h1 class="product__Title max-w-2xl mb-2 mt-6 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl text-blue-50">Le logiciel</h1>
                <h1 class="max-w-2xl mb-4 text-2xl tracking-tight"><span class="product__text-gradient" >JDOC</span></h1>
                <p class="product__Description max-w-2xl mb-2 font-semibold md:text-lg lg:text-xl">La solution sp??cialement con??ue pour la digitalisation des d??partements juridiques. Son r??le est l???automatisation de la gestion des dossiers juridique depuis la cr??ation jusqu???aux cl??ture et la gestion d???archivage ??lectronique des dossiers.</p>
                
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-purple-300 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Consultation contr??le et suivi en ligne</span> 
                </a>
                <br>
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-purple-300 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Archivage ??lectronique des documents</span> 
                </a>
                <br>
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-purple-300 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Traitement automatis?? des dossiers juridiques</span> 
                </a>
                <br>
                <a href="#" class="product__Button-Jdoc mt-4 inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                  Voir Plus
                  <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
                  </svg>
                </a>
            </div>
            <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
              <img src="../assets/Images/Capture d?????cran 2023-01-25 124117 1.svg" alt="mockup">
          </div>
        </div>
    </div>
    <div class="px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 border-b border-gray-200 dark:border-gray-600">
        <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 pr-10 pl-10 ">
            <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
              <img src="../assets/Images/Capture d?????cran 2023-01-25 124117 1.svg" alt="mockup">
            </div>
            <div class="mr-auto place-self-center lg:col-span-7 p-6">
                <span class="product__Badge-OmegaPointage bg-indigo-100 text-indigo-800 text-sm font-medium mr-auto rounded dark:bg-indigo-900 dark:text-indigo-300">Solution logicielle</span>
                <h1 class="product__Title max-w-2xl mb-2 mt-6 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl text-blue-50">Solution de pointage</h1>
                <h1 class="max-w-2xl mb-4 text-2xl tracking-tight"><span class="product__text-gradient" >OmegaPointage</span></h1>
                <p class="product__Description max-w-2xl mb-2 font-semibold md:text-lg lg:text-xl">Une solution de gestion des pointages compl??te et bien pens??e Son r??le est param??trer, traiter et g??rer les pointages de ses salari??s en toute fluidit??.</p>
                
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Pointage Facial</span> 
                </a>
                <br>
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Pointage biom??trique</span> 
                </a>
                <br>
                <a class="inline-flex justify-between items-center py-1 px-1 pr-4 pt-4 text-sm text-gray-700 rounded-full" role="alert">
                  <div class="bg-blue-400 rounded-full px-1.5 py-1.5 mr-3 "></div><span class="product__Points font-semibold text-base">Pointage par badge</span> 
                </a>
                <br>
                <a href="#" class="product__Button-OmegaPointage mt-4 inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                  Voir Plus
                  <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
                  </svg>
                </a>
            </div>
          </div>
    </div>
  </section>
  <section class="partenaires__Background px-2 sm:px-4 dark:bg-gray-900 h-full w-full z-20 top-0 left-0 ">
   <!-- -----------------------------------------------------Partenaires-------------------------------------------------------------- -->
   <div class="flex center max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
    <div class="mr-auto ml-auto  place-self-center">
      <h1 class="justify-center max-w-2xl mt-4 text-xl font-bold md:text-5xl xl:text-2xl text-blue-50">Nos Partenaireses</h1>
    </div>
  </div>
  <div class="flex max-w-screen-xl px-4 py-8 ml-auto mr-auto mt-auto lg:gap-8 xl:gap-0 lg:py-4 lg:grid-cols-12 pr-10 pl-10 ">
    <div class="flex flex-wrap justify-center mr-auto ml-auto place-self-center lg:col-span-7">

    <div class="partenaires__Card flex flex-wrap justify-center max-w-xs p-6 m-4 ">
      <img class="w-16 h-16 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/Google logo.svg" alt="mockup">
      <p class="partenaires__Description mb-3 ">Les assistants exp??riment??s en Google Workspace de la soci??t?? OMEGASOFT, vous pouvez vous concentrer sur vos activit??s sans vous inqui??tez des al??as technologiques.</p>
        <a href="#" class="partenaires__Button-Google inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
          Voir Plus
          <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
          </svg>
      </a>
    </div>

    <div class="partenaires__Card flex flex-wrap justify-center max-w-xs p-6 m-4 ">
      <img class="w-32 h-16 mb-2" src="../assets/Images/Sage logo.svg" alt="mockup">
      <p class="partenaires__Description mb-3 ">Omega Soft propose des solutions de la gestion et la comptabilit?? de votre entreprise adapt??es ?? vos besoins afin de vous aider ?? cr??er votre propre tableau de bord.</p>
        <a href="#" class="partenaires__Button-Sage inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
          Voir Plus
          <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
          </svg>
      </a>
    </div>

    <div class="partenaires__Card flex flex-wrap justify-center max-w-xs p-6 m-4 ">
      <img class="w-16 h-16 mb-2 text-gray-500 dark:text-gray-400" src="../assets/Images/office-1 1.svg" alt="mockup">
      <p class="partenaires__Description mb-3 ">Les assistants experts des fonctionnalit??s des solutions Office 365, b??n??ficiez de la totalit?? des services de ce derniers avec les meilleurs prix et le meilleur accompagnement</p>
        <a href="#" class="partenaires__Button-Office inline-flex items-center px-3 py-2 text-sm font-medium text-center text-blue-900 bg-blue-300 rounded-lg hover:bg-blue-900 hover:text-blue-50 hover:px-5 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
          Voir Plus
          <svg fill="none" stroke="currentColor" class="w-3 h-3 mt-1 ml-2 -mr-1 " stroke-width="4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"></path>
          </svg>
      </a>
    </div>
    </div>
  </div>
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
