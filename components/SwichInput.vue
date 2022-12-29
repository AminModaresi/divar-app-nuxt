<template>
  <div class="relative inline-block w-8 h-4 cursor-pointer rounded-full">
    <input
      id="switch-component"
      type="checkbox"
      class="
        peer
        appearance-none
        w-8
        h-4
        absolute
        bg-gray-400
        rounded-full
        cursor-pointer
        transition-colors
        duration-300
        checked:bg-red-500
        peer-checked:border-red-500 peer-checked:before:bg-red-500
        right-0
      "
      checked="true"
    /><label
      for="switch-component"
      class="
        bg-white
        w-5
        h-5
        border border-blue-gray-100
        rounded-full
        shadow-md
        absolute
        top-2/4
        right-4
        -translate-y-2/4
        peer-checked:translate-x-full
        transition-all
        duration-300
        cursor-pointer
        before:content['']
        before:block
        before:bg-blue-gray-500
        before:w-10
        before:h-10
        before:rounded-full
        before:absolute
        before:top-2/4
        before:left-2/4
        before:-translate-y-2/4
        before:-translate-x-2/4
        before:transition-opacity
        before:opacity-0
        hover:before:opacity-10
        peer-checked:border-red-500 peer-checked:before:bg-red-500
      "
      ><div
        class="
          inline-block
          top-2/4
          left-2/4
          -translate-x-2/4 -translate-y-2/4
          p-5
          rounded-full
        "
        style="position: relative; overflow: hidden"
      ></div
    ></label>
  </div>
</template>