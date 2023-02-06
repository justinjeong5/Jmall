<script setup>
import Drawer from "@components/navigation/drawer.vue";
</script>

<template>
    <v-app>
        <v-navigation-drawer app>
            <Drawer />
        </v-navigation-drawer>

        <v-app-bar app>
            <div>app bar</div>
        </v-app-bar>

        <!-- Sizes your content based upon application components -->
        <v-main>

            <!-- Provides the application the proper gutter -->
            <v-container fluid>
                <div>
                    container
                </div>
                <!-- If using vue-router -->
                <router-view></router-view>
            </v-container>
        </v-main>

        <v-footer app>
            <!-- -->
            <div>footer</div>
        </v-footer>
    </v-app>
</template>

<style lang="scss" scoped>
@import "@styles/style.scss";
</style>
