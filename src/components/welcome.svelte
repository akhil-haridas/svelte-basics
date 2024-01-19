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
      <slot/>
   </div>
   <div class="content">
      <slot/>
   </div>
   <div class="footer">
      <slot/>
   </div>
</div>