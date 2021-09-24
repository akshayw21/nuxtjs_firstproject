<template>
  <div>
    <h1>Happy customers around the world.</h1>
    <p>
      At Enside, you’ll make world-class work with a<br />
      friendly and talented team.
    </p>

    <h1>Let's talk about how Enside can help you</h1>
    <p>
      Hire us now -we are here to assist you. Drop us a line,<br />
      and we will answer on all your questions.
    </p>

    <form>
      <div class="mb-3">
        <label for="exampleInputEmail1" class="form-label">Name</label>
        <input
          id="exampleInputEmail1"
          type="email"
          class="form-control"
          aria-describedby="emailHelp" required
        />
      </div>
      <div class="mb-3">
        <label for="exampleInputPassword1" class="form-label">Email</label>
        <input
          id="exampleInputPassword1"
          type="password"
          class="form-control" required
        />
      </div>
      <div class="form-floating">
        <textarea
        id="floatingTextarea2"
          class="form-control"
          placeholder="Leave a comment here" required
          
          style="height: 100px"
        ></textarea>
        <label for="floatingTextarea2">Message</label>
      </div>
      
      <div class="d-grid gap-2">
  <button class="btn btn-dark text-white pb-2 ma-3 fs-2" type="button"><b>submit</b></button>
  
</div>
    </form>
  </div>
</template>

<style scoped>
h1 {
  margin-top: 1%;
  text-align: center;
}
p {
  margin-top: 1%;
  text-align: center;
  font-size: 20px;
}
</style>
