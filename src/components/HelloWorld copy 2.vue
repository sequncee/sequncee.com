<template>

  <div class="fullpage" id="fullpage">
    <remote-js cdn="https://cdnjs.cloudflare.com/ajax/libs/fullPage.js/3.0.9/fullpage.js"></remote-js>

    <img
      class="img-big"
      src="../assets/images/bg/glitch-2717636_960_720.jpg"
      alt="image description"
    />
    <div class="text-holder random-words align-center">
      <h1>
        我们 <span class="mark" style="opacity: 1;">诞生于虚无</span>,
        <span class="mark" style="opacity: 1;">致力于人类</span>
        <!-- <span class="mark" style="opacity: 1;">Gnarwahl</span> -->
        <br/>为了
        <span class="mark" style="opacity: 1;">填满空虚</span>
        <br/><br/><br/>
        虚拟组织
        <span class="mark" style="opacity: 1;">Sequnce E</span>

        <div class="text-center">
          <span class="icon-wrap"
            ><a
              aria-label="Random tagline generator"
              href="#"
              class="fa fa-random"
              aria-hidden="true"
            ></a
          ></span>
        </div>
      </h1>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
// @Component
// export default class HelloWorld extends Vue {
//   @Prop() private path!: string;
  
// }

</script>
<script>
export default {
  components: {
    'remote-js': {
        render(h) {
            return (
                <script type= 'text/javascript' src={this.cdn}/>
            )
        },
        props: {
            cdn:  {
                type: String,
                required: true
            }
        }
    },
    'remote-css': {
        render(h) {
            return (
                <link rel='stylesheet' type='text/css' href={this.cdn} />
            )
        },
        props: {
            cdn:  {
                type: String,
                required: true
            }
        }
    }
}
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// .hello {
//   background: #3f3f41;
//   position: relative;
// }
.img-big {
  width: 100%;
  opacity: 0.45;
}

.align-center {
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  padding: 30px 24px 0;
  position: absolute;
  max-width: 1048px;
}
.mark {
  // color: #f86249;
  color: #ff7f00;
}
h1 {
  color: #fff;
  font-size: 68px;
  line-height: 1.097;
  margin: 0;
}
*,
::before,
::after {
  box-sizing: inherit;
}
.image-replace {
  margin-bottom: 85px;
}
.image-replace {
  margin-bottom: 0px;
}
</style>
