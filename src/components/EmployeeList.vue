<template>
  <ol class="employee-list">
    <li 
      v-for="(employee, index) in employees" 
      :key="index" 
      class="employee-item"
    >
      {{ employee.name }}
    </li>
  </ol>
</template>

<script>
export default {
  name: 'EmployeeList',
  data() {
    return {
      employees: [
        { name: 'Assa Baradji' },
        { name: 'Thillo Sem' },
        { name: 'Aichetou Sy' },
        { name: 'Fatima Cissé' }
      ]
    };
  }
};
</script>

<style scoped>
.employee-list {
  list-style-type: decimal;
  padding: 0;
  margin: 20px;
  width: 300px;
 
}

.employee-item {
  background-color: #f9f9f9;
  margin: 10px 0;
  padding: 20px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.employee-item:hover {
  background-color:#2d4768  ;
  cursor: pointer;
  color: #f9f9f9;
}
</style>
