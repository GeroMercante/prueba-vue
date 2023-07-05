<template>
  <div class="container mt-2">
    <div class="row">
      <div class="col-md-5">
        <div class="card shadow-lg">
          <div class="card-body">
            <p class="h3">
              Hola <span class="fw-bold">{{ this.msg }}</span>
            </p>
            <button class="btn btn-success m-1" @click="greet('Buenos días!')">
              Buen día
            </button>
            <button
              class="btn btn-warning m-1"
              @click="greet('Buenas tardes!')"
            >
              Buenas tardes
            </button>
            <button class="btn btn-danger m-1" @click="greet('Buenas noches!')">
              Buenas noches
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Greeting",
  data: function () {
    return {
      msg: "",
    };
  },
  methods: {
    greet: function (value) {
      this.msg = value;
    },
  },
};
</script>

<style></style>
