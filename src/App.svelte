<script>
  import { shuffle } from "lodash";
  // const mobileCompanies = ["Apple","Pixel","Nothing","Samsung","OnePlus"]
  let mobileCompanies = [
    { name: "Apple" },
    { name: "Pixel" },
    { name: "Nothing" },
    { name: "Samsung" },
    { name: "OnePlus" },
  ];

  const shuffleArray = () => {
    mobileCompanies = shuffle(mobileCompanies);
  };

  let count = 0 ;
  let addOn = 5
  $: doubled = count * 2

  let numbers = [1,2,3,4,5]

  const increment = ()=> {
    count++ ;
  }

  const addon = ()=> {
    if(addOn) count = count + addOn
  }

  const addby5 = ()=> {
    
  }
</script>
<!-- 
<div>
	<button type="button" on:click={shuffleArray}>SHUFFLE</button>
  {#each mobileCompanies as company (company.name)}
    <h1>{company.name}</h1>
    <input type="text" placeholder="Enter name" />
  {/each}
</div> -->


<div>
  <h1>Event Handling in svelte</h1>
  <h2>Count : {count}</h2>
  <h2>Doubled : {doubled}</h2>
  <button on:click={addby5}>Addby5</button>
  <button on:click={increment}>+</button>
  <button on:click={addon}>Addon</button>
</div> 