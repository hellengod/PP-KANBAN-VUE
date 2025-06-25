<template>
    <div class="col-md-3">
        <div class="p-2 alert" :class="alertClass">
            <h3>{{ titulo }}</h3>
            <draggable class="list-group kanban-column" :list="tasks" group="tasks" item-key="name">
                <template #item="{ element }">
                    <div class="list-group-item">
                        {{ element.name }}
                    </div>
                </template>
            </draggable>
        </div>
    </div>
</template>

<script lang="js">
import draggable from "vuedraggable";

export default {
    name: 'KanbanColumn',
    components: { draggable },
    props: {
        titulo: { type: String, required: true },
        tasks: { type: Array, required: true },
        alertClass: { type: String, default: 'alert-secondary' },
    }

}
</script>

<style scoped>
.kanban-column {
    min-height: 200px;
}
</style>