<template>
 <div class="container">
   <app-new-quote @quoteAdded="newQuote"></app-new-quote>
   <app-quote-grid :quotes="quotes"></app-quote-grid>
   </div> 
</template>
<script>
import QuoteGride from './components/QuoteGride.vue';
import NewQuote from './components/NewQuote.vue';
export default {
 data: function(){
   return {
     quotes: [
             'A just A quote to see something'
     ],
     maxQuote: 10
   }
 },
 methods: {
   newQuote: function(quote){
     this.quotes.push(quote);
   }
 },
 components: {
   appQuoteGrid: QuoteGride,
   appNewQuote: NewQuote 
 } 
}
</script>
<style scoped>

</style>