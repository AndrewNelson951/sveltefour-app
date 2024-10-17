<script>
  import Face from "./Face.svelte";
  import Container from "./Container.svelte";

  let say = 'hi';
  setTimeout(() => {
    say = 'bye';
    }, 1000);
</script>

<Container>
<div>
    Say: {say}
</div>

<Face size={4} index={1}/>
<Face />
<Face size={10} index={2}/>
</Container>



<style>
    div {
        color: red;
    }
    :global(*) {
		box-sizing: border-box;
	}
	:global(body, html) {
		margin: 0;
		height: 100vh;
		overflow: hidden;
	}
</style>

