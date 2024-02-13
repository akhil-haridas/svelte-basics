<script>
  import { shuffle } from "lodash";......
  import Welcome from "./components/welcome.svelte";
  import Names from "./components/names.svelte";
  import Mount from "./components/mount.svelte";
  import Fetchtodo from "./components/fetchtodo.svelte";
  // const mobileCompanies = ["Apple","Pixel","Nothing","Samsung","OnePlus"];
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
    numbers = [...numbers,5]
  }

  $: sum = numbers.reduce((total,curr)=> (total+curr),0)


let volume =0;

$:if(volume > 20){
  volume = 20
  alert("Max limit is 20")
}else if (volume < 0){
  volume = 0
  alert("Min limit is 0")
}

let age = 23;

</script>

<Fetchtodo/>

<!-- <Mount/> -->

<!-- 
<Names let:firstName let:lastName>
  <h1>{firstName} : {lastName}</h1>
</Names> -->

<!-- <div>
  <Welcome>
    <div slot="header">
      <h1>Hi</h1>
    </div>
    <div slot="content">
      <h2>I'm AKhil K</h2>
    </div>
    <div slot="footer">
      <p>I'm a Full stack Developer</p>
    </div>
  </Welcome>
    <Welcome>
    <div slot="header">
      <h1>Hi</h1>
    </div>
    <div slot="content">
      <h2>I'm AKhil K</h2>
    </div>
  </Welcome>
</div> -->

<!-- <div>
  <Welcome>
    <h1>Hi</h1>
  </Welcome>
  <Welcome>
    <p>I'm a MERN Stack Developer</p>
  </Welcome>
  <Welcome>

  </Welcome>
</div> -->

<!-- <div>
  <Welcome value="Hi" {age} />
  <Welcome value="Hi i'm" {age} />
  <Welcome value="Hi i'm Akhil!"{age} />
</div> -->

<!-- <div>
  <h1>VOLUME : {volume}</h1>
  <button on:click={()=> volume = volume + 1}>Increase Button</button>
  <button on:click={()=> volume = volume - 1}>Decrease Button</button>
</div> -->

<!-- 
<div>
	<button type="button" on:click={shuffleArray}>SHUFFLE</button>
  {#each mobileCompanies as company (company.name)}
    <h1>{company.name}</h1>
    <input type="text" placeholder="Enter name" />
  {/each}
</div> -->


<!-- <div>
  <h1>Event Handling in svelte</h1>
  <h2>Count : {count}</h2>
  <h2>Doubled : {doubled}</h2>
  <h2>Sum : {sum}</h2>
  <button on:click={addby5}>Addby5</button>
  <button on:click={increment}>+</button>
  <button on:click={addon}>Addon</button>
</div>  -->
