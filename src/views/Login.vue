<template>
    <v-container fill-height style="max-width:400px">
        <v-layout align-center row rwap>
            <v-flex xs12>
            <v-card>
              <v-toolbar flat height="30" class="pa-3">
                <v-toolbar-title>Login</v-toolbar-title>
                <v-spacer></v-spacer>
              </v-toolbar>
              <div class="pa-3">
              <v-text-field
                  v-model="email"
                  label="email@sample.com"
          ></v-text-field>
          <v-text-field
                  v-model="password"
                  type="password"
                  label="password"
          ></v-text-field>
          <v-btn block large depressed color="cyan accent"
            @click="login">Login</v-btn>
              </div>
          </v-card>
          </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default ({
  data () {
    return {
      email: null,
      password: null,
      allUsers: [
        { id: 1, name: 'ej', email: 'abc@adw.com', password: '1234' },
        { id: 1, name: 'ej1', email: 'abc@def.com', password: '1234' },
        { id: 1, name: 'ej2', email: 'abc@adw.com', password: '1234' }
      ]
    }
  },
  methods: {
    login () {
      alert()
    }
  }
})
</script>
