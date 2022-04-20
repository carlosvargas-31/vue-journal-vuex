<template>
  <div class="entry-container mb-3 pointer p-2"
       @click="$router.push({ name: 'entry', params: {id:10}})"
  >
      <div class="entry-title d-flex">
          <!-- Título -->
          <span class="text-success fs-5 fw-bold">18</span>
          <span class="mx-1 fs-5">abril</span>
          <span class="mx-2 fw-light">2022, lunes</span>
      </div>

      <div class="entry-description">
          “Sed ut perspiciatis, unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam eaque ipsa, quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt, explicabo. Nemo enim ipsam voluptatem, quia voluptas sit, aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos, qui ratione voluptatem sequi nesciunt, neque porro quisquam est, qui dolorem ipsum, quia dolor sit amet consectetur adipisci[ng] velit, sed quia non numquam [do] eius modi tempora inci[di]dunt, ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit, qui in ea voluptate velit esse, quam nihil molestiae consequatur, vel illum, qui dolorem eum fugiat, quo voluptas nulla pariatur?”
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s all ease-in;

    &:hover {
        background-color: lighten($color: grey, $amount: 45);
    }

    .entry-description {
        font-size: 12px;
    }
}
</style>