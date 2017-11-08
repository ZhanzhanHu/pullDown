# README
一个高度自定义的上拉加载，下拉刷新插件

# **Installation**
`将文件中的plugin文件夹导入自己项目的src文件中`
    
# **Usage**

### 导入`pull`到项目中
`import mypull from './plugin/pull'`


##### Register component:    
`Vue.use(pull)`

##### Then use it:
    <template>
	  <wapper :loadMore='func1' :refreshPage='func2'> content </wapper>
    </template>
    
    js
    export default {
    methods: {
      func1(loadMoreEnd) {
        .....加载代码
        loadMoreEnd()
      },
     func2(refreshEnd) {
        ....刷新代码
        refreshEnd()
      }
    }
