<template>
    <img src="@/assets/autophoto.jpg" class="img-thumbnail" alt="autophoto.jpg">
    <br><br>
    <div>
      <button
      v-for="(button, index) in buttons"
      :key="index"
      :class="['btn', `btn-${button.variant}`, 'btn-sm', 'me-2']"
      @click="navigate(button.link)"
      :title="button.text"
    >
      <i :class="button.icon"></i>
    </button>
  </div>

</template>

<script>
export default {
  name: "SmallButtons",
  props: {
    buttons: {
      type: Array,
      required: true,
      default: () => [],
    },
  },
  methods: {
    navigate(link) {
      if (link) {
        window.location.href = link;
      }
    },
  },
};


</script>

<style>
.img-thumbnail{
    width: 350px;
    height: 300px;
}
.me-2 {
    margin-right: 0.5rem;
    }

button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  padding: 0;
  border-radius: 50%;
}
</style>