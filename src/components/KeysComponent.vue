<template>

    <div>
        <!-- Header -->
        <div class="pt-3 grey--text text--lighten-1 d-flex justify-center">
            <h3>Keys</h3>
        </div>
    
    <!-- Row -->
    <div class="d-flex justify-space-between px-5 mt-4 align-center grey--text text--lighten-1">
        <div class="d-flex align-center text-body-2">
            <div icon class="mr-2">
                <v-icon class="grey--text text--lighten-1">mdi-check</v-icon>
            </div>
            <div >accepted</div>
        </div>
        <div >
            1/1
        </div>
    </div>
    <v-divider class="mt-2 bg-grey"></v-divider>
        
    <div class="d-flex justify-space-between px-5 mt-3 align-center grey--text text--lighten-1">
        <div class="d-flex align-center text-body-2">
            <div icon class="mr-2">
                <v-icon class="grey--text text--lighten-1">mdi-arrow-expand-left</v-icon>
            </div>
            <div >rejected</div>
        </div>
        <div>
            0/1
        </div>
    </div>
    
    
    <v-divider class="mt-2 bg-grey" ></v-divider>
       
    <div class="d-flex justify-space-between px-5 mt-3 align-center grey--text text--lighten-1">
        <div class="d-flex align-center text-body-2">
            <div icon class="mr-2">
                <v-icon class="grey--text text--lighten-1">mdi-reload</v-icon>
            </div>
            <div >pending</div>
        </div>
        <div>
            0/1
        </div>
    </div>
    <v-divider class="mt-2 bg-grey"></v-divider>
        
    <div class="d-flex justify-space-between px-5 mt-3 align-center grey--text text--lighten-1">
        <div class="d-flex align-center text-body-2">
            <div icon class="mr-2">
                <v-icon class="grey--text text--lighten-1">mdi-cancel</v-icon>
            </div>
            <div >denied</div>
        </div>
        <div>
            0/1
        </div>
    </div>
        
        
        </div>
</template>