<template>
  <section class="page-detail">
    <div class="job-detail">
      <div class="sidebar-top">
        <div>
          <p>Jobs at NuxtBoard</p>
        </div>
        <div href="#job-form" class="apply-btn">
          <p>Apply Now</p>
        </div>
      </div>
      <div class="sidebar-item">
        <p class="sidebar-item-title">Location</p>
        <p class="sidebar-item-data">Lausanne, Switzerland</p>
      </div>
      <div class="sidebar-item">
        <p class="sidebar-item-title">Salary</p>
        <p class="sidebar-item-data">CHF55000 - CHF85000 /year</p>
      </div>
      <div class="sidebar-item">
        <p class="sidebar-item-title">Job Type</p>
        <p class="sidebar-item-data">Full-time</p>
      </div>
      <div class="sidebar-item">
        <p class="sidebar-item-title">Date Posted</p>
        <p class="sidebar-item-data">July 27th, 2023</p>
      </div>
    </div>
    <div class="job-description">


      <div class="job-form">
        <form>
          <div class="job-form-names">
            <div class="job-form-firstname">
              <label for="f_name">First Name <span style="color: rgb(140, 196, 46);">*</span></label>
              <input type="text" name="f_name" maxlength="32" required="">
            </div>
            <div class="job-form-lastname">
              <div><label for="l_name">Last Name
                  <span style="color: rgb(140, 196, 46);">*</span></label><input type="text" name="l_name" maxlength="32"
                  required>
              </div>
            </div>
          </div>

          <div class="job-form-contact">
            <div class="job-form-email"><label for="email">Email Address <span
                  style="color: rgb(140, 196, 46);">*</span></label><input type="email" name="email" maxlength="64"
                required>
            </div>
            <div class="job-form-phone"><label for="email">Phone</label><input type="text" name="phone" maxlength="16">
            </div>
          </div>

          <div class="job-form-links">
            <div class="job-form-github">
              <div><label for="github">Github/Linkedin<span style="color: rgb(140, 196, 46);">*</span></label>
                <input type="text" name="github" maxlength="32" required>
              </div>
            </div>
          </div>

          <div class="job-form-letter">
            <div><label for="cover_letter">Cover
                Letter<span style="color: rgb(140, 196, 46);">*</span></label>
              <textarea cols="23" required name="cover_letter"></textarea>
            </div>
          </div>

          <div class="job-upload">

            <div><label>CV / Resume <span style="color: rgb(140, 196, 46);">*</span></label><input id="attach" type="file"
                style="display: none;" accept=".pdf,.doc,.docx,.rtf,.jpg,.jpeg"><label for="attach"
                class="job-upload-label"><svg class="svg-inline--fa fa-upload" aria-hidden="true" focusable="false"
                  data-prefix="fad" data-icon="upload" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                  data-fa-i2svg="">
                  <g class="fa-duotone-group">
                    <path class="fa-secondary" fill="currentColor"
                      d="M288 352v32c0 17.7-14.3 32-32 32s-32-14.3-32-32V352H64c-35.3 0-64 28.7-64 64v32c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V416c0-35.3-28.7-64-64-64H288zm120 80a24 24 0 1 1 48 0 24 24 0 1 1 -48 0z">
                    </path>
                    <path class="fa-primary" fill="currentColor"
                      d="M256 416c17.7 0 32-14.3 32-32V109.3l73.4 73.4c12.5 12.5 32.8 12.5 45.3 0s12.5-32.8 0-45.3l-128-128c-12.5-12.5-32.8-12.5-45.3 0l-128 128c-12.5 12.5-12.5 32.8 0 45.3s32.8 12.5 45.3 0L224 109.3V384c0 17.7 14.3 32 32 32z">
                    </path>
                  </g>
                </svg>Attach CV/Resume</label>
              <div class="job-upload-tip">
                <p><strong>Tip: </strong>Allowed file types; pdf, doc, docx,
                  rtf, jpg, jpeg. No larger than 10mb.</p>
              </div>

              <div class="job-sumbit">
                <div class="job-submit-inner">
                  <div class="job-submit-powered">
                    <a target="_blank" href="https:/thebcms.com">Powered by THEBCMS</a>
                  </div>

                  <div class="job-submit-btn" style="background-color: rgb(140, 196, 46);">
                    <p>Submit</p>
                  </div>

                </div>
              </div>
            </div>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>

</script>

<style>
* {
  margin: 0;
  padding: 0;
  font-family: 'Inter', sans-serif;
}

.page-detail {
  margin: 50px auto 70px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.job-detail {
  min-width: 300px;
  border: solid 1px #EBEDF5;
  border-radius: 10px;
  margin: auto;
  padding: 35px 25px;
}

.sidebar-top {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
  width: 100%;
}

.sidebar-top p {
  font-size: 24px;
  font-weight: 600;
  padding: 0;
  color: #091E42;
}

.apply-btn {
  background-color: #016A70;
  margin-top: 40px;
  padding: 5px 0;
  width: 100%;
  max-width: 100%;
  height: 45px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 4px;
  cursor: pointer;
  white-space: nowrap;
}

.apply-btn p {
  color: #FFFF;
}

.sidebar-item {
  display: flex;
  flex-direction: column;
  border-bottom: none;
  padding: 8px 0;
}

.sidebar-item-title {
  font-size: 12.8px;
  color: #A5ADBA;
  line-height: 1.7;
  letter-spacing: 0.32px;
}

.sidebar-item-data {
  color: #091E42;
  font-size: 14.4px;
  letter-spacing: 0.32px;
  font-weight: 400;
}

label {
  font-size: 12.8px;
  font-weight: 700;
  line-height: 20.8px;
  margin-bottom: 7px;
  display: flex;
  text-align: left;
  color: #091e42;
}

.job-description {
  padding-top: 15px;
}

.job-form {
  padding: 25px 20px;
  width: 80%;
  margin: 40px auto 0;
}

.job-form form {
  width: 80%;
  margin: auto;
}

.job-form-names,
.job-form-contact {
  display: flex;
  flex-direction: column;
  gap: 40px;
}

.job-form-firstname,
.job-form-lastname,
.job-form-phone,
.job-form-email,
.job-form-github {
  width: 100%;
  margin-bottom: 20px;
}

.job-form-firstname input,
.job-form-lastname input,
.job-form-phone input,
.job-form-email input,
.job-form-github input {
  color: #091e42;
  font-size: 14.08px;
  padding: 15px 10px;
  /* margin-right: 10px; */
}

input {
  border-radius: 4px;
  transition: all .4s;
  background-color: 1px solid #fff;
  border: 1px solid #ebedf5;
  outline: none;
  appearance: none;
  display: block;
  width: 100%;
}

.job-form-letter textarea {
  line-height: 1.5;
  color: #091e42;
  resize: none;
  appearance: none;
  font-size: 14.08px;
  min-height: 160px;
  padding: 10px;
  outline: none;
  overflow: auto;
  max-width: 100%;
  border: 1px solid #ebedf5;
  border-radius: 3px;
  transition: all .2s;
  font-weight: 600;

  margin-bottom: 20px;
}

.job-upload-label {
  max-width: 145px;
  margin: 6px 0 0;
  font-weight: 700;
  font-size: 12.8px;
  line-height: 20.8px;
  background-color: #fff;
  box-shadow: inset 0 0 0 1px #dce0e8;
  height: 40px;
  padding: 0 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  border-radius: 4px;
  cursor: pointer;
  user-select: none;
  transition: all .5s;
  text-align: left;
}

.svg-inline--fa {
  overflow: visible;
  box-sizing: content-box;
  color: #091e42;
  transition: all .5s;
  font-size: 11.2px;
  padding: 0 5px 0 0 !important;
  height: 1em;
}

.job-upload-tip {
  margin-top: 8px;
}

.job-upload-tip p {
  color: #7a869a;
  font-size: 12px;
  font-weight: 600;
}

.job-submit-inner {
  height: 70px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.job-submit-powered {
  display: flex;
  flex-direction: row;
}

.job-submit-powered a {
  color: #7a869a;
  text-decoration: underline;
  transition: all .2s;
  font-size: 13.12px;
  font-weight: 700;
}

.job-submit-btn {
  margin-left: auto;
  padding: 0 40px;
  height: 40px;
  padding: 0 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  border-radius: 4px;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  transition: all .5s;
}

@media only screen and (min-width: 768px) {
  .job-form form {
    margin: auto;
  }

  .job-form-names,
  .job-form-contact {
    flex-direction: row;
  }

  .job-form-github input {
    width: 100%;
  }

  .job-form-firstname input,
  .job-form-email input {
    margin-right: 10px;
  }

  .job-form-letter textarea {
    width: 100%;
  }
}

@media only screen and (min-width: 1150px) {
  .page-detail {
    flex-direction: row;
  }
}
</style>