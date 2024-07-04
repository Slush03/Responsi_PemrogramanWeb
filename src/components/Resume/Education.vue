<script>
export default {
  data(){return{
    educations: [
      {
        year: "2019 - 2022",
        school: "Muhammadiyah Batam",
        location: "Batam",
        field: "TKJ",
        description: [
         "In TKJ, I get to learn all about the basics of networking, including how to use a mikrotik and some basic computer science."
        ]
      },
      {
        year: "2022 - Present",
        school: "Amikom Yogyakarta",
        location: "Yogyakrta",
        field: "Informatics",
        description: [
          "In the Informatics Study Program I learned a lot about the basics of Programming and continued up to Advance Programming.",
          "My IPK is still 3.85.",
        ]
      }
    ]
  }}
}
</script>

<template>
  <section>
    <h2 class="text-secondary fw-bolder mb-4">Education</h2>

    <div v-for="education of educations" class="card shadow border-0 rounded-4 mb-5">
      <div class="card-body px-3 px-md-5 py-5">
        <div class="row align-items-center gx-5">
          <div class="col text-center text-lg-start mb-4 mb-lg-0">
            <div class="p-4 rounded-4">
              <div class="text-secondary fw-bolder mb-2">{{education.year}}</div>
              <div class="mb-2">
                <div class="small fw-bolder">{{education.univ}}</div>
                <div class="small text-muted">{{education.location}}</div>
              </div>
              <div class="fst-italic">
                <div class="small text-muted">{{education.degree}}</div>
                <div class="small text-muted">{{education.field}}</div>
              </div>
            </div>
          </div>
          <div class="col-lg-8">
            <div>
              <ul class="mb-0">
                <li v-for="desc of education.description">
                  {{desc}}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>