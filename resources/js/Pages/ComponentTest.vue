<script setup>
import GuestLayout from '@/Layouts/GuestLayout.vue'
import Lavel from '@/Components/InputLabel.vue'
import Input from '@/Components/TextInput.vue'

const emitTest = e => console.log(e)
</script>

<template>
<GuestLayout>
<Lavel value="件名">タイトル</Lavel>
<Input 
model-value="初期値が入ります"
@update:model-value="emitTest"
></Input>
</GuestLayout>


</template>