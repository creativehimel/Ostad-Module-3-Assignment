<script setup>
import heroSection from "./data/heroSection.js";
import heroSectionData from "./data/heroSection.js";
import featuresSectionData from "./data/featuresSection.js";
import serviceSectionData from "./data/serviceSection.js";
import PricingSectionPlan from "./data/pricingSection.js";
import advantageSectionInfo from "./data/advantageSection.js";
import aboutSectionData from "./data/aboutSection.js";
import contactSectionData from "./data/contactSection.js";


</script>

<template>
  <section>
    <!--  Header Section Start  -->
    <header class="container">
      <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
          <a class="navbar-brand fs-3 fw-bold pe-5" href="#">Launch <span class="text-primary">.</span></a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item pe-2">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>
              <li class="nav-item dropdown pe-2">
                <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  Dropdown
                </a>
                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#">Testimonials</a></li>
                  <li><a class="dropdown-item" href="#">Menu Two</a></li>
                  <li><a class="dropdown-item" href="#">Menu Three</a></li>
                </ul>
              </li>
              <li class="nav-item pe-2">
                <a class="nav-link">Features</a>
              </li>
              <li class="nav-item pe-2">
                <a class="nav-link">Pricing</a>
              </li>
              <li class="nav-item pe-2">
                <a class="nav-link">About</a>
              </li>
              <li class="nav-item pe-2">
                <a class="nav-link">Contact</a>
              </li>
            </ul>
            <div class="d-flex">
              <button class="btn btn-outline-secondary me-3 rounded-pill shadow-none px-4">Sign In</button>
              <button class="btn btn-primary rounded-pill shadow-none px-4">Register</button>
            </div>
          </div>
        </div>
      </nav>
    </header>
    <!--  Header Section End  -->
    <!--  Hero Section Start  -->
    <section class="container">
      <div class="row d-flex justify-content-between align-items-center py-5 ">
        <div class="col-md-5">
          <h2 class="display-1 fw-bold pb-4">{{ heroSectionData[0].heroTitle }}</h2>
          <p class="pb-4 text-secondary fs-5">{{ heroSectionData[0].heroInfo }}</p>
          <div>
            <button class="btn btn-primary px-5 py-3 rounded-pill me-4 text-uppercase">See Features</button>
            <button class="btn btn-outline-primary px-5 py-3 rounded-pill text-uppercase">Pricing</button>
          </div>
        </div>
        <div class="col-md-7">
          <img :src="heroSection[1].heroImage" :alt="heroSection[1].imageTitle">
        </div>
      </div>

    </section>
    <!--  Hero Section End  -->
    <!--  Features Section start  -->
    <section class="container my-5 py-5">
      <div class="row">
        <div class="col-md-4 me-5">
          <span class="text-primary fw-semibold text-uppercase">{{ featuresSectionData[0].feaCaption }}</span>
          <h2 class="fs-1 mt-2">{{ featuresSectionData[0].feaTitle }}</h2>
          <p class="mt-4 fs-5 fw-normal text-secondary">{{ featuresSectionData[0].feaInfo }}</p>
          <ul class="list-unstyled">
            <li class="fs-6"><i class="fa-solid fa-check text-primary pe-2"></i> {{ featuresSectionData[0].feaKey.feaKey1 }}</li>
            <li><i class="fa-solid fa-check text-primary pe-2"></i> {{ featuresSectionData[0].feaKey.feaKey2 }}</li>
          </ul>
          <blockquote class="">{{ featuresSectionData[0].feaTestimonial.tesQuote }}</blockquote>
          <div class="d-flex align-items-center">
            <div>
              <img :src="featuresSectionData[0].feaTestimonial.userImage" alt="" width="60" height="60" class="rounded-circle">
            </div>
            <div class="ms-3">
              <h4 class="m-0">{{ featuresSectionData[0].feaTestimonial.userName }}</h4>
              <p class="m-0">{{ featuresSectionData[0].feaTestimonial.userJob }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-7">
            <img :src="featuresSectionData[1].feaImage" :alt="featuresSectionData[1].feaImageTitle" class="rounded p-2 shadow-sm img-thumbnail">
        </div>
      </div>
    </section>
    <!--  Features Section End  -->
    <!--  Features Section start  -->
    <section class="bg-body-secondary py-5 pt-5">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <div class="d-flex align-items-start">
              <div class="tab-content" id="v-pills-tabContent">
                <div class="tab-pane fade show active" id="v-pills-home" role="tabpanel" aria-labelledby="v-pills-home-tab" tabindex="0">
                  <img :src="featuresSectionData[1].feaImage" alt="" class="rounded p-2 shadow-sm img-thumbnail">
                </div>
                <div class="tab-pane fade" id="v-pills-profile" role="tabpanel" aria-labelledby="v-pills-profile-tab" tabindex="0">
                  <img :src="featuresSectionData[1].feaImage" alt="" class="rounded p-2 shadow-sm img-thumbnail">
                </div>
                <div class="tab-pane fade" id="v-pills-disabled" role="tabpanel" aria-labelledby="v-pills-disabled-tab" tabindex="0">
                  <img :src="featuresSectionData[1].feaImage" alt="" class="rounded p-2 shadow-sm img-thumbnail">
                </div>
                <div class="tab-pane fade" id="v-pills-messages" role="tabpanel" aria-labelledby="v-pills-messages-tab" tabindex="0">
                  <img :src="featuresSectionData[1].feaImage" alt="" class="rounded p-2 shadow-sm img-thumbnail">
                </div>
              </div>
              <div class="nav flex-column  nav-color ms-3" id="v-pills-tab" role="tablist" aria-orientation="vertical">
                <button class="nav-link active" id="v-pills-home-tab" data-bs-toggle="pill" data-bs-target="#v-pills-home" type="button" role="tab" aria-controls="v-pills-home" aria-selected="true">
                  <div class="d-flex align-items-center">
                    <div class="border border-info rounded-4 bg-info bg-gradient">
                      <img :src="serviceSectionData[0].serviceIcon" :alt="serviceSectionData[0].serviceIconName" width="30" height="30" class="m-3">
                    </div>
                    <div>
                      <h6 class="fs-3 text-start ps-3 text-secondary">{{ serviceSectionData[0].serviceTitle }}</h6>
                      <p class="fs-5 text-start ps-3 text-secondary">{{ serviceSectionData[0].serviceInfo }}</p>
                    </div>
                  </div>
                </button>
                <button class="nav-link "  id="v-pills-profile-tab" data-bs-toggle="pill" data-bs-target="#v-pills-profile" type="button" role="tab" aria-controls="v-pills-profile" aria-selected="false">
                  <div class="d-flex align-items-center">
                    <div class="border border-warning rounded-4 bg-warning bg-gradient">
                      <img :src="serviceSectionData[1].serviceIcon" :alt="serviceSectionData[1].serviceIconName" width="30" height="30" class="m-3">
                    </div>
                    <div>
                      <h6 class="fs-3 text-start ps-3 text-secondary">{{ serviceSectionData[1].serviceTitle }}</h6>
                      <p class="fs-5 text-start ps-3 text-secondary">{{ serviceSectionData[1].serviceInfo }}</p>
                    </div>
                  </div>
                </button>
                <button class="nav-link " id="v-pills-disabled-tab" data-bs-toggle="pill" data-bs-target="#v-pills-disabled" type="button" role="tab" aria-controls="v-pills-disabled" aria-selected="false">
                  <div class="d-flex align-items-center">
                    <div class="border border-danger rounded-4 bg-danger bg-gradient">
                      <img :src="serviceSectionData[2].serviceIcon" :alt="serviceSectionData[2].serviceIconName" width="30" height="30" class="m-3">
                    </div>
                    <div>
                      <h6 class="fs-3 text-start ps-3 text-secondary">{{ serviceSectionData[2].serviceTitle }}</h6>
                      <p class="fs-5 text-start ps-3 text-secondary">{{ serviceSectionData[2].serviceInfo }}</p>
                    </div>
                  </div>
                </button>
                <button class="nav-link " id="v-pills-messages-tab" data-bs-toggle="pill" data-bs-target="#v-pills-messages" type="button" role="tab" aria-controls="v-pills-messages" aria-selected="false">
                  <div class="d-flex align-items-center">
                    <div class="border border-primary rounded-4 bg-primary bg-gradient">
                      <img :src="serviceSectionData[3].serviceIcon" :alt="serviceSectionData[3].serviceIconName" width="30" height="30" class="m-3">
                    </div>
                    <div>
                      <h6 class="fs-3 text-start ps-3 text-secondary">{{ serviceSectionData[3].serviceTitle }}</h6>
                      <p class="fs-5  text-start ps-3 text-secondary">{{ serviceSectionData[3].serviceInfo }}</p>
                    </div>
                  </div>
                </button>

              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--  Features Section End  -->
    <!--  Service Section Start  -->
    <section class="container my-5 py-5">
      <div class="row">
        <div class="col-md-6 col-lg-3 mb-4 mb-lg-0">
          <div>
            <div >
              <img :src="serviceSectionData[0].serviceIcon" :alt="serviceSectionData[0].serviceIconName" width="90" height="90" class="border border-info rounded-4 p-3 bg-info bg-gradient">
            </div>
            <div class="mt-5">
              <h3 class="fs-3 text-secondary">{{ serviceSectionData[0].serviceTitle }}</h3>
              <p class="pt-2 fs-5 text-secondary">{{ serviceSectionData[0].serviceInfo }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3 mb-4 mb-lg-0">
          <div>
            <div >
              <img :src="serviceSectionData[1].serviceIcon" :alt="serviceSectionData[1].serviceIconName" width="90" height="90" class="border p-3 border-warning rounded-4 bg-warning bg-gradient">
            </div>
            <div class="mt-5">
              <h3 class="fs-3 text-secondary">{{ serviceSectionData[1].serviceTitle }}</h3>
              <p class="pt-2 fs-5 text-secondary">{{ serviceSectionData[1].serviceInfo }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-3 mb-4 mb-lg-0">
          <div>
            <div >
              <img :src="serviceSectionData[2].serviceIcon" :alt="serviceSectionData[2].serviceIconName" width="90" height="90" class="p-3 border border-danger rounded-4 bg-danger bg-gradient">
            </div>
            <div class="mt-5">
              <h3 class="fs-3 text-secondary">{{ serviceSectionData[2].serviceTitle }}</h3>
              <p class="pt-2 fs-5 text-secondary">{{ serviceSectionData[2].serviceInfo }}</p>
            </div>
          </div>
        </div><div class="col-md-6 col-lg-3 mb-4 mb-lg-0">
          <div>
            <div >
              <img :src="serviceSectionData[3].serviceIcon" :alt="serviceSectionData[3].serviceIconName" width="90" height="90" class=" p-3 border border-primary rounded-4 bg-primary bg-gradient">
            </div>
            <div class="mt-5">
              <h3 class="fs-3 text-secondary">{{ serviceSectionData[3].serviceTitle }}</h3>
              <p class="pt-2 fs-5 text-secondary">{{ serviceSectionData[3].serviceInfo }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--  Service Section End  -->
    <!--  Pricing Section Start  -->
    <section class="bg-body-secondary py-5 pt-5">
      <div class="container mb-5">
        <div class="row">
          <div class="text-center">
            <h2 class="display-2 fw-bold mt-5 mb-3">{{ PricingSectionPlan[0] }}</h2>
            <p class="fs-4 mb-5">{{ PricingSectionPlan[1] }}</p>
          </div>
          <div class="col-md-4">
            <div class="pricing ">
              <div class="body shadow-sm">
                <div class="price">
                  <span class="d-block plan display-4 fw-semibold mb-2">{{ PricingSectionPlan[2].planName }}</span>
                  <span class="price">
                    <sup class="fs-2 text-primary">$</sup>
                    <span class="display-4 fw-semibold text-primary ps-2">{{ PricingSectionPlan[2].planPrice }}</span>
                  </span>
                </div>
                <ul class="list-unstyled ul-check primary my-5">
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[2].planFeatures.key1 }}</p>
                  </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[2].planFeatures.key2 }}</p>
                     </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p> {{ PricingSectionPlan[2].planFeatures.key3 }}</p>
                    </li>
                </ul>
                <p class="text-center mb-0">
                  <a href="#" class="btn btn-outline-primary py-3 px-5 fs-4 rounded-pill">Get Started</a>
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="pricing">
              <div class="body shadow-sm">
                <div class="price">
                  <span class="d-block plan display-4 fw-semibold mb-2">{{ PricingSectionPlan[3].planName }}</span>
                  <span class="price">
                    <sup class="fs-2 text-primary">$</sup>
                    <span class="display-4 fw-semibold text-primary ps-2">{{ PricingSectionPlan[3].planPrice }}</span>
                  </span>
                </div>
                <ul class="list-unstyled ul-check primary my-5">
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[3].planFeatures.key1 }}</p>
                  </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[3].planFeatures.key2 }}</p>
                     </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p> {{ PricingSectionPlan[3].planFeatures.key3 }}</p>
                    </li>
                </ul>
                <p class="text-center mb-0">
                  <a href="#" class="btn btn-primary py-3 px-5 fs-4 rounded-pill">Get Started</a>
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="pricing">
              <div class="body shadow-sm">
                <div class="price">
                  <span class="d-block plan display-4 fw-semibold mb-2">{{ PricingSectionPlan[4].planName }}</span>
                  <span class="price">
                    <sup class="fs-2 text-primary">$</sup>
                    <span class="display-4 fw-semibold text-primary ps-2">{{ PricingSectionPlan[4].planPrice }}</span>
                  </span>
                </div>
                <ul class="list-unstyled ul-check primary my-5">
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[4].planFeatures.key1 }}</p>
                  </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p>{{ PricingSectionPlan[4].planFeatures.key2 }}</p>
                     </li>
                  <li class="fs-4 d-flex">
                    <p><i class="fa-solid fa-check text-primary me-2"></i></p>
                    <p> {{ PricingSectionPlan[4].planFeatures.key3 }}</p>
                    </li>
                </ul>
                <p class="text-center mb-0">
                  <a href="#" class="btn btn-outline-primary py-3 px-5 fs-4 rounded-pill">Get Started</a>
                </p>
              </div>
            </div>
          </div>


        </div>
      </div>
    </section>
    <!--  Pricing Section End  -->
    <!--  Advantage Section Start  -->
    <section class="container mt-5 py-5">
      <div class="row">
        <h3 class="text-center display-4 fw-semibold">{{ advantageSectionInfo[0] }}</h3>
        <p class="text-center fs-4 lh-lg mb-5">{{ advantageSectionInfo[1] }}</p>
        <div class="col-md-6 py-4 px-2">
          <div class="d-flex justify-content-between align-items-center">
            <div class="me-5">
              <img :src="advantageSectionInfo[2].serviceIcon" :alt="advantageSectionInfo[2].serviceIconName" width="70" height="70" class="border border-info rounded-4 p-3 bg-info bg-gradient">
            </div>
            <div>
              <h3 class="fs-3 fw-semibold">{{ advantageSectionInfo[2].serviceTitle }}</h3>
              <p class="fs-5 lh-md">{{ advantageSectionInfo[2].serviceInfo }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 py-4 px-2">
          <div class="d-flex justify-content-between">
            <div class="me-5">
              <img :src="advantageSectionInfo[3].serviceIcon" :alt="advantageSectionInfo[3].serviceIconName" width="70" height="70" class="border border-warning rounded-4 p-3 bg-warning bg-gradient">
            </div>
            <div>
              <h3 class="fs-3 fw-semibold">{{ advantageSectionInfo[3].serviceTitle }}</h3>
              <p class="fs-5 lh-md">{{ advantageSectionInfo[3].serviceInfo }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 py-4 px-2">
          <div class="d-flex justify-content-between">
            <div class="me-5">
              <img :src="advantageSectionInfo[4].serviceIcon" :alt="advantageSectionInfo[4].serviceIconName" width="70" height="70" class="border border-danger rounded-4 p-3 bg-danger bg-gradient">
            </div>
            <div>
              <h3 class="fs-3 fw-semibold">{{ advantageSectionInfo[4].serviceTitle }}</h3>
              <p class="fs-5 lh-md">{{ advantageSectionInfo[4].serviceInfo }}</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 py-4 px-2">
          <div class="d-flex justify-content-between">
            <div class="me-5">
              <img :src="advantageSectionInfo[5].serviceIcon" :alt="advantageSectionInfo[5].serviceIconName" width="70" height="70" class="border border-primary rounded-4 p-3 bg-primary bg-gradient">
            </div>
            <div>
              <h3 class="fs-3 fw-semibold">{{ advantageSectionInfo[5].serviceTitle }}</h3>
              <p class="fs-5 lh-md">{{ advantageSectionInfo[5].serviceInfo }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--  Advantage Section End  -->
    <!--  About Section start  -->
    <section class="container my-5 py-5">
      <div class="row">
        <div class="col-md-7">
          <img :src="aboutSectionData.sectionImage" width="800" height="1000">
        </div>
        <div class="col-md-5 ps-5">
          <span class="text-primary fw-semibold fs-3">{{ aboutSectionData.sectionCation }}</span>
          <h2 class="display-3 fw-bold">{{ aboutSectionData.sectionHeading }}</h2>
          <p class="fs-4 text-secondary lh-md pt-4">{{ aboutSectionData.sectionInfo1 }}</p>
          <p class="fs-4 text-secondary lh-md mb-5">{{ aboutSectionData.sectionInfo2 }}</p>
          <ul class="list-unstyled">
            <li class="fs-3 text-secondary"><i class="text-primary me-3 fa-solid fa-check"></i> {{ aboutSectionData.sectionFeatures.key1 }}</li>
            <li class="fs-3 text-secondary"><i class="text-primary me-3 fa-solid fa-check"></i> {{ aboutSectionData.sectionFeatures.key2 }}</li>
            <li class="fs-3 text-secondary"><i class="text-primary me-3 fa-solid fa-check"></i> {{ aboutSectionData.sectionFeatures.key3 }}</li>
          </ul>
          <div class="d-flex mt-5">
            <div class="me-5 pe-5">
              <h2>{{ aboutSectionData.users.members }}</h2>
              <h6>MEMBERS</h6>
            </div>
            <div>
              <h2>{{ aboutSectionData.users.team }}</h2>
              <h6>TEAM</h6>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--  About Section End  -->
    <!--  Contact Section Start  -->
    <section class="container my-5 py-5">
      <div class="row">
        <div class="col-md-8">
          <form class="row">
            <div class="col-md-6 mb-4">
              <label for="fname" class="form-label">First Name</label>
              <input type="text" class="form-control shadow-none" id="fname">
            </div>
            <div class="col-md-6 mb-4">
              <label for="lname" class="form-label">Last Name</label>
              <input type="text" class="form-control shadow-none" id="lname">
            </div>
            <div class="col-md-12 mb-4">
              <label for="email" class="form-label">Email Address</label>
              <input type="email" class="form-control shadow-none" id="email">
            </div>
            <div class="col-md-12">
              <label for="msg" class="form-label">Message</label>
              <textarea class="form-control" id="msg" rows="3"></textarea>
            </div>
          </form>
          <button type="submit" class="btn btn-primary mt-3 px-4 py-3 rounded-pill">Send Message</button>
        </div>
        <div class="col-md-4 ps-5">
          <h3>{{ contactSectionData.contactInfo.contactTitle }}</h3>
          <ul class="list-unstyled">
            <li class="pb-2">
              <a href="" class="text-dark text-decoration-none"><i class="fa-solid fa-location-dot me-2"></i> {{ contactSectionData.contactInfo.address }}</a>
            </li>
            <li  class="pb-2">
              <a href="tel:123-456-7890" class="text-dark text-decoration-none"><i class="fa-solid fa-phone me-2"></i> {{ contactSectionData.contactInfo.phone1 }}</a>
            </li>
            <li class="pb-2">
              <a href="tel:123-456-7890" class="text-dark text-decoration-none"><i class="fa-solid fa-phone me-2"></i> {{ contactSectionData.contactInfo.phone2 }}</a>
            </li>
            <li class="pb-2">
              <a href="mailto:email@example.com" class="text-dark text-decoration-none"><i class="fa-solid fa-envelope me-2"></i> {{ contactSectionData.contactInfo.email }}</a>
            </li>
            <li class="pb-2">
              <a :href="contactSectionData.contactInfo.website" class="text-dark text-decoration-none"><i class="fa-solid fa-globe me-2"></i> {{ contactSectionData.contactInfo.website }}</a>
            </li>
          </ul>
        </div>
      </div>
    </section>
    <!--  Contact Section End  -->
    <!--  Footer Section Start  -->
    <footer class="bg-body-secondary py-5">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <h5>About Launch.</h5>
            <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.</p>
            <div class="py-4">
              <h5>Connect</h5>
              <ul class="list-unstyled d-flex gap-3 py-1">
                <li><i class="fa-brands fa-facebook"></i></li>
                <li><i class="fa-brands fa-twitter"></i></li>
                <li><i class="fa-brands fa-instagram"></i></li>
                <li><i class="fa-brands fa-linkedin-in"></i></li>
                <li><i class="fa-brands fa-pinterest"></i></li>
                <li><i class="fa-solid fa-globe"></i></li>
              </ul>
            </div>
          </div>
          <div class="col-md-2">
            <h5>Projects</h5>
            <ul class="list-unstyled py-4">
              <li class="pb-2">La Lega Stadium</li>
              <li class="pb-2">France Building</li>
              <li class="pb-2">22 New Homes</li>
              <li class="pb-2">Manage Center</li>
              <li>Sports Hall</li>
            </ul>
          </div>
          <div class="col-md-2">
            <h5>Services</h5>
            <ul class="list-unstyled py-4">
              <li class="pb-2">Architect</li>
              <li class="pb-2">Interior Design</li>
              <li class="pb-2">Landscape Design</li>
              <li class="pb-2">Consultancy</li>
            </ul>
          </div>
          <div class="col-md-4">
            <h5>Contact</h5>
            <ul class="list-unstyled">
              <li class="pb-2">
                <a href="" class="text-dark text-decoration-none"><i class="fa-solid fa-location-dot me-2"></i> {{ contactSectionData.contactInfo.address }}</a>
              </li>
              <li  class="pb-2">
                <a href="tel:123-456-7890" class="text-dark text-decoration-none"><i class="fa-solid fa-phone me-2"></i> {{ contactSectionData.contactInfo.phone1 }}</a>
              </li>
              <li class="pb-2">
                <a href="tel:123-456-7890" class="text-dark text-decoration-none"><i class="fa-solid fa-phone me-2"></i> {{ contactSectionData.contactInfo.phone2 }}</a>
              </li>
              <li class="pb-2">
                <a href="mailto:email@example.com" class="text-dark text-decoration-none"><i class="fa-solid fa-envelope me-2"></i> {{ contactSectionData.contactInfo.email }}</a>
              </li>
              <li class="pb-2">
                <a :href="contactSectionData.contactInfo.website" class="text-dark text-decoration-none"><i class="fa-solid fa-globe me-2"></i> {{ contactSectionData.contactInfo.website }}</a>
              </li>
            </ul>
          </div>
          <div class="col-md-12">
            <p class="text-center mt-3">Copyright ©2023 All rights reserved | This template is made with  by Colorlib</p>
          </div>
        </div>
      </div>
    </footer>
    <!--  Footer Section End  -->
  </section>
</template>

<style scoped>
.nav-color .nav-link.active,
.nav-color .show>.nav-link{
  background-color: #ffffff;
  border-radius: 5px;
}
.pricing .body{
  position: relative;
  z-index: 1;
  background: #ffffff;
  border-radius: 40px;
  padding: 50px;
}
.pricing .body .price{
  text-align: center;
}
</style>
