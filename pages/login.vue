<script setup>
definePageMeta({
  layout: "custom",
});

const supabase = useSupabaseClient();
const email = ref("");
const password = ref("");

const login = async () => {
  const { data, error } = await supabase.auth.signUp({
    email: email.value,
    password: password.value,
  });

  if (error) {
    console.log(error);
  }
};
</script>

<template>
  <div class="mt-10">
    <h1 class="text-5xl font-bold mb-7">Log in</h1>
    <form
      class="border border-gray-300 flex flex-col gap-4 p-8 rounded-lg max-w-lg mx-auto"
    >
      <input
        type="email"
        class="border p-2 rounded outline-none"
        placeholder="Email"
        v-model="email"
      />
      <input
        type="password"
        class="border p-2 rounded outline-none"
        placeholder="Password"
        v-model="password"
      />
      <button @submit.prevent="login" class="bg-red-400 p-3 rounded text-white font-bold">
        Login
      </button>
    </form>
  </div>
</template>
