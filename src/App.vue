<template>
 <div class="container">
   <app-quote-grid :quotes="quotes"></app-quote-grid>
   </div> 
</template>
<script>
import QuoteGride from './components/QuoteGride';
export default {
 data: function(){
   return {
     quotes: [
             'A just A quote to see something'
     ],
     maxQuote: 10
   }
 },
 components: {
   appQuoteGrid: QuoteGride
 } 
}
</script>
<style scoped>

</style>