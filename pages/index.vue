<template>
  <div class="w-full overflow-hidden">
    <div class="hero md:min-h-screen md:max-h-screen md:h-screen w-full relative">
      <HeaderParts/>
      <div class="flex mx-4 md:mx-0 flex-col items-center justify-center mt-20 relative z-10" data-aos="fade-left">
        <h1 class="text-4xl md:text-5xl text-center text-white font-semibold" >
          Build Your Carrer. <br/>
          Grow Together & Faster
        </h1>
        <nuxt-link to="/home" class="rounded-full mt-4 mb-24 px-6 py-2 inline-block" style="background-color: #F2AD5F" >Explore Mine</nuxt-link>
      </div>
      <PassThrough class="transform -translate-x-48 md:translate-x-0 -translate-y-48 md:-translate-y-32 absolute top-0 scale-75 md:scale-100"/>
    </div>
    <div class="illustration flex items-center justify-center -mt-16 md:-mt-48 relative z-20">
      <img src="~assets/images/illustration.png"/>
    </div>
    <BannerParts/>
    <ServicesParts/>
    <div class="flex mt-32 flex-col items-center justify-center" data-aos="slide-up">
      <h1 class="text-center font-color-one text-4xl mx-4 md:mx-0 font-semibold" data-aos="slide-down" data-aos-duration="1000">Our Feature Jobs <br/> That Might You Need</h1>
      <JobsItem/>
      <nuxt-link to="/home" class="block hover:underline my-6" data-aos="slide-down" data-aos-duration="1000">View More Incoming Jobs</nuxt-link>
    </div>
    <FooterParts/>
  </div>
</template>

<script>
import PassThrough from "~/assets/images/pass-through.svg?inline"
export default {
  components : {
    PassThrough
  }
}
</script>

<style>
.container {
  font-family: 'Quicksand', sans-serif;
  background: #e5e5e5;
}
.hero {
  background: #10495C;
  border-bottom-left-radius: 42%;
  border-bottom-right-radius: 42%;
}
.link-color {
  color: #B0C3C9
}
.link-color.active,
.link-color:hover {
  color: #F2AD5F; 
}
.link-color.active::before {
  position: absolute;
  top:25px;
  height: 3px;
  content: "";
  width:100%;
  background: #F2AD5F;
}
.link-color:hover::before {
  position: absolute;
  top:25px;
  height: 3px;
  content: "";
  width:100%;
  background: #F2AD5F;
}
.color-one {
  background:  #F2AD5F;
}
.color-two {
  background: #10495C;
}
.ellipse {
  top: -4px;
  left:-4px;
}
.-z-1 {
  z-index: -1;
}
.image-one {
  border-color: #10495C;
}
.image-two {
  border-color: #F2AD5F; 
}
.font-color-one{
  color:#10495C;
}
.img-part-one {
  left: 75px;
}
.img-part-two {
  top: 220px;
  left: 200px;
}
.img-part-three {
  right: 75px;
}
</style>
