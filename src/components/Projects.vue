<<template>
  <div class="main">
        <div class="bg-white bg-white column  main shadow-2 text-primary">
            <h3>Current project's list</h3>
            <p>This projects are open source and are used by users.</p>  
        </div>
        <div class="row wrap">
             <div class="col-xs-12 col-md-6" v-for="p in projects">
                 <card-project :project="p"></card-project>
            </div>   
        </div>
  </div>
</template>
<script>
import CardProject from './projects/CardProject.vue'
import projects from '../projects.json';

export default {
    name: 'Projects',
    data() {
        return {projects};
    },
    components: {CardProject}
}
</script>
<style scoped>
    .main {
        padding:10px;
    }
</style>
