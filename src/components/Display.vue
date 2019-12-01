<template>
    <div class="display">
        {{ value | exponential }}
    </div>
</template>

<script>
export default {
    props: ['value'],
    filters: {
        exponential(number) {
            if(number.length > 8) {
                return parseFloat(number).toExponential(4)
            } else {
                return number
            }
        }
    },
}
</script>

<style>
    .display {
        grid-column: span 4;
        background-color: #0004;

        display: flex;
        justify-content: flex-end;
        align-items: center;
        padding: 20px;
        font-size: 2em;
        overflow: hidden;
    }
</style>