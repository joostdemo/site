<template>
  <div>
    <blockquote>
    <h3>{{ $t('youAreNotLoggedIn') }}</h3>
    <p>
      {{ $t('thisPageIsOnlyAvailableToFreesewingUsers') }}
    </p>
    <div class="mt-5">
    <v-btn :to="$fs.path('/login')" large color="primary" class="mb-3">
      <v-icon class="mr-3">vpn_key</v-icon>
      {{ $t('logIn') }}
    </v-btn>
    <v-btn large class="mb-3" :to="$fs.path('/signup')">
      <v-icon class="mr-3">undo</v-icon>
      {{ $t('signUp') }}
    </v-btn>
    </div>
    </blockquote>
  </div>
</template>

<script>
export default {
  name: 'FsMessageLoginRequired'
}
</script>

<style scoped>
  blockquote {
    max-width: 800px;
    margin: 40px auto;
    text-align: center;
  }
</style>

