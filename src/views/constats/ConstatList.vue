<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12">
        <h4>La liste de tous les constats</h4>
      </div>
    </div>
    <div class="row filter">
      <div class="col-12 col-md-2">
        <label for="country" class="form-label">Année</label>
        <select
          class="form-select"
          id="country"
          placeholder="Quelle année?"
          required>
          <option>2023</option>
          <option>2022</option>
          <option>2021</option>
          <option>2020</option>
        </select>
        <div class="invalid-feedback">Veuillez choisir l'année</div>
      </div>

      <div class="col-12 col-md-2">
        <label for="state" class="form-label">Mois</label>
        <select class="form-select" id="state" required>
          <option>Janvier</option>
          <option>Fevrier</option>
          <option>Mars</option>
          <option>Avril</option>
          <option>Mai</option>
          <option>Juin</option>
          <option>Juillet</option>
          <option>Aout</option>
          <option>Septembre</option>
          <option>Octobre</option>
          <option>Novembre</option>
          <option>Decembre</option>
        </select>
        <div class="invalid-feedback">Please provide a valid state.</div>
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <table
          class="table table-sm table-light border-top-color table-striped">
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
  </div>
</template>

<script setup lang="ts">
import { useRouter } from "vue-router";
const router = useRouter();

const goToDetails = () => {
  router.push("/constat-details/55146436");
};
</script>

<style scoped lang="scss">
.table {
  width: 60%;
  margin: auto;
}

.filter {
  justify-content: center;
}
</style>
