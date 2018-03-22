<template>
  <div class="test">
    <h1>{{ title }}</h1>
    <p v-if="showName">{{ user.firstName }}</p>
    <p v-else>Nobody</p>
    <ul>
      <li id="center" v-for="item in items">{{ item.title }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'test',
  data() {
    return {
      title: '<h1>Welcome to Wizzair</h1>',
      user: {
        firstName: 'John',
        lastName: 'Doe'
      },
      showName: true,
      items: [
        { title: 'Item One' },
        { title: 'Item Two' },
        { title: 'Item Three' }
      ]
    }
  }
}
</script>

<style scoped>
  #center {
    align-items: center;
    
  }
</style>
