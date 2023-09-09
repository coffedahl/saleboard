<script lang="ts">
	export let title: string
    export let data: any
</script>

<div>
	<h1>{title}</h1>
	<h2>{data}</h2>
</div>

<style lang="scss">
    div{
        background-color: transparent;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>