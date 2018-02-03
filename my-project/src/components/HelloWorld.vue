<template>
  <div class="hello">
    <Carousel autoplay v-model="value" loop>
        <CarouselItem>
            <div class="demo-carousel">1</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">2</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">3</div>
        </CarouselItem>
        <CarouselItem>
            <div class="demo-carousel">4</div>
        </CarouselItem>
    </Carousel>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      value: 0
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  width:200px;
  height: 100px;
  margin: 100px auto;

}
.hello .ivu-carousel,.demo-carousel{
   width: inherit;
   height: inherit
}
.hello .ivu-carousel-item{
  height: 100px!important;
  background: #cd5d13;
  color:white;
}
.demo-carousel{
   line-height: 100px;
   font-size: 16px
}
</style>
