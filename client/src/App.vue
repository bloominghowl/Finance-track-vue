<script setup>
import Header from './components/Header.vue';
import Balance from './components/Balance.vue';
import IncomeExpenses from './components/IncomeExpense.vue';
import TransactionList from './components/TransactionList.vue';
import AddTransaction from './components/AddTransaction.vue';

import { ref, computed, onMounted } from 'vue';
</script>

<template>
  <Header />
  <Balance />
  <IncomeExpense />
  <TransactionList />
  <AddTransaction />
</template>
