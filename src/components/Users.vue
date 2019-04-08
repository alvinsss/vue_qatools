<template>
  <div class="users">
    <!--<h1>Hello Users</h1>-->
    <ul>

      <li v-for="user in users"
          v-on:click="user.show = !user.show ">
        <h2>{{user.name}}</h2>
        <h3 v-show="user.show">
          <a :href='user.linklist' target="_blank" >{{user.dec}}</a>
        </h3>
      </li>

    </ul>
  </div>
</template>

<script>
export default{
    name:'users',
    data(){
      return {
        users:[
          {name:"UI 测试",dec:"",linklist:".",show:true},
          {name:"XX1业务线",dec:"QAdev开发",linklist:"https://ai.taobao.com",show:false},
          {name:"XX2业务线",dec:"QAdev开发",linklist:"https://dianying.2345.com/new.html?browser_xbqy",show:false},
          {name:"XX3业务线",dec:"QAdev开发",linklist:"https://ai.taobao.com",show:false},
          {name:"测试工具",dec:"",linklist:"",show:true},
          {name:"制造测试数据",dec:"QAdev开发",linklist:"https://ai.taobao.com",show:false},
          {name:"MOCK工具",dec:"QAdev开发",linklist:"https://ai.taobao.com",show:false},
          {name:"API测试工具",dec:"QAdev开发",linklist:"https://ai.taobao.com",show:false},
        ]
      }
    }
}
</script>


<style scoped >
h1{
  color:green;
  margin: 0 auto;
}
.users{
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
  ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
  }

  li{
    flex-grow: 1;
    flex-basis: 200px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
  }
</style>
