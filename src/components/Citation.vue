<template>
<div>
    <citation-albert/>
    <citation-confucius/>
    <citation-hamlet/>
    <citation-jean-paul/>
    <citation-raymond/>
</div>
    
</template>

<script>
import CitationHamlet from './citation/CitationHamlet.vue'
import CitationConfucius from './citation/CitationConfucius.vue'
import CitationJeanPaul from './citation/CitationJeanPaul.vue'
import CitationAlbert from './citation/CitationAlbert.vue'
import CitationRaymond from './citation/CitationRaymond.vue'

export default {
    name : 'Citation',
    data () {
    return {
      componentNames : [
        'CitationHamlet',
        'CitationConfucius',
        'CitationJeanPaul',
        'CitationAlbert',
        'CitationRaymond'
      ]
    }
  },
  components: {
    CitationHamlet,
    CitationConfucius,
    CitationJeanPaul,
    CitationAlbert,
    CitationRaymond
  }
}
</script>

<style>

</style>
