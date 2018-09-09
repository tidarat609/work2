<template>
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
        <td>{{ props.item.s_code }}</td>
<<<<<<< HEAD
        <td class="text-xs-lelt">{{ props.item.s_cord }}</td>
        <td class="text-xs-lelt">{{ props.item.s_name }}</td>
        <td class="text-xs-lelt">{{ props.item.s_class }}</td>
        <td class="text-xs-lelt">{{ props.item.s_group }}</td>
        <td class="text-xs-lelt">{{ props.item.s_iron }}</td>
      </template>
    </v-data-table>
    <div>
      <v-btn color="success">เพิ่มข้อมูล</v-btn>
      <v-btn color="error">ลบข้อมูล</v-btn>
    </div>
=======
        <td class="text-xs-left">{{ props.item.s_name }}</td>
        <td class="text-xs-left">{{ props.item.s_class }}</td>
        <td class="text-xs-left">{{ props.item.s_group }}</td>
      </template>
    </v-data-table>
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
  </div>
</template>
<script>
export default {
  data () {
    return {
      headers: [
        {
          text: 'รหัสนักศึกษา',
          align: 'left',
          sortable: false,
          value: 'name',
        },
<<<<<<< HEAD
        { text: '', value: '' },
        { text: 'ชื่อ-นามสกุล', value: 'fat' },
        { text: 'แผนกวิชา', value: 'carbs' },
        { text: 'กลุ่ม', value: 'protein' },
        { text: 'หมายเหตุ', value: 'iron' },
=======
        { text: 'ชื่อนักศึกษา', value: 'ชื่อนักศึกษา' },
        { text: 'แผนกวิชา', value: 'แผนกวิชา' },
        { text: 'คะแนนที่ได้', value: 'คะแนนที่ได้' },
        
       
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
      ],
      desserts: [],
    }
  },
async created() {
    this.getstudent()
  }, 
methods: {
    async getstudent() {
      let res = await this.$http.get('http://127.0.0.1/php-api/list-student.php')
      this.desserts = res.data.student
    },
}
}
<<<<<<< HEAD
</script>
=======
</script>
>>>>>>> 438d09dd7dedb8a1b26fd5e203144e4f78eaaafb
