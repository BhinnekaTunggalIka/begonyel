<template>
  <div id="SearchBar">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="input-group flex-nowrap">
            <input
              type="text"
              class="form-control"
              placeholder="Mau makan apa hari ini..."
              aria-label="Mau makan apa hari ini..."
              aria-describedby="addon-wrapping"
            />
            <span class="input-group-text" id="addon-wrapping"
              ><i class="fas fa-search"></i
            ></span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SearchBar",
};
</script>