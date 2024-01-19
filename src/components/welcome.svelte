<!-- 
<script>
   export let value;
   export let age;
</script>

<h1>{value} : {age}</h1> -->

<!-- <div>
   <slot>
      Default
   </slot>
</div> -->

<div class="card">
   <div class="header">
      <slot name="header"/>
   </div>
   <div class="content">
      <slot name="content"/>
   </div>
   {#if $$slots.footer}
   <hr/>
   <div class="footer">
      <slot name="footer"/>
   </div>
   {/if}
</div>