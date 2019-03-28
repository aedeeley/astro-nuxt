<template>
   <div id="main" class="pt-5 mt-5">
        <div class="container">
          <div class="row mt-5 mb-5">
            <div class="col big text-center">
              <h3 class="mb-5" data-aos="zoom-in-up" data-aos-delay="100" data-aos-duration="500">We're easy to talk to</h3>
              <p data-aos="zoom-in-up" data-aos-delay="400" data-aos-duration="500">Ready to start a conversation about your next big idea? Have questions or concerns? Just want to say hi? Just fill out the form below and you'll hear from us soon!</p>
            </div>
          </div>
          <div class="row mb-5">
            <div class="col mt-5 pt-5">
            <form action="https://formspree.io/alex@astroweb.io" method="POST">
        <div class="container mb-5 pb-5">
          <div class="row" data-aos="fade" data-aos-delay="50" data-aos-duration="2000">
            <div class="col-4">
              <h4></h4>
            </div>
            <div class="col-8 mb-3">
              <center>click to select</center>
            </div>
          </div>
          <div class="row split mb-5">
            <div class="col-4" data-aos="fade" data-aos-delay="100" data-aos-duration="2000">
              <h4 class="mt-5 pt-3">Type of work?</h4>
            </div>
            <div class="col-8">
              <input type="checkbox" id="webdev" name="webdev">
              <label for="webdev"><div class="sprite contact-webdev" data-aos="fade" data-aos-delay="300" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="300" data-aos-duration="2000">Website</center></label>

              <input type="checkbox" name="mobileapp" id="mobileapp" />
              <label for="mobileapp"><div class="sprite contact-mobileapp" data-aos="fade" data-aos-delay="200" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="200" data-aos-duration="2000">Mobile App</center></label>

              <input type="checkbox" name="other" id="other" />
              <label for="other"><div class="sprite contact-other" data-aos="fade" data-aos-delay="400" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="400" data-aos-duration="2000">Other</center></label>

            </div>
          </div>
          <div class="row mb-5">
            <div class="col-4">
              <h4 class="mt-5 pt-3">Project details?</h4>
            </div>
            <div class="col-8">
              <input type="checkbox" id="frontend" name="frontend">
              <label for="frontend"><div class="sprite contact-frontend" data-aos="fade" data-aos-delay="500" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="500" data-aos-duration="2000">Frontend</center></label>

              <input type="checkbox" name="backend" id="backend" />
              <label for="backend"><div class="sprite contact-backend" data-aos="fade" data-aos-delay="100" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="100" data-aos-duration="2000">Backend</center></label>

              <input type="checkbox" name="design" id="design" />
              <label for="design"><div class="sprite contact-design" data-aos="fade" data-aos-delay="800" data-aos-duration="2000"></div><center data-aos="fade" data-aos-delay="800" data-aos-duration="2000">Design</center></label>

            </div>
            </div>

            <div class="row mb-5">
            <div class="col-2 pt-5 mt-5">
            </div>
            <div class="col-8">
              <input type="text" id="name" name="name" placeholder="Full Name" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500">
              <input type="text" id="location" name="location" placeholder="Location" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500">
              <input type="text" id="telephone" name="telephone" placeholder="Telephone" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500">
              <input type="text" id="email" name="email" placeholder="Email" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500">
              <textarea type="text" id="message" name="message" placeholder="Message" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500" rows="5" />

                <input type="submit" value="Contact us today" data-aos="fade-up" data-aos-delay="300" data-aos-duration="500">

            </div>
            <div class="col-2">
            </div>
            </div>
        </div>
     </form>
              </div>
            </div>
          </div>
          </div>
</template>

<script>
</script>

<style scoped>
  input[type=checkbox] {
    display:none;
  }

  input[type=checkbox] + label {
    padding:10px 55px;
    cursor:pointer;
    opacity:.3;
  }

  input[type=checkbox] + label:hover {
    opacity:.4;
  }
  input[type=checkbox] + label div {
    clear:both;
    margin:20px auto;
  }

  input[type=checkbox]:checked + label {
    opacity:1.0;
}

input[type=text],textarea {
  width:100%;
  margin-bottom:12px;
  border:1px solid #E8E8E8;
  padding:12px 0;
  text-indent:24px;
  border-radius:4px;
}

input[type=text]::placeholder, textarea::placeholder {
  color:#C7C7CA;
}

input[type=submit] {
  width:100%;
  background-color:#7E57C2;
  border:1px solid #7E57C2;
  padding:12px 0;
  text-indent:24px;
  border-radius:4px;
  color:#fff;
  font-weight:bold;
}
</style>
