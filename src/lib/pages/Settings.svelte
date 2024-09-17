<script>
  import settings from "../stores/settings";
</script>

<h2>Settings</h2>
<h2>
  {$settings.colorScheme}
</h2>
<button
  on:click={() => {
    $settings.colorScheme = $settings.colorScheme === "dark" ? "light" : "dark";
  }}>toggle color scheme</button
>
<label for="dark">
  <input
    type="radio"
    bind:group={$settings.colorScheme}
    name="colorScheme"
    id=""
    value="dark"
  /> Dark
</label>
<label for="light">
  <input
    type="radio"
    bind:group={$settings.colorScheme}
    name="colorScheme"
    id=""
    value="light"
  /> Light
</label>
