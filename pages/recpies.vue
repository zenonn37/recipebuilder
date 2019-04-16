<template>
<el-container>
    <el-main >
    <el-row :gutter="10" >
  <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6"
  v-for="f in food" :key='f.id'>
      
      
      
      
      <el-card  shadow="hover" :body-style="{ padding: '0' }">
          <div class="image-control">
      <img  src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png" class="image">
      </div>
      <div style="padding: 14px;">
        <div class="meal-title">{{f.title}}</div>
        <div class="macro-container">
            <div class="macro">
                <h6>Protein</h6>
                <span>{{f.protein}}g</span>
            </div>
             <div class="macro">
                <h6>Fat</h6>
                <span>{{f.fat}}g</span>
            </div>
             <div class="macro">
                <h6>Net Carbs</h6>
                <span>{{f.carbs}}g</span>
            </div>

            
        </div>
<el-collapse v-model="activeName" accordion class="control-accord">
  <el-collapse-item title="Ingredients" :name="f.id">
    <div>Consistent with real life: in line with the process and logic of real life, and comply with languages and habits that the users are used to;</div>
    <div>Consistent within interface: all elements should be consistent, such as: design style, icons and texts, position of elements, etc.</div>
  </el-collapse-item>
            </el-collapse>
       
         <div>

         </div>
      
      </div>
    </el-card>
      
      
      
      
      </el-col>
  <!-- <el-col :xs="4" :sm="6" :md="8" :lg="9" :xl="11"><div class="grid-content bg-purple-light"></div></el-col>
  <el-col :xs="4" :sm="6" :md="8" :lg="9" :xl="11"><div class="grid-content bg-purple"></div></el-col>
  <el-col :xs="8" :sm="6" :md="4" :lg="3" :xl="1"><div class="grid-content bg-purple-light"></div></el-col> -->
</el-row>
    
    </el-main>
    </el-container>
    
</template>

<script>
export default {
  data() {
    return {
      activeName: '1',
      food: [
        {
          id: 1,
          title: 'Chicken Sandwich',
          carbs: 45,
          protein: 12,
          fat: 11
        },
        {
          id: 2,
          title: 'Hamburger',
          carbs: 0,
          protein: 30,
          fat: 20
        },
        {
          id: 3,
          title: 'Pizza',
          carbs: 50,
          protein: 6,
          fat: 12
        },
        {
          id: 4,
          title: 'Cookies',
          carbs: 19,
          protein: 2,
          fat: 15
        }
      ]
    }
  }
}
</script>

<style scoped>
.control-accord {
  margin-top: 20px;
}
.image-control {
  display: flex;
  justify-content: center;
}
.el-card {
  width: 315px;
}
.meal-title {
  color: #262a2e;
  margin-bottom: 10px;
  font-size: 25px;
}
.macro-container {
  display: flex;
  justify-content: space-between;
}
.macro {
  flex-basis: 30%;
  text-align: center;
  border-radius: 5px;
  background: #cbd4e0;
  padding: 10px;
}

.image {
  width: 315px;
  height: 215px;
  /* border-radius: 50%;
  border: 2px solid gray; */
}
.containers {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
</style>
