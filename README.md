vue路由传参，使用props获取参数
      {
        path: "/register/:id",
        name: "register",
        component: () => import("../views/register/examine.vue"),
        props: (route) =>  ({id: +route.params.id})
      },
      
      
          this.$router.push("/register/561156");
          
  mounted(){
    console.log(this.id)
  }
