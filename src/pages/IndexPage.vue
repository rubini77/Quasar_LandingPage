<template>
  <q-page>
    <div class="banner q-pb-md">
        <div class="row justify-center">
        <div class="col-12 col-md q-pa-md text-white">
        <div style="max-width: 650px;" class="q-ml-auto q-mr-auto">
        <h3 class="text-weight-bolder q-mt-xl q-pt-sm">FullStack Developer Training &amp; Placement</h3>
        <div class="mixedcolor q-pa-sm text-weight-bolder text-blue-10">100% Job Guarantee</div>
        <div class="landing_banner">
          <p class="text-weight-bold q-pt-sm">Ranked #1 Full Stack Training Institute with Placement</p>
        </div>
        <div>
          <p class="text-weight-medium ">Edex IT Solutions provides the Best Full Stack Training in Chennai, Bangalore &amp; Online with 100% placements. Learn Full Stack Course from Basics to Advanced and get real-time experience.</p>
        </div>
        <div class="text-weight-medium">
          <div><q-icon name="check" class="q-pa-sm"></q-icon><span>Enroll Now for Trending Courses with Job Assurance</span></div>
          <div><q-icon name="check" class="q-pa-sm"></q-icon><span>5+ Years Experinced Mentors</span></div>
          <div><q-icon name="check" class="q-pa-sm"></q-icon><span>4+ Branches in Tamilnadu</span></div>
        </div>
        <div class="row q-pt-md">
          <div clas="col-5"><q-btn class="bg-red-13 text-white text-weight-bold">Download Brouchure</q-btn></div>
          <div class="col-6 text-weight-bolder q-pa-sm">*Available for Both <span class="text-yellow-8"> Online& Classroom</span></div>
        </div>
       </div>
      </div>

      <div class="col-12 col-md gt-sm">
        <div style="max-width: 550px;" class="q-ml-auto q-mr-auto">
          <div class="q-mt-xl q-pt-xl">
            <div class="q-pa-md scroll shadow-up-9 " style="height: 400px;border-radius: 20px;background-color: white;">
              <div>
                <div class="text-weight-bold">Course Path :</div>
                <ul>
                  <li class="q-py-xs">Front End Development with HTML, CSS, and Javascript</li>
                  <li class="q-py-xs">Backend Development with Core Java</li>
                  <li class="q-py-xs">Web Services with Spring and Spring Boot</li>
                  <li class="q-py-xs">SQL and Databases</li>
                </ul>
                <div class="text-weight-bold">Valur-Added Courses :</div>
                <ul>
                  <li class="q-py-xs">API creation using ExpressJS and MongoDB</li>
                  <li class="q-py-xs">CSS Preprocessor (Intermediate + Advanced)</li>
                  <li class="q-py-xs">UI/UX Fundamentals</li>
                  <li class="q-py-xs">Responsive Web Design Frameworks using Material UI</li>
                  <li  class="q-py-xs" >DevSecOps Tools Overview</li>
                  <li  class="q-py-xs" >Application Deployment on Cloud</li>
                </ul>
              </div>
              <p class="row">
                <img src="/completion-01.png"><span class="q-mt-xs q-pa-xs text-weight-bolder">Course Completion Certificate</span></p>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
  <div class="lt-md justify-center">
        <div style="max-width: 550px;" class="q-ml-auto q-mr-auto">
          <div class="">
            <div class="q-pa-md shadow-up-9 " style="height:;background-color: white;">
              <div>
                <div class="text-weight-bold">Course Path :</div>
                <ul>
                  <li class="q-py-xs">Front End Development with HTML, CSS, and Javascript</li>
                  <li class="q-py-xs">Backend Development with Core Java</li>
                  <li class="q-py-xs">Web Services with Spring and Spring Boot</li>
                  <li class="q-py-xs">SQL and Databases</li>
                </ul>
                <div class="text-weight-bold">Valur-Added Courses :</div>
                <ul>
                  <li class="q-py-xs">API creation using ExpressJS and MongoDB</li>
                  <li class="q-py-xs">CSS Preprocessor (Intermediate + Advanced)</li>
                  <li class="q-py-xs">UI/UX Fundamentals</li>
                  <li class="q-py-xs">Responsive Web Design Frameworks using Material UI</li>
                  <li  class="q-py-xs" >DevSecOps Tools Overview</li>
                  <li  class="q-py-xs" >Application Deployment on Cloud</li>
                </ul>
              </div>
              <p class="row">
                <img src="/completion-01.png"><span class="q-mt-xs q-pa-xs text-weight-bolder">Course Completion Certificate</span></p>

            </div>
          </div>
        </div>
      </div>

<div class="bg-blue-9 q-pa-md">
  <div class="text-center">
    <div class="row q-gutter">
      <div class="col-12 col-md col-sm-4 q-pa-sm align-center" v-for="img in images">
      <img :src="img">
      </div>
    </div>
  </div>
</div>

<!-- program highlights -->
<div class="bg-blue-grey-1 q-pb-lg">
  <div class="q-pa-md text-center">
      <div class="row q-px-xl q-pt-lg text-h5 text-weight-bold">Program Highlights</div>

      <div class="text-center">
      <div class="row q-pa-md q-gutter-sm">
         <q-card class="my-card col-12 col-sm-12 col-md align-center" v-for="x in cardItems">
          <div class="text-center bg-blue-grey-1"><img :src="x.img" class="img-fluid"></div>
              <q-card-section>
                <div class="text-h6">{{ x.name }}</div>
                <div class="">{{ x.des }}</div>
              </q-card-section>
    </q-card>
    </div> 
  </div>

  </div>
</div>

</q-page>

<q-page>
  <div class="row">
    <div class="col text-center">
    <q-parallax :height="500" :speed="1.5">
      <template v-slot:media>
        <img src="/besanttechnologies-career.webp" style="background: #0e2f53 none repeat scroll 0 0;opacity: 0.6;">
      </template>
     <div class="q-pa-sm">
      <h4 class="text-black text-weight-bold">Want to pursue the Best Full Stack Training with Edex Technologies?</h4>
      <p class="text-h6 text-weight-bold" style="color: rgb(31, 31, 31);">Edex Tech Full Stack Developer Course is all about your growth as a developer.
         Our hands on training will make you a jack of all trades, which is the current demand in the market of developers.</p>
         <q-btn class="bg-deep-orange-14 text-white">Get Started</q-btn>
        </div>
    </q-parallax>
  </div>
  </div>

<div class="bg-blue-9 q-pa-lg">  
<div class="q-pa-md">
  <div class="row q-px-lg q-pt-lg q-pb-lg justify-center  text-h5 text-weight-bold text-white">Recommened Combo Courses</div>

  <div>
    <div class="row q-pa-sm q-gutter-sm">
      <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in comboCourses">
          <div class="bg-blue-grey-1 q-pa-sm">
            <div class="row q-gutter-sm">
            <div class="col-3 q-pa-sm"><img :src="x.img" style="height: 50px;width: 60px;"></div>
            <div class="col q-pt-lg text-weight-bold"><span>{{ x.h3 }}</span>
            <span><img src=""></span></div>
            </div>
          </div>
              <q-card-section class="text-center">
                <div class="row q-pa-md">
                  <div class="col" style="border-right: 1px solid rgb(141, 140, 140);">
                    <div class="text-blue-grey-9 text-weight-bold">Skill Level</div>
                    <div class="text-blue-grey-7">Beginner</div>
                  </div>
                  <div class="col" style="border-right: 1px solid rgb(141, 140, 140);">
                    <div class="text-blue-grey-9 text-weight-bold">Hours</div>
                    <div class="text-blue-grey-7">30</div>
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
      <div><q-btn class="bg-deep-orange-14 text-white">Enroll Now</q-btn></div>
    </div>
  </div>
</div>
</div>
</div>

  

</q-page>
<q-page class="">
<!-- tools covered -->
<div class="text-center">
  <div class="row q-px-xl q-pt-lg text-h5 text-weight-bold q-pa-lg">Tools Covered</div>
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

<!-- skills covered -->
<div class="text-center bg-blue-grey-1">
  <div class="row q-px-xl q-pt-lg text-h5 text-weight-bold q-pa-lg">Skills Covered</div>
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

</q-page>
<q-page>
  <div class="q-pa-lg q-mx-md">
    <div class="q-pa-md">
      <div class="row  q-pt-sm q-pb-sm  text-h5 text-weight-bold">Projects Milestones</div>
        <div class="q-pa-lg">
          <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in projects">
              <div class="bg-blue-9 q-pa-md">
                <div class="text-weight-bold q-pa-sm text-h6 text-white">{{ x.title }}</div>
              </div>
              <q-card-section class="q-pa-lg">
                <div class="text-weight-bold q-pa-sm">{{ x.subtitle }}</div>
                <div class="text-blue-grey-9">{{ x.des }}</div>
              </q-card-section>
            </q-card>
          </div>
          <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in projectsTwo">
              <div class="bg-blue-9 q-pa-md">
                <div class="text-weight-bold q-pa-sm text-h6 text-white">{{ x.title }}</div>
              </div>
              <q-card-section class="q-pa-lg">
                <div class="text-weight-bold q-pa-sm">{{ x.subtitle }}</div>
                <div class="text-blue-grey-9">{{ x.des }}</div>
              </q-card-section>
            </q-card>
          </div>
        </div>
    </div>
  </div>

  <!-- why edex -->
  <div class="q-pa-lg bg-blue-grey-1">
    <div class="q-pa-md">
      <div class="row  q-pt-sm q-pb-sm  text-h5 text-weight-bold">Why Edex</div>
      <div class="q-pa-lg">
        <div class="row q-pa-sm q-gutter-md">
          <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in arrayOne">
             <div class="row q-pa-sm">
              <div class="col-4"><img :src="x.img" style="height: 70px;width: 90px;"> </div>
              <div class="col q-px-md" style="display: flex;flex-direction: column;justify-content: center;align-items: center;">{{ x.des }}</div>
             </div>
            </q-card>
        </div>
        <div class="row q-pa-sm q-gutter-md">
            <q-card class="my-card col-12 col-sm-12 col-md" v-for="x in arrayTwo">
              <div class="row q-pa-sm">
                <div class="col-4"><img :src="x.img" style="height: 70px;width: 90px;"> </div>
                <div class="col q-px-md text-center" style="display: flex;flex-direction: column;justify-content: center;align-items: center;">{{ x.des }}</div>
             </div>
            </q-card>
          </div>
      </div>
    </div>
  </div>


  <div class="q-pa-md bg-blue-8">
    <div class="row q-px-xl q-pt-md text-white justify-center text-h5 text-weight-bold">Learning Path</div>
    
   
    <div class=" q-ma-lg q-pa-md" style="display: flex;justify-content: center;align-items: center;flex-direction: column;">
    <q-stepper
      v-model="step"
      header-nav
      color="primary"
      animated
      style="max-width: 990px ;"
      
    >
      <q-step
        :name="1"
        title="MILESTONE 1"
        icon="check"
        :done="done1"
        
        
      >
      <div class="text-weight-medium">Frontend Tools and Technologies :</div>
              
              <ul v-for="x in frontend" type="none">
                <li><q-icon name="star" color="blue-9" style="font-size: 20px;" class="q-px-sm"></q-icon> {{ x }}</li>
              </ul> 
              
      <div><q-btn class="bg-deep-orange-9 text-white q-pa-sm">Download Curriculum</q-btn></div>
         
      </q-step>

      <q-step
        :name="2"
        title="MILESTONE 2"
        caption=""
        icon="check"
        :done="done2"
        
        
      >
      <div class="text-weight-medium">Backend Tools and Technologies :</div>
              
              <ul v-for="x in backend" type="none">
                <li><q-icon name="star" color="blue-9" style="font-size: 20px;"  class="q-px-sm"></q-icon> {{ x }}</li>
              </ul> 
              
      <div><q-btn class="bg-deep-orange-9 text-white q-pa-sm">Download Curriculum</q-btn></div>
         
      </q-step>

      <q-step
        :name="3"
        title="MILESTONE 3"
        icon="check"
        
        
      
      >
      <div class="text-weight-medium">Database:</div>
              
              <ul v-for="x in database" type="none">
                <li><q-icon name="star" color="blue-9" style="font-size: 20px;"  class="q-px-sm"></q-icon> {{ x }}</li>
              </ul> 
              <div class="text-weight-medium">Interview Preparations:</div>
              
              <ul v-for="x in interview" type="none">
                <li><q-icon name="star" color="blue-9" style="font-size: 20px;"  class="q-px-sm"></q-icon> {{ x }}</li>
              </ul> 
              
      <div><q-btn class="bg-deep-orange-9 text-white q-pa-sm">Download Curriculum</q-btn></div>
         
      </q-step>
    </q-stepper>
  </div>
<!-- </div> -->

  </div>

    <div class="container" style="display: flex;flex-direction: column;justify-content: center;align-items: center;">
      <div class="box q-pa-md">
        <div class="row q-pa-md">
            <q-card class="col" style="border-radius: 5px;">
              <div class="bg-blue-grey-2 text-black q-pa-md">
                <div class="text-weight-bold q-pa-sm text-h6">Live Virtual Classroom</div>
              </div>
              <q-card-section class="q-pa-md">
                <ul class="q-pl-xl" >
                  <li class="q-py-md text-weight-medium">Guaranteed job interviews until you get placed</li>
                  <li class="q-py-md text-weight-medium">Intensive interview preparation from Day 1</li>
                  <li class="q-py-md text-weight-medium">Real-life interview case study analysis</li>
                </ul>
                <div class="q-pa-sm text-h6 text-weight-bold"><b>For more details consult our career counselors</b></div>
                <div class="text-center q-pa-sm"><q-btn class="bg-deep-orange-14 text-white">Enroll Now</q-btn></div>
              </q-card-section>
            </q-card>
          </div>

      </div>
    </div>


<div class="bg-blue-9 q-pb-lg">
  <div class="text-center">
    <div style="display: flex; flex-direction: column;justify-content: center;align-items: center;">
    <div class="text-weight-bold text-h5 text-white q-pa-lg ">
      Do you want to know how the Full Stack Development<br>
      Course will be an excellent fit for your career?
    </div>
    <div class="" >
      <q-card class="col" style="border-radius: 5px;min-width: 320px;">
          <div class="bg-blue-grey-2 text-black q-pa-md">
          <div class="text-weight-bold text-h6">Request a Call Now</div>
      </div>
    <q-card-section>
      <q-form
       @submit="onSubmit"
       @reset="onReset"
       class="q-gutter-md bg-white q-pa-md"
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
    type="number"
    v-model="mobile"
    label="Your mobile *"
    hint="Enter your mobile number"
    lazy-rules
    :rules="[ val => val && val.length == 10 || 'Please Enter Your Mobile Number']"
  />

  <q-toggle v-model="accept" label="I accept the license and terms" />

  <div>
    <q-btn label="Submit" type="submit" color="primary"/>
    <q-btn label="Reset" type="reset" color="primary" flat class="q-ml-sm" />
  </div>
</q-form>
</q-card-section>
</q-card>

</div>
  </div>
  </div>
</div>

<!-- place QPageScroller at end of page -->
<q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
    <q-btn fab icon="keyboard_arrow_up" color="red" />
</q-page-scroller>

<div class="bg-black q-pa-sm text-center">
  <div class="text-white q-pa-sm">Copyright 2023 Edex | All Rights Resrved</div>
</div>
</q-page>
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
                            h3:"HTML+CSS+JS",p:"5.0(1965)",c3:"2360"},
                    {img:"/combo_course_2.jpg",h3:"ANGULAR & REACT",p:"5.0(1865)",c3:"1989"},
                    {img:"/combo_course_3.jpg",h3:"PYTHON & JAVA+SQL",p:"5.0(1970)",c3:"2051"}]
      
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
    background: #cfe5ff;
    position: absolute;
    left: 0;
    top: 5px;
    width: 2px;
    height: 70%;
}
.mixedcolor{
  background:linear-gradient(90deg,rgb(255, 255, 255),rgb(172, 171, 171),rgb(114, 113, 113),rgb(37,37,37),black 98.24%)
}
.banner{
  background-image: url(../assets/Banner.jpg);
}
.container{
  background-image: url(../assets/corporateform_bg_2.jpg);
   background-position: fixed;
  background-size: cover;
  background-repeat: no-repeat;
}

</style>
