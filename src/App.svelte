<!-- <script>
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
</script>

<div>
	<button type="button" on:click={shuffleArray}>SHUFFLE</button>
  {#each mobileCompanies as company (company.name)}
    <h1>{company.name}</h1>
    <input type="text" placeholder="Enter name" />
  {/each}
</div> -->


<div>
  <h1>Event Handling in svelte</h1>
</div>