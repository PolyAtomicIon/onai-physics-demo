<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
    text: {
        default: '',
    },
    imgSrc: {
        default: null,
    },
    solution: {
        default: '',
    },
})

</script>

<template>
    <div class="problem">
        <div class="problem__statement">
            <p class="problem__text">
                {{props.text}}
            </p>
            <div v-if="props.imgSrc" class="problem__img">
                <img :src="props.imgSrc"
                    alt="problem-img">
            </div>
        </div>
        <div v-if="props.solution"  class="spoileropen" role="tab" tabindex="1">
            <div role="tabpanel" class="problem__solution">
                <p>{{props.solution}}</p>
            </div>
            <span role="button" tabindex="0" class="spoilerclose">Hide</span>
        </div>
    </div>
</template>


<style scoped>
.problem {
    background: #454545;
    padding: 15px;
    border-radius: 15px;
    position: relative;
    overflow: hidden;
    color: #fff;
    max-width: 600px;
    -webkit-box-shadow: 4px 4px 8px 0px rgba(107, 157, 195, 0.2);
    -moz-box-shadow: 4px 4px 8px 0px rgba(107, 157, 195, 0.2);
    box-shadow: 4px 4px 8px 0px rgba(107, 157, 195, 0.2);
}

.problem__statement {
    margin-bottom: 15px;
    display: flex;
    justify-content: space-between;
    gap: 20px;
}

.problem__text {
    max-width: 350px;
}

.problem__solution {
    padding: 0 10px;
    border-left: 3px solid #4EC5D4;
    margin-top: 40px;
    margin-left: 12px;
}

.problem__img img {
    margin-top: 15px;
    border-radius: 15px;
    max-height: 250px;
}

.spoilerclose {
    display: none;
    background-color: #0d5f7d;
    background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    font-size: 24px;
    width: 100%;
    cursor: pointer;
    height: 40px;
    text-indent: 10px;
    position: absolute;
    top: 0px;
    left: 0;
}

.spoilerclose:hover {
    background-image: linear-gradient(45deg, #35737c 10%, #146b8c 20%);
}

.spoileropen:before {
    content: 'Solution';
    cursor: default;
    text-indent: 10px;
    width: 100%;
    cursor: pointer;
    height: 40px;
    background-color: #2B90B6;
    background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    font-size: 24px;
    display: block;
    position: absolute;
    top: 0px;
    left: 0;
}

.spoileropen:hover:before {
    background-image: linear-gradient(45deg, rgb(45, 151, 167) 10%, #146b8c 20%);
}

.spoileropen {
    height: 40px;
    width: 100%;
    outline: none;
    float: left;
    position: relative;
    overflow: hidden;
    -webkit-transition: height 0.3s ease;
    -moz-transition: height 0.3s ease;
    -ms-transition: height 0.3s ease;
    -o-transition: height 0.3s ease;
    transition: height 0.3s ease;
}

.spoileropen:focus {
    height: auto;
}

.spoileropen:focus .spoilerclose {
    display: block;
}

.spoileropen:focus:before {
    display: none;
}
</style>