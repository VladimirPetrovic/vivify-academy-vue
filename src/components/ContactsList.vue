<template>
  <div>
    <h1>Contacts</h1>
    <table>
      <thead>
        <th>First Name</th>
        <th>Last Name</th>
        <th>Email Name</th>
      </thead>
      <tbody>
        <tr v-for="(contact, key) in contacts" :key="key">
          <td>{{ contact.first_name }}</td>
          <td>{{ contact.last_name}}</td>
          <td>{{ contact.email }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'ContactsList',
  data() {
    return {
      contacts: [
        { first_name: "John", last_name: "Johnson", email: "john@gmail.com"},
        { first_name: "Jack", last_name: "Jackson", email: "jack@gmail.com"},
        { first_name: "Patric", last_name: "Pat", email: "patrick@gmail.com"}
      ]
    }
  }
}
</script>

<style>

</style>
