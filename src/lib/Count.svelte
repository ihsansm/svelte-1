<script>
    let count = $state(0)
    const increment = () => {
        count += 1
    }
    const decrement = () => {
        count -= 1
    }
</script>

<h1>
    count : {count}
    <br>

    <br>
    
    <button onclick={increment}>+</button>
    <button onclick={decrement}>-</button>
</h1>