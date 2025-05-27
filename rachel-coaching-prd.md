# Product Requirements Document (PRD)
## Rachel Smith Intuitive Leadership Coaching Website

---

## **Project Overview**
**Client**: Rachel Smith - Transitioning from 25+ years corporate telemarketing/operations to intuitive leadership coaching  
**Product**: Static business website serving as digital business card/pamphlet  
**Timeline**: Single day build  
**Purpose**: Establish professional online presence for coaching business launch in 2025  
**Type**: Static site with Netlify form integration (no e-commerce/booking systems)  

---

## **Business Context**
Rachel is launching an intuitive leadership coaching business targeting mid-level to senior executives. She combines traditional leadership coaching with intuitive insights, drawing from her extensive corporate background and certified coaching credentials. Her unique approach balances professional credibility with transformational coaching methods.

**Key Business Details:**
- **Services**: 12-week coaching programs ($3,000-$7,500), B2B consulting, future membership community
- **Unique Value**: Combines corporate experience with intuitive coaching methodologies
- **Launch Goals**: TEDx talk September 2025, 5 paying clients year 1

---

## **Target Audience**
**Primary Avatar "Mandy"**: 
- Ages 35-55, married, college-educated
- Executive leaders, $80k-$250k income
- Seeking personal/professional development
- Values authentic leadership and growth
- Frustrated with current challenges, seeking new perspectives

**Secondary**: HR professionals, business owners, organizational leaders seeking team development

**User Journey**: Discovery → Credibility Assessment → Trust Building → Contact → Offline Conversion

---

## **File Structure**
```
rachel-coaching-website/
├── index.html                 # Homepage
├── about.html                 # About Rachel page
├── services.html              # Services overview/landing
├── executive-coaching.html    # B2C Services page
├── corporate-consulting.html  # B2B Services page
├── blog.html                  # Blog landing page
├── resources.html             # Resources placeholder page
├── contact.html               # Contact page
├── assets/
│   ├── css/
│   │   ├── main.css          # Main stylesheet
│   │   ├── animations.css    # Scroll animations
│   │   └── responsive.css    # Media queries
│   ├── js/
│   │   └── scroll-animations.js  # Minimal JS for animations (if needed)
│   └── images/
│       ├── hero-bg.jpg       # Homepage hero background
│       ├── rachel-portrait.jpg # Professional headshot
│       ├── about-photo.jpg   # About page photo
│       ├── services-b2c.jpg  # Executive coaching imagery
│       ├── services-b2b.jpg  # Corporate consulting imagery
│       ├── blog-thumbnails/
│       │   ├── blog-1.jpg    # VIEW from the Top thumbnail
│       │   ├── blog-2.jpg    # Journey story thumbnail
│       │   └── blog-3.jpg    # Corporate Empath thumbnail
│       └── icons/
│           ├── view-icon.svg # VIEW methodology icon
│           ├── rock-icon.svg # ROCK methodology icon
│           └── contact-icons/ # Social/contact icons
├── blog/
│   ├── view-from-the-top.html        # Blog post 1
│   ├── telemarketing-to-transformation.html # Blog post 2
│   └── corporate-empath.html         # Blog post 3
├── netlify.toml              # Netlify configuration
└── README.md                 # Project documentation
```

---

## **Technical Requirements**

### **Technology Stack**
- **Frontend**: HTML5, CSS3 only
- **JavaScript**: Minimal usage (scroll animations, form validation only if absolutely necessary)
- **Forms**: Netlify Forms integration
- **Hosting**: Static hosting compatible (Netlify recommended)
- **No Backend**: No server-side processing required

### **Performance Requirements**
- **Load Time**: <3 seconds on desktop, <5 seconds on mobile
- **Responsive**: Mobile-first design, works on all screen sizes
- **Browser Support**: Modern browsers (Chrome, Firefox, Safari, Edge)
- **Accessibility**: WCAG 2.1 AA compliance, `prefers-reduced-motion` support

### **Animation Requirements**
- **Scroll Animations**: Subtle fade-in/slide-in effects as user scrolls
- **Implementation**: CSS-only preferred, minimal JS if necessary
- **Performance**: Hardware accelerated, 60fps smooth
- **Elements**: Section reveals, image fades, text slide-ins
- **Style**: Professional, subtle, enhances rather than distracts

---

## **Design Requirements**

### **Visual Identity & Brand**
- **Design Philosophy**: "Professional Intuition" - balancing corporate credibility with intuitive warmth
- **Approach**: Yin and Yang balance between executive-level professionalism and transformational coaching

### **Color Palette**
- **Primary Purple**: #6B46C1 (intuition, wisdom)
- **Secondary Gray**: #6B7280 (professionalism)
- **Accent Gold**: #F59E0B (transformation, energy)
- **Neutrals**: #FFFFFF, #F9FAFB, #E5E7EB
- **Usage**: Purple accents, gray/white base, gold for CTAs and highlights

### **Typography**
- **Headers**: Modern serif font (professional authority)
- **Body Text**: Clean sans-serif (readability)
- **Hierarchy**: H1 (48px), H2 (36px), H3 (24px), Body (16px)

### **Imagery Style**
- **Type**: Professional stock photos sourced from internet
- **Mood**: Warm corporate settings, diverse professionals, coaching scenarios
- **Quality**: High-resolution, consistent lighting and style
- **People**: Authentic, diverse, executive-level professionals

---

## **Site Architecture & Navigation**

### **Primary Navigation**
```
Home | About | Services | Blog | Resources | Contact
```

### **Services Dropdown** (if space allows)
- Executive Coaching
- Corporate Consulting

---

## **Page-by-Page Requirements**

### **Homepage (index.html)**
**Purpose**: First impression, credibility, clear value proposition

**Sections**:
1. **Hero Section**
   - Headline: "Strategic Leadership Through Intuitive Insight" or similar
   - Subheadline: Brief value proposition
   - Professional photo of Rachel
   - Primary CTA: "Start Your Transformation"
   
2. **About Preview**
   - Brief background: 25+ years corporate experience
   - Transition to coaching story
   - Credentials highlight
   
3. **Services Overview**
   - Two-column layout: B2C Executive Coaching | B2B Corporate Consulting
   - Brief descriptions with links to dedicated pages
   
4. **Methodology Teaser**
   - Introduction to VIEW and ROCK methods
   - Visual icons or graphics
   
5. **Testimonials**
   - 3-4 placeholder testimonials (see content section)
   - Mix of individual and organizational clients
   
6. **Contact CTA**
   - Contact form or link to contact page
   - "Ready to transform your leadership?" messaging

### **About Rachel (about.html)**
**Purpose**: Build credibility, share authentic story, establish expertise

**Content Structure**:
1. **Professional Journey**
   - Started in telemarketing (part-time during college)
   - Worked up from agent to Director of Global Operations
   - 25+ years corporate leadership experience
   - Global team management (US, Europe, Brazil, Philippines, Jamaica)
   
2. **The Awakening**
   - Burnout period and 5-year break from telemarketing
   - Psychic consultation experience (turning point)
   - Discovery of intuitive abilities and empathic nature
   - Personal development journey
   
3. **Coaching Credentials**
   - Certified life coach since 2018
   - Professional development and leadership training
   - Corporate coaching experience within organizations
   
4. **Methodology Development**
   - Creation of VIEW method (Visualize, Incorporate, Empowerment, Walk Forward)
   - Development of ROCK approach (Recognize & Release, Open to NEW Perspective, Cultivate Confidence, Kickstart Purposeful Action)
   
5. **Personal Touch**
   - Identical twin sister
   - Family values (role model for children)
   - Commitment to authentic, judgment-free coaching

### **Services Overview (services.html)**
**Purpose**: Present both service offerings, guide to specific pages

**Content**:
- Introduction to Rachel's dual approach
- Executive Coaching (B2C) overview with link
- Corporate Consulting (B2B) overview with link
- Methodology explanation
- Contact information

### **Executive Coaching (executive-coaching.html)**
**Purpose**: Detail B2C individual coaching services

**Content Structure**:
1. **Target Audience**
   - Mid-level to senior executives
   - Leaders facing complex challenges
   - Professionals seeking new perspectives
   
2. **Program Structure**
   - 12-week coaching engagement
   - 60-minute sessions
   - Optional bi-monthly follow-ups
   
3. **VIEW Method Breakdown**
   - **V**isualize: Assessing current state and desired outcomes
   - **I**ncorporate Perspective: New ways of seeing challenges
   - **E**mpowerment: Building confidence and strategies
   - **W**alk Forward: Implementation with ongoing support
   
4. **Transformation Outcomes**
   - Increased clarity and confidence
   - Enhanced leadership effectiveness
   - Improved relationship dynamics
   - Strategic problem-solving abilities
   
5. **Contact Form** (Netlify)
   - Fields: Name, Email, Company, Current Challenge, Preferred Contact Method

### **Corporate Consulting (corporate-consulting.html)**
**Purpose**: Detail B2B organizational services

**Content Structure**:
1. **Organizational Focus**
   - Leadership development programs
   - Team dynamics improvement
   - Change management support
   - Executive coaching at scale
   
2. **ROCK Method for Organizations**
   - **R**ecognize & Release: Identifying organizational blocks
   - **O**pen to NEW Perspective: Shifting team mindsets
   - **C**ultivate Confidence: Building organizational resilience
   - **K**ickstart Purposeful Action: Implementation strategies
   
3. **Engagement Types**
   - Leadership workshops
   - Executive team coaching
   - Organizational assessments
   - Custom consulting projects
   
4. **Contact Form** (Netlify)
   - Fields: Name, Email, Company, Role, Team Size, Challenge Description

### **Blog Landing (blog.html)**
**Purpose**: Showcase thought leadership, drive newsletter signups

**Content**:
- Introduction to Rachel's insights and perspectives
- Featured blog posts (3 initial posts)
- Newsletter signup form
- Categories/tags for future organization

### **Blog Posts**

#### **1. "The VIEW from the Top: Why Executive Leaders Need a New Perspective" (blog/view-from-the-top.html)**
**Content Outline**:
- Leadership challenges in modern organizations
- The limitation of traditional problem-solving approaches
- Introduction to perspective-shifting techniques
- VIEW method overview
- Call-to-action for coaching consultation

#### **2. "From Telemarketing to Transformation: My Journey to Intuitive Leadership" (blog/telemarketing-to-transformation.html)**
**Content Outline**:
- Personal story: Starting as part-time telemarketer
- Corporate climb and leadership lessons learned
- Burnout and awakening experience
- Integration of intuitive abilities with business acumen
- How this unique background serves executive clients

#### **3. "The Corporate Empath: How Intuition Becomes Your Leadership Superpower" (blog/corporate-empath.html)**
**Content Outline**:
- Defining empathic leadership in corporate settings
- The business case for intuitive decision-making
- Practical applications of empathic leadership
- Overcoming skepticism about "intuitive" approaches
- Tools and techniques for developing intuitive leadership skills

### **Resources (resources.html)**
**Purpose**: Placeholder for future content library

**Content**:
- "Coming Soon" messaging
- Newsletter signup to be notified of new resources
- Preview of planned resources (worksheets, assessments, etc.)

### **Contact (contact.html)**
**Purpose**: Primary conversion page

**Content**:
1. **Contact Information**
   - Email: rachel@rachelsmithcoaching.com (placeholder)
   - Phone: (330) XXX-XXXX (placeholder)
   - Location: Youngstown, Ohio area
   
2. **Consultation Request Form** (Netlify)
   - Name, Email, Phone
   - Company/Organization
   - Role/Title
   - Service Interest (dropdown: Executive Coaching, Corporate Consulting, Speaking)
   - Current Challenge (textarea)
   - Preferred Contact Method
   - How did you hear about us?
   
3. **Next Steps**
   - What to expect after submitting form
   - Typical response timeframe
   - Initial consultation process

---

## **Content Requirements**

### **Placeholder Testimonials** (Mix throughout site)
1. **"Rachel's intuitive approach helped me see challenges from completely new angles. Her corporate background gave her instant credibility, but her coaching methods delivered transformation I didn't think was possible."** - *Sarah M., VP of Operations, Tech Company*

2. **"Working with Rachel was like having a strategic advisor and life coach rolled into one. She helped our leadership team move from conflict to collaboration in just a few months."** - *Michael R., CEO, Manufacturing Company*

3. **"I was skeptical about 'intuitive coaching' until I experienced Rachel's process. Her VIEW method is practical, actionable, and surprisingly powerful."** - *Jennifer L., Director of HR, Healthcare Organization*

4. **"Rachel doesn't just coach - she helps you discover perspectives you never knew existed. My confidence as a leader has grown exponentially."** - *David K., Senior Executive, Financial Services*

### **Case Study Placeholders**
1. **"From Conflict to Collaboration"** - How a C-suite team resolved interpersonal challenges and improved decision-making
2. **"The Stuck VP"** - Individual executive who broke through limiting beliefs to achieve promotion
3. **"Cultural Transformation"** - Organization that shifted from reactive to proactive leadership culture

---

## **Form Configuration (Netlify)**

### **Form Fields Specifications**
- **All forms require**: Name (required), Email (required), Message (required)
- **Contact page additional fields**: Phone, Company, Service Interest (dropdown), Challenge Description
- **Service page forms**: Customized based on B2C vs B2B focus
- **Newsletter signups**: Email only with optional name

### **Form Actions**
- **Success page**: Thank you message with next steps
- **Email notifications**: Send to Rachel's email address
- **Form storage**: Netlify dashboard for management

---

## **SEO Requirements**
- **Page Titles**: Unique, descriptive titles for each page
- **Meta Descriptions**: Compelling descriptions under 160 characters
- **Header Tags**: Proper H1, H2, H3 hierarchy
- **Alt Text**: Descriptive alt text for all images
- **Schema Markup**: Local business and professional service markup
- **Open Graph**: Social media sharing optimization

---

## **Responsive Design Breakpoints**
- **Mobile**: 320px - 768px
- **Tablet**: 768px - 1024px
- **Desktop**: 1024px+
- **Large Desktop**: 1440px+

---

## **Success Metrics & Goals**
- **Primary**: Contact form submissions
- **Secondary**: Time on site, page views, newsletter signups
- **Qualitative**: Professional appearance, trust building, credibility establishment

---

## **Future Enhancement Considerations**
- **Phase 2**: Payment integration (Stripe), online booking system
- **Phase 3**: Client portal, expanded resource library
- **Phase 4**: Blog CMS, automated email sequences
- **Scalability**: Easy to enhance without complete rebuild

---

## **Key Messaging Themes**
- **Credibility**: 25+ years corporate leadership experience
- **Uniqueness**: Intuitive approach combined with practical business acumen
- **Results**: Transformation through new perspectives
- **Authenticity**: Real person with genuine story and proven methods
- **Professionalism**: Executive-level service delivery

---

## **Call-to-Action Strategy**
- **Primary CTA**: "Start Your Transformation" / "Schedule Consultation"
- **Secondary**: Newsletter signup, resource downloads
- **Placement**: Homepage hero, end of each page, within blog posts
- **Design**: Consistent styling using accent gold color

---

**This PRD provides complete specifications for building Rachel Smith's intuitive leadership coaching website. The site should balance professional credibility with transformational coaching elements, creating trust while showcasing her unique value proposition.**
