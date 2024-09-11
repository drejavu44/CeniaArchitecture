<script setup>
import { RouterLink, useRoute } from 'vue-router';

const route = useRoute();
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="../assets/cenia logo wht.png" width="100" height="40" alt="Logo" />
      </a>
      <div class="navbar-menu">
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/' }" to="/">Home</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/about' }" to="/about">About</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/projects' }" to="/projects">Projects</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/pricing' }" to="/pricing">Pricing</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/contact' }" to="/contact">Contact</RouterLink>
        </li>
      </div>
      <div class="navbar-right">
        <li class="nav-item">
          <RouterLink class="nav-link" :class="{ 'nav-link-active': route.path === '/login' || route.path === '/signup' }" to="/login">
            <i class="fa-solid fa-user"></i> Login / Register
          </RouterLink>
        </li>
      </div>
    </div>
  </nav>
</template>

<style scoped>
/* Overall Navbar styling */
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between; /* Ensures that the brand, menu, and right items are spaced apart */
  background-color: #1e1e1e; /* Dark background similar to bg-dark */
  padding: 0 10%; /* Adjusts padding to your layout needs */
  font-family: 'Jost', sans-serif;
  height: 60px; /* Adjust height if necessary */
}

/* Branding section styling */
.navbar-brand {
  display: flex;
  align-items: center;
}

/* Flex container for menu and right-aligned items */
.container {
  display: flex;
  justify-content: space-between; /* Spreads out the brand, menu, and right items */
  width: 100%;
}

/* Navigation menu styling */
.navbar-menu {
  display: flex;
  align-items: center;
  flex-grow: 1; /* Takes up available space */
  justify-content: center; /* Centers the nav links horizontally */
}

/* Navigation item styling */
.nav-item {
  margin: 0 15px; /* Adds horizontal spacing between the nav items */
  list-style: none;
}

/* Link styling */
.nav-link {
  text-decoration: none;
  color: white; /* Default color for links */
  font-size: 16px; /* Adjust font size if necessary */
  display: flex;
  align-items: center; /* Aligns text and icon vertically */
}

/* Hover effect for links */
.nav-link:hover {
  color: #adb5bd; /* Light grey for hover effect */
}

/* Active link styling */
.nav-link-active {
  color: #adb5bd !important; /* Highlight color for active link with higher specificity */
}

/* Right-aligned navigation items */
.navbar-right {
  display: flex;
  align-items: center;
}

i {
  margin-right: 10px;
}
</style>
