<template>
  <div class="d-flex align-items-center">
    <b-form-input
      v-model="value"
      :required="required"
      pattern="#[0-9A-Fa-f]{6}"
      @input="$emit('input', value)"
    />
    <color-picker v-model="value" />
  </div>
</template>

<script>
import ColorPicker from "@reciprocity/color-picker";
import { BFormInput } from "bootstrap-vue";

export default {
  name: "ColorInput",
  components: {
    ColorPicker,
    BFormInput
  },
  props: {
    value: {
      type: String,
      required: true
    },
    required: {
      type: Boolean,
      default: false
    }
  }
};
</script>

<style lang="scss" scoped>
.form-control {
  max-width: 175px;
  margin-right: 15px;
}
</style>
