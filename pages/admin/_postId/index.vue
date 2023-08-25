<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '../../../components/Admin/AdminPostForm.vue';

export default {
    layout: 'admin',
    components: {
    AdminPostForm
},
    data() {
        return {
            loadedPost: {
                author: 'Alessia',
                title: 'My awesome Post',
                content: 'Super amazing, thanks for that!',
                thumbnailLink: 'https://media.istockphoto.com/id/1305012465/it/vettoriale/connessione-internet-senso-astratto-della-scienza-e-della-tecnologia-illustrazione.jpg?s=612x612&w=0&k=20&c=r9U1QleziK9ptof9-cWY--AKQ9lt4MV055D9NBA3AF8='
               }
        }
    }

}
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>