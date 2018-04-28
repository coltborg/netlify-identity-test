<template>
  <div class="flex justify-center items-center">
    <main class="mt-26 ml-22 pt-8 font-light text-center">
      <div class="flex justify-around mr-4 sm:ml-8 sm:mr-16 md:ml-16 md:mr-24 lg:ml-36 lg:mr-16 text-2xl md:text-3xl lg:text-5xl xl:text-6xl">
        <a href="#" class="flex-1 text-blue no-underline py-4 border-t-4 border-transparent hover:border-t-4 hover:border-blue-light">
          <div class="tracking-wide">$0</div>
          <div class="text-sm text-grey-dark">overdue</div>
        </a>
        <a href="#" class="flex-1 text-blue no-underline py-4 border-t-4 border-transparent hover:border-t-4 hover:border-blue-light">
          <div class="tracking-wide">$0</div>
          <div class="text-sm text-grey-dark truncate">total outstanding</div>
        </a>
        <a href="#" class="flex-1 text-blue no-underline py-4 border-t-4 border-transparent hover:border-t-4 hover:border-blue-light">
          <div class="tracking-wide">$0</div>
          <div class="text-sm text-grey-dark">in draft</div>
        </a>
      </div>

      <div class="flex flex-col mt-8 mr-4 sm:ml-10 md:ml-24 lg:ml-48 text-left">
        <h2 class="font-light text-lg mb-4">Recently Active</h2>

        <div class="flex flex-col sm:flex-row flex-wrap">
          <div class="flex-shrink sm:w-64 mb-6 sm:mr-6">
            <div class="flex flex-col">
              <a href="#" class="no-underline">
                <div class="border-t-8 border-pink-light rounded-t-lg"></div>
                <div class="border-b border-l border-r border-grey shadow-md rounded-b-lg p-4">
                  <div class="flex">
                    <div class="flex justify-center items-center text-lg border-2 border-pink-light text-pink-light rounded-full w-12 h-12 font-medium">BA</div>
                    <div class="flex flex-col ml-8 mt-1">
                      <div class="flex-1 text-black">Bud Abbott</div>
                      <div class="flex-1 text-xs text-grey mt-2">Old School Comedy</div>
                      <div class="flex-1 text-xs text-grey mt-4">
                        <i class="far fa-envelope"></i>
                        <span>bud@abbott.com</span>
                      </div>
                      <div class="flex-1 text-xs text-grey mt-2">
                        <i class="fas fa-phone"></i>
                        <span>111-222-3333</span>
                      </div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>

          <div class="flex-shrink sm:w-64 mb-6 sm:mr-6">
            <div class="flex flex-col">
              <a href="#" class="no-underline">
                <div class="border-t-8 border-purple-light rounded-t-lg"></div>
                <div class="border-b border-l border-r border-grey shadow-md rounded-b-lg p-4">
                  <div class="flex">
                    <div class="flex justify-center items-center text-lg border-2 border-purple-light text-purple-light rounded-full w-12 h-12 font-medium">LC</div>
                    <div class="flex flex-col ml-8 mt-1">
                      <div class="flex-1">Lou Costello</div>
                      <div class="flex-1 text-xs text-grey mt-2">Old School Comedy</div>
                      <div class="flex-1 text-xs text-grey mt-4">
                        <i class="far fa-envelope"></i>
                        <span>lou@costello.com</span>
                      </div>
                      <div class="flex-1 text-xs text-grey mt-2">
                        <i class="fas fa-phone"></i>
                        <span>444-555-6666</span>
                      </div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>

          <div class="flex-shrink sm:w-64 mb-6 sm:mr-6">
            <div class="flex flex-col">
              <a href="#" class="no-underline">
                <div class="border-t-8 border-blue-light rounded-t-lg"></div>
                <div class="border-b border-l border-r border-grey shadow-md rounded-b-lg p-4">
                  <div class="flex">
                    <div class="flex justify-center items-center text-lg border-2 border-blue-light text-blue-light rounded-full w-12 h-12 font-medium">TH</div>
                    <div class="flex flex-col ml-8 mt-1">
                      <div class="flex-1">Tim Hawkins</div>
                      <div class="flex-1 text-xs text-grey mt-2">New School Comedy</div>
                      <div class="flex-1 text-xs text-grey mt-4">
                        <i class="far fa-envelope"></i>
                        <span>tim@hawkins.com</span>
                      </div>
                      <div class="flex-1 text-xs text-grey mt-2">
                        <i class="fas fa-phone"></i>
                        <span>999-888-7777</span>
                      </div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="flex flex-col mt-6 text-center">
        <div class="flex-1">
          <button class="border-2 border-grey-light hover:bg-grey-light rounded-lg text-xs py-1 px-2 text-grey-darker">View Archived Clients</button>
        </div>
        <div class="flex-1 mt-2 text-xs text-grey-dark">
          or <a href="#" class="text-grey-dark">deleted</a>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "Content"
};
</script>
