# vuex
    const store = new Vuex.Store({

      state:{
  
         nickName:'',
    
         cartCount:0
    
      },
  
      mutations:{
  
         updateUserInfo(state,nickName){
    
          state.nickName=nickName
      
        },
    
         updateCartCount(state,cartCount){
    
          state.cartCount=cartCount
      
        }
    
      }
  
    })

     computed:{
 
        nickName(){
    
          return this.$store.state.nickName
      
        }
    
      },
  
    this.$store.commit('updateUserInfo',res.result.userName)
