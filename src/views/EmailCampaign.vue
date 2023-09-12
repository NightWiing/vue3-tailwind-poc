<template>
  <div>
    <div class="bg-white flex justify-between items-center py-4 px-5 shadow-login-card">
      <label class="text-base font-medium">All Campaigns (24)</label>
      <div class="flex items-center">
        <BaseInput
          v-model="search"
          class="mr-16 w-[264px]"
          placeholder="Search Campaign"
          @input="searchCampaign($event)"
        >
          <template v-slot:leftIcon>
            <MagnifyingGlassIcon class="w-6 h-6 text-[#696D8B]" />
          </template>
        </BaseInput>
        <BaseButton>
          <template v-slot:leftIcon>
            <PlusIcon class="h-5 w-5 mr-2" />
          </template>
          Add Campaign
        </BaseButton>
      </div>
    </div>
    <CampaignTable :data="data" />
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import CampaignTable from '@/components/CampaignTable.vue';
import BaseButton from '@/components/BaseButton.vue';
import BaseInput from '@/components/BaseInput.vue';
import { PlusIcon, MagnifyingGlassIcon } from '@heroicons/vue/24/outline'
import { campaigns } from '@/stores/DB.json'

const data = ref(campaigns)
const search = ref('')

const searchCampaign = (val: any) => {
  if (val.target.value.length >= 3) {
    const res = data.value.filter(d => d.name.toLocaleLowerCase().includes(val.target.value))
    data.value = res;
  } else if (val.target.value.length === 0) {
    data.value = campaigns
  }
}
</script>
