<template>
  <div>
    <div class="bg-white flex justify-between items-center p-4 shadow-login-card">
      <label class="text-base font-medium">All Campaigns (24)</label>
      <div>
        <BaseButton>
          <template v-slot:leftIcon>
            <PlusIcon class="h-5 w-5 mr-2" />
          </template>
          Add Campaign
        </BaseButton>
      </div>
    </div>
    <CampaignTable />
  </div>
</template>

<script setup lang="ts">
import CampaignTable from '@/components/CampaignTable.vue';
import BaseButton from '@/components/BaseButton.vue';
import { PlusIcon } from '@heroicons/vue/24/outline'
</script>
