<script lang="ts">
  import { Link, page } from '@inertiajs/svelte'
  import { inertia } from '@inertiajs/svelte'
  import { rootPath } from '@/routes'
  import Button from '@/components/ui/button/button.svelte'
  import IconGitBranch from '@lucide/svelte/icons/git-branch'

  import ArrowUpIcon from '@lucide/svelte/icons/arrow-up'

  const links = [{}]
</script>

<svelte:head>
  <link
    rel="preconnect"
    href="https://rsms.me/"
  />
  <link
    rel="stylesheet"
    href="https://rsms.me/inter/inter.css"
  />
</svelte:head>

<div
  class="flex min-h-screen flex-col items-center bg-[#FDFDFC] p-6 text-[#1b1b18] lg:justify-center lg:p-8 dark:bg-[#0a0a0a]"
>
  <header
    class="mb-6 w-full max-w-[335px] text-sm not-has-[nav]:hidden lg:max-w-4xl"
  >
    <h3>It's header</h3>
  </header>
  <a
    href={rootPath()}
    use:inertia
    class="inline-block rounded-sm border border-[#19140035] px-5 py-1.5 text-sm leading-normal text-[#1b1b18] hover:border-[#1915014a] dark:border-[#3E3E3A] dark:text-[#EDEDEC] dark:hover:border-[#62605b]"
  >
    Root
  </a>
  <div class="flex flex-wrap items-center gap-2 md:flex-row">
    <Button variant="outline">Button</Button>
    <Button
      variant="outline"
      size="icon"
      aria-label="Submit"
    >
      <ArrowUpIcon />
    </Button>
    <Button variant="secondary">Secondary</Button>
    <Button
      variant="outline"
      size="sm"
    >
      <IconGitBranch /> New Branch
    </Button>
  </div>

  <h2>It Works</h2>
</div>
