<template lang="">
  <div class="mt-8">
    <div class="container mx-auto px-8">
      <!-- Start: Form -->
      <form
        class="flex flex-col justify-start space-y-6"
        @submit.prevent="onSubmit"
      >
        <div class="row">
          <label for="fullname" class="flex flex-col">
            <span class="">fullname</span>
            <input
              type="text"
              name="fullname"
              id="fullname"
              class="px-4 py-3 rounded-lg rounder-lg border border-gray-100 mt-1"
              placeholder="imoney..."
            />
          </label>
        </div>
        <div class="row">
          <label for="email" class="flex flex-col">
            <span class="">Email address</span>
            <input
              autocomplete="username"
              type="email"
              name="email"
              id="email"
              class="px-4 py-3 rounded-lg rounder-lg border border-gray-100 mt-1"
              placeholder="email..."
            />
          </label>
        </div>
        <div class="row">
          <label for="password" class="flex flex-col">
            <span class="">Email address</span>
            <input
              autocomplete="current-password"
              type="password"
              name="password"
              id="password"
              class="px-4 py-3 rounded-lg rounder-lg border border-gray-100 mt-1"
              placeholder="password..."
            />
          </label>
        </div>
        <div class="row">
          <button
            class="py-3 text-center text-white font-bold rounded-lg bg-primary w-full"
            type="submit"
          >
            Sign Up
          </button>
        </div>
      </form>

      <!-- Start: Direction -->
      <div class="w-full text-center mt-6">
        <span class="font-semibold">I'm already a member.</span>
        <span class="ml-1">
          <router-link
            :to="{ name: 'Login', params: {} }"
            class="text-primary font-bold"
            >Sign In</router-link
          >
        </span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "register-page",
  setup() {
    function onSubmit() {}
    return {
      onSubmit,
    };
  },
};
</script>
