<script>
 export default{
  data(){
    const a=4;const b=10;
    const br = document.createElement('br');
    return{
    
    text : a * b,
    arr:['A','B','C','D','E'], //\
    examQue:[{q:'How many villages',ans:{A:'1',B:'10',C:'4',D:'50'}}]//\
    //text : 'message'
  }
 }
}
</script>
<template>
  <h3>Hello World, am trying to build e-commerce site using vue and python</h3>
  <p> Seems vues requires internet always.  Oh my God that means a lot of data to be used.
      Thought i could do the stuff offline.
      ok this is great. Seems working ofline. I need write some functions now
  </p>
  <p>{{ text }}</p>
  <Ol>
    <li v-for = "a in arr">{{a}}</li>
  </Ol>
  <ul>
    <li v-for="el in examQue ">{{"Question"+parseInt(examQue.findIndex(z => z == el)+1)+ el.q+":"+Object.keys(el.ans)+el.ans.A+"<::>"+el.ans.B}}</li>
  </ul>
  
</template>
<style></style>
