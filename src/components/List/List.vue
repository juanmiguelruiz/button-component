<template>
  <div id="list">
    <h1>Buttons</h1>
    <div>
      <div class="row">
        <div class="button-container">
          <Label text='Button text="Click here"' />
          <Button text="Click here" />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text='Button variant="outline"' />
          <Button variant="outline" />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text='Button variant="text"' />
          <Button variant="text" />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text="Button disableShadow" />
          <Button disableShadow />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text="Button disabled" />
          <Button disabled />
        </div>

        <div class="button-container">
          <Label text='Button variant="text" disabled' />
          <Button variant="text" disabled />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text='Button startIcon="local_grocery_store"' />
          <Button startIcon="local_grocery_store" />
        </div>

        <div class="button-container">
          <Label text='Button endIcon="local_grocery_store"' />
          <Button endIcon="local_grocery_store" />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text='Button size="sm"' />
          <Button size="sm" />
        </div>

        <div class="button-container">
          <Label text='Button size="md"' />
          <Button size="md" />
        </div>

        <div class="button-container">
          <Label text='Button size="lg"' />
          <Button size="lg" />
        </div>
      </div>

      <div class="row">
        <div class="button-container">
          <Label text='Button color="default' />
          <Button color="default" />
        </div>

        <div class="button-container">
          <Label text='Button color="primary' />
          <Button color="primary" />
        </div>

        <div class="button-container">
          <Label text='Button color="secondary' />
          <Button color="secondary" />
        </div>

        <div class="button-container">
          <Label text='Button color="danger' />
          <Button color="danger" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Label from "./Label";
import Button from "../Button";

export default {
  name: "List",
  components: {
    Label,
    Button,
  },
};
</script>

<style src="./styles.css"></style>
