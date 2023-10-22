<template>
    <!-- Modal Logs-->
    
    <div class="modal fade" :id="`modalLogs`" tabindex="-1" aria-labelledby="labelLogs" aria-hidden="true">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title" id="labelLogs">Resultados de procesar la cola de {{dataLogs.tituloCola}}.</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
            </div>
            <div class="modal-body">
                <textarea class="form-control sc" v-html="dataLogs.logs" readonly rows="5"></textarea>
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
            </div>
        </div>
    </div>
</div>
</template>

<script>
    export default {
        props:['dataLogs']
    }
</script>