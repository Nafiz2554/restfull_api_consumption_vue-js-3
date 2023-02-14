<template>
  <div>
    <div class="card">
      <div class="card-header">
        <h4>Students <router-link class="btn btn-primary float-end" to="student/create">Add Student</router-link></h4>
      </div>
      <div class="card-body">
        <table class="table table-bordered">
          <thead>
             <tr>
              <th>Id</th>
              <th>Name</th>
              <th>Course</th>
              <th>Email</th>
              <th>Phone</th>
              <th>Created at</th>
              <th>Action</th>
             </tr>
          </thead>
          <tbody>
            <tr>

            </tr>
          </tbody>

        </table>
      </div>
    </div>
  </div>
</template>
<script>
import axios from 'axios';
export default{
  name:'students',
  data(){
    return {
      students:[]
    }
  },
  mounted(){
    this.getStudents();
    //console.log('I am here')
  },
  methods: {
    getStudents(){
      axios.get('').then(res=>{
        console.log(res)

      });
    }
  }
};
</script>
