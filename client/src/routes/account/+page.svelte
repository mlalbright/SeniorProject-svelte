<script>
    import { Navbar, NavBrand, NavLi, NavUl, Button, Input, Modal, Label, Checkbox } from 'flowbite-svelte'
    import { page } from '$app/stores'

    let formModal = true
</script>

    <div class="flex md:order-2">
      <Modal bind:open={formModal} size="xs" autoclose={false} class="w-full">
        <form class="flex flex-col space-y-6" action="#">
          <h3 class="text-xl font-medium text-gray-900 dark:text-white p-0">Create Account</h3>
          <Label class="space-y-2">
            <span>Email</span>
            <Input type="email" name="email" placeholder="name@company.com" required />
          </Label>
          <Label class="space-y-2">
            <span>Password</span>
            <Input type="password" name="password" placeholder="••••••••••" required />
          </Label>
          <Label class="space-y-2">
            <span>Re-enter Password</span>
            <Input type="password" name="password" placeholder="••••••••••" required />
          </Label>
          <Label class="space-y-2">
            <span>Organization Passcode</span>
            <Input type="password" name="Organizationpasscode" placeholder="••••••••••" required />
          </Label>
          <div class="flex items-start">
              <Checkbox>Remember me</Checkbox>
          </div>
          <Button type="submit" class="w-full1">Create your account</Button>
        </form>
      </Modal>
    </div>
