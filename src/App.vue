<script setup>
// import FooterComponent from "./components/FooterComponent.vue";

import Header from "./components/Header.vue";
import FooterComponent from "./components/FooterComponent.vue";
import User from "./components/User.vue";
import Modal from "./components/Modal.vue";
import Bai1 from "./components/Bai1";
import Bai2 from "./components/Bai2";
import Bai3 from "./components/Bai3";
import Bai4 from "./components/Bai4";
import Bai5 from "./components/Bai5";
import Bai6 from "./components/Bai6";
import AdminIndex from "../components/bai7/AdminIndex";
import UserLayout from "../components/bai8/UserLayout";
</script>

<template>
  <div>
    <h1>Hello world</h1>

    <Header></Header>

    <!-- <Header /> -->

    <User />

    <footer-component></footer-component>

    <!-- Modal -->
    <Modal />
    <Bai1/>
    <Bai2/>
    <Bai3/>
    <Bai4/>
    <Bai5/>
    <Bai6/>
    <AdminIndex/>
    <UserLayout/>
  </div>
</template>