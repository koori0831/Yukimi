<script setup lang="ts">
import { Button } from './components/ui/button'
</script>

<template>
  <main class="min-h-screen bg-zinc-950 text-zinc-50">
    <div class="mx-auto max-w-3xl px-6 py-10 space-y-6">
      <h1 class="text-3xl font-bold tracking-tight">
        Tailwind / TSX Button 테스트
      </h1>

      <div class="flex flex-wrap gap-3 items-center">
        <Button>Shadcn TSX Button</Button>

        <button
          class="rounded-lg bg-indigo-500 px-4 py-2 text-sm font-semibold hover:bg-indigo-400 active:bg-indigo-600"
          type="button"
        >
          Tailwind 버튼
        </button>

        <span class="rounded-md bg-emerald-500/15 px-3 py-1 text-sm text-emerald-300 ring-1 ring-emerald-500/30">
          배경/폰트/테두리 보이면 OK
        </span>
      </div>

      <div class="grid gap-4 sm:grid-cols-3">
        <div class="rounded-xl border border-zinc-800 bg-zinc-900/40 p-4">
          <div class="text-sm text-zinc-400">Typography</div>
          <div class="mt-2 text-xl font-bold">굵게/크기 변화</div>
        </div>
        <div class="rounded-xl border border-zinc-800 bg-zinc-900/40 p-4">
          <div class="text-sm text-zinc-400">Spacing</div>
          <div class="mt-2 flex gap-2">
            <div class="h-6 w-6 rounded bg-zinc-700" />
            <div class="h-6 w-6 rounded bg-zinc-600" />
            <div class="h-6 w-6 rounded bg-zinc-500" />
          </div>
        </div>
        <div class="rounded-xl border border-zinc-800 bg-zinc-900/40 p-4">
          <div class="text-sm text-zinc-400">Border / Radius</div>
          <div class="mt-2 rounded-2xl border border-zinc-700 bg-zinc-950 p-3 text-sm">
            둥근 모서리 + 테두리
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
