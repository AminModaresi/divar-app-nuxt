<template>
  <nav class="my-5">
    <div class="container px-2 mx-auto">
      <div class="bg-white py-4 px-6 flex justify-between items-center rounded-xl shadow">
        <p class="text-xl font-bold text-red-600">دیوار</p>
        <ul class="text-sm flex gap-5">
          <li>نشان‌ها</li>
          <li>یادداشت‌ها</li>
          <li>بازدیدهای اخیر</li>
          <li>دیوار برای کسب‌وکارها</li>
        </ul>
        <button
          class="
            middle
            none
            font-bold
            center
            uppercase
            transition-all
            disabled:opacity-50
            disabled:shadow-none
            disabled:pointer-events-none
            text-xs
            py-2
            px-3
            rounded-lg
            bg-gradient-to-tr
            from-red-600
            to-red-400
            text-white
            shadow-md shadow-red-500/20
            hover:shadow-lg hover:shadow-red-500/40
            active:opacity-[0.85]
          "
        >
          ثبت اگهی
        </button>
      </div>
    </div>
  </nav>
  <div>
    <div class="container px-2 mx-auto">
        <div class="flex flex-wrap">
            <aside class="hidden lg:block lg:w-3/12 pl-6">
                <div class="h-[100vh - 400px] bg-white p-5 rounded-lg shadow">
                    <SwichInput />
                </div>
            </aside>
            <main class="w-full lg:w-9/12">
                <slot />
            </main>
        </div>
    </div>
  </div>
</template>