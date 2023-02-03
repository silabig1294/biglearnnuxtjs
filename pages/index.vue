<!--template>
  <div id = "app-1"> 
    <h1>{{ reverseMes }}</h1>
    <span :title = "message">
      Hover your mouse over me for a few seconds to see my dynamically bound
      title!
    </span>
    <br>
    <span v-if="canSee">you can see 1</span>
    <span v-else>you cannot see 1</span>
    <div id="app-2">
      <ol -->
        <!-- <li v-for="x in todos" :key="x.id">{{ x.text }}</li> -->
        <!-- <li v-for="(x,index) in todos" :key="index">{{ x.text }}</li> -->
      <!-- /ol>
    </div>
    <div id="app-3">
      <button @click="reverseMessage">Reverse</button>
    </div>
    <br>
    <br>
    <span>{{ messageOne }}</span>
    <br>
    <div id="app-4">
      <input type="text" v-model="messageOne" >
    </div>
  </div>
</template -->
<!-- <template>
  <div>
    <ol>
      <li v-for="doDi in doDid" :key="doDi.id">
      {{ doDi.text }}
      </li>
    </ol>
    <br>
    <ol>
      <TodoItem v-for="todo in todos" :key="todo.id" :item="todo">

      </TodoItem>
    </ol>
  </div>
</template> -->
<!-- <template lang="html" -->
  <!-- <div v-once>{{ msg }}</div> -->
  <!-- <div v-html="htmlraw"></div> -->
  <!--div -->
      <!-- <span v-bind:id="spanId">hello</span> -->
      <!-- <span :[spanAttr]="spanId">hello</span>
      <br>
      <button :disabled="buttonDisabled">cannot click</button>
      <br>
      {{ 10 + 20 }}
      <br>
      {{ 10+20 > 35 ? "more than 5" : 'less or equal to 5' }}
      <br>
      {{ 'hello world'.split('').join(',') }}
      <br>
      <button v-if="showButton">you can see me</button>
      <br>
      <a :href="link">welcome google</a>
      <button @click="handleButtonClicked">click me</button>
  </div> -->

<!--/template> -->

<!-- <template lang="html">
   <div> -->
    <!-- {{message.split('').reverse().join('')}} -->
    <!-- <p>Original message: "{{ message }}"</p>
    <p>Computed reversed message: "{{ reversedMessage }}"</p>
    <p>Computed reversed message method: "{{ reversedMessageMethod('Hey,') }}"</p>
   </div>
</template> -->

<!-- <template lang="html">
  <div>
    <p>
      Ask a yes/no question:
      <input v-model="question" />
    </p><br/>
    <p>{{ answer }}</p>
  </div>
</template> -->

<template lang="html">
  <div>
    <h1 :style="{color:'yellow',backgroundColor:'black', margin:'30px 10px 30px 10px'}"> Hello Mr.Silas10</h1>
    <!-- <h1 :class="{active: isActive, 'text-danger': hasError}">Hello, world</h1> -->
    <!-- <h1 :class="classObject">Hello, world</h1> -->
    <h1 :class="[activeClass,errorClass]">Hello, world</h1>
  </div>
</template>
<script>

// import TodoItem from '../components/TodoItem.vue';
// import _ from 'lodash'
// import axios from 'axios'
// const axios = require('axios').default;

export default {
  // 1 components: {
  //   TodoItem
  // },
  // beforeCreate(){
  //   console.log('beforeCreate')
  // },
  // created(){
  //   console.log('created')
  // },
  // beforeMount(){
  //   console.log('beforeMount')
  // },
  // mounted(){
  //   console.log('mounted')
  // },
  // data(){
  //   return{
  //     reverseMes: "Hello Nuxt!",
  //     messageOne: 'Hello Big',
  //     message: "You loaded this page on" + new Date().toLocaleDateString(),
  //     canSee: true,
  //     todos: [
  //       {text: 'Learn Javascript'},
  //       {text: 'Learn Vue'},
  //       {text: 'Hello Angular'},
  //       {text: 'Build something awesome'}
  //       // {id: 1, text: 'Learn Javascript'},
  //       // {id: 2, text: 'Learn Vue'},
  //       // {id: 3, text: 'Hello Angular'},
  //       // {id: 4, text: 'Build something awesome'}
  //     ],
  //     doDid : [
  //       {id: 1, text: 'Hi Silas'},
  //       {id: 2, text: 'Hi Genny'},
  //       {id: 3, text: 'Hello Angaloong'},
  //       {id: 4, text: 'Sawasdee'}
  //     ]
  //   }
  // 1}, 
  // 2 data(){
  //   return{
  //     spanAttr: 'id',
  //     msg: 'hello world',
  //     htmlraw: '<h1>This is raw</h1>',
  //     spanId: 'hello',
  //     buttonDisabled: false,
  //     showButton: true,
  //     link: 'https://www.google.com'
  //   }
  // },
  // methods: {
  //   reverseMessage(){
  //     return (this.reverseMes = this.reverseMes.split("").reverse().join(""))
  //   },
  //   handleButtonClicked(){
  //     console.warn('handleButtonclicked')
  //   }
  //   // buttonDisabled(){

  //   // }
  // }
  // 2computed Properties and Watchers
    // data(){
    //   return{
    //     message : "sila siangchin",
    //     firstName: "Sila",
    //     lastName: "Siangchin"
    //   }
    // },

    // // fullName(){
    // //   return this.firstName + this.lastName
    // // },
    // computed: {
    //     fullName: {
    //       get(){
    //         return this.firstName+' '+this.lastName

    //       },
    //       set(val){
    //         // var names = val.split(' ')
    //         this.firstName = val.split(' ')[0]
    //         this.lastName = val.split(' ')[1]
    //       }
    //     },
    //     // fullName(){
    //     //   return this.firstName + this.lastName
    //     // },
    //     reversedMessage : function(){
    //     return this.message.split('').reverse().join('')
    //   }
    // },
    // 3 name: 'index',
    // created(){
    //   this.debouncedGetAnswer = _.debounce(this.getAnswer,500)
    // },
    // watch: {
    //   question(newQuestion,oldQuestion) {
    //     console.log('NEWQUESTION,OLDQUESTION',newQuestion,oldQuestion)
    //     this.answer =  'Waiting for you to stop typing...'
    //     this.debouncedGetAnswer()
    //   }
    // },
    // data() {
    //   return {
    //     question: '',
    //     answer: 'I cannot give you an answer until you ask a question!'
    //   }
    // },
    // methods: {
    //   // reversedMessageMethod(prefix) {
    //   //   return ( prefix + this.message).split('').reverse().join('')
    //   // },
    //   getAnswer() {
    //     if (!this.question.includes('?')) {
    //       this.answer = 'Questions usually contain a question mark. ;-)'
    //     }else {
    //       this.answer = 'Thinking...'
    //       axios.get(`https://yesno.wtf/api`)
    //       .then((res)=>{
    //         this.answer = _.capitalize(res.data.answer)
    //         // console.log(res)
    //       })
    //       .catch((err)=>{
    //         this.answer = ' Error! Could not reach the API. '+ err
    //       })
    //     }

    //   }
    // }
    // class & style
    data() {
      return {
        // isActive: true,
        // hasError: false,
        // classObject: {
        //   active : true,
        //   'text-danger' : true
        // }
        isActive : true,
        error: null,
        activeClass: 'active',
        errorClass: 'text-danger'
      }
    },
    // it has not parenthesis in script
    computed: {
      classObject: function(){
        return {
          active : this.isActive && !this.error,
          'text-danger' : this.error && this.error.type === 'fatal'
        }
      }
    }
}
</script>



<style lang="css" scoped>
h1.active{
  color:rgb(234, 48, 6);
}

</style>
