<template>
<<<<<<< HEAD
<div>
  <v-data-table
    :headers="headers"
    :items="desserts"
    class="elevation-1"
  >
    <template slot="items" slot-scope="props">
=======
  <div>
    <v-data-table
      :headers="headers"
      :items="desserts"
      class="elevation-1"
    >
      <template slot="headerCell" slot-scope="props">
        <v-tooltip bottom>
          <span slot="activator">
            {{ props.header.text }}
          </span>
          <span>
            {{ props.header.text }}
          </span>
        </v-tooltip>
      </template>
      <template slot="items" slot-scope="props">
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
      <td>{{ props.item.b_id }}</td>
      <td class="text-xs-center">{{ props.item.b_name }}</td>
      <td class="text-xs-center">{{ props.item.b_group }}</td>
      <td class="text-xs-center">{{ props.item.b_price }}</td>
<<<<<<< HEAD

    </template>
    <template slot="pageText" slot-scope="props">
    Lignes {{ props.pageStart }} - {{ props.pageStop }} de {{ props.itemsLength }}
    </template>
  </v-data-table>
  <div>
    <v-btn color="brown lighten-1">แก้ไขข้อมูล</v-btn>
    <v-btn color="brown lighten-1">เพิ่มข้อมูล</v-btn>
    <v-btn color="error">ลบ</v-btn>
  </div>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        headers: [
=======
      </template>
    </v-data-table>
    <div>
    <v-btn color="brown lighten-1">แก้ไขข้อมูล</v-btn>
    <v-btn color="brown lighten-1">เพิ่มข้อมูล</v-btn>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      headers: [
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
          {
            text: 'B_ID',
            align: 'left',
            sortable: false,
            value: 'name'
          },
          { text: 'B_Name', value: 'B_Name', align: 'center' },
          { text: 'B_Group', value: 'B_Group', align: 'center' },
          { text: 'B_Price', value: 'B_Price', align: 'center' },
        ],
<<<<<<< HEAD
        desserts: [],
      }
    },
    async created() {
=======
      desserts: [],
    }
  },
async created() {
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
    this.getstudent()
  }, 
methods: {
    async getstudent() {
<<<<<<< HEAD
      let res = await this.$http.get('http://127.0.0.1/php-test1/list-book.php')
      this.desserts = res.data.student
    },
    
},
  }
=======
      let res = await this.$http.get('127.0.0.1/php-test1/list_book.php')
      this.desserts = res.data.student
    },
}
}
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
</script>