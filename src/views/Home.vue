<template>
  <v-container class="home mt-n3 white--text">
    <v-row class="mx-auto" no-gutters>
      <v-col class="d-flex flex-column d-sm-none blue-grey darken-3" cols="3">
        <v-img
          src="http://placekitten.com/200/200"
          aspect-ratio="1"
          max-width="100%"
        />
      </v-col>
      <v-col class="blue-grey darken-3" cols="9" sm="3">
        <v-img
          class="d-none d-sm-block"
          src="http://placekitten.com/300/400"
          aspect-ratio="1"
          width="100%"
        />
        <v-list-item>
          <div class="display-1 py-4 white--text font-weight-bold">
            Ahmad Al&#8209;Sharif
          </div>
        </v-list-item>
        <v-list-item class="d-flex">
          <div class="headline pb-4 white--text">
            Software Engineer
          </div>
        </v-list-item>
        <v-divider class="primary darken-2 mx-4" />
        <v-list-item>
          <v-list-item-icon>
            <v-icon large color="primary">mdi-account-circle-outline</v-icon>
          </v-list-item-icon>
          <v-list-item-title class="white--text">About</v-list-item-title>
        </v-list-item>
        <v-list-item class="white--text">
          I am an enthusiastic software developer that is craving to learn new
          technologies and get into various experiences. So far I’ve collected
          over 20 technologies and whatever the job requires I always seek to
          adapt. I prefer working in a team as I believe working in a team
          enhances my productivity and perhaps I would provide higher value to
          the team.
        </v-list-item>

        <v-divider class="primary darken-2 mx-4 my-2" />

        <v-list-item class="white--text">
          <div class="d-flex flex-column">
            <div class="headline white--text my-3">
              Skills
            </div>
            <ul>
              <li>Vue.js</li>
              <li>Golang</li>
              <li>HTML, CSS</li>
              <li>JavaScript ES6</li>
              <li>MySQL</li>
              <li>MongoDB</li>
              <li>Firebase</li>
              <li>Java</li>
              <li>Kotlin</li>
              <li>Docker</li>
              <li>Linux</li>
            </ul>
          </div>
        </v-list-item>
        <v-list-item> </v-list-item>
      </v-col>

      <v-col class="ps-3" cols="12" sm="9">
        <v-list class="primary darken-1 mt-3">
          <v-list-item
            id="#work-experience"
            class="text-uppercase headline font-weight-bold"
          >
            Work Experience
          </v-list-item>
          <WorkExperienceCard
            class="mb-2"
            from="Mar 2020"
            to="PRESENT"
            title="Software Development Mentor"
            work-place="<a href='https://reach-academy.net/' target='_blank'>Reach Academy (Remote)</a>"
            :experiences="[
              `Developed and lead the following practical programs with <b>100+ members</b>`,
              `<b>Practical</b> software development and engineering`,
              `<b>Vue.js</b> advanced development`,
              `<b>Machine Learning with Tensorflow</b>`
            ]"
          />
          <WorkExperienceCard
            class="mb-2"
            from="Aug 2018"
            to="Mar 2020"
            title="Software Engineer"
            work-place="Kidzie International (Remote)"
            :experiences="[
              `Engineered and developed a multi-website e-commerce solution from
               scratch in <b>GoLang, Vue.js, MongoDB, and Docker<b/>`,
              '<b>Lead a team</b> of 10+ developers, testers, and UI/UX designers',
              'Developed complex backends and frontends based on <b>client requirements and meetings<b/>'
            ]"
          />
          <WorkExperienceCard
            class="mb-2"
            from="2017"
            to="2019"
            title="Software Developer"
            work-place="<a href='https://switchtech.com/' target='_blank'>Switch Technology (Remote)</a>"
            :experiences="[
              `Software development on government level encryption solutions`,
              'Web development in PHP, Phalcon, Vue.js',
              'DevOps and server maintenance with Intel servers and Raspberry'
            ]"
          />
          <WorkExperienceCard
            class="mb-2"
            from="2016"
            to="2017"
            title="Mobile/Web Developer"
            work-place="<a href='https://www.playmyway.com/' target='_blank'>Play.My.Way</a>"
            :experiences="[
              'Android app development',
              'Web development in PHP',
              'Tracking Android app crashes and bugs with <b>Crashlytics</b>'
            ]"
          />
          <WorkExperienceCard
            class="mb-2"
            from="2011"
            to="2016"
            title="Android Developer"
            work-place="Freelance"
            :experiences="[
              'Independent development',
              'Application got featured on XDA-Developers',
              'Received 30,000+ downloads and some donations'
            ]"
          />
        </v-list>

        <v-list class="primary darken-1 mt-3">
          <v-list-item
            id="#education"
            class="text-uppercase headline font-weight-bold"
          >
            Education
          </v-list-item>
          <ul class="text-h5 ms-6">
            <li>Bachelor's in Computer Sciences</li>
          </ul>
        </v-list>

        <v-list class="primary darken-1 mt-3">
          <v-list-item
            id="#hobbies"
            class="text-uppercase headline font-weight-bold"
          >
            Hobbies
          </v-list-item>
          <ul class="text-h5 ms-6">
            <li>Independent software development for communities</li>
            <li>Competitive Gaming</li>
            <li>Streaming</li>
          </ul>
        </v-list>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import WorkExperienceCard from "@/components/WorkExperienceCard";

export default {
  name: "Home",
  components: { WorkExperienceCard },
  data() {
    return {};
  }
};
</script>
