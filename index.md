---
title: TeamWork U
layout: default
cta:
  title: "TeamWork U helps students get hired faster"
  email: "buffy@teamworkonline.com"
  subject: "Test subject"
---
{% assign page_data = site.data.posts.teamWorkU[0] %}

{% include mega-header.html %}

<section class="py4">
<div class="container mx-auto flex flex-wrap">

{% assign item = site.data.posts.educatorTestimonial[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h2 class="oswald my0 h2">{{ item.title }}</h2>
<p class="h5 regular pb2">{{ item.sub_title }}</p>
{% include cta.html inverted=true %}
</div>
</div>
<div class="md-col-5 wow fadeInUp card-shadow my4" data-wow-delay="0.3s">
<div class="bg-black col-12 px2 py3 flex-none" style="background-color: #002244;">
<h3 class="oswald line-height-4 ltr-spacing-2 h4 m0 regular white">{{ item.quote }}</h3>
</div>
<div class="col-12 bg-white px2 py3 flex-auto">
<div class="flex items-center">
<div class="mr2 flex-none" style="background-image: url({{ item.image.url }}); background-size: cover; background-repeat: no-repeat; background-position: center; height: 64px; width: 64px;"></div>
<div class="flex-auto">
<p class="line-height-1 h5 regular mt0 mb1 black semibold">{{ item.name }}</p>
<p class="line-height-4 h5 regular m0 muted">{{ item.desc }}</p>
</div>
</div>
</div>
</div>

</div>
</section>

<section class="bg-gray benefits">
<div class="container mx-auto py4" style="margin-top: 8rem;">
<div class="flex flex-wrap" style="margin-top: -8rem;">
{% assign benefits = site.data.posts.benefits | sort: 'sort' %}
{% for item in benefits %}
<div class="flex-auto md-col-4 col-12 mx2 mb4 px3 pt3 card-shadow bg-white">
<h3 class="oswald black mb3 center h3">{{ item.title }}</h3>
<div class="pb3">
<ul>
<li><p class="line-height-6 py1 regular black checkmark">{{ item.ben1 }}</p></li>
<li><p class="line-height-6 py1 regular black checkmark">{{ item.ben2 }}</p></li>
<li><p class="line-height-6 py1 regular black checkmark">{{ item.ben3 }}</p></li>
</ul>
</div>
</div>

{% endfor %}
</div>
</div>
</section>


<section class="py4">
<div class="container mx-auto flex flex-wrap">


{% assign item = site.data.posts.calculator[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h3 class="oswald h3">{{ item.title }}</h3>
<p class="p">{{ item.desc }}</p>
</div>
</div>

<div class="px2 col-12 md-col-6 mx-auto flex">
<div class="flex items-center card-shadow bg-white">

<form class="px4">
  <label class="p black bold my0">Students</label>
  <input type="number" class="js-savings-input block col-12 mt1 mb3 field regular" placeholder="Enter no. of students" value="1000" step="100" onchange="savingsUpdate()">
  <p class="p black bold my0 tooltip">{{ item.savings_title }}<span class="tooltiptext ml1">{{ item.help }}</span></p>
  <h2 class="h2 green7 my0">$<span class="js-savings-value">28,800</span></h2>
</form>
<script>
// Ability to stringify and add commas
function numberWithCommas(x) {
    return x.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ",");
}

// Update the .js-savings-value based on .js-savings-input
function savingsUpdate() {
var savingsInput = document.querySelector(".js-savings-input").value;
// Formula for calculating the savings
var savingsValue = numberWithCommas((savingsInput * 30) - 1200);
document.querySelector(".js-savings-value").textContent = savingsValue;
}

// Run savingsUpdate on load to ensure a correct number
var ready = (callback) => {
if (document.readyState != "loading") callback();
else document.addEventListener("DOMContentLoaded", callback);
}

ready(() => {
savingsUpdate();
});
</script>

</div>
</div>

</div>
</section>


<section class="py4 bg-white">
<div class="container py4  mx-auto flex flex-wrap">

{% assign item = site.data.posts.schools[0] %}

<div class="md-col-8 col-12 mx-auto black mb2 flex items-center center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h2 class="oswald h2">{{ item.title }}</h2>
{% include cta.html inverted=true %}
</div>
</div>

<div class="flex flex-wrap my3">
  {% for item in item.image %}
  <div class="col-6 md-col-3 center px2 mt2">
    <img class="inline-block mb1" src="{{ item.url }}" alt="{{ item.title }}" width="100" />
  </div>
  {% endfor %}

</div>

</div>
</section>

<section class="py4">
<div class="container mx-auto flex flex-wrap">

{% assign item = site.data.posts.studentTestimonial[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h2 class="oswald my0 h2">{{ item.title }}</h2>
<p class="h5 regular pb2">{{ item.sub_title }}</p>
{% include cta.html inverted=true %}
</div>
</div>

<div class="md-col-5 wow fadeInUp card-shadow my4" data-wow-delay="0.3s">
<div class="bg-black col-12 px2 py3 flex-none" style="background-color: #CE1141;">
<h3 class="oswald line-height-4 ltr-spacing-2 h4 m0 pb2 regular white">{{ item.quote }}<i class="icofont-dart icofont-1x"></i></h3>

<a href="{{ item.url }}" target="new" class="oswald white text-decoration-none">〉{{ item.cta }}</a>
</div>

<div class="col-12 bg-white px2 py3 flex-auto">
<div class="flex items-center">
<div class="mr2 flex-none" style="background-image: url({{ item.image.url }}); background-size: cover; background-repeat: no-repeat; background-position: center; height: 64px; width: 64px;"></div>
<div class="flex-auto">
<p class="line-height-1 h5 regular mt0 mb1 black semibold">{{ item.name }}</p>
<p class="line-height-4 h5 regular m0 muted">{{ item.desc }}</p>
</div>
</div>
</div>
</div>

</div>
</section>
