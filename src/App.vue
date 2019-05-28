<template>
  <div id="app">
    <Demo1 :node="root"/>
  </div>
</template>

<script>
import Demo1 from './components/Demo1'

export default {
  components: {
    Demo1
  },
  name: 'app',
  data () {
    return {
      root: 
        {
        name: 'Click Me',
        children: [
          {
            name: 'Mobile',
            children: [
              {
                name: 'Apple',
                children: [
                  {
                    name: 'XS'
                  },
                  {
                    name: 'XS Max'
                  }
                ]
              },
              {
                name: 'Blackberry',
                children: [
                  {
                    name: 'Evolve'
                  },
                  {
                    name: 'Elite'
                  }
                ]
              }
            ]
          },
          {
            name: 'TV',
            children: [
              {
                name: 'Samsung',
                children: [
                  {
                    name: 'Samsung1'
                  },
                  {
                    name: 'Samsung2'
                  }
                ]
              },
              {
                name: 'Sony',
                children: [
                  {
                    name: 'Sony1'
                  },
                  {
                    name: 'Sony2'
                  }
                ]
              }
            ]
          },
          {
            name: 'Cars',
            children: [
              {
                name: 'Volkswagen',
                children: [
                  {
                    name: 'Passat'
                  },
                  {
                    name: 'Polo'
                  }
                ]
              },
              {
                name: 'Hyundai',
                children: [
                  {
                    name: 'Creta'
                  },
                  {
                    name: 'Xcent'
                  }
                ]
              }
            ]
          },
          
        ]
      }
      
      
    }
  }
}
</script>

<style>

</style>

