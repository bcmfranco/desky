<template>
  <v-dialog width="500">
    <template v-slot:activator="{ props }">
      <v-btn v-bind="props" text="Open Dialog"> </v-btn>
    </template>

    <template v-slot:default="{ isActive }">
      <v-card title="Dialog">
        <v-card-text>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </v-card-text>

        <v-card-actions>
          <v-spacer></v-spacer>

          <v-btn
            text="Close Dialog"
            @click="isActive.value = false"
          ></v-btn>
        </v-card-actions>
      </v-card>
    </template>
  </v-dialog>
</template>
  
  <script>

  // Hay que laburar en el modalBox

  export default {
    data() {
      return {
        linkText: '',
        linkURL: '',
      };
    },
    methods: {
      closeModal() {
        this.$emit('closeModal');
      },
      saveLink() {
        // Puedes agregar lógica aquí para guardar el enlace
        // Puedes emitir un evento para informar a tu componente principal sobre la acción realizada
        this.$emit('linkSaved', { text: this.linkText, url: this.linkURL });
        this.closeModal();
      },
    },
  };
  </script>
  
  <style scoped>
  /* Estilos para el modal */
  .modal-container {
    display: flex;
    align-items: center;
    justify-content: center;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
  }
  
  .modal-content {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    text-align: center;
  }
  
  .close {
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 20px;
    cursor: pointer;
  }
  </style>
  