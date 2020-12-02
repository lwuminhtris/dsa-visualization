<template>
  <v-container>
    <v-row align="center" no-gutters style="padding-top: 80px;">
      <v-col>
      </v-col>
      <v-col md="0" alignSelf="center">
        <v-card
          width="600px"
          height="500px"
        >
        <v-card-title>
          <img src="../assets/gaia.png" style = "height: 20px;" />
          <v-spacer>

          </v-spacer>
          Data Structure Visualization
        </v-card-title>
        <v-tabs>
          <v-tab
            v-for="item in items"
            :key="item"
          >
            {{item}}
          </v-tab>

          <v-tab-item>
            <v-text-field
              placeholder="Your array"
              solo
              style = "margin-left: 20px; margin-right: 20px; margin-top: 20px;" 
              dark
            >
              
            </v-text-field>
          </v-tab-item>

          <v-tab-item>

          </v-tab-item>
        </v-tabs>
        </v-card>
      </v-col>
      <v-col>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      items: ['Binary Search Tree', 'AVL Tree', 'Heap', 'Hash'],
      detail: ['BST', 'AVL', 'HEAP', 'HASH']
    }),
  }
</script>
