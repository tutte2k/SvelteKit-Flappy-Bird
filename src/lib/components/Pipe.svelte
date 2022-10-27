<script lang="ts">
    import type {PipePair} from './Game'
    export let pipe: PipePair;
</script>


<style>
    .pipe{
        position:absolute;
        background-color: grey;
    }
</style>

{#if pipe.show }
<section
  style="left: {pipe.left}px; top: {pipe.topPipe.top}px; width: {pipe.width}px; height: {pipe.topPipe.height}px;"
  class="top-pipe pipe"
></section>
<section
  style="left: {pipe.left}px; top: {pipe.bottomPipe.top}px; width: {pipe.width}px; height: {pipe.bottomPipe.height}px;"
  class="top-bottom pipe"
></section>
{/if}