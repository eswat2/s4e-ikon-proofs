<script>
  import Toggle from "./Toggle.svelte"
  import { navy } from "../utils"

  export let size = undefined

  const Keys = [
    "acura",
    "alfa-romeo",
    "am-general",
    "aston-martin",
    "audi",
    "bently",
    "bmw",
    "bugatti",
    "buick",
    "cadillac",
    "chevrolet",
    "chrysler",
    "citroen",
    "daewoo",
    "dodge",
    "eagle",
    "ferrari",
    "fiat",
    "fisker",
    "ford",
    "genesis",
    "geo",
    "gmc",
    "honda",
    "hummer",
    "hyundai",
    "infiniti",
    "isuzu",
    "jaguar",
    "jeep",
    "kia",
    "lamborghini",
    "land-rover",
    "lexus",
    "lincoln",
    "lotus",
    "maserati",
    "maybach",
    "mazda",
    "mclaren",
    "mercedes-benz",
    "mercury",
    "mini",
    "mitsubishi",
    "nissan",
    "oldsmobile",
    "opel",
    "panoz",
    "peugeot",
    "plymouth",
    "pontiac",
    "porsche",
    "ram",
    "renault",
    "rolls-royce",
    "saab",
    "saturn",
    "scion",
    "seat",
    "skoda",
    "smart",
    "spyder",
    "subaru",
    "suzuki",
    "tesla",
    "toyota",
    "volkswagen",
    "volvo",
  ]
</script>

<div class="proofs">
  {#each Keys as key}
    <Toggle hex={navy} {key} {size} />
  {/each}
</div>

<style>
  .proofs {
    display: flex;
    justify-content: center;
    align-content: center;
    flex-wrap: wrap;
    width: 100%;
    padding-bottom: 100px;
  }
</style>
