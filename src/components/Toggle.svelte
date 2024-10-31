<script>
  let { key, size } = $props();

  let selected = $state(false);
  let color = $derived(selected ? 'red' : 'navy');

  const handleClick = () => {
    selected = !selected;
  };
</script>

<div
  class={`ikon ${color}`}
  onclick={handleClick}
  onkeydown={e => e.key === 'Enter' && handleClick()}
  width={size}
  height={size}
  title={key}
  role="button"
  tabindex="0"
  aria-label="title"
  {selected}
>
  <proto-ikon-loader name={key} {size}></proto-ikon-loader>
</div>

<style>
  .ikon {
    display: flex;
    margin: 5px;
  }

  .navy {
    color: var(--clrs-navy);
  }

  .red {
    color: var(--clrs-red);
  }
</style>
