<template>
  <div class="webinar-registration-form-wrapper">
    <form class="webinar-registration-form">
      <div class="form-control">
        <div class="control-label">
          <label>Name</label>
        </div>
        <div class="control-input">
          <input type="text" name="name" placeholder="Name">
        </div>
      </div>
      <div class="form-control">
        <div class="control-label">
          <label>Email</label>
        </div>
        <div class="control-input">
          <input type="email" name="email" placeholder="Email">
        </div>
      </div>
      <div class="form-control">
        <button class="btn btn-blue w-full">
          RESERVE MY SPOT NOW
        </button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'WebinarRegistrationForm'
}
</script>

<style>
.form-control {
  @apply py-2
}
.control-input input {
  @apply border border-gray-400 py-3 px-4 w-full
}
.btn {
  @apply font-bold py-2 px-4 rounded
}
.btn-blue {
  @apply bg-blue-500 text-white
}
.btn-blue:hover {
  @apply bg-blue-700
}
</style>
