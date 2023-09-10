<template>
  <div class="mt-7 overflow-x-auto">
    <table class="w-full whitespace-nowrap">
      <tbody>
        <tr
          tabindex="0"
          class="bg-white"
        >
          <td>
            <div class="ml-5">
              <CheckBox />
            </div>
          </td>
          <td>
            <div class="ml-5">
              <PieIcon />
            </div>
          </td>
          <td class="">
            <div class="flex flex-col pl-5 py-4">
              <p class="text-base text-btn font-bold mb-2 leading-none mr-2">SW Zero Personalization 1</p>
              <label class="text-sm text-side-nav flex items-center">
                <span class="bg-positive border rounded-full h-2 w-2 block mr-2">&nbsp;</span>
                Sent on 15th Apr 2023 | 3 Sequences
              </label>
            </div>
          </td>
          <td class="pl-5">
            <div class="flex flex-col">
              <p class="text-btn text-base font-bold mb-2">520</p>
              <label class="text-sm text-side-nav">Sent</label>
            </div>
          </td>
          <td class="pl-5">
            <div class="flex flex-col">
              <p class="text-warning text-base font-bold mb-2">39
                <span class="text-xs text-side-nav">20%</span>
              </p>
              <label class="text-sm text-side-nav">Clicked</label>
            </div>
          </td>
          <td class="pl-5">
            <div class="flex flex-col">
              <p class="text-pink text-base font-bold mb-2">202
                <span class="text-xs text-side-nav">20%</span>
              </p>
              <label class="text-sm text-side-nav">Opened</label>
            </div>
          </td>
          <td class="pl-5">
            <div class="flex flex-col">
              <p class="text-sea text-base font-bold mb-2">4
                <span class="text-xs text-side-nav">20%</span>
              </p>
              <label class="text-sm text-side-nav">Replied</label>
            </div>
          </td>
          <td class="pl-5">
            <div class="flex flex-col">
              <p class="text-positive text-base font-bold mb-2">0
                <span class="text-xs text-side-nav">20%</span>
              </p>
              <label class="text-sm text-side-nav">Positve Reply</label>
            </div>
          </td>
          <td class="pl-4">
            <button class=" text-sm leading-none text-gray-400 p-2 bg-gray-100 rounded hover:bg-gray-200">
              <PauseCircleIcon class="w-5 h-5" />
            </button>
          </td>
          <td class="pl-4">
            <button class=" text-sm leading-none text-gray-400 p-2 bg-gray-100 rounded hover:bg-gray-200">
              <PencilIcon class="w-5 h-5" />
            </button>
          </td>
          <td class="pl-4">
            <button class=" text-sm leading-none text-gray-400 p-2 bg-gray-100 rounded hover:bg-gray-200">
              <EllipsisHorizontalIcon class="w-5 h-5" />
            </button>
          </td>
        </tr>
        <tr class="h-3"></tr>
      </tbody>
    </table>
  </div>
</template>

<script setup lang="ts">
import CheckBox from './CheckBox.vue';
import PieIcon from '@/components/icons/PieIcon.vue'
import { PauseCircleIcon, PencilIcon, EllipsisHorizontalIcon } from '@heroicons/vue/24/outline'
</script>
