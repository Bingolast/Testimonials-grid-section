# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- Overall it was a fun challenge and probably easist way to learn
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![image](https://github.com/Bingolast/Testimonials-grid-section/blob/main/testimonials-grid-section-main/Testimonials.jpg?raw=true)
### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process
Still in the process of making it responsive
### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned
The first and very important thing to learn for me in this challenge was to be able to use CSS Grid and Flexbox more effciently. How to tackle 

To see how you can add code snippets, see below:

```html
<div class="testimonial">
        <div class="card card-bg-purple">
            <header class="card-header">
                <img src="/images/image-daniel.jpg" alt="" class="card-img">
                <div>
                    <h3>Daniel Clifford</h3>
                    <p>Verified Graduate</p>
                </div>
            </header>
            <p class="card__lead">
                I received a job offer mid-course, and the subjects I learned were current, if not more so,
                in the company I joined. I honestly feel I got every penny’s worth.
            </p>
            <p class="card__quote">
                “ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a
                transition and have heard some people who had an amazing experience here. I signed up
                for the free intro course and found it incredibly fun! I enrolled shortly thereafter.
                The next 12 weeks was the best - and most grueling - time of my life. Since completing
                the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”
            </p>
        </div>
        <div class="card card-bg-grey">
            <header class="card-header">
                <img src="/images/image-jonathan.jpg" alt="" class="card-img">
                <div>
                    <h3>Jonathan Walters</h3>
                    <p>Verified Graduate</p>
                </div>
            </header>
            <p class="card__lead">
                The team was very supportive and kept me motivated
            </p>
            <p class="card__quote">
                “ I started as a total newbie with virtually no coding skills. I now work as a mobile engineer
                for a big company. This was one of the best investments I’ve made in myself. ” </p>
        </div>
        <div class="card card-bg-white">
            <header class="card-header">
                <img src="/images/image-kira.jpg" alt="" class="card-img">
                <div class="text-white">
                    <h3>Kira Whittle</h3>
                    <p>Verified Graduate</p>
                </div>
            </header>
            <p class="card__lead">
                An overall wonderful and rewarding experience
            </p>
            <p class="card__quote"> “ Before joining the bootcamp, I’ve never written a line of code. I needed some
                structure from
                professionals who can help me learn programming step by step. I was encouraged to enroll by a former
                student of theirs who can only say wonderful things about the program. The entire curriculum and staff
                did not disappoint. They were very hands-on and I never had to wait long for assistance. The agile team
                project, in particular, was outstanding. It took my learning to the next level in a way that no tutorial
                could ever have. In fact, I’ve often referred to it during interviews as an example of my developent
                experience. It certainly helped me land a job as a full-stack developer after receiving multiple offers.
                100% recommend! ”
            </p>
        </div>
        <div class="card card-bg-black">
            <header class="card-header">
                <img src="/images/image-patrick.jpg" alt="" class="card-img">
                <div>
                    <h3>Patrick Abrams</h3>
                    <p>Verified Graduate</p>
                </div>
            </header>
            <p class="card__lead">
                Awesome teaching support from TAs who did the bootcamp themselves. Getting guidance from them and
                learning from their experiences was easy.
            </p>
            <p class="card__quote">“ The staff seem genuinely concerned about my progress which I find really
                refreshing. The program
                gave me the confidence necessary to be able to go out in the world and present myself as a capable
                junior developer. The standard is above the rest. You will get the personal attention you need from
                an incredible community of smart and amazing people.”</p>

        </div>
        <div class="card card-bg-white">
            <header class="card-header">
                <img src="/images/image-jeanette.jpg" alt="" class="card-img">
                <div class="text-white">
                    <h3>Jeanette Harmon</h3>
                    <p>Verified Graduate</p>
                </div>
            </header>
            <p class="card__lead">
                Such a life-changing experience. Highly recommended!
            </p>
            <p class="card__quote">
                “ Thank you for the wonderful experience! I now have a job I really enjoy, and make a good living
                while doing something I love. ”
            </p>
        </div>
    </div>
    <div class="attribution">
        Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
        Coded by <a href="#">Parth Tiwari</a>.
    </div>
```
```css
.testimonial {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 30px;
  max-width: 1440px;
  margin: 100px auto;
  padding: 20px;
}

.card {
  background: #fff;
  border-radius: 10px;
  padding: 30px;
  box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
  margin-bottom: 10px;
}

.card-header {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.card-header h3 {
  font-size: 15px;
}

.card-header p {
  opacity: 50%;
}

.card-img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  border: 2px solid rgb(153, 110, 217);
  margin-right: 10px;
}

.card__lead {
  font-size: 1.5rem;
  font-weight: 500;
  line-height: 1.3;
  margin-bottom: 20px;
}

.card__quote {
  font-size: 15px;
  font-weight: 500;
  line-height: 1.4;
  opacity: 70%;
  margin-bottom: 20px;
}

.card-bg-purple {
  background: hsl(263, 55%, 52%);
  color: #fff;
  background-image: url(/images/bg-pattern-quotation.svg);
  background-repeat: no-repeat;
  background-position: top 10px right 100px;
}

.card-bg-grey {
  background: hsl(217, 19%, 35%);
  color: #fff;
}

.card-bg-black {
  background: hsl(219, 29%, 14%);
  color: #fff;
}

.card:nth-of-type(1) {
  grid-column: 1/3;
}

.card:nth-of-type(3) {
  grid-column: 4/5;
  grid-row: 1/3;
}

.card:nth-of-type(4) {
  grid-row: 2/3;
  grid-column: 2/4;
}

/* footer */
.attribution {
  font-size: 2rem;
  text-align: center;
}
.attribution a {
  color: hsl(228, 45%, 44%);
}

```

### Continued development
The main and the very frist thing is I want to make this project responsive.
Also I will host this site.

## Author
- Frontend Mentor - [Bingoblast](https://www.frontendmentor.io/profile/Bingolast)
- Twitter - [@Tiwariparth6165](https://twitter.com/Tiwariparth6165)
