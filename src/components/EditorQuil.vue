<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <h1>Editor</h1>
      <div>
        <quill-editor v-model="conteudo" theme="snow"></quill-editor>
      </div>
    </v-responsive>
  </v-container>
</template>

<script lang="ts">
  import {QuillEditor} from '@vueup/vue-quill'
  import '@vueup/vue-quill/dist/vue-quill.snow.css';

  import { defineComponent } from 'vue'

  export default defineComponent({
    name: 'Editor',
    components: {
      QuillEditor,
    },
    data() {
      return {
        count: 1,
        conteudo: '',
      }
    }
  })
</script>
