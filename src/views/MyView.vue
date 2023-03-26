<script>
import DirectiveVFor from '../components/directives/DirectiveVFor.vue';
import DirectiveVif from '../components/directives/DirectiveVif.vue';
import DirectiveVModel from '../components/directives/DirectiveVModel.vue';
import DirectiveVShow from '../components/directives/DirectiveVShow.vue';
import ComputedProps from '../components/myComponents/computed-properties/ComputedProps.vue';
import RawHtmlData from '../components/myComponents/RawHtmlData.vue';
import SingleComponent from '../components/myComponents/SingleComponent.vue'
import ChildComponent from '../components/props/ChildComponent.vue';
import ParentComponent from '../components/props/ParentComponent.vue';

export default {
    components: { SingleComponent, RawHtmlData, DirectiveVShow, DirectiveVif, DirectiveVModel, DirectiveVFor, ComputedProps, ChildComponent, ParentComponent },
}
</script>

<template>
    <div>
        <h1>My Single Page from FemCoders</h1>
        ---------------------------------
        <RawHtmlData />
        <SingleComponent></SingleComponent>
        ---------------------------------
        <DirectiveVShow />
        ----------------------------------
        <DirectiveVif />

        <directive-v-model></directive-v-model>

        <directive-v-for></directive-v-for>

        <computed-props></computed-props>

        <ParentComponent />
        
    </div>
</template>

<style lang="css" scoped>
h1{
    color: red;
}

</style>