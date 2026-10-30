<template>
    <h2 class="mb-4">ยินดีต้อนรับ {{ state.user.full_name }}</h2>
    <v-card class="pa-4" max-width="600">
        <p>บทบาท: <strong>{{ roleNames[state.user.role] }}</strong></p>
        <p>หน้านี้เป็นหน้าชั่นคราวของเล่มซ้อม Login เมนูจริงของแต่ละบทบาทจะทำให้คู่มือหลักขั้น 6-7 </p>
    </v-card>
</template>

<script setup>
import { state, roleName } from  '../api';

const roleNames = roleName;
</script>
