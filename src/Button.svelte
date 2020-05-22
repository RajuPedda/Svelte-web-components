<svelte:options  tag='fpix-button' immutable={true}/>
<script>
export let label= 'button'
</script>

<div>
<button  name={label}>{label}</button>
</div>
