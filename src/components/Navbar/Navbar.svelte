<script>
	import {
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		Avatar,
		Dropdown,
		DropdownItem,
		DropdownHeader,
		DropdownDivider,
		DarkMode
	} from 'flowbite-svelte';
</script>

<Navbar>
	<NavBrand href="/">
		<img src="" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span
		>
	</NavBrand>
	<div class="flex items-center md:order-2">
		<Avatar id="avatar-menu" src="" />
		<NavHamburger class1="w-full md:flex md:w-auto md:order-1" />
	</div>
	<Dropdown placement="bottom" triggeredBy="#avatar-menu">
		<DropdownHeader>
			<span class="block text-sm">Administrator</span>
			<span class="block truncate text-sm font-medium">Z6S9H@example.com</span>
		</DropdownHeader>
		<DropdownItem>Dashboard</DropdownItem>
		<DropdownItem>Settings</DropdownItem>
		<DropdownItem>Earnings</DropdownItem>
		<DropdownDivider />
		<DropdownItem>Sign out</DropdownItem>
	</Dropdown>
	<NavUl>
		<NavLi href="/" active={true}>მთავარი</NavLi>
		<NavLi href="/tours">ტურები</NavLi>
		<NavLi href="/order">შეკვეთა</NavLi>
		<NavLi href="/contact">კავშირი</NavLi>
		<NavLi href="/registraiton">რეგისტრაცია</NavLi>
	</NavUl>
	<DarkMode />
</Navbar>
