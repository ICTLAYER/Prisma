<script setup>
import { PrismaClient } from '@prisma/client'

const prisma = new PrismaClient({})

const invoices = await prisma.invoice.findMany({
  orderBy: {
    invoice_id: 'desc',
  },
})
</script>

<template>
  <div v-for="inv in invoices" :key="inv.invoice_id">
    <p>{{ inv.invoice_id }} || {{ inv.invoice_date }}</p>
  </div>
</template>
