<template>
  <section class="page-section bg-light" id="team">
    <div class="container">
      <div class="text-center">
        <h2 class="section-heading text-uppercase">Our Amazing Team</h2>
        <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
      </div>
      <div class="row">
        <div class="col-lg-4" v-for="(obj,key) in teamMemberJson" :key="key">
          <div class="team-member">
            <img :src="obj.image" class="mx-auto rounded-circle" >
            <h4>{{ obj.name}}</h4>
            <p class="text-muted">{{ obj.designation}}</p>
            <a class="btn btn-dark btn-social mx-2" target="_blank" v-bind:href="obj.twitter"  ><i class="fab fa-twitter"></i></a>
            <a class="btn btn-dark btn-social mx-2" target="_blank" v-bind:href="obj.fb"><i class="fab fa-facebook-f"></i></a>
            <a class="btn btn-dark btn-social mx-2" target="_blank" v-bind:href="obj.linkedin"><i class="fab fa-linkedin-in"></i></a>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-8 mx-auto text-center"><p class="large text-muted">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eaque, laboriosam veritatis, quos non quis ad perspiciatis, totam corporis ea, alias ut unde.</p></div>
      </div>
    </div>
  </section>
</template>

<script>
import arifAliImg from '../assets/img/team/arif_ali_1.jpg';
import rupomImg from '../assets/img/team/arif_rupom.jpg';
import shohagImg from '../assets/img/team/omar_shohag.jpg';
export default {
  data:()=>({
    teamMemberJson:[
      {
        image:arifAliImg,
        name:'Arif Ibne Ali',
        designation:'Managing Director',
        fb:'https://www.facebook.com/arifibneali',
        twitter:'https://www.twitter.com/arifibneali',
        linkedin:'https://www.linkedin.com/in/arifibneali/',
      },
      {
        image:rupomImg,
        name:'Ariful Islam',
        designation:'Project Manager',
        fb:'https://www.facebook.com/arifrupom.0507',
        twitter:'https://www.twitter.com/arifibneali',
        linkedin:'https://www.linkedin.com/in/arif-rupom-8451bb11b/',
      },{
        image:shohagImg,
        name:'Md Omar Faruk',
        designation:'Software Developer',
        fb:'https://www.facebook.com/omarshohag93',
        twitter:'https://www.twitter.com/arifibneali',
        linkedin:'https://www.linkedin.com/in/omar-shohag/',
      },

    ]
  })
}
</script>

<style >

</style>