<script setup>
import Header from './components/Header.vue';
import Balance from './components/Balance.vue';
import IncomeExpense from './components/IncomeExpense.vue';
import TransactionList from './components/TransactionList.vue';
import AddTransaction from './components/AddTransaction.vue';

import { ref, computed, onMounted } from 'vue';

const transactions = ref([]);

onMounted(() => {
  const savedTransactions = JSON.parse(localStorage.getItem('transactions'));

  if (savedTransactions) {
    transactions.value = savedTransactions;
  }
});
</script>


<template>
  <Header />
  <div class="container">
     <Balance :total="total" />

     <IncomeExpense :income="+income" :expense="+expense" />

     <TransactionList 
     :transactions="transactions"
      @transactionDeleted="handleTransactionDeleted" />

     <AddTransaction @transactionSubmitted="handleTransactionSubmitted" />
  </div>
</template>