<template>
    <v-container fluid>
        <v-form>
            <v-file-input label="Selecione as legendas:" prepend-icon="mdi-message-text" append-icon="mdi-send" outlined
                chips multiple v-model="files" @click:append="processCaptions" />
        </v-form>
        <div class="pills">
            <pill-component v-for="word in groupedWords" :key="word.name" :name="word.name" :amount="word.amount" />
        </div>
    </v-container>
</template>

<script>
import PillComponent from './PillComponent.vue'

export default {
    components: { PillComponent },
    data: function () {
        return {
            files: [],
            groupedWords: [
                { name: 'i', amount: 1204 },
                { name: 'love', amount: 34 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
                { name: 'you', amount: 3043 },
            ]
        }
    },
    methods: {
        processCaptions() {
            console.log(this.files)
        }
    }
}
</script>

<style>
.pills {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
</style>