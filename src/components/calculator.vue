<script setup>
import { ref } from 'vue'

const x = ref(0)
const y = ref(0)
const result = ref(0)
</script>

<template>
    
    <div class="container">
        <div class="row align-items-center justify-content-center" style="height: 100vb;">
            <div class="col-lg-8 align-self-center">
                <div class="card">
                    <h5 class="card-header">Calculator</h5>
                    <div class="card-body">
                        <input id="x" class="form-control number" type="text" v-model="x">
    
                        <button id="add" @click="result = parseInt(x) + parseInt(y)" class="m-3 btn btn-secondary" type="button"> + </button>
                        <button id="sub" @click="result = x-y" class="m-3 btn btn-secondary" type="button"> - </button>
                        <button id="mul" @click="result = x*y" class="m-3 btn btn-secondary" type="button"> x </button>
                        <button id="div" @click="result = x/y" class="m-3 btn btn-secondary" type="button"> / </button>
    
                        <input id="y" class="form-control number" type="text" v-model="y">
                        =
                        <input id="result" class="form-control number" type="text" v-model="result">
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style>
</style>