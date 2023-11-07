<template>
  <div>
    <div class="mb-4">
      <p class="...">Data Collection Form</p>
      <label>
        <span class="font-semibold mr-2">Name</span>
        <input :value="name" name="name" class="..." />
      </label>
    </div>
    <div>
      <label>
        <span class="font-semibold mr-2">Email</span>
        <input type="email" :value="email" name="email" />
      </label>
    </div>
    <div class="flex pl-24">
      <button class="..." @click.prevent="submitChange">Update</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "FormComponent",
  props: {
    name: {
      type: String,
      required: true,
    },
    email: {
      type: String,
      require: true,
    },
  },
  methods: {
    submitChange() {
      console.log(`You're updating ${this.name} and ${this.email}`);
    },
  },
};
</script>
