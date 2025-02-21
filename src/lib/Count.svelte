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

    <button onclick={increment} 
    id="i-button">
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
    </button>
    <button onclick={decrement} 
    id="d-button">
    -
    </button>

    {#if count > 10}
        <p>{count} is greater than 10</p>
    {:else if count > 5}
        <p>{count} is greater than 5</p>
    {:else}
        <p>{count} is between 5 and 10</p>
    {/if}
</h1>