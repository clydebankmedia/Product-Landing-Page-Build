# Solution Code - Styling Practice with Mockup

<details>
<summary> Step 1 Solution - Review the Mockup & Copy</summary>
    
```html
<!-- NO SOLUTION CODE REQUIRED -->
```

</details>

<details>
<summary>Step 2 Solution – Add Semantic HTML Structure</summary>
HTML – `index.html` 

```html
<!-- <html> and <head> content above --> 

<body>
  <header>
    <nav class="site-nav">
      <div class="nav-inner container">
        <a class="brand" href="#">Purr &amp; Paws</a>
        <ul class="nav-links">
          <li><a href="#why">Why Us</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#reviews">Reviews</a></li>
          <li><a href="#cta" class="nav-cta">Book</a></li>
        </ul>
      </div>
    </nav>
    
  </header>

  <main>
	  <section id="hero"></section>
    <section id="why"></section>
    <section id="services"></section>
    <section id="reviews"></section>
    <section id="cta"></section>
  </main>

  <footer></footer>
</body>

<!-- </html> content below -->
```

</details>  
<details>
<summary>Step 3 Solution –  Add Navigation</summary>

HTML - `index.html`

```html
<nav class="site-nav">
  <div class="nav-inner container">
    <a class="brand" href="#">Purr &amp; Paws</a>
    <ul class="nav-links">
      <li><a href="#why">Why Us</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#reviews">Reviews</a></li>
      <li><a href="#cta" class="nav-cta">Book</a></li>
    </ul>
  </div>
</nav>
```

CSS – `styles.css`

```css
.site-nav {
  background: #fff;
  border-bottom: 1px solid #ddd;
}
.nav-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.brand {
  font-weight: 700;
  letter-spacing: 0.3px;
  text-decoration: none;
  color: #2C3E50;
}
.nav-links {
  display: flex;
  gap: 1.25rem;
  list-style: none;
}
.nav-cta {
  border: 1px solid #3498DB;
  border-radius: 6px;
  padding: 0.35rem 0.6rem;
}
```

</details>   
<details>
<summary> Step 4A Solution – Build the Hero Section</summary>

HTML – `index.html`

```html
<section id="hero">
  <div class="overlay">
    <div class="container">
      <h1>Purr &amp; Paws Pet Cleaning</h1>
      <p>Gentle care, sparkling clean — because your pets deserve the best.</p>
      <a href="#cta" class="btn btn-primary">Schedule Now</a>
    </div>
  </div>
</section>
```

CSS – `styles.css`

```css
#hero {
  background: url('https://images.unsplash.com/photo-1517849845537-4d257902454a?w=1600&q=80&auto=format&fit=crop')
              center/cover no-repeat;
  min-height: 78vh;
  display: flex;
  align-items: center;
  color: #fff;
}

#hero .overlay {
  background: rgba(0,0,0,0.4);
  width: 100%;
  display: flex;
  align-items: center;
  padding: 4rem 0;
}

```

</details>   



<details>
<summary> Step 4B Solution – Create “Why Choose Us” Cards</summary>

HTML – `index.html`

```html
<section id="why" class="container">
      <h2>Why Choose Us</h2>
      <p class="section-intro">
        We’re a gentle, pet-first grooming team focused on comfort, cleanliness, and confidence.
        From first-timers to frequent visitors, our approach keeps stress low and tails wagging.
        Expect clear communication, fair pricing, and a spotless finish.
      </p>
      <ul class="feature-list">
        <li class="feature-card">
          <h3>Safer Products</h3>
          <p>We use gentle, vet-reviewed shampoos and cleaners that protect sensitive skin.</p>
        </li>
        <li class="feature-card">
          <h3>Handled with Care</h3>
          <p>Our groomers are trained to reduce stress and keep sessions calm and friendly.</p>
        </li>
        <li class="feature-card">
          <h3>Flexible Packages</h3>
          <p>Pick a plan that fits your schedule and budget—no surprise add-ons.</p>
        </li>
      </ul>
</section>

```

CSS – `styles.css`

```css
.feature-list {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
.feature-card {
  flex: 0 0 33.333%;
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1rem;
}
```

</details>   



<details>
<summary> Step 4C Solution – Add Service Cards with Hover Interaction</summary>

HTML – `index.html`

```html
<section id="services" class="container">
  <h2>Our Services</h2>
  <ul class="card-list">
    <li>Full-service grooming</li>
    <li>Wash &amp; dry</li>
    <li>Nail trimming</li>
    <li>Ear cleaning</li>
  </ul>
</section>
```

CSS – `styles.css`

```css
.card-list {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
.card-list li {
	flex: 1 1 calc(25% - 1rem);
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 1.25rem;
  text-align: center;
  transition: 0.2s;
}
.card-list li:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 12px rgba(0,0,0,0.08);
}
```

</details>   

<details>
<summary> Step 4D Solution – Review Core Sections</summary>

```html
<!-- Style QA Step - No code changes provided -->
```

</details>  

<details>
<summary> Step 5 Solution – Build the Footer</summary>

HTML – `index.html`

```html
<footer class="site-footer">
  <div class="container">
    <p>© 2025 Purr &amp; Paws Pet Cleaning. All rights reserved.</p>
    <p>Contact: info@purrandpaws.com</p>
  </div>
</footer>
```

CSS – `styles.css`

```css
.site-footer {
  border-top: 1px solid #ddd;
  text-align: center;
  color: #666;
  padding: 1rem;
  font-size: 0.9rem;
}
```
</details>   

<details>
<summary> Step 6 Solution – Typography Pass</summary>

CSS – `styles.css`

```css
body {
  font-family: 'Open Sans', Arial, sans-serif;
  font-size: 16px;
  line-height: 1.6;
  color: #2C3E50;
}

h1, h2, h3 {
  font-family: 'Montserrat', sans-serif;
  color: #2C3E50;
}

h1 { font-size: 2.5rem; line-height: 1.2; }
h2 { font-size: 1.6rem; margin-bottom: 0.5rem; }
h3 { font-size: 1.15rem; }
```

</details> 

<details>
<summary> Step 7 Solution – Add the Reviews Section</summary>

HTML – `index.html`

```html
<section id="reviews" class="container">
  <h2>What Pet Parents Say</h2>
  <ul class="reviews-grid">
    <li>
      <blockquote>“My dog has never looked happier after a wash!”</blockquote>
      <cite>— Happy Dog Parent</cite>
    </li>
    <li>
      <blockquote>“Finally a grooming service that treats cats gently.”</blockquote>
      <cite>— Cat Guardian</cite>
    </li>
    <!-- add 4 more -->
  </ul>
</section>

```

CSS – `styles.css`

```css
.reviews-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}
.reviews-grid li {
  flex: 0 0 calc(33.333% - 1rem);
  min-width: 240px;
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 1rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
}

blockquote {
  border-left: 4px solid #3498DB;
  padding-left: 0.5rem;
  font-style: italic;
}

cite {
  display: block;
  color: #666;
  font-size: 0.9rem;
}
```
</details> 

<details>
<summary> Step 8 Solution – Add the CTA Section</summary>

HTML – `index.html`

```html
<section id="cta" class="cta-band">
  <div class="container">
    <h2>Book Today</h2>
    <p>Book your pet’s first clean today and get 20% off.</p>
    <a href="#" class="btn btn-light">Get 20% Off</a>
  </div>
</section>
```

CSS – `styles.css`

```css
.cta-band {
  background: linear-gradient(135deg, #3498DB, #E67E22);
  text-align: center;
  color: #fff;
  padding: 4rem 1.5rem;
}
.cta-band h2, 
.cta-band p {
  color: #fff;
}
```
</details> 

<details>
<summary> Step 9 Solution – Refine & Polish</summary>

CSS – `styles.css`

```css
/* CTA Band polish */
.cta-band {
  background: linear-gradient(135deg, #2C3E50 0%, #3b4d63 100%);
  text-align: center;
  color: #fff;
  padding: 4rem 1.5rem;
}
.cta-band h2 { color: #fff; }

/* Navigation hover */
.nav-links a:hover {
  color: #3498DB;
}

/* Button consistency */
.btn-primary:hover { background: #cf6916; }
.btn-light:hover   { background: #F0F0F0; }

/* Card hover (Services + Reviews) */
.card-list li:hover,
.reviews-grid li:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 12px rgba(0,0,0,0.08);
}
```
</details> 

<details>
<summary> Step 10 Solution – Add Responsive Enhancements (Optional)</summary>

CSS – `styles.css`

```css
@media (max-width: 768px) {
  .nav-inner {
    flex-direction: column;
  }
  
  .feature-card,
  .card-list li,
  .reviews-grid li {
    flex: 0 0 100%;
    max-width: 100%;
  }
}
```
</details> 

<details>
<summary>Final Solution</summary>

HTML – `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Purr & Paws Pet Cleaning</title>
  <link rel="stylesheet" href="styles.css" />
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Open+Sans:wght@400;500&display=swap" rel="stylesheet">
</head>
<body>

  <header>
    <!-- Full-width nav bar; content sits inside guttered container -->
    <nav class="site-nav">
      <div class="nav-inner container">
        <a class="brand" href="#">Purr &amp; Paws</a>
        <ul class="nav-links">
          <li><a href="#why">Why Us</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#reviews">Reviews</a></li>
          <li><a href="#cta" class="nav-cta">Book</a></li>
        </ul>
      </div>
    </nav>
  </header>

  <main>
  
	  <!-- Hero with Unsplash background + overlay -->
    <section id="hero">
      <div class="overlay">
        <div class="container">
          <h1>Purr &amp; Paws Pet Cleaning</h1>
          <p>Gentle care, sparkling clean — because your pets deserve the best.</p>
          <a href="#cta" class="btn btn-primary">Schedule Now</a>
        </div>
      </div>
    </section>
    
    <!-- Why Choose Us -->
    <section id="why" class="container">
      <h2>Why Choose Us</h2>
      <p class="section-intro">
        We’re a gentle, pet-first grooming team focused on comfort, cleanliness, and confidence.
        From first-timers to frequent visitors, our approach keeps stress low and tails wagging.
        Expect clear communication, fair pricing, and a spotless finish.
      </p>
      <ul class="feature-list">
        <li class="feature-card">
          <h3>Safer Products</h3>
          <p>We use gentle, vet-reviewed shampoos and cleaners that protect sensitive skin.</p>
        </li>
        <li class="feature-card">
          <h3>Handled with Care</h3>
          <p>Our groomers are trained to reduce stress and keep sessions calm and friendly.</p>
        </li>
        <li class="feature-card">
          <h3>Flexible Packages</h3>
          <p>Pick a plan that fits your schedule and budget—no surprise add-ons.</p>
        </li>
      </ul>
    </section>

    <!-- Our Services -->
    <section id="services" class="container">
      <h2>Our Services</h2>
      <ul class="card-list">
        <li>Full-service grooming</li>
        <li>Wash &amp; dry</li>
        <li>Nail trimming</li>
        <li>Ear cleaning</li>
      </ul>
    </section>

    <!-- Customer Reviews -->
    <section id="reviews" class="container">
      <h2>What Pet Parents Say</h2>
      <p class="section-intro">
        Real feedback from our community. We read every comment and improve our care based on your experience.
      </p>

      <ul class="reviews-grid">
        <li>
          <blockquote class="quote">“My dog has never looked happier after a wash!”</blockquote>
          <cite>— Happy Dog Parent</cite>
        </li>
        <li>
          <blockquote class="quote">“Finally a grooming service that treats cats gently.”</blockquote>
          <cite>— Cat Guardian</cite>
        </li>
        <li>
          <blockquote class="quote">“Quick booking, fair pricing, and super kind staff. Five stars.”</blockquote>
          <cite>— Busy Pet Owner</cite>
        </li>
        <li>
          <blockquote class="quote">“They noticed a skin irritation early and suggested a vet check. So grateful.”</blockquote>
          <cite>— Grateful Human</cite>
        </li>
        <li>
          <blockquote class="quote">“Our anxious pup handled the visit like a champ thanks to their calm approach.”</blockquote>
          <cite>— First-Time Visitor</cite>
        </li>
        <li>
          <blockquote class="quote">“Clean, fast, friendly—our go-to for monthly baths.”</blockquote>
          <cite>— Regular Client</cite>
        </li>
      </ul>
    </section>

    <!-- CTA Band -->
    <section id="cta" class="cta-band">
      <div class="container">
        <h2>Book Today</h2>
        <p>Book your pet’s first clean today and get 20% off.</p>
        <a href="#" class="btn btn-light">Get 20% Off</a>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="site-footer">
    <div class="container">
      <p>© 2025 Purr &amp; Paws Pet Cleaning. All rights reserved.</p>
      <p>Contact: info@purrandpaws.com</p>
    </div>
  </footer>

</body>
</html>

```

CSS – `styles.css`

```css
/* =========================
   Reset / Base
   ========================= */
*,
*::before,
*::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html,
body {
    height: 100%;
}

body {
    font-family: 'Open Sans', Arial, sans-serif;
    font-size: 16px;
    line-height: 1.6;
    color: #2C3E50;
    background: #F9F9F9;
}

/* Reusable container with gutters */
.container {
    max-width: 1120px;
    margin: 0 auto;
    padding: 0 1rem;
}

/* Headings */
h1,
h2,
h3 {
    font-family: 'Montserrat', sans-serif;
    color: #2C3E50;
}

h1 {
    font-size: 2.5rem;
    line-height: 1.2;
}

h2 {
    font-size: 1.6rem;
    margin-bottom: 0.5rem;
}

h3 {
    font-size: 1.15rem;
}

/* Paragraphs and helper */
.section-intro {
    color: #666666;
    margin-top: 0.25rem;
    margin-bottom: 1rem;
    max-width: 65ch;
}

/* Space sections consistently */
main section.container {
    margin: 3rem auto;
    /* more vertical margin */
    padding: 3rem 1.5rem;
    /* more inner padding */
}

/* =========================
   Navigation
   ========================= */
.site-nav {
    width: 100%;
    background: #FFFFFF;
    border-bottom: 1px solid #DDDDDD;
}

.nav-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    min-height: 64px;
    padding: 0.5rem 0;
}

.brand {
    font-weight: 700;
    letter-spacing: 0.3px;
    text-decoration: none;
    color: #2C3E50;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 1.25rem;
}

.nav-links a {
    text-decoration: none;
    color: #2C3E50;
    font-weight: 500;
    padding: 0.25rem 0.5rem;
}

.nav-links a:hover {
    color: #3498DB;
}

.nav-cta {
    border: 1px solid #3498DB;
    border-radius: 6px;
    padding: 0.35rem 0.6rem;
}

/* =========================
   Hero
   ========================= */
#hero {
    background: url('https://images.unsplash.com/photo-1517849845537-4d257902454a?q=80&w=1600&auto=format&fit=crop') center/cover no-repeat;
    position: relative;
    color: #FFFFFF;
    min-height: 78vh;
    display: flex;
    align-items: stretch;
}

#hero .overlay {
    background: rgba(0, 0, 0, 0.4);
    width: 100%;
    display: flex;
    align-items: center;
    padding: 4rem 0;
}

#hero h1 {
    margin-bottom: 0.75rem;
    color: #ccc
}

#hero p {
    margin-bottom: 1.25rem;
    max-width: 56ch;
}

/* Buttons */
.btn {
    display: inline-block;
    padding: 0.8rem 1.25rem;
    border-radius: 8px;
    font-weight: 600;
    text-decoration: none;
    transition: 0.2s ease;
    cursor: pointer;
}

.btn-primary {
    background: #E67E22;
    color: #FFFFFF;
}

.btn-primary:hover {
    background: #cf6916;
}

.btn-light {
    background: #FFFFFF;
    color: #2C3E50;
    border: 1px solid #DDDDDD;
}

.btn-light:hover {
    background: #F0F0F0;
}

/* =========================
   Why Choose Us (Flexbox)
   ========================= */
#why {
    background: #FFFFFF;
}

.feature-list {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-top: 1rem;
    padding: 0;
}

.feature-card {
    flex: 1 1 30%;
    /* 3 columns created by baseline value */
    max-width: 33.333%;
    min-width: 220px;
    background: #FFFFFF;
    border: 1px solid #DDDDDD;
    border-radius: 12px;
    padding: 1rem;
}

.feature-card h3 {
    margin-bottom: 0.35rem;
}

.feature-card p {
    color: #666666;
    line-height: 1.55;
}

/* =========================
   Services (Flexbox)
   ========================= */
.card-list {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 1.25rem;
    margin-top: 1rem;
    padding: 0;
}

.card-list li {
    flex: 1 1 calc(25% - 1rem);
    /* 3 columns created by baseline value */
    min-width: 240px;
    /* min-width: 240px; */
    background: #FFFFFF;
    border: 1px solid #DDDDDD;
    border-radius: 12px;
    padding: 1.25rem;
    text-align: center;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    border-top: 4px solid transparent;
}

.card-list li:nth-child(odd) {
    border-top-color: #3498DB;
}

.card-list li:nth-child(even) {
    border-top-color: #E67E22;
}

.card-list li:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
}

/* =========================
   Reviews
   ========================= */
#reviews {
    background: #FFFFFF;
}

.reviews-grid {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-top: 1rem;
    padding: 0;
}

.reviews-grid>li {
    flex: 1 1 calc(33.333% - 1rem);
    /* 3 columns created by baseline value */
    min-width: 240px;
    background: #FFFFFF;
    border: 1px solid #DDDDDD;
    border-radius: 10px;
    padding: 1rem;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.reviews-grid>li:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
}

.reviews-grid .quote {
    border-left: 4px solid #3498DB;
    padding-left: 0.75rem;
    margin-bottom: 0.5rem;
    font-style: italic;
}

.reviews-grid cite {
    display: block;
    color: #666666;
    font-size: 0.9rem;
}

/* =========================
   CTA Band
   ========================= */
.cta-band {
    background: linear-gradient(135deg, #2C3E50 0%, #3b4d63 100%);
    color: #FFFFFF;
    text-align: center;
    padding: 4rem 1.5rem;
}

.cta-band h2,
.cta-band p {
    color: #FFFFFF;
}

/* =========================
   Footer
   ========================= */
.site-footer {
    background: #FFFFFF;
    border-top: 1px solid #DDDDDD;
    color: #666666;
    text-align: center;
    padding: 1.25rem 1rem;
    font-size: 0.9rem;
}

@media (max-width: 768px) {

    .feature-card,
    .card-list li,
    .reviews-grid li {
        flex: 0 0 100%;
        max-width: 100%;
    }

    .nav-inner {
        flex-direction: column;
    }
}
```
</details>