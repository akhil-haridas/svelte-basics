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
  let addOn
  const increment = ()=> {
    count++ ;
  }

  const addon = ()=> {
    if(addOn) count = count + addOn
    window.alert("Please enter a value")
  }

  const inputHandler = (e) => {
    if (e.target.name === 'add-on'){
      addOn=Number(e.target.value)
  }
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
  <button on:click={increment}>+</button>
  <input type="number" onchange={inputHandler} name="add-on" />
  <button on:click={addon}>Addon</button>
</div> 