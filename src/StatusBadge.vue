<script setup>
defineProps({status:String});
const labels={queued:'排队中',running:'处理中',succeeded:'已完成',failed:'失败',cancelled:'已取消'};
</script><template><span class="status" :class="status"><span class="status-dot" aria-hidden="true"></span>{{labels[status]||status}}</span></template>
