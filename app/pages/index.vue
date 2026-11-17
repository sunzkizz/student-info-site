<!-- Home page: uses InfoCard and AppButton -->
<template>
  <section>
    <h1>Welcome Golden Paddlers!</h1>
    <p>Caraga State University primarily provides advanced education, higher technological, 
        professional instruction, and training in agriculture, environmental studies, fishery, 
        engineering, forestry, industrial technology, education, law, medicine and health-related 
        programs, information technology, arts and sciences, and related courses. It also conducts 
        research, extension services, and progressive leadership in its specialized fields.</p>

    <div class="grid">
      <InfoCard
        title="Mission"
        description="As a transformative university, CSU is a responsible steward of problem-solvers and value creators who are driven to create a sustainable future for the region, the nation, and beyond."
      />
      <InfoCard
        title="Vision"
        description="A socially-engaged digital, innovation, and entrepreneurial university excelling globally in science, engineering, and the arts by 2028."
      />
      <InfoCard
        title="Core Values"
        description="Competence.Service.Uprightness."
      />
    </div>

    <div class="actions">
      <AppButton label="View Students" color="blue" to="/students" />
      <AppButton label="About This Site" color="green" to="/about" />
    </div>
  </section>
</template>

<style scoped>
.actions { margin-top: 24px; display: flex; gap: 12px; }
</style>
