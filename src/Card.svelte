<svelte:options tag="fpix-card" immutable= {true} />
<script>
export let title = 'Add title here';
export let content = 'Add Card content here';
export let count = 0;

function sayHi() {
    this.dispatchEvent(new CustomEvent('hi', {composed: true}));
}
</script>

<div class="card">
    <h1>{title}</h1>
    <p>{content}</p>
    {count}

    <button on:click= {()=> count++ }>count</button>
    <button>send message</button>
</div>

<style>
.card{
    border: solid #FF22FF 3px;
    box-shadow: 1px 1px;
    border-radius: 10px;
    width: 220px;
    padding: 5px;
    text-align: center;
}
</style>
