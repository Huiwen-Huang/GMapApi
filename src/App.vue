<template>
  <MapsApi />
  <!-- Open the modal using ID.showModal() method -->
  <button class="btn" onclick="my_modal_2.showModal()">open modal</button>
  <dialog id="my_modal_2" class="modal">
    <div class="modal-box">
      <form method="dialog">
        <button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
      </form>
      <h3 class="text-lg font-bold">Hello!</h3>
      <p class="py-4">Press ESC key or click outside to close</p>
    </div>
    <form method="dialog" class="modal-backdrop">
      <button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
      <button>close</button>
    </form>
  </dialog>
</template>

<script>
import MapsApi from './components/MapsApi.vue'
import { BeakerIcon } from '@heroicons/vue/24/solid'

export default{
  data() {
    return {
      text: 'Hello'

    }
  },
  components: {
    MapsApi,
    BeakerIcon
  }
}
</script>