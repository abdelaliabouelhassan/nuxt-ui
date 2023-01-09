<template>
  <div class="w-full h-screen p-10 bg-[#28293D] space-y-4">
    <span class=" text-white text-base">{{opt}}</span>
    <DropDown v-model="opt" :options="options" />
  </div>
</template>

<script>
import DropDown from "@/components/UI/DropDown.vue";
export default {
  name: "IndexPage",
  components: {
    DropDown,
  },
  data() {
    return {
      opt: "easy",
      options: ["easy", "Average", "Hard", "Severe"],
    };
  },
};
</script>
