<script>
    import { Navbar, NavBrand, NavLi, NavUl, Button, Input, Modal, Label, Checkbox } from 'flowbite-svelte'
    import { page } from '$app/stores'

    let formModal = true
</script>

    <div class="flex md:order-2">
      <Modal bind:open={formModal} size="xs" autoclose={false} class="w-full">
        <form class="flex flex-col space-y-6" action="#">
          <h3 class="text-xl font-medium text-gray-900 dark:text-white p-0">Password Assistace</h3>
          <Label class="space-y-2">
            <span>Email</span>
            <Input type="email" name="email" placeholder="name@company.com" required />
          </Label>
          <Button type="submit" class="w-full1">Continue</Button>
        </form>
      </Modal>
    </div>
