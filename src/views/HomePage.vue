<template>
    <div>
        <div class="container-fluid">
            <div class="row">
                <div class="col-12">
                    <h4>Les derniers accidents</h4>
                    <table class="table table-sm table-light border-top-color table-striped ">
                        <thead class="thead-light">
                            <tr>
                                <th>Date et heure</th>
                                <th>Lieu</th>
                                <th>Type</th>
                                <th>Gravité</th>
                            </tr>
                        </thead>
                        <tbody class="">
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Materiel</td>
                                <td>Sans</td>
                            </tr>

                        </tbody>
                      
                    </table>
                </div>
                
            </div>
            <div class="row">
                <div class="col-12">
                    <h4>Les dernieres contraventions</h4>
                    <table class="table table-sm table-light border-top-color table-striped ">
                        <thead class="thead-light">
                            <tr>
                                <th>Date et heure</th>
                                <th>Lieu</th>
                                <th>Type</th>
                                <th>Vehicule</th>
                            </tr>
                        </thead>
                        <tbody class="">
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Feu rouge</td>
                                <td>524D100</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Feu rouge</td>
                                <td>524D100</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Feu rouge</td>
                                <td>524D100</td>
                            </tr>
                            <tr @click="goToDetails">
                                <td>Jeudi 9 Avril 2020</td>
                                <td>Ambouli</td>
                                <td>Feu rouge</td>
                                <td>524D100</td>
                            </tr>
                     
                   
                        </tbody>
                      
                    </table>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import {  useRouter } from 'vue-router';
const router = useRouter()

const goToDetails = ()=>{
    router.push('/constat-details/55146436');
}
</script>

<style scopped lang="scss">
.row{padding-top: 20px;
margin-bottom: 50px;}

h4{
    margin-bottom: 30px;
    
}
.table{
    width: 60%;
    margin: auto;
}
tbody>tr{
    cursor: pointer;
    &:hover{
     td{
        &:last-child{
            &::after{
                content: '',
                
            }
        }
     }
        
      
    }
}
</style>