<template>
<div>
    <div class="container-1">
        <div class="box-1">
            <h3>Box1</h3>
            <p>Some content</p>
        </div>
          <div class="box-2">
            <h3>Box2</h3>
            <p>Some content</p>
        </div>
          <div class="box-3">
            <h3>Box3</h3>
            <p>Some content Lorem ipsum dolor sit amet consectetur adipisicing elit.
                 Necessitatibus nesciunt suscipit minima laboriosam maxime pariatur facilis maiores sit. 
                 Reprehenderit enim deleniti temporibus voluptates animi rem eveniet! Est quia obcaecati 
                 libero!</p>
        </div>
      

 
    </div>



      <div class="container-2">
        <div class="container-2-box">
            <h3>Box1</h3>
            <p>Some content</p>
        </div>
          <div class="container-2-box">
            <h3>Box2</h3>
            <p>Some content</p>
        </div>
          <div class="container-2-box">
            <h3>Box3</h3>
            <p>Some content Lorem ipsum dolor sit amet consectetur adipisicing elit.
                 Necessitatibus nesciunt suscipit minima laboriosam maxime pariatur facilis maiores sit. 
                 Reprehenderit enim deleniti temporibus voluptates animi rem eveniet! Est quia obcaecati 
                 libero!</p>
        </div>
      

 
     </div>



       <div class="container-3">
        <div class="container-3-box">
            <h3>Box1</h3>
            <p>Some content</p>
        </div>
          <div class="container-3-box">
            <h3>Box2</h3>
            <p>Some content</p>
        </div>
          <div class="container-3-box">
            <h3>Box3</h3>
            <p>Some content Lorem ipsum dolor sit amet consectetur adipisicing elit.
                 Necessitatibus nesciunt suscipit minima laboriosam maxime pariatur facilis maiores sit. 
                 Reprehenderit enim deleniti temporibus voluptates animi rem eveniet! Est quia obcaecati 
                 libero!</p>
        </div>
      

 
     </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
@media (min-width: 768px) {
  .container-2 {
    display: flex;
    justify-content: space-between;
  }

  .container-1 {
    display: flex;
    /* align-items: flex-start;
  align-items: flex-end;
  align-items: center;
  flex-direction: column;
   */
  }
}

.container-3 {
  display: flex;
  flex-wrap: wrap;
}

.container-2-box {
  flex-basis: 30%;
}
.container-3-box {
  flex-basis: 30%;
}

.container-1 div,
.container-3 div {
  border: 1px #ccc solid;
  padding: 10px;
  margin: 60px 20px 0 20px;
}
.container-2 div {
  border: 1px #ccc solid;
  padding: 10px;
}

.box-1 {
  flex: 1;
}
.box-2 {
  flex: 1;
}
.box-3 {
  flex: 2;
}
</style>

