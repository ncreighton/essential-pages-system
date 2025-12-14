# Essential Pages System

Complete templates for all required site pages: 404, About, Contact, Privacy Policy, Terms, and site-specific special pages.

---

## Page Inventory Per Site

### Required Pages (All Sites)
| Page | URL | Purpose |
|------|-----|---------|
| 404 Error | /404 | Custom error page |
| About | /about | Site/author story |
| Contact | /contact | Contact form |
| Privacy Policy | /privacy-policy | GDPR/CCPA compliance |
| Terms of Service | /terms | Legal terms |
| Affiliate Disclosure | /affiliate-disclosure | FTC compliance |
| Cookie Policy | /cookie-policy | EU compliance |

### Site-Specific Pages

#### AI Sites (wealthfromai, aidiscoverydigest, aiinactionhub, clearainews)
- /ai-tools - AI tools directory
- /resources - Curated resources
- /start-here - Beginner's guide
- /newsletter - Newsletter archive

#### Review Sites (pulsegear, wearable, smarthome)
- /best-of - Category best-of landing pages
- /deals - Current deals/sales
- /comparison - Product comparisons
- /how-we-test - Testing methodology
- /buyers-guide - Category buyer guides

---

## 404 Page Templates

### Structure
```html
<section class="error-404">
  <div class="error-container">
    <div class="error-visual">
      <!-- Site-specific illustration/animation -->
    </div>
    <div class="error-content">
      <h1 class="error-code">404</h1>
      <h2 class="error-title">[SITE-SPECIFIC-HEADLINE]</h2>
      <p class="error-message">[SITE-SPECIFIC-MESSAGE]</p>
      <div class="error-actions">
        <a href="/" class="btn-primary">Back to Home</a>
        <a href="/search" class="btn-secondary">Search Site</a>
      </div>
      <div class="error-suggestions">
        <h3>Popular Articles</h3>
        <!-- Dynamic recent/popular posts -->
      </div>
    </div>
  </div>
</section>
```

### Site-Specific 404 Content

#### wealthfromai.com
```
Headline: "This Investment Didn't Pay Off"
Message: "The page you're looking for has moved or doesn't exist. Let's get you back on track to building AI-powered wealth."
Visual: Animated downward chart that bounces back up
CTA: "Explore AI Strategies"
```

#### aidiscoverydigest.com
```
Headline: "Discovery Not Found"
Message: "This page seems to have slipped through our curation. Let's find something amazing for you instead."
Visual: Magnifying glass searching animation
CTA: "Browse Latest Discoveries"
```

#### aiinactionhub.com
```
Headline: "Action Interrupted"
Message: "This page isn't responding. But don't worry—there's plenty more AI in action to explore."
Visual: Glitchy terminal effect with recovery animation
CTA: "See AI in Action"
```

#### clearainews.com
```
Headline: "Story Not Found"
Message: "This article may have been moved or removed. Check our latest coverage instead."
Visual: Newspaper pages fluttering away
CTA: "Read Latest News"
```

#### pulsegearreviews.com
```
Headline: "Workout Interrupted"
Message: "This page took an unscheduled rest day. Let's get you back to finding the perfect gear."
Visual: Heart rate flatline that restarts
CTA: "Browse Fitness Tech"
```

#### wearablegearreviews.com
```
Headline: "Connection Lost"
Message: "We couldn't sync with this page. Let's reconnect you with our latest reviews."
Visual: Smartwatch searching for signal animation
CTA: "Find Your Wearable"
```

#### smarthomegearreviews.com
```
Headline: "Device Not Responding"
Message: "This page seems to be offline. Let's get your smart home search back on track."
Visual: Smart bulb flickering then turning on
CTA: "Explore Smart Home"
```

---

## About Page Templates

### Structure
```html
<section class="about-hero">
  <div class="hero-content">
    <h1>[SITE-NAME] Story</h1>
    <p class="hero-subtitle">[MISSION-STATEMENT]</p>
  </div>
</section>

<section class="about-mission">
  <h2>Our Mission</h2>
  <p>[DETAILED-MISSION]</p>
</section>

<section class="about-founder" itemscope itemtype="https://schema.org/Person">
  <div class="founder-image">
    <img src="nick-photo.jpg" alt="Nick Creighton" itemprop="image">
  </div>
  <div class="founder-bio">
    <h2>Meet the Founder</h2>
    <h3 itemprop="name">Nick Creighton</h3>
    <p itemprop="description">[FOUNDER-BIO-TAILORED-TO-SITE]</p>
  </div>
</section>

<section class="about-values">
  <h2>What We Stand For</h2>
  <div class="values-grid">
    <!-- 3-4 core values -->
  </div>
</section>

<section class="about-cta">
  <h2>Join Our Community</h2>
  <p>[CTA-MESSAGE]</p>
  <!-- Newsletter signup -->
</section>
```

### Site-Specific About Content

#### wealthfromai.com
```
Mission: "Democratizing AI-powered wealth building strategies for everyday investors."

Values:
1. Transparency - We show our reasoning, not just conclusions
2. Education First - Understanding beats following blindly
3. Ethical AI Use - Technology should enhance, not replace judgment
4. Accessibility - Premium insights for everyone

Founder Angle: Focus on Nick's journey discovering AI tools for financial analysis, 
his passion for making sophisticated strategies accessible.
```

#### pulsegearreviews.com
```
Mission: "Helping athletes and fitness enthusiasts find gear that actually performs."

Values:
1. Real-World Testing - We test during actual workouts
2. Honesty - Even when manufacturers won't like it
3. Data-Driven - Numbers don't lie
4. Athlete-First - Reviews by athletes, for athletes

Founder Angle: Nick as an active fitness enthusiast who got frustrated with biased
reviews and decided to create truly independent testing.
```

---

## Contact Page Templates

### Structure
```html
<section class="contact-page">
  <div class="contact-intro">
    <h1>Get in Touch</h1>
    <p>[CONTACT-MESSAGE]</p>
  </div>
  
  <div class="contact-grid">
    <div class="contact-form-wrapper">
      <form class="contact-form" action="/api/contact" method="POST">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
          <label for="subject">Subject</label>
          <select id="subject" name="subject">
            <option value="general">General Inquiry</option>
            <option value="partnership">Partnership Opportunity</option>
            <option value="press">Press/Media</option>
            <option value="correction">Article Correction</option>
            <option value="feedback">Feedback</option>
          </select>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="5" required></textarea>
        </div>
        <button type="submit" class="btn-submit">Send Message</button>
      </form>
    </div>
    
    <div class="contact-info">
      <div class="info-card">
        <h3>Response Time</h3>
        <p>We typically respond within 24-48 hours.</p>
      </div>
      <div class="info-card">
        <h3>Partnerships</h3>
        <p>For business inquiries, please include your company name and proposal.</p>
      </div>
      <div class="info-card">
        <h3>Press</h3>
        <p>Media inquiries welcome. Please include your outlet and deadline.</p>
      </div>
    </div>
  </div>
</section>
```

---

## Legal Pages

### Privacy Policy Template
- GDPR compliant
- CCPA compliant
- Includes: Data collection, cookies, third parties, user rights
- Auto-generates based on site name and contact info

### Terms of Service Template
- Covers: Usage terms, disclaimers, limitations
- Affiliate disclosure integration
- Copyright/IP protection

### Affiliate Disclosure (Review Sites)
```html
<section class="affiliate-disclosure-page">
  <h1>Affiliate Disclosure</h1>
  
  <div class="disclosure-content">
    <p><strong>[SITE-NAME]</strong> is a participant in various affiliate marketing 
    programs, including the Amazon Services LLC Associates Program.</p>
    
    <h2>What This Means</h2>
    <p>When you click on product links and make a purchase, we may earn a small 
    commission at no extra cost to you. This helps us keep creating honest, 
    in-depth reviews.</p>
    
    <h2>Our Promise</h2>
    <ul>
      <li>We never let affiliate relationships influence our ratings</li>
      <li>We buy most products ourselves for unbiased testing</li>
      <li>Negative reviews don't get softened for affiliate partners</li>
      <li>We clearly mark affiliate links throughout the site</li>
    </ul>
    
    <h2>Amazon Associates Disclosure</h2>
    <p>[SITE-NAME] is a participant in the Amazon Services LLC Associates Program, 
    an affiliate advertising program designed to provide a means for sites to earn 
    advertising fees by advertising and linking to Amazon.com.</p>
    
    <p>Amazon and the Amazon logo are trademarks of Amazon.com, Inc. or its affiliates.</p>
  </div>
</section>
```

---

## Review Site Special Pages

### How We Test Page
```html
<section class="methodology-page">
  <h1>How We Test</h1>
  
  <div class="methodology-intro">
    <p>At [SITE-NAME], we believe in rigorous, real-world testing. Here's exactly 
    how we evaluate every product we review.</p>
  </div>
  
  <div class="methodology-steps">
    <div class="step">
      <span class="step-number">01</span>
      <h3>Acquisition</h3>
      <p>We purchase products at retail price whenever possible. When manufacturers 
      provide review units, we disclose this clearly.</p>
    </div>
    
    <div class="step">
      <span class="step-number">02</span>
      <h3>Controlled Testing</h3>
      <p>Each product category has standardized tests. [SITE-SPECIFIC-TESTS]</p>
    </div>
    
    <div class="step">
      <span class="step-number">03</span>
      <h3>Real-World Use</h3>
      <p>Beyond benchmarks, we use products in daily life for [TIMEFRAME].</p>
    </div>
    
    <div class="step">
      <span class="step-number">04</span>
      <h3>Scoring</h3>
      <p>Our rating system weighs: [CRITERIA-LIST-WITH-WEIGHTS]</p>
    </div>
  </div>
  
  <div class="methodology-equipment">
    <h2>Our Testing Equipment</h2>
    <!-- List reference devices used for comparison -->
  </div>
</section>
```

### Site-Specific Test Methods

#### pulsegearreviews.com
```
Tests: GPS accuracy vs reference device, heart rate vs chest strap, 
battery drain under various conditions, water resistance verification,
comfort during extended workouts, app responsiveness
```

#### wearablegearreviews.com
```
Tests: Optical heart rate vs medical-grade ECG, SpO2 vs pulse oximeter,
sleep staging vs polysomnography studies, step counting accuracy,
skin comfort assessment, display visibility in sunlight
```

#### smarthomegearreviews.com
```
Tests: Setup time measurement, voice command response rate,
cross-platform compatibility verification, latency testing,
reliability over 30-day period, security audit
```

---

## CSS Base for Essential Pages

```css
/* 404 Page */
.error-404 {
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: var(--space-8);
}

.error-container {
  max-width: 800px;
  text-align: center;
}

.error-code {
  font-size: clamp(6rem, 15vw, 12rem);
  font-weight: 800;
  line-height: 1;
  background: var(--gradient-primary);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.error-title {
  font-size: var(--text-3xl);
  margin-bottom: var(--space-4);
}

.error-actions {
  display: flex;
  gap: var(--space-4);
  justify-content: center;
  margin-top: var(--space-6);
}

/* About Page */
.about-hero {
  padding: var(--space-16) var(--space-4);
  text-align: center;
  background: var(--color-surface);
}

.about-founder {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: var(--space-8);
  padding: var(--space-12) var(--space-4);
  max-width: var(--container-lg);
  margin: 0 auto;
}

.founder-image img {
  border-radius: var(--radius-lg);
  width: 100%;
  aspect-ratio: 1;
  object-fit: cover;
}

.values-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: var(--space-6);
}

/* Contact Page */
.contact-grid {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: var(--space-8);
  max-width: var(--container-lg);
  margin: 0 auto;
  padding: var(--space-8);
}

.contact-form .form-group {
  margin-bottom: var(--space-4);
}

.contact-form label {
  display: block;
  margin-bottom: var(--space-2);
  font-weight: 500;
}

.contact-form input,
.contact-form select,
.contact-form textarea {
  width: 100%;
  padding: var(--space-3);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-md);
  font-size: var(--text-base);
}

/* Legal Pages */
.legal-page {
  max-width: var(--container-md);
  margin: 0 auto;
  padding: var(--space-8);
}

.legal-page h1 {
  margin-bottom: var(--space-6);
}

.legal-page h2 {
  margin-top: var(--space-8);
  margin-bottom: var(--space-4);
}

.legal-page p,
.legal-page li {
  margin-bottom: var(--space-3);
  line-height: 1.7;
}

/* Responsive */
@media (max-width: 768px) {
  .about-founder {
    grid-template-columns: 1fr;
    text-align: center;
  }
  
  .contact-grid {
    grid-template-columns: 1fr;
  }
}
```

---

## Files Reference

```
essential-pages-system/
├── SKILL.md (this file)
├── templates/
│   ├── 404/
│   │   ├── 404-base.html
│   │   ├── 404-wealthfromai.html
│   │   └── ... (all sites)
│   ├── about/
│   │   ├── about-base.html
│   │   └── about-content-[site].md
│   ├── contact/
│   │   └── contact-base.html
│   └── legal/
│       ├── privacy-policy.html
│       ├── terms-of-service.html
│       └── affiliate-disclosure.html
├── css/
│   └── essential-pages.css
├── js/
│   └── contact-form.js
└── review-site-pages/
    ├── how-we-test.html
    ├── deals.html
    └── buyers-guide.html
```
