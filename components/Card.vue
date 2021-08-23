<template>
  <div class="col-md-4">
    <div class="card mb-4 shadow-sm">
       <!--<svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false">
      -  <--<title>Placeholder</title>
        <rect width="100%" height="100%" fill="#55595c"/>
        <text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text>
      </svg>-->
       <img class="bd-placeholder-img card-img-top"  width="100%" height="400" :src="coffeeData.image" alt="Image-coffee">
      <div class="card-body">
        <p class="card-text">{{coffeeData.name}}</p>
        <ul>
          <!-- propriedades do café -->
          <li v-for="char in coffeeData.characteristics" :key="char">
            {{char}}
          </li>
        </ul>
        <div class="d-flex justify-content-between align-items-center">
          <div class="btn-group">
            <b-button type="button" 
            class="btn btn-sm btn-outline-secondary"
            variant="link"
            :href="coffeeData.link"
            >Comprar</b-button>
          </div>
          <small class="text-muted">{{coffeeData.weight}}</small>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
   props: {
    coffeeData: {
      required: true,
      type: Object
    }
  }
}
</script>