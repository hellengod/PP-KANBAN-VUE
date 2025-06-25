<template>
    <div class="row">

        <div class="d-flex align-items-center">
            <b-form-input :value="modelValue" @input="$emit('update:modelValue', $event)" @keyup.enter="$emit('add')"
                placeholder="Adicione uma atividade" style="width: 200px; margin-right: 12px;"></b-form-input>

            <b-button variant="primary" @click="$emit('add')">
                adicionar
            </b-button>

        </div>

    </div>
</template>

<script lang="js">
export default {
    name: 'FormTask',
    props: {
        modelValue: String
    },
    emits: ['update:modelValue', 'add']
}
</script>