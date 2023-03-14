<td v-if="editando === persona.id">
    <button class="btn btn-success" @click="guardarPersona(persona)">&#x1F5AB; Guardar</button>
    <button class="btn btn-secondary ml-2" @click="cancelarEdicion(persona)">&#x1F5D9; Cancelar</button>
 </td>
 <td v-else>
    <button class="btn btn-info" @click="editarPersona(persona)">&#x1F58A; Editar</button>
    <button class="btn btn-danger ml-2" @click="$emit('delete-persona', persona.id)">&#x1F5D1; Eliminar</button>
 </td>