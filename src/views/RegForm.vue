<template>
	<ion-page>
		<ion-header>
			<ion-toolbar>
				<ion-buttons slot="start">
					<ion-button href="/tabs/ponds">
						<img src="/assets/icon/Home.svg" alt="">
					</ion-button>
				</ion-buttons>
				<ion-title>Registration Form</ion-title>
			</ion-toolbar>
		</ion-header>

		<ion-content :fullscreen="true">
			<ion-header collapse="condense">
				<ion-toolbar>
					<ion-title size="large">Registration Form</ion-title>
				</ion-toolbar>
			</ion-header>
			<ion-list>
				<ion-item>
					<ion-label position="stacked">Nama Kolam</ion-label>
					<ion-input placeholder="Kolam 1" v-model="namakolam"></ion-input>
				</ion-item>
			</ion-list>
			<ion-list>
				<ion-item>
					<ion-label position="stacked">Lokasi Kolam</ion-label>
					<ion-input placeholder="Blok A" v-model="lokasikolam"></ion-input>
				</ion-item>
			</ion-list>
			<ion-list>
				<ion-item>
					<ion-label position="stacked">Material Kolam</ion-label>
					<ion-select interface="action-sheet" v-model="materialkolam">
						<ion-select-option value="tanah">Tanah</ion-select-option>
						<ion-select-option value="beton">Beton</ion-select-option>
						<ion-select-option value="terpal">Terpal</ion-select-option>
					</ion-select>
				</ion-item>
			</ion-list>
			<ion-list>
				<ion-item>
					<ion-label position="stacked">Bentuk Kolam</ion-label>
					<ion-select interface="action-sheet" v-model="bentukkolam">
						<ion-select-option value="kotak">Kotak</ion-select-option>
						<ion-select-option value="bundar">Bundar</ion-select-option>
					</ion-select>
				</ion-item>
			</ion-list>

			<ion-button expand="block" @click="getFormValues()">Registrasi</ion-button>
		</ion-content>
	</ion-page>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonButton, IonButtons, IonLabel, IonInput, IonItem, IonList, IonSelect, IonSelectOption } from '@ionic/vue';
export default defineComponent({
	name: 'Tab1Page',
	components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonButton, IonButtons, IonLabel, IonInput, IonItem, IonList, IonSelect, IonSelectOption },
	data() {
		return {
			namakolam: '',
			lokasikolam: '',
			materialkolam: '',
			bentukkolam: '',
		}
	},
	methods: {
		getFormValues() {
			console.log(this.namakolam)
			console.log(this.lokasikolam)
			console.log(this.materialkolam)
			console.log(this.bentukkolam)

			var pond = { 'nama-kolam': this.namakolam, 'lokasi-kolam': this.lokasikolam, 'material-kolam': this.materialkolam, 'bentuk-kolam': this.bentukkolam }
			console.log(pond)
		}
	}
});
</script>

<style scoped>
ion-button {
	--background: #6C5ECF;
}
</style>