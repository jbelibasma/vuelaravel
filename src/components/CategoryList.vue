<template>
  <table class="table caption-top">
    <thead>
        <tr>
        <th scope="col">id</th>
        <th scope="col">category</th>
        </tr>
    </thead>
    <tbody>
        <tr v-for="contact in list"
                v-bind:key="contact.id">
        <td>{{ contact.id }}</td>
        <td>{{ contact.category }}</td>
        <td><button type="submit" class="btn btn-primary">supprimer</button></td>
        <td><button type="submit" class="btn btn-primary">modifier</button></td>
        </tr>
    </tbody>
  </table>

</template>

<script>
export default {
    name: 'CategoryList',
    props: {
        list: Array
    },
}
</script>

<style>

</style>