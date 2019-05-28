<template>
    <div>
        <div 
            @click="expandIcon"
            :style="{'margin-left': `${depth * 20}px`}"
        >
        <h1>{{node.name}}</h1>
        </div>
        <Demo1
            v-if="expanded"
            v-for="(child, index) in node.children" :key="index"
            :node="child"
            :depth = "depth + 1"
        />
    </div>
</template>

<script>
export default {
    name: 'Demo1',
    props: {
        node: Object,
        depth: {
            type: Number,
            default: 0
        }
    },
    data() {
        return {
            expanded: false,
        }
    },
    methods: {
      expandIcon(){
        this.expanded = !this.expanded;
      }
    }
    
}
</script>

<style>

</style>
