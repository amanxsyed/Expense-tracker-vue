<template>
    <Header />
    <div class="container">
        <Balance />
        <IncomeExpenses />
        <TransactionList />
        <AddTransactions />

    </div>
</template>

<script>
    import Header from './components/Header.vue'
    import Balance from './components/Balance.vue'
    import IncomeExpenses from './components/IncomeExpenses.vue'
    import TransactionList from './components/TransactionList.vue'
    import AddTransactions from './components/AddTransactions.vue'

    export default {
        components: {
            Header,
            Balance,
            IncomeExpenses,
            TransactionList,
            AddTransactions,
        },
    };
</script>