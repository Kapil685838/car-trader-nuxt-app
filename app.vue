<template>
  <div>
    <!-- NAVBAR -->
    <header class="sticky top-0 z-50 border-b bg-white shadow-md px-4 py-3">
      <nav class="max-w-7xl mx-auto flex justify-between items-center space-x-1">
        <a href="#" class="text-3xl font-mono">CarTrader</a>
      </nav>
    </header>
    <!-- NAVBAR -->

    <div>
      <!-- Home hero -->
      <div class="relative h-screen w-100 bg-no-repeat bg-cover bg-bottom bg-[url('https://img.freepik.com/free-photo/sports-car-driving-asphalt-road-night-generative-ai_188544-8052.jpg?w=996&t=st=1704004307~exp=1704004907~hmac=7a635ea7e3b3d62653d692e27e0ca11274b0d93cad7f0bf029b7bb6bab8e591a')]">
        <div class="z-10 absolute w-full h-full flex justify-center items-center">
          <div class="text-center w-full sm:w-3/5 lg:w-1/2">
            <h1 class="text-3xl md:text-4xl lg:text-5xl font-serif mb-4 md:mb-6 lg:mb-8 text-white">Find Your Drive</h1>

            <!-- Home search bar -->
            <div class="font-serif w-full text-sm md:text-lg lg:text-2xl rounded-full bg-white flex justify-between overflow-hidden drop-shadow-2xl mx-auto">
              <input 
                type="text" 
                class="py-2 px-5 lg:py-3 lg:px-6 w-full rounded-full focus:outline-none"
                placeholder="Search by city..."
              />
              <button class="bg-sky-500 px-6 md:px-10 text-white">Search</button>
            </div>
            <!-- Home search bar -->
          </div>
        </div>
        <div class="z-1 absolute w-full h-full bg-black opacity-50"></div>
      </div>
      <!-- Home hero -->
    </div>

    <!-- Cars page -->
    <div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-16">
      <div class="mt-32 flex">
        <!-- Car side bar -->
        <div class="shadow border mr-10 z-30 max-w-64 max-h-max">
          <div class="p-5 flex justify-between gap-12 relative cursor-pointer border-b">
            <h3>Location</h3>
            <h3 class="text-blue-400 capitalize">Toronto</h3>
            <!-- <div class="absolute border shadow left-56 p-5 top-1 -m-1 bg-white">
              <input type="text" class="border p-1 rounded">
              <button class="bg-blue-400 w-full mt-2 rounded text-white p-1">
                Apply
              </button>
            </div> -->
          </div>

          <div class="p-5 flex justify-between gap-12 relative cursor-pointer border-b">
            <h3>Make</h3>
            <h3 class="text-blue-400 capitalize">Toyota</h3>
          </div>

          <div class="p-5 flex justify-between gap-12 relative cursor-pointer border-b">
            <h3>Price</h3>
            <h3 class="text-blue-400 capitalize">Any</h3>
          </div>
        </div>
        <!-- Car side bar -->

        <!-- Car cards -->
        <div class="w-full">
          <!-- Car card -->
          <div class="shadow border rounded w-full overflow-hidden mb-5 cursor-pointer h-[200px]">
            <div class="flex h-full">
              <img 
                src="https://imageio.forbes.com/specials-images/imageserve/5d35eacaf1176b0008974b54/2020-Chevrolet-Corvette-Stingray/0x0.jpg?format=jpg&crop=4560,2565,x790,y784,safe&width=1440" 
                alt=""
                class="w-[300px] h-full"
              />
              <div class="p-4 flex flex-col">
                <div>
                  <h1 class="text-2xl text-blue-700">
                    Volvo
                  </h1>
                  <p class="text-gray-700">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <h1 class="mt-auto text-xl">$39,555</h1>
              </div>
            </div>
          </div>
          <!-- Car card -->
        </div>
        <!-- Car cards -->
      </div>
    </div>
    <!-- Cars page -->
  </div>
</template>
