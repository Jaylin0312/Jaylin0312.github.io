<template>
  <div id="bg" class="p-4">
    <nav class="navbar navbar-light">
      <a class="navbar-brand"><img class="logo" src="../assets/logo.png" /></a>
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#"
            >Home <span class="sr-only">(current)</span></a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#education">Education</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#timetable">Cry</a>
        </li>
      </ul>
    </nav>
    <div class="container text-center">
      <div class="typed-out">Hello there!</div>
    </div>
    <div class="section-about">
      <div
        class="prodile_card d-flex flex-column justify-content-center align-items-center"
      >
        <div class="profile">
          <img
            class="rounded-circle"
            src="../assets/myProfile.jpg"
            width="100%"
            height="100%"
          />
        </div>
        <div class="card info_card shadow p-3 mb-5 bg-white rounded">
          <div>
            I am Jie Ling. I am a sophomore in SMU studying Information System.
            I love meeting new people, having new friends, and gaining new
            experience.
          </div>
        </div>
      </div>
    </div>
    <div id="education" class="edu text-center mt-5">My Education Journey</div>
    <div class="text-center mb-5">I swear I am not depressed 🥹</div>
    <div class="row mb-3 d-flex justify-content-center">
      <div class="card mb-2 shadow p-3 mb-5 bg-white rounded">
        <div class="row p-3">
          <div class="col-6 p-3">
            <p>Singapore Management University</p>
            <ul>
              <li>Bachelor of Science (Information Systems)</li>
              <li>GPA is a secret</li>
            </ul>
          </div>
          <div class="col-6 p-3 text-right">Aug 2021 to Aug 2025</div>
        </div>
      </div>
      <div class="card mb-2 shadow p-3 mb-5 bg-white rounded">
        <div class="row p-3">
          <div class="col-6 p-3">
            <p>Sunway College Johor Bahru</p>
            <ul>
              <li>Cambridge GCE A-level</li>
              <li>Again result is a secret</li>
            </ul>
          </div>
          <div class="col-6 p-3 text-right">Apr 2019 to Jun 2020</div>
        </div>
      </div>
    </div>
    <div id="education" class="edu text-center mt-5">My Not-so-fun Stuff</div>
    <div class="text-center mb-5">I am actually depressed 🥹</div>
    <table id="timetable" class="table table-striped mx-auto">
      <thead class="thead-dark">
        <tr>
          <th scope="col">Time</th>
          <th scope="col">Course Name</th>
          <th scope="col">Difficulty</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td scope="row">3.30 pm to 6.45 pm</td>
          <td>BPAS</td>
          <td>Confusing</td>
        </tr>
        <tr>
          <td scope="row">12.00 pm to 3.30 pm</td>
          <td>WAD</td>
          <td>It is manageable</td>
        </tr>
        <tr>
          <td scope="row">3.30 pm to 6.45 pm</td>
          <td>IDP</td>
          <td>Ruin Frienship</td>
        </tr>
        <tr>
          <td scope="row">12.00 pm to 3.30 pm</td>
          <td>BGS</td>
          <td>Even more confusing</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style>
#bg {
  background-image: url(../assets/bg.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
}
.container {
  width: 200px;
  margin-bottom: 120px;
}
.logo {
  max-width: 50px;
}
.typed-out {
  overflow: hidden;
  border-right: 0.15em solid rgb(143, 196, 215);
  white-space: nowrap;
  font-size: 1.6rem;
  width: 0;
  animation: typing 2s steps(20, end) forwards, blink 0.8s infinite;
}
@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}
@keyframes blink {
  from {
    border-color: transparent;
  }
  to {
    border-color: rgb(243, 182, 226);
  }
}
.navbar-nav {
  flex-direction: row !important;
}
.nav-link {
  margin-right: 20px;
}
.profile_card {
  position: relative;
}
.profile {
  position: absolute;
  top: 180px;
  z-index: 2;
}
.info_card {
  padding: 100px !important;
  border: none !important;
  text-align: center;
  width: 80% !important;
}
.edu {
  font-size: 1.6rem;
}
.card,
.table {
  width: 80%;
}

@media screen and (max-width: 425px) {
  .profile {
    width: 100px;
  }
  .info_card {
    padding: 40px !important;
  }
}
</style>

<script>
export default {
  name: "IndexPage",
};
</script>
