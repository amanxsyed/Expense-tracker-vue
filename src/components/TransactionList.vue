<template>
    <h3>History</h3>
    <ul id="list" class="list">
        <li v-for="t in transactions" :key="t.id">
            {{  t.text }} <span>${{ t.amount }}</span>
        </li>
        <button class="delete-btn">x</button>
        <!-- <li class="minus">
            Cash <span>-$400</span>
            <button class="delete-btn">x</button>
        </li>
        <li class="plus">
            paycheck <span>$800</span>
            <button class="delete-btn">x</button>
        </li> -->
    </ul>
</template>

<script>
    export default {
        data() {
            return {
                transactions:[
                    { id: 1, text: 'Flower', amount: -400 },
                    { id: 2, text: 'Salary', amount: 800 },
                    { id: 3, text: 'Book', amount: -40 },
                    { id: 4, text: 'Camera', amount: -200 }
                ]
            }

        }
    }
</script>