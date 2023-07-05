<template>
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card shadow-lg">
          <div class="card-body">
            <p class="h3 display-3">Event Handling</p>
            <p class="h3 display-3">{{ this.count }}</p>
            <button @click="incr" class="btn btn-success m-1">
              Incrementar
            </button>
            <button @click="decr" class="btn btn-warning m-1">Disminuir</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contador",
  data: function () {
    return {
      count: 0,
    };
  },
  methods: {
    incr: function () {
      this.count = this.count + 1;
    },
    decr: function () {
      this.count = this.count - 1;
    },
  },
};
</script>

<style></style>
