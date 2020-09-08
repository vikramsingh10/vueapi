<template>
    <div>
       
        <form @submit="ucase">
        <input type="text" v-model="title" name="title" placeholder="enter text to be converted in UPPERCASE">
          
        <input type="submit" value="Submit" class="btn" />
        
        </form>
        <h3> {{ustring}} </h3>  
    </div>
</template>

<script>
export default {
    name: "upper",
    data() {
        return {
            title: '',
            ustring: ''
        }
    },
    methods: {
        ucase: function (e) {
            e.preventDefault();
            this.ustring = this.title.toUpperCase();
            this.title = '';        }
    }
}
</script>

<style scoped>
    form {
        display: flex;
    }

    input[type="text"] {
        flex: 10;
        padding: 5px;
    }

    input[type="submit"] {
        flex: 2;
    }

</style>