<template>
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
                        <img src="https://imageio.forbes.com/specials-images/imageserve/5d35eacaf1176b0008974b54/2020-Chevrolet-Corvette-Stingray/0x0.jpg?format=jpg&crop=4560,2565,x790,y784,safe&width=1440"
                            alt="" class="w-[300px] h-full" />
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
</template>