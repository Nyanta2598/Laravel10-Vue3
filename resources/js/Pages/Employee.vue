<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import LedgerTable from '@/Components/LedgerTable.vue';
import TransactionListFirstSemester from '@/Components/TransactionListFirstSemester.vue';
import TransactionListSecondSemester from '@/Components/TransactionListSecondSemester.vue';
import TransactionListThirdSemester from '@/Components/TransactionListThirdSemester.vue';
import TransactionListFourthSemester from '@/Components/TransactionListFourthSemester.vue';
</script>

<template>
    <Head title="Student Ledger" />
    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Student Ledger
            </h2>
        </template>
        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-4 space-y-6">
                <div class=" sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg">
                        <LedgerTable />
                    </div>
                <div class="grid mb-8 rounded-lg  md:mb-12 md:grid-cols-1 gap-6">
                    <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg text-center">
                        <h1 class="text-lg font-medium text-gray-900 dark:text-gray-100">2020</h1>
                        <p class="mt-1 text-sm text-gray-600 dark:text-gray-400 mb-4">
                            Transaction list on First Semester
                        </p>
                        <TransactionListFirstSemester />
                    </div>
                    <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg text-center">
                        <h1 class="text-lg font-medium text-gray-900 dark:text-gray-100">2020</h1>
                        <p class="mt-1 text-sm text-gray-600 dark:text-gray-400 mb-4">
                            Transaction list on Second Semester
                        </p>
                        <TransactionListSecondSemester />
                    </div>
                    
                    <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg text-center">
                        <h1 class="text-lg font-medium text-gray-900 dark:text-gray-100">2020</h1>
                        <p class="mt-1 text-sm text-gray-600 dark:text-gray-400 mb-4">
                            Transaction list on Third Semester
                        </p>
                        <TransactionListThirdSemester />
                    </div>
                    <div class="p-4 sm:p-8 bg-white dark:bg-gray-800 shadow sm:rounded-lg text-center">
                        <h1 class="text-lg font-medium text-gray-900 dark:text-gray-100">2020</h1>
                        <p class="mt-1 text-sm text-gray-600 dark:text-gray-400 mb-4">
                            Transaction list on Fourth Semester
                        </p>
                        <TransactionListFourthSemester />
                    </div>
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


