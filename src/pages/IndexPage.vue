<template>
  <div class="bg-white">
  <q-page>
    <div class="banner" style="background-color: white;">
      <div class="q-pa-md">
        <div class="row justify-center">
        <div class="col-12 col-md q-pa-md text-black">
        <div style="max-width: 650px;" class="q-ml-auto q-mr-auto">
        <h3 class="text-weight-bolder q-mt-lg">FullStack Developer Training &amp; Placement</h3>
        <div class="mixedcolor q-pa-sm text-weight-bolder text-white">100% Job Guarantee</div>
        <div class="landing_banner">
          <p class="text-weight-bold q-pt-sm">Ranked #1 Full Stack Training Institute with Placement</p>
        </div>
        <div>
          <p class="text-weight-medium ">Edex IT Solutions provides the Best Full Stack Training in Madurai, Chennai &amp; Online with 100% placements. Learn Full Stack Course from Basics to Advanced and get real-time experience.</p>
        </div>
        <div class="text-weight-medium">
          <div><q-icon name="star" class="q-pa-sm"></q-icon><span>Enroll Now for Trending Courses with Job Assurance</span></div>
          <div><q-icon name="star" class="q-pa-sm"></q-icon><span>5+ Years Experinced Mentors</span></div>
          <div><q-icon name="star" class="q-pa-sm"></q-icon><span>4+ Branches in Tamilnadu</span></div>
        </div>
        <div class="row q-pt-md">
          <div clas="col-6"><q-btn href="DOC-20231204-WA0009" download="edex.pdf" target="_blank" class="bg-red-13 text-white text-weight-bold">Download Brouchure</q-btn></div>
          <div class="col-6 text-weight-bolder q-pa-sm">*Available for Both <span class="text-yellow-9"> Online& Classroom</span></div>
        </div>
       </div>
      </div>

      <div class="col-12 col-md gt-sm">
        <div style="max-width: 550px;" class="q-ml-auto q-mr-auto">
          <div class="q-pt-md">
            <div class="q-mt-lg">
              <img src="../assets/banner-6-desktop.jpg" style="height: 440px;width: 440px;">
            </div>       
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
  <div class="lt-md justify-center">
        <div style="max-width: 550px;display: flex;justify-content: center;align-items: center;" >
          <div class="">
            <div class="">
              <img src="../assets/banner-6-desktop.jpg" style="height: 440px;width: 370px;">
            </div>       
          </div>
        </div>
      </div>

<div class="bg-blue-9 q-pa-lg">
  <div class="text-center">
    <div class="row q-gutter">
      <div class="col-12 col-md col-sm-4 align-center" v-for="img in images">
      <img :src="img">
      </div>
    </div>
  </div>
</div>

<!-- program highlights -->
<section id="programHighlights">
<div class="bg-white q-pb-lg">
  <div class="q-pa-md text-center">
      <div class="row q-px-xl q-pt-lg q-pb-sm text-h5 text-weight-bold" 
      style="display: flex;flex-direction: column;justify-content: center;align-items: center;">
        Program Highlights</div>
        <div class="radiantthemes-separator-block" style="width: 100px; height: 2px;">
          <div class="radiantthemes-separator-block-gap"></div>
        </div>

      <div class="text-center">
      <div class="row q-pa-md q-gutter-sm">
         <q-card class="my-card col-12 col-sm-12 col-md align-center" v-for="x in cardItems">
          <div class="text-center bg-blue-grey-1"><img :src="x.img" class="img-fluid"></div>
              <q-card-section>
                <div class="text-weight-bold">{{ x.name }}</div>
                <div class="q-py-md text-blue-grey-8">{{ x.des }}</div>
              </q-card-section>
    </q-card>
    </div> 
  </div>

  </div>
</div>
</section>
</q-page>

<q-page>
  <div class="q-pb-lg" id="startnow">
  <div class="q-pa-md text-center">
      <div class="row q-px-xl q-pb-sm text-h5 text-weight-bold text-black" 
      style="display: flex;flex-direction: column;justify-content: center;align-items: center;">
        Start With Us</div>
        <div class="radiantthemes-separator-block" style="width: 100px; height: 2px;">
          <div class="radiantthemes-separator-block-gap"></div>
        </div>
  <div  class="q-pa-md" style="display: flex;flex-direction:column;justify-content: center;align-items: center;">
    <div class="row bg-white q-pa-lg" style="border-radius: 20px;">
      <div class="col-6">
        <div class="text-weight-bold text-blue-7">Let Us Help</div>
          <div class="text-blue-8 text-weight-bold">Finding Your <span class="text-weight-bold text-black">Right Courses</span></div>
      </div>
      <div class="col-6 text-center q-pt-sm">
          <q-btn href="https://edextech.io/" target="_blank" class="bg-deep-orange-9 text-white text-weight-bold" style="border-radius: 5px;">Get started</q-btn>
      </div>
    </div>
  </div>

<div class="q-px-xl">
  <div class="row q-gutter-sm">
    <div class="col-12 col-md bg-white" style="border-radius: 20px;">
      <div class="row text-center">
        <div class="col text-center q-pa-lg">
          <div>
            <div class="text-weight-bold text-blue-9">Enroll Now at Edex</div>
            <div class=" text-blue-grey-9 text-weight-bold q-pa-sm">Discover How We Simplify Your Learning Path</div>
            <div><q-btn @click="enquiry = true" class="bg-deep-orange-9 text-white text-weight-bold" style="border-radius: 5px;">Book A Free Demo</q-btn>
              <q-dialog v-model="enquiry">
              <div class="col-12 col-md bg-white" style="max-width: 500px;border-radius: 20px;border:1px solid grey">
    
     <div class="q-pa-md bg-blue-grey-2 text-center  text-h6 text-weight-bold" style="border-top-right-radius: 15px;border-top-left-radius: 15px;">Book a free demo</div>
    
    <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="q-gutter-md q-pa-md"
            style=""
            >
            <q-input
            outlined
            v-model="name"
            label="Your name *"
            hint="Name and surname"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Enter Your Name']"
            />

            <q-input
            outlined
            type="email"
            v-model="email"
            label="Your Email *"
            hint="Enter Your Email "
            lazy-rules
            :rules="[
            val => !!val || 'Please type your email',
            val => /.+@.+\..+/.test(val) || 'Please type a valid email'
            ]"
            />
            <q-input
            outlined
            type="text"
            v-model="mobile"
            label="Your mobile *"
            hint="Enter your mobile number"
            lazy-rules
            :rules="[ val => val && val.length == 10 || 'Please Enter Your Mobile Number']"
            />

            <div class="text-center">
            <q-btn label="Submit" type="submit" color="deep-orange-9"/>

            </div>
    </q-form>
  </div> 
          </q-dialog>

            </div>
          </div>
        </div>
         </div>
    </div>
    <div class="col-12 col-md bg-white" style="border-radius: 20px;">
      <div class="row text-center">
        <div class="col text-center q-pa-lg">
          <div>
            <div class="text-weight-bold text-blue-9">Enroll Now at Edex</div>
            <div class=" text-blue-grey-9 text-weight-bold q-pa-sm">Start Climbing Up Your Career Ladder With Edex</div>
            <div><q-btn href="https://edextech.io/" target="_blank" class="bg-deep-orange-9 text-white text-weight-bold" style="border-radius: 5px;">Explore Courses</q-btn></div>
          </div>
        </div>
        </div>
    </div> 
  </div>
</div>
</div>
</div>

<!-- skills covered -->
<div class="text-center bg-blue-grey-1">
  <div class="row q-px-xl justify-center q-pt-lg text-h5 text-weight-bold q-pb-sm">Skills Covered</div>
  <div class="radiantthemes-separator-block" style="width: 100px; height: 2px;">
    <div class="radiantthemes-separator-block-gap"></div>
  </div>
  <div class="text-center q-pa-lg">
  <div class="row">
    <div class="col-12 col-md col-sm-4  align-center" v-for="x in skillImages">
      <div class="q-pa-md">
        <q-img :src="x.img" style="height: 100px;width: 150px;"></q-img>
        <div class="text-blue-grey-10 text-weight-bold q-pa-sm">{{ x.title }}</div>
      </div>  
    </div>
  </div>

  <div class="row">
    <div class="col-12 col-md col-sm-4  align-center" v-for="x in skillImagesTwo">
      <div class="q-pa-md">
        <q-img :src="x.img" style="height: 100px;width: 150px;"></q-img>
        <div class="text-blue-grey-10 text-weight-bold q-pa-sm">{{ x.title }}</div>
      </div>
      
    </div>

  </div>
</div>
</div>
<!-- skills covered end -->

<section id="courseDetails">
<div class="q-pa-lg">  
<div class="q-pa-md text-center">
  <div class="row q-px-lg q-pt-lg q-pb-sm justify-center  text-h5 text-weight-bold ">Course Content</div>
  <div class="radiantthemes-separator-block" style="width: 100px; height: 2px;">
    <div class="radiantthemes-separator-block-gap"></div>
  </div>
  <div>
    <div class="row q-pa-sm q-gutter-sm">
      <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in comboCourses">
          <div class="bg-blue-grey-1 q-pa-sm">
            <div class="row q-gutter-sm">
            <div class="col-3 q-pa-sm"><img :src="x.img" style="height: 50px;width: 90px;"></div>
            <div class="col q-pt-lg q-px-md text-weight-bold"><span>{{ x.h3 }}</span>
            <span><img src=""></span></div>
            </div>
          </div>
              <q-card-section class="text-center">
                <div class="row q-pa-md">
                  <div class="col" style="border-right: 1px solid rgb(141, 140, 140);">
                    <div class="text-blue-grey-9 text-weight-bold">Skill Level</div>
                    <div class="text-blue-grey-7">Advanced</div>
                  </div>
                  <div class="col" style="border-right: 1px solid rgb(141, 140, 140);">
                    <div class="text-blue-grey-9 text-weight-bold">days</div>
                    <div class="text-blue-grey-7">60</div>
                  </div>
                  <div class="col">
                    <div class="text-blue-grey-9 text-weight-bold">Learners</div>
                  <div class="text-blue-grey-7">{{ x.c3 }}</div>
                </div>
                </div>
              </q-card-section>
    </q-card>
    
    </div>
  </div>
  <div class="text-center">
  <div class="row bg-white q-pa-md" style="border-radius: 5px;">
    <div class="col q-pa-sm">
      <div class="text-weight-bolder q-pa-sm text-h6">Enroll Now at 40,000/- Only</div>
      <div><q-btn @click="enquiry = true" class="bg-deep-orange-14 text-white">Enroll Now</q-btn>
        <q-dialog v-model="enquiry">
              <div class="col-12 col-md bg-white" style="max-width: 500px;border-radius: 20px;border:1px solid grey">
    
     <div class="q-pa-md bg-blue-grey-2 text-center  text-h6 text-weight-bold" style="border-top-right-radius: 15px;border-top-left-radius: 15px;">Enquiry Now</div>
    
    <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="q-gutter-md q-pa-md"
            style=""
            >
            <q-input
            outlined
            v-model="name"
            label="Your name *"
            hint="Name and surname"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Enter Your Name']"
            />

            <q-input
            outlined
            type="email"
            v-model="email"
            label="Your Email *"
            hint="Enter Your Email "
            lazy-rules
            :rules="[
            val => !!val || 'Please type your email',
            val => /.+@.+\..+/.test(val) || 'Please type a valid email'
            ]"
            />
            <q-input
            outlined
            type="text"
            v-model="mobile"
            label="Your mobile *"
            hint="Enter your mobile number"
            lazy-rules
            :rules="[ val => val && val.length == 10 || 'Please Enter Your Mobile Number']"
            />

            <div class="text-center">
            <q-btn label="Submit" type="submit" color="deep-orange-9"/>

            </div>
    </q-form>
  </div> 
          </q-dialog>
      </div>
    </div>
  </div>
</div>
</div>
</div>
</section>


<div class="bg-blue-grey-1">
  <div class="q-pa-lg q-mx-md bg-blue-grey-1">
    <div class="q-pa-md text-center">
      <div class="row justify-center q-pt-sm q-pb-sm  text-h5 text-weight-bold">Added Advantages</div>
      <div class="radiantthemes-separator-block justify-center" style="width: 100px; height: 2px;">
          <div class="radiantthemes-separator-block-gap"></div>
      </div>
        <div class="q-pa-lg">
          <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in best">
              <div class="bg-blue-9 q-pa-md">
                <div class="text-weight-bold q-pa-sm text-h6 text-white">{{ x.title }}</div>
              </div>
              <q-card-section class="q-pa-lg">
                <div class="text-weight-bold"><img :src="x.img" style="height: 100px;width: 100px;"></div>
                <div class="text-blue-grey-9">{{ x.des }}</div>
              </q-card-section>
            </q-card>
          </div>
          <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in bestTwo">
              <div class="bg-blue-9 q-pa-md">
                <div class="text-weight-bold q-pa-sm text-h6 text-white">{{ x.title }}</div>
              </div>
              <q-card-section class="q-pa-lg">
                <div class="text-weight-bold"><img :src="x.img" style="height: 100px;width: 100px;"></div>
                <div class="text-blue-grey-9">{{ x.des }}</div>
              </q-card-section>
            </q-card>
          </div>
        </div>
    </div>
  </div>
</div>

 <!-- tools covered -->
<div class="text-center bg-white">
  <div class="row q-px-xl justify-center q-pt-lg q-pb-sm text-h5 text-weight-bold ">Tools Covered</div>
  <div class="radiantthemes-separator-block" style="width: 100px; height: 2px;">
    <div class="radiantthemes-separator-block-gap"></div>
  </div>
  <div class="text-center q-pa-lg">
    <div class="row">
    <div class="col-12 col-md col-sm-4  align-center" v-for="x in toolsImages">
      <div class="q-pa-md">
        <q-img :src="x.img" style="height: 100px;width: 150px;"></q-img>
        <div class="text-blue-grey-10 text-weight-bold q-pa-sm">{{ x.title }}</div>
      </div>  
    </div>
  </div>

  <div class="row">
    <div class="col-12 col-md col-sm-4  align-center" v-for="x in toolsImagesTwo">
      <div class="q-pa-md">
        <q-img :src="x.img" style="height: 100px;width: 150px;"></q-img>
        <div class="text-blue-grey-10 text-weight-bold q-pa-sm">{{ x.title }}</div>
      </div>  
    </div>
  </div>

  </div>
</div>
<!-- tools covered end -->


   


  <!-- why edex -->
  <div class="q-pa-lg ">
    <div class="q-pa-md text-center">
      <div class="row  q-pt-sm justify-center text-h5 text-weight-bold">Why Edex</div>
      <div class="radiantthemes-separator-block" style="width: 90px; height: 2px;">
    <div class="radiantthemes-separator-block-gap"></div>
  </div>
      <div class="q-pa-lg">
        <div class="row q-pa-sm q-gutter-md">
          <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in arrayOne" style="border-bottom: 3px solid #0e81de;">
             <div class="row q-pa-sm">
              <div class="col-4"><img :src="x.img" style="height: 70px;width: 90px;"> </div>
              <div class="col q-px-md text-blue-grey-10" style="display: flex;flex-direction: column;justify-content: center;align-items: center;">{{ x.des }}</div>
             </div>
            </q-card>
        </div>
        <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in arrayTwo" style="border-bottom: 3px solid #0e81de;">
              <div class="row q-pa-sm">
                <div class="col-4"><img :src="x.img" style="height: 70px;width: 90px;"> </div>
                <div class="col q-px-md text-center text-blue-grey-10" style="display: flex;flex-direction: column;justify-content: center;align-items: center;">{{ x.des }}</div>
             </div>
            </q-card>
          </div>
      </div>
    </div>
  </div>




<section id="contact">
<div class="q-pa-md" style="display: flex;justify-content: center;align-items: center;">
      <div class="q-pa-md text-center">
        <div class="row  q-pt-sm q-pb-sm justify-center text-h5 text-weight-bold">Enquiry Now</div>
      <div class="radiantthemes-separator-block" style="width: 90px; height: 2px;">
    <div class="radiantthemes-separator-block-gap"></div>
  </div>
  <div class="row q-pa-sm" style="display: flex;flex-direction: row;justify-content: space-evenly;align-items: center;">
  <div class="col-12 col-md gt-xs" style="text-align: center;">
    <img src="/logo-edex.jpg" style="height: 70px;width: 70px;">
    <div class="text-h6 text-weight-bold">Empowering Your Future in IT</div>
    <div class="q-px-md text-weight-bold">We are happy to help you 24/7.</div>
      <div class="q-px-xl q-py-md text-blue-grey-9">Unlock Your Potential with IT Training.Embark on a journey to success with our comprehensive IT training programs. 
    Our expert instructors and hands-on learning approach ensure you gain practical knowledge and real-world experience.
    Join us to build a solid foundation and excel in the dynamic field of information technology.
  </div>
    
    <img src="../assets/program.jpg">
       
  </div>
  <div class="lt-sm">
      <img src="/logo-edex.jpg" style="height: 70px;width: 70px;">
    <div class="text-h6 q-pa-sm text-weight-bold">Empowering Your Future in IT</div>
    <div class="q-pa-xs text-weight-bold">We are happy to help you 24/7.</div>
      
    </div>
  <div class="col-12 col-md" style="min-width: 320px;border-bottom: 10px solid #0e81de;border-left: 8px solid #0e81de;border-radius: 20px;">
    
    <div class="q-pa-md bg-blue-grey-1 text-h6 text-weight-bold" style="border-top-right-radius: 15px;border-top-left-radius: 15px;">Submit Your Details</div>
    
    <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="q-gutter-md q-pa-md"
            style=""
            >
            <q-input
            outlined
            v-model="name"
            label="Your name *"
            hint="Name and surname"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Enter Your Name']"
            />

            <q-input
            outlined
            type="email"
            v-model="email"
            label="Your Email *"
            hint="Enter Your Email "
            lazy-rules
            :rules="[
            val => !!val || 'Please type your email',
            val => /.+@.+\..+/.test(val) || 'Please type a valid email'
            ]"
            />
            <q-input
            outlined
            type="text"
            v-model="mobile"
            label="Your mobile *"
            hint="Enter your mobile number"
            lazy-rules
            :rules="[ val => val && val.length == 10 || 'Please Enter Your Mobile Number']"
            />

            <div class="text-center">
            <q-btn label="Submit" type="submit" color="deep-orange-9"/>

            </div>
    </q-form>
  </div>
</div>
      
      
  </div>
</div>
</section> 

<!-- place QPageScroller at end of page -->
<q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
    <q-btn fab icon="keyboard_arrow_up" color="red" />
</q-page-scroller>

<div class="bg-blue-grey text-white" style="display: flex;justify-content: center;align-items: center;">

  <div class="row q-pa-sm justify-center">
    <div class="q-pa-sm">Chennai: +918055224403</div>
    <div class="q-pa-sm">Madurai: +918055224403</div>
    <div class="q-pa-sm">Online: +918055224403</div>
    <div class="q-pa-sm"><q-icon name="email" class="q-pa-xs"></q-icon>contact@edextech.in</div>

  </div>
</div>

<div class="bg-black q-pa-sm text-center">
  <div class="text-white q-pa-md">Copyright 2023 Edex | All Rights Resrved</div>
</div>
</q-page>
</div>
</template>

<script>
import { defineComponent,ref } from 'vue'
import {useQuasar} from 'quasar'

export default defineComponent({
  name: 'IndexPage',
  
  setup(){

    const $q = useQuasar()

    const name = ref(null)
    const email = ref(null)
    const mobile = ref(null)
    const accept = ref(false)
    return{
      enquiry: ref(false),
      step: ref(1),
      name,
      email,
      mobile,
      accept,

      onSubmit () {
        if (accept.value !== true) {
          $q.notify({
            color: 'red-5',
            textColor: 'white',
            icon: 'warning',
            message: 'You need to accept the license and terms first'
          })
        }
        else {
          $q.notify({
            color: 'green-4',
            textColor: 'white',
            icon: 'cloud_done',
            message: 'Submitted'
          })
        }
      },
      onReset () {
        name.value = null
        email.value = null
        mobile.value = null
        accept.value = false
      },



      images:["/icon_1.png",
      "/icon_2.png",
      "/icon_3.png",
      "/icon_4.png",
      "/icon_5.png",
      "/icon_6.png"
      
       ],
    cardItems:[{img:"card_icon_1.png",name:"Top-Notch Faculty",des:"Trainers at Edex are passionate  about training, and carry 6+ years  of industry experience."},
               {img:"card_icon_2.png",name:"Hackathons and Coding Challenges",des:"Sharpen your skills by engaging in coding contests that involve collaborating with your peers."},
               {img:"card_icon_3.png",name:"Guaranteed Job Interviews",des:"Your placement preparation starts from Day 1 and prepares you for guaranteed job interviews across our 2000+ partner companies until you receive your first job offer."},
               {img:"card_icon_4.png",name:"Real-life Projects and Bootcamps",des:"Learners will work on real-life scenarios from various domains to get application knowledge."}
      ],
      comboCourses:[{img:"/combo_course_1.png",
                            h3:"FRONTEND",p:"5.0(1965)",c3:"150+"},
                    {img:"/backend.jpg",h3:"BACKEND",p:"5.0(1865)",c3:"150+"},
                    {img:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR606sHWwbqvnffryckkukv9IwycRCF3sXZxQ&usqp=CAU",h3:"DATABASE",p:"5.0(1970)",c3:"150+"}]
      
    , toolsImages:[{img:"/Tools_1.png",title:"JAVA DEVELOPMENT KIT"},
                  {img:"/Tools_2.png",title:"ECLIPSE"},
                  {img:"/Tools_3.png",title:"SPRINGBOOT SUIT"},
                  {img:"/Tools_4.png",title:"AWS"},
                  {img:"/Tools_5.png",title:"GITHUB"},
                  {img:"/Tools_6.png",title:"POSTMAN"},
                ],
    toolsImagesTwo:[
                {img:"/Tools_7.png",title:"MONGOD DB"},
                  {img:"/Tools_8.png",title:"APACHE MAVEN"},
                  {img:"/Tools_9.png",title:"MySQL WORKBENCH"},
                  {img:"/Tools_10.png",title:"JSON"},
                  {img:"/Tools_11.png",title:"REACT"},
                  {img:"/Tools_12.png",title:"KUBERNETES"},
                
                ],
    
    skillImages:[{img:"/Skill_1.png",title:"HTML"},
                    {img:"/Skill_2.png",title:"CSS"},
                    {img:"/Skill_3.png",title:"JAVAVSCRIPT"},
                    {img:"/Skill_4.png",title:"JAVA"},
                    {img:"/Skill_5.png",title:"PYTHON"},
                    {img:"/Skill_6.png",title:"SPRING FRAMEWORK"}, 
    ],
    skillImagesTwo:[
                    {img:"/Skill_7.png",title:"REST API"},
                    {img:"/Skill_8.png",title:"POSTGRE SQL"},
                    {img:"/Skill_9.png",title:"REACTJS"},
                    {img:"/Skill_10.png",title:"My SQL"},
                    {img:"/Skill_11.png",title:"CLOUD COMPUTING"},
                    {img:"/Skill_12.png",title:"DEPLOYMENT"}
            
            
            
                  ],
    best:[{title:"100% Placement",img:"https://www.getintech.in/wp-content/uploads/2022/09/assured-placement-150x150.png",des:"Our Quality Placement Team assured to get 100% Placement to our students as a Fresher or Experienced Placement."},
          {title:"Low Cost Budget",img:"https://www.getintech.in/wp-content/uploads/2022/09/cost-150x150.png",des:"Learn Software courses in Low cost with Installment Payment Option. You can get Course and Placement in Reasonable Fees."},
          {title:"World Class Amenities",img:"https://www.getintech.in/wp-content/uploads/2022/09/parking-150x150.png",des:"Our Institution Building has been equipped with Fully Air conditioned, Projector Classrooms and Large Parking Area."}],
    bestTwo:[{title:"Elastic Timing",img:"https://www.getintech.in/wp-content/uploads/2022/09/flexible-timing-150x150.png",des:"Our students can select the flexible time slots for their classroom and Online Sessions. Backup classes also available for missed Sessions."},
          {title:"Mock Interview",img:"https://www.getintech.in/wp-content/uploads/2022/09/mock-interview-150x150.png",des:"Our Mock Interview Sessions boost our students Placement ratio. Our students can attend interviews confidently and Clearly."},
          {title:"Security Features",img:"https://www.getintech.in/wp-content/uploads/2023/08/Security-150x150.png",des:"Our Building fully Equipped with High Resolution CCTV for All classrooms and Entrance Gate. So Feel free about your Children’s Security."}],
    
    projects:[{title:"Beginner",subtitle:"To-Do List App",des:"Build a simple to-do list app using ReactJS for the front-end and Java for the back-end. The app should allow users to create and manage tasks, mark tasks as complete, and delete tasks."},
              {title:"Intermediate",subtitle:"Recipe App",des:"Build a recipe app using ReactJS for the front-end and Java for the back-end. The app should allow users to search for recipes, view recipe details, and save their favorite recipes."},
              {title:"Intermediate",subtitle:"E-commerce Store",des:"Build an e-commerce store using ReactJS for the front-end and Java for the back-end. The store should allow users to browse products, add products to their cart, and checkout."},
              ],
    projectsTwo:[{title:"Advanced",subtitle:"Weather App",des:"Build a weather app using ReactJS for the front-end and Java for the back-end. The app should allow users to enter a location and get the current weather conditions for that location."},
              {title:"Advanced",subtitle:"Expense Tracker",des:"Build an expense tracker app using ReactJS for the front-end and Java for the back-end. The app should allow users to enter their expenses, categorize them, and view reports on their spending."},
              {title:"Advanced",subtitle:"Income Tax Application",des:"Build an income tax application using ReactJS for the front-end and Java for the back-end. The project will also involve choosing an appropriate database, designing an API, and deploying the application to a server."},
            ],
    frontend:["HTML Basics","CSS3","Bootstrap","Javascript","ReactJS","Vue.Js","Express.js","NodeJs"],
    backend:["C Programming","Java","Python","SpringBoot","Git&GitHub","AWS","DevOps","Azure"],
    database:["H2 Database","SQL and MySQL","Postgre","MongoDB"],
    interview:["Mock Interviews","Daily Tests","Spoken English"],
    arrayOne:[{img:"/we_icon1.png",des:"Industry-Based Course Curriculum"},
              {img:"/we_icon2.png",des:"Seven Value Added Courses"},
              {img:"/we_icon3.png",des:"Work Hands-on with 100+ Hours of Internship and 10+ Bootcamps"},
    ],
    arrayTwo:[{img:"/we_icon4.png",des:"Guaranteed Job Interview Calls with our 2000+ partner companies"},
              {img:"/we_icon5.png",des:"Support through WhatsApp, Calls, & Emails"},
              {img:"/we_icon6.png",des:"Lifetime Learning Access"},]
                
                  }
  }
})
</script>
<style>
*{
  box-sizing: border-box;
}
.landing_banner p {
    
    font-size: 18px;
    line-height: 30px;
    padding-left: 10px;
    position: relative;
    opacity: 0.9;
}
.landing_banner p::before {
    content: "";
    background: #4497fe;
    position: absolute;
    left: 0;
    top: 5px;
    width: 3px;
    height: 70%;
}
.mixedcolor{
  background:linear-gradient(90deg,rgb(2, 113, 249),rgb(79, 161, 249),rgb(134, 188, 247),rgb(215, 228, 247),rgb(252, 252, 253) 98.24%)
}
.banner{
  /* background-image: url(https://kvch.in/assets-new/img/banner/full_stack_development_banner.webp); */
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  background-color: #f6f6fa;
}
.container{
  background-image: url(../assets/corporateform_bg_2.jpg);
   background-position: fixed;
  background-size: cover;
  background-repeat: no-repeat;
}
#startnow{
  background-image: url(../assets/banner-img.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
.radiantthemes-separator-block{
  background-color: #2275d5;
  position: relative;
  display: inline-block;
  vertical-align: top;
  overflow: hidden;
}
.radiantthemes-separator-block-gap{
  background-color: #fff;
  position: absolute;
  top: 0;
  bottom: 0;
  width: 20px;
  animation: RadiantThemesSeparatorAnimation 1.5s infinite ease-in-out;
}
@keyframes RadiantThemesSeparatorAnimation {
  0%{
    left: -12px;
  }
  100%{
    left: 100%;
  }
  
}

</style>
