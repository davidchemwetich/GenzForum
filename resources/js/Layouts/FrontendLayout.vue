<template>

    <AuthenticatedLayout>
        <div class="py-8 max-w-7xl mx-auto space-y-6 md:space-y-0 md:grid grid-cols-7 gap-6 sm:px-6 lg:px-8">
            <div class="col-span-2 space-y-3">
                <slot name="side" />
            </div>
            <div class="col-span-5">
                <slot />
            </div>
        </div>
    </AuthenticatedLayout>

    <CreateDiscussionForm />


    <CreatePostForm />
    <Footer/>

</template>

<script setup>
    import AuthenticatedLayout from './AuthenticatedLayout.vue'
    import CreateDiscussionForm from '@/Components/Frontend/CreateDiscussionForm.vue'
    import CreatePostForm from '@/Components/Frontend/CreatePostForm.vue'
    import Footer from "@/Components/Frontend/Footer.vue";
</script>
