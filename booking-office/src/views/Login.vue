<template>
    <v-row>
        <v-col class="pr-0 pb-0">
            <v-img width="100%" src="../assets/img/background.png"/>
        </v-col>
        <v-col class="pl-0">
            <v-card class="ma-16" flat>
                <v-card-text class="text-center heading-1">
                    Masuk
                </v-card-text>

                <v-card-text class="pa-0 body-regular-2">
                    Email
                </v-card-text>
                <v-text-field
                 outlined
                 placeholder="Masukan email anda"
                 class="body-regular-3"
                />

                <v-card-text class="pa-0 body-regular-2">
                    Kata Sandi
                </v-card-text>
                <v-text-field
                 :append-icon="show3 ? 'mdi-eye' : 'mdi-eye-off'"
                 :type="show3 ? 'text' : 'password'"
                 name="input-10-2"
                 value=""
                 outlined
                 placeholder="Masukan kata sandi anda"
                 class="body-regular-3"
                 @click:append="show3 = !show3"
                />

                <v-row>
                    <v-col class="text-left py-0">
                        <v-checkbox
                        class="my-0 py-0"
                        color="green"
                        >
                            <template v-slot:label>
                                <div class="body-regular-3">
                                    Simpan Kata Sandi
                                </div>
                            </template>
                        </v-checkbox>
                    </v-col>
                    <v-col class="text-right py-0">
                        <a href="#">Lupa kata sandi ?</a>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col class="text-center">
                        <v-btn
                         color="#606FAA"
                         dark
                         class="px-10"
                        >
                            Masuk
                        </v-btn>
                    </v-col>
                </v-row>

                <v-card-text class="text-center">
                    atau
                </v-card-text>

                <v-card-text class="text-center">
                    Belum punya akun ? <a href="/register">Daftar</a>
                </v-card-text>
                
                
            </v-card>
        </v-col>
    </v-row>
</template>

<script>
export default {
    name: 'LoginPage'
}
</script>

<style scoped>
 .heading-1 {
     font-family: 'Nunito', sans-serif;
     font-weight: 700 !important;
     font-size: 32px !important;
     color: #606FAA !important;
 }
 .body-regular-2 {
     font-family: 'Work Sans', sans-serif;
     font-weight: 400 !important;
     font-size: 14px !important;
     color: #121950 !important;
 }
 .body-regular-3 {
     font-family: 'Work Sans', sans-serif;
     font-weight: 400 !important;
     font-size: 12px !important;
     color: #121950 !important;
 }
 .link-forger-pass {
     color: #455392 !important;
 }
</style>