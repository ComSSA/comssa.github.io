<template>
  <b-container fluid>
    <b-row>
      <b-col class="mt-3">
        <h1>About</h1>
        <p>
          ComSSA has been a second family to many computing students and enthusiasts alike, being the biggest Computing orientated
          club at Curtin. <br><br>

          Our aim as a club is to:
          <ul>
            <li>Foster a thriving community of future and active computing professionals and programming enthusiasts.</li>
            <li>Provide a place for students and members with similar interests to study, connect, and enjoy university life.</li>
            <li>
              Provide computing students and our members with opportunities and resources to further their professional development.
              Some of these opportunities include networking with industry professionals and running workshops that expose students to
              industry-relevant technology.
            </li>
          </ul> <br>

          Our <a href="/constitution.pdf">constitution</a> outlines the rules by which ComSSA runs. The ComSSA committee is made up of executive committee members and ordinary committee members.<br><br>
          <!--
          Catch up on previous meetings by reading the meeting minutes
          <NuxtLink to="/minutes">
            here.
          </NuxtLink>
          -->
        </p>
      </b-col>
      <b-col md="auto" class="mt-5" style="width: 500px;">
        <v-lazy-image
          class="mb-5 rounded-corner"
          width="500"
          :src="'https://res.cloudinary.com/dec6mijn3/image/upload/c_scale,w_1000/v1693068628/ComSSA-Website/General/about_2024'"
          :src-placeholder="'https://res.cloudinary.com/dec6mijn3/image/upload/c_scale,w_200/v1693068628/ComSSA-Website/General/about_2024'"
        />
      </b-col>
    </b-row>
    <h2>
      Committee Members
    </h2>
    <h3 class="exec-subheading">
      Executive Committee Members
    </h3>
    <b-row align-h="around" class="mt-3 mb-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Sophie Melville"
          title="President"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Sean McGinty"
          title="Vice President"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Stanley Zhong"
          title="Treasurer"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Cindy Lawrence"
          title="Secretary"
        />
      </b-col>
    </b-row>
    <h3 class="ord-subheading">
      Ordinary Committee Members
    </h3>
    <b-row align-h="around" class="mt-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Khidir Azhar"
          title="Events Coordinator"
        />
      </b-col><b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Ethan Olson"
          title="Marketing Coordinator"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Justis Koh"
          title="Technical Coordinator"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Joleen Chong"
          title="Revision Session Coordinator"
        />
      </b-col>
    </b-row>
    <b-row align-h="around" class="mt-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Alice Arvidson"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Henry Truong"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Jimmy Yang"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Kai Chen Chai"
        />
      </b-col>
    </b-row>
    <b-row align-h="around" class="mt-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Laura Jiang"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Mia Tran"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Nathaniel White"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Nikki Doan"
        />
      </b-col>
    </b-row>
    <b-row align-h="around" class="mt-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Peter Dang"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Raphael Ho"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Tri Dao"
        />
      </b-col>
    </b-row>
    <h3 class="ord-subheading">
      Sub-Committee Members
      <!--Added extra row to balance subs better-->
    </h3>
    <b-row align-h="around" class="mt-3 text-center">
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Daniela Degasperi"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Hua Chen"
        />
      </b-col>
      <b-col cols="6" md="3" class="mb-3">
        <CloudProfile
          name="Patrick Jong"
        />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
    head: {
        title: "About"
    }
}
</script>
