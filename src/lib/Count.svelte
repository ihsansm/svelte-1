<script>
    let count = $state(0)
    const increment = () => {
        count += 1
    }
    const decrement = () => {
        if (count > 0) {
            count -= 1
        }
    }
</script>

<h1>
    count : {count}
    <br>

    <br>

    <button onclick={increment} id="i-button">+</button>
    <button onclick={decrement} id="d-button">-</button>
</h1>