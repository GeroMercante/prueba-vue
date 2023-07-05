<template>
  <div class="container mt-3">
    <div class="grid">
      <div class="row">
        <div class="col">
          <p class="h3 text-success fw-bold">App Component</p>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Blanditiis
            dolore dolorum rerum voluptatem quam quas molestiae odit officiis
            dolores iste. Vitae quo reprehenderit maxime culpa fugit accusamus
            incidunt suscipit quaerat, iure, optio ducimus delectus illum enim
            porro, amet labore. Necessitatibus!
          </p>
        </div>
      </div>
    </div>
    <Contador />

    <Greeting />
  </div>
</template>

<script>
import Contador from "@/components/Contador";
import Greeting from "@/components/Greeting";

export default {
  name: "Home",
  components: { Contador, Greeting },
};
</script>

<style>
@import "./style.css";
</style>
