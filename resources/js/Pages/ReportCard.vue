<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import ReportCardTable from '@/Components/ReportCardTable.vue';
</script>
<template>
    <Head title="ReportCard" />
    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Report Card
            </h2>
        </template>
        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-4 space-y-6">
                <div class=" sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg">
                    
                    
                    <ReportCardTable />
                </div> 
            </div>
        </div>  
    </AuthenticatedLayout>
</template>
<script>
export default {
    components: {
        
    },
    data: function () {
        return {
            
        }
    },
    methods: {
        
    },
    created() {
        
    }
}
</script>