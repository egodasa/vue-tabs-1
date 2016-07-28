<template>
    <ul class="nav nav-tabs">
        <li role="presentation" :class="{'active':tab.active}" v-for="tab in tablist" ><a href="#{{tab.name}}" aria-controls="{{tab.name}}" role="tab" data-toggle="tab">{{tab.title}}</a></li>
    </ul>  
    <div class="tab-content">
        <slot></slot>
    </div>
</template>
<script>
    export default{
       data () {
          return {
            tablist: []
          }
      },
      ready(){
        //console.log(this.$children);
        let self = this;
        this.$children.forEach(c=>{
            self.tablist.push({
                    "name": c.name,
                    "title": c.title,
                    "active": c.active
                });
        })
      }
  }
</script>